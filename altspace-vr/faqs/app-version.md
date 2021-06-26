---
title: Recherche de la version de l’application AltspaceVR
description: Découvrez comment utiliser l’application AltspaceVR, les paramètres et les journaux des clients pour rechercher la version de AltspaceVR en cours d’exécution.
ms.date: 02/10/2021
ms.topic: article
keywords: version de l’application
ms.openlocfilehash: 6b710e1724b890fa7ba0eecfcd774ef63128d5b7
ms.sourcegitcommit: 2db596ab5a1ecd4901a8c893741cc4d06f6aecea
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2021
ms.locfileid: "112923176"
---
# <a name="finding-the-altspacevr-app-version"></a><span data-ttu-id="ba63c-104">Recherche de la version de l’application AltspaceVR</span><span class="sxs-lookup"><span data-stu-id="ba63c-104">Finding the AltspaceVR app version</span></span>

<span data-ttu-id="ba63c-105">Au cours de la résolution d’un problème, vous pouvez être invité à indiquer la version de l’application AltspaceVR en cours d’exécution.</span><span class="sxs-lookup"><span data-stu-id="ba63c-105">In the course of troubleshooting an issue, you may be asked what version of the AltspaceVR app you're currently running.</span></span>

## <a name="in-altspacevr"></a><span data-ttu-id="ba63c-106">Dans AltspaceVR</span><span class="sxs-lookup"><span data-stu-id="ba63c-106">In AltspaceVR</span></span>

<span data-ttu-id="ba63c-107">Pour trouver la version de l’application dans AltspaceVR, accédez au **menu paramètres** et sélectionnez **à propos** de dans la barre de navigation de gauche.</span><span class="sxs-lookup"><span data-stu-id="ba63c-107">To find the app version in AltspaceVR, navigate to the **settings menu** and select **About** in the left navigation bar.</span></span> <span data-ttu-id="ba63c-108">La version de l’application est indiquée ici, comme indiqué dans la capture d’écran ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="ba63c-108">The 'App Version' is reported here, as shown in the screenshot below.</span></span>

![Menu paramètres ouvert avec à propos du panneau ouvert](images/app-version-img-01.png)

## <a name="in-windows-system-settings"></a><span data-ttu-id="ba63c-110">Dans les paramètres système Windows</span><span class="sxs-lookup"><span data-stu-id="ba63c-110">In Windows System Settings</span></span>

<span data-ttu-id="ba63c-111">Si vous avez installé AltspaceVR via la Microsoft Store, vous pouvez également trouver la version de l’application dans les paramètres système Windows.</span><span class="sxs-lookup"><span data-stu-id="ba63c-111">If you installed AltspaceVR via the Microsoft Store, you can additionally find the app version in the Windows system settings.</span></span>  <span data-ttu-id="ba63c-112">Ce scénario est adapté lorsque vous signalez la version de l’application si vous ne parvenez pas à vous connecter au client.</span><span class="sxs-lookup"><span data-stu-id="ba63c-112">This scenario is a good fit when reporting the app version if you're unable to successfully log into the client.</span></span>

<span data-ttu-id="ba63c-113">Pour rechercher la version de l’application dans les paramètres système Windows, ouvrez le **menu Démarrer**, tapez dans **applications & fonctionnalités**, puis sélectionnez le résultat.</span><span class="sxs-lookup"><span data-stu-id="ba63c-113">To find the app version in Windows system settings, open the **Start Menu**, type in **Apps & Features**, and select the result.</span></span> <span data-ttu-id="ba63c-114">Accédez à **AltspaceVR** dans la liste des applications.</span><span class="sxs-lookup"><span data-stu-id="ba63c-114">Navigate to **AltspaceVR** in the list of apps.</span></span> <span data-ttu-id="ba63c-115">Cliquez sur AltspaceVR et sélectionnez **Options avancées** dans le menu qui s’affiche.</span><span class="sxs-lookup"><span data-stu-id="ba63c-115">Left-click AltspaceVR and select **Advanced Options** from the menu that appears.</span></span>

