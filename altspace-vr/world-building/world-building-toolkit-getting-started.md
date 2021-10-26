---
title: Présentation du chargeur Altspace
description: Découvrez comment configurer et télécharger vos mondes AltspaceVR à l’aide de modèles de scène Unity avec le chargeur Altspace.
ms.date: 09/29/2021
ms.author: v-vtieto
ms.topic: article
keywords: Toolkit, Altspace, téléchargeur
ms.openlocfilehash: 8d71551fe552159c0078105307802774f44c0d47
ms.sourcegitcommit: 8c58f9f9ad1a3f9534141dee2c78e32792d0db7a
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/25/2021
ms.locfileid: "130298799"
---
# <a name="introducing-the-altspace-uploader"></a>Présentation du chargeur Altspace

> [!NOTE]
> - Si vous êtes intéressé, participez au [AltspaceVR officiel](https://discordapp.com/invite/altspacevr) et visitez le canal de construction #world.  
> - Si vous essayez de réactiver un ancien espace, consultez le [Guide de mise à niveau](upgrading-old-unity-projects.md). 

Le chargeur vous permet d’utiliser une scène Unity comme modèle pour vos mondes. Vous pouvez mettre en place une maison hanté pour Halloween ou la création de vos favoris à partir de Minecraft. Si vous pouvez l’importer dans Unity, vous pouvez probablement le faire Altspace de cette façon. Voici quelques exemples de [mondes](https://account.altvr.com/worlds/1046572460192825569).

![Exemples de mondes](images/unity-uploader-img-01.png)

## <a name="setup"></a>Programme d’installation

1. Participez au [AltspaceVR officiel](https://discordapp.com/invite/altspacevr) et visitez le canal de génération de #world. Les amis ne permettent pas aux amis de créer des mondes uniquement.
2. Lisez notre [Guide de prise en main international](world-building-getting-started.md) pour les principes de base
3. [Installez Unity Hub](https://unity3d.com/get-unity/download) et **Unity 2020.3.9**. Le téléchargeur ne fonctionne pas, sauf si vous faites correspondre exactement cette version. Si vous n’en avez pas, vous aurez besoin d’un compte Free Unity. Pendant l’installation, choisissez la version **personnelle** (puisque vous êtes en train de vous amuser !) et assurez-vous d’effectuer les opérations suivantes :
    * Incluez le module de **prise en charge de la build Android** .
    * sur Windows, incluez le module **prise en charge des builds Mac (Mono)** .
    * sur Mac, incluez le module **Windows Build Support (Mono)** .
4. [Télécharger le programme de chargement AltspaceVR](https://aka.ms/AvrUrpUploader)
5. [Créez un modèle](https://account.altvr.com/space_templates/new) sur notre site Web. Nommez-le **Hello World modèle**.
6. [Créez un monde](https://account.altvr.com/worlds/my) et nommez-le **Hello World**. Sélectionnez **Hello World modèle** comme modèle.

![Écran du monde créé](images/unity-uploader-img-02.png)

## <a name="upload-your-scene"></a>Télécharger votre scène

> [!NOTE]
> Vous trouverez un guide pas à pas détaillé [ici](https://buildingthemetaverse.medium.com/how-to-make-your-own-altspace-templates-and-kits-unity-2020-3-9-uploader-2-x-5b40e92bb759).

1. Ouvrez Unity Hub et créez un nouveau projet Unity 2020.3.9. Pour votre modèle, sélectionnez **pipeline de rendu universel**.

    ![Choisir le modèle URP Unity](images/001-unity-templates.png)

1. Accédez au dossier dans lequel vous avez téléchargé le programme de chargement Altspace, puis copiez-le ou déplacez-le à partir de ce dossier vers le dossier racine de votre nouveau projet Unity.
1. dans unity dans la barre de menus, sélectionnez Gestionnaire de package de la **fenêtre**  >  **.**
1. dans la barre de menus Gestionnaire de package, sélectionnez la liste déroulante signe plus (« + »), puis sélectionnez **ajouter un package à partir de tarball**.
1. Accédez au dossier qui contient le téléchargeur Altspace, sélectionnez le téléchargeur, puis cliquez sur **ouvrir**.  Une fois le package chargé, **AltspaceVR** apparaît dans la barre de menus :

    ![AltspaceVR dans la barre de menus](images/002-altspacevr-on-menu-bar.png)

> [!NOTE]
> Vous devez importer le package du téléchargeur Altspace dans chaque projet Unity que vous souhaitez utiliser avec Altspace.
1. Dans la barre de menus, sélectionnez **AltspaceVR > modèles**.
1. Dans la boîte de dialogue **ALTSPACE VR templates** , connectez-vous avec les informations d’identification de votre compte Altspace. (La connexion MSA sera bientôt disponible. Si vous ne vous êtes jamais connecté à Altspace avec votre compte Microsoft, vous devrez créer un mot de passe à l’aide de l’option « vous avez oublié votre mot de passe » sur le site Web.)
1. Cliquez sur la liste déroulante **Sélectionner un modèle** , puis sélectionnez **Hello World modèle**.
1. Choisissez une scène : cliquez sur le bouton **de sélection de fichier. Unity** (trois points), puis accédez au dossier **Assets**  >  **scenes** dans votre projet, puis sélectionnez **SampleScene. Unity** et ouvrez-le.
1. sous **Build pour les plateformes :**, vérifiez **Windows** est sélectionné. Pour le moment, les deux autres options, **Android** et **Mac**, ne doivent **pas** être sélectionnées. Une fois que vous souhaitez que les utilisateurs accèdent à, vous devez générer et charger pour toutes les plateformes.
1. sélectionnez le bouton **générer & Télécharger** . Ce processus peut prendre une ou deux minutes.
1. Lancez Altspace, puis sélectionnez **menu principal**, puis dans la barre de menus, sélectionnez **mes mondes**.
1. Accédez à **Hello World** , puis ouvrez-le.

    Votre scène doit être similaire à ce que vous avez vu dans l’éditeur Unity.

## <a name="whats-supported"></a>Opérations prises en charge

* Oui : modèles, collisions, animations, effets de particules, audio, skyboxes, etc.
* Non : scripts. Pour des raisons de sécurité, les chargements contenant des scripts sont rejetés.
* Peut-être : des éléments fantaisie tels que l’éclairage global dynamique.
* Télécharger des scènes pour différentes plateformes séparément ou ensemble.
* Consultez les [mondes proposés](https://account.altvr.com/worlds/featured). De nombreuses fonctionnalités ont été créées à l’aide du chargeur.

## <a name="tips"></a>Conseils

* Participez au [décordon AltspaceVR officiel](https://discordapp.com/invite/altspacevr).
* Sur la page du modèle sur le côté gauche, nous vous montrons les derniers téléchargements par plateforme. En cas de réussite, il y a **1-2 minutes**. 

![Volet modèles ouvert avec les chargements mis en surbrillance](images/template-upload-list.png)

* Vous pouvez être dans le monde lorsque vous mettez à jour. le moment où le téléchargeur indique **Télécharger terminé** , vous pouvez réinitialiser le monde pour voir les modifications.
* Lors de la création de PC avec une scène simple, il faut prendre moins d’une minute pour voir une modification dans Altspace.
* Définissez votre monde comme privé et dérépertorié pour éviter les distractions.
* Placez un cube à l’origine pour voir où les gens seront générés par défaut. Masquez le cube lors du téléchargement.

## <a name="troubleshooting"></a>Dépannage

**Je suis en chute ou ne peut pas se téléporter sur quoi que ce soit** Vous devez ajouter des collisions à des objets pour les réutiliser.

**Rien n’a changé**
    * Avez-vous enregistré la scène dans Unity ?
    * Avez-vous choisi la plateforme sur laquelle vous effectuez le test ?
    * Êtes-vous dans le monde ? Avez-vous choisi le modèle approprié dans le chargeur et dans le formulaire ?
    * Avez-vous vérifié les statistiques de page de modèle ?

**Télécharger échoue ou expire**
    * L’erreur de chargement la plus courante est due à une mauvaise version d’Unity. Vous devez faire correspondre exactement la version requise.
    * Le chargement est peut-être trop important. Essayez de conserver les scènes de PC < 100 Mo. Commencez petit et de Build. Optimisation, optimisation, optimisation.
    * Essayez avec un nouveau projet qui contient un cube simple.
    * Ne pas forcer la fermeture pendant une génération : elle peut endommager votre scène. Essayez de recharger le téléchargement.

**Il s’agit d’un processus lent**
    * Nous vous recommandons de créer pour PC uniquement lors de l’itération et d’Android plus tard.
    * Essayez de supprimer les fichiers inutilisés. Pour une raison quelconque, Unity obtient parfois des overzealous.

**Je ne parviens pas à me connecter avec mes informations d’identification Altspace**
    * Les e-mails respectent la casse.
    * Essayez avec un nouveau projet.
    * Assurez-vous que votre compte Altspace est en bonne position.

## <a name="see-also"></a>Voir aussi

* [Apprentissage Unity](https://unity3d.com/learn)
* [Forums Unity](https://forum.unity.com)  
