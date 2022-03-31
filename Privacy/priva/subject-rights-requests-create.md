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
ms.openlocfilehash: 9de1047950a556b4456fd4453ea8d860a0a01c38
ms.sourcegitcommit: 16dd1c0320bf1c58ad75edbbe2113fc79013f504
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/25/2022
ms.locfileid: "64404608"
---
# <a name="create-a-subject-rights-request"></a>Créer une demande de droits d’objet

Les administrateurs de la gestion des droits de l’objet peuvent ouvrir de nouvelles demandes via la page principale Des demandes de droits d’objet de Priva. Un Assistant vous guide tout au long du processus de recherche de données personnelles sur une objet de données et de démarrage du processus de traitement de leur demande.

Vous pouvez également choisir de télécharger du contenu supplémentaire pour permettre à Priva d’identifier les personnes liées aux données en fonction des valeurs de données exactes fournies. Pour plus d’informations, voir [Correspondance des données pour les demandes de droits de l’objet](subject-rights-requests-data-match.md).

## <a name="request-types"></a>Types de demandes

Les demandes de droits de l’objet Priva prend en charge trois types de demandes différents :

1. **Accès** : fournit un résumé des informations personnelles de la sujet de données détenues par votre organisation dans Microsoft 365.

2. **Exportation** : fournit un résumé et un fichier exporté d’éléments de contenu qui contiennent les informations personnelles de la sujet de données. Voici les éléments examinés et marqués **comme inclus** lors de l’examen des données collectées par vos paramètres de recherche.

3. **Liste balisé pour** le suivi : génère un résumé de tous les fichiers qui ont été marqués au cours de la révision des données et qui peuvent nécessiter une action supplémentaire en dehors de Priva. Par exemple, vous devrez peut-être faciliter la suppression des informations personnelles de la sujet de données en fonction de leur demande. Vous pouvez afficher les balises incluses et configurer des balises personnalisées pour votre organisation dans les [paramètres Priva](priva-settings.md).

## <a name="use-the-subject-rights-request-creation-wizard"></a>Utiliser l’Assistant Création de demande de droits d’objet

