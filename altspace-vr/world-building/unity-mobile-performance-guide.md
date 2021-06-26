---
title: Guide des performances mobile AltspaceVR
description: Découvrez comment utiliser diverses propriétés Unity pour rendre vos mondes performants sur des appareils mobiles comme Oculus Quest
ms.date: 04/20/2021
ms.topic: article
keywords: éditeur universel, performance, Oculus, Quest, Unity, textures, lightmaps, stats, profiler, appels de dessin, altspacevr, téléchargeur
ms.openlocfilehash: 9d6afba6fff85adfaa2ba290916f25c84c5377cd
ms.sourcegitcommit: 2db596ab5a1ecd4901a8c893741cc4d06f6aecea
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2021
ms.locfileid: "112961227"
---
# <a name="altspacevr-mobile-performance-guide"></a>Guide des performances mobile AltspaceVR

## <a name="main-points"></a>**Points principaux :**

* **72 fps** sur Oculus Quest 1 et 2 est la cible.
* Il est essentiel de **réduire les appels de dessin via le traitement par lot statique** , en vue de **moins de 25 drawcalls**
* **Un matériau par objet** pour encourager le traitement par lot statique (fractionner les objets MULTIMATÉRIAU en objets distincts).
* Dans la plupart des cas, les **objets** d’un environnement doivent avoir la valeur **« static »** .
* **Un lightmap par scène**, un 2 k ou 4 Ko pour l’ensemble de la scène, ~ 25 texels par unité, la mise à l’échelle lightmap doit être paramétrée par objet (mise à l’échelle du graphique ci-dessous)
* **Utilisez les nuanceurs de qualité Mobile** (c’est-à-dire « mobile/diffuse », etc.), évitez les sondes standard/de nuanceur/PBR/reflet standard Unity, car il s’agit d’opérations lourdes et, dans le cas des sondes, ajoutera des appels de dessin.
* **Moins de 100 000 triangles** à l’écran
* L' **élimination des occlusions** peut aider à réduire les polygones à l’écran, bien qu’il y ait un coût initial pour activer l’élimination des occlusions, ce qui mesure l’effet sur la cadence dans Altspace à l’aide du panneau Diagnostics.
* Pour toutes les **textures** dans une scène, utilisez **« override pour Android »** et affectez-leur le **format de bloc ASTC 6X6 compressé RVB (a)**.  Laissez la compression des paramètres de build Android à la valeur par défaut (trouvée dans : paramètres de fichier/Build/Android/compression de texture : 'ne pas remplacer'), afin que lightmaps n’obtient pas la compression ASTC.  En procédant de la façon décrite ci-dessus, et en partageant des documents entre les objets, nous essayons de conserver le package Unity de notre scène à environ **10-20 Mo pour Android**.

L’objectif général est d’atteindre une cadence acceptable entre les appareils : sur Oculus Quest 1 et 2, idéalement, la scène s’exécutera à 72 FPS à partir de tous les points de bourré lorsque la scène est remplie, bien qu’une plage de 60-72 FPS soit souvent plus réaliste.

La cadence peut être mesurée dans AltspaceVR sur l’appareil que vous utilisez (situé dans l’application AltspaceVR sous **Paramètres/support/afficher le panneau diagnostic/fps**).

Un récapitulatif des outils Unity standard disponibles pour vous aider à optimiser vos scènes :

## <a name="stats-panelframe-debuggerprofiler"></a>**Panneau des statistiques/débogueur de frame/profileur**

* Ces outils seront vos meilleurs amis pour améliorer les performances de votre scène.  Ils ne peuvent **être référencés que pendant la durée de la séquence de la scène dans l’éditeur**, car leurs valeurs sont différentes lorsque la scène n’est pas lue (autrement dit, le traitement par lots statique automatique ne se produit pas lorsque la scène n’est pas jouée)

* Le **panneau statistiques** (visible dans la vue de jeu sous stats) vous indique la quantité de **lots/lots enregistrés, les appels setpass et la fréquence** d’images.

    * Lots : nombre d’appels de dessin actuels visibles du point de vue actuel de l’appareil photo.  **Moins de 25 lots** pour un environnement sont une bonne cible à viser.
    * Lots enregistrés (visibles uniquement lorsque la scène est jouée) : nombre d’appels de dessin qui ont été réduits via le **traitement par lots statique ou l’instanciation GPU**
    * Les appels SetPass : nombre de matériaux visibles différents dans une scène
    * Cadence : nombre d’images par seconde dans la vue de jeu (vous donne une idée approximative de ce qui se passe ; les scènes doivent toujours être testées dans l’application, dans le casque, à l’aide du panneau Oculus, car la lecture FPS est toujours différente de celle de l’éditeur)

