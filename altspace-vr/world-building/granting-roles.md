---
title: Attribution de rôles de monde
description: Découvrez le système de rôles et de capacités et obtenez des instructions pas à pas pour donner aux utilisateurs des rôles dans vos mondes AltspaceVR.
ms.date: 03/11/2021
ms.topic: article
keywords: roles
ms.openlocfilehash: f8cd55fbd8ede6cedd199724a3e6b2413c5bc3e6
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/08/2021
ms.locfileid: "107212202"
---
# <a name="granting-world-roles"></a>Attribution de rôles de monde

Altspace dispose d’un système de rôles et de capacités. Chaque personne peut avoir plusieurs rôles et leurs rôles peuvent être différents en fonction de leur emplacement. Chaque rôle, à son tour, vous offre une ou plusieurs capacités. Par exemple, lorsque vous êtes dans votre propre événement, vous recevez automatiquement les rôles de **présentateur** et de **modérateur** . Avec ces deux rôles, vous pouvez lancer des utilisateurs Unruly, être à la phase et peut-être publier les confetti. 

1. Modifiez votre monde et faites défiler jusqu’à la section **en VR** ([Comment gérer les mondes](managing-worlds.md))

![Modification des rôles dans la section VR des mondes](images/granting-roles.png)

2. Modifiez le champ **rôles** si vous souhaitez accorder des rôles spécifiques à des utilisateurs spécifiques uniquement pour ce monde. Par exemple, si vous souhaitez obtenir le modérateur de **presenter**  +   et donner au **modérateur** de calen, vous devez ajouter ce qui suit et sélectionner **Enregistrer**. Le format est **{role}, {username ou email}** sur chaque ligne. Le nom d’utilisateur ne respecte pas la casse. 

```
presenter,jimmy
moderator,jimmy
moderator,calen
```

3. Si vous sélectionnez **modifier** à nouveau, vous devez voir les éléments suivants au-dessus du champ rôles. Il s’agit de la façon dont vous savez que la base de données a été mise à jour.

```
Presenters: jimmy
Moderators: jimmy,calen
```

* Pour que la modification soit prise en compte dans Altspace, vous devez réinitialiser le monde, en forçant tout le monde à se reconnecter. Voici une liste complète des rôles ci-dessous.

4. Modifiez le champ **rôles contextuels** si vous souhaitez accorder un rôle à chacun d’entre eux qui rejoint votre monde. Par exemple, si vous souhaitez permettre aux utilisateurs de voler et d’utiliser le mégaphone pour qu’ils puissent entendre l’un après l’autre, ajoutez les éléments suivants :

```
pilot,megaphone_only
```

Après avoir sélectionné **mettre à jour**, réinitialisez le monde. Cela n’affecte que ce monde. Si vous souhaitez accorder des rôles à un univers entier, modifiez les mêmes champs sur l’univers. 

## <a name="roles"></a>Rôles 

* **Présentateur** : des capacités telles que la possibilité d’être à la phase
* **Modérateur** -les capacités telles que le **lancement** de decorum
* **Terraformer** -possibilité d’utiliser l’éditeur de monde
* **Pilote** : possibilité de basculer en mode volant et de générer l’outil de vol 6DOF
* **Megaphone_only** -possibilité de parler des oreilles des utilisateurs où qu’ils se trouvent dans le monde
* **Showcase_new_sdk** -possibilité de générer des applications SDK MRE

## <a name="troubleshooting"></a>Résolution des problèmes

**Puis-je supprimer des rôles ?**
À partir du formulaire, à ce stade, le fichier a Support request sur help.altvr.com et nous en prendre en charge pour vous

**Les rôles sont-ils copiés lorsqu’un monde importe à partir d’un autre ?**
Non, les rôles ne sont pas copiés