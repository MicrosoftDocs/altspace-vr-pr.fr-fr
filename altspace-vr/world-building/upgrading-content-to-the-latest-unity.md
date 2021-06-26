---
title: Mise à jour du contenu vers la dernière version Unity
description: Découvrez comment mettre à jour votre contenu vers la dernière version d’Unity.
ms.date: 06/4/2021
ms.topic: article
keywords: kits, mondes, Unity, mise à jour, nuanceurs, téléchargeur, résolution des problèmes
ms.openlocfilehash: f8a805c4b3350f2c97c43d3d48c35733ec7e9710
ms.sourcegitcommit: 2db596ab5a1ecd4901a8c893741cc4d06f6aecea
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2021
ms.locfileid: "112961222"
---
# <a name="updating-content-to-the-latest-unity-version"></a>Mise à jour du contenu vers la dernière version Unity

## <a name="moving-to-unity-202039"></a>Déplacement vers Unity 2020.3.9

À partir de maintenant, AltspaceVR a été mis à niveau vers une version récente d’Unity (2020.3.9). En plus de certaines améliorations de performances, cette mise à jour a pour but de nous assurer que nous sommes ravis d’intégrer les fonctionnalités à venir. Cette modification doit être compatible avec tout le contenu existant. Si ce n’est pas le cas, n’hésitez pas à contacter le support technique : altvr.com/support

