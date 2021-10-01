---
title: Forum aux questions sur l’audio AltspaceVR
description: Résolution des problèmes liés à l’audio et à la prise en charge.
ms.date: 8/23/2021
author: qianw211
ms.author: v-qianwen
ms.topic: article
keywords: VR, audio, dépannage, support
ms.openlocfilehash: 05c8a477b9e50b5067e62b934fe2ff8bd656f06c
ms.sourcegitcommit: 5c452a9092297c0bfbc8efabebf395e7ee31853f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/30/2021
ms.locfileid: "129311870"
---
# <a name="frequently-asked-questions-about-audio"></a>Forum aux questions sur l’audio

## <a name="does-my-vr-headset-have-a-built-in-mic"></a>Mon casque VR possède-t-il un MIC intégré ?

### <a name="oculus-riftrift-s-oculus-questquest-2-windows-mixed-reality-and-htc-vive"></a>Oculus rift/rift S, Oculus quest/quest 2, Windows Mixed Reality et HTC Vive

Oui, ces casques VR ont des microphones intégrés.

### <a name="windows"></a>Windows

pour les casques utilisés avec Windows, vous devez être en mesure de trouver le microphone listé sous vos **appareils d’enregistrement** lorsque le casque est branché.

### <a name="further-troubleshooting"></a>Résolution des problèmes

