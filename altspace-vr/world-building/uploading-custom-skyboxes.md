---
title: Téléchargement de skyboxes personnalisés
description: Obtenir des instructions pas à pas sur le téléchargement et la résolution des problèmes de votre skyboxes personnalisé dans les expériences AltspaceVR.
ms.date: 03/11/2021
ms.topic: article
keywords: skyboxes, résolution des problèmes
ms.openlocfilehash: 02d5bc762dc36d4195100e8155d6250789e833f7
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/08/2021
ms.locfileid: "107212435"
---
# <a name="uploading-custom-skyboxes"></a><span data-ttu-id="349dd-104">Téléchargement de skyboxes personnalisés</span><span class="sxs-lookup"><span data-stu-id="349dd-104">Uploading custom Skyboxes</span></span>

<span data-ttu-id="349dd-105">Un skybox est un moyen de créer un **arrière-plan** pour votre monde qui rend l’expérience plus immersive.</span><span class="sxs-lookup"><span data-stu-id="349dd-105">A Skybox is a way to create a **background** for your World that makes the experience more immersive.</span></span> <span data-ttu-id="349dd-106">Il existe différents types de skyboxes, mais nous prenons actuellement en charge **équirectangulaire**.</span><span class="sxs-lookup"><span data-stu-id="349dd-106">There are different kinds of Skyboxes but we currently support **equirectangular**.</span></span> <span data-ttu-id="349dd-107">Voici un exemple pris avec une caméra 360 (plus d’exemples [ici](http://moments.mankindforward.com/)) :</span><span class="sxs-lookup"><span data-stu-id="349dd-107">Here's an example taken with a 360 camera (more example [here](http://moments.mankindforward.com/)):</span></span> 

![360 équirectangulaire vue d’un salon](images/custom-skyboxes-img-01.jpeg)

<span data-ttu-id="349dd-109">Vous pouvez également utiliser le [chargeur Unity](world-building-toolkit-getting-started.md) , mais cette approche est plus simple.</span><span class="sxs-lookup"><span data-stu-id="349dd-109">You can also use the [Unity Uploader](world-building-toolkit-getting-started.md) but this approach is simpler.</span></span>

1. <span data-ttu-id="349dd-110">Accédez à [mondes > skyboxes](https://account.altvr.com/skyboxes) et appuyez sur le bouton **créer** à droite</span><span class="sxs-lookup"><span data-stu-id="349dd-110">Navigate to [Worlds > Skyboxes](https://account.altvr.com/skyboxes) and press the **Create** button on the right</span></span>

![Page de site Web mondes ouverte dans le panneau skyboxes](images/custom-skyboxes-img-02.png)

2. <span data-ttu-id="349dd-112">Renseignez un nom et spécifiez votre image 360.</span><span class="sxs-lookup"><span data-stu-id="349dd-112">Fill in a name and specify your 360 image.</span></span> <span data-ttu-id="349dd-113">Il n’est pas nécessaire qu’il s’agit d’une photo. il existe des programmes qui vous permettent de créer les vôtres, ou vous pouvez rechercher des en ligne.</span><span class="sxs-lookup"><span data-stu-id="349dd-113">It doesn't have to be a photo, there are programs that let you draw your own or you can search for some online.</span></span> <span data-ttu-id="349dd-114">Quand vous êtes prêt, sélectionnez **Créer**.</span><span class="sxs-lookup"><span data-stu-id="349dd-114">When you're ready, select **Create**.</span></span> 

![Formulaire de création de skybox](images/custom-skyboxes-img-03.png)

3. <span data-ttu-id="349dd-116">Vous pouvez éventuellement télécharger une image d' **Aperçu** afin de pouvoir identifier facilement ce skybox.</span><span class="sxs-lookup"><span data-stu-id="349dd-116">You can optionally upload a **preview** image so you can easily identify this skybox.</span></span> <span data-ttu-id="349dd-117">Vous pouvez également charger des données audio ambiantes au format WAV.</span><span class="sxs-lookup"><span data-stu-id="349dd-117">You can also upload ambient audio in WAV format.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="349dd-118">Nous vous recommandons de charger les images d’aperçu et l’audio ambiant séparément, une fois que vous avez téléchargé l’image 360.</span><span class="sxs-lookup"><span data-stu-id="349dd-118">We recommend you upload preview images and ambient audio separately, after you upload the 360 image.</span></span> <span data-ttu-id="349dd-119">Si vous les Téléchargez ensemble, la taille des fichiers peut être suffisamment grande pour bloquer le processus.</span><span class="sxs-lookup"><span data-stu-id="349dd-119">If you upload them together the file sizes can be large enough to stall the process.</span></span> <span data-ttu-id="349dd-120">[Jetsons World](https://account.altvr.com/worlds/1004174988393054363/spaces/1084431533181240311) est un excellent exemple illustrant l’utilisation d’un skybox avec l’audio ambiant.</span><span class="sxs-lookup"><span data-stu-id="349dd-120">[Jetsons World](https://account.altvr.com/worlds/1004174988393054363/spaces/1084431533181240311) is a great example of how to use a Skybox with ambient audio.</span></span> <span data-ttu-id="349dd-121">Notez que le monde entier a conservé le volume audio faible et que les sons que vous entendez sont sporadiques pour que les gens ne soient pas importuns.</span><span class="sxs-lookup"><span data-stu-id="349dd-121">Notice how the World-Builder kept the audio volume low and sounds you hear are sporadic so people don't get annoyed.</span></span> 

4. <span data-ttu-id="349dd-122">Accédez à votre monde et ouvrez l’éditeur de monde.</span><span class="sxs-lookup"><span data-stu-id="349dd-122">Enter your World and open the World Editor.</span></span> <span data-ttu-id="349dd-123">Sous skyboxes, sélectionnez votre nouveau skybox.</span><span class="sxs-lookup"><span data-stu-id="349dd-123">Under Skyboxes, select your new Skybox.</span></span> <span data-ttu-id="349dd-124">En quelques secondes, le ciel change littéralement.</span><span class="sxs-lookup"><span data-stu-id="349dd-124">In a few seconds, the sky will literally change.</span></span> <span data-ttu-id="349dd-125">D’autres dans votre monde voient également la modification du ciel.</span><span class="sxs-lookup"><span data-stu-id="349dd-125">Others in your World will also see the sky change.</span></span> <span data-ttu-id="349dd-126">Pour revenir en arrière, choisissez le skybox **par défaut** dans cette même liste.</span><span class="sxs-lookup"><span data-stu-id="349dd-126">To switch back, choose the **default** skybox in that same list.</span></span> 

## <a name="troubleshooting"></a><span data-ttu-id="349dd-127">Résolution des problèmes</span><span class="sxs-lookup"><span data-stu-id="349dd-127">Troubleshooting</span></span>

<span data-ttu-id="349dd-128">**Il y a une couture ou une ligne dans le ciel :-(.**</span><span class="sxs-lookup"><span data-stu-id="349dd-128">**There's a seam or line in the sky :-(.**</span></span> <span data-ttu-id="349dd-129">Il s’agit d’un bogue que nous corrigerons bientôt</span><span class="sxs-lookup"><span data-stu-id="349dd-129">It's a bug that we'll fix soon</span></span>

<span data-ttu-id="349dd-130">**Échec du chargement**</span><span class="sxs-lookup"><span data-stu-id="349dd-130">**Upload failed**</span></span>
    * <span data-ttu-id="349dd-131">essayez de charger uniquement l’image 360 seule</span><span class="sxs-lookup"><span data-stu-id="349dd-131">try uploading just the 360 image on its own</span></span>
    * <span data-ttu-id="349dd-132">Essayez avec un autre fichier plus petit comme un test</span><span class="sxs-lookup"><span data-stu-id="349dd-132">try with another, smaller file as a test</span></span>

<span data-ttu-id="349dd-133">**Je ne trouve pas de photo 360**</span><span class="sxs-lookup"><span data-stu-id="349dd-133">**I can't find a 360 photo**</span></span>
    * <span data-ttu-id="349dd-134">Flickr est une bonne source (modifiez les filtres pour rechercher des éléments créatifs)</span><span class="sxs-lookup"><span data-stu-id="349dd-134">Flickr is a good source (change the filters to find creative commons ones)</span></span>
    * <span data-ttu-id="349dd-135">Prenez votre propre !</span><span class="sxs-lookup"><span data-stu-id="349dd-135">Take your own!</span></span> <span data-ttu-id="349dd-136">Nous avons réussi à utiliser les caméras de la Ricoh.</span><span class="sxs-lookup"><span data-stu-id="349dd-136">We've had success with Ricoh's cameras.</span></span> 
<span data-ttu-id="349dd-137">**Le ciel semble granuleux ou bloqué** Vous devrez peut-être Rechercher une image de résolution supérieure.</span><span class="sxs-lookup"><span data-stu-id="349dd-137">**The sky looks grainy or blocky** You may need to find a higher-resolution image.</span></span> <span data-ttu-id="349dd-138">En général environ 2-5 Mo et ~ 5000 PX x 2000 PX</span><span class="sxs-lookup"><span data-stu-id="349dd-138">Typically around 2-5 MB and ~5000 px x 2000 px</span></span>

<span data-ttu-id="349dd-139">**Cela nuit à la fréquence d’images !**</span><span class="sxs-lookup"><span data-stu-id="349dd-139">**It hurts my World's framerate!**</span></span>
<span data-ttu-id="349dd-140">L’image est probablement trop grande.</span><span class="sxs-lookup"><span data-stu-id="349dd-140">The image is probably too large.</span></span> <span data-ttu-id="349dd-141">Certains skyboxes générés peuvent être de 8 Ko.</span><span class="sxs-lookup"><span data-stu-id="349dd-141">Some generated skyboxes can be 8k.</span></span> <span data-ttu-id="349dd-142">Ils sont généralement fournis avec des versions de 2 Ko faciles à utiliser.</span><span class="sxs-lookup"><span data-stu-id="349dd-142">They usually come with mobile-friendly 2k versions--use that.</span></span>

<span data-ttu-id="349dd-143">**Aidez-moi avec l’audio ambiant**</span><span class="sxs-lookup"><span data-stu-id="349dd-143">**Help me with the ambient audio**</span></span>
    * <span data-ttu-id="349dd-144">Utilisez des logiciels gratuits comme Audacity pour réduire le volume ou créer vos propres boucles.</span><span class="sxs-lookup"><span data-stu-id="349dd-144">Use free software like Audacity to lower the volume or create your own loops.</span></span> <span data-ttu-id="349dd-145">N’oubliez pas que l’audio sera répété et joué dans les oreilles des gens.</span><span class="sxs-lookup"><span data-stu-id="349dd-145">Remember that the audio will be repeated and playing in people's ears so keep it low and not annoying</span></span>
    * <span data-ttu-id="349dd-146">Le [son gratuit](https://freesound.org/) est une bonne source de sons sans royalties</span><span class="sxs-lookup"><span data-stu-id="349dd-146">[Free Sound](https://freesound.org/) is a good source of royalty-free sounds</span></span>