1. Dans la [Centre de conformité Microsoft 365](https://compliance.microsoft.com/), sélectionnez **Demandes des droits de l’objet Priva** à partir du navigation de gauche.

2. Dans le coin supérieur droit, **sélectionnez Créer une demande**.

3. Dans **la page** Informations sur la sujet des données, ajoutez le prénom et le nom de famille, l’adresse e-mail, le pays de résidence et spécifiez leur relation avec votre société. Ensuite, sélectionnez **Suivant**.

4. Dans la page **Emplacements**, choisissez les emplacements Microsoft 365 où vous souhaitez rechercher les données personnelles de la sujet de données. Obtenir des détails sur les [paramètres d’emplacement](#choose-locations). Lorsque vous avez terminé de choisir des emplacements, sélectionnez **Suivant.**

5. Dans la page **Paramètres de recherche** , vous pouvez modifier les paramètres de recherche pour affiner votre recherche et choisir d’obtenir une estimation avant de récupérer des données. Vous n’avez pas à choisir d’options sur cette page, ce qui entraîne une recherche par défaut basée sur les emplacements que vous avez spécifiés à l’étape précédente. Pour plus d’informations sur vos options, voir [Définir les paramètres de recherche](#define-search-settings). Quand vous êtes prêt à continuer, sélectionnez **Suivant**.

6. Dans la page **Type** de demande, choisissez un [type](#request-types) de demande en fonction de ce que la personne objet de données souhaite que vous faites avec leurs données : **Accès**, **Exportation** ou Liste balisé pour le **suivi**. Si leur demande concerne un règlement spécifique sur la confidentialité des données, vous pouvez également la sélectionner dans une liste fournie pour ajouter davantage de contexte. La définition d’une échéance (obligatoire) permet de trier facilement les demandes en retard ou d’approche et de les résoudre en temps voulu. Lorsque vous avez terminé, sélectionnez **Suivant**.

7. Sur le **nom de la** demande, confirmez ou modifiez le nom de cette demande et ajoutez une description facultative pour référence. Ensuite, sélectionnez **Suivant**.

8. Dans la page **Révision et fin** , examinez vos sélections. N’importe quelle section peut être modifiée. Lorsque vous avez terminé, sélectionnez **Créer une demande**.

Votre demande aura sa propre page de détails et sera répertoriée sur votre page principale de demande de droits d’objet. Après avoir créé votre demande, Priva commence à chercher des correspondances avec les informations de la sujet de données que vous avez fournies aux emplacements que vous avez spécifiés. L’application d’une estimation des données sur la page de détails de la demande peut prendre plusieurs minutes en fonction de l’étendue de votre recherche.

## <a name="choose-locations"></a>Choisir des emplacements

Pour chaque demande de droits d’objet, vous pouvez définir votre recherche de façon à rechercher des données à tous les emplacements ou à des emplacements spécifiques dans Exchange et SharePoint. Choisissez un emplacement en déplaçant son bouton bascule vers la position **Sur** . Vous pouvez choisir de rechercher tous les comptes et tous les sites ou de désigner des comptes ou des sites spécifiques à l’intérieur de chaque emplacement. Lisez les détails ci-dessous sur ce qui est abordé dans chaque emplacement.

- **Exchange** : cette option recherche des données dans Exchange boîtes aux lettres et dans des conversations individuelles ou Teams groupe. Vous pouvez choisir de rechercher tous les comptes Exchange de votre organisation ou sélectionner Choisir des comptes pour sélectionner des **utilisateurs individuels** dans le  volet volant Exchange boîtes aux lettres.

- **SharePoint** : cette option recherche les données dans les sites SharePoint, les sites OneDrive Entreprise sites et les canaux Teams réseau. Vous pouvez choisir de rechercher tous les sites SharePoint de votre organisation, ou sélectionner Choisir des **sites** pour sélectionner des utilisateurs individuels dans le volet volant SharePoint **sites** web.

Pour obtenir de l’aide sur l’identification des termes de recherche appropriés, consultez les rubriques suivantes :

- **SharePoint sites** et URL : la gestion des sites dans le Centre d’administration [SharePoint](/sharepoint/manage-sites-in-new-admin-center) donne des conseils sur la façon de trier et de filtrer des sites, et sur la recherche d’un site SharePoint site. Utilisez cette fonction pour rechercher les URL à entrer dans le champ de recherche du **volet** de SharePoint sites.

- **Teams conversations et** canaux : [Get-Team](/powershell/module/teams/get-team) montre comment trouver des équipes dans Microsoft Teams en fournissant des propriétés ou des informations spécifiques.

- **OneDrive sites** et URL : à propos OneDrive URL fournit des informations sur le format et les [propriétés appropriés](/onedrive/list-onedrive-urls#about-onedrive-urls) pour l’URL OneDrive’un utilisateur. Utilisez cette opération pour vous aider à identifier OneDrive sites dans votre recherche.

Nous vous recommandons d’examiner attentivement vos sélections pour vous assurer que vous identifiez la bonne objet de données. Par exemple, si vous recherchez des boîtes aux lettres par nom et que vous recherchez plusieurs personnes avec des noms similaires, vérifiez celle qui est correcte avant de les ajouter à votre demande.

## <a name="define-search-settings"></a>Définir les paramètres de recherche

Lorsque vous créez une demande de droits d’objet, une recherche par défaut s’exécute en fonction de vos sélections dans **la page** Emplacements de l’Assistant de création. Si vous souhaitez effectuer une recherche plus ciblée, ou si vous souhaitez obtenir une estimation de vos données avant la récupération des éléments de contenu, vous pouvez effectuer ces sélections sur la page **Paramètres** de recherche de l’Assistant Création de demande.

### <a name="advanced-search-options"></a>Options de recherche avancées

- **Affiner votre recherche** : cette option vous permet de spécifier des propriétés supplémentaires pour vous aider à identifier la sujet de données parmi les données de votre organisation. Après avoir choisi cette option, vous serez invité à ajouter d’autres paramètres de recherche, expliqués ci-dessous dans [Affiner votre recherche](#refine-your-search).
- **Inclure le contenu rédigé par la** sujet de données : cette option recherche le contenu qui a été rédigé par la sujet de données. Par exemple, les fichiers créés par la SharePoint données ou téléchargés vers celui-ci. La sélection de cette option peut augmenter considérablement la quantité de données renvoyées.
- **Incluez toutes les versions** des éléments : si vous avez sélectionné SharePoint comme emplacement de recherche, la requête de recherche par défaut ne retourne que la version actuelle SharePoint éléments. La case à cochant cette case retourne les versions actuelles et précédentes des éléments SharePoint, ce qui vous donne une quantité de données beaucoup plus importante à réviser.

### <a name="data-estimate"></a>Estimation des données

**L’option** Obtenir une estimation en premier présente une estimation de la quantité de données que nous prévoyons de trouver avant la récupération automatique de vos données. Lorsque votre estimation est affichée sur la page de détails de la demande, vous pouvez choisir d’afficher les résultats de la recherche et d’afficher un aperçu d’un échantillonnage des éléments qui ont été découverts. Si les éléments représentent les résultats attendus, vous devez sélectionner Récupérer les  données pour poursuivre la récupération réelle des éléments de contenu.

## <a name="refine-your-search"></a>Affiner votre recherche

Si vous choisissez  Affiner votre recherche sur la page **Paramètres** de recherche, lorsque vous  sélectionnez Suivant, vous êtes invité à fournir des détails sur les attributs et conditions personnels afin de cibler davantage vos résultats de recherche. Vous pouvez ajouter des ajouts dans l’une ou l’autre des catégories ou les deux. Lorsque vous avez terminé d’effectuer des sélections dans cette section, la récupération des données pour la demande sera basée sur vos paramètres de recherche.

#### <a name="add-personal-attributes"></a>Ajouter des attributs personnels

Entrez des valeurs dans les champs de texte pour les noms, surnoms, adresses e-mail et adresse de la sujet de données. Vous pouvez ajouter d’autres identificateurs tels que la date de naissance ou le numéro de téléphone, et les champs de texte peuvent prendre en charge plusieurs entrées séparées par un point-virgule. Lorsque vous avez terminé, sélectionnez **Suivant** pour continuer à la page **Conditions** .

#### <a name="conditions"></a>Conditions

Sélectionnez le bouton Ajouter une **condition** pour choisir parmi une plage de conditions afin de cibler davantage votre recherche, y compris le nom de l’élément, les noms des expéditeurs et des destinataires, le type de données personnelles et si l’élément a été partagé en externe à l’extérieur de votre organisation. Les champs de texte peuvent être séparés par des points-virgules. Lorsque vous avez terminé, sélectionnez **Suivant** pour enregistrer vos paramètres de recherche et l’avancement vers le paramètre de type de requête.

## <a name="next-steps"></a>Étapes suivantes

Une fois que vous avez créé votre demande, elle est répertoriée sur votre page de demande de droits d’objet. Pour en savoir plus sur la façon de passer à la révision, consultez [les données de révision et collaborez sur les demandes](subject-rights-requests-data-review.md).

## <a name="legal-disclaimer"></a>Clause d’exclusion de responsabilité légale

[Clause d’exclusion de responsabilité légale Microsoft Priva](priva-disclaimer.md)
