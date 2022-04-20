---
title: Créer une demande de droits d’objet
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
description: Découvrez comment créer une demande de droits d’objet dans Microsoft Priva.
ms.openlocfilehash: b2d846aa4020be315705bbd16e00378c7514146c
ms.sourcegitcommit: 09ecdaded9a9f8f79587f2acb978dc53b83e5c01
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/19/2022
ms.locfileid: "64930605"
---
# <a name="create-a-subject-rights-request"></a>Créer une demande de droits d’objet

Les administrateurs de gestion des droits de l’objet peuvent ouvrir de nouvelles demandes via la page principale demandes de droits d’objet de Priva. Un Assistant vous guide tout au long du processus de recherche de données personnelles sur un sujet de données et de démarrage du processus de traitement de leur demande.

Vous pouvez également choisir de charger du matériel supplémentaire pour permettre à Priva d’identifier les personnes concernées en fonction des valeurs de données exactes fournies. Pour plus d’informations, consultez [La correspondance des données pour les demandes de droits des personnes concernées](subject-rights-requests-data-match.md).

## <a name="request-types"></a>Types de demandes

Priva Subject Rights Requests prend en charge trois types de demandes différents :

1. **Accès** : fournit un résumé des informations personnelles de la personne concernée détenues par votre organisation dans Microsoft 365.

2. **Exportation** : fournit un résumé et un fichier exporté d’éléments de contenu qui contiennent les informations personnelles de la personne concernée. Il s’agit des éléments examinés et marqués comme **inclus** lors de votre examen des données collectées par vos paramètres de recherche.

3. **Liste balisé pour le suivi** : génère un résumé de tous les fichiers qui ont été marqués lors de l’examen des données qui peuvent nécessiter une action supplémentaire en dehors de Priva. Par exemple, vous devrez peut-être faciliter la suppression des informations personnelles de la personne concernée en fonction de sa demande. Vous pouvez afficher les balises incluses et configurer des balises personnalisées pour votre organisation dans [les paramètres Priva](priva-settings.md).

## <a name="use-the-subject-rights-request-creation-wizard"></a>Utiliser l’Assistant de création de demande de droits d’objet

