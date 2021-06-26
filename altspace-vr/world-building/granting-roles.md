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
# <a name="granting-world-roles"></a><span data-ttu-id="ebfd4-104">Attribution de rôles de monde</span><span class="sxs-lookup"><span data-stu-id="ebfd4-104">Granting world roles</span></span>

<span data-ttu-id="ebfd4-105">Altspace dispose d’un système de rôles et de capacités.</span><span class="sxs-lookup"><span data-stu-id="ebfd4-105">Altspace has a Roles and Abilities system.</span></span> <span data-ttu-id="ebfd4-106">Chaque personne peut avoir plusieurs rôles et leurs rôles peuvent être différents en fonction de leur emplacement.</span><span class="sxs-lookup"><span data-stu-id="ebfd4-106">Each person can have multiple roles and their roles can be different depending on where they are.</span></span> <span data-ttu-id="ebfd4-107">Chaque rôle, à son tour, vous offre une ou plusieurs capacités.</span><span class="sxs-lookup"><span data-stu-id="ebfd4-107">Each role, in turn, gives you one or more abilities.</span></span> <span data-ttu-id="ebfd4-108">Par exemple, lorsque vous êtes dans votre propre événement, vous recevez automatiquement les rôles d' **hôte** et de **modérateur** .</span><span class="sxs-lookup"><span data-stu-id="ebfd4-108">For example, when you're in your own event, you automatically receive the **host** and **moderator** roles.</span></span> <span data-ttu-id="ebfd4-109">Avec ces deux rôles, vous pouvez lancer des utilisateurs Unruly, être à la phase et peut-être publier les confetti.</span><span class="sxs-lookup"><span data-stu-id="ebfd4-109">With those two roles you can kick unruly users, be on stage, and maybe release the confetti.</span></span>

1. <span data-ttu-id="ebfd4-110">Modifiez votre univers et reportez-vous à la colonne de droite pour connaître les **rôles contextuels** ([Comment gérer les mondes](managing-worlds.md))</span><span class="sxs-lookup"><span data-stu-id="ebfd4-110">Edit your World and look over to the right column for **Contextual Roles** ([How to manage Worlds](managing-worlds.md))</span></span>

![Modification des rôles dans la section des rôles contextuels de mondes](images/granting-roles.png)

2. <span data-ttu-id="ebfd4-112">Cliquez sur **Ajouter un utilisateur** sous le champ **rôles contextuels** si vous souhaitez accorder des rôles spécifiques à des utilisateurs spécifiques pour ce monde uniquement.</span><span class="sxs-lookup"><span data-stu-id="ebfd4-112">Click **Add User** under the **Contextual Roles** field if you want to grant specific roles to specific users just for this World.</span></span> <span data-ttu-id="ebfd4-113">Par exemple, si vous souhaitez me donner le   +  **modérateur** de l’hôte, vous devez ajouter le ci-dessus et sélectionner **Enregistrer**.</span><span class="sxs-lookup"><span data-stu-id="ebfd4-113">For example, if you want to give me **host** + **moderator**, you would add the above and select **Save**.</span></span> <span data-ttu-id="ebfd4-114">Le format est **nom d’utilisateur**, le nom d’utilisateur ne respecte pas la casse, choisissez le rôle dans le menu déroulant **terraformer**, cliquez sur Ajouter un utilisateur plusieurs fois pour ajouter d’autres utilisateurs, puis cliquez sur **mettre à jour**.</span><span class="sxs-lookup"><span data-stu-id="ebfd4-114">The format is **username**, username is case-insensitive, choose the role from the dropdown menu **Terraformer**, click Add User multiple times to keeping adding more users and then click **Update**.</span></span>

* <span data-ttu-id="ebfd4-115">Pour que la modification soit prise en compte dans Altspace, vous devez réinitialiser l’espace, ce qui obligerait tout le monde à rejoindre ou à avoir chaque utilisateur avec un nouveau rôle rejoindre le monde.</span><span class="sxs-lookup"><span data-stu-id="ebfd4-115">In order for the change to take effect in Altspace, you should Reset Space the world forcing everyone to rejoin or have each user with a new role rejoin the world.</span></span>

3. <span data-ttu-id="ebfd4-116">Modifiez le champ **rôles contextuels par défaut** , sous la section **en VR** , si vous souhaitez accorder un rôle à chacun d’entre eux qui rejoint votre monde.</span><span class="sxs-lookup"><span data-stu-id="ebfd4-116">Edit the **Default Contextual Roles** field, under the **In VR** section, if you want to grant a role to every one that joins your World.</span></span> <span data-ttu-id="ebfd4-117">Par exemple, si vous souhaitez permettre aux utilisateurs de voler et d’utiliser le mégaphone pour qu’ils puissent entendre l’un après l’autre, ajoutez les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="ebfd4-117">For example, if you want to let people fly and use the megaphone so they can hear each other while far part, add the following:</span></span>

