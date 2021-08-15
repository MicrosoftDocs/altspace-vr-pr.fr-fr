---
title: Utilisation de la console multimédia
description: Découvrez comment démarrer la configuration, la publication et le contrôle de la console multimédia dans vos expériences AltspaceVR.
ms.date: 03/11/2021
ms.topic: article
keywords: console, multimédia
ms.openlocfilehash: a24b3700f1687aed6bc00fd218aacd7cc12908e521af6239fac0ae97f48b4b9a
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/11/2021
ms.locfileid: "119127366"
---
# <a name="using-the-multimedia-console"></a>Utilisation de la console multimédia

La console multimédia est un outil qui permet le partage de médias dans les événements et les mondes. Vous pouvez l’utiliser pour partager des éléments tels que des images, des diapositives de présentation, des livestreams, des vidéos, des sélections, etc. Vous trouverez ci-dessous une instruction pas à pas sur l’utilisation de la console multimédia **v 0.5.0 +**. 

## <a name="getting-started"></a>Prise en main

La prise en main de la console multimédia est un processus en deux parties.  Tout d’abord, le portail Web que vous utiliserez pour générer et publier une configuration pour la session de console multimédia que vous placez dans votre environnement.  Deuxièmement est le placement de l’application de console multimédia réelle dans votre environnement et la définition du code de configuration qu’elle doit utiliser.

### <a name="configuring-the-multimedia-console-with-the-web-portal"></a>Configuration de la console multimédia avec le portail Web