1. Dans le [portail de conformité Microsoft Purview](https://compliance.microsoft.com/), accédez à la section Priva et sélectionnez **Priva Subject Rights Requests**.
1. Pour démarrer une nouvelle demande, sélectionnez **Créer une requête**.
1. Identifiez la personne concernée qui a effectué la demande et spécifiez leur relation avec votre entreprise.
1. Nous allons exécuter une recherche par défaut pour les éléments liés à la personne concernée. Si vous souhaitez affiner votre recherche ou obtenir une estimation avant de récupérer des données, vous pouvez effectuer ces sélections à ce stade. Vous pouvez également laisser tous les éléments vides et passer à l’étape suivante. Pour plus d’informations sur vos options, consultez [Définir les paramètres de recherche](#define-search-settings) et [Affiner votre recherche](#refine-your-search).
1. Choisissez un type de requête en fonction de ce que la personne concernée souhaite que vous fassiez avec ses données. Si leur demande concerne un règlement spécifique sur la confidentialité des données, vous pouvez également la sélectionner dans une liste fournie pour ajouter un contexte supplémentaire. La définition d’une échéance (obligatoire) permet de trier facilement les demandes en attente ou en retard et de les résoudre en temps voulu. Les types de demande sont les suivants :
   - **Accès** : fournit un résumé des informations personnelles de la personne concernée détenues par votre organisation dans Microsoft 365.
   - **Exportation** : fournit un résumé et une exportation des informations personnelles de la personne concernée, telles qu’elles sont collectées et annotées lors de l’examen.
   - **Liste balisé pour le suivi** : génère un résumé des fichiers que les utilisateurs balisent lors de la révision et qui peuvent nécessiter une action supplémentaire en dehors de Priva. Par exemple, vous devrez peut-être faciliter la suppression des informations personnelles de la personne concernée en fonction de sa demande. Les balises de révision de données personnalisées pour les demandes de droits d’objet peuvent être gérées dans **des Paramètres globales.**
1. Confirmez le nom de cette demande et ajoutez une description facultative pour référence.
1. Passez en revue le résumé de ce que vous avez entré au cours des étapes précédentes. N’importe quel champ peut être modifié avant de sélectionner **Créer une requête**.

Pour chaque demande de droits d’objet, vous pouvez définir votre recherche pour rechercher des données dans tous les emplacements ou emplacements spécifiques dans Exchange et Sharepoint. Choisissez un emplacement en déplaçant son commutateur bascule vers la position **Activé** . Vous pouvez choisir de rechercher tous les comptes et sites ou de désigner des comptes ou des sites spécifiques dans chaque emplacement. Lisez les détails ci-dessous sur ce qui est couvert dans chaque emplacement.

- **Exchange** : cette option recherche des données dans Exchange boîtes aux lettres et dans des conversations Teams individuelles ou de groupe. Vous pouvez choisir de rechercher tous les comptes Exchange de votre organisation, ou de sélectionner **des comptes** pour sélectionner des utilisateurs individuels dans le volet volant **Exchange boîtes aux lettres**.

- **SharePoint** : cette option recherche des données dans des sites SharePoint, des sites OneDrive Entreprise et des canaux Teams. Vous pouvez choisir de rechercher tous les sites SharePoint de votre organisation, ou sélectionner **Choisir des sites** pour sélectionner des utilisateurs individuels dans le volet volant **SharePoint sites**.

Pour obtenir de l’aide sur l’identification des termes de recherche appropriés, reportez-vous aux rubriques suivantes :

- **SharePoint sites et URL** : [La gestion des sites dans le centre d’administration SharePoint](/sharepoint/manage-sites-in-new-admin-center) fournit des conseils sur le tri et le filtrage des sites, ainsi que sur la recherche d’un site SharePoint. Utilisez cette option pour rechercher des URL à entrer dans le champ de recherche dans le volet de menu volant **SharePoint sites**.

- **Teams conversations et canaux** : [Get-Team](/powershell/module/teams/get-team) montre comment trouver des équipes dans Microsoft Teams en fournissant des propriétés ou des informations spécifiques.

- **OneDrive sites et URL** : [À propos des URL OneDrive](/onedrive/list-onedrive-urls#about-onedrive-urls) fournit des informations sur le format et les propriétés appropriés pour l’URL OneDrive d’un utilisateur. Utilisez-la pour vous aider à identifier OneDrive sites dans votre recherche.

Nous vous recommandons d’examiner attentivement vos sélections pour vous assurer d’identifier le sujet de données approprié. Par exemple, si vous recherchez des boîtes aux lettres par nom et trouvez plusieurs personnes portant des noms similaires, vérifiez la bonne avant de les ajouter à votre demande.

## <a name="define-search-settings"></a>Définir les paramètres de recherche

Lorsque vous créez une demande de droits d’objet, une recherche par défaut s’exécute en fonction de vos sélections sur la page **Emplacements** de l’Assistant création. Si vous souhaitez effectuer une recherche plus ciblée ou si vous souhaitez choisir d’obtenir une estimation de vos données avant la récupération des éléments de contenu, vous pouvez effectuer ces sélections dans la page **Paramètres de recherche** de l’Assistant Création de demande.

### <a name="advanced-search-options"></a>Options de recherche avancées

- **Affiner votre recherche** : cette option vous permet de spécifier des propriétés supplémentaires pour aider à identifier la personne concernée parmi les données de votre organisation. Après avoir choisi cette option, vous êtes invité à ajouter d’autres paramètres de recherche, comme expliqué ci-dessous dans [Affiner votre recherche](#refine-your-search).
- **Inclure le contenu créé par l’objet de données** : cette option recherche le contenu qui a été créé par la personne concernée. Par exemple, les fichiers créés par la personne concernée ou chargés vers SharePoint par. La sélection de cette option peut augmenter considérablement la quantité de données retournées.
- **Inclure toutes les versions d’éléments** : si vous avez sélectionné SharePoint comme emplacement de recherche, la requête de recherche par défaut renvoie uniquement la version actuelle des éléments SharePoint. Cette case à cocher renvoie les versions actuelles et toutes les versions précédentes des éléments SharePoint, ce qui génère une quantité de données beaucoup plus importante à examiner.

### <a name="data-estimate"></a>Estimation des données

La **première option Obtenir une estimation** présente une estimation de la quantité de données que nous nous attendons à trouver avant que vos données ne sont récupérées automatiquement. Lorsque votre estimation est affichée sur la page de détails de la demande, vous pouvez choisir d’afficher les résultats de la recherche et d’afficher un aperçu d’un échantillon d’éléments qui ont été découverts. Si les éléments représentent les résultats attendus, vous devez sélectionner **Récupérer les données** afin de poursuivre la récupération réelle des éléments de contenu.

## <a name="refine-your-search"></a>Affiner votre recherche

Si vous choisissez **Affiner votre recherche** dans la page **Paramètres** de recherche, lorsque vous sélectionnez **Suivant** , vous êtes invité à fournir des détails sur les attributs personnels et les conditions afin de cibler davantage vos résultats de recherche. Vous pouvez effectuer des ajouts dans l’une ou l’autre des catégories ou dans les deux catégories. Lorsque vous avez terminé d’effectuer des sélections dans cette section, la récupération des données pour la demande est basée sur vos paramètres de recherche.

#### <a name="add-personal-attributes"></a>Ajouter des attributs personnels

Entrez des valeurs dans les champs de texte pour les noms, surnoms, adresses e-mail et adresses de la personne concernée. Vous pouvez ajouter d’autres identificateurs tels que la date de naissance ou le numéro de téléphone, et les champs de texte prennent en charge plusieurs entrées séparées par un point-virgule. Lorsque vous avez terminé, sélectionnez **Suivant** pour passer à la page **Conditions** .

#### <a name="conditions"></a>Conditions

Sélectionnez le bouton **Ajouter une condition** pour choisir parmi une plage de conditions pour cibler davantage votre recherche, notamment le nom de l’élément, les noms d’expéditeur et de destinataire, le type de données personnelles, et si l’élément a été partagé en externe à l’extérieur de votre organisation. Les champs de texte prennent en charge plusieurs entrées séparées par un point-virgule. Lorsque vous avez terminé, sélectionnez **Suivant** pour enregistrer vos paramètres de recherche et la progression vers le paramètre de type de requête.

## <a name="next-steps"></a>Étapes suivantes

Une fois que vous avez créé votre demande, elle apparaît dans la page de votre demande de droits d’objet. Pour en savoir plus sur la procédure de révision, consultez [Vérifier les données et collaborer sur les demandes](subject-rights-requests-data-review.md).

## <a name="legal-disclaimer"></a>Exclusion de responsabilité légale

[Exclusion de responsabilité légale de Microsoft Priva](priva-disclaimer.md)
