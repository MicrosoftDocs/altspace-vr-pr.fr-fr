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
# <a name="granting-world-roles"></a><span data-ttu-id="c875b-104">Attribution de rôles de monde</span><span class="sxs-lookup"><span data-stu-id="c875b-104">Granting world roles</span></span>

<span data-ttu-id="c875b-105">Altspace dispose d’un système de rôles et de capacités.</span><span class="sxs-lookup"><span data-stu-id="c875b-105">Altspace has a Roles and Abilities system.</span></span> <span data-ttu-id="c875b-106">Chaque personne peut avoir plusieurs rôles et leurs rôles peuvent être différents en fonction de leur emplacement.</span><span class="sxs-lookup"><span data-stu-id="c875b-106">Each person can have multiple roles and their roles can be different depending on where they are.</span></span> <span data-ttu-id="c875b-107">Chaque rôle, à son tour, vous offre une ou plusieurs capacités.</span><span class="sxs-lookup"><span data-stu-id="c875b-107">Each role, in turn, gives you one or more abilities.</span></span> <span data-ttu-id="c875b-108">Par exemple, lorsque vous êtes dans votre propre événement, vous recevez automatiquement les rôles de **présentateur** et de **modérateur** .</span><span class="sxs-lookup"><span data-stu-id="c875b-108">For example, when you're in your own event, you automatically receive the **presenter** and **moderator** roles.</span></span> <span data-ttu-id="c875b-109">Avec ces deux rôles, vous pouvez lancer des utilisateurs Unruly, être à la phase et peut-être publier les confetti.</span><span class="sxs-lookup"><span data-stu-id="c875b-109">With those two roles you can kick unruly users, be on stage, and maybe release the confetti.</span></span> 

1. <span data-ttu-id="c875b-110">Modifiez votre monde et faites défiler jusqu’à la section **en VR** ([Comment gérer les mondes](managing-worlds.md))</span><span class="sxs-lookup"><span data-stu-id="c875b-110">Edit your World and scroll down to the **In VR** section ([How to manage Worlds](managing-worlds.md))</span></span>

![Modification des rôles dans la section VR des mondes](images/granting-roles.png)

2. <span data-ttu-id="c875b-112">Modifiez le champ **rôles** si vous souhaitez accorder des rôles spécifiques à des utilisateurs spécifiques uniquement pour ce monde.</span><span class="sxs-lookup"><span data-stu-id="c875b-112">Edit the **Roles** field if you want to grant specific roles to specific users just for this World.</span></span> <span data-ttu-id="c875b-113">Par exemple, si vous souhaitez obtenir le modérateur de **presenter**  +   et donner au **modérateur** de calen, vous devez ajouter ce qui suit et sélectionner **Enregistrer**.</span><span class="sxs-lookup"><span data-stu-id="c875b-113">For example, if you want to give me **presenter** + **moderator** and give Calen **moderator**, you would add the following and select **Save**.</span></span> <span data-ttu-id="c875b-114">Le format est **{role}, {username ou email}** sur chaque ligne.</span><span class="sxs-lookup"><span data-stu-id="c875b-114">The format is **{role},{username or email}** on each line.</span></span> <span data-ttu-id="c875b-115">Le nom d’utilisateur ne respecte pas la casse.</span><span class="sxs-lookup"><span data-stu-id="c875b-115">Username is case-insensitive.</span></span> 

```
presenter,jimmy
moderator,jimmy
moderator,calen
```

3. <span data-ttu-id="c875b-116">Si vous sélectionnez **modifier** à nouveau, vous devez voir les éléments suivants au-dessus du champ rôles.</span><span class="sxs-lookup"><span data-stu-id="c875b-116">If you select **Edit** again, you should see the following above the Roles field.</span></span> <span data-ttu-id="c875b-117">Il s’agit de la façon dont vous savez que la base de données a été mise à jour.</span><span class="sxs-lookup"><span data-stu-id="c875b-117">That's how you know updated in the database.</span></span>

```
Presenters: jimmy
Moderators: jimmy,calen
```

* <span data-ttu-id="c875b-118">Pour que la modification soit prise en compte dans Altspace, vous devez réinitialiser le monde, en forçant tout le monde à se reconnecter.</span><span class="sxs-lookup"><span data-stu-id="c875b-118">In order for the change to take effect in Altspace, you should reset the world, forcing everyone to rejoin.</span></span> <span data-ttu-id="c875b-119">Voici une liste complète des rôles ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="c875b-119">There's a full list of roles below.</span></span>

