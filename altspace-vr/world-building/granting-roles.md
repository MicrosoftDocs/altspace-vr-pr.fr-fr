---
title: Attribution de rôles de monde
description: Découvrez le système de rôles et de capacités et obtenez des instructions pas à pas pour donner aux utilisateurs des rôles dans vos mondes AltspaceVR.
ms.date: 04/14/2021
ms.topic: article
keywords: roles
ms.openlocfilehash: 3a1d0f138b29fe545f52d851ff00062f156a860e
ms.sourcegitcommit: 2db596ab5a1ecd4901a8c893741cc4d06f6aecea
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2021
ms.locfileid: "112923190"
---
# <a name="granting-world-roles"></a>Attribution de rôles de monde

Altspace dispose d’un système de rôles et de capacités. Chaque personne peut avoir plusieurs rôles et leurs rôles peuvent être différents en fonction de leur emplacement. Chaque rôle, à son tour, vous offre une ou plusieurs capacités. Par exemple, lorsque vous êtes dans votre propre événement, vous recevez automatiquement les rôles d' **hôte** et de **modérateur** . Avec ces deux rôles, vous pouvez lancer des utilisateurs Unruly, être à la phase et peut-être publier les confetti.

1. Modifiez votre univers et reportez-vous à la colonne de droite pour connaître les **rôles contextuels** ([Comment gérer les mondes](managing-worlds.md))

![Modification des rôles dans la section des rôles contextuels de mondes](images/granting-roles.png)

2. Cliquez sur **Ajouter un utilisateur** sous le champ **rôles contextuels** si vous souhaitez accorder des rôles spécifiques à des utilisateurs spécifiques pour ce monde uniquement. Par exemple, si vous souhaitez me donner le   +  **modérateur** de l’hôte, vous devez ajouter le ci-dessus et sélectionner **Enregistrer**. Le format est **nom d’utilisateur**, le nom d’utilisateur ne respecte pas la casse, choisissez le rôle dans le menu déroulant **terraformer**, cliquez sur Ajouter un utilisateur plusieurs fois pour ajouter d’autres utilisateurs, puis cliquez sur **mettre à jour**.

* Pour que la modification soit prise en compte dans Altspace, vous devez réinitialiser l’espace, ce qui obligerait tout le monde à rejoindre ou à avoir chaque utilisateur avec un nouveau rôle rejoindre le monde.

3. Modifiez le champ **rôles contextuels par défaut** , sous la section **en VR** , si vous souhaitez accorder un rôle à chacun d’entre eux qui rejoint votre monde. Par exemple, si vous souhaitez permettre aux utilisateurs de voler et d’utiliser le mégaphone pour qu’ils puissent entendre l’un après l’autre, ajoutez les éléments suivants :

```
pilot,megaphone_only
```

Après avoir sélectionné **mettre à jour**, réinitialisez l’espace dans le monde. Cela n’affecte que ce monde. Si vous souhaitez accorder des rôles à un univers entier, modifiez les mêmes champs sur l’univers. Il en va de même pour les événements, si vous souhaitez que tous les membres de votre événement aient ces rôles, vous devez les ajouter aux **rôles Contexual par défaut** de l’événement lui-même.

## <a name="roles"></a>Rôles

* **Megaphone_only** -possibilité de parler des oreilles des utilisateurs où qu’ils se trouvent dans le monde
* **Modérateur** -les capacités telles que le **lancement** de decorum
* **Pilote** : possibilité de basculer en mode volant et de générer l’outil de vol 6DOF
* Les capacités de l' **hôte** , comme la possibilité d’être en phase, ont mégaphone
* **Terraformer** -possibilité d’utiliser l’éditeur du monde plus d’informations sur ([rôles dans les événements, mondes, groupes et dans AltspaceVR](../getting-started/roles.md))

## <a name="troubleshooting"></a>Dépannage

**Puis-je supprimer des rôles ?**
Oui, modifiez votre environnement, cliquez sur **supprimer** sous le rôle que vous souhaitez supprimer, puis cliquez sur **mettre à jour** .

**Les rôles sont-ils copiés lorsqu’un monde importe à partir d’un autre ?**
Non, les rôles ne sont pas copiés