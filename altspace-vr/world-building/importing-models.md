---
title: Importation de modèles glTF
description: Découvrez comment importer correctement des modèles glTF 3D dans vos expériences AltspaceVR et résoudre les problèmes.
ms.date: 03/11/2021
ms.topic: article
keywords: modèles, glTF, importation, sketchfab, résolution des problèmes
ms.openlocfilehash: 4489f90832bd1cf85ff161caed11684257cce6ab
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/08/2021
ms.locfileid: "107212434"
---
# <a name="importing-gltf-models"></a><span data-ttu-id="2f44b-104">Importation de modèles glTF</span><span class="sxs-lookup"><span data-stu-id="2f44b-104">Importing glTF models</span></span>

> [!NOTE]
> <span data-ttu-id="2f44b-105">Cette fonctionnalité est disponible pour les utilisateurs sélectionnés dans le programme d’accès anticipé à l’heure actuelle.</span><span class="sxs-lookup"><span data-stu-id="2f44b-105">This feature is available for select users in the Early Access program at this time.</span></span>

<span data-ttu-id="2f44b-106">L’une des façons de placer des modèles et des scènes 3D dans Altspace consiste à utiliser la [norme glTF](https://en.wikipedia.org/wiki/GlTF).</span><span class="sxs-lookup"><span data-stu-id="2f44b-106">One way to bring 3D models and scenes into Altspace is using the [glTF standard](https://en.wikipedia.org/wiki/GlTF).</span></span> <span data-ttu-id="2f44b-107">Vous pouvez télécharger un fichier. GLB (compressé glTF) pour créer un modèle que vous pouvez générer ultérieurement dans l’éditeur de monde.</span><span class="sxs-lookup"><span data-stu-id="2f44b-107">You can upload a .glb file (packed glTF) to create a Model that you can later spawn in the World Editor.</span></span> <span data-ttu-id="2f44b-108">Il s’agit d’une alternative au [téléchargement de vos propres kits](uploading-custom-kits.md).</span><span class="sxs-lookup"><span data-stu-id="2f44b-108">It's an alternative to [uploading your own Kits](uploading-custom-kits.md).</span></span> <span data-ttu-id="2f44b-109">Nous vous recommandons de créer des modèles pour les démonstrations rapides, car vous n’aurez pas besoin d’utiliser Unity et de kits lorsque vous souhaitez optimiser les performances et la réutilisation.</span><span class="sxs-lookup"><span data-stu-id="2f44b-109">We recommend creating Models for quick demonstrations because you won't need to use Unity, and Kits when you want to maximize performance and reusability.</span></span> 

1. <span data-ttu-id="2f44b-110">Recherchez des ressources 3D glTF.</span><span class="sxs-lookup"><span data-stu-id="2f44b-110">Find some glTF 3D assets.</span></span> <span data-ttu-id="2f44b-111">Un emplacement à rechercher est Sketchfab (essayez de filtrer les modèles **téléchargeables** comme [celui-ci](https://sketchfab.com/search?features=downloadable&q=low+poly+wolf&sort_by=-pertinence&type=models)).</span><span class="sxs-lookup"><span data-stu-id="2f44b-111">One place to search is Sketchfab (try filtering for **Downloadable** models like [this](https://sketchfab.com/search?features=downloadable&q=low+poly+wolf&sort_by=-pertinence&type=models)).</span></span> <span data-ttu-id="2f44b-112">Une fois que vous l’avez trouvé, sélectionnez **Télécharger le modèle 3D**:</span><span class="sxs-lookup"><span data-stu-id="2f44b-112">Once you find it, select **Download 3D Model**:</span></span>

![modèle de chien 3D à partir de Sketchfab](images/importing-models-img-01.png)

2. <span data-ttu-id="2f44b-114">Copiez le lien vers le modèle et lisez les conditions de licence.</span><span class="sxs-lookup"><span data-stu-id="2f44b-114">Copy the link to the model and read the licensing requirements.</span></span> 
3. <span data-ttu-id="2f44b-115">Télécharger la version de **format autoconversion (glTF)**</span><span class="sxs-lookup"><span data-stu-id="2f44b-115">Download the **Autoconverted Format (glTF)** version</span></span>

![Options de téléchargement Sketchfab avec le format de conversion automatique mis en surbrillance](images/importing-models-img-02.png)

4. <span data-ttu-id="2f44b-117">Ouvrez le site [GLB Packer](https://glb-packer.glitch.me) et cochez la case **convertir png en JPEG (bêta)**</span><span class="sxs-lookup"><span data-stu-id="2f44b-117">Open the [GLB Packer](https://glb-packer.glitch.me) site and check the box **Convert PNG to JPEG (beta)**</span></span>
5. <span data-ttu-id="2f44b-118">Décompressez les fichiers glTF que vous avez téléchargés et faites-les glisser tous en même temps dans l’onglet du navigateur GLB Packer</span><span class="sxs-lookup"><span data-stu-id="2f44b-118">Uncompress the glTF files you downloaded and drag them all at once into the GLB Packer browser tab</span></span>

![Fenêtre présentant la décompression du modèle](images/importing-models-img-03.png)

6. <span data-ttu-id="2f44b-120">Selon le nombre et la taille des fichiers, le traitement peut prendre un certain temps.</span><span class="sxs-lookup"><span data-stu-id="2f44b-120">Depending on the number and size of the files, it may take a while to process.</span></span> <span data-ttu-id="2f44b-121">Lorsque le traitement est terminé, un fichier **out. GLB** est téléchargé.</span><span class="sxs-lookup"><span data-stu-id="2f44b-121">When processing is done, an **out.glb** file will be downloaded.</span></span> <span data-ttu-id="2f44b-122">Renommez ce fichier avec un nom informatif. il s’agit du nom de l’objet dans le monde (par exemple, **Low Wolf. GLB**)</span><span class="sxs-lookup"><span data-stu-id="2f44b-122">Rename that file to something informative--this will be the name of the object in the world (e.g **Low Poly Wolf.glb**)</span></span>
7. <span data-ttu-id="2f44b-123">Accédez à [altvr.com > plus > modèles](https://account.altvr.com/users/sign_in) , puis sélectionnez **créer**</span><span class="sxs-lookup"><span data-stu-id="2f44b-123">Navigate to [altvr.com > More > Models](https://account.altvr.com/users/sign_in) and select **Create**</span></span>
8. <span data-ttu-id="2f44b-124">Spécifiez l’emplacement du fichier. GLB et veillez à copier le lien Sketchfab dans la description de l’attribution.</span><span class="sxs-lookup"><span data-stu-id="2f44b-124">Specify the location of the .glb file and make sure you copy the Sketchfab link into the description for attribution.</span></span> <span data-ttu-id="2f44b-125">Vous pouvez spécifier une image d’aperçu si vous le souhaitez, puis sélectionner **créer un modèle**:</span><span class="sxs-lookup"><span data-stu-id="2f44b-125">You can specify a preview image if you want, then select **Create Model**:</span></span>

![Aperçu du modèle dans AltspaceVR](images/importing-models-img-04.png)

9. <span data-ttu-id="2f44b-127">Sélectionner **copier dans le presse-papiers**</span><span class="sxs-lookup"><span data-stu-id="2f44b-127">Select **Copy to Clipboard**</span></span>
10. <span data-ttu-id="2f44b-128">Ouvrez l' **éditeur World > Altspace > basics > GLTF**</span><span class="sxs-lookup"><span data-stu-id="2f44b-128">Open the **World Editor > Altspace > Basics > GLTF**</span></span>
11. <span data-ttu-id="2f44b-129">Collez votre URL et sélectionnez **confirmer**</span><span class="sxs-lookup"><span data-stu-id="2f44b-129">Paste in your url and select **Confirm**</span></span>

<span data-ttu-id="2f44b-130">Félicitations !</span><span class="sxs-lookup"><span data-stu-id="2f44b-130">Congrats!</span></span> <span data-ttu-id="2f44b-131">Vous venez de générer votre premier modèle.</span><span class="sxs-lookup"><span data-stu-id="2f44b-131">You just spawned your first Model.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="2f44b-132">Résolution des problèmes</span><span class="sxs-lookup"><span data-stu-id="2f44b-132">Troubleshooting</span></span>

<span data-ttu-id="2f44b-133">**Lorsque j’ai cliqué sur **confirmer** , rien ne s’est produit**</span><span class="sxs-lookup"><span data-stu-id="2f44b-133">**When I clicked **Confirm** nothing happened**</span></span>
    * <span data-ttu-id="2f44b-134">Nous avons actuellement une limite de 100 000 polygone.</span><span class="sxs-lookup"><span data-stu-id="2f44b-134">We currently have a 100k polygon limit.</span></span> <span data-ttu-id="2f44b-135">En cas d’échec, supprimez l’objet pour éviter des problèmes potentiels avec les utilisateurs qui rejoignent votre monde</span><span class="sxs-lookup"><span data-stu-id="2f44b-135">If it fails, delete the Object to avoid potential problems with users joining your World</span></span>
    * <span data-ttu-id="2f44b-136">Il peut y avoir d’autres problèmes avec la ressource.</span><span class="sxs-lookup"><span data-stu-id="2f44b-136">There may be other problems with the asset.</span></span> <span data-ttu-id="2f44b-137">Essayez d’utiliser des ressources avec le moins de polygones possible.</span><span class="sxs-lookup"><span data-stu-id="2f44b-137">Try to use assets with as few polygons as possible.</span></span>
    * <span data-ttu-id="2f44b-138">Le modèle que vous apportez peut être petit ou grand.</span><span class="sxs-lookup"><span data-stu-id="2f44b-138">The model you're bringing in may be small or large.</span></span> <span data-ttu-id="2f44b-139">Essayez d’augmenter/de réduire la mise à l’échelle ou de déplacer votre avatar, vous êtes peut-être à l’intérieur du modèle !</span><span class="sxs-lookup"><span data-stu-id="2f44b-139">Try increasing/decreasing the Scale or move your avatar around, you might be standing inside the model!</span></span>

<span data-ttu-id="2f44b-140">**Le chargement est lent** La vitesse à laquelle les autres utilisateurs du monde se chargent en fonction de leurs vitesses de connexion.</span><span class="sxs-lookup"><span data-stu-id="2f44b-140">**It's slow to load** How quickly other users in the World load it will depend on their connection speeds.</span></span> <span data-ttu-id="2f44b-141">Il n’est pas non plus mis en cache comme des ressources de kit.</span><span class="sxs-lookup"><span data-stu-id="2f44b-141">It's also not cached like Kit assets.</span></span> <span data-ttu-id="2f44b-142">Si vous en Placez un dans votre foyer, vous retéléchargerez le même modèle chaque fois que vous vous joignez, ce qui n’est pas très utile.</span><span class="sxs-lookup"><span data-stu-id="2f44b-142">If you place one in your Home, you'll end up redownloading the same Model every time you join, which isn't great.</span></span>

<span data-ttu-id="2f44b-143">**Il n’y a aucune collision** Par défaut, il n’y a aucune collision sur les objets qui sont importés de cette façon</span><span class="sxs-lookup"><span data-stu-id="2f44b-143">**There's no collision** By default there's no collision on the objects that are brought in this way</span></span>

<span data-ttu-id="2f44b-144">**Lorsque je le génère, je perd mes contrôles sur six DDL ou je suis à l’intérieur, il est difficile de le manipuler** . Oui, nous sommes conscients de ces problèmes et espérons les résoudre bientôt.</span><span class="sxs-lookup"><span data-stu-id="2f44b-144">**When I spawn it, I lose my controls on six DOF or I'm inside so it's hard to manipulate it** Yes, we're aware of these issues and hope to address them soon.</span></span>  