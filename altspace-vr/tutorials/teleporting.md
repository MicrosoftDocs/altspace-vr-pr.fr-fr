---
title: Utilisation du téléportateur
description: Découvrez comment vous déplacer d’un événement ou d’un monde à un autre à l’aide d’un téléportateur dans AltspaceVR.
ms.date: 03/11/2021
ms.topic: article
keywords: téléporteur
ms.openlocfilehash: afc199e958824bb5f0a9ff6d74865cbcd3f16868
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/08/2021
ms.locfileid: "107212510"
---
# <a name="using-the-teleporter"></a>Utilisation du téléportateur

Le passage d’un événement ou d’un monde à un autre est un excellent moyen pour vous et la communauté d’explorer tout ce que AltspaceVR a à offrir.

## <a name="the-short-version"></a>Version abrégée

![Procédure de téléportage à partir du panneau de l’éditeur vers la définition d’une destination de téléporting](images/teleporter.png)

## <a name="the-slightly-longer-version"></a>Version légèrement plus longue

Tout d’abord, assurez-vous que vous êtes dans votre Homespace, dans un événement ou dans le monde que vous avez créé ou que vous avez donné le rôle terraformer dans. Si vous êtes en mode 2D et que vous ne voyez pas le bouton éditeur de monde dans le coin inférieur droit de votre interface utilisateur, cliquez avec le bouton droit sur le bouton de la souris pour activer/désactiver cette option. Si vous ne voyez toujours pas le bouton éditeur de monde, vous pouvez être dans l’espace de quelqu’un d’autre. Si c’est le cas, demandez à l’hôte de vous fournir le rôle terraformer.

Cela vous aidera également à : 
1. Créez d’abord les événements ou les mondes
2. Accédez à l’emplacement où vous souhaitez générer le téléportateur, afin que vos événements/mondes s’affichent dans le panneau de destination du téléportateur et vous permettent de les connecter plus rapidement et plus facilement.

Une autre astuce pour vous aider à naviguer avec les téléporteurs en mode 2D consiste à utiliser Ctrl + barre d’espace. L’invite de commandes s’affiche et vous pouvez taper : Back-This (arrière-plan) pour revenir au dernier espace dans lequel vous étiez. 

À présent, accédez à l’emplacement où vous souhaitez générer un téléportateur et sélectionnez dans le panneau éditeur/éditeur du monde/les éléments de base/téléportateur.

Le panneau de destination du téléporteur s’affiche. Vous pouvez choisir parmi trois catégories :

* **Mes espaces** : liste des mondes que vous avez créés.
* **Récent** -liste des événements récents que vous avez apportés. Utilisez cette option si vous souhaitez vous déplacer vers un événement. il s’agit de la seule option qui vous permet d’aller à un événement, l’autre 2 vous permet uniquement de vous déplacer entre des mondes. Remarque : Voir la section ci-dessous si vous connectez des événements de ligne avant qui ont importé des mondes, vous devez générer et configurer les téléporteurs dans le monde importé et non dans l’événement réel.
* Liste **proposée** des mondes proposés vous pouvez définir le téléportateur sur lequel se déplacer.

Sélectionnez l’événement ou le monde que vous souhaitez utiliser, ce qui génère le téléportateur et place une étiquette de texte de l’événement ou du nom de monde légèrement en arrière-plan. Vous pouvez donc sélectionner l’icône d’engrenage dans la section objets présents pour modifier le nom de l’étiquette.

Vous pouvez sélectionner l’option sur le téléporteur à l’aide de votre curseur (vous serez invité à indiquer s’il est possible de le faire, en cas de clic) ou de déplacer votre avatar directement dans le téléporteur et, Presto, vous êtes en déplacement vers votre destination. Dites-le Bonjour !

## <a name="advanced-features"></a>Fonctionnalités avancées

Si vous créez une conférence, un sommet ou un événement plus grand en utilisant une ligne de base avec un monde personnalisé (par exemple, un modèle de fondation, un modèle d’espace de téléchargeur Unity, Re-Import monde), vous devez configurer le téléportateur dans le monde de la Fondation et non pas dans l’événement réel. Assurez-vous que vous configurez le téléporteur pour vous déplacer vers le bon événement (qui doit figurer dans la liste récente) dans le monde de la Fondation, puis Re-Import monde dans l’éventualité de faire apparaître les téléporteurs dans tous les espaces d’événements de ligne avant.

## <a name="faqs"></a>Foire aux questions

**Erreur : «Désolé, nous aimerions, mais nous ne pouvons pas vous laisser ici**

Un groupe peut être associé à un groupe, de sorte que seuls les noms d’utilisateur du groupe peuvent accéder à cet événement de groupe privé.

**Combien de téléporteurs puis-je utiliser dans un espace ?**

Les téléporteurs utilisent des textures transparentes avec des effets de particules animés. il est donc préférable de ne pas en avoir trop dans le même emplacement/qui se chevauche, car cela peut affecter les performances. Essayez de ne pas avoir plus de 4 dans la même zone ou plus de 10 s’ils sont tous répartis dans votre espace.