4. <span data-ttu-id="c875b-120">Modifiez le champ **rôles contextuels** si vous souhaitez accorder un rôle à chacun d’entre eux qui rejoint votre monde.</span><span class="sxs-lookup"><span data-stu-id="c875b-120">Edit the **Contextual Roles** field if you want to grant a role to every one that joins your World.</span></span> <span data-ttu-id="c875b-121">Par exemple, si vous souhaitez permettre aux utilisateurs de voler et d’utiliser le mégaphone pour qu’ils puissent entendre l’un après l’autre, ajoutez les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="c875b-121">For example, if you want to let people fly and use the megaphone so they can hear each other while far part, add the following:</span></span>

```
pilot,megaphone_only
```

<span data-ttu-id="c875b-122">Après avoir sélectionné **mettre à jour**, réinitialisez le monde.</span><span class="sxs-lookup"><span data-stu-id="c875b-122">After you select **Update**, reset the World.</span></span> <span data-ttu-id="c875b-123">Cela n’affecte que ce monde.</span><span class="sxs-lookup"><span data-stu-id="c875b-123">This will only affect this World.</span></span> <span data-ttu-id="c875b-124">Si vous souhaitez accorder des rôles à un univers entier, modifiez les mêmes champs sur l’univers.</span><span class="sxs-lookup"><span data-stu-id="c875b-124">If you want to grant roles to an entire Universe, edit the same fields on the Universe.</span></span> 

## <a name="roles"></a><span data-ttu-id="c875b-125">Rôles</span><span class="sxs-lookup"><span data-stu-id="c875b-125">Roles</span></span> 

* <span data-ttu-id="c875b-126">**Présentateur** : des capacités telles que la possibilité d’être à la phase</span><span class="sxs-lookup"><span data-stu-id="c875b-126">**Presenter** - abilities like being able to be on stage</span></span>
* <span data-ttu-id="c875b-127">**Modérateur** -les capacités telles que le **lancement** de decorum</span><span class="sxs-lookup"><span data-stu-id="c875b-127">**Moderator** - abilities like **kick** to maintain decorum</span></span>
* <span data-ttu-id="c875b-128">**Terraformer** -possibilité d’utiliser l’éditeur de monde</span><span class="sxs-lookup"><span data-stu-id="c875b-128">**Terraformer** - ability to use the World Editor</span></span>
* <span data-ttu-id="c875b-129">**Pilote** : possibilité de basculer en mode volant et de générer l’outil de vol 6DOF</span><span class="sxs-lookup"><span data-stu-id="c875b-129">**Pilot** - ability to toggle fly mode and spawn the 6DOF flight tool</span></span>
* <span data-ttu-id="c875b-130">**Megaphone_only** -possibilité de parler des oreilles des utilisateurs où qu’ils se trouvent dans le monde</span><span class="sxs-lookup"><span data-stu-id="c875b-130">**Megaphone_only** - ability to speak into users' ears wherever they are in the World</span></span>
* <span data-ttu-id="c875b-131">**Showcase_new_sdk** -possibilité de générer des applications SDK MRE</span><span class="sxs-lookup"><span data-stu-id="c875b-131">**Showcase_new_sdk** - ability to spawn MRE SDK apps</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="c875b-132">Résolution des problèmes</span><span class="sxs-lookup"><span data-stu-id="c875b-132">Troubleshooting</span></span>

<span data-ttu-id="c875b-133">**Puis-je supprimer des rôles ?**</span><span class="sxs-lookup"><span data-stu-id="c875b-133">**Can I delete roles?**</span></span>
<span data-ttu-id="c875b-134">À partir du formulaire, à ce stade, le fichier a Support request sur help.altvr.com et nous en prendre en charge pour vous</span><span class="sxs-lookup"><span data-stu-id="c875b-134">Not from the form right now so file a Support request at help.altvr.com and we'll take care of it for you</span></span>

<span data-ttu-id="c875b-135">**Les rôles sont-ils copiés lorsqu’un monde importe à partir d’un autre ?**</span><span class="sxs-lookup"><span data-stu-id="c875b-135">**Are roles copied when a World is importing from another?**</span></span>
<span data-ttu-id="c875b-136">Non, les rôles ne sont pas copiés</span><span class="sxs-lookup"><span data-stu-id="c875b-136">No, roles aren't copied</span></span>