---
title: Les autres utilisateurs ne m’entendent pas
description: Découvrez comment identifier et résoudre les problèmes liés à d’autres utilisateurs qui ne sont pas en mesure de s’entendre dans AltspaceVR.
ms.date: 03/11/2021
ms.topic: article
keywords: faq
ms.openlocfilehash: 189d96790207085a2a2c47e964c0db8a08ed95a76d91d2ced3026ba3455b45e3
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/11/2021
ms.locfileid: "119128090"
---
# <a name="other-users-cant-hear-me"></a>Les autres utilisateurs ne m’entendent pas

Tout d’abord, déterminez si AltspaceVR détecte le son à partir de votre microphone. Vous pouvez le déterminer en examinant si l’icône de microphone dans le coin inférieur gauche de votre vue clignote lorsque vous parlez. Si l’icône clignote lorsque vous conversez, c’est que votre microphone fonctionne. Si l’icône est rouge, vous êtes muet. Sélectionnez l’icône pour activer ou désactiver le son.

si vous ne voyez pas votre icône de microphone clignoter après la désactivation, vous devrez peut-être ajuster les paramètres du microphone dans AltspaceVR, accéder à Menu/Paramètres/audio/sélection d’entrée audio. Puis, à l’aide des boutons fléchés, sélectionnez le micro que vous souhaitez utiliser.
 
## <a name="oculus-quest"></a>Oculus Quest 

Veillez à accorder des autorisations d’utilisation de l’audio MIC lorsque vous installez AltspaceVR. une autre vérification que vous pouvez effectuer consiste à rechercher dans la sélection d’entrée de Menu/Paramètres/audio/audio et à vous assurer qu’elle est définie sur entrée audio Android (c’est le mic par défaut Quest/Quest2's).
 
## <a name="windows-mixed-reality-oculus-rift-htc-vive-or-2d-mode"></a>Windows Mixed Reality, Oculus, ou en Mode 2d

vérifiez que vous disposez des paramètres de microphone corrects dans AltspaceVR : Menu/Paramètres/audio/sélection d’entrée audio. Puis, à l’aide des boutons fléchés, sélectionnez le micro que vous souhaitez utiliser.

Avant de démarrer AltspaceVR, vérifiez que le microphone approprié est défini comme périphérique d’enregistrement par défaut dans Windows. Le rift et le HTC Oculus disposent d’un microphone intégré, si vous avez un autre microphone branché sur AltspaceVR peut essayer d’utiliser cet appareil.
 
Pour modifier votre appareil d’enregistrement par défaut dans Windows :
* cliquez avec le bouton droit sur l’icône de haut-parleur dans Windows puis sélectionnez **périphériques de lecture** .
* Accéder à l’onglet **enregistrement**
* Recherchez le microphone que vous souhaitez utiliser. Le microphone en vive HTC s’intitule **microphone-USB Audio Device** et le microphone Oculus s’intitule microphone **-Rift audio**.
* Cliquez avec le bouton droit sur ce microphone et sélectionnez **définir comme périphérique par défaut** .
* Après le redémarrage de AltspaceVR, votre microphone est maintenant sélectionné
 
Si, après avoir effectué ces étapes, vous rencontrez toujours des problèmes, vous risquez de rencontrer d’autres problèmes :
* Si vous Alt-Tab pendant plus de 30 secondes, AltspaceVR vous permet de désactiver le mode de désactivation de l’option en utilisant le raccourci clavier : barre d’espace pour activer/désactiver le mode muet.
* Le système audio AltspaceVR a un seuil de volume qui peut être indiqué ci-dessous. Définissez niveaux mic sur Max, définissez le micro plus près de votre embouchure et parlez sur volume normal.
* Quittez VR, puis branchez le cordon USB de votre casque dans un port USB 3,0 alternatif. Dans notre expérience, certains ports USB 3,0 provoquent des problèmes.

AltspaceVR ne reconnaît peut-être pas les modifications apportées aux paramètres audio dans le jeu. par conséquent, vous devrez peut-être redémarrer AltspaceVR des modifications du microphone ci-dessus pour prendre effet.  Lorsque vous repassez le jeu, regardez l’icône du microphone et regardez si elle clignote. Si l’icône clignote, cela signifie que votre microphone fonctionne.