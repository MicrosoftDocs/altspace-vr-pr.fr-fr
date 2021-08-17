---
title: Importation des modèles glTF
description: Découvrez comment importer correctement des modèles glTF 3D dans vos expériences AltspaceVR et résoudre les problèmes.
ms.date: 03/11/2021
ms.topic: article
keywords: modèles, glTF, importation, sketchfab, résolution des problèmes
ms.openlocfilehash: 527c38fc49028258fa432445fe14a355710a18be65ee74252a8c39bc1bfe5190
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/11/2021
ms.locfileid: "119127058"
---
# <a name="importing-gltf-models"></a>Importation des modèles glTF

> [!NOTE]
> Cette fonctionnalité est disponible pour les utilisateurs sélectionnés dans le programme d’accès anticipé à l’heure actuelle.

L’une des façons de placer des modèles et des scènes 3D dans Altspace consiste à utiliser la [norme glTF](https://en.wikipedia.org/wiki/GlTF). Vous pouvez télécharger un fichier. GLB (compressé glTF) pour créer un modèle que vous pouvez générer ultérieurement dans l’éditeur de monde. Il s’agit d’une alternative au [téléchargement de vos propres kits](uploading-custom-kits.md). Nous vous recommandons de créer des modèles pour les démonstrations rapides, car vous n’aurez pas besoin d’utiliser Unity et de kits lorsque vous souhaitez optimiser les performances et la réutilisation. 

1. Recherchez des ressources 3D glTF. Un emplacement à rechercher est Sketchfab (essayez de filtrer les modèles **téléchargeables** comme [celui-ci](https://sketchfab.com/search?features=downloadable&q=low+poly+wolf&sort_by=-pertinence&type=models)). Une fois que vous l’avez trouvé, sélectionnez **Télécharger le modèle 3D**:

![modèle de chien 3D à partir de Sketchfab](images/importing-models-img-01.png)

2. Copiez le lien vers le modèle et lisez les conditions de licence. 
3. Télécharger la version de **format autoconversion (glTF)**

![Options de téléchargement Sketchfab avec le format de conversion automatique mis en surbrillance](images/importing-models-img-02.png)

4. Ouvrez le site [GLB Packer](https://glb-packer.glitch.me) et cochez la case **convertir png en JPEG (bêta)**
5. Décompressez les fichiers glTF que vous avez téléchargés et faites-les glisser tous en même temps dans l’onglet du navigateur GLB Packer

![Fenêtre présentant la décompression du modèle](images/importing-models-img-03.png)

6. Selon le nombre et la taille des fichiers, le traitement peut prendre un certain temps. Lorsque le traitement est terminé, un fichier **out. GLB** est téléchargé. Renommez ce fichier avec un nom informatif. il s’agit du nom de l’objet dans le monde (par exemple, **Low Wolf. GLB**)
7. Accédez à [altvr.com > plus > modèles](https://account.altvr.com/users/sign_in) , puis sélectionnez **créer**
8. Spécifiez l’emplacement du fichier. GLB et veillez à copier le lien Sketchfab dans la description de l’attribution. Vous pouvez spécifier une image d’aperçu si vous le souhaitez, puis sélectionner **créer un modèle**:

![Aperçu du modèle dans AltspaceVR](images/importing-models-img-04.png)

9. Sélectionner **copier dans le presse-papiers**
10. Ouvrez l' **éditeur World > Altspace > basics > GLTF**
11. Collez votre URL et sélectionnez **confirmer**

Félicitations ! Vous venez de générer votre premier modèle.

## <a name="troubleshooting"></a>Dépannage

**Lorsque j’ai cliqué sur **confirmer** , rien ne s’est produit**
    * Nous avons actuellement une limite de 100 000 polygone. En cas d’échec, supprimez l’objet pour éviter des problèmes potentiels avec les utilisateurs qui rejoignent votre monde
    * Il peut y avoir d’autres problèmes avec la ressource. Essayez d’utiliser des ressources avec le moins de polygones possible.
    * Le modèle que vous apportez peut être petit ou grand. Essayez d’augmenter/de réduire la mise à l’échelle ou de déplacer votre avatar, vous êtes peut-être à l’intérieur du modèle !

**Le chargement est lent** La vitesse à laquelle les autres utilisateurs du monde se chargent en fonction de leurs vitesses de connexion. Il n’est pas non plus mis en cache comme des ressources de kit. Si vous en Placez un dans votre foyer, vous retéléchargerez le même modèle chaque fois que vous vous joignez, ce qui n’est pas très utile.

**Il n’y a aucune collision** Par défaut, il n’y a aucune collision sur les objets qui sont importés de cette façon

**Lorsque je le génère, je perd mes contrôles sur six DDL ou je suis à l’intérieur, il est difficile de le manipuler** . Oui, nous sommes conscients de ces problèmes et espérons les résoudre bientôt.  