---
title: Ajout de points de génération personnalisés
description: Découvrez comment créer, ajouter et dépanner vos points de génération personnalisés vers AltspaceVR.
ms.date: 03/11/2021
ms.topic: article
keywords: spawnpoint, résolution des problèmes
ms.openlocfilehash: 0f53bdc229eb21e50edef34981c592556236fc55
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/08/2021
ms.locfileid: "107212221"
---
# <a name="adding-custom-spawn-points"></a>Ajout de points de génération personnalisés

Les personnes qui entrent dans votre monde peuvent **générer** ou apparaître à l’origine, position (0, 0, 0), quand elles entrent dans votre monde. Toutefois, vous pouvez ajouter un ou plusieurs points de génération si vous le souhaitez, par exemple, que les gens commencent à l’entrée à votre Castle. Si vous spécifiez plusieurs points de génération, un est choisi de façon aléatoire chaque fois qu’un utilisateur entre et l’origine n’est pas incluse. Vous pouvez gérer des points de génération pour n’importe quel environnement ou événement où votre éditeur de monde est activé. Vous contrôlez où les gens génèrent (position) et la direction dans laquelle ils sont dirigés (rotation). Les points de génération ne sont visibles qu’en mode édition. 

1. Accédez à proximité de l’endroit où vous souhaitez que les gens se génèrent. Ouvrez l' **éditeur World > notions de base** et assurez-vous que la **rotation de verrouillage** est activée. Sélectionnez le **point de génération** pour en créer un. Déplacez-le vers la position exacte souhaitée :

![Fenêtre de base de l’éditeur universel ouverte](images/spawn-points-img-01.png)

2. Sélectionnez l’icône paramètres pour le point de génération et assurez-vous que la **rotation > X** et la **rotation > Z** sont tous deux **0**. S’il s’agit de petits nombres comme **8.537777745 e-07**, c’est également parfait. C’est une particularité du traitement des nombres à virgule flottante :

![Mettre à jour les points de génération dans le monde des paramètres de l’éditeur](images/spawn-points-img-02.png)

3. Entrez à nouveau votre univers via les **paramètres de > de Menu > général > entrer à nouveau l’espace >**
4. Vous devez générer votre nouveau point de génération !
5. Si vous souhaitez que les gens fassent face à une direction différente, sélectionnez les paramètres du point de génération et définissez la **Rotation > Y** uniquement. Essayez d’affecter la valeur 180 à X et Z à 0 (AVERTISSEMENT : X et Z sont avancés peuvent rendre les personnes malades). Sélectionnez ensuite **confirmer** et entrez de nouveau le monde. Cela devrait vous faire face à la direction opposée. 

## <a name="troubleshooting"></a>Résolution des problèmes

**Les gens génèrent toujours à l’origine ?**
    * Assurez-vous que vos points de génération sont légèrement au-dessus du sol ou de la surface. Si le point de génération chevauche d’autres objets, les personnes génèrent à l’emplacement par défaut, l’origine. Cela peut se produire si le point de génération à l’intérieur d’un objet et la hauteur de la personne varient. 
    * Essayez de réinitialiser votre environnement via le **Menu > paramètres > l’espace de réinitialisation modérée >**

**Vous avez plusieurs points de Spawn, tout en continuant de générer le même emplacement ?**
Vous êtes peut-être Unlucky--il est aléatoire après tout. Essayez une entrée de nouveau au moins cinq fois avant de supposer qu’il y a une erreur. 

Les **personnes ne sont pas à l’aise ou leur tête est inclinée** Vous avez peut-être oublié de cocher la case **verrouiller la rotation** ou de définir la valeur X et Z pour la rotation. Ceux-ci doivent généralement avoir la valeur 0, sauf si vous créez un monde exotique. 

**Les gens sont-ils en baisse ?**
Ne définissez pas la position du point de génération trop élevée au-dessus d’un objet. S’ils sont trop éloignés, ils seront regénérés à l’origine.