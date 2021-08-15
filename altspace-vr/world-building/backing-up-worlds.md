---
title: Sauvegarde de vos mondes
description: Découvrez comment créer, gérer et dépanner des instantanés de sauvegarde de vos mondes AltspaceVR.
ms.date: 03/11/2021
ms.topic: article
keywords: enregistrer
ms.openlocfilehash: 2f4f232fd843b612563b2d7425de2b5d17720c539cc02a1493bc4b118de4f117
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/11/2021
ms.locfileid: "119125467"
---
# <a name="backing-up-your-worlds"></a>Sauvegarde de vos mondes

Une sauvegarde est un « instantané » ou un enregistrement de tous les objets d’un monde à un point spécifique dans le temps. Supposons que vous soyez en train de créer votre maison de rêve et un jour où vous avez accidentellement supprimé le salon. Si vous aviez créé une sauvegarde de votre monde le jour qui précède, vous pouviez restaurer cette sauvegarde spécifique, réinitialiser votre monde et éviter une attaque par panique. Ou peut-être avez-vous une version de votre cabine-en-dessous pour chaque saison et que vous souhaitez basculer entre elles, vous pouvez le faire avec les sauvegardes. Chaque sauvegarde est spécifique à un seul monde et contient non seulement les transformations (position, rotation, échelle), mais également d’autres paramètres sur les objets. Il n’existe aucune limite quant au nombre de sauvegardes que vous pouvez créer pour un monde.  

## <a name="whats-included-in-a-backup"></a>Qu’est-ce qui est inclus dans une sauvegarde ?

Une sauvegarde contient actuellement la plupart des éléments que vous pouvez générer avec l’éditeur de monde :
* Artifacts (objets de Kit)
* Étiquettes
* Téléporteurs
* Points de génération
* Photo
* Applications SDK MRE
* applications natives (par exemple, Hologrammes contre la réalité)

Les éléments suivants ne sont pas inclus :

* Remplacements de la disposition
* Skyboxes et son ambiant
* Modèles
* Instructions
* Rôles mondiaux et rôles contextuels

## <a name="managing-backups"></a>Gestion des sauvegardes

Vous pouvez créer une sauvegarde en ouvrant votre éditeur de monde/Altspace et en cliquant sur « sauvegardes ». Le premier bouton est le bouton « nouvelle sauvegarde ». Lors de la création d’une sauvegarde, vous êtes invité à fournir un nom abrégé. Cette option est facultative, mais vivement recommandée, car elle peut être déroutante rapidement. Les sauvegardes existantes seront listées après le bouton « créer ». Cliquez sur une sauvegarde existante pour démarrer une restauration. Lors de la restauration d’une sauvegarde, votre monde se réinitialise après quelques instants, mais vous risquez de ne pas voir les modifications reflétées. Attendez une minute ou deux et réinitialisez votre monde. **Il n’existe actuellement aucun moyen de modifier ou de supprimer une sauvegarde en VR**. Pour l’instant, vous devez gérer vos sauvegardes sur notre site Web. (La gestion des sauvegardes en VR sera bientôt améliorée. En attendant, nous nous engageons).

Pour gérer vos sauvegardes sur notre site Web :

1. Accédez à [mondes > mien](https://account.altvr.com/users/sign_in), recherchez votre monde, puis appuyez sur « sauvegardes » dans les contrôles administrateur :

![Contrôles administrateur sur le site Web des mondes avec le volet sauvegardes ouvert](images/world-backup-img-01.png)

2. Vous pouvez créer, modifier et supprimer vos sauvegardes, vérifier le nombre d’objets qui se trouvent dans et même charger une image d’aperçu : 

![Fenêtre sauvegardes avec les commandes créer, modifier et supprimer mises en surbrillance](images/world-backup-img-02.png)

Il n’y a pas de limite au nombre de sauvegardes et le fait d’avoir plus de sauvegardes n’aura pas d’impact sur les performances de votre monde.

## <a name="other-ways-to-back-up-your-worlds"></a>Autres moyens de sauvegarder vos mondes

* Créez un autre environnement, affichez les options avancées et importez à partir de tout le monde. Choisissez le monde que vous souhaitez sauvegarder dans le menu déroulant dans le nouveau. Aucune limite n’est définie pour les importations.
* Si vous utilisez le chargeur Unity, nous vous recommandons vivement d’utiliser le contrôle de version. Par exemple, [GitHub pour Unity](https://unity.github.com).

## <a name="troubleshooting"></a>Résolution des problèmes

**Aide ! J’ai restauré accidentellement une sauvegarde et mon travail n’a** pas de crainte. Nous créons automatiquement une nouvelle sauvegarde avant la restauration de l’ancienne. Recherchez-en un dont le nom commence par **auto** avec l’horodateur approprié et restaurez celui-ci (par exemple, **auto-01-14T08:23:33-08:00**).  Si cela ne fonctionne pas, envoyer un [support Request](https://help.altvr.com/hc/requests/new)

**J’ai restauré une sauvegarde et certains objets sont manquants** Si vous avez des photos, ces photos ont-elles été supprimées ? Nous ne pouvons pas restaurer les photos supprimées pour des raisons de confidentialité. Envoyer un [support Request](https://help.altvr.com/hc/requests/new) pour pouvoir examiner

**Je ne vois aucune modification** Les sauvegardes sont restaurées de manière asynchrone, ce qui signifie que la restauration peut prendre quelques minutes en fonction du nombre d’objets. N’oubliez pas de réinitialiser votre environnement et, si vous ne voyez rien après quelques minutes, essayez de réinitialisation. À l’avenir, nous pouvons fournir des commentaires supplémentaires sur l’état du processus de restauration