* [Support AltspaceVR : les autres utilisateurs ne peuvent pas m’entendre](#what-do-i-do-if-other-users-cant-hear-me)
* [Prise en charge AltspaceVR-gestion des autorisations pour Oculus Quest](../getting-started/oculus-controls.md#managing-permissions)

## <a name="is-there-a-push-to-talk-button"></a>Existe-t-il un bouton où appuyer pour parler ?

Il n’existe aucun bouton d’envoi à la communication.  Si vous regardez dans le coin inférieur gauche de votre affichage, une icône de microphone peut être utilisée pour activer la voix. Vous pouvez également utiliser le raccourci clavier, la barre d’espace pour activer/désactiver votre microphone.

Si l’icône clignote lorsque vous conversez, c’est que votre microphone fonctionne !
 
## <a name="what-do-i-do-if-my-audio-is-choppy"></a>Que dois-je faire si mon audio est haché ?

Certains utilisateurs ont remarqué que lorsqu’un autre avatar parle de la voix, le son est instable ou avec des dépassements réguliers. Vous pouvez être informé par d’autres utilisateurs que votre propre audio est instable ou robotique.

La première chose à essayer consiste toujours à entrer à nouveau l’espace dans lequel vous vous trouvez, ou même à redémarrer AltspaceVR en cas d’échec. Les problèmes audio ne sont pas courants, mais lorsqu’ils se produisent, il s’agit souvent d’une solution simple. 

Si ce n’est pas le cas, vous pouvez examiner les éléments suivants :

#### <a name="cpu-performance-for-desktop-users"></a>Performances de l’UC pour les utilisateurs du Bureau

Passez en revue les [Spécifications système recommandées](../getting-started/system-requirements.md) pour le matériel que nous suggérons d’exécuter AltspaceVR. Nous avons constaté que les processeurs i3 ou inférieurs causent des problèmes non seulement avec les cadences d’images de la vidéo, mais ils peuvent contribuer à des problèmes audio tels que les dépassements et la qualité médiocre.

#### <a name="internet-bandwidth-and-network-connection"></a>Bande passante Internet et connexion réseau

Les utilisateurs sur des connexions Internet lentes (moins de 5Mbps) ou sur WiFi peuvent rencontrer des problèmes audio, tels que des dépassements. Nous recommandons la connexion Hardline d’un câble Ethernet à votre ordinateur et une connexion plus rapide que 5Mbps. Vous pouvez fermer tous les programmes susceptibles d’utiliser la connectivité Internet en arrière-plan.

## <a name="what-do-i-do-if-other-users-cant-hear-me"></a>Que dois-je faire si d’autres utilisateurs ne peuvent pas m’en apprendre ?

Tout d’abord, déterminez si AltspaceVR détecte le son à partir de votre microphone. Vous pouvez le déterminer en examinant si l’icône de microphone dans le coin inférieur gauche de votre vue clignote lorsque vous parlez. Si l’icône clignote lorsque vous conversez, c’est que votre microphone fonctionne. Si l’icône est rouge, vous êtes muet. Sélectionnez l’icône pour activer ou désactiver le son.

si vous ne voyez pas votre icône de microphone clignoter après la désactivation, vous devrez peut-être ajuster les paramètres du microphone dans AltspaceVR, accéder à Menu/Paramètres/audio/sélection d’entrée audio. Puis, à l’aide des boutons fléchés, sélectionnez le micro que vous souhaitez utiliser.
 
### <a name="oculus-questquest-2"></a>Oculus Quest/Quest 2

Veillez à accorder des autorisations d’utilisation de l’audio MIC lorsque vous installez AltspaceVR. vous pouvez également effectuer une vérification dans : Menu/Paramètres/audio/sélection d’entrée audio, et en veillant à ce qu’elle soit définie sur entrée audio Android, qui est Quest/Quest2's par défaut mic.
 
### <a name="windows-mixed-reality-oculus-riftrift-s-htc-vive-or-2d-mode"></a>Windows Mixed Reality, Oculus-rift/rift S, HTC Vive ou 2d

vérifiez que vous disposez des paramètres de microphone corrects dans AltspaceVR : Menu/Paramètres/audio/sélection d’entrée audio. Puis, à l’aide des boutons fléchés, sélectionnez le micro que vous souhaitez utiliser.

Avant de démarrer AltspaceVR, vérifiez que le microphone approprié est défini comme périphérique d’enregistrement par défaut dans Windows. Le Oculus/le rift S et HTC vives ont tous deux un microphone intégré, si vous avez un autre microphone branché sur AltspaceVR peut essayer d’utiliser cet appareil.
 
Pour modifier votre appareil d’enregistrement par défaut dans Windows :

* cliquez avec le bouton droit sur l’icône de haut-parleur dans Windows et sélectionnez **ouvrir les paramètres audio**.
* Accédez à l’entrée/choisissez la liste déroulante de **votre appareil d’entrée** .
* Choisissez le microphone que vous souhaitez utiliser dans le menu déroulant : 
    * Le microphone en vive HTC s’intitule **microphone-USB Audio Device**.
    * Le microphone du Rift Oculus sera intitulé **casque microphone (périphérique audio virtuel Oculus)**.
* Après le redémarrage de AltspaceVR, votre microphone est maintenant sélectionné
 
Si, après avoir effectué ces étapes, vous rencontrez toujours des problèmes, il se peut que vous rencontriez les éléments suivants :

* Si vous Alt-Tab pendant plus de 30 secondes, AltspaceVR se désactivera automatiquement. vous pouvez désactiver cette option dans le **Menu > Paramètres > son > muet quand AltspaceVR est inactif**.
* Le système audio AltspaceVR a un seuil de volume qui peut être indiqué ci-dessous. Définissez niveaux mic sur Max, définissez le micro plus près de votre embouchure et parlez sur volume normal.
* Quittez VR, puis branchez le cordon USB de votre casque dans un port USB 3,0 alternatif. Dans notre expérience, certains ports USB 3,0 provoquent des problèmes.

AltspaceVR ne reconnaît peut-être pas les modifications apportées aux paramètres audio dans le jeu. par conséquent, vous devrez peut-être redémarrer AltspaceVR pour que les modifications du microphone ci-dessus prennent effet.  Lorsque vous entrez à nouveau le jeu, regardez l’icône du microphone et regardez si elle clignote quand vous y êtes en contact. Si l’icône clignote, cela signifie que votre microphone fonctionne.

## <a name="support"></a>Support

Vous avez des questions ou des commentaires pour l’équipe AltspaceVR ? 

> [!div class="nextstepaction"]
> [Cliquez ici pour envoyer une demande de support](https://help.altvr.com/hc/requests/new)