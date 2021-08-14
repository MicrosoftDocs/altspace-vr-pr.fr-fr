---
title: Utilisation du projecteur Web pour diffuser un navigateur
description: Découvrez comment utiliser le projecteur Web pour diffuser du contenu à partir d’un navigateur désigné dans des expériences AltspaceVR.
ms.date: 03/11/2021
ms.topic: article
keywords: projecteur Web, flux, navigateur
ms.openlocfilehash: 8f25de68ba633e10b9192b85c883de4ba48fd7987ec5d301ebac8443982a1a55
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/11/2021
ms.locfileid: "119127303"
---
# <a name="using-the-web-projector-to-stream-a-browser"></a>Utilisation du projecteur Web pour diffuser un navigateur

Le projecteur Web AltspaceVR est une solution de partage de médias robuste qui vous permet de diffuser un onglet de navigateur désigné de votre ordinateur de bureau directement dans AltspaceVR. Il peut être utilisé pour partager des diapositives, des vidéos, des photos et d’autres éléments que vous pouvez ouvrir à partir d’un navigateur. * le projecteur Web nécessite le téléchargement d’une extension de navigateur et est actuellement disponible exclusivement par le biais de l’éditeur du monde. Vous trouverez ci-dessous une vue d’ensemble complète de la fonctionnalité et de son utilisation :

## <a name="requirements"></a>Configuration requise

1. Vous devez utiliser un PC ou un Mac pour diffuser votre navigateur.
2. L’extension de navigateur nécessaire est actuellement prise en charge par le navigateur Edge. (Nous travaillons pour développer cette liste.)
3. Si vous pouvez diffuser en continu à partir d’un ordinateur Mac, le projecteur Web n’est pas encore disponible dans le client Mac AltspaceVR.
4. Si tout est correctement configuré (connecté à l’extension de navigateur/AltspaceVR avec le même compte, connecté/diffusé avec le projecteur Web dans AltspaceVR) et que vous voyez toujours un écran vert, webprojecter a besoin du port TCP 443 ouvert et de la plage de ports UDP 20000-20400.

> [!NOTE]
> Cette fonctionnalité est principalement conçue pour diffuser un onglet de navigateur de votre choix. Si vous tentez de diffuser en continu votre application de bureau, le projecteur Web diffuse en continu toutes les données audio de l’ordinateur (y compris AltspaceVR), ce qui peut générer des échos et des commentaires. Vous devez désactiver AltspaceVR pour éviter ce problème. Vous pouvez également utiliser un autre appareil pour exécuter AltspaceVR pendant que vous diffusez en continu à partir de votre ordinateur.

## <a name="getting-started"></a>Prise en main

1. Pour commencer, vous devez télécharger et installer l’extension de navigateur, qui se trouve [ici](https://account.altvr.com/web_projector).
2. Ensuite, [chargement votre extension dans votre navigateur Edge](https://docs.microsoft.com/microsoft-edge/extensions-chromium/getting-started/extension-sideloading).
    * Une fois le téléchargement terminé, accédez à la section **Extensions** de votre navigateur. (trouvé sous **Paramètres**)
    * Décompressez le fichier .zip.
    * Basculer en **mode développeur** et sélectionner **charger décompressé**
    * Choisissez le dossier que vous venez de décompressé. Il s’agit de l’extension de projecteur Web.
    * Une fois votre extension ajoutée, vous pouvez accéder à des **Détails** pour configurer vos paramètres.

## <a name="setting-up-a-shareable-browser"></a>Configuration d’un navigateur partageable

Une fois votre extension téléchargée et installée, vous êtes prêt à l’utiliser !

1. Ouvrez un onglet dans votre navigateur Edge et accédez au média que vous souhaitez partager.
2. Configurez votre fenêtre pour que vous soyez prêt à partager. (Remarque : la totalité de la fenêtre du navigateur sera projetée dans le monde entier)
3. Recherchez l’extension qui vient d’être installée (qui s’affiche sous la forme d’une icône de AltspaceVR près de votre barre d’URL dans votre navigateur). Sélectionnez AltspaceVR. Vous serez invité à vous connecter à votre compte. (* Remarque : il est important que vous vous connectiez au même compte que celui que vous utiliserez pour configurer votre projecteur Web.)
4. Une fois que vous êtes connecté, l’écran extension vous offre une option **Démarrer la diffusion en continu** . Sélectionnez-le.

## <a name="projecting-your-browser-in-world"></a>Projection de votre navigateur dans le monde entier

1. Une fois que votre navigateur est configuré pour la projection et que vous avez commencé la diffusion en continu par le biais de l’extension, ouvrez AltspaceVR.
2. Configurez le projecteur Web dans l’environnement de votre choix en ouvrant votre éditeur World > principes fondamentaux > projecteur Web
3. Une fois que vous avez placé, vous pouvez utiliser vos contrôles d’éditeur de monde pour redimensionner le projecteur Web. (Elle inclut également des instructions, à l’écran).
4. sélectionnez le bouton **Connecter** pour démarrer la diffusion en continu de votre navigateur Edge.
5. N’oubliez pas de cliquer sur **diffusion** pour commencer à partager avec tous les invités dans l’espace.
6. N’oubliez pas d' **arrêter la diffusion en continu.** Le délai d’expiration de votre session est dépassé, mais jusqu’à ce qu’elle continue à s’exécuter en temps réel dans votre navigateur. Il est préférable de mettre fin à votre session dès que vous avez terminé.

![Navigateur projeté dans AltspaceVR World](images/web-project-img-01.png)

**Astuce de diffusion vidéo :** Si la vidéo subit des interruptions, arrêtez la diffusion, réglez la qualité vidéo sur 480p ou 360p, puis redémarrez votre flux et votre diffusion. Des résolutions plus élevées peuvent décharger le processeur et la bande passante de téléchargement.

> [!NOTE]
> À ce stade, les autres boutons de contrôle situés en haut du projecteur Web ne sont pas encore en ligne. Ils restent gris et ne peuvent pas être cliqués. Ce n’est pas un bogue, c’est par conception (pour l’instant).

> [!IMPORTANT]
> exclusion de responsabilité : remarque : l’utilisation du projecteur Web, comme toutes les autres fonctionnalités de AltspaceVR, est soumise aux [conditions de Service](../community/terms-of-service.md) et à nos [normes de Community](../community/community-standards.md). Par conséquent, le projecteur Web ne peut pas être utilisé pour diffuser du contenu qui n’est pas conforme à l’un ou l’autre des accords. Cela entraînera des actions de modération effectuées par AltspaceVR. L’accès au projecteur Web Open Beta n’est pas garanti et peut uniquement être accordé pour une version d’évaluation temporaire. La durée de la version bêta et la durée de votre participation sont à la discrétion de l’équipe AltspaceVR. L’utilisation de la version bêta du projecteur Web n’est pas obligatoire et la participation à la version bêta est purement volontaire. Les participants sont encouragés à proposer des commentaires sur le projecteur Web qui contribueront à la mise en forme des fonctionnalités et de l’utilisation de la fonctionnalité à mesure que le développement se poursuit. La version bêta du projecteur Web peut avoir des fonctionnalités limitées et peut faire l’objet de bogues inattendus. Merci, à l’avance, de votre participation.
