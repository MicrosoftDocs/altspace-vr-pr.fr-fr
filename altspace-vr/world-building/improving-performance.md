---
title: Amélioration des performances mondiales
description: Apprenez à mesurer, dépanner et améliorer les performances de vos mondes AltspaceVR à l’aide des outils de diagnostic.
ms.date: 03/11/2021
ms.topic: article
keywords: performances, résolution des problèmes
ms.openlocfilehash: 79d2bc43858c99652439aafa159c23f48eb3aa299c2b183936e40b1794fe444e
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/11/2021
ms.locfileid: "119126919"
---
# <a name="improving-world-performance"></a>Amélioration des performances mondiales

Nous souhaitons que les gens aient une bonne expérience en ce qui concerne les performances, ou la manière dont votre monde s’exécute sur des casques de VR, est très important. Notre système de construction mondiale est conçu pour des performances exceptionnelles pour les cas d’utilisation les plus courants. Si vous envisagez d’optimiser la présence, ce guide vous est destiné. Altspace aspire à prendre en charge toutes les plateformes matérielles. nous encourageons les intégrateurs de systèmes à pousser les limites, pour les mondes publics, nous vous recommandons de cibler le Oculus Quest et toute plateforme PC comme Windows Mixed Reality, le rift Oculus/le rift S ou HTC Vive. Pour simplifier, si votre monde s’exécute bien sur une quête, c’est probablement parfait pour Altspace.

## <a name="tools-and-measurement"></a>Outils et mesures