* **Débogueur de frame** (trouvé sous le débogueur Window/Analysis/Frame).  Le panneau statistiques sur steroids qui, lorsqu’il est activé, vous permet de voir ce que le GPU dessine pour créer l’image finale, en vous indiquant une liste de drawcalls du premier au dernier.  Il vous donnera des raisons pour lesquelles un appel de dessin n’a pas été traité par lot avec un appel de dessin précédent (autrement dit, « cet objet utilise un autre matériau » ou « cet objet utilise un lightmap différent ») et est un excellent moyen de développer une compréhension de ce qui se passe dans votre scène, et comment et pourquoi certains choix visuels peuvent être coûteux en calcul.

* Le **profileur** vous indique quelles parties de l’ordinateur sont utilisées à tout moment pendant l’exécution du jeu. Utile pour déterminer où les performances sont des goulots d’étranglement.  Par exemple, si vous constatez une utilisation intensive du processeur dans votre scène, il peut s’agir d’un trop grand nombre d’appels de dessin, ou si vous constatez une utilisation intensive du GPU, il se peut qu’il y ait trop de surdessin (c’est-à-dire le nombre de fois qu’un seul pixel est rendu pour produire l’image finale), ce qui peut être dû à l' , ou les objets ne sont pas supprimés lorsque vous êtes hors de l’affichage.

## <a name="draw-calls-shadersmaterialsobjects"></a>**Appels de dessin (nuanciers/matériaux/objets)**

* Chaque fois qu’un nuanceur, un matériau ou un objet doit être rendu, le processeur doit indiquer au GPU du commutateur (également appelé « appels de dessin », en commun **« drawcalls »**).  Autrement dit, si vous avez 5 nuanceurs, 10 matériaux et 20 objets, avec la valeur la plus grande ; vous aurez environ 20 drawcalls.  D’autres choses qui peuvent multiplier les drawcalls incluent l’utilisation d’objets sur des lightmaps différents ou la présence de plusieurs lumière en temps réel dans une scène (autrement dit, un point lumineux ajoute un autre drawcall à chaque objet qui se trouve dans sa plage). en général, tout ce qui n’est pas une lumière directionnelle d’une scène doit être évité.  Les sondes de réflexion et les sondes légères multiplient également les appels de dessin sur les objets qu’elles rencontrent, afin de pouvoir les éviter.

* Le **traitement par lots statique** regroupera des objets qui partagent des matériaux similaires dans un objet unique lorsqu’ils sont envoyés au GPU (avec l’élimination d’occlusion qui ignore les maillages). par conséquent, en affectant à tous les objets de l’exemple ci-dessus la valeur « static », vous réduisez la scène à environ 10 drawcalls, 1 pour chaque matière. 

* Les **lots de matériau** se produisent quand un objet a les matériaux exacts comme un autre objet. Toutefois, si un objet a plusieurs documents, il n’utilise pas de traitement par lots avec un objet qui a moins de documents.  Pour cette raison : les **objets ne doivent avoir qu’un seul matériau**, et les objets qui utilisent plusieurs matériaux doivent être fractionnés en objets distincts par matière.  Les **lots de matériau** peuvent être réduits par le biais d’une Atlas de **texture** (en combinant les textures de plusieurs objets uniques pour partager une même feuille de texture afin qu’elles utilisent toutes le même matériau).  Essayez de faire en sorte que la quantité d’Atlas soit réduite à une texture/un matériau de 2 Ko ou 4 Ko par scène, si possible.

## <a name="scene-complexity"></a>**Complexité de la scène**

* **Geometry** : essayez de conserver les triangles à l’écran pour les environnements inférieurs à 100 000.  Utilisez l’onglet « statistiques » dans le panneau de configuration de Unity pour voir quel est le nombre de triangles que vous atteignez à partir de différents points de bourré dans la scène.  Par exemple, les propriétés doivent se trouver dans la plage de « centaines » de facettes, avec uniquement des props « héros » importantes dans la plage de milliers d’angles. 

