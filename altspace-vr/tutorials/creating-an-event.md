---
title: Création d’un événement
description: En savoir plus sur les événements AltspaceVR, sur la façon de les créer et d’ajouter des personnalisations et des objets 3D avec l’éditeur de monde.
ms.date: 03/11/2021
ms.topic: article
keywords: événements, terminologie, console, multimédia, éditeur universel, flux en direct
ms.openlocfilehash: 0c6e59604339ad354dc0241ca81335f92d65b0845529f6d1fe5eb2eb0d18627f
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/11/2021
ms.locfileid: "119127451"
---
# <a name="creating-an-event"></a>Création d’un événement

Il s’agit d’un guide pas à pas pour la création d’événements dans AltspaceVR. Il est fortement recommandé d’assister à plusieurs événements dans AltspaceVR pour avoir une idée de leur fonctionnement. Consultez le [calendrier des événements AltspaceVR](https://account.altvr.com/events) pour obtenir la liste de tous nos événements.

Cet article porte sur les points suivants :

* Terminologie des événements AltspaceVR
* Création de votre événement et de votre espace d’événements ou de votre monde
* Utilisation de la console multimédia pour une présentation de diapositives
* Personnalisation de votre événement à l’aide d’images
* Ajout d’objets 3D à l’aide de l’éditeur/kits World
* Comment enregistrer ou Flux temps réel mon événement

## <a name="altspacevr-event-terminology"></a>Terminologie des événements AltspaceVR

Vous devez connaître les termes suivants pour créer votre événement et votre espace d’événements :

</br>

| Terme | Définition |
|---|---|
| Génération mondiale | AltspaceVR offre la possibilité de créer et de personnaliser des mondes virtuels. AltspaceVR héberge la documentation de support, les canaux de distribution et les événements dans le monde pour vous aider à [en savoir plus sur la façon d’obtenir de l’aide et de commencer à créer des mondes](../world-building/world-building-faq.md). |
| World (Monde) | Un monde est un espace virtuel dans AltspaceVR. Il peut s’agir d’un bureau ou d’un large éventail de montagnes. Il s’agit d’un environnement hautement personnalisable. Il se trouve dans un univers et il peut y avoir plusieurs mondes au sein de cet univers. Si vous souhaitez avoir plusieurs espaces d’événements pour les événements spéciaux, les centres de formation et les différents espaces de réunion pour améliorer votre travail, ajoutez les mondes sous le même univers pour les rassembler en groupe. |
| Univers | Un univers dans AltspaceVR World Building Vernacular représente la catégorisation de vos mondes. Chaque univers peut contenir plusieurs mondes. Les mondes héritent des paramètres de l’univers, ce qui facilite l’ajout de personnes à la liste verte pour plusieurs mondes et autres fonctionnalités de contrôle. Pour plus d’informations, consultez [gestion de vos mondes](../world-building/managing-worlds.md) . |
| Modèle | Un modèle (ou modèle d’espace) est un environnement ou un environnement prédéfinis qui peut être utilisé au lieu d’en créer un à l’aide des fonctionnalités de création de monde. AltspaceVR offre une large gamme de modèles pour différentes expériences et événements. |
| Espace d’événements | Un espace d’événements est un synonyme de World dans AltspaceVR. En général, il fait référence à un monde utilisé pour héberger des événements. |
| Site web | Les références au « site Web » sont le [site Web de AltspaceVR](https://altvr.com/). Il est souvent plus facile de créer et de modifier des événements via la [page Web événements](https://account.altvr.com/events/my) sur un ordinateur ou une tablette, plutôt que via votre appareil VR. Vous devez également accéder au site Web pour le [monde entier](../world-building/managing-worlds.md) . |
| Rôles contextuels | Les [rôles contextuels](../getting-started/roles.md) sont assignés par le créateur d’événements ou le générateur de monde. Ces rôles offrent aux utilisateurs dans un monde entier ou des fonctions et fonctionnalités supplémentaires. À l’heure actuelle, il s’agit de l’hôte, du modérateur, du pilote (vol), de terraformer (bâtiment universel) et de mégaphone uniquement. Ils peuvent être attribués individuellement ou globalement, ce qui permet à tous les utilisateurs d’avoir les mêmes rôles dans l’espace ou le monde de l’événement. |
| Interface utilisateur (IU)/menu | Lorsque vous êtes dans AltspaceVR dans le monde entier, il y a des menus à gauche et à droite de votre écran. Le cercle ou le menu principal avec le logo AltspaceVR ouvre l’interface utilisateur principale (IU) ou le menu permettant d’accéder à différents écrans permettant d’explorer AltspaceVR et de personnaliser votre expérience. Les éléments d’interface utilisateur facultatifs se trouvent à la bonne taille de l’écran et incluent généralement l’éditeur de monde et les outils hôtes. Vous pouvez les ouvrir et interagir avec en cliquant dessus avec votre curseur. |
| SDK/MRE | Il s’agit des conditions générales associées au kit de développement logiciel (SDK) et aux [extensions de réalité mixte](../world-building/using-mixed-reality-extensions.md) utilisées pour ajouter des fonctionnalités et des fonctionnalités à l’expérience de création mondiale. Ils sont généralement destinés aux utilisateurs plus expérimentés. |

## <a name="understanding-events"></a>Fonctionnement des événements

AltspaceVR facilite la création d’un monde dans lequel vous pouvez utiliser un espace de modèle prédéfini pour l’utiliser ou le personnaliser pour vos besoins spécifiques, ou créer un monde à partir de zéro. Cet article aborde l’utilisation d’un modèle prédéfini pour créer votre événement. Les sections ci-dessous sur la [Personnalisation de votre événement avec des images](#branding-your-event-with-images) et [l’ajout d’objets 3D à l’aide de l’éditeur et des kits](#adding-3d-objects-using-world-editor-and-kits) sont des conseils pour une personnalisation plus poussée. Pour plus d’informations sur la création d’un monde personnalisé à partir de zéro, participez à la visite guidée du monde rassemblements dans AltspaceVR et [consultez la documentation du support Building World](../world-building/world-editor-getting-started.md).

AltspaceVR propose deux méthodes pour créer un espace pour votre événement.

* **Utilisation ponctuelle :** Créez un événement et sélectionnez un monde de modèles.
* **Utilisation répétée :** Créez un espace universel et importez-le dans l’événement.

Le processus de création d’un événement est le même pour les deux, à une exception près : la [création d’un monde et son importation](../world-building/managing-worlds.md) sous la forme d’un espace d’événements REPEAT-use. Vous devez également connaître les éléments suivants :

</br>

| Terme | Définition |
|---|---|
| Copie du monde | L’utilisation d’un espace universel pour un événement répété permet une personnalisation permanente. Les signes, les images, les points de génération et d’autres personnalisations sont conservés d’un événement à l’autre au lieu de personnaliser l’espace d’événement à chaque fois. |
| Personnaliser le monde des événements | Lorsqu’un événement est créé, le modèle ou le monde importé est copié et verrouillé dans cet événement. Vous pouvez apporter des modifications au monde de l’événement et ne pas avoir d’impact sur le monde d’origine, et l’inverse. Envisagez d’ajouter des décorations, des images ou d’autres éléments décoratifs à l’aide d’un éditeur de monde unique pour rendre l’espace d’événement plus agréable et approprié à l’événement. |

Les modifications apportées au monde d’origine ne seront pas dans le monde de l’événement, sauf si l’espace de l’événement est mis à jour :
1. Utilisez le bouton **RÉimporter le monde** dans la page Web de l’événement.
2. Autorisez 2-3 minutes avant la fin de la synchronisation. 
3. si l’espace de l’événement n’a pas changé, accédez à **Paramètres > modéré > réinitialiser l’espace** pour réinitialiser l’espace de l’événement. Vous allez réinitialiser l’espace d’un grand nombre en tant que générateur de monde !

si vous avez des problèmes techniques, tels que les éléments ne se chargent pas correctement, accédez à votre menu AltspaceVR et sélectionnez **Paramètres > modéré > réinitialiser l’espace** pour réinitialiser l’espace d’événements et voir les nouvelles modifications. Windows Les utilisateurs de PC en 2D peuvent utiliser le raccourci clavier : **Ctrl + Alt + R** dans AltspaceVR pour réinitialiser rapidement l’espace.

## <a name="creating-your-event-and-event-space-or-world"></a>Création de votre événement et de votre espace d’événements ou de votre monde

Voici des instructions pas à pas pour créer un événement pour un événement unique ou répété. En sélectionnant le modèle ou en important un monde pour l’événement. 

> [!NOTE]
> La page Web événements AltspaceVR fournit des instructions sur chaque aspect du formulaire à l’aide des boutons de point d’interrogation verts. Pour obtenir des instructions spécifiques, remontez votre curseur dessus.

Dans la page [événements > mes événements](https://account.altvr.com/events/my) du site Web de AltspaceVR, sélectionnez **planifier un événement** ou accédez directement à la [page Web créer un événement dans AltspaceVR](https://account.altvr.com/events/new).

1. **Titre de l’événement :** Tapez le nom de l’événement. Assurez-vous qu’elle est spécifique et concise pour l’affichage sur les différents affichages de calendrier sur le site Web de AltspaceVR et l’interface dans le monde. Essayez de conserver votre titre sous 23 caractères, y compris les espaces entre les mots.
2. **Description :** Tapez la description de l’événement.
    * Doit comporter au moins 10 caractères dans la description, sans quoi votre événement ne sera pas créé.
    * Ajoutez un espace vide entre les paragraphes.
    * Pour ajouter un lien vers le site Facebook, le discordon, le site Web ou d’autres ressources, utilisez le format suivant (cette démarque fonctionne uniquement sur la page de promotion de votre événement sur le site Web, ce rendu ne s’affiche pas correctement dans les menus AltspaceVR) : `[Event Name](http://example.com/)`

3. Date de **début/Date de fin :** Définissez l’heure de début et assurez-vous que l’heure de fin est postérieure à l’heure de début.
4. **Catégorie :** Choisissez la catégorie qui décrit le mieux votre type d’événement. 
5. Définissez l’événement sur **privé** ou **public**.
    * Visibilité : les événements publics sont visibles dans l' [onglet tout](https://account.altvr.com/events/all) du calendrier des événements de site Web AltspaceVR et sont ouverts au public.
    * Les événements privés ne sont pas visibles dans les calendriers des événements AltspaceVR et requièrent que l’URL de l’événement entre dans l’espace de l’événement.
    * Si vous souhaitez « ajouter en tant qu’événement principal », l’événement doit être défini sur public.
6. **Sélectionnez un modèle :** Le long du côté droit de la page Web est une liste d’images miniatures des modèles disponibles dans AltspaceVR. Il existe des salles de jeu, des bureaux, des espaces de réunion, des espaces de présentation et des espaces Meetup amusants. Sélectionnez une apparence intéressante. Si ce n’est pas le cas, n’hésitez pas à créer un nouvel événement avec un nouveau modèle. Si vous souhaitez créer votre propre environnement d’événements personnalisé, sélectionnez le **ciel cool** comme modèle par défaut et suivez les instructions ci-dessous pour importer votre monde.
7. Sélectionner les **Options avancées**

### <a name="advanced-options"></a>Options avancées

1. **Promouvoir :** Chaque événement requiert deux images de personnalisation (ces images s’affichent sur le site Web AltspaceVR et n’apparaissent pas dans votre événement dans AltspaceVR) :
    * **Vignette :** L’image de la vignette doit être 1920 x 1080 pixels. Cette image sera mise à l’échelle en fonction des différentes tailles de miniatures et affichée dans le calendrier des événements AltspaceVR avec d’autres événements. Assurez-vous que l’image est claire et qu’elle n’est pas très importante. N’utilisez pas d’images/logos droits d’auteur dont vous n’êtes pas propriétaire.
    * **Bannière :** Les images de bannière doivent être 1920x576. Ce sera automatiquement redimensionné en fonction des besoins et sera visible dans les informations sur l’événement ou la page Web. Une superposition semi-transparente couvre les 25% inférieurs de l’image. Évitez de placer du texte dans cette zone.
    * Une autre option (plus rapide) consiste à copier l’image **de vignette sur une image de bannière d’arrière-plan**, qui utilise également votre image de vignette comme image de bannière. Essayez :). Si le résultat n’est pas correct, vous pouvez créer une nouvelle image de bannière.
2. **En VR :** Cette section comprend des fonctionnalités qui s’appliquent à l’expérience virtuelle pendant l’événement à l’intérieur de l’application AltspaceVR :
    * **Rôles contextuels par défaut :** Le point d’interrogation vert répertorie les rôles spécifiques disponibles pour *tous les membres du public dans l’événement*. Le plus courant est *megaphone_only*. Ajoutez ceci pour attribuer à l’option « amplifier ma voix », sous le bouton outils de l’ordinateur hôte, tous les membres de l’audience, afin qu’ils puissent être entendus dans votre événement s’il s’agit d’un espace important. Si votre événement requiert Flight, ajoutez le *pilote*. Pour les ajouter, le format est le suivant : *megaphone_only, pilote*. chaque utilisateur doit activer le mode de vol dans l’application AltspaceVR en accédant à Paramètres/Input/Fly.
    * **Instructions :** Les [instructions s’affichent](../world-building/adding-welcome-messages.md) pour le texte qui génère une image de bienvenue à l’arrivée dans l’espace. Les utilisateurs doivent sélectionner « OK » pour le supprimer de leur affichage. Il est souvent utilisé pour fournir des instructions d’assistance telles que « Restez en sourdine jusqu’à ce qu’il soit invité à parler » ou « Bienvenue à l’événement XYZ où nous allons nous intéresser à ABC ». Cela n’est pas obligatoire, donc utilisez judicieusement. Vous pouvez également utiliser la démarque pour ajouter le dimensionnement de la couleur et de la police, plus de détails : [http://digitalnativestudios.com/textmeshpro/docs/rich-text](http://digitalnativestudios.com/textmeshpro/docs/rich-text)
3. **Avancé :** Vous trouverez ci-dessous une explication rapide des fonctionnalités avancées des événements (certaines de ces fonctionnalités ne s’affichent pas tant que l’événement n’a pas été créé et que vous ne modifiez pas l’événement) :
    * **Administrateurs :** Les administrateurs sont des utilisateurs AltspaceVR auxquels vous faites confiance pour vous aider à gérer votre événement. Il peut s’agir de vos cohôtes ou de vos hôtes de sauvegarde. En ajoutant leur nom d’utilisateur à la liste des administrateurs, ils peuvent :
        * Modifiez le titre, la description et d’autres fonctionnalités de l’événement.
        * Ajoutez et supprimez des rôles contextuels pour les modérateurs, les hôtes et les autres rôles.
        * Supprimez l’événement.
    * **Groupe :** Choisissez parmi vos [groupes](group-features.md) privés à l’aide du menu déroulant. S’affiche uniquement si votre compte a été créé ou ajouté à un groupe.
    * **Slogan :** Cette phrase concise s’affiche sur la page Web de l’événement sous le titre.
    * **Importer à partir du monde :** Pour utiliser un espace de l’événement universel créé pour une utilisation répétée, il s’agit de la section du formulaire à utiliser pour importer la disposition et la personnalisation du monde dans votre événement. Tenez compte des points suivants :

    **Importez votre propre monde :** Pour importer un monde, vous avez créé et êtes propriétaire des éléments suivants :
    * Sélectionnez la flèche déroulante pour afficher la liste des mondes que vous avez créés.
    * Sélectionnez le monde.
    * Après avoir terminé le reste du formulaire d’événement, attendez au moins 2 minutes avant de consulter l’espace d’événements dans AltspaceVR pour vous assurer que les informations de la base de données sont mises à jour et que le monde est généré.
    
    **Utilisez le monde de quelqu’un d’autre :**
    * Contactez le propriétaire du monde pour demander à ce qu’il utilise la fonctionnalité **partager avec les amis** sur un monde individuel pour le partager avec vous.

3. **ID vidéo YouTube :** Visible sur la page Web de l’événement, cela ajoute des codes de fin ou des vidéos d’événements YouTube à la page Web d’événement, pas dans le monde. Vous n’aurez besoin que de la partie ID vidéo de l’URL : dQw4w9WgXcQ
4. **Gestionnaire Twitter :** Vous ajoutez ainsi votre flux Twitter à la page Web de l’événement. Si le compte Twitter est personnel et non lié à l’événement ou à l’Association, vous êtes peut-être en cours de partage. Vous n’aurez besoin que du descripteur : @elonmusk
5. **Rôles contextuels :** C’est là que vous contrôlez les super pouvoirs ou les [rôles contextuels](../world-building/granting-roles.md) de vos hôtes d’événements, modérateurs et autres rôles au sein de l’événement. Pour les ajouter, entrez leur nom d’utilisateur AltspaceVR et affectez-leur un rôle dans le menu déroulant. Pour les supprimer, activez la case à cocher pour supprimer et enregistrer la page Web de l’événement. Remarque : Si vous souhaitez accorder une fonctionnalité de modération de l’hôte, vous devez les ajouter en tant qu’hôte et modérateur. Les rôles contextuels suivants sont actuellement disponibles :
    * **Hôte :** Ajoute les [fonctionnalités de ligne avant](../faqs/front-row-events.md) à l’interface de la personne dans AltspaceVR pour ajouter ces fonctionnalités.
    * **Modérateur :** Ajoute des fonctionnalités de modération à l’interface d’un individu, y compris la possibilité de texte pour chaque participant, de le désactiver globalement pour l’événement ou de les supprimer de l’événement. Rajoutez l’ordinateur hôte et donnez-lui des rôles de modération si vous souhaitez qu’ils aient des privilèges de modération.
    * **Mégaphone uniquement :** Ajoute le bouton amplifier ma voix à leur interface via le bouton outils de l’ordinateur hôte.
    * **Terraformer :** Ajoute le bouton éditeur de monde à leur interface.
    * **Pilote :** Ajoute des fonctionnalités de vol pour cette personne. remarque : ils doivent l’activer dans Paramètres/Input/Fly
    * **Intervenant musical :** Ajoute des fonctionnalités et des fonctionnalités associées à des événements de concert et de musique.
6. **Bloquer les utilisateurs listés :** Si vous souhaitez empêcher un utilisateur d’accéder à un utilisateur ou qu’un utilisateur a été précédemment supprimé de l’événement par un modérateur ou un hôte et si l’événement a été dupliqué, le nom de l’utilisateur de la liste rouge apparaîtra dans la liste. Les hôtes d’événements ou les administrateurs peuvent ajouter ou supprimer un blocage de l’utilisateur dans la liste à tout moment.

Une fois le formulaire terminé et triple coché, sélectionnez **créer un événement**.

> [!IMPORTANT]
> Si votre événement n’est pas créé correctement, assurez-vous que vous avez au moins 10 caractères dans votre description et/ou que vous avez sélectionné un modèle, le nom du modèle passe du blanc au bleu s’il est sélectionné.

## <a name="event-page-actions"></a>Actions de la page d’événements

Sur la page Web de l’événement, vous disposez des actions et options suivantes :

1. Sélectionnez **modifier** pour apporter des modifications aux paramètres de l’événement.
2. Sélectionnez **End Event** pour mettre fin à l’événement (si votre événement se trouve plus tôt par exemple).
3. Sélectionnez **définir sur brouillon** pour définir votre événement sur brouillon au lieu de actif.
4. Si vous avez effectué une mise à jour de votre environnement importé, vous devrez sélectionner **RÉimporter le monde** pour que ces modifications apparaissent dans votre événement, n’oubliez pas de réinitialiser l’espace dans l’événement :)
5. Sélectionnez **événement dupliqué** pour dupliquer l’événement pour les événements futurs. Ce doublon apparaît alors dans mes événements/Mes brouillons, vous devez mettre à jour le nouveau jour/l’heure et l’activer à partir de là.
6. Sélectionnez **Ajouter en tant qu’événement principal** pour définir votre événement dans la liste calendrier.
7. Sélectionnez **Supprimer l’événement** si vous souhaitez supprimer complètement l’événement (vous ne pouvez pas le récupérer).

Lorsque vous êtes prêt, accédez au menu **événements > mes événements** dans l’interface dans le monde de AltspaceVR et entrez l’espace de l’événement pour réinitialiser l’espace, inspectez vos modifications ou continuez la personnalisation. 

> [!IMPORTANT]
> Il s’agit d’une copie et les personnalisations apportées à l’espace de l’événement sont uniquement destinées à cet événement. Si vous passez beaucoup de temps à personnaliser l’espace de votre événement, il peut être préférable de créer un monde pour votre **événement d’utilisation répétée**.

Pour plus d’informations sur la personnalisation de votre espace d’événements ou sur la création d’un espace d’événements d’origine pour l’importation :

* [Comment faire accorder des rôles à d’autres personnes dans mes mondes ?](../world-building/granting-roles.md)
* [Comment faire laisser les gens voler (ou avoir d’autres possibilités) dans mon monde ?](../world-building/adding-user-abilities.md)
* [Où puis-je obtenir de l’aide sur la création de monde ?](../world-building/getting-help.md)
* [Comment faire gérer mes mondes ?](../world-building/managing-worlds.md)
* [FAQ sur la création de monde](../world-building/world-building-faq.md)
* [Comment faire ajouter des points de génération personnalisés à mes mondes ?](../world-building/adding-custom-spawn-points.md)
* [Comment faire télécharger mes propres kits ?](../world-building/uploading-custom-kits.md)
* [Comment faire la prise en main de la création de Shared Computer Toolkit universels (rechargeur unity)](../world-building/world-building-toolkit-getting-started.md)

## <a name="using-the-multimedia-console-for-a-slide-presentation"></a>Utilisation de la console multimédia pour une présentation de diapositives

La console multimédia est un excellent moyen d’organiser votre contenu pour une présentation, notamment des images, de l’audio ou de la vidéo. Suivez les [instructions de la console multimédia](multimedia-console.md) pour obtenir ce programme d’installation pour votre événement.

## <a name="branding-your-event-with-images"></a>Personnalisation de votre événement à l’aide d’images

Vous pouvez facilement ajouter des images à votre espace d’événements ou à votre logo et votre marque de société, ou même des photographies de vous-même, de votre équipe ou de tout autre contenu visuel dans AltspaceVR.

Les exigences en matière d’images sont les suivantes :
* Les fichiers JPG ou PNG sont acceptés
* Taille d’image maximale : 1920 x 1080
* Résolution : 72 ppp
* Taille de fichier : inférieure à 250 Ko par fichier

le processus implique le téléchargement de votre image vers votre [Photos AltspaceVR](https://account.altvr.com/photos), puis l’utilisation de l’Photos dans l’éditeur universel dans le monde entier pour l’importer et la placer dans l’espace universel des événements.

1. accédez à [Photos](https://account.altvr.com/photos) sur le site web AltspaceVR.
2. Sélectionnez **Charger**.
3. Sélectionnez **Parcourir** pour ouvrir une boîte de dialogue sur votre ordinateur, puis recherchez et sélectionnez l’image optimisée.
4. Sélectionnez **Ouvrir**.
5. Sélectionnez **créer une photo**.
6. Répétez cette opération pour toutes vos images.

Dans AltspaceVR et dans le monde de l’événement, placez-vous à proximité de l’emplacement où vous souhaitez placer l’image. (Si vous créez cela pour un **événement d’utilisation répétée**, assurez-vous que vous êtes dans votre monde et pas dans l’espace de l’événement !)

1. Dans l’interface utilisateur, dans l’angle inférieur droit, sélectionnez **éditeur universel/panneau** de l’éditeur
2. Cliquez sur l’onglet **mine** en bas.
3. Sélectionnez **photos**.
4. Photos sont stockées dans l’ordre chronologique de chargement, la dernière image téléchargée doit être la première image de la liste. Sélectionnez-le pour l’ajouter dans le monde.
5. À l’aide du curseur de votre appareil, récupérez l’image et placez-la là où vous le souhaitez.
    * Vous pouvez le redimensionner à l’aide de vos contrôleurs (en faisant glisser le curseur horizontalement sur le pavé tactile en VR ou en utilisant votre souris en mode 2D).
    * Pour ajuster la position et la rotation de l’image, sélectionnez le symbole de l' **engrenage** sur l’image dans l’éditeur et définissez la rotation et la position de manière appropriée.
    * Vous pouvez également redimensionner l’image avec la fonctionnalité de mise à l’échelle.

> [!NOTE]
> Lorsque le mode édition est activé (texte orange), vous pouvez passer automatiquement à la volée, ce qui permet un déplacement plus facile pour placer les images plus haut dans le monde de l’événement.

6. Répétez cette opération pour chaque placement d’image.
7. Lorsque les images sont définies sur place, sélectionnez **Verrouiller tout** si vous ne les avez pas verrouillées individuellement, puis désactivez le mode édition et fermez l’éditeur.
8. utilisez uniquement un maximum de cinq Photos par événement.

## <a name="adding-3d-objects-using-world-editor-and-kits"></a>Ajout d’objets 3D à l’aide de l’éditeur et des kits World

AltspaceVR permet d’importer des objets 3D dans des mondes avec l’éditeur du monde. De nombreux kits d’éditeurs de monde sont actuellement disponibles pour l’utilisation, et bien plus encore. Il existe des Spaceships, des fusées, des animaux animés, des sculptures, des arbres, des usines et de nombreux objets différents. Vous pouvez également ajouter vos propres kits à la collection publique ou pour votre usage personnel, ou envisager d’utiliser l’une des [applications ALTSPACEVR MRE](../world-building/using-mixed-reality-extensions.md), qui apportent des objets interactifs dans votre monde, tels que des casques, des épées, des ailes, des vêtements, des chapeaux ou d’autres objets interactifs. Attendez que la liste des objets se développe bientôt.

Les instructions ici se concentrent sur l’utilisation des éléments déjà présents dans les kits. Pour plus d’informations sur l’ajout et l’importation d’objets 3D dans AltspaceVR, consultez [« Comment importer des modèles glTF dans mes mondes »](../world-building/importing-models.md) . et [« Comment faire télécharger mes propres kits ? »](../world-building/uploading-custom-kits.md).

Pour ajouter un objet 3D existant à partir des kits de construction dans le monde de l’événement, avec le panneau éditeur/éditeur du monde ouvert et le mode édition activé :

1. Explorez les kits pour l’objet que vous souhaitez importer et sélectionnez-le.
2. Sélectionnez l’objet de kit à l’aide de votre curseur et positionnez-le. Utilisez l’icône d’engrenage sur l’objet dans l’éditeur de monde pour utiliser les options de position, de rotation et de mise à l’échelle pour une entrée de nombre manuelle.
3. Lorsque l’objet est placé à la position de droite, verrouillez-le en cliquant sur l’icône de verrou.
4. Ajoutez un autre objet si vous le souhaitez. Soyez judicieux d’ajouter des objets 3D, en conservant vos sélections à des éléments de cinq kits distincts différents, pour une meilleure prise en charge de l’utilisateur Oculus Quest. N’utilisez pas plus de 200 objets dans un monde.
5. Lorsque vous avez terminé, verrouillez tous les éléments, désactivez le mode édition et fermez l’éditeur de monde. Vous déplacer. Invitez quelques testeurs à visiter et à découvrir et à vous préparer à votre remarquable événement !

Pour plus d’informations sur les kits de l’éditeur World et l’ajout d’objets 3D à AltspaceVR :

* [Qu’est-ce que le programme d’accès anticipé ?](../world-building/early-access.md)
* [Comment importer des modèles glTF dans mes mondes ?](../world-building/importing-models.md)
* [Comment faire utiliser un MRE dans mon monde ?](../world-building/using-mixed-reality-extensions.md)

## <a name="how-to-record-or-live-stream-my-event"></a>Comment enregistrer ou Flux temps réel mon événement

Consultez le document de support suivant pour obtenir des instructions sur l’enregistrement ou la diffusion en continu de votre événement :

* [Comment enregistrer ou Flux temps réel mon événement](recording-and-live-streaming.md)