![Menu applications et fonctionnalités ouvert avec l’option avancé mise en surbrillance](images/app-version-img-02.png)

<span data-ttu-id="ba63c-117">Dans les **Options avancées**, sous l’en-tête **spécifications** , la version de l' **application** doit figurer à droite de l’étiquette **version** .</span><span class="sxs-lookup"><span data-stu-id="ba63c-117">In the **Advanced Options**, under the **Specifications** header, the **App Version** should be listed to the right of the **Version** label.</span></span>

![Options avancées ouvertes avec la version de l’application mise en surbrillance](images/app-version-img-03.png)

## <a name="in-client-logs"></a><span data-ttu-id="ba63c-119">Dans les journaux client</span><span class="sxs-lookup"><span data-stu-id="ba63c-119">In Client Logs</span></span>

<span data-ttu-id="ba63c-120">AltspaceVR signale la version de l’application dans le fichier journal du client en tant que « version Altspace » au démarrage de l’application.</span><span class="sxs-lookup"><span data-stu-id="ba63c-120">AltspaceVR reports the app version in the client logs file as "Altspace Version" during application startup.</span></span> <span data-ttu-id="ba63c-121">Il s’agit d’une bonne option pour obtenir la version de l’application si vous ne parvenez pas à vous connecter au client, mais qu’elle a tenté de démarrer avant d’échouer.</span><span class="sxs-lookup"><span data-stu-id="ba63c-121">This would be a good option to get the app version if you can't successfully log into the client, but it did attempt to start before failing.</span></span>

## <a name="windows"></a><span data-ttu-id="ba63c-122">Windows</span><span class="sxs-lookup"><span data-stu-id="ba63c-122">Windows</span></span>

<span data-ttu-id="ba63c-123">Sur Windows, vous pouvez trouver le fichier journal du client via l’Explorateur Windows à l’adresse suivante :</span><span class="sxs-lookup"><span data-stu-id="ba63c-123">On Windows, the client logs file can be found via Windows Explorer at:</span></span>

```
%userprofile%\AppData\LocalLow\Microsoft\AltspaceVR\Player.log
%userprofile%\AppData\LocalLow\Microsoft\AltspaceVR\Player-prev.log
```

<span data-ttu-id="ba63c-124">Ce fichier est remplacé chaque fois que vous lancez AltspaceVR.</span><span class="sxs-lookup"><span data-stu-id="ba63c-124">This file is overwritten each time you launch AltspaceVR.</span></span> <span data-ttu-id="ba63c-125">'Player. log’représente la dernière session et’Player-PREV. log’représente la session précédente.</span><span class="sxs-lookup"><span data-stu-id="ba63c-125">'Player.log' represents your latest session, and 'Player-prev.log' represents the previous session.</span></span>

## <a name="via-powershell"></a><span data-ttu-id="ba63c-126">Via PowerShell</span><span class="sxs-lookup"><span data-stu-id="ba63c-126">Via PowerShell</span></span>

<span data-ttu-id="ba63c-127">Les utilisateurs avancés peuvent rechercher cette chaîne dans les journaux du client à l’aide de PowerShell comme suit :</span><span class="sxs-lookup"><span data-stu-id="ba63c-127">Advanced users can search the client logs for this string via PowerShell as follows:</span></span>

<span data-ttu-id="ba63c-128">Entrée :</span><span class="sxs-lookup"><span data-stu-id="ba63c-128">Input:</span></span>

```
gc $env:userprofile\appdata\locallow\altspacevr\altspacevr\Player.log | ? { $_ -match "Altspace Version" }
```

<span data-ttu-id="ba63c-129">Sortie :</span><span class="sxs-lookup"><span data-stu-id="ba63c-129">Output:</span></span>

<span data-ttu-id="ba63c-130">[2,047] version de AltspaceVR : 3.2.23. e66c2</span><span class="sxs-lookup"><span data-stu-id="ba63c-130">[2.047] AltspaceVR Version: 3.2.23.e66c2</span></span>