* Techniquement, vous pouvez utiliser **LODs** (niveau de maillage des détails), bien que la solution lightmap par défaut d’Unity ne partage pas de données lightmap entre LODs, vous pouvez donc recevoir des artefacts Lightmapping lorsque le commutateur LODs à cette résolution.  Vous pouvez également utiliser le composant de groupe LOD pour l’élimination des distances simples, même si l’objet n’a pas de maillage de niveau de vue réduit :

![Fenêtre de groupe LOD dans Unity](images/world-building-lod-Group.png)

* L' **élimination des occlusions** réduit le nombre d’objets qui sont rendus à ce qui se trouve dans le frustum View de la caméra, et qui sont immédiatement visibles (autrement dit, les objets qui sont des bloqués de la vue sont éliminés).  L’élimination des occlusions doit presque toujours être intégrée à votre scène, et les niveaux doivent être conçus pour le prendre en charge (autrement dit, si vous avez un grand niveau, les murs ou les grands objets peuvent être utilisés pour scinder la vision du joueur, afin qu’ils ne puissent pas toujours voir à l’extrémité opposée du niveau).  Les paramètres de cuisson par défaut doivent fonctionner, même si vous devrez peut-être réduire les valeurs les plus petites OCCLUDER ou les plus petites.  Pour les objets tels que les délimitations où vous pouvez voir des fissures dans l’objet ou des objets transparents, vous devez désactiver l’État « OCCLUDER » de l’objet dans le menu déroulant « statique » afin que les objets qui se trouvent sous-jacents ne soient pas bloqués par erreur. 

## <a name="lightmaps"></a>**Lightmaps**

* Idéalement, **une seule lightmap par scène** (1 Ko ou 1 Ko pour tout), si ce n’est pas le cas ; moins de lightmaps de résolutions plus élevées sont préférables à de nombreux lightmaps de résolutions inférieures.
* Le fait de disposer de plusieurs lightmaps peut également avoir une incidence sur le nombre d’appels de dessin, car les objets qui ont ou n’ont pas de lightmaps se trouvent sur des lots différents et d’autres lightmaps seront également sur des lots différents.
* En règle générale, une résolution lightmap d’environ **25 texels par unité** doit suffire (définir la résolution dans les paramètres d’éclairage/de scène).  Si vous disposez d’un espace supplémentaire dans votre lightmap, vous pouvez augmenter cette valeur.
* Modifiez le paramètre de **mise à l’échelle lightmap** par objet afin que la résolution soit enregistrée pour les objets qui en ont besoin. 

* **Graphique de mise à l’échelle lightmap** (règle de pouce) 
    * **Premier plan** (géo-niveau de parcours) : 1 
    * **Props** (surtout les props inférieures à celles d’un homme) : **2-3** (pour éviter les artefacts et les coutures lightmap sur vos objets) 
    * **Midground** (Geometry qui se trouve juste en dehors de la zone parcourue et/ou des objets volumineux tels que des bâtiments) : **0,5**
    * **Arrière-plan** (Vista/objets distants) : **0,02** 
    * **Surfaces transparentes** (telles que le verre) : **0** (avec les ombres « Cast/réception » désactivées) 

En outre, comme référence, voici quelques paramètres qui ont été utilisés pour l’environnement d’effet de la porte d’écran :

![Fenêtre d’éclairage dans Unity](images/world-building-lightmaps.png)

## <a name="texture-compressionfile-size"></a>**Compression de texture/taille de fichier**

* Pour notre Build Android, nous essayons de conserver la taille de la scène du package Unity à environ 10-20 Mo au total.  Nous faisons cela en partageant des matériaux génériques entre plusieurs objets, en utilisant la couleur du vertex pour teinter les objets, et en définissant des remplacements manuels pour Android afin que les textures utilisent la **compression de bloc ASTC 6X6**, qui sera inférieure à la compression par défaut.

* La raison pour laquelle nous ne définissons pas les paramètres de build Android pour utiliser ASTC est que les lightmaps ne sont pas corrects avec cette compression (un grand nombre d’artefacts bloquants) et que nous aurions dû définir le lightmap à utiliser, ETC., il est donc plus facile de configurer le remplacement de toutes les textures de scène une seule fois pour mettre à jour les paramètres de compression

![Fenêtre de texture dans Unity](images/world-building-texutres.png)

* En outre, la définition de textures pour utiliser le mode de filtre trilinéaire avec un niveau anisotrope peut les aider à rester nettes aux angles parcourant.

Vous trouverez d’autres conseils et astuces sur les performances dans la documentation sur l' [amélioration des performances mondiales](improving-performance.md).