---
title: Impossible de lancer AltspaceVR
description: Découvrez comment identifier, signaler et résoudre les problèmes liés au lancement de votre environnement AltspaceVR.
ms.date: 02/10/2021
ms.topic: article
keywords: faq
ms.openlocfilehash: fc49b5b7ed708e43a12616d782a397a364b2264e
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/08/2021
ms.locfileid: "107212383"
---
# <a name="i-cant-launch-altspacevr"></a>Impossible de lancer AltspaceVR

Il existe plusieurs raisons pour lesquelles AltspaceVR peut ne pas s’exécuter pour vous. Essayez les étapes suivantes pour vous assurer que l’application est installée correctement avec les logiciels tiers nécessaires.

## <a name="if-youre-trying-to-launch-altspacevr-for-the-first-time"></a>Si vous essayez de lancer AltspaceVR pour la première fois :

1. Vérifiez que votre appareil est pris en charge et répond à la [Configuration minimale requise spécifiée](../getting-started/system-requirements.md).
2. Assurez-vous que le dernier [logiciel Oculus](https://www.oculus.com/setup) est installé et que paramètres-> général-> périphériques inconnus est défini sur activé. Si vous lancez en mode 2D, Oculus n’est pas nécessaire.
3. Vérifiez que vous disposez d’une connexion Internet opérationnelle. Si vous essayez de lancer Altspace à partir d’un pare-feu réseau, ouvrez les ports UDP 5055 et 5056, ainsi que les ports TCP 80 et 443. Si vous vous trouvez dans le réseau d’un pare-feu d’entreprise ou d’éducation, vous devrez peut-être contacter l’administrateur réseau ou le service informatique.
4. Voir aussi :
    * [Installation de AltspaceVR pour Oculus Quest](../getting-started/oculus-installation.md)
    * [Installation de AltspaceVR pour Windows Mixed Reality](../getting-started/wmr-installation.md)

## <a name="if-altspacevr-reports-that-the-current-version-is-out-of-date"></a>Si AltspaceVR signale que la version actuelle est obsolète :

* La version de l’application que vous utilisez n’est plus prise en charge. Si vous avez téléchargé AltspaceVR dans une vitrine, la mise à jour a peut-être été lancée récemment avant que votre magasin ait pu mettre à jour votre client.
* Si vous souhaitez forcer la mise à jour, vous pouvez le faire via les différentes vitrines :
    * **Microsoft Store :** [Microsoft Store support-obtenir des mises à jour pour les applications et les jeux dans Microsoft Store](https://support.microsoft.com/account-billing/get-updates-for-apps-and-games-in-microsoft-store-a1fe19c0-532d-ec47-7035-d1c5a1dd464f)
    * **Oculus :** Ouvrez votre bibliothèque Oculus et accédez à « mises à jour » dans la barre de navigation de gauche.
    * **Vapeur :** [support à la vapeur-mettre à jour & problèmes d’installation](https://support.steampowered.com/kb_article.php?ref=2274-IFLV-5334)

## <a name="if-the-program-was-working-but-ceased-to-launch-after-update"></a>Si le programme fonctionnait, mais a cessé de s’exécuter après la mise à jour :

* Effectuez une nouvelle réinstallation du logiciel. Cela nécessite la désinstallation ou la suppression des versions existantes de l’application. Une fois entièrement supprimé de votre système, installez Altspace via Steam, Oculus ou Microsoft Store.
* Si vous rencontrez un problème lors du lancement de AltspaceVR, faites-le nous savoir via un [ticket de support](https://help.altvr.com/hc/requests/new). Incluez un [fichier journal](uploading-client-logs.md) de votre session.

## <a name="if-altspacevr-fails-to-launch-after-customizing-your-home-space"></a>Si AltspaceVR ne parvient pas à démarrer après avoir personnalisé votre espace d’hébergement :

* Accédez au [site Web de votre espace de bureau](https://account.altvr.com/users/sign_in).
* Vérifiez que le modèle de votre monde existe toujours. Si le modèle a été partagé avec vous, il a peut-être été supprimé par le propriétaire, ce qui entraînerait l’échec du chargement de votre espace d’origine.
    * Si le modèle a été supprimé, il vous suffit de « modifier » le monde dans le panneau « Outils de l’environnement » de gauche, de remplacer le modèle existant par un autre modèle et de « mettre à jour » pour enregistrer les modifications.
* Supprimez les objets susceptibles de ne pas pouvoir être chargés en sélectionnant « objets » dans le panneau de gauche « outils du monde ». Les objets problématiques peuvent inclure :
    * Objets des kits supprimés, ou objets supprimés des kits, qui sont toujours présents dans votre monde.
    * GLTFs expérimental.
* Après avoir traité les éléments ci-dessus, essayez de saisir à nouveau AltspaceVR.

Pour plus d’informations sur la prise en charge des administrateurs réseau ou des services informatiques, y compris les plages d’adresses IP et les balises de service Azure, consultez les [Détails du téléchargement](https://www.microsoft.com/en-us/download/details.aspx?id=56519).