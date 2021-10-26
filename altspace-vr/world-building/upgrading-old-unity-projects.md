---
title: Mise à niveau des anciens projets Unity
description: Découvrez comment mettre à jour votre contenu vers la dernière version d’Unity.
ms.date: 10/19/2021
ms.topic: article
keywords: kits, mondes, Unity, mise à jour, nuanceurs, téléchargeur, résolution des problèmes
ms.openlocfilehash: 06af70164e5bf870a10bf1ee9e949e09dfa69fd2
ms.sourcegitcommit: 8c58f9f9ad1a3f9534141dee2c78e32792d0db7a
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/25/2021
ms.locfileid: "130302390"
---
<a name="upgrading-old-unity-projects"></a>Mise à niveau des anciens projets Unity
=============================

Au fil des années, AltspaceVR a subi plusieurs mises à niveau peu fréquentes nécessitant que les utilisateurs modifient leur contenu. Si vous constatez qu’un modèle ou un kit que vous avez téléchargé dans le passé n’est pas accessible dans la version la plus récente de AltspaceVR, suivez ce guide pour que votre contenu soit de nouveau opérationnel.

> [!NOTE]
> Avant de suivre les étapes de ce guide, vous devez créer une sauvegarde complète de votre projet si la mise à niveau ne se déroule pas correctement. La méthode la plus simple consiste à créer une seconde copie de l’ensemble du dossier du projet. Pour une solution plus avancée, envisagez d’utiliser un système de contrôle de version comme git et GitHub.

<a name="overview"></a>Vue d’ensemble
---------

À la suite de cet article, la version actuelle de AltspaceVR utilise la configuration suivante :

* Moteur de jeu : Unity 2020.3.18 F1 (également acceptable : Unity 2020.3.9 F1)
* Télécharger Outil : téléchargeur 2,2
* Rendu : pipeline de rendu universel (URP)
* Mode stéréo : instanciation de Single-Pass (SPI) ou multivue sur Quest

Si la version de votre projet Unity est antérieure à 2020,3, vous devrez probablement effectuer toutes ces mises à jour à la fois. Suivez ce guide dès le début. Si vous êtes déjà sur Unity 2020,3, mais avec le chargeur 0,9, commencez à l’étape 6.

1. **Sauvegarder votre projet** : créez une copie de l’intégralité de votre répertoire de projet et mettez-la à un endroit sûr. Cette mise à niveau étant une mise à niveau destructrice, vous allez perdre vos fichiers de projet d’origine une fois que vous avez terminé.
    Si vous rencontrez des problèmes pendant cette mise à niveau, vous aurez besoin d’une copie propre de votre projet pour revenir en arrière.

2. **Supprimer l’ancien chargeur** : effectuez cette étape si votre projet utilise le téléchargeur AltspaceVR 0,8 ou une version antérieure. Avec Unity Closed, supprimez les fichiers/dossiers suivants, et les fichiers. meta correspondants. Si le fichier/dossier n’existe pas, ignorez-le.

    * Ressources/Altspace
    * Ressources/plug-ins
    * Ressources/Prefabs/test-Folder
    * Ressources/Prefabs/Readme.txt
    * Ressources/ressources/BG. jpeg
    * Ressources/ressources/BG2. jpeg
    * Ressources/ressources/logo.png
    * Ressources/ressources/UserPreferences. Asset
    * Ressources/DFloor_v004. FBX

3. **Supprimer les éléments** multimédias traités : effectuez cette étape si vous effectuez une mise à niveau vers une nouvelle version Unity. Avec Unity Closed, supprimez le dossier de bibliothèque du projet. Il s’agit d’un dossier système Unity contenant des ressources spécifiques au moteur et des fichiers qui sont générés automatiquement à partir du contenu du dossier de ressources (entre autres choses).

