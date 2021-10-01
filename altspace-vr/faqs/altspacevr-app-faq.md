---
title: Forum aux questions sur l’application AltspaceVR
description: Dépannage et prise en charge de l’application AltspaceVR.
ms.date: 8/16/2021
author: qianw211
ms.author: v-qianwen
ms.topic: article
keywords: VR, AltspaceVR, dépannage, support
ms.openlocfilehash: a0df1e100ef8511fe3c9129548529577964c2336
ms.sourcegitcommit: 5c452a9092297c0bfbc8efabebf395e7ee31853f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/30/2021
ms.locfileid: "129311865"
---
# <a name="frequently-asked-questions-about-the-altspacevr-app"></a>Forum aux questions sur l’application AltspaceVR

## <a name="finding-the-altspacevr-app-version"></a>Recherche de la version de l’application AltspaceVR

Au cours de la résolution d’un problème, vous pouvez être invité à indiquer la version de l’application AltspaceVR en cours d’exécution.

### <a name="in-altspacevr"></a>Dans AltspaceVR

Pour trouver la version de l’application dans AltspaceVR, accédez au **menu paramètres** et sélectionnez **à propos** de dans la barre de navigation de gauche. La version de l’application est indiquée ici, comme indiqué dans la capture d’écran ci-dessous.

![Paramètres menu ouvert avec à propos du panneau ouvert](images/app-version-img-01.png)

### <a name="in-windows-system-settings"></a>dans Windows Paramètres système

si vous avez installé AltspaceVR via la Microsoft Store, vous pouvez également trouver la version de l’application dans les paramètres du système Windows.  Ce scénario est adapté lorsque vous signalez la version de l’application si vous ne parvenez pas à vous connecter au client.

pour trouver la version de l’application dans Windows paramètres système, ouvrez le **Menu démarrer**, tapez **applications & fonctionnalités**, puis sélectionnez le résultat. Accédez à **AltspaceVR** dans la liste des applications. Cliquez sur AltspaceVR et sélectionnez **Options avancées** dans le menu qui s’affiche.

![Menu applications et fonctionnalités ouvert avec l’option avancé mise en surbrillance](images/app-version-img-02.png)

Dans les **Options avancées**, sous l’en-tête **spécifications** , la version de l' **application** doit figurer à droite de l’étiquette **version** .

![Options avancées ouvertes avec la version de l’application mise en surbrillance](images/app-version-img-03.png)

### <a name="app-version-in-client-logs"></a>Version de l’application dans les journaux client

AltspaceVR signale la version de l’application dans le fichier journal du client en tant que « version Altspace » au démarrage de l’application. Il s’agit d’une bonne option pour obtenir la version de l’application si vous ne parvenez pas à vous connecter au client, mais qu’elle a tenté de démarrer avant d’échouer.

### <a name="windows"></a>Windows

sur Windows, le fichier journal du client est accessible via Windows Explorer à l’adresse suivante :

```
%userprofile%\AppData\LocalLow\Microsoft\AltspaceVR\Player.log
%userprofile%\AppData\LocalLow\Microsoft\AltspaceVR\Player-prev.log
```

Ce fichier est remplacé chaque fois que vous lancez AltspaceVR. 'Player. log’représente la dernière session et’Player-PREV. log’représente la session précédente.

### <a name="via-powershell"></a>Via PowerShell

Les utilisateurs avancés peuvent rechercher cette chaîne dans les journaux du client à l’aide de PowerShell comme suit :

Entrée :

```
gc $env:userprofile\appdata\locallow\altspacevr\altspacevr\Player.log | ? { $_ -match "Altspace Version" }
```

Sortie :

[2,047] version de AltspaceVR : 3.2.23. e66c2

## <a name="how-do-i-upload-my-client-logs"></a>Comment faire télécharger mes journaux client ?

L’application cliente AltspaceVR conserve un journal des données de diagnostic et des événements qui se produisent lorsque vous utilisez AltspaceVR. Au cours de la résolution d’un problème, il se peut que vous soyez invité à « télécharger vos journaux » pour que notre équipe puisse les passer en revue. Il s’agit d’une fonctionnalité de AltspaceVR qui vous permet d’envoyer à notre équipe votre contenu de journal local pour nous aider à résoudre le problème.

### <a name="in-altspacevr"></a>Dans AltspaceVR

Pour télécharger les journaux du client dans AltspaceVR, accédez au **menu paramètres** et sélectionnez **prise en charge** dans la barre de navigation de gauche. Plusieurs options de téléchargement des journaux sont disponibles ici, comme indiqué dans la capture d’écran ci-dessous.

![menu Paramètres avec le volet de support ouvert et les champs de journal mis en surbrillance](images/help-altvr-uploadlogs.png)

### <a name="fields"></a>Champs

**« Que s’est-il passé ? »**
Décrivez ce qui s’est passé : par exemple, si vous trouvez un bogue, décrivez ce que vous attendiez à ce qu’il s’est effectivement produit. Ces informations sont envoyées avec le journal lorsque vous appuyez sur Télécharger.

**« journaux de Télécharger »** Ce bouton permet de charger les journaux à partir de la session active. Utilisez cette option si vous rencontrez un problème dans cette même session (par exemple, si vous n’avez pas fermé le client AltspaceVR) et que vous souhaitez le signaler.

**« Télécharger les derniers journaux »** Ce bouton permet de charger les journaux à partir de la session précédente.

**« Télécharger dernier journal des incidents »** Ce bouton permet de charger plus de contenu du journal à partir de l’incident le plus récent que vous avez rencontré.

