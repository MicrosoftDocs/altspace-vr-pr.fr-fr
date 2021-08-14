---
title: Recherche de la version de l’application AltspaceVR
description: Découvrez comment utiliser l’application AltspaceVR, les paramètres et les journaux des clients pour rechercher la version de AltspaceVR en cours d’exécution.
ms.date: 02/10/2021
ms.topic: article
keywords: version de l’application
ms.openlocfilehash: fbf67a8302a67ddb916772420949cf0509a0d4a60c472711975c651862438b93
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/11/2021
ms.locfileid: "119128250"
---
# <a name="finding-the-altspacevr-app-version"></a>Recherche de la version de l’application AltspaceVR

Au cours de la résolution d’un problème, vous pouvez être invité à indiquer la version de l’application AltspaceVR en cours d’exécution.

## <a name="in-altspacevr"></a>Dans AltspaceVR

Pour trouver la version de l’application dans AltspaceVR, accédez au **menu paramètres** et sélectionnez **à propos** de dans la barre de navigation de gauche. La version de l’application est indiquée ici, comme indiqué dans la capture d’écran ci-dessous.

![Paramètres menu ouvert avec à propos du panneau ouvert](images/app-version-img-01.png)

## <a name="in-windows-system-settings"></a>dans Windows Paramètres système

si vous avez installé AltspaceVR via la Microsoft Store, vous pouvez également trouver la version de l’application dans les paramètres du système Windows.  Ce scénario est adapté lorsque vous signalez la version de l’application si vous ne parvenez pas à vous connecter au client.

pour trouver la version de l’application dans Windows paramètres système, ouvrez le **Menu démarrer**, tapez **applications & fonctionnalités**, puis sélectionnez le résultat. Accédez à **AltspaceVR** dans la liste des applications. Cliquez sur AltspaceVR et sélectionnez **Options avancées** dans le menu qui s’affiche.

![Menu applications et fonctionnalités ouvert avec l’option avancé mise en surbrillance](images/app-version-img-02.png)

Dans les **Options avancées**, sous l’en-tête **spécifications** , la version de l' **application** doit figurer à droite de l’étiquette **version** .

![Options avancées ouvertes avec la version de l’application mise en surbrillance](images/app-version-img-03.png)

## <a name="in-client-logs"></a>Dans les journaux client

AltspaceVR signale la version de l’application dans le fichier journal du client en tant que « version Altspace » au démarrage de l’application. Il s’agit d’une bonne option pour obtenir la version de l’application si vous ne parvenez pas à vous connecter au client, mais qu’elle a tenté de démarrer avant d’échouer.

## <a name="windows"></a>Windows

sur Windows, le fichier journal du client est accessible via Windows Explorer à l’adresse suivante :

```
%userprofile%\AppData\LocalLow\Microsoft\AltspaceVR\Player.log
%userprofile%\AppData\LocalLow\Microsoft\AltspaceVR\Player-prev.log
```

Ce fichier est remplacé chaque fois que vous lancez AltspaceVR. 'Player. log’représente la dernière session et’Player-PREV. log’représente la session précédente.

## <a name="via-powershell"></a>Via PowerShell

Les utilisateurs avancés peuvent rechercher cette chaîne dans les journaux du client à l’aide de PowerShell comme suit :

Entrée :

```
gc $env:userprofile\appdata\locallow\altspacevr\altspacevr\Player.log | ? { $_ -match "Altspace Version" }
```

Sortie :

[2,047] version de AltspaceVR : 3.2.23. e66c2