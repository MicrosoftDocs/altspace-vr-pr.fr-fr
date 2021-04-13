---
title: Utilisation d’une extension de réalité mixte
description: Découvrez comment utiliser et résoudre les problèmes liés aux extensions de réalité mixte pour étendre et adapter vos mondes AltspaceVR.
ms.date: 03/11/2021
ms.topic: article
keywords: réalité mixte, extensions, résolution des problèmes
ms.openlocfilehash: 498e71c48f7c67abc40ce4f4667c9eeac4c4e73b
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/08/2021
ms.locfileid: "107212121"
---
# <a name="using-a-mixed-reality-extension"></a>Utilisation d’une extension de réalité mixte

Les [extensions de réalité mixte](https://developer.altvr.com/) (MREs) sont des applications que vous pouvez utiliser dans vos mondes, des [casques](https://account.altvr.com/mres/1173667287173955931) à un [Stargate](https://account.altvr.com/mres/1152987031857529562)opérationnel. C’est ainsi que les membres de la communauté avec l’expérience de programmation peuvent étendre Altspace et les générateurs de monde unidirectionnels peuvent rendre leurs mondes plus interactifs. Même si MREs peut être utilisé par n’importe qui dans un monde, seules les personnes du monde bâtiment peuvent parcourir et générer des MREs dans leurs mondes. 

1. Parcourez la section MRE de notre [site Web](https://account.altvr.com/mres). Par défaut, vous verrez votre propre MREs. par conséquent, sélectionnez **Altspace** pour voir les MREs **officiels et les** afficher à partir de la communauté. Familiarisez-vous avec les MRE avant de l’utiliser dans votre monde. 
2. Accédez à la mre [casques](https://account.altvr.com/mres/1173667287173955931) , puis sélectionnez **copier dans le presse-papiers**. 
3. Accédez à votre monde et ouvrez l’éditeur du monde pour accéder aux **bases > application SDK**. Collez l’URL des casques dans le champ URI cible et sélectionnez **confirmer**. L’objet MRE doit apparaître et tenter de se connecter au MRE qui s’exécute dans le Cloud. Vous devez maintenant voir certains casques sur lesquels vous pouvez cliquer.
4. Déplacez/faites pivoter/mettez à l’échelle le MRE comme vous le feriez pour tout autre objet monde.

Félicitations ! Vous utilisez MREs Now, vous êtes tellement cool !

## <a name="troubleshooting"></a>Résolution des problèmes

**MRE présente un Emoji mécontent** 
    * Vérifier que l’URL est correcte
    * **Option Activer** /désactiver de l’objet et choisir **confirmer**
    * Essayer à nouveau

**MRE est en retard** En fonction de l’emplacement d’hébergement d’un MRE, vous pouvez rencontrer une latence du réseau.

**Pourquoi devons-nous coller des URL ?**
À l’avenir, vous pouvez gérer et générer des MREs comme des artefacts à partir de kits. Jusqu’à présent, nous continuerons à utiliser des URL