### <a name="in-client-logs"></a>Dans les journaux client

Vous pouvez également récupérer vos fichiers journaux à partir de votre ordinateur. Vous trouverez des instructions sur la récupération de ces journaux [ici](#app-version-in-client-logs).


Une fois que vous avez localisé ces fichiers, [ouvrez un ticket de support](https://help.altvr.com/hc/en-us/requests/new) et chargez vos journaux sur votre demande de ticket avant de cliquer sur Envoyer.

## <a name="what-do-i-do-if-i-cant-launch-altspacevr"></a>Que dois-je faire si je ne peux pas lancer AltspaceVR

Il existe plusieurs raisons pour lesquelles AltspaceVR peut ne pas s’exécuter pour vous. Essayez les étapes suivantes pour vous assurer que l’application est installée correctement avec les logiciels tiers nécessaires.

### <a name="if-youre-trying-to-launch-altspacevr-for-the-first-time"></a>Si vous essayez de lancer AltspaceVR pour la première fois :

1. Vérifiez que votre appareil est pris en charge et répond à la [Configuration minimale requise spécifiée](../getting-started/system-requirements.md).
2. assurez-vous que le dernier [logiciel Oculus](https://www.oculus.com/setup) est installé et que Paramètres > général-> périphériques inconnus est défini sur activé. Si vous lancez en mode 2D, Oculus n’est pas nécessaire.
3. Vérifiez que vous disposez d’une connexion Internet opérationnelle. Si vous essayez de lancer Altspace à partir d’un pare-feu réseau, ouvrez les ports UDP 5055 et 5056, ainsi que les ports TCP 80 et 443. Si vous vous trouvez dans le réseau d’un pare-feu d’entreprise ou d’éducation, vous devrez peut-être contacter l’administrateur réseau ou le service informatique.
4. Voir aussi :
    * [Installation de AltspaceVR pour Oculus Quest](../getting-started/oculus-installation.md)
    * [Installation de AltspaceVR pour Windows Mixed Reality](../getting-started/wmr-installation.md)

### <a name="if-altspacevr-reports-that-the-current-version-is-out-of-date"></a>Si AltspaceVR signale que la version actuelle est obsolète :

* La version de l’application que vous utilisez n’est plus prise en charge. Si vous avez téléchargé AltspaceVR dans une vitrine, la mise à jour a peut-être été lancée récemment avant que votre magasin ait pu mettre à jour votre client.
* Si vous souhaitez forcer la mise à jour, vous pouvez le faire via les différentes vitrines :
    * **Microsoft Store :** [Microsoft Store Support-obtenir des mises à jour pour les applications et les jeux dans Microsoft Store](https://support.microsoft.com/account-billing/get-updates-for-apps-and-games-in-microsoft-store-a1fe19c0-532d-ec47-7035-d1c5a1dd464f)
    * **Oculus :** Ouvrez votre bibliothèque Oculus et accédez à « mises à jour » dans la barre de navigation de gauche.
    * **Vapeur :** [support à la vapeur-mettre à jour & problèmes d’installation](https://support.steampowered.com/kb_article.php?ref=2274-IFLV-5334)

### <a name="if-the-program-was-working-but-ceased-to-launch-after-update"></a>Si le programme fonctionnait, mais a cessé de s’exécuter après la mise à jour :

* Effectuez une nouvelle réinstallation du logiciel. Cela nécessite la désinstallation ou la suppression des versions existantes de l’application. Une fois entièrement supprimé de votre système, installez Altspace via Steam, Oculus ou Microsoft Store.
* Si vous rencontrez un problème lors du lancement de AltspaceVR, faites-le nous savoir via un [ticket de support](https://help.altvr.com/hc/requests/new). Incluez un [fichier journal](altspacevr-app-faq.md#how-do-i-upload-my-client-logs) de votre session.

### <a name="if-altspacevr-fails-to-launch-after-customizing-your-home-space"></a>Si AltspaceVR ne parvient pas à démarrer après avoir personnalisé votre espace d’hébergement :

* Accédez au [site Web de votre espace de bureau](https://account.altvr.com/users/sign_in).
* Vérifiez que le modèle de votre monde existe toujours. Si le modèle a été partagé avec vous, il a peut-être été supprimé par le propriétaire, ce qui entraînerait l’échec du chargement de votre espace d’origine.
    * Si le modèle a été supprimé, il vous suffit de « modifier » le monde dans le panneau « Outils de l’environnement » de gauche, de remplacer le modèle existant par un autre modèle et de « mettre à jour » pour enregistrer les modifications.
* Supprimez les objets susceptibles de ne pas pouvoir être chargés en sélectionnant « objets » dans le panneau de gauche « outils du monde ». Les objets problématiques peuvent inclure :
    * Objets des kits supprimés, ou objets supprimés des kits, qui sont toujours présents dans votre monde.
    * GLTFs expérimental.
* Après avoir traité les éléments ci-dessus, essayez de saisir à nouveau AltspaceVR.

Pour plus d’informations sur la prise en charge des administrateurs réseau ou des services informatiques, y compris les plages d’adresses IP et les balises de service Azure, consultez les [Détails du téléchargement](https://www.microsoft.com/en-us/download/details.aspx?id=56519).

## <a name="support"></a>Support

Vous avez des questions ou des commentaires pour l’équipe AltspaceVR ? 

> [!div class="nextstepaction"]
> [Cliquez ici pour envoyer une demande de support](https://help.altvr.com/hc/requests/new)