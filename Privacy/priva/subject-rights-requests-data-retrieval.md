---
title: Estimation et récupération des données dans les demandes de droits d’objet
f1.keywords:
- CSH
ms.author: chvukosw
author: chvukosw
manager: laurawi
audience: Admin
ms.topic: article
ms.service: O365-seccomp
ms.localizationpriority: medium
ms.collection:
- M365-security-compliance
- M365-priva-subject-rights-requests
search.appverid:
- MOE150
- MET150
description: Comprendre comment les données sont récupérées et comment modifier les paramètres de recherche dans Demandes de droits des personnes concernées Microsoft Priva.
ms.openlocfilehash: a2586e987f7a03905feedfd587aab43dba3d9e6b
ms.sourcegitcommit: 8cbafebb1a1b26a0bd92e500a1e6d6c60243c64b
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/20/2022
ms.locfileid: "66166663"
---
# <a name="data-estimate-and-retrieval"></a>Estimation et récupération des données

**Dans cet article** : Comprendre l’estimation des données et les étapes de récupération des données d’une demande de droits d’objet. Découvrez comment afficher la requête de recherche d’une requête et apporter des modifications pour affiner la recherche.

## <a name="data-estimate"></a>Estimation des données
Une fois que vous avez créé une demande, Priva commence immédiatement à rechercher des correspondances avec la personne concernée dans le contenu de votre environnement Microsoft 365. Une fois que nous avons identifié tous les éléments que nous pensons correspondre à vos critères, vous verrez l’estimation dans la carte **de résumé de l’estimation des données** dans la page **Vue d’ensemble** de la demande. La quantité de données dans l’étendue de votre recherche affecte la durée nécessaire pour terminer l’estimation.

Votre demande passe automatiquement à l’étape suivante de la **récupération des données**, où tous les éléments de contenu sont regroupés pour permettre aux parties prenantes de collaborer à l’examen des données. Dans certains cas, nous suspendons l’estimation des données avant de passer à la récupération et vous informons des prochaines étapes à suivre avant de continuer.

### <a name="pause-in-data-estimate"></a>Pause dans l’estimation des données

Il existe deux raisons pour lesquelles une demande s’interrompt à l’étape **d’estimation des données** :

1. Lors de la création d’une demande, vous pouvez choisir d’obtenir une estimation en premier. Pour plus d’informations, consultez l’étape 6 de [création d’une demande personnalisée](subject-rights-requests-create.md#custom-setup-guided-process-to-choose-all-settings) .

2. Si l’estimation est projetée pour retourner un grand nombre d’éléments à examiner (plus de 10 000 éléments), le flux de travail s’interrompt. À ce stade, vous pouvez afficher un aperçu des résultats et décider s’il faut [modifier votre requête de recherche](subject-rights-requests-create.md#refining-your-search) ou continuer à récupérer les éléments identifiés.

Lorsque la demande est suspendue à **l’estimation des données**, une carte apparaît sur la page de détails de votre demande avec des informations récapitulatives sur le nombre d’éléments, le volume, leur emplacement et un lien vous permettant d’afficher **les détails de la requête de recherche**.

![Carte d’estimation des données.](../media/priva-srr-data-estimate.png)

## <a name="view-and-edit-search-queries"></a>Afficher et modifier des requêtes de recherche

Pour afficher des informations détaillées sur la recherche de la demande, sélectionnez **Afficher les détails de la requête de recherche** sur la carte **de résumé de l’estimation des données** . Un volet volant s’ouvre, qui résume la requête et affiche des détails supplémentaires sur ce qui a été trouvé. À partir de là, vous disposez des options suivantes :

- Sélectionnez **aperçu des résultats** pour obtenir un aperçu du type de contenu qui sera retourné sous les paramètres de recherche actuels.
- Sélectionnez **Modifier la requête de recherche** pour modifier les paramètres de recherche.

Lorsque vous **sélectionnez Modifier la requête de recherche**, vous êtes dirigé par un processus guidé pour modifier ou ajouter des propriétés pour identifier l’objet des données, modifier les conditions et ajuster les emplacements que vous souhaitez que la recherche couvre. Suivez les instructions [fournies lors de l’affinement de votre recherche](subject-rights-requests-create.md#refining-your-search) pour obtenir des informations plus détaillées. Vous pouvez passer en revue la version finale de votre nouvelle requête de recherche, puis sélectionner **Enregistrer** pour recommencer la recherche.

Une nouvelle estimation est générée et l’état de la demande revient à **l’estimation des données**. La nouvelle recherche peut prendre jusqu’à 60 minutes. Une fois l’opération terminée, les résultats mis à jour s’affichent sur la page de détails de la demande.

Lorsque vous êtes prêt à continuer, **sélectionnez récupérer les données** dans le coin supérieur droit de votre écran pour passer à l’étape de récupération des données.

## <a name="retrieve-data"></a>Récupérer des données

L’étape de récupération des données consiste à récupérer tous les fichiers, e-mails, conversations, images et autres éléments de contenu contenant les données personnelles de la personne concernée. Les éléments sont regroupés dans un conteneur Stockage Blob Azure à réviser. La récupération des données peut prendre quelques minutes ou beaucoup plus longtemps en fonction du volume de données.

Une fois cette étape terminée, la demande passe automatiquement à l’étape suivante de **la révision des données**.

## <a name="next-steps"></a>Prochaines étapes

[Visitez les données de révision pour une demande de droits de sujet](subject-rights-requests-data-review.md) pour en savoir plus sur les tâches clés et la collaboration avec les parties prenantes pour **l’étape De révision des données**.

## <a name="legal-disclaimer"></a>Exclusion de responsabilité légale

[Microsoft Priva exclusion de responsabilité légale](priva-disclaimer.md)