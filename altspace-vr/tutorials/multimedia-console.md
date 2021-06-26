---
title: Utilisation de la console multimédia
description: Découvrez comment démarrer la configuration, la publication et le contrôle de la console multimédia dans vos expériences AltspaceVR.
ms.date: 03/11/2021
ms.topic: article
keywords: console, multimédia
ms.openlocfilehash: 4a51ff76e44d3870972bc17288ae77c1fa888922
ms.sourcegitcommit: 2db596ab5a1ecd4901a8c893741cc4d06f6aecea
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2021
ms.locfileid: "112923006"
---
# <a name="using-the-multimedia-console"></a><span data-ttu-id="a1962-104">Utilisation de la console multimédia</span><span class="sxs-lookup"><span data-stu-id="a1962-104">Using the multimedia console</span></span>

<span data-ttu-id="a1962-105">La console multimédia est un outil qui permet le partage de médias dans les événements et les mondes.</span><span class="sxs-lookup"><span data-stu-id="a1962-105">The Multimedia Console is a tool that enables media sharing in events and worlds.</span></span> <span data-ttu-id="a1962-106">Vous pouvez l’utiliser pour partager des éléments tels que des images, des diapositives de présentation, des livestreams, des vidéos, des sélections, etc.</span><span class="sxs-lookup"><span data-stu-id="a1962-106">You can use it to share things like images, presentation slides, livestreams, videos, playlists, and more.</span></span> <span data-ttu-id="a1962-107">Vous trouverez ci-dessous une instruction pas à pas sur l’utilisation de la console multimédia **v 0.5.0 +**.</span><span class="sxs-lookup"><span data-stu-id="a1962-107">Below is a step-by-step instruction on how to use the Multimedia Console **v0.5.0+**.</span></span> 

## <a name="getting-started"></a><span data-ttu-id="a1962-108">Prise en main</span><span class="sxs-lookup"><span data-stu-id="a1962-108">Getting started</span></span>

<span data-ttu-id="a1962-109">La prise en main de la console multimédia est un processus en deux parties.</span><span class="sxs-lookup"><span data-stu-id="a1962-109">Getting started with the Multimedia Console is a two part process.</span></span>  <span data-ttu-id="a1962-110">Tout d’abord, le portail Web que vous utiliserez pour générer et publier une configuration pour la session de console multimédia que vous placez dans votre environnement.</span><span class="sxs-lookup"><span data-stu-id="a1962-110">First there's the web portal that you'll use to generate and publish a configuration for the Multimedia Console session you place in your environment.</span></span>  <span data-ttu-id="a1962-111">Deuxièmement est le placement de l’application de console multimédia réelle dans votre environnement et la définition du code de configuration qu’elle doit utiliser.</span><span class="sxs-lookup"><span data-stu-id="a1962-111">Second is the placement of the actual Multimedia Console app in your environment and setting the configuration code it should use.</span></span>

### <a name="configuring-the-multimedia-console-with-the-web-portal"></a><span data-ttu-id="a1962-112">Configuration de la console multimédia avec le portail Web</span><span class="sxs-lookup"><span data-stu-id="a1962-112">Configuring the Multimedia console with the web portal</span></span>

