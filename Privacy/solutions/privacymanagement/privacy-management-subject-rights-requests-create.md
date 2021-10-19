---
title: Créer une demande de droits d’objet dans la gestion de la confidentialité
f1.keywords:
- CSH
ms.author: v-jgriffee
author: jmgriffee
manager: laurawi
audience: Admin
ms.topic: article
ms.service: O365-seccomp
ms.localizationpriority: medium
ms.collection:
- M365-security-compliance
- M365-privacy-management
search.appverid:
- MOE150
- MET150
description: Découvrez comment créer une demande de droits d’objet dans la gestion de la confidentialité.
ms.openlocfilehash: 316d515be454b6aceed95f68c6f3da6fa0e7567c
ms.sourcegitcommit: 85e085eb17af8b4efd1f45207445e1b3c3679600
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/19/2021
ms.locfileid: "60478246"
---
# <a name="create-a-subject-rights-request"></a>Créer une demande de droits d’objet

Les administrateurs de la gestion des droits de l’objet peuvent ouvrir de nouvelles demandes de droits d’objet via la page principale des demandes de droits d’objet de la gestion de la confidentialité. Un Assistant vous guide tout au long du processus de recherche de données personnelles sur une objet de données et de démarrage du processus de traitement de leur demande.

Vous pouvez également choisir de télécharger des documents supplémentaires pour permettre à la gestion de la confidentialité d’identifier les personnes liées aux données en fonction des valeurs de données exactes fournies. Pour plus d’informations, voir [Gérer la correspondance des données.](privacy-management-subject-rights-requests-data-matching.md)

## <a name="use-the-subject-rights-request-creation-wizard"></a>Utiliser l’Assistant Création de demande de droits d’objet

