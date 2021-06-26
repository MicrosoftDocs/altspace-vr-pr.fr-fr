---
title: Enregistrement et diffusion en continu en direct
description: Découvrez comment enregistrer et diffuser en direct vos événements AltspaceVR à partir de votre PC pour les promouvoir et les partager avec vos utilisateurs.
ms.date: 04/26/2021
ms.topic: article
keywords: streaming, enregistrement, vidéo, audio, YouTube, OBS
ms.openlocfilehash: 0bf32d8ac7e2d409eb5e2c31a9da8a878e0e5eef
ms.sourcegitcommit: 2db596ab5a1ecd4901a8c893741cc4d06f6aecea
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2021
ms.locfileid: "112923016"
---
# <a name="recording-and-live-streaming"></a>Enregistrement et diffusion en continu en direct

L’enregistrement et la diffusion en continu de votre expérience AltspaceVR pour montrer d’autres personnes du monde entier sont un excellent moyen de promouvoir vos événements, AltspaceVR et VR en général ! Jetez un coup d’œil ci-dessous pour découvrir comment démarrer :

Dans cet article, vous allez apprendre à :

* [Enregistrer AltspaceVR en mode 2D sur le PC](#recording-altspacevr-in-2d-mode-on-pc)
* [Flux Live vers YouTube dans AltspaceVR en mode 2D sur PC](#live-streaming-to-youtube-in-altspacevr-2d-mode-on-pc)

## <a name="recording-altspacevr-in-2d-mode-on-pc"></a>Enregistrement de AltspaceVR en mode 2D sur le PC

### <a name="the-short-version"></a>Version abrégée

1. AltspaceVR et OBS doivent être installés. Lancez AltspaceVR en mode 2D, lancez OBS, définissez OBS pour enregistrer AltspaceVR et enregistrer !

### <a name="the-slightly-longer-version"></a>Version légèrement plus longue

1. Consultez [https://obsproject.com/](https://obsproject.com/)
2. Sélectionnez **Windows** pour télécharger OBS. Cette publication utilise **OBS v 22.0.2**
3. Installer OBS

### <a name="have-altspacevr-running-in-2d-mode-before-you-run-obs"></a>AltspaceVR s’exécuter en mode 2D avant d’exécuter OBS

1. Téléchargez et installez AltspaceVR à partir de notre site Web : [altvr.com/Get](https://altvr.com/getaltspacevr)
2. Veillez à lancer AltspaceVR en mode 2D en débranchant le câble USB de votre HMD de votre ordinateur ou, si vous avez un Rift : Ctrl + Alt + Suppr, services, service d’exécution Oculus VR, cliquez avec le bouton droit, puis arrêtez. 
    * Cela désactive Oculus et démarre AltspaceVR en mode 2D, répétez ces étapes et utilisez Start pour revenir en mode VR.

Maintenant, Alt-Tab sur OBS :

1. Sous sources, sélectionnez : **+ > la capture de jeu > créer**
2. Modifiez Text en « AltspaceVR capture », Tick **Make source visible**, puis sélectionnez OK.
3. Double-cliquez sur **AltspaceVR capture** sous sources
4. Changer le **mode** pour **capturer une fenêtre spécifique**
5. Fenêtre : [AltspaceVR.exe] : AltspaceVR
6. Priorité de la fenêtre de correspondance : titre de correspondance, sinon Rechercher une fenêtre du même exécutable
7. Faites défiler jusqu’au curseur de capture : décochez
8. Sélectionnez OK (OK).

Cela devrait faire apparaître AltspaceVR dans OBS. Maintenant, pour définir les propriétés suivantes dans OBS, accédez à **fichier > paramètres**:

|Onglet|Paramètres|
|---|---|
| **Général** | Conservez la valeur par défaut |
| **STREAM** | Conservez la valeur par défaut |
| Mode de sortie | Basculer vers la configuration avancée |
| Onglet streaming | Piste audio 1 <br> Encodeur : x264 <br> Mise à l’échelle de la sortie : incochée <br> Contrôle de la fréquence : CBR <br> Débit binaire : 6000 (6000 pour 30 i/s ou 9000 pour 60 fps) <br> Intervalle d’image clé = 2 <br> Présélection de l’utilisation de l’UC = veryfast |
| Onglet Enregistrement | Type : standard <br> Chemin d’enregistrement : D:/Video (accédez à l’emplacement où vous souhaitez enregistrer le fichier vidéo) <br> Format d’enregistrement : MP4 (si vous recevez un incident lors de l’enregistrement, essayez FLV ici au lieu de MP4, si vous rencontrez une panne, la vidéo sera toujours utilisable avec FLV) <br> Piste audio 1 <br> Encodeur : utiliser l’encodeur de flux |
| Onglet Audio | Débit binaire audio : 160 (pour toutes les pistes) |
| Onglet mémoire tampon de relecture | Conservez la valeur par défaut |
| **Audio** | Taux d’échantillonnage : 48 kHz <br> Canaux : stéréo <br> Périphérique audio du Bureau : par défaut <br> Périphérique audio de bureau 2 : désactiver <br> Périphérique audio MIC/auxiliaires : par défaut |
| **Vidéo** | Résolution de base (canevas) : 1920 x 1080 <br> Résolution de sortie (mise à l’échelle) : 1920 x 1080 <br> Filtre réduire : bicubique (mise à l’échelle accentuée, 16 échantillons) <br> Valeurs d’FPS courantes : 30 |
| **Touches d’accès rapide** | Conservez la valeur par défaut |
| **Avancée** | Priorité du processus : normale | <br>

<br>Bien, veillez à sélectionner **appliquer**, puis cliquez sur **OK** pour enregistrer tous vos paramètres OBS. 

1. Alt-Tab à AltspaceVR, accédez à l’espace/au monde/à l’événement approprié et aligner votre appareil photo (c’est-à-dire, votre avatar) nous sommes sur le point d’enregistrer une vidéo !
2. Alt-Tab sur OBS et, lorsque vous êtes prêt, cliquez sur **Démarrer l’enregistrement**.

Vous verrez en bas à droite de OBS que REC : commence à compter et le point est rouge, ce qui signifie que vous enregistrez !

Procédez à un enregistrement de test : 
1. Dans AltspaceVR, ouvrez/fermez/survolé les menus pour créer des sons d’interface utilisateur
2. Assurez-vous que vous êtes bien désactivé, dites « sibilance, sibilance » ou demandez à un autre utilisateur de vous communiquer sur un volume normal.
3. Examinez les niveaux audio et MIC/aux au fur et à mesure que vous le faites pour voir s’ils fonctionnent.

En général, le micro/les est muet lors de l’enregistrement. Continuez et sélectionnez l’icône en forme de haut-parleur pour MIC/aux, et la couleur rouge avec un X.

* Il est très difficile de faire correspondre votre audio et l’audio de l’autre utilisateur, de sorte que le micro est le meilleur en sourdine lorsque vous enregistrez un événement.
* Un autre problème avec l’audio est la configuration de OBS. Il capture tout l’audio de votre ordinateur, si bien que vous regardez YouTube sur votre ordinateur, il enregistre ces notifications audio ou de discordon.
* Pour enregistrer uniquement l’audio de AltspaceVR, accédez à mixer de volume (cliquez avec le bouton droit sur l’icône en forme de haut-parleur en bas à droite de Windows) et désactivez les sons système, les navigateurs, etc., mais pas muet OBS ou AltspaceVR.

> [!IMPORTANT]
> N’oubliez pas de réactiver ces paramètres de mélangeur de volume après l’enregistrement.

À présent, revenez à OBS et sélectionnez **arrêter l’enregistrement** à partir du **fichier>afficher les enregistrements**. Cela ouvre le dossier avec vos fichiers vidéo OBS, double-cliquez sur la vidéo de test.

Parfois, l’enregistrement est très bruyant. par conséquent, réduisez le curseur pour le son de bureau et effectuez un autre enregistrement pour le test.


## <a name="live-streaming-to-youtube-in-altspacevr-2d-mode-on-pc"></a>Streaming en direct vers YouTube en mode AltspaceVR 2D sur PC

### <a name="the-short-version"></a>Version abrégée

AltspaceVR et OBS doivent être installés. Lancez AltspaceVR en mode 2D, lancez OBS, ou créez un « nouvel événement en direct » sur YouTube, configurez OBS à l’aide de votre clé de flux YouTube, commencez la diffusion en continu dans OBS, commencez la diffusion sur YouTube et vous êtes en train de les concurrences !

### <a name="the-slightly-longer-version"></a>Version légèrement plus longue

1. Consultez [https://obsproject.com/](https://obsproject.com/)
2. Sélectionnez **Windows** pour télécharger OBS (ce billet utilise OBS v 22.0.2)
3. Installer OBS

AltspaceVR s’exécuter en mode 2D avant d’exécuter OBS
1. Téléchargez AltspaceVR à partir de notre site Web : [https://account.altvr.com/downloads](https://account.altvr.com/downloads)
2. Pour vous assurer que vous lancez AltspaceVR en mode 2D, débranchez le câble USB de votre HMD de votre ordinateur ou, si vous avez un Rift : Ctrl + Alt + Suppr, services, service d’exécution Oculus VR, cliquez avec le bouton droit, puis arrêtez. Cela va entraîner la désactivation de Oculus à la page d’accueil et du démarrage de AltspaceVR en mode 2D, répétez ces étapes et redémarrez le mode VR.

3. Alt-Tab à OBS

4. Sous sources, sélectionnez **+** , sélectionnez capture de jeu, créer, modifier le texte pour « AltspaceVR capture », Tick make source visible, OK
5. Double-cliquez sur AltspaceVR capture.
6. Mode : capturer une fenêtre spécifique
7. Fenêtre : [AltspaceVR.exe] : AltspaceVR
8. Priorité de la fenêtre de correspondance : titre de correspondance, sinon Rechercher une fenêtre du même exécutable
9. Faites défiler jusqu’au curseur de capture : décocher OK

Cela devrait faire apparaître AltspaceVR dans OBS. Bravo !

Maintenant, dans OBS, accéder aux paramètres de>de fichiers :

| Onglet | Paramètres |
|---|---|
| Général | Tick enregistre automatiquement la diffusion en continu (enregistre un fichier vidéo sur votre ordinateur en plus de la diffusion en continu) |
| STREAM | Type de flux : services de streaming <br> Service : jeu YouTube/YouTube (peut également diffuser en continu vers Twitch, mixer, Facebook Live, etc.)<br>Serveur : serveur de réception YouTube principal <br>Clé de flux : collez votre clé de flux à partir de YouTube * * * (consultez « Configuration de la diffusion en continu en direct sur YouTube » ci-dessous) |
| Sortie | Mode de sortie : basculer vers avancé |
| Diffusion en continu | Piste audio 1 <br>Encodeur : x264 <br>Appliquer les paramètres de l’encodeur de service de diffusion en continu : Tick <br>Mise à l’échelle de la sortie : incochée <br>Contrôle de la fréquence : CBR <br>Débit binaire : 6000 (6000 pour 30 i/s ou 9000 pour 60 fps) <br>Intervalle d’image clé = 2 <br>Présélection de l’utilisation de l’UC = veryfast |
| Enregistrement | Type : standard <br>Chemin d’enregistrement : D:/Video (accédez à l’emplacement où vous souhaitez enregistrer le fichier vidéo si vous avez sélectionné enregistrer automatiquement lors de la diffusion en continu) <br>Format d’enregistrement : MP4 (si vous recevez un incident lors de l’enregistrement, essayez FLV ici au lieu de MP4, si vous rencontrez une panne, la vidéo sera toujours utilisable avec FLV) <br>Piste audio 1 <br>Encodeur : utiliser l’encodeur de flux |
| Audio | Débit audio : 160 (pour toutes les pistes) taux d’échantillonnage : 48 kHz <br>Canaux : stéréo <br>Périphérique audio du Bureau : par défaut <br>Périphérique audio de bureau 2 : désactiver <br>Périphérique audio MIC/auxiliaires : par défaut |
| Mémoire tampon de relecture | Conservez la valeur par défaut |
| Vidéo | Résolution de base (canevas) : 1920 x 1080 <br>Résolution de sortie (mise à l’échelle) : 1920 x 1080 <br>Filtre réduire : bicubique (mise à l’échelle accentuée, 16 échantillons) <br>Valeurs d’FPS courantes : 30 |
| Touches d’accès rapide | Conservez la valeur par défaut |
| Avancé | Priorité du processus : normale |
|||

<br>Bien, veillez à cliquer sur appliquer, puis sur OK, puis fermez et rouvrez OBS. Cela permet d’enregistrer vos paramètres OBS. Recherche de bons :)

Consultez la section « Comment enregistrer des AltspaceVR en mode 2D sur le PC » ci-dessus pour obtenir des instructions sur la façon de tester l’enregistrement à l’aide d’un enregistrement local au lieu du flux de données en direct et comment faire commencer la configuration de votre appareil photo avant l’enregistrement.

Un autre problème avec l’audio est la configuration de OBS. Il capture tous les éléments audio de votre ordinateur. par conséquent, si vous regardez YouTube, il enregistre ces messages audio ou d’équipe, ou les sons de notification.

Pour enregistrer uniquement l’audio de AltspaceVR, accédez à mixer de volume (cliquez avec le bouton droit sur l’icône en forme de haut-parleur en bas à droite de Windows) et désactivez les sons système, les navigateurs, etc., mais pas muet OBS ou AltspaceVR.

N’oubliez pas de réactiver l’audio après l’enregistrement ;)

Vous êtes un enregistreur vidéo AltspaceVR !

## <a name="setting-up-live-streaming-on-youtube"></a>Configuration de la diffusion en continu en direct sur YouTube

Vous pouvez obtenir rapidement un flux en direct (**flux**) ou configurer un futur événement Live Stream (**gérer**). Je vous conseille de le configurer de manière « gérer ».

1. Ouvrez votre navigateur et connectez-vous [https://www.youtube.com/](https://www.youtube.com/) , puis accédez à [https://www.youtube.com/my_live_events](https://www.youtube.com/my_live_events)
2. Sélectionnez sur l’icône de votre compte, en haut à droite, sélectionnez Creator Studio dans la liste déroulante.
3. STREAMING en direct sur le côté gauche de la page.

Méthode «**Stream Now**» :

* Sélectionnez Modifier pour entrer vos informations de flux Live<br>
* Sous paramètres de flux, conservez les valeurs par défaut<br>
* Clé de flux (coller dans l’encodeur), sélectionnez « révéler » et copiez cette clé pour pouvoir la coller dans OBS<br>
* Ouvrir OBS/Settings/Stream<br>
* Collez la clé de flux de YouTube dans le champ de clé de flux dans OBS<br>
* Appliquer, puis sur OK<br>
* Sélectionnez Démarrer la diffusion en continu dans OBS<br>
* Basculez vers YouTube et vous verrez que vous êtes désormais en ligne sur YouTube !<br>
* Pour voir votre véritable page vidéo de flux Live YouTube, vous devez sélectionner l’icône de partage en haut à droite.<br>
* Copiez et collez la « liaison vidéo » dans un nouvel onglet de navigateur. vous verrez votre page de flux Live YouTube.<br>
* Cette URL est votre lien de flux Live et peut être partagée vers tous vos canaux de réseaux sociaux :)<br>
* Pour arrêter le flux en direct, sélectionnez arrêter la diffusion sur OBS, ce qui mettra fin au flux Live sur YouTube.<br>
* Arrêter ensuite Stream sur YouTube<br>

Méthode'**Manage**' :
* Sélectionnez « planifier le flux »
* Créer des paramètres ou les réutiliser si vous avez déjà configuré un flux Live managé précédent
* Ajouter un titre, une date, une heure de début, une description, charger une miniature et des balises – n’oubliez pas de baliser AltspaceVR :)
* Choisissez public dans le menu déroulant (la valeur par défaut est « non répertoriée »)
* Utilisation des valeurs par défaut
* Copier la clé de flux (coller dans l’encodeur)
* Pour voir votre véritable page vidéo de flux Live YouTube, vous devez sélectionner l’icône de partage en haut à droite. Il s’agit de votre lien d’événement de flux Live YouTube. vous pouvez le partager sur les réseaux sociaux avant votre événement réel !
* Maintenant, ouvrez OBS
* Fichier/paramètres
* STREAM
* Collez la clé de flux que vous avez copiée dans le champ de clé de flux.
* Appliquer, puis sur OK
* Sélectionnez « Démarrer la diffusion en continu »
* Dans YouTube, vous verrez que la fenêtre « Aperçu » affiche votre flux et que vous êtes en ligne.
* Sélectionner GO LIVE
* Vous êtes maintenant en ligne !
* Accédez à l’onglet de votre navigateur avec le lien « Afficher sur la page espion » ouvert pour vous assurer que la vidéo semble correcte. N’oubliez pas que vous n’entendez pas le son, car vous avez désactivé l’audio de vos navigateurs lorsque vous les avez mis en sourdine dans le mélangeur de volume Windows. Vérifiez le son sur votre téléphone ou demandez à un ami de vérifier le son pour vous.
* L’aspect est parfait !
* Alt-Tab de revenir à AltspaceVR pour déplacer votre appareil photo (c’est-à-dire votre avatar) dans votre événement.
* Une fois que vous avez terminé avec votre flux Live, revenez à la page « salle de contrôle en direct » de YouTube.
* Sélectionner « arrêter la diffusion en continu »
* S’ouvre et vous demande si vous souhaitez arrêter la diffusion en continu de l’événement en direct, OK
* Accédez à OBS et sélectionnez arrêter la diffusion.
* Félicitations, vous êtes maintenant un AltspaceVR.

Pour les points de bonus, partagez vos vidéos avec le monde sur les réseaux sociaux et veillez @AltspaceVR :)