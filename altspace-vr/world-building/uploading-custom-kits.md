---
title: Téléchargement de kits personnalisés
description: Découvrez comment configurer, générer et télécharger vos propres kits personnalisés dans AltspaceVR, ainsi que l’aide sur le dépannage.
ms.date: 03/11/2021
ms.topic: article
keywords: kits, téléchargement, résolution des problèmes
ms.openlocfilehash: 9a90bff2360d854dc398a35501f07cddcbce5c6c66ef8230f2e412a022f8aed0
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/11/2021
ms.locfileid: "119125524"
---
# <a name="uploading-custom-kits"></a>Téléchargement de kits personnalisés

l’éditeur World contient des Kits contenant Artifacts que vous pouvez générer dans votre monde. Par exemple, le [Kit Campfire](https://account.altvr.com/kits/993516233267609824) a de nombreux types d’arborescences : chaque type d’arborescence est un artefact. Pour créer votre propre kit, vous devez créer Unity AssetBundles et charger un fichier .zip contenant un Prefab Unity pour chaque artefact et inscrire chaque artefact sur notre site Web. Heureusement, le chargeur d’Unity piloté par la communauté automatise la majeure partie du flux de travail. Une fois chargé, vous pouvez générer des objets à partir de vos propres kits dans vos mondes, et les autres utilisateurs peuvent les voir automatiquement. plus tard, vous pourrez partager votre Kit avec vos amis, ou même avec l’intégralité de la Community, en étant en vedette.

## <a name="prerequisites"></a>Prérequis

1. [Installer Unity Hub et Unity](world-building-toolkit-getting-started.md)
2. Télécharger la dernière version du [chargeur Unity](https://altvr.com/download-latest-unity-uploader/)

## <a name="setup"></a>Installation 

> [!VIDEO https://channel9.msdn.com/Shows/Docs-Mixed-Reality/How-to-upload-my-own-Kits-Part-1-Setup/player]

1. Créer un kit sur notre site Web à l’adresse [mondes > kits](https://account.altvr.com/kits)
2. Copiez l’ID du kit à partir de la barre d’adresses de votre navigateur dans le presse-papiers (cette étape sera plus facile dans les versions de téléchargeur 0.9 +)
3. Créer une unité de Project Unity
4. Importez le chargeur Unity en double-cliquant sur le package

![Package du téléchargeur Unity importé](images/custom-kits-img-01.png)

5. Connectez-vous au téléchargeur avec votre adresse de messagerie et votre mot de passe Altspace

![Interface de connexion AltspaceVR dans Unity](images/custom-kits-img-02.png)

## <a name="generate-and-upload-your-kit"></a>Générer et charger votre kit

> [!VIDEO https://channel9.msdn.com/Shows/Docs-Mixed-Reality/How-to-upload-my-own-Kits-Part-2/player]

1. Renseignez le **nom du dossier du kit** avec votre ID de kit en tant que préfixe et un thème (par exemple, **1137484494681408069_pirates**), puis renseignez le **nom** du composant du kit avec votre ID de kit comme préfixe. Toutes les ressources devront avoir ce préfixe.

![Interface AltspaceVR dans Unity avec nom de dossier du kit](images/custom-kits-img-03.png)

2. Pour chaque artefact ou ensemble de Artifacts :
* Faites glisser vos Prefab sources dans l’onglet hiérarchie
* Sélectionnez ceux que vous souhaitez inclure dans un ensemble, par exemple cinq types de barils
* Mettre à jour le nom de la **ressource du kit** avec **Barrel**
* Sélectionnez **convertir gameobject (s) en kit Prefab**
* Vérifier que les nouveaux Prefabs et captures d’écran ont été créés dans le dossier ressources/Prefabs

![Interface AltspaceVR dans Unity avec les artefacts sélectionnés](images/custom-kits-img-04.png)

> [!NOTE]
> Si vous souhaitez apporter des modifications à un Prefab généré, refaites-le glisser dans la hiérarchie, apporter des modifications, puis cliquer sur **appliquer** sous l’onglet inspecteur pour mettre à jour Prefab. 

3. Quand vous êtes prêt, faites défiler l’onglet du téléchargeur et préparez-vous à générer un fichier zip avec le bundle de ressources
4. Pour accélérer l’itération, décochez le **Kit de build pour Android ?**. N’oubliez pas de créer et de télécharger une version pour Android plus tard lorsque vous avez terminé l’itération ou que vous souhaitez partager/faire figurer votre kit. 
5. Sélectionner les **répertoires Prefab du kit de chargement**
6. Choisissez **générer** en regard de celui correspondant au nom de votre dossier de kit. Il est courant de produire plusieurs kits à partir du même projet Unity. Cela peut prendre un certain temps en fonction de la taille de votre kit. Une fois l’opération terminée, le dossier contenant votre fichier zip s’ouvre automatiquement. 
7. Accédez au site Web, modifiez le kit que vous avez créé précédemment, puis chargez le fichier zip que vous avez créé. Ce chargement peut prendre un certain temps en fonction de la taille du fichier.
    * En cas de réussite, vous verrez sur le côté gauche sous « charge » la taille des fichiers et pour PC et Android, ainsi que la date de leur dernière mise à jour.
    * En cas d’échec, assurez-vous que vous n’avez aucun script, nous ne prenons pas en charge les scripts, nous vérifions ceux-ci pour la sécurité, puis réessayez.

Félicitations ! Vous êtes prêt à créer des mondes avec votre propre kit !

## <a name="troubleshooting"></a>Dépannage 

**Existe-t-il des limites ?**
Il n’existe pas encore de limite inconditionnelle, mais n’oubliez pas que les utilisateurs doivent télécharger le AssetBundle pour leur plateforme pour l’ensemble du Kit, même si un seul artefact est utilisé. Essayez de conserver le téléchargement par plateforme à 5 Mo ou moins. Pour ce faire, vous pouvez diviser les éléments en petits kits. Par exemple, 200 props doivent être divisées en deux. 

**Vous voyez « fractionner l’œil » ?**
Réimporter le téléchargeur le plus récent pour accéder aux bons paramètres de rendu

**Mises à jour/modifications non reflétées ?**
    * Vérifier l’heure mise à jour sur la page du kit
    * La réentrée du monde ne fonctionnera pas--redémarrez le client. Même si la mise à jour peut prendre quelques minutes
    * Assurez-vous qu’il n’y a pas d’espaces dans les noms de dossiers ou **de Prefab, par exemple, « party_favors » vs « tiers favorables »**

**Je n’ai pas de script, mais je n’ai pas** Le navigateur AssetBundle comprend automatiquement des fichiers. Essayez d’isoler le modèle que vous apportez. Par exemple, ne le faites pas glisser dans lorsqu’il fait partie d’un autre Prefab déjà

**Qu’en est-il des systèmes de particule et des animations ?**
Pour ceux-ci, ils sont ensuite sous un cube 1x1x1 positionné à l’origine avec le rendu du maillage et la collision désactivés. Les systèmes de particules doivent avoir une boucle activée et la **mise à l’échelle** doit être définie sur la **hiérarchie** afin que nous puissions les mettre à l’échelle correctement dans Altspace. Après avoir généré le prefabs pour toutes les animations, désactivez les collisions sur les objets de **collision** pour chaque.

**les Artifacts sont sombres** Avez-vous défini le nuanceur de matériau du modèle sur les **lumières directionnelles allumées en mode mobile/vertex uniquement**?

**L’artefact n’est pas face à la bonne voie** Faites pivoter le **modèle** et le **conflit** et mettez à jour le Prefab. La rotation du parent ne fait rien, ce qui est ignoré. Vous pouvez utiliser le champ de **remplacement de rotation** pour effectuer cette opération facilement.

**ces Artifacts peuvent-elles être utilisées avec la fonction **CreateFromLibrary** du kit de développement logiciel (SDK) ?**
Oui