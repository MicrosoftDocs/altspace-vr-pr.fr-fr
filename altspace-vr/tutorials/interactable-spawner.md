---
title: Utilisation du Spawn Interactables
description: Découvrez comment créer, utiliser et personnaliser le Spawn interactables pour placer des éléments dans vos espaces AltspaceVR.
ms.date: 02/10/2021
ms.topic: article
keywords: Spawn, interactions, personnalisations
ms.openlocfilehash: 7f4b87591b2e11b2084af4d2bf83748ed51fd193
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/08/2021
ms.locfileid: "107212575"
---
# <a name="using-the-interactables-spawner"></a><span data-ttu-id="20ea1-104">Utilisation du Spawn Interactables</span><span class="sxs-lookup"><span data-stu-id="20ea1-104">Using the Interactables Spawner</span></span>

<span data-ttu-id="20ea1-105">Le Spawn Interactables vous permet de placer des éléments interactifs dans votre événement, votre monde ou votre espace d’habitation.</span><span class="sxs-lookup"><span data-stu-id="20ea1-105">The Interactables Spawner allows you to place interactable items in your event, world, or home-space.</span></span> <span data-ttu-id="20ea1-106">Cette fonctionnalité fait actuellement partie de notre [programme d’accès anticipé](../world-building/early-access.md) et n’est pas disponible, sauf si vous avez choisi le menu principal.</span><span class="sxs-lookup"><span data-stu-id="20ea1-106">This feature is currently part of our [Early Access Program](../world-building/early-access.md) and won't be available unless you've opted in through your Main Menu.</span></span>

> [!NOTE]
> <span data-ttu-id="20ea1-107">Pendant que nous continuons à piloter cette fonctionnalité, sachez que la génération d’un trop grand nombre de interactables peut affecter les performances de votre environnement ou de votre événement.</span><span class="sxs-lookup"><span data-stu-id="20ea1-107">While we continue to pilot this feature please be aware that spawning too many interactables may affect the performance of your environment or event.</span></span> 

## <a name="creating-an-interactable"></a><span data-ttu-id="20ea1-108">Création d’une</span><span class="sxs-lookup"><span data-stu-id="20ea1-108">Creating an interactable</span></span>

<span data-ttu-id="20ea1-109">Pour transformer votre objet en objet exploitable :</span><span class="sxs-lookup"><span data-stu-id="20ea1-109">To turn your object into an interactable object:</span></span>

1. <span data-ttu-id="20ea1-110">Placez l’objet dans votre espace.</span><span class="sxs-lookup"><span data-stu-id="20ea1-110">Place the object in your space.</span></span>
2. <span data-ttu-id="20ea1-111">Ensuite, recherchez l’entrée dans la liste d’objets, puis sélectionnez l' **icône d’engrenage** en regard de celle-ci pour ouvrir ses paramètres :</span><span class="sxs-lookup"><span data-stu-id="20ea1-111">Then, find the entry in the object list, and select the **gear icon** next to it to open its settings:</span></span>

![Éditeur de monde ouvert avec la liste d’objets mise en surbrillance](images/interactables-spawner-img-01.png)

<span data-ttu-id="20ea1-113">Dans la page Paramètres, vous trouverez une nouvelle case à cocher **« génération d’objets »**, qui est utilisée pour en faire un objet pouvant être utilisé.</span><span class="sxs-lookup"><span data-stu-id="20ea1-113">On the settings page you’ll find a new checkbox **“Object spawner“**, which is used to make it an interactable object.</span></span>

1. <span data-ttu-id="20ea1-114">Cochez la case et sélectionnez **confirmer**.</span><span class="sxs-lookup"><span data-stu-id="20ea1-114">Check the box and select **confirm**.</span></span>
2. <span data-ttu-id="20ea1-115">En mode édition, vous pouvez vous déplacer autour de l’emplacement de génération de l’objet dans l’espace.</span><span class="sxs-lookup"><span data-stu-id="20ea1-115">While in edit mode, you can move around the object’s spawn location in the space.</span></span>
3. <span data-ttu-id="20ea1-116">**Quittez le mode d’édition** pour activer l’interaction des éléments.</span><span class="sxs-lookup"><span data-stu-id="20ea1-116">**Exit edit mode** to enable item interaction.</span></span>

![Mettre à jour la fenêtre d’artefact ouverte dans l’application AltspaceVR](images/interactables-spawner-img-02.png)

## <a name="other-customizations"></a><span data-ttu-id="20ea1-118">Autres personnalisations</span><span class="sxs-lookup"><span data-stu-id="20ea1-118">Other customizations</span></span>

<span data-ttu-id="20ea1-119">Une fois que vous avez activé la **« génération d’objets »** lorsque vous revenez dans les propriétés de cet objet, il y aura un paramètre supplémentaire que vous pouvez appliquer à la façon dont l’objet généré se comporte.</span><span class="sxs-lookup"><span data-stu-id="20ea1-119">After enabling **“Object spawner”** when you go back into the properties for that object, there will be an extra setting you can apply to how the spawned object behaves.</span></span>

> [!NOTE]
> <span data-ttu-id="20ea1-120">Mise à l’échelle des objets interactifs : définit l’échelle de l’objet lorsqu’il est sélectionné, par rapport à « Scale », qui est l’échelle de la façon dont l’objet apparaît dans le monde avant de le choisir pour la première fois.</span><span class="sxs-lookup"><span data-stu-id="20ea1-120">Interactable object scale: This sets the scale of the object when it gets picked up, compared to “Scale” which is the scale of how the object appears in the world prior to picking it up for the first time.</span></span>

<span data-ttu-id="20ea1-121">Les décideurs peuvent remarquer que les modifications apportées à votre kit pendant l’exécution de AltspaceVR ne prennent pas effet tant que vous n’avez pas redémarré AltspaceVR.</span><span class="sxs-lookup"><span data-stu-id="20ea1-121">Kit makers may notice that changes to your Kit while AltspaceVR is running won't take effect until you restart AltspaceVR.</span></span>

<span data-ttu-id="20ea1-122">Récemment, nous avons ajouté un bouton sous l’onglet **paramètres modérés** appelé **recharger les kits**.</span><span class="sxs-lookup"><span data-stu-id="20ea1-122">Recently we’ve added a button under the **Moderate Settings** tab called **Reload Worlds Kits**.</span></span> <span data-ttu-id="20ea1-123">Si vous cliquez sur ce bouton, (vous pouvez simplement) entrer à nouveau l’espace, recharger tous les kits, ce qui a pour effet de télécharger uniquement les nouvelles versions des kits qui ont été mis à jour pendant que vous étiez dans AltspaceVR.</span><span class="sxs-lookup"><span data-stu-id="20ea1-123">Clicking this button causes (just you) to reenter the space, reloading all Kits again, which will download only new versions of the Kits that have been updated while you were in AltspaceVR.</span></span>

![Panneau Paramètres modérés ouvert dans l’application AltspaceVR](images/interactables-spawner-img-03.png)