1. <span data-ttu-id="a1962-113">Tout d’abord, vous devez vous assurer que votre contenu est hébergé en ligne, car vous aurez besoin d’une URL.</span><span class="sxs-lookup"><span data-stu-id="a1962-113">First, you'll need to make sure your content is hosted online because you'll need a URL.</span></span> <span data-ttu-id="a1962-114">(Vous pouvez télécharger des photos sur altvr.com, héberger une vidéo .mp4 fichier en ligne ou utiliser un lien Dlive Live Stream : https://dlive.tv/yourlivestream)</span><span class="sxs-lookup"><span data-stu-id="a1962-114">(You can upload photos to altvr.com, host a video .mp4 file online or use a Dlive live stream link: https://dlive.tv/yourlivestream)</span></span> 
2. <span data-ttu-id="a1962-115">Accédez au portail Web pour la console multimédia à l’adresse [https://multimedia-console.altvr.com/](https://multimedia-console.altvr.com/)</span><span class="sxs-lookup"><span data-stu-id="a1962-115">Navigate to the web portal for the Multimedia Console at [https://multimedia-console.altvr.com/](https://multimedia-console.altvr.com/)</span></span>
3. <span data-ttu-id="a1962-116">À partir du portail Web, vous pouvez générer et publier une configuration pour la console multimédia.</span><span class="sxs-lookup"><span data-stu-id="a1962-116">From the web portal, you can generate and publish a configuration for the Multimedia Console.</span></span>  <span data-ttu-id="a1962-117">(Voir ci-dessous pour plus d’informations sur les différentes propriétés).</span><span class="sxs-lookup"><span data-stu-id="a1962-117">(See below for details about the various properties).</span></span>
4. <span data-ttu-id="a1962-118">Une fois que vous avez entré le média dans la liste des médias et que vous avez configuré les paramètres généraux, sélectionnez le bouton publier dans la partie supérieure droite de l’application.</span><span class="sxs-lookup"><span data-stu-id="a1962-118">Once you've entered the media into the media list and have configured the general settings, select the publish button in the top-right part of the app.</span></span>
5. <span data-ttu-id="a1962-119">Une fois la publication terminée, une boîte de dialogue s’affiche avec un code de deux mots que vous pouvez entrer dans la console multimédia que vous avez placée.</span><span class="sxs-lookup"><span data-stu-id="a1962-119">Once the publish has completed, a dialog will pop up with a two word code for you to enter in to the Multimedia Console you placed.</span></span>
  
### <a name="placing-the-multimedia-console-in-your-environment"></a><span data-ttu-id="a1962-120">Placement de la console multimédia dans votre environnement</span><span class="sxs-lookup"><span data-stu-id="a1962-120">Placing the Multimedia console in your environment</span></span>

1. <span data-ttu-id="a1962-121">Sélectionnez **éditeur > panneau de l’éditeur > applications SDK > console multimédia**.</span><span class="sxs-lookup"><span data-stu-id="a1962-121">Select on **World Editor > Editor Panel > SDK Apps > Multimedia Console**.</span></span> <span data-ttu-id="a1962-122">(N’accédez pas à l' **éditeur World > notions de base > application SDK**, pour les applications non inscrites.)</span><span class="sxs-lookup"><span data-stu-id="a1962-122">(Don't go to **World Editor > Basics > SDK App**--that's for unregistered apps.)</span></span>  
2. <span data-ttu-id="a1962-123">Placez la console multimédia sur la suite la mieux adaptée à votre espace et à votre public.</span><span class="sxs-lookup"><span data-stu-id="a1962-123">Position the Multimedia Console to best suite your space and audience.</span></span>
3. <span data-ttu-id="a1962-124">Quittez le mode d’édition en cliquant sur le bouton orange en mode d’édition.</span><span class="sxs-lookup"><span data-stu-id="a1962-124">Get out of Edit Mode by clicking the orange Edit Mode button.</span></span>
4. <span data-ttu-id="a1962-125">Vous êtes invité à indiquer **le propriétaire du lecteur multimédia ?**</span><span class="sxs-lookup"><span data-stu-id="a1962-125">You'll be prompted **Are you the media player owner?**</span></span> <span data-ttu-id="a1962-126">Si vous êtes la personne qui doit être le propriétaire officiel de cette session de console multimédia, confirmez et continuez.</span><span class="sxs-lookup"><span data-stu-id="a1962-126">If you're the person who should be the official owner of this Multimedia Console session, confirm and continue.</span></span> <span data-ttu-id="a1962-127">(D’autres rôles permissions sont également disponibles.</span><span class="sxs-lookup"><span data-stu-id="a1962-127">(Other permissioned roles are available as well.</span></span> <span data-ttu-id="a1962-128">Pour obtenir une liste détaillée, voir ci-dessous.)</span><span class="sxs-lookup"><span data-stu-id="a1962-128">See below for a detailed list.)</span></span>
5. <span data-ttu-id="a1962-129">Sélectionnez Oui pour confirmer que vous êtes l’hôte principal.</span><span class="sxs-lookup"><span data-stu-id="a1962-129">Select Yes to confirm that you are the primary host.</span></span>  
6. <span data-ttu-id="a1962-130">Une boîte de dialogue s’affiche pour vous demander d’entrer un code à partir du portail Web ou un JSON valide.</span><span class="sxs-lookup"><span data-stu-id="a1962-130">A dialog should pop up that asks you to enter a code from the web portal or valid JSON.</span></span>  <span data-ttu-id="a1962-131">Entrez les deux codes de mot du portail Web, y compris le tiret, puis appuyez sur OK.</span><span class="sxs-lookup"><span data-stu-id="a1962-131">Enter the two word code from the web portal including the dash and hit OK.</span></span> <span data-ttu-id="a1962-132">(JSON est une configuration avancée décrite ci-dessous)</span><span class="sxs-lookup"><span data-stu-id="a1962-132">(JSON is an advanced configuration described below)</span></span>
7. <span data-ttu-id="a1962-133">La console multimédia doit être chargée après quelques secondes avec la configuration que vous avez créée dans le portail Web.</span><span class="sxs-lookup"><span data-stu-id="a1962-133">The Multimedia Console should load after a few seconds with the configuration you built in the web portal.</span></span>

### <a name="controlling-the-multimedia-console"></a><span data-ttu-id="a1962-134">Contrôle de la console multimédia</span><span class="sxs-lookup"><span data-stu-id="a1962-134">Controlling the Multimedia console</span></span>

1. <span data-ttu-id="a1962-135">Une fois que vous avez entré votre code et terminé le processus de configuration, vous voyez s’afficher les boutons de contrôle sous un affichage de média.</span><span class="sxs-lookup"><span data-stu-id="a1962-135">After you input your code and complete the configuration process, you'll see control buttons appear below a media display.</span></span> 
    * <span data-ttu-id="a1962-136">**Play** démarre la visionneuse multimédia (ou redémarre à l’entrée en cours, si elle s’est arrêtée précédemment)</span><span class="sxs-lookup"><span data-stu-id="a1962-136">**Play** starts the media viewer (or restarts at current entry, if previously stopped)</span></span> 
    * <span data-ttu-id="a1962-137">**Arrêter** arrête la visionneuse multimédia et masque le média actuel.</span><span class="sxs-lookup"><span data-stu-id="a1962-137">**Stop** stops the media viewer, and hides current media.</span></span>  
    * <span data-ttu-id="a1962-138">**Suivant/précédent** passe au support suivant ou précédent</span><span class="sxs-lookup"><span data-stu-id="a1962-138">**Next/Prev** skips to next or previous media</span></span> 
    * <span data-ttu-id="a1962-139">**x/x**   affiche l’index actuel dans la liste des médias et vous permet d’accéder à n’importe quel point de la liste</span><span class="sxs-lookup"><span data-stu-id="a1962-139">**x/x** shows the current index into the media list, and allows you to jump to any point in the list</span></span>
    * <span data-ttu-id="a1962-140">La **configuration permet de** réentrer un nouveau code à partir du portail Web pour définir une nouvelle configuration dans la console.</span><span class="sxs-lookup"><span data-stu-id="a1962-140">**Config** allows reentering a new code from the web portal to set a new configuration in the console.</span></span> 

<span data-ttu-id="a1962-141">Vous êtes maintenant prêt à commencer le partage via la console multimédia !</span><span class="sxs-lookup"><span data-stu-id="a1962-141">Now you're set to begin sharing via the Multimedia Console!</span></span>  
 
## <a name="working-with-the-web-portal"></a><span data-ttu-id="a1962-142">Utilisation du portail Web</span><span class="sxs-lookup"><span data-stu-id="a1962-142">Working with the web portal</span></span>

<span data-ttu-id="a1962-143">Le portail Web est une application Web qui permet de configurer les différentes fonctionnalités de la console multimédia.</span><span class="sxs-lookup"><span data-stu-id="a1962-143">The web portal is a web app that enables configuring the various features of the Multimedia Console.</span></span>  <span data-ttu-id="a1962-144">Ces fonctionnalités se répartissent en deux catégories : les paramètres généraux de la console média et la liste des médias.</span><span class="sxs-lookup"><span data-stu-id="a1962-144">These features fall in to two categories; general media console settings, and the media play list.</span></span>

### <a name="multimedia-console-general-settings"></a><span data-ttu-id="a1962-145">Paramètres généraux de la console multimédia</span><span class="sxs-lookup"><span data-stu-id="a1962-145">Multimedia console general settings</span></span>

<span data-ttu-id="a1962-146">**Paramètres Playback**</span><span class="sxs-lookup"><span data-stu-id="a1962-146">**Playback Settings**</span></span>

<span data-ttu-id="a1962-147">Paramètres de lecture généraux pour la liste des médias</span><span class="sxs-lookup"><span data-stu-id="a1962-147">General playback settings for the media list</span></span>

* <span data-ttu-id="a1962-148">**Liste des médias en boucle**: détermine si la liste des médias doit boucler une fois que vous avez atteint la fin de la liste.</span><span class="sxs-lookup"><span data-stu-id="a1962-148">**Loop Media List**- Determines whether the media list should loop around once you reach the end of the list.</span></span>
* <span data-ttu-id="a1962-149">**Start, méthode** : sélectionne la méthode par laquelle la console multimédia doit démarrer.</span><span class="sxs-lookup"><span data-stu-id="a1962-149">**Start Method** - Selects the method by which the multimedia console should start.</span></span>
    * <span data-ttu-id="a1962-150">Manuel : attend que le bouton de lecture soit enfoncé avant de démarrer le média.</span><span class="sxs-lookup"><span data-stu-id="a1962-150">Manual - Waits for the play button to be pressed before starting the media</span></span>
    * <span data-ttu-id="a1962-151">Démarrage automatique à partir du début-démarre automatiquement la liste des médias à partir du début de la liste</span><span class="sxs-lookup"><span data-stu-id="a1962-151">Auto Start from Beginning - Auto start the media list from the beginning of the list</span></span>
    * <span data-ttu-id="a1962-152">Démarrage automatique aléatoire : démarre automatiquement le support à partir d’un point de départ aléatoire dans la liste</span><span class="sxs-lookup"><span data-stu-id="a1962-152">Auto Start Random - Auto starts the media from a random starting point in the list</span></span>

<span data-ttu-id="a1962-153">**Rôles**</span><span class="sxs-lookup"><span data-stu-id="a1962-153">**Roles**</span></span>

<span data-ttu-id="a1962-154">Attributions de rôles pour le contrôle et la configuration de la console multimédia.</span><span class="sxs-lookup"><span data-stu-id="a1962-154">Role assignments for controlling and configuring the Multimedia Console.</span></span>    <span data-ttu-id="a1962-155">Ces rôles sont décomposés dans l’ensemble suivant :</span><span class="sxs-lookup"><span data-stu-id="a1962-155">These roles are broken down in to the following set:</span></span>

* <span data-ttu-id="a1962-156">**Propriétaire uniquement** : utilisateur propriétaire de la session de la console multimédia</span><span class="sxs-lookup"><span data-stu-id="a1962-156">**Owner Only** - The user that is the owner of the Multimedia Console Session</span></span>
* <span data-ttu-id="a1962-157">**Utilisateurs avec élévation de privilèges** : utilisateurs disposant d’un modérateur ou de rôles d’hôte dans l’espace dans lequel la console multimédia est configurée à l’origine</span><span class="sxs-lookup"><span data-stu-id="a1962-157">**Elevated Users** - Users that have moderator or host roles in the space that the Multimedia Console is configured in originally</span></span>
* <span data-ttu-id="a1962-158">**Tous les utilisateurs** -tous les utilisateurs</span><span class="sxs-lookup"><span data-stu-id="a1962-158">**All Users** - All users</span></span>

<span data-ttu-id="a1962-159">Ces rôles empilent dans le sens que tous les rôles au-dessus de celui choisi dans cette liste seront également autorisés à utiliser cette fonctionnalité.</span><span class="sxs-lookup"><span data-stu-id="a1962-159">These roles stack in the sense that all roles above the one chosen in this list will also be granted permission to use that feature.</span></span>  <span data-ttu-id="a1962-160">Exemple : les **utilisateurs avec élévation de privilèges** incluent le **propriétaire** même s’ils ne sont pas un modérateur ou un hôte \* \* dans AltspaceVR.</span><span class="sxs-lookup"><span data-stu-id="a1962-160">Example: **Elevated Users** includes the **Owner** even if they aren't a moderator or host\*\* in AltspaceVR.</span></span> <span data-ttu-id="a1962-161">Les fonctionnalités contrôlées par les attributions de rôles sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="a1962-161">Features that are controlled by role assignments are as follows</span></span>

* <span data-ttu-id="a1962-162">**Peut contrôler le lecteur multimédia** : détermine les rôles qui peuvent contrôler les boutons de lecture du média pour la console multimédia.</span><span class="sxs-lookup"><span data-stu-id="a1962-162">**Can control media player** - Determines what roles can control the media playback buttons for the Multimedia Console</span></span>
* <span data-ttu-id="a1962-163">**Peut configurer le lecteur multimédia** : détermine les rôles qui peuvent configurer la console multimédia en lui accordant l’accès au bouton de **configuration**</span><span class="sxs-lookup"><span data-stu-id="a1962-163">**Can configure the media player** - Determines what roles can configure the Multimedia Console by being granted access to the **Config** button</span></span>

### <a name="adding-photos-and-videos-to-the-media-list"></a><span data-ttu-id="a1962-164">Ajout de photos et de vidéos à la liste des médias</span><span class="sxs-lookup"><span data-stu-id="a1962-164">Adding photos and videos to the media list</span></span>

<span data-ttu-id="a1962-165">Le média est le cœur de la console multimédia.</span><span class="sxs-lookup"><span data-stu-id="a1962-165">Media is the heart of the Multimedia Console.</span></span>  <span data-ttu-id="a1962-166">Les images et les liens vidéo sont pris en charge en tant que types de média dans la console multimédia.</span><span class="sxs-lookup"><span data-stu-id="a1962-166">Images and video links are supported as media types within the Multimedia Console.</span></span>  <span data-ttu-id="a1962-167">Pour ajouter un nouveau média, sélectionnez les icônes **Ajouter une image** ou ajouter une **vidéo** pour afficher une boîte de dialogue pour entrer les informations et les paramètres du média.</span><span class="sxs-lookup"><span data-stu-id="a1962-167">To add new media, select either the **Add Image** or **Add Video** icons to have a dialog pop up to enter the media information and settings.</span></span>  <span data-ttu-id="a1962-168">Voici la répartition des types de médias et des paramètres associés</span><span class="sxs-lookup"><span data-stu-id="a1962-168">Below is the breakdown of the media types and associated settings</span></span>

<span data-ttu-id="a1962-169">**Image**</span><span class="sxs-lookup"><span data-stu-id="a1962-169">**Image**</span></span>

<span data-ttu-id="a1962-170">Les images doivent être un type d’image standard comme JPEG, png et fils sur.</span><span class="sxs-lookup"><span data-stu-id="a1962-170">Images should be a standard image type such as jpeg, png, and son on.</span></span> <span data-ttu-id="a1962-171">Ils doivent être hébergés dans un emplacement avec un lien public.</span><span class="sxs-lookup"><span data-stu-id="a1962-171">They need to be hosted somewhere with a public link.</span></span>

* <span data-ttu-id="a1962-172">**Nom** -(obligatoire) nom avec lequel vous souhaitez identifier l’image.</span><span class="sxs-lookup"><span data-stu-id="a1962-172">**Name** - (Required) Name that you wish to identify the image with.</span></span>
* <span data-ttu-id="a1962-173">**URL** de l’image : (obligatoire) URL publique de l’image</span><span class="sxs-lookup"><span data-stu-id="a1962-173">**Image URL** - (Required) The public url of the image</span></span>
* <span data-ttu-id="a1962-174">**Ignorer après** : nombre de secondes pendant lequel l’image doit être ignorée après</span><span class="sxs-lookup"><span data-stu-id="a1962-174">**Skip After** - The number of seconds that the image should be skipped after</span></span>

<span data-ttu-id="a1962-175">**Vidéo**</span><span class="sxs-lookup"><span data-stu-id="a1962-175">**Video**</span></span>

<span data-ttu-id="a1962-176">Les vidéos peuvent être des vidéos hébergées ou des flux en direct via Twitch et DLive.</span><span class="sxs-lookup"><span data-stu-id="a1962-176">Videos can be hosted videos or live streams through Twitch and DLive.</span></span>  <span data-ttu-id="a1962-177">(Un autre support peut fonctionner avec un travail supplémentaire pour récupérer l’URL de flux appropriée, mais n’est pas entièrement pris en charge dans la console multimédia)</span><span class="sxs-lookup"><span data-stu-id="a1962-177">(Other support may function with extra work to get the proper stream url, but aren't fully supported within the Multimedia Console)</span></span>

* <span data-ttu-id="a1962-178">**Nom** : nom (obligatoire) avec lequel vous souhaitez identifier la vidéo.</span><span class="sxs-lookup"><span data-stu-id="a1962-178">**Name** - (Required) Name that you wish to identify the video with.</span></span>
* <span data-ttu-id="a1962-179">**URL** de la vidéo : (obligatoire) URL à partir de laquelle la vidéo est hébergée ou à partir de laquelle le flux en direct est servi.</span><span class="sxs-lookup"><span data-stu-id="a1962-179">**Video URL** - (Required) The public url that the video is hosted at or the live stream is served from.</span></span>
* <span data-ttu-id="a1962-180">**Ignorer après** : nombre de secondes pendant lesquelles la vidéo doit être ignorée après</span><span class="sxs-lookup"><span data-stu-id="a1962-180">**Skip After** - The number of seconds that the video should be skipped after</span></span>

> [!NOTE]
> <span data-ttu-id="a1962-181">OBLIGATOIRE : placez dans le temps qui correspond à la longueur de la vidéo pour permettre aux vidéos de se transférer correctement.</span><span class="sxs-lookup"><span data-stu-id="a1962-181">REQUIRED: Put in the time that matches the length of the video to enable videos to properly forward.</span></span> <span data-ttu-id="a1962-182">Par exemple, si votre vidéo dure 5 minutes à 300 secondes, dans le cas contraire, votre vidéo ne passera pas à la partie suivante du contenu.</span><span class="sxs-lookup"><span data-stu-id="a1962-182">For example, if your video is 5 minutes long put 300 seconds, otherwise your video won't skip to the next piece of content.</span></span>

* <span data-ttu-id="a1962-183">**Volume** : volume de la vidéo de 0 (min)-1 (max) valeurs.</span><span class="sxs-lookup"><span data-stu-id="a1962-183">**Volume** - The volume of the video from 0 (min) - 1 (max) values.</span></span>
* <span data-ttu-id="a1962-184">**Heure de début** : nombre de secondes à partir du début de la vidéo à partir de.</span><span class="sxs-lookup"><span data-stu-id="a1962-184">**Start Time** - The number of seconds from the beginning of the video start from.</span></span>
* <span data-ttu-id="a1962-185">**Distance de début** de l’annulation : distance en mètres dans le monde selon laquelle le volume commence à tomber à mesure que vous quittez la console multimédia</span><span class="sxs-lookup"><span data-stu-id="a1962-185">**Roll Off Start Distance** - The distance in meters in world that the volume begins to fall off at as you move away from the Multimedia Console</span></span>
* <span data-ttu-id="a1962-186">**Action de fin de vidéo** -action à effectuer une fois la fin de la vidéo atteinte.</span><span class="sxs-lookup"><span data-stu-id="a1962-186">**End of Video Action** - The action to take once the end of the video is reached.</span></span>
    * <span data-ttu-id="a1962-187">Arrêter : la liste des médias s’arrête après la fin de la vidéo</span><span class="sxs-lookup"><span data-stu-id="a1962-187">Stop - The media list stops after the video has ended</span></span>
    * <span data-ttu-id="a1962-188">Loop : la vidéo est en boucle jusqu’à ce qu’elle soit ignorée manuellement</span><span class="sxs-lookup"><span data-stu-id="a1962-188">Loop - The video will loop until manually skipped</span></span>
    * <span data-ttu-id="a1962-189">Lire suivant : le média suivant dans la liste des médias sera démarré après la fin de la vidéo actuelle.</span><span class="sxs-lookup"><span data-stu-id="a1962-189">Play Next - The next media in the media list will be started after the current video ends.</span></span>

## <a name="working-with-json-directly-advancedoptional"></a><span data-ttu-id="a1962-190">Utilisation directe de JSON (avancé/facultatif)</span><span class="sxs-lookup"><span data-stu-id="a1962-190">Working with JSON directly (advanced/optional)</span></span>

<span data-ttu-id="a1962-191">La console multimédia prend en charge l’entrée de JSON directement dans à l’invite de la console dans AltspaceVR.</span><span class="sxs-lookup"><span data-stu-id="a1962-191">The Multimedia Console supports entering JSON directly in to the prompt of the console in AltspaceVR.</span></span>  <span data-ttu-id="a1962-192">JSON est le mécanisme interne avec lequel nous activons les configurations de lecteur multimédia.</span><span class="sxs-lookup"><span data-stu-id="a1962-192">JSON is the internal mechanism with which we enable media player configurations.</span></span> <span data-ttu-id="a1962-193">L’exposition de la possibilité de définir JSON directement est un outil qui permet aux utilisateurs plus expérimentés de créer leurs propres flux de travail qui reposent leurs besoins et leur familiarité avec JSON.</span><span class="sxs-lookup"><span data-stu-id="a1962-193">Exposing the ability to set JSON directly is something that allows for more advanced users to build their own workflows that suites their needs and familiarity with JSON.</span></span>  <span data-ttu-id="a1962-194">Vous trouverez ci-dessous une brève description de la structure JSON et du schéma par lequel le JSON est validé.</span><span class="sxs-lookup"><span data-stu-id="a1962-194">The following is a brief description of the JSON structure and the schema by which the JSON is validated.</span></span> <span data-ttu-id="a1962-195">Pour obtenir une description plus détaillée des propriétés ci-dessous, consultez les sections ci-dessus relatives à la configuration de la console multimédia.</span><span class="sxs-lookup"><span data-stu-id="a1962-195">For more detailed descriptions of the properties below, see the above sections that talk about configuring the Multimedia Console.</span></span>  <span data-ttu-id="a1962-196">Cette section se concentre principalement sur les exemples de schémas et la structuration des données JSON.</span><span class="sxs-lookup"><span data-stu-id="a1962-196">This section is focused primarily on the schema examples and structuring for the JSON data.</span></span>

### <a name="global-media-settings"></a><span data-ttu-id="a1962-197">Paramètres multimédias globaux</span><span class="sxs-lookup"><span data-stu-id="a1962-197">Global media settings</span></span>

```json
{
  "loopMediaList": true | false
  "startMethod": "manual" | "autostart-beginning" | "autostart-random"
  "controlMediaPlayer": "everyone" | "elevated" | "owner"
  "configureMediaPlayer": "elevated" | "owner"
  ...
}
```

### <a name="media-list"></a><span data-ttu-id="a1962-198">Liste des médias</span><span class="sxs-lookup"><span data-stu-id="a1962-198">Media list</span></span>

<span data-ttu-id="a1962-199">La liste des médias est une propriété définie à la racine de la structure JSON, comme les rôles et les paramètres de lecture.</span><span class="sxs-lookup"><span data-stu-id="a1962-199">The media list is a property set at the root of the JSON structure like the Roles and Playback Settings.</span></span>  <span data-ttu-id="a1962-200">Il s’agit d’un tableau simple qui peut contenir l’une des structures de configuration de média suivantes.</span><span class="sxs-lookup"><span data-stu-id="a1962-200">It's a simple array that can contain one of the following media configuration structures.</span></span> <span data-ttu-id="a1962-201">(Consultez les descriptions de propriétés ci-dessus pour plus d’informations sur ce que fait.)</span><span class="sxs-lookup"><span data-stu-id="a1962-201">(See property descriptions above for details on what each does.)</span></span>

<span data-ttu-id="a1962-202">**Exemple d’image**</span><span class="sxs-lookup"><span data-stu-id="a1962-202">**Image example**</span></span>

<span data-ttu-id="a1962-203">*Champs obligatoires : « Name » et « imageUrl »*</span><span class="sxs-lookup"><span data-stu-id="a1962-203">*Required fields: "name" and "imageUrl"*</span></span>

```json
{
    "name": "Altspace Screenshot",
    "imageUrl": "https://pbs.twimg.com/media/CxJ-fJqUsAAFtd9.jpg",
    "skipAfter": 10
}
```

<span data-ttu-id="a1962-204">**Exemple de vidéo**</span><span class="sxs-lookup"><span data-stu-id="a1962-204">**Video example**</span></span>

<span data-ttu-id="a1962-205">*Champs obligatoires : « Name » et « videoUrl »*</span><span class="sxs-lookup"><span data-stu-id="a1962-205">*Required fields: "name" and "videoUrl"*</span></span>

```json
{
    "name": "Ninja Twitch Live Stream",
    "videoUrl":"https://www.twitch.tv/ninja",
    "volume":0.2,
    "startTime":0,
    "endOfVideoAction":"play-next"
}
```

### <a name="example-json"></a><span data-ttu-id="a1962-206">Exemple JSON</span><span class="sxs-lookup"><span data-stu-id="a1962-206">Example JSON</span></span>

```json
{
  "loopMediaList": false,
  "startMethod": "autostart-beginning",
  "controlMediaPlayer": "everyone",
  "configureMediaPlayer": "elevated",
  "mediaList": [
    {
      "videoUrl": "https://www.twitch.tv/ninja",
      "volume": 0.2,
      "startTime": 0,
      "endOfVideoAction": "play-next"
    },
    {
      "imageUrl": "http://www.hypergridbusiness.com/wp-content/uploads/2016/09/AltspaceVR-highrise.jpg",
      "skipAfter": 10
    },
    {
      "imageUrl": "https://d1qb2nb5cznatu.cloudfront.net/startups/i/333629-6ffd7199b9bcf34d8957e8e09d974a38-medium_jpg.jpg?buster=1423092095",
      "skipAfter": 5
    },
    {
      "imageUrl": "https://pbs.twimg.com/media/CxJ-fJqUsAAFtd9.jpg",
      "skipAfter": 10
    },
    {
      "imageUrl": "https://altvr-wpengine.netdna-ssl.com/wp-content/uploads/2019/05/Educators-in-VR-Social-VR-AltspaceVR.png",
      "skipAfter": 10
    },
    {
      "videoUrl": "https://www.twitch.tv/shroud",
      "volume": 1,
      "startTime": 0,
      "endOfVideoAction": "stop"
    }
  ]
}
```

### <a name="schema"></a><span data-ttu-id="a1962-207">schéma</span><span class="sxs-lookup"><span data-stu-id="a1962-207">Schema</span></span>

```json
{
  "$schema": "https://json-schema.org/draft-04/schema#",
  "type": "object",
  "required": [
    "mediaList"
  ],
  "properties": {
    "loopMediaList": {
      "type": "boolean",
      "description": "Whether to loop through the media list when reaching the beginning or end of the list."
    },
    "controlMediaPlayer": {
      "type": "string",
      "enum": [
        "everyone",
        "elevated",
        "owner"
      ],
      "default": "owner",
      "description": "What roles are able to control the media player. (Owner can always control player)"
    },
    "configureMediaPlayer": {
      "type": "string",
      "enum": [
        "elevated",
        "owner"
      ],
      "default": "owner",
      "description": "What roles are allowed to configure the media play list.  Note: This role needs to be able to control the media player in order to configure it. (Owner can always configure media)"
    },
    "startMethod": {
      "type": "string",
      "enum": [
        "manual",
        "autostart-beginning",
        "autostart-random"
      ],
      "default": "manual",
      "description": "The method by which the media player should start"
    },
    "mediaList": {
      "description": "A list of images or videos to configure the media player to operate on.",
      "type": "array",
      "items": {
        "oneOf": [
          {
            "title": "Image",
            "type": "object",
            "description": "Configuration for an image media.",
            "properties": {
              "imageUrl": {
                "type": "string",
                "description": "The url for the image to load."
              },
              "skipAfter": {
                "type": "number",
                "minimum": 5,
                "default": null,
                "description": "The number of seconds that should pass before skipping to the next media. (Minimum 5)."
              }
            },
            "required": [
              "imageUrl"
            ]
          },
          {
            "title": "Video",
            "type": "object",
            "description": "Configuration for a video media.",
            "properties": {
              "videoUrl": {
                "type": "string",
                "description": "The url of the video to load."
              },
              "skipAfter": {
                "type": "number",
                "minimum": 5,
                "default": null,
                "description": "The number of seconds that should pass before skipping to the next media. (Minimum 5)."
              },
              "volume": {
                "type": "number",
                "minimum": 0,
                "maximum": 1,
                "default": null,
                "description": "The volume to play the video at. (Minimum 0, maximum 1)"
              },
              "startTime": {
                "type": "number",
                "minimum": 0,
                "default": null,
                "description": "The time in seconds from the start of the video to begin playing the video at. (Minimum of 0)"
              },
              "rolloffStartDistance": {
                "type": "number",
                "minimum": 0,
                "default": null,
                "description": "The distance in meters away from the media player that the volume will begin to fall off. (Minimum 0)"
              },
              "endOfVideoAction": {
                "type": "string",
                "enum": [
                  "stop",
                  "loop",
                  "play-next"
                ],
                "default": null,
                "description": "The type of action to take at the end of the video."
              }
            },
            "required": [
              "videoUrl"
            ]
          }
        ]
      }
    }
  }
}
```

> [!NOTE]
> <span data-ttu-id="a1962-208">À jour avec la console multimédia v 0.5.0</span><span class="sxs-lookup"><span data-stu-id="a1962-208">Up to date with Multimedia Console v0.5.0</span></span>