Bien que ce déplacement vers 2020.3.9 n’ait pas affecté le contenu généré par l’utilisateur, dans quelques semaines, nous apportons une modification au [mode de rendu stéréo de AltspaceVR qui obligera les utilisateurs à mettre à jour leur contenu]( https://docs.unity3d.com/Manual/SinglePassStereoRendering.html). Cette mise à niveau vers l' [instanciation à passage unique](https://docs.unity3d.com/Manual/SinglePassInstancing.html) permet d’améliorer considérablement les performances de vos mondes. N’oubliez pas que cette nouvelle build ne prend plus en charge la compatibilité descendante avec le contenu de 2019,4 et les versions antérieures. Il est urgent que tout le contenu détenu par le créateur soit mis à jour dès que possible pour éviter toute modification avec rupture. Suivez le guide ci-dessous pour mettre à jour votre contenu et garantir une transition en douceur vers l’instanciation à passage unique sur Unity 2020.3.9.

> [!NOTE]
> Si vous utilisez régulièrement du contenu qui est détenu par quelqu’un d’autre et qui a été partagé avec vous, contactez le propriétaire du monde entier et assurez-vous qu’il envisage de mettre à jour son contenu.

> Si vous êtes un créateur de contenu et que vous avez des questions ou besoin d’aide, contactez notre équipe de support technique pour obtenir de l’aide : altvr.com/support

## <a name="testing-your-spi-content"></a>Test de votre contenu SPI

Utilisez les versions préliminaires suivantes de AltspaceVR pour tester votre contenu récemment mis à jour en VR. Les versions préliminaires sont à des fins de test uniquement et ne doivent pas être utilisées pour une utilisation générale de la plateforme.

* [AltspaceVR SPI Preview pour Windows Mixed Reality](https://aka.ms/AvrSpiMr)
* [AltspaceVR SPI Preview pour SteamVR](https://aka.ms/AvrSpiSteam)
* [AltspaceVR SPI Preview pour le rift Oculus](https://aka.ms/AvrSpiRift)

> Remarque : seules les préversions de PC VR ont été fournies. Le rendu d’instance à passage unique n’est pas disponible sur Android et n’est pas nécessaire sur les plateformes non-VR comme Mac. Ainsi, vous pouvez utiliser la version générale pour tester ces appareils.


## <a name="storecompatibilitycheck"></a>Vérification de la compatibilité du magasin

La mise à niveau vers Unity 2020.3.9 affecte également la compatibilité du casque et de la build de magasin. Vous devez maintenant télécharger AltspaceVR à partir du Windows Store qui est compatible avec votre casque. Par exemple : pour un casque WinMR ou Oculus, téléchargez AltspaceVR à partir du Windows Store ou du magasin Oculus, respectivement. Les utilisateurs de Windows Mixed Reality doivent télécharger AltspaceVR à partir du Windows Store, des utilisateurs SteamVR à partir de la vapeur et des utilisateurs Oculus.

## <a name="altspacevr-uploader-v090-upgrade-guide"></a>Guide de mise à niveau de AltspaceVR TELECHARGER v 0.9.0 

Le chargeur 0,9 est empaqueté différemment des versions précédentes du chargeur. Simultanément avec cette modification de Packaging, le nouveau téléchargeur requiert une nouvelle version d’Unity. Ce guide est conçu pour rendre ce processus de mise à niveau plus lisse et plus sûr pour tous ceux qui sont impliqués.

1. **Sauvegarder votre projet** : créez une copie de l’intégralité de votre répertoire de projet et mettez-la à un endroit sûr. Cette mise à niveau est une mise à niveau destructrice. vous ne pourrez donc pas créer ou charger des offres groupées pour Unity 2019,4 une fois celle-ci terminée. Si vous rencontrez des problèmes pendant cette mise à niveau, vous aurez besoin d’une copie propre de votre projet pour revenir en arrière. Vous en aurez également besoin pour mettre à jour les kits ou modèles actifs avant que AltspaceVR ne soit officiellement mis à niveau vers Unity 2020.3.9.

2. **Supprimer l’ancien** téléchargeur : avec Unity fermé, supprimez les fichiers/dossiers suivants, et les fichiers. meta correspondants :

    ```console
    * Assets/Altspace

    * Assets/Plugins

    * Assets/Prefabs/test-folder, Readme.txt

    * Assets/Resources/bg.jpeg, bg2.jpeg, logo.png, UserPreferences.asset

    * Assets/DFloor_v004.fbx

    * Library (This is a Unity system folder, not an Uploader folder. Delete it anyway, and let it be rebuilt during the upgrade.)
    ```

3. **Version du moteur de téléchargement** : Ouvrez Unity Hub et installez Unity 2020.3.9 (ou [cliquez ici](https://unity3d.com/ru/unity/whats-new/2020.3.9) pour installer directement).

4. **Mettre à niveau le projet** : Ouvrez votre projet nettoyé dans Unity 2020.3.9 et autorisez Unity à mettre à niveau votre projet.

5. (PC uniquement) **Outil de téléchargement de la fonctionnalité de réalité mixte** : suivez les instructions pour télécharger l’outil de la [fonctionnalité de réalité mixte](/windows/mixed-reality/develop/unity/welcome-to-mr-feature-tool), que vous utiliserez pour gérer l’installation du package du téléchargeur.

6. **Installer le** téléchargeur : utilisez l’outil de fonctionnalité Mr pour sélectionner votre projet Unity, puis ajoutez la fonctionnalité AltspaceVR TELECHARGER (sous l’en-tête AltspaceVR). Suivez les instructions de l’outil.

Sur macOS, téléchargez manuellement la dernière version à partir du [Registre](https://dev.azure.com/aipmr/MixedReality-Unity-Packages/_packaging?_a=package&feed=Unity-packages&package=com.microsoft.altspacevr_uploader&protocolType=Npm&version=0.9.0&view=versions)et installez-la à partir du gestionnaire de package de l’éditeur Unity (Windows > package Manager > + > ajouter un package à partir de tarball).

Une fois l’importation du package terminée, la fenêtre de chargeur familière doit être disponible dans l’élément de menu AltspaceVR.

## <a name="troubleshooting-tips"></a>Conseils de dépannage

1. Si vous rencontrez des problèmes de contrôleur ou d’entrée sur votre casque WinMR, assurez-vous qu’il est positionné sur votre tête pour faire fonctionner correctement le capteur de présence. Il s’agit d’un problème connu et Microsoft travaille activement à le résoudre.

2. Vérifiez la compatibilité de votre casque et de la build de magasin. Si vous utilisez un casque WinMR, par exemple, assurez-vous que votre Build AltspaceVR a été acquise par le biais du Windows Store.

3. Si, au cours du test, vous découvrez que votre contenu ne s’affiche que dans un seul œil en mode VR, il est probable que les nuanceurs personnalisés que vous utilisez ne prennent pas en charge le rendu SPI. Vous devez choisir un autre nuanceur ou suivre le [Guide de mise à niveau SPI d’Unity](https://docs.unity3d.com/Manual/SinglePassInstancing.html) pour modifier manuellement le nuanceur et ajouter la prise en charge.

4. Pour ceux sur WinMR, n’oubliez pas que pour pouvoir accéder au mode VR dans AltspaceVR, vous devez : 
    1. Téléchargez et installez OpenXR pour Windows Mixed Reality à partir de la Microsoft Store.
        1. Ouvrir l’application portail de réalité mixte
        2. Dans le coin inférieur gauche de l’application, sélectionnez « voir plus »
        3. Dans le menu qui s’affiche, sélectionnez configurer OpenXR. Cela entraîne le lancement du Windows Store à partir duquel vous pouvez installer le Runtime. Si cet élément de menu n’apparaît pas, OpenXR est peut-être déjà installé sur votre PC.