---
title: Aide du chargeur d’Unity
description: Restez à jour sur les dernières questions et solutions fréquemment posées pour le chargeur AltspaceVR Unity.
ms.date: 02/10/2021
ms.topic: article
keywords: aide, FAQ
ms.openlocfilehash: 814ff293cb98490900cd929f33477d15d3d668ae
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/08/2021
ms.locfileid: "107212494"
---
# <a name="unity-uploader-help"></a>Aide du chargeur d’Unity

**1. Comment cet outil est-il génial ?**

> [!VIDEO https://channel9.msdn.com/Shows/Docs-Mixed-Reality/cheyenne-mountain-gate-room-v1/player]

C’est ma scène Stargate Unity avec une application SDK qui alimente la porte et DND

**2. je suis un apprenant vidéo, où sont mes vidéos ?**

[Consultez nos vidéos](https://youtu.be/km9CnVYPzoM)

**3. où puis-je trouver des exemples ?**

Les [mondes vedettes](https://account.altvr.com/worlds/featured) et les [exemples de la](https://account.altvr.com/worlds/1046572460192825569) solution sont les bons emplacements à démarrer

**4. cela fonctionne-t-il avec les kits et le nouveau kit de développement logiciel (SDK) ?**
Oui, vous pouvez utiliser tous les outils ensemble si vous le souhaitez. Nous essayons de les développer pour travailler en toute transparence.

**5. prend-il en charge les effets de particule ?**

![GIF d’effets de particules de neige](images/uploader-faq-img-01.gif)

**6. puis-je recevoir des données audio spatiales ?**
Ce n’est pas le moment, mais vous pouvez placer des sources audio à jouer dans des zones localisées. 

**7. l’éclairage cuit est-il opérationnel ?**
Oui, mais vos lumières doivent être définies sur « cuit » et non sur « mixte »

**8. l’éclairage global fonctionne-t-il ?**
Yes

**9. avez-vous toujours besoin de réinitialiser le monde ?**
Oui. Nous devons recharger les regroupements d’actifs Unity à chaque fois. 

**10. puis-je utiliser mes propres matériaux et nuanceurs personnalisés ?**

![GIF de matériaux et de nuanceurs personnalisés](images/uploader-faq-img-02.gif)

**11. puis-je télécharger sur une seule plate-forme ?**
Oui, à l’aide de l’outil de chargement. Toutefois, les personnes qui se trouvent sur Android ne voient rien dans votre univers tant que vous n’avez pas téléchargé la scène pour leur plateforme. 

**12. les scripts sont-ils autorisés ?**
Non, pour des raisons de sécurité, nous ne pouvons pas autoriser les scripts ou les références de script. Si votre téléchargement contient des scripts ou des références de script, il est rejeté. Jetez un coup d’œil au nouveau kit de développement logiciel (SDK) si vous avez besoin de scripts. 

**13. quelle est la taille d’une scène puis-je la télécharger ?**
Nous vous suggérons de commencer petit et de tenir à l’esprit des gens de Altspace qui n’ont pas de Monster PC. Cela dit, nous avons fait en sorte que les jeux fassent apparaître leurs cartes pour des flux en direct (par exemple, un jeu de VR Shooter)

![Capture d’écran du jeu VR dans AltspaceVR](images/uploader-faq-img-03.png)

**14. dois-je héberger les fichiers de scène ?**
Non, Altspace sert les fichiers une fois que vous les avez téléchargés

**15. les ombres sont-elles autorisées ?**
Yes

**16. quelle est la rapidité avec laquelle puis-je effectuer une itération à l’aide du chargeur ?**
Si vous êtes déjà dans votre monde, vous pouvez appuyer sur Télécharger dans le téléchargeur, réinitialiser votre univers et voir la scène mise à jour en 10 secondes. En règle générale, vous verrez des boucles de 30 secondes à quelques minutes, selon la complexité de votre scène. Ayez une boisson, vous méritez-vous qu’il s’agit d’un générateur de monde !

**17. où puis-je me procurer des modèles 3D ?**
Sketchfab, SketchUp, Minecraft, Unity Asset Store, etc.

**18. les animations sont-elles prises en charge ?**

![GIF d’animations personnalisées en cours d’exécution](images/uploader-faq-img-04.gif)

**19. Comment configurer le son spatial ?** Importez le fichier WAV de votre choix, créez un objet de jeu vide dans la scène et sélectionnez cet objet. Faites glisser et déposez le son importé dans l’inspecteur de l’objet pour créer une source audio. Ajustez ensuite le volume à 0,5, modifiez le lissage spatial en 3D et ajustez les distances min et Max pour créer une zone de son appropriée. Cela s’affiche comme une sphère comme les conflits par défaut. Pour obtenir une véritable remise, vous devez ajuster la courbe de dépose à votre convenance. [(via @IsThatToasted )](https://www.youtube.com/watch?v=ktb2vAAwknw&list=PLGmYIROty-5bpzKQNK3mRMi4pmh_LinV4&t=642s&index=29)

**20. Comment suis-je confronté à ébahis/étrange ?**
Parfois, le chargeur ne parvient pas à remplacer vos paramètres de rendu. « Accédez à modifier > paramètres du projet > Player ». Vérifiez que la case à cocher « paramètres XR > la réalité virtuelle prise en charge » est activée et que « méthode de rendu stéréo » est « passe unique » ou « passe unique (préversion) » pour PC et Android (sélectionnez l’icône de l’automate). Ensuite, générez + téléchargez à nouveau et réinitialisez votre monde. 