1. Tout d’abord, vous devez vous assurer que votre contenu est hébergé en ligne, car vous aurez besoin d’une URL. (Vous pouvez télécharger des photos sur altvr.com, héberger une vidéo .mp4 fichier en ligne ou utiliser un lien Dlive Live Stream : https://dlive.tv/yourlivestream) 
2. Accédez au portail Web pour la console multimédia à l’adresse [https://multimedia-console.altvr.com/](https://multimedia-console.altvr.com/)
3. À partir du portail Web, vous pouvez générer et publier une configuration pour la console multimédia.  (Voir ci-dessous pour plus d’informations sur les différentes propriétés).
4. Une fois que vous avez entré le média dans la liste des médias et que vous avez configuré les paramètres généraux, sélectionnez le bouton publier dans la partie supérieure droite de l’application.
5. Une fois la publication terminée, une boîte de dialogue s’affiche avec un code de deux mots que vous pouvez entrer dans la console multimédia que vous avez placée.
  
### <a name="placing-the-multimedia-console-in-your-environment"></a>Placement de la console multimédia dans votre environnement

1. Sélectionnez **éditeur > panneau de l’éditeur > applications SDK > console multimédia**. (N’accédez pas à l' **éditeur World > notions de base > application SDK**, pour les applications non inscrites.)  
2. Placez la console multimédia sur la suite la mieux adaptée à votre espace et à votre public.
3. Quittez le mode d’édition en cliquant sur le bouton orange en mode d’édition.
4. Vous êtes invité à indiquer **le propriétaire du lecteur multimédia ?** Si vous êtes la personne qui doit être le propriétaire officiel de cette session de console multimédia, confirmez et continuez. (D’autres rôles permissions sont également disponibles. Pour obtenir une liste détaillée, voir ci-dessous.)
5. Sélectionnez Oui pour confirmer que vous êtes l’hôte principal.  
6. Une boîte de dialogue s’affiche pour vous demander d’entrer un code à partir du portail Web ou un JSON valide.  Entrez les deux codes de mot du portail Web, y compris le tiret, puis appuyez sur OK. (JSON est une configuration avancée décrite ci-dessous)
7. La console multimédia doit être chargée après quelques secondes avec la configuration que vous avez créée dans le portail Web.

### <a name="controlling-the-multimedia-console"></a>Contrôle de la console multimédia

1. Une fois que vous avez entré votre code et terminé le processus de configuration, vous voyez s’afficher les boutons de contrôle sous un affichage de média. 
    * **Play** démarre la visionneuse multimédia (ou redémarre à l’entrée en cours, si elle s’est arrêtée précédemment) 
    * **Arrêter** arrête la visionneuse multimédia et masque le média actuel.  
    * **Suivant/précédent** passe au support suivant ou précédent 
    * **x/x**   affiche l’index actuel dans la liste des médias et vous permet d’accéder à n’importe quel point de la liste
    * La **configuration permet de** réentrer un nouveau code à partir du portail Web pour définir une nouvelle configuration dans la console. 

Vous êtes maintenant prêt à commencer le partage via la console multimédia !  
 
## <a name="working-with-the-web-portal"></a>Utilisation du portail Web

Le portail Web est une application Web qui permet de configurer les différentes fonctionnalités de la console multimédia.  Ces fonctionnalités se répartissent en deux catégories : les paramètres généraux de la console média et la liste des médias.

### <a name="multimedia-console-general-settings"></a>Paramètres généraux de la console multimédia

**Paramètres Playback**

Paramètres de lecture généraux pour la liste des médias

* **Liste des médias en boucle**: détermine si la liste des médias doit boucler une fois que vous avez atteint la fin de la liste.
* **Start, méthode** : sélectionne la méthode par laquelle la console multimédia doit démarrer.
    * Manuel : attend que le bouton de lecture soit enfoncé avant de démarrer le média.
    * Démarrage automatique à partir du début-démarre automatiquement la liste des médias à partir du début de la liste
    * Démarrage automatique aléatoire : démarre automatiquement le support à partir d’un point de départ aléatoire dans la liste

**Rôles**

Attributions de rôles pour le contrôle et la configuration de la console multimédia.    Ces rôles sont décomposés dans l’ensemble suivant :

* **Propriétaire uniquement** : utilisateur propriétaire de la session de la console multimédia
* **Utilisateurs avec élévation de privilèges** : utilisateurs disposant d’un modérateur ou de rôles d’hôte dans l’espace dans lequel la console multimédia est configurée à l’origine
* **Tous les utilisateurs** -tous les utilisateurs

Ces rôles empilent dans le sens que tous les rôles au-dessus de celui choisi dans cette liste seront également autorisés à utiliser cette fonctionnalité.  Exemple : les **utilisateurs avec élévation de privilèges** incluent le **propriétaire** même s’ils ne sont pas un modérateur ou un hôte * * dans AltspaceVR. Les fonctionnalités contrôlées par les attributions de rôles sont les suivantes :

* **Peut contrôler le lecteur multimédia** : détermine les rôles qui peuvent contrôler les boutons de lecture du média pour la console multimédia.
* **Peut configurer le lecteur multimédia** : détermine les rôles qui peuvent configurer la console multimédia en lui accordant l’accès au bouton de **configuration**

### <a name="adding-photos-and-videos-to-the-media-list"></a>Ajout de photos et de vidéos à la liste des médias

Le média est le cœur de la console multimédia.  Les images et les liens vidéo sont pris en charge en tant que types de média dans la console multimédia.  Pour ajouter un nouveau média, sélectionnez les icônes **Ajouter une image** ou ajouter une **vidéo** pour afficher une boîte de dialogue pour entrer les informations et les paramètres du média.  Voici la répartition des types de médias et des paramètres associés

**Image**

Les images doivent être un type d’image standard comme JPEG, png et fils sur. Ils doivent être hébergés dans un emplacement avec un lien public.

* **Nom** -(obligatoire) nom avec lequel vous souhaitez identifier l’image.
* **URL** de l’image : (obligatoire) URL publique de l’image
* **Ignorer après** : nombre de secondes pendant lequel l’image doit être ignorée après

**Vidéo**

Les vidéos peuvent être des vidéos hébergées ou des flux en direct via Twitch et DLive.  (Un autre support peut fonctionner avec un travail supplémentaire pour récupérer l’URL de flux appropriée, mais n’est pas entièrement pris en charge dans la console multimédia)

* **Nom** : nom (obligatoire) avec lequel vous souhaitez identifier la vidéo.
* **URL** de la vidéo : (obligatoire) URL à partir de laquelle la vidéo est hébergée ou à partir de laquelle le flux en direct est servi.
* **Ignorer après** : nombre de secondes pendant lesquelles la vidéo doit être ignorée après

> [!NOTE]
> OBLIGATOIRE : placez dans le temps qui correspond à la longueur de la vidéo pour permettre aux vidéos de se transférer correctement. Par exemple, si votre vidéo dure 5 minutes à 300 secondes, dans le cas contraire, votre vidéo ne passera pas à la partie suivante du contenu.

* **Volume** : volume de la vidéo de 0 (min)-1 (max) valeurs.
* **Heure de début** : nombre de secondes à partir du début de la vidéo à partir de.
* **Distance de début** de l’annulation : distance en mètres dans le monde selon laquelle le volume commence à tomber à mesure que vous quittez la console multimédia
* **Action de fin de vidéo** -action à effectuer une fois la fin de la vidéo atteinte.
    * Arrêter : la liste des médias s’arrête après la fin de la vidéo
    * Loop : la vidéo est en boucle jusqu’à ce qu’elle soit ignorée manuellement
    * Lire suivant : le média suivant dans la liste des médias sera démarré après la fin de la vidéo actuelle.

## <a name="working-with-json-directly-advancedoptional"></a>Utilisation directe de JSON (avancé/facultatif)

La console multimédia prend en charge l’entrée de JSON directement dans à l’invite de la console dans AltspaceVR.  JSON est le mécanisme interne avec lequel nous activons les configurations de lecteur multimédia. L’exposition de la possibilité de définir JSON directement est un outil qui permet aux utilisateurs plus expérimentés de créer leurs propres flux de travail qui reposent leurs besoins et leur familiarité avec JSON.  Vous trouverez ci-dessous une brève description de la structure JSON et du schéma par lequel le JSON est validé. Pour obtenir une description plus détaillée des propriétés ci-dessous, consultez les sections ci-dessus relatives à la configuration de la console multimédia.  Cette section se concentre principalement sur les exemples de schémas et la structuration des données JSON.

### <a name="global-media-settings"></a>Paramètres multimédias globaux

```json
{
  "loopMediaList": true | false
  "startMethod": "manual" | "autostart-beginning" | "autostart-random"
  "controlMediaPlayer": "everyone" | "elevated" | "owner"
  "configureMediaPlayer": "elevated" | "owner"
  ...
}
```

### <a name="media-list"></a>Liste des médias

la liste des médias est une propriété définie à la racine de la structure JSON, comme les rôles et la lecture Paramètres.  Il s’agit d’un tableau simple qui peut contenir l’une des structures de configuration de média suivantes. (Consultez les descriptions de propriétés ci-dessus pour plus d’informations sur ce que fait.)

**Exemple d’image**

*Champs obligatoires : « Name » et « imageUrl »*

```json
{
    "name": "Altspace Screenshot",
    "imageUrl": "https://pbs.twimg.com/media/CxJ-fJqUsAAFtd9.jpg",
    "skipAfter": 10
}
```

**Exemple de vidéo**

*Champs obligatoires : « Name » et « videoUrl »*

```json
{
    "name": "Ninja Twitch Live Stream",
    "videoUrl":"https://www.twitch.tv/ninja",
    "volume":0.2,
    "startTime":0,
    "endOfVideoAction":"play-next"
}
```

### <a name="example-json"></a>Exemple JSON

```json
{
  "loopMediaList": false,
  "startMethod": "autostart-beginning",
  "controlMediaPlayer": "everyone",
  "configureMediaPlayer": "elevated",
  "mediaList": [
    {
      "videoUrl": "https://www.twitch.tv/ninja",
      "volume": 0.2,
      "startTime": 0,
      "endOfVideoAction": "play-next"
    },
    {
      "imageUrl": "http://www.hypergridbusiness.com/wp-content/uploads/2016/09/AltspaceVR-highrise.jpg",
      "skipAfter": 10
    },
    {
      "imageUrl": "https://d1qb2nb5cznatu.cloudfront.net/startups/i/333629-6ffd7199b9bcf34d8957e8e09d974a38-medium_jpg.jpg?buster=1423092095",
      "skipAfter": 5
    },
    {
      "imageUrl": "https://pbs.twimg.com/media/CxJ-fJqUsAAFtd9.jpg",
      "skipAfter": 10
    },
    {
      "imageUrl": "https://altvr-wpengine.netdna-ssl.com/wp-content/uploads/2019/05/Educators-in-VR-Social-VR-AltspaceVR.png",
      "skipAfter": 10
    },
    {
      "videoUrl": "https://www.twitch.tv/shroud",
      "volume": 1,
      "startTime": 0,
      "endOfVideoAction": "stop"
    }
  ]
}
```

### <a name="schema"></a>schéma

```json
{
  "$schema": "https://json-schema.org/draft-04/schema#",
  "type": "object",
  "required": [
    "mediaList"
  ],
  "properties": {
    "loopMediaList": {
      "type": "boolean",
      "description": "Whether to loop through the media list when reaching the beginning or end of the list."
    },
    "controlMediaPlayer": {
      "type": "string",
      "enum": [
        "everyone",
        "elevated",
        "owner"
      ],
      "default": "owner",
      "description": "What roles are able to control the media player. (Owner can always control player)"
    },
    "configureMediaPlayer": {
      "type": "string",
      "enum": [
        "elevated",
        "owner"
      ],
      "default": "owner",
      "description": "What roles are allowed to configure the media play list.  Note: This role needs to be able to control the media player in order to configure it. (Owner can always configure media)"
    },
    "startMethod": {
      "type": "string",
      "enum": [
        "manual",
        "autostart-beginning",
        "autostart-random"
      ],
      "default": "manual",
      "description": "The method by which the media player should start"
    },
    "mediaList": {
      "description": "A list of images or videos to configure the media player to operate on.",
      "type": "array",
      "items": {
        "oneOf": [
          {
            "title": "Image",
            "type": "object",
            "description": "Configuration for an image media.",
            "properties": {
              "imageUrl": {
                "type": "string",
                "description": "The url for the image to load."
              },
              "skipAfter": {
                "type": "number",
                "minimum": 5,
                "default": null,
                "description": "The number of seconds that should pass before skipping to the next media. (Minimum 5)."
              }
            },
            "required": [
              "imageUrl"
            ]
          },
          {
            "title": "Video",
            "type": "object",
            "description": "Configuration for a video media.",
            "properties": {
              "videoUrl": {
                "type": "string",
                "description": "The url of the video to load."
              },
              "skipAfter": {
                "type": "number",
                "minimum": 5,
                "default": null,
                "description": "The number of seconds that should pass before skipping to the next media. (Minimum 5)."
              },
              "volume": {
                "type": "number",
                "minimum": 0,
                "maximum": 1,
                "default": null,
                "description": "The volume to play the video at. (Minimum 0, maximum 1)"
              },
              "startTime": {
                "type": "number",
                "minimum": 0,
                "default": null,
                "description": "The time in seconds from the start of the video to begin playing the video at. (Minimum of 0)"
              },
              "rolloffStartDistance": {
                "type": "number",
                "minimum": 0,
                "default": null,
                "description": "The distance in meters away from the media player that the volume will begin to fall off. (Minimum 0)"
              },
              "endOfVideoAction": {
                "type": "string",
                "enum": [
                  "stop",
                  "loop",
                  "play-next"
                ],
                "default": null,
                "description": "The type of action to take at the end of the video."
              }
            },
            "required": [
              "videoUrl"
            ]
          }
        ]
      }
    }
  }
}
```

> [!NOTE]
> À jour avec la console multimédia v 0.5.0