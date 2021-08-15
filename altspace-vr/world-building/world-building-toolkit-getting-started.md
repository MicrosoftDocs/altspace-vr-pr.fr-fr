---
title: présentation du Shared Computer Toolkit de la construction mondiale
description: apprenez à configurer et à télécharger vos mondes AltspaceVR à l’aide de modèles de scène unity avec le Shared Computer Toolkit de construction mondial.
ms.date: 03/11/2021
ms.topic: article
keywords: Phone
ms.openlocfilehash: 8b66e35509060e00b2e52d3770380d009d7060339003f534d23fdd47372a57f0
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/11/2021
ms.locfileid: "119125404"
---
# <a name="introducing-the-world-building-toolkit"></a>présentation du Shared Computer Toolkit de la construction mondiale

> [!NOTE]
> le monde immeuble Shared Computer Toolkit est un projet communautaire exécuté par notre amie, [Anthony Madden](https://twitter.com/chigamesstudio), avec la prise en charge de notre part. Si vous êtes intéressé, participez au [AltspaceVR officiel](https://discordapp.com/invite/altspacevr) et visitez le canal de construction #world. Nous disposons actuellement d’une version bêta de Mac pour l’instant, [plus de détails](https://altvr.com/altspacevr-mac)

Le chargeur vous permet d’utiliser une scène Unity comme modèle pour vos mondes. Vous pouvez mettre en place une maison hanté pour Halloween ou la création de vos favoris à partir de Minecraft. Si vous pouvez l’importer dans Unity, vous pouvez probablement le faire Altspace de cette façon. Voici quelques exemples de [mondes](https://account.altvr.com/worlds/1046572460192825569).

![Exemples de mondes](images/unity-uploader-img-01.png)

## <a name="setup"></a>Installation

1. Rejoignez le [AltspaceVR officiel](https://discordapp.com/invite/altspacevr) et visitez le #world-les amis de la création de canaux ne permettent pas aux amis de créer des mondes uniquement.
2. Lisez notre [Guide de prise en main international](world-building-getting-started.md) pour les principes de base
3. [Installez Unity Hub](https://blogs.unity3d.com/2018/01/24/streamline-your-workflow-introducing-unity-hub-beta) et installez **Unity 2020.3.9**. Le téléchargeur ne fonctionne pas, sauf si vous faites correspondre exactement cette version. Si vous n’en avez pas, vous aurez besoin d’un compte Free Unity, si vous n’en avez pas et si vous **le souhaitez.** Pendant l’installation, vérifiez que l’option **Builds Android** est cochée et désactivez la mise à jour automatique.
4. [Téléchargez le dernier chargeur Unity](upgrading-content-to-the-latest-unity.md#altspacevr-uploader-v090-upgrade-guide)
5. [Créez un modèle](https://account.altvr.com/space_templates/new) sur notre site Web. Nommez-le **Hello World modèle**.
6. [Créez un monde](https://account.altvr.com/worlds/my) et nommez-le **Hello World**. Sélectionnez **Hello World modèle** comme modèle.

![Écran du monde créé](images/unity-uploader-img-02.png)

## <a name="upload-your-scene"></a>Télécharger votre scène

> [!VIDEO https://channel9.msdn.com/Shows/Docs-Mixed-Reality/How-to-upload-a-Template/player]

1. Ouvrez Unity Hub et créez un nouveau projet Unity 2020.3.9.
2. Une fois votre projet ouvert, importez le programme de chargement en double-cliquant sur le fichier que vous avez téléchargé (il s’agit d’un package Unity). Vous devez maintenant voir un nouvel onglet appelé **AltspaceVR**. Vous devez importer le package pour chaque projet Unity que vous souhaitez utiliser avec Altspace
3. ouvrez le **Menu > AltspaceVR > Build Paramètres**
4. Connectez-vous avec vos informations d’identification de compte Altspace
5. Sélectionnez **charger les modèles** , puis sélectionnez **Hello World modèle** .
6. Ajoutez un cube à votre scène et enregistrez.
7. vérifier la **build pour Windows ?** et décocher **générer pour Android ?**
8. Sélectionnez **Télécharger**. en environ une minute, vous devriez voir **Télécharger** terminé.
9. Rejoignez **Hello World** en lançant Altspace et en entrant à partir de **Menu > mondes > mes mondes**
10. réinitialiser le monde à partir du **Menu > Paramètres > l’espace de réinitialisation modérée >**
11. Le cube doit s’afficher. Si vous le faites rapidement comme dans la vidéo ci-dessus, vous pouvez voir les modifications en moins de 10 secondes.

## <a name="whats-supported"></a>Opérations prises en charge

* Oui : modèles, collisions, animations, effets de particules, audio, skyboxes, etc.
* Non : scripts. Pour des raisons de sécurité, les chargements contenant des scripts sont rejetés
* Peut-être : des éléments fantaisie tels que l’éclairage global dynamique
* Télécharger des scènes pour différentes plateformes séparément ou ensemble
* Découvrez les [mondes proposés](https://account.altvr.com/worlds/featured), nombreux ont été créés à l’aide du chargeur

## <a name="tips"></a>Conseils

* Participez au [décordon AltspaceVR officiel](https://discordapp.com/invite/altspacevr).
* Sur la page du modèle sur le côté gauche, nous vous montrons les derniers téléchargements par plateforme. En cas de réussite, il y a **1-2 minutes**. Screen_Shot_2019-01-11 _at_1.21.04_AM.png

![Volet modèles ouvert avec les chargements mis en surbrillance](images/unity-uploader-img-03.png)

* Vous pouvez être dans le monde lorsque vous mettez à jour. le moment où le téléchargeur indique **Télécharger terminé** , vous pouvez réinitialiser le monde pour voir les modifications.
* La création d’un PC avec une scène simple prend moins d’une minute pour voir une modification dans Altspace
* Définissez votre monde comme privé et dérépertorié pour éviter les distractions.
* Placez un cube à l’origine pour voir où les gens seront générés par défaut. Masquez le cube lors du téléchargement.

## <a name="troubleshooting"></a>Résolution des problèmes

**Je suis en chute ou ne peut pas se téléporter sur quoi que ce soit** Vous devez ajouter des collisions à des objets pour les réutiliser.

**Rien n’a changé**
    * Avez-vous enregistré la scène dans Unity ?
    * Avez-vous choisi la plateforme sur laquelle vous effectuez le test ?
    * Êtes-vous dans le monde ? Avez-vous choisi le modèle approprié dans le chargeur et dans le formulaire ?
    * Avez-vous vérifié les statistiques de page de modèle ?

**Télécharger échoue ou expire**
    * L’erreur de chargement la plus courante est la mauvaise version d’Unity. Il doit correspondre exactement à la version requise.
    * Le chargement est peut-être trop important. Essayez de conserver les scènes de PC < 100 Mo. Commencez petit et de Build. Optimisation, optimisation, optimisation.
    * Essayez avec un nouveau projet avec un cube simple.
    * Ne pas forcer la fermeture pendant une génération : elle peut endommager votre scène. Essayez de relancer le téléchargement.

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