4. **Version du moteur de téléchargement** : effectuez cette étape si vous effectuez une mise à niveau vers une nouvelle version Unity. Ouvrez Unity Hub et installez Unity 2020.3.18 F1 à partir de l’archive de téléchargement ([lien vers le moteur d’installation](unityhub://2020.3.18f1/a7d1c678663c)).
    * si vous créez sur un PC Windows, activez les cases à cocher pour la prise en charge des builds Android et Mac.
    * si vous créez sur un Mac, activez les cases à cocher pour Android et Windows Build Support.

5. **Mettre à niveau le projet** : Ouvrez votre projet nettoyé dans Unity 2020.3.18 F1 et autorisez Unity à mettre à niveau votre projet.
    Cette opération prend du temps.

6. **Télécharger le** téléchargeur : Téléchargez la dernière version du chargeur [ici](https://aka.ms/AvrUrpUploader)et enregistrez-la dans le dossier Packages de votre projet. Ce fichier doit avoir l’extension de fichier « . tgz ».
    > [!NOTE]
    > Si vous utilisez le navigateur Safari pour le téléchargement, il sera automatiquement extrait dans un fichier « . tar », qui ne peut pas être utilisé par Unity. Vous pouvez soit utiliser un autre navigateur pour télécharger, soit utiliser l’utilitaire système « gzip » pour le recompresser.
    
7. **Installer le** téléchargeur : Installez le programme de chargement à partir du gestionnaire de package de l’éditeur Unity :
    1. ouvrez la fenêtre de Gestionnaire de package unity : Windows > Gestionnaire de package
    2. En haut à gauche de la fenêtre, cliquez sur l’icône « + », puis sélectionnez « Ajouter un package à partir de tarball ».
    3. Sélectionnez le fichier tgz que vous avez téléchargé à la dernière étape.
    4. Attendez que Unity décompresse le package.

8. **Ouvrir le** téléchargeur : si l’installation a réussi, un menu « AltspaceVR » est disponible dans la barre supérieure.
    Ce menu contient des fenêtres distinctes pour les kits et les modèles. Ouvrez celui qui convient le mieux à votre projet.
    La première fois que la fenêtre s’ouvre, les paramètres de votre projet sont configurés pour correspondre au client du jeu Altspace : activation du pipeline de rendu universel et instanciation de l' Single-Pass

9. **Corriger les nuanceurs** -pendant que la première installation est en cours d’exécution, une fenêtre PowerShell peut s’afficher temporairement.
    Vous pouvez être invité à mettre à niveau certains des nuanceurs personnalisés/téléchargés. Si vous approuvez l’invite, le script PowerShell tente de mettre automatiquement à niveau les nuanceurs, mais les chances de réussite sont faibles. Vous devrez vérifier manuellement si le nuanceur fonctionne toujours correctement dans URP.

10. **Corriger les matériaux** : certains/tous vos documents peuvent devenir roses/magenta pendant le processus de mise à niveau. Cela indique une erreur dans le nuanceur utilisé par ce matériel. si vous avez utilisé les nuanceurs intégrés unity, vous pouvez généralement les migrer automatiquement vers des nuanceurs compatibles URP à partir du menu : modifier > pipeline de rendu > pipeline de rendu universel > mettre à niveau les documents Project vers les matériaux UniversalRP.

11. **Créer et télécharger** : à ce stade, votre projet doit être entièrement mis à niveau. Suivez les instructions du Guide de [prise en main](world-building-toolkit-getting-started.md) pour générer et charger votre kit/modèle.

<a name="troubleshooting-tips"></a>Conseils de dépannage
---------------------

1. Si vous découvrez que votre contenu ne s’affiche que dans un seul œil en mode VR, il est probable que les nuanceurs personnalisés que vous utilisez ne prennent pas en charge le rendu SPI. Vous devez choisir un autre nuanceur ou suivre le [Guide de mise à niveau SPI d’Unity](https://docs.unity3d.com/Manual/SinglePassInstancing.html) pour modifier manuellement le nuanceur et ajouter la prise en charge.

2. Si vous découvrez que votre contenu est rose/magenta en jeu ou qu’il est totalement invisible, cela peut être dû à l’incompatibilité d’un nuanceur avec URP. Vous devrez soit remplacer le nuanceur, soit le mettre à niveau vous-même.