1. Dans la [Centre de conformité Microsoft 365,](https://compliance.microsoft.com/)allez à la section Gestion de la confidentialité et sélectionnez **Demandes de droits de l’objet.**
1. Pour démarrer une nouvelle demande, **sélectionnez Créer une demande.**
1. Identifiez la personne qui a effectué la demande et spécifiez sa relation avec votre entreprise.
1. Nous allons exécuter une recherche par défaut pour les éléments liés à la sujet de données. Si vous souhaitez affiner votre recherche ou obtenir une estimation avant de récupérer des données, vous pouvez effectuer ces sélections à ce stade. Vous pouvez également laisser tous les éléments vides et passer à l’étape suivante. Pour plus d’informations sur vos options, voir [Définir les paramètres de recherche](#define-search-settings) et affiner votre [recherche.](#refine-your-search)
1. Choisissez un type de demande en fonction de ce que la personne à qui vous souhaitez faire des données. Si leur demande concerne un règlement spécifique sur la confidentialité des données, vous pouvez également la sélectionner dans une liste fournie pour ajouter davantage de contexte. La définition d’une échéance (obligatoire) permet de trier facilement les demandes en retard ou d’approche et de les résoudre en temps voulu. Les types de requête sont les suivants :
   - **Access**: fournit un résumé des informations personnelles de la sujet de données détenues par votre organisation dans Microsoft 365.
   - **Export**: fournit un résumé et une exportation des informations personnelles de la sujet de données, telles que collectées et annotées lors de la révision.
   - **Liste marquée pour le** suivi : génère un résumé de tous les fichiers que les utilisateurs balisent lors de la révision et qui peuvent nécessiter une action supplémentaire en dehors de la gestion de la confidentialité. Par exemple, vous devrez peut-être faciliter la suppression des informations personnelles de la personne à l’aide de sa demande. Les balises de révision de données personnalisées pour les demandes de droits d’objet peuvent être gérées dans les **Paramètres.**
1. Confirmez le nom de cette demande et ajoutez une description facultative pour référence.
1. Examinez le résumé de ce que vous avez entré au cours des étapes précédentes. N’importe quel champ peut être modifié avant de sélectionner **Créer une demande.**

### <a name="define-search-settings"></a>Définir les paramètres de recherche

Lors de la création d’une demande de droits d’objet, vous pouvez choisir une ou toutes ces options de recherche pour rechercher des données sur l’objet :

- **Inclure le contenu rédigé par la** sujet des données : cela inclut le contenu rédigé par la sujet de données et peut renvoyer un volume de données plus élevé.
- **Affiner votre recherche**: cela vous permettra de spécifier des propriétés supplémentaires qui vous aideront à identifier la sujet des données. Ici, vous pouvez étendue votre recherche à Microsoft 365 services ou ressources spécifiques, ou sélectionner d’autres conditions pour ajuster l’étendue de la demande. Après avoir choisi cette option, vous êtes invité à entrer vos paramètres de recherche personnalisés.
- **Obtenez d’abord une** estimation : cela vous permet de voir la quantité de données que nous prévoyons de trouver avant que vos données ne sont récupérées automatiquement.

### <a name="refine-your-search"></a>Affiner votre recherche

Si vous avez choisi d’affiner votre recherche lors de la définition de vos paramètres de recherche, vous serez invité à remplir vos paramètres de recherche avancés. Vous pouvez ajouter **des identificateurs, définir** **des conditions** et choisir **des** emplacements spécifiques Microsoft 365 à rechercher.

- **Ajouter des identificateurs**: fournir plus d’informations d’identification sur la sujet des données, telles que les noms, les adresses e-mail et/ou d’autres options. Séparez plusieurs valeurs dans chaque champ par un point-virgule.
- **Conditions**: commencez à ajouter des conditions pour votre recherche en choisissant un type dans la zone de la zone de la demande. Ces types correspondent aux propriétés possibles des données, telles que la période, la taille, les étiquettes de rétention, les expéditeurs et les destinataires, et bien d’autres encore. Sélectionnez n’importe quel type pour l’ajouter, puis définissez les propriétés souhaitées. Pour les entrées de champ de texte, vous pouvez ajouter plusieurs mots clés séparés par des points-virgules. Vous pouvez ajouter autant de types de contenu que vous le souhaitez.
- **Emplacements**: vous pouvez cibler des sites SharePoint, des canaux Teams et des emplacements OneDrive Entreprise spécifiques. Pour chaque emplacement, vous pouvez sélectionner toutes les instances, telles que toutes les boîtes aux lettres Exchange, ou des instances spécifiques, telles que la boîte aux lettres d’un utilisateur. Sélectionnez **le lien Choisir...** pour chaque option d’emplacement afin d’entrer des informations sur des instances spécifiques. Pour obtenir de l’aide sur l’identification des termes de recherche appropriés, consultez les conditions suivantes :
  - Gérer les sites dans le nouveau centre [d SharePoint d’administration](/sharepoint/manage-sites-in-new-admin-center): fournit des conseils pour trier et filtrer des sites et pour rechercher un site SharePoint site. Utilisez cette opération pour rechercher les URL du champ SharePoint recherche.
  - [Get-Team](/powershell/module/teams/get-team): fournit des informations sur la façon de trouver des équipes dans Microsoft Teams par des propriétés/informations spécifiques. Utilisez-le pour vous aider à identifier Teams conversations et canaux.
  - [À propos OneDrive URL :](/onedrive/list-onedrive-urls#about-onedrive-urls)fournit des informations sur le format et les propriétés appropriés pour l’URL OneDrive’utilisateur. Utilisez cette opération pour vous aider à identifier OneDrive sites dans votre recherche.

Nous vous recommandons d’examiner attentivement vos sélections pour vous assurer que vous identifiez la bonne objet de données. Par exemple, si vous recherchez des boîtes aux lettres par leur nom et que vous recherchez plusieurs personnes avec des noms similaires, vérifiez celle qui est correcte avant de les ajouter à votre demande.

## <a name="next-steps"></a>Étapes suivantes

Une fois que vous avez créé votre demande, elle est répertoriée sur votre page de demande de droits d’objet. Pour en savoir plus sur la façon de passer à la révision, consultez les données de révision [et collaborez sur les demandes.](privacy-management-subject-rights-requests-review.md)

## <a name="legal-disclaimer"></a>Clause d’exclusion de responsabilité légale

[Clause d’exclusion de responsabilité légale de gestion de la confidentialité](privacy-management-disclaimer.md)