Diagnostics de l’administrateur est un outil hors connexion disponible sur notre site Web, altvr.com. Si vous accédez à [mondes > mes mondes](https://account.altvr.com/users/sign_in), recherchez votre monde et sélectionnez « Diagnostics », vous verrez ce qui suit :

![Fenêtre Diagnostics de l’administrateur](images/performance.png)

Il s’agit d’instructions supplémentaires par rapport aux exigences. Les performances dépendent du nombre d’objets dont vous disposez et de la façon dont ils sont organisés. Par exemple, si vous avez 500 objets répartis sur 2 kilomètres, les performances seront probablement correctes. Toutefois, si vous placez les mêmes 500 objets dans une zone fortement empaquetée, vous verrez probablement des problèmes. Cela est dû au fait que les performances dépendent de ce qui se trouve dans le champ d’affichage d’une personne. La meilleure façon de tester est de passer à Altspace et de vous téléfaire à travers le monde. Si vous constatez des problèmes ou des problèmes, il s’agit de problèmes que vous souhaitez examiner.

En respectant ces recommandations, vous vous configurez pour la réussite. Passons en revue cet exemple de diagnostic tiré d’un monde réel : 

* **Objets** -nombre total d’objets dans le monde. tout est un objet, Artifacts, Photos, générer des Points, etc. Nous vous recommandons de rester sous un certain nombre, mais cela est flexible. Si vous continuez, nous indiquons notre préoccupation avec un point d’exclamation jaune, comme illustré ici. Toutefois, dans ce cas, il existe deux zones distinctes dans ce monde, ce qui signifie que la densité n’est pas élevée.
* **Kits** : nombre total de kits de construction universels uniques utilisés. Cela a un impact sur le temps de téléchargement initial lors du chargement du monde. les Kits contiennent des Artifacts, le menu des objets que vous pouvez générer dans le monde entier. 

> [!NOTE] 
> Si un seul artefact est utilisé à partir d’un kit, les ressources de ce kit doivent être téléchargées. il est donc terriblement coûteux d’utiliser simplement quelques Artifacts à partir d’un seul Kit. 

* **Kits--mobile** : taille totale de toutes les ressources de kit qu’une personne sur une quête doit télécharger avant de pénétrer dans le monde. Essayez de ne pas faire patienter 5 minutes pour télécharger tout ce dont il a besoin pour votre monde.
* **Photos** : nombre Total de Photos utilisées, qui ont tendance à avoir un impact plus élevé sur les performances que Artifacts. Utilisez avec modération.
Modèle--mobile : Si vous utilisez le chargeur Unity, conservez une taille de téléchargement faible.
* **Skybox--mobile** : Si vous utilisez des skyboxes personnalisées, conservez une taille de fichier réduite afin que les utilisateurs n’obtiennent pas « écran noir » (mémoire vidéo insuffisante).
* **kits/Artifacts manquants/non valides** -références aux kits ou Artifacts problématiques... Vous avez une idée d’une mesure ? Faites-le nous savoir !
Une fois encore, il n’y a pas d’exigences pour les icônes d’état vert, jaune et rouge. Même un monde avec un ensemble d’indicateurs rouges peut toujours être proposé. Nous testons Altspace. [N’hésitez pas à nous contacter si vous avez besoin d’aide](getting-help.md). 

## <a name="load-time"></a>Temps de chargement

Lorsqu’une personne commence à se déplacer vers votre monde (tentatives d’entrée), elle commence par charger le modèle. Ils téléchargent les ressources de modèle (fichiers) pour leur plateforme et voient « environnement de chargement ». Ils téléchargent ensuite les ressources skybox et kit. Enfin, ils chargent tous les objets lorsqu’ils voient « chargement d’objets ». Le téléchargement de tous les éléments multimédias peut durer quelques minutes en fonction de la bande passante Internet : le chargement d’objets est relativement rapide. Tandis que les ressources sont téléchargées à partir de serveurs rapides partout dans le monde, Altspace utilise des techniques de mise en cache pour éviter de retélécharger les mêmes fichiers à plusieurs reprises. Techniquement, le temps de chargement initial n’affecte pas les performances d’une personne lorsqu’il entre dans le monde, mais elle fait partie de l’expérience globale, alors essayez de ne pas faire en sorte que les gens attendent trop longtemps quand ils se déplacent dans votre monde. Nous vous suggérons de réfléchir soigneusement aux kits à utiliser et à imaginatives en effectuant davantage de tâches avec moins.

## <a name="troubleshooting-and-tips"></a>Résolution des problèmes et conseils

**Les personnes voient un « écran noir »** En général, cela est dû au fait que l’appareil a manqué de mémoire vidéo. Essayez de réduire le nombre d’objets dans la zone problématique du monde et de réduire les tailles d’éléments tels que votre skybox ou modèle ou le nombre de Photos. Ces types ont tendance à avoir l’impact le plus élevé sur l’utilisation de la mémoire vidéo.

**Les personnes se bloquent**
    * Parfois, un kit ou un artefact cassé peut entraîner ce problème.
    * Les nuanceurs ou les animations bizarres peuvent être à l’origine de ce problème.
    * Regardez les choses dans les modèles et les kits personnalisés.
    * Sauvegardez votre monde souvent, en particulier lors du développement anticipé. Utilisez ces sauvegardes pour vous faire savoir ce que vous avez ajouté récemment, ce qui entraîne un blocage des personnes.

**Laissez « espace »**
    * N’oubliez pas que vous pouvez avoir 20-30 personnes dans le monde en même temps. Que se passe-vous si toutes ces personnes étaient huddled autour d’un Campfire. Voulez-vous toujours placer 200 Pebbles par le feu ? Ce n’est probablement pas une bonne idée. Laissez de l’espace pour les avatars et les Interactables (comme les basket-basket).
    * La concision est un atout.

**Planifier** à l’avance Réfléchissez à ce que vous souhaitez créer et à faire des choses. Il est facile de se familiariser avec Altspace.

**Utilisation précoce et fréquente de l’outil de diagnostic** Ajoutez un signet et actualisez-le une fois dans un moment. En réalité, il existera des outils similaires qui seront plus accessibles.

**Faire des amis avec les utilisateurs de Oculus Quest** Invitez-les à entrer dans votre monde pour vous aider à effectuer des tests. Testez minutieusement et souvent ! Testez les mondes de chaque autre. Rien ne fait des tests sur le réel.

**Ajoutez des amis comme « administrateurs » pour votre monde** Modifiez votre monde et ajoutez vos amis à la liste des administrateurs. Cela leur permet de voir l’outil de diagnostic pour votre monde. Soyez prudent, car ils peuvent également modifier d’autres aspects de votre monde. 

**L’optimisation des performances est difficile, donc notre communauté est impatiente d’aider** Participez à la [AltspaceVR officielle](https://discordapp.com/invite/altspacevr) * visitez le canal de construction #world pour obtenir une assistance générale sur les mondes.
    * Visitez les canaux du kit de développement logiciel (SDK) MRE pour obtenir une assistance spécifique avec une aide connexe plus technique et Unity (modèles et kits personnalisés)