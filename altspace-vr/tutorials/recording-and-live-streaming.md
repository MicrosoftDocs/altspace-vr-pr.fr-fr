---
title: Enregistrement et streaming en direct
description: Découvrez comment enregistrer et diffuser en direct vos événements AltspaceVR à partir de votre PC pour les promouvoir et les partager avec vos utilisateurs.
author: qianw211
ms.author: v-qianwen
ms.date: 11/1/2021
ms.topic: article
keywords: streaming, enregistrement, vidéo, audio, YouTube, OBS, en direct
ms.openlocfilehash: e82960097103df25c50f0b03b76d21e10b1cbbd6
ms.sourcegitcommit: 20605c50a93852f93a3464c5c339f6a7da67a047
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/03/2021
ms.locfileid: "131278977"
---
# <a name="recording-and-live-streaming"></a>Enregistrement et streaming en direct

L’enregistrement et la diffusion en continu de votre expérience AltspaceVR pour montrer d’autres personnes du monde entier sont un excellent moyen de promouvoir vos événements, AltspaceVR et VR en général ! Jetez un coup d’œil pour voir comment commencer.

Dans cet article, vous allez apprendre à :

* [Enregistrer AltspaceVR en mode 2D sur le PC](#recording-altspacevr-in-2d-mode-on-pc)
* [Flux Live vers YouTube dans AltspaceVR en mode 2D sur PC](#live-streaming-to-youtube-in-altspacevr-2d-mode-on-pc)

## <a name="recording-altspacevr-in-2d-mode-on-pc"></a>Enregistrement de AltspaceVR en mode 2D sur le PC

### <a name="the-short-version"></a>Version abrégée

1. Installez AltspaceVR et OBS (logiciel Open diffuser). Lancez AltspaceVR en mode 2D, lancez OBS, définissez OBS pour enregistrer AltspaceVR et enregistrer !

### <a name="the-slightly-longer-version"></a>Version légèrement plus longue

1. Consultez [https://obsproject.com/](https://obsproject.com/)
2. sélectionnez **Windows** pour télécharger OBS. Cette publication utilise **OBS v 26.1.1**
3. Installer OBS

### <a name="have-altspacevr-running-before-you-run-obs"></a>AltspaceVR en cours d’exécution avant d’exécuter OBS

1. Téléchargez et installez AltspaceVR à partir de notre site Web : [altvr.com/Get](https://altvr.com/getaltspacevr)
2. Si vous souhaitez stabiliser votre vidéo VR et éliminer les mouvements des têtes saccadées, veillez à utiliser le client 2D ou lancez AltspaceVR en mode 2D en débranchant le câble USB de votre casque sur votre PC. Si vous avez un Rift, appuyez sur Ctrl + Alt + Suppr, sélectionnez **services**, **service d’exécution Oculus VR**, cliquez avec le bouton droit, puis sélectionnez **arrêter**. Cela va entraîner la désactivation de Oculus et le démarrage de AltspaceVR en mode 2D. Répétez ces étapes et utilisez Start pour revenir en mode VR.
3. Vous pouvez également enregistrer votre expérience en mode VR, à l’aide de la capture de jeux avec OBS

Maintenant, Alt-Tab sur OBS :

1. Sous **scènes**, sélectionnez **+** et nommez votre nouvelle scène
2. Ensuite, sous **sources**, sélectionnez : **+ > la Capture de jeu > créer**
2. Modifiez Text en « AltspaceVR capture », Tick **Make source visible**, puis sélectionnez **OK** .
3. Double-cliquez sur **AltspaceVR capture** sous **sources**
4. Changer le **mode** pour **capturer une fenêtre spécifique**
5. Fenêtre : [AltspaceVR.exe] : AltspaceVR
6. Priorité de la fenêtre de correspondance : titre de correspondance, sinon Rechercher une fenêtre du même exécutable
7. Faites défiler jusqu’au **curseur de capture**: décochez
8. Sélectionnez **OK**.
9. Cela devrait faire apparaître AltspaceVR dans OBS.

maintenant, pour définir les propriétés suivantes dans OBS, accédez à **fichier > Paramètres**:

|Onglet|Paramètres|
|---|---|
| **Généralités** | Conservez la valeur par défaut |
| **Train** | Conservez la valeur par défaut |
| **Sortie** | Basculer vers la configuration avancée |
| **-Onglet streaming** | Piste audio 1 <br> Encodeur : x264 <br> Mise à l’échelle de la sortie : incochée <br> Contrôle de la fréquence : CBR <br> Débit binaire : 6000 (6000 pour 30 i/s ou 9000 pour 60 fps) <br> Intervalle d’image clé = 2 <br> Présélection de l’utilisation de l’UC = veryfast |
| **-Onglet Enregistrement** | Type : Standard. <br> Chemin d’enregistrement : D:/Video (accédez à l’emplacement où vous souhaitez enregistrer les fichiers vidéo) <br> Format d’enregistrement : MP4 (si vous recevez un incident lors de l’enregistrement, essayez FLV ici au lieu de MP4, si vous rencontrez un incident, la vidéo sera toujours utilisable avec FLV) <br> Piste audio 1 <br> Encodeur : utiliser l’encodeur de flux |
| **-Onglet Audio** | Débit binaire audio : 160 (pour toutes les pistes) |
| **-Onglet tampon de relecture** | Conservez la valeur par défaut |
| **Audio** | Taux d’échantillonnage : 44,1 kHz <br> Canaux : stéréo <br> Audio du Bureau : par défaut <br> Desktop audio 2 : désactiver <br> MIC/auxiliaires : par défaut |
| **Vidéo** | Résolution de base (canevas) : 1920 x 1080 <br> Résolution de sortie (mise à l’échelle) : 1920 x 1080 <br> Filtre réduire : bicubique (mise à l’échelle accentuée, 16 échantillons) <br> Valeurs d’FPS courantes : 30 (ou 60) |
| **Touches d’accès rapide** | Conservez la valeur par défaut |
| **Avancée** | Priorité du processus : normale | <br>

<br>Bien, veillez à sélectionner **appliquer**, puis cliquez sur **OK** pour enregistrer tous vos paramètres OBS. 

1. Alt-Tab à AltspaceVR, accédez à l’espace/au monde/à l’événement approprié et aligner votre appareil photo (autrement dit, votre avatar) nous sommes sur le point d’enregistrer une vidéo !
2. Alt-Tab sur OBS et, lorsque vous êtes prêt, cliquez sur **Démarrer l’enregistrement**.

Vous verrez en bas à droite de OBS que **Rec :** commence à compter et le point est rouge, ce qui signifie que vous enregistrez !

Procédez à un enregistrement de test : 
1. Dans AltspaceVR, ouvrez/fermez/survolé les menus pour créer des sons d’interface utilisateur
2. Assurez-vous que vous êtes bien désactivé, dites « sibilance, sibilance » ou demandez à un autre utilisateur de vous communiquer sur un volume normal.
3. Examinez les niveaux **audio** et **MIC/** aux au fur et à mesure que vous le faites pour vérifier si le contenu audio est correctement choisi.

En général, le micro/les est muet lors de l’enregistrement. Continuez et sélectionnez l’icône en forme de haut-parleur pour MIC/aux, et la couleur rouge avec un X.

* Il est très difficile de faire correspondre les niveaux audio de votre micro à l’audio de l’autre utilisateur, de sorte que le micro est le meilleur en sourdine lorsque vous enregistrez un événement.
* Un autre problème avec l’audio est la configuration de OBS. Il capture tout l’audio de votre ordinateur. Si vous regardez YouTube ou recevez des notifications sonores sur votre ordinateur, il enregistre ce fichier audio.
* pour enregistrer uniquement l’audio à partir de AltspaceVR, accédez à **ouvrir le mélangeur de Volume** (cliquez avec le bouton droit sur l’icône de haut-parleur en bas à droite de Windows) et désactivez les sons système, les navigateurs, etc., mais pas muet OBS ou AltspaceVR.

> PRÉCIEUSE N’oubliez pas de désactiver ces paramètres de mélangeur de volume après l’enregistrement.

À présent, revenez à OBS et sélectionnez **arrêter l’enregistrement**. Pour trouver la vidéo que vous venez d’enregistrer, accédez à **fichier>afficher les enregistrements**. Cela ouvre le dossier avec vos fichiers vidéo OBS, double-cliquez sur la vidéo de test.

Parfois, l’enregistrement est très bruyant. par conséquent, réduisez le curseur pour le son de bureau dans OBS et effectuez un autre enregistrement pour le test.

Pro-conseil : utilisez les touches Ctrl + Alt + P pour basculer en Mode photographie, mais supprimez l’interface utilisateur de votre affichage pour obtenir une bonne capture.

Vous êtes un enregistreur vidéo AltspaceVR !

## <a name="live-streaming-to-youtube-in-altspacevr-2d-mode-on-pc"></a>Streaming en direct vers YouTube en mode AltspaceVR 2D sur PC

### <a name="the-short-version"></a>Version abrégée

AltspaceVR et OBS doivent être installés. Lancez AltspaceVR et OBS. Vous pouvez soit diffuser en direct « maintenant », soit à une date ultérieure. Sur YouTube, configurez OBS avec votre clé de flux YouTube. Commencez la diffusion en continu dans OBS et dans YouTube, et vous êtes en concurrence !

### <a name="the-slightly-longer-version"></a>Version légèrement plus longue

Consultez la section [Recording AltspaceVR in 2D mode on PC](#recording-altspacevr-in-2d-mode-on-pc) en haut de cette page pour obtenir des instructions sur la façon de tester l’enregistrement à l’aide d’un enregistrement local au lieu du flux de données en direct et sur la configuration de la capture de votre appareil photo.

## <a name="setting-up-live-streaming-on-youtube"></a>Configuration de la diffusion en continu en direct sur YouTube

Vous pouvez obtenir un flux Live en direct, ou configurer un flux Live futur avec « date ultérieure ».

1. Ouvrez votre navigateur et connectez-vous [https://www.youtube.com/](https://www.youtube.com/) , puis accédez à [https://studio.youtube.com/](https://studio.youtube.com/)
2. Accédez au coin supérieur droit et sélectionnez **créer** , puis en **ligne**

Méthode **« Right Now »** :

1. Sélectionnez immédiatement **/Démarrer**
1. Sélectionner les **logiciels de streaming/Go**
1. Choisissez **modifier**, en haut à droite, pour modifier les détails et personnalisations de la vidéo.
1. sous **Paramètres de flux**, conservez les valeurs par défaut
1. En regard de **clé de flux (coller dans l’encodeur)**, **Copiez** la clé afin de pouvoir la coller dans OBS
1. ouvrir le flux OBS/ **Paramètres**  /  
1. Dans le menu déroulant **service** , sélectionnez **YouTube-RTMPS**
1. Collez la clé de flux de YouTube dans le champ de **clé de flux** dans OBS
1. Cliquez sur **appliquer**, puis sur **OK** .
1. Sélectionnez **Démarrer la diffusion en continu** dans OBS
1. Basculez vers YouTube et vous verrez que vous êtes désormais en ligne sur YouTube !
1. Pour afficher la page vidéo de flux Live YouTube, vous devez sélectionner l’icône partager en haut à droite.
1. Cliquez sur la « liaison vidéo » pour voir et entendre votre flux YouTube Live 
1. Cette URL est votre lien de flux Live et peut être partagée vers tous vos canaux de réseaux sociaux :)
1. Pour arrêter le flux en direct, sélectionnez END STREAM sur YouTube, puis arrêter la diffusion sur OBS

Méthode «**date ultérieure**» :
1. En haut à gauche, choisissez l’icône **gérer**
1. Sélectionner un **flux de planification**, en haut à droite
1. Ajouter un titre, une description, une catégorie, une miniature (1280 x 720), puis **suivant**
1. Options de conversation en direct, puis **suivant**
1. Privé, non répertorié ou public (choisir public)
1. Planifiez la date et l’heure auxquelles vous souhaitez vous connecter, puis **faites** -le

 **Lorsque vous êtes prêt à démarrer votre flux Live à l’avenir :**
1. sous Paramètres de flux, conservez les valeurs par défaut
1. En regard de **clé de flux (coller dans l’encodeur)**, **Copiez** la clé afin de pouvoir la coller dans OBS
1. ouvrir le flux OBS/ **Paramètres**  /  
* Dans le menu déroulant **service** , sélectionnez **YouTube-RTMPS**
1. Collez la clé de flux de YouTube dans le champ de **clé de flux** dans OBS
1. Cliquez sur **appliquer**, puis sur **OK** .
1. Sélectionnez **Démarrer la diffusion en continu** dans OBS
1. Basculez vers YouTube et vous verrez que vous êtes désormais en ligne sur YouTube !
1. Pour afficher la page vidéo de flux Live YouTube, vous devez sélectionner l’icône partager en haut à droite.
1. Cliquez sur la « liaison vidéo » pour voir et entendre votre flux YouTube Live 
1. Cette URL est votre lien de flux Live et peut être partagée vers tous vos canaux de réseaux sociaux :)
1. Pour arrêter le flux en direct, sélectionnez **end Stream** sur YouTube, puis **arrêter la diffusion** sur OBS

Pour les points de bonus, partagez vos vidéos sur les réseaux sociaux et veillez à les baliser @AltspaceVR :)