```
pilot,megaphone_only
```

<span data-ttu-id="ebfd4-118">Après avoir sélectionné **mettre à jour**, réinitialisez l’espace dans le monde.</span><span class="sxs-lookup"><span data-stu-id="ebfd4-118">After you select **Update**, Reset Space in the World.</span></span> <span data-ttu-id="ebfd4-119">Cela n’affecte que ce monde.</span><span class="sxs-lookup"><span data-stu-id="ebfd4-119">This will only affect this World.</span></span> <span data-ttu-id="ebfd4-120">Si vous souhaitez accorder des rôles à un univers entier, modifiez les mêmes champs sur l’univers.</span><span class="sxs-lookup"><span data-stu-id="ebfd4-120">If you want to grant roles to an entire Universe, edit the same fields on the Universe.</span></span> <span data-ttu-id="ebfd4-121">Il en va de même pour les événements, si vous souhaitez que tous les membres de votre événement aient ces rôles, vous devez les ajouter aux **rôles Contexual par défaut** de l’événement lui-même.</span><span class="sxs-lookup"><span data-stu-id="ebfd4-121">The same goes for events, if you want everyone in your event to have these roles you'll need to add this to the **Default Contexual Roles** of the event itself.</span></span>

## <a name="roles"></a><span data-ttu-id="ebfd4-122">Rôles</span><span class="sxs-lookup"><span data-stu-id="ebfd4-122">Roles</span></span>

* <span data-ttu-id="ebfd4-123">**Megaphone_only** -possibilité de parler des oreilles des utilisateurs où qu’ils se trouvent dans le monde</span><span class="sxs-lookup"><span data-stu-id="ebfd4-123">**Megaphone_only** - ability to speak into users' ears wherever they are in the World</span></span>
* <span data-ttu-id="ebfd4-124">**Modérateur** -les capacités telles que le **lancement** de decorum</span><span class="sxs-lookup"><span data-stu-id="ebfd4-124">**Moderator** - abilities like **kick** to maintain decorum</span></span>
* <span data-ttu-id="ebfd4-125">**Pilote** : possibilité de basculer en mode volant et de générer l’outil de vol 6DOF</span><span class="sxs-lookup"><span data-stu-id="ebfd4-125">**Pilot** - ability to toggle fly mode and spawn the 6DOF flight tool</span></span>
* <span data-ttu-id="ebfd4-126">Les capacités de l' **hôte** , comme la possibilité d’être en phase, ont mégaphone</span><span class="sxs-lookup"><span data-stu-id="ebfd4-126">**Host** - abilities like being able to be on stage, have megaphone</span></span>
* <span data-ttu-id="ebfd4-127">**Terraformer** -possibilité d’utiliser l’éditeur du monde plus d’informations sur ([rôles dans les événements, mondes, groupes et dans AltspaceVR](../getting-started/roles.md))</span><span class="sxs-lookup"><span data-stu-id="ebfd4-127">**Terraformer** - ability to use the World Editor More information about ([Roles in events, worlds, groups, and in AltspaceVR](../getting-started/roles.md))</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="ebfd4-128">Dépannage</span><span class="sxs-lookup"><span data-stu-id="ebfd4-128">Troubleshooting</span></span>

<span data-ttu-id="ebfd4-129">**Puis-je supprimer des rôles ?**</span><span class="sxs-lookup"><span data-stu-id="ebfd4-129">**Can I delete roles?**</span></span>
<span data-ttu-id="ebfd4-130">Oui, modifiez votre environnement, cliquez sur **supprimer** sous le rôle que vous souhaitez supprimer, puis cliquez sur **mettre à jour** .</span><span class="sxs-lookup"><span data-stu-id="ebfd4-130">Yes, edit your world, click **Remove** below the role you'd like to delete and click **Update**</span></span>

<span data-ttu-id="ebfd4-131">**Les rôles sont-ils copiés lorsqu’un monde importe à partir d’un autre ?**</span><span class="sxs-lookup"><span data-stu-id="ebfd4-131">**Are roles copied when a World is importing from another?**</span></span>
<span data-ttu-id="ebfd4-132">Non, les rôles ne sont pas copiés</span><span class="sxs-lookup"><span data-stu-id="ebfd4-132">No, roles aren't copied</span></span>