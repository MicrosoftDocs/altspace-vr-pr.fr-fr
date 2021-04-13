---
title: Téléchargement de skyboxes personnalisés
description: Obtenir des instructions pas à pas sur le téléchargement et la résolution des problèmes de votre skyboxes personnalisé dans les expériences AltspaceVR.
ms.date: 03/11/2021
ms.topic: article
keywords: skyboxes, résolution des problèmes
ms.openlocfilehash: 02d5bc762dc36d4195100e8155d6250789e833f7
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/08/2021
ms.locfileid: "107212435"
---
# <a name="uploading-custom-skyboxes"></a>Téléchargement de skyboxes personnalisés

Un skybox est un moyen de créer un **arrière-plan** pour votre monde qui rend l’expérience plus immersive. Il existe différents types de skyboxes, mais nous prenons actuellement en charge **équirectangulaire**. Voici un exemple pris avec une caméra 360 (plus d’exemples [ici](http://moments.mankindforward.com/)) : 

![360 équirectangulaire vue d’un salon](images/custom-skyboxes-img-01.jpeg)

Vous pouvez également utiliser le [chargeur Unity](world-building-toolkit-getting-started.md) , mais cette approche est plus simple.

1. Accédez à [mondes > skyboxes](https://account.altvr.com/skyboxes) et appuyez sur le bouton **créer** à droite

![Page de site Web mondes ouverte dans le panneau skyboxes](images/custom-skyboxes-img-02.png)

2. Renseignez un nom et spécifiez votre image 360. Il n’est pas nécessaire qu’il s’agit d’une photo. il existe des programmes qui vous permettent de créer les vôtres, ou vous pouvez rechercher des en ligne. Quand vous êtes prêt, sélectionnez **Créer**. 

![Formulaire de création de skybox](images/custom-skyboxes-img-03.png)

3. Vous pouvez éventuellement télécharger une image d' **Aperçu** afin de pouvoir identifier facilement ce skybox. Vous pouvez également charger des données audio ambiantes au format WAV. 

> [!IMPORTANT]
> Nous vous recommandons de charger les images d’aperçu et l’audio ambiant séparément, une fois que vous avez téléchargé l’image 360. Si vous les Téléchargez ensemble, la taille des fichiers peut être suffisamment grande pour bloquer le processus. [Jetsons World](https://account.altvr.com/worlds/1004174988393054363/spaces/1084431533181240311) est un excellent exemple illustrant l’utilisation d’un skybox avec l’audio ambiant. Notez que le monde entier a conservé le volume audio faible et que les sons que vous entendez sont sporadiques pour que les gens ne soient pas importuns. 

4. Accédez à votre monde et ouvrez l’éditeur de monde. Sous skyboxes, sélectionnez votre nouveau skybox. En quelques secondes, le ciel change littéralement. D’autres dans votre monde voient également la modification du ciel. Pour revenir en arrière, choisissez le skybox **par défaut** dans cette même liste. 

## <a name="troubleshooting"></a>Résolution des problèmes

**Il y a une couture ou une ligne dans le ciel :-(.** Il s’agit d’un bogue que nous corrigerons bientôt

**Échec du chargement**
    * essayez de charger uniquement l’image 360 seule
    * Essayez avec un autre fichier plus petit comme un test

**Je ne trouve pas de photo 360**
    * Flickr est une bonne source (modifiez les filtres pour rechercher des éléments créatifs)
    * Prenez votre propre ! Nous avons réussi à utiliser les caméras de la Ricoh. 
**Le ciel semble granuleux ou bloqué** Vous devrez peut-être Rechercher une image de résolution supérieure. En général environ 2-5 Mo et ~ 5000 PX x 2000 PX

**Cela nuit à la fréquence d’images !**
L’image est probablement trop grande. Certains skyboxes générés peuvent être de 8 Ko. Ils sont généralement fournis avec des versions de 2 Ko faciles à utiliser.

**Aidez-moi avec l’audio ambiant**
    * Utilisez des logiciels gratuits comme Audacity pour réduire le volume ou créer vos propres boucles. N’oubliez pas que l’audio sera répété et joué dans les oreilles des gens.
    * Le [son gratuit](https://freesound.org/) est une bonne source de sons sans royalties
