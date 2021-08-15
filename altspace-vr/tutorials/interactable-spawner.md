---
title: Utilisation du Spawn Interactables
description: Découvrez comment créer, utiliser et personnaliser le Spawn interactables pour placer des éléments dans vos espaces AltspaceVR.
ms.date: 02/10/2021
ms.topic: article
keywords: Spawn, interactions, personnalisations
ms.openlocfilehash: abeddec5c2b50e0612db5efb6bc2e3c5bd9de4a8b67c50b19afee18b17c5e746
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/11/2021
ms.locfileid: "119127398"
---
# <a name="using-the-interactables-spawner"></a>Utilisation du Spawn Interactables

Le Spawn Interactables vous permet de placer des éléments interactifs dans votre événement, votre monde ou votre espace d’habitation. Cette fonctionnalité fait actuellement partie de notre [programme d’accès anticipé](../world-building/early-access.md) et n’est pas disponible, sauf si vous avez choisi le menu principal.

> [!NOTE]
> Pendant que nous continuons à piloter cette fonctionnalité, sachez que la génération d’un trop grand nombre de interactables peut affecter les performances de votre environnement ou de votre événement. 

## <a name="creating-an-interactable"></a>Création d’une

Pour transformer votre objet en objet exploitable :

1. Placez l’objet dans votre espace.
2. Ensuite, recherchez l’entrée dans la liste d’objets, puis sélectionnez l' **icône d’engrenage** en regard de celle-ci pour ouvrir ses paramètres :

![Éditeur de monde ouvert avec la liste d’objets mise en surbrillance](images/interactables-spawner-img-01.png)

Dans la page Paramètres, vous trouverez une nouvelle case à cocher **« génération d’objets »**, qui est utilisée pour en faire un objet pouvant être utilisé.

1. Cochez la case et sélectionnez **confirmer**.
2. En mode édition, vous pouvez vous déplacer autour de l’emplacement de génération de l’objet dans l’espace.
3. **Quittez le mode d’édition** pour activer l’interaction des éléments.

![Mettre à jour la fenêtre d’artefact ouverte dans l’application AltspaceVR](images/interactables-spawner-img-02.png)

## <a name="other-customizations"></a>Autres personnalisations

Une fois que vous avez activé la **« génération d’objets »** lorsque vous revenez dans les propriétés de cet objet, il y aura un paramètre supplémentaire que vous pouvez appliquer à la façon dont l’objet généré se comporte.

> [!NOTE]
> Mise à l’échelle des objets interactifs : définit l’échelle de l’objet lorsqu’il est sélectionné, par rapport à « Scale », qui est l’échelle de la façon dont l’objet apparaît dans le monde avant de le choisir pour la première fois.

Les décideurs peuvent remarquer que les modifications apportées à votre kit pendant l’exécution de AltspaceVR ne prennent pas effet tant que vous n’avez pas redémarré AltspaceVR.

récemment, nous avons ajouté un bouton sous l’onglet **modéré Paramètres** appelé **recharger les Kits**. Si vous cliquez sur ce bouton, (vous pouvez simplement) entrer à nouveau l’espace, recharger tous les kits, ce qui a pour effet de télécharger uniquement les nouvelles versions des kits qui ont été mis à jour pendant que vous étiez dans AltspaceVR.

![Panneau Paramètres modérés ouvert dans l’application AltspaceVR](images/interactables-spawner-img-03.png)