---
title: Démarrer avec Priva
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
- M365-priva-privacy-risk-management
search.appverid:
- MOE150
- MET150fcf
description: Découvrez comment configurer Microsoft Priva pour votre organisation, définir des rôles et des autorisations, et configurer des paramètres importants.
ms.openlocfilehash: 945cbfd2625be50cb89eeaa8fe09e0effaea79d5
ms.sourcegitcommit: 3c27ecf7c86c8a3db38cae8819fc090eed192b4f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/25/2022
ms.locfileid: "65678211"
---
# <a name="get-started-with-priva"></a>Démarrer avec Priva

Si vous êtes prêt à commencer à utiliser Microsoft Priva pour aider votre organisation à identifier et à atténuer les risques de confidentialité, suivez ces étapes pour vous aider à vous configurer.

## <a name="confirm-subscriptions-and-licensing"></a>Confirmer les abonnements et les licences

Priva est disponible dans le [portail de conformité Microsoft Purview](https://compliance.microsoft.com/) et peut être acheté par les organisations disposant des licences suivantes :

- Microsoft 365 E3, E5, A3, A5
- Office 365 E1, E3, E5, A1, A3, A5

Priva offre des options de licence pour deux solutions différentes : Gestion des risques de confidentialité Priva et Demandes de droits des personnes concernées Priva. Ceux-ci peuvent être achetés individuellement ou ensemble. Lorsque vous obtenez des licences pour les demandes de droits d’objet, vous pouvez choisir le niveau de licence approprié pour le nombre de demandes que vous devez gérer. Vous pouvez acheter des demandes supplémentaires à tout moment.

Pour obtenir des instructions détaillées sur les licences, consultez [instructions relatives aux licences Microsoft 365 pour la sécurité et la conformité](/office365/servicedescriptions/microsoft-365-service-descriptions/microsoft-365-tenantlevel-services-licensing-guidance/microsoft-365-security-compliance-licensing-guidance#microsoft-priva).

> [!Note]
> Priva n’est pas disponible pour les clients Community du gouvernement des États-Unis (Cloud de la communauté du secteur public) Modéré, Cloud de la communauté du secteur public High ou Department of Defense (DoD).

### <a name="start-a-free-trial"></a>Démarrez une version d’essai gratuite

Utilisez un abonnement d’essai gratuit pour explorer toutes les fonctionnalités des deux solutions Priva. Découvrez comment vous inscrire à [l’essai Priva](priva-trial.md).

## <a name="enable-the-microsoft-365-audit-log"></a>Activer le journal d’audit Microsoft 365

Microsoft 365 journaux d’audit sont un récapitulatif de toutes les activités au sein de votre organisation. Les stratégies de gestion des risques de confidentialité peuvent utiliser ces activités pour générer des insights de stratégie.

Il se peut que les journaux d’audit soient déjà activés dans votre organisation. Si vous devez commencer à les utiliser pour la première fois, consultez [Activer ou désactiver la recherche dans le journal d’audit](/microsoft-365/compliance/turn-audit-log-search-on-or-off) pour obtenir des instructions pas à pas pour activer l’audit. Une fois l’audit activé, le message qui apparaît indique que le journal d’audit est en cours de préparation et que vous pourrez effectuer une recherche environ deux heures après la fin de la préparation. Vous n'avez à faire cette action qu'une seule fois. Pour plus d’informations sur l’utilisation du journal d’audit Microsoft 365, consultez [Rechercher dans le journal d’audit](/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).

## <a name="set-user-permissions-and-assign-roles"></a>Définir les autorisations utilisateur et attribuer des rôles

Priva utilise un modèle d’autorisation de contrôle d’accès en fonction du rôle (RBAC). Seuls les utilisateurs auxquels un rôle est attribué peuvent accéder à Priva, et les actions autorisées par chaque utilisateur sont limitées par type de rôle.

Votre administrateur général dispose des autorisations nécessaires pour accéder à Priva et affecter d’autres utilisateurs à des rôles. Ils peuvent se connecter et définir des autorisations utilisateur dans le [portail de conformité Microsoft Purview](https://compliance.microsoft.com/) pour Priva. Pour commencer rapidement, le groupe de rôles Gestion de la confidentialité dispose des autorisations nécessaires pour accéder à toutes les fonctionnalités de Priva. Ce groupe peut être adapté aux organisations où la même personne peut effectuer toutes les tâches. D’autres rôles de confidentialité vous permettent de prendre un contrôle plus précis et d’affecter des utilisateurs à des fonctionnalités ou des fonctions sélectionnées.

Pour en savoir plus sur les groupes de rôles et sur la façon d’accorder l’accès, consultez [Définir les autorisations utilisateur et attribuer des rôles dans Priva](priva-permissions.md).

## <a name="start-finding-and-visualizing-your-data"></a>Commencer à rechercher et à visualiser vos données

Une fois connecté à Priva, la page **Vue d’ensemble** s’affiche. Cette page fournit des insights dynamiques sur l’évolution des données personnelles dans votre environnement Microsoft 365 pour vous aider à identifier rapidement les problèmes, à identifier les indicateurs de risque et à prendre des mesures pour résoudre les problèmes. Votre vue d’ensemble doit être renseignée avec les informations initiales dans les 24 premières heures suivant l’inscription. À mesure que vous continuerez à utiliser Priva, la page de vue d’ensemble s’actualisera pour continuer à fournir des informations actuelles.

Pour plus d’informations sur vos données au fil du temps, votre page **Profil** de données fournit davantage de visualisations et d’analyses et vous donne une vue holistique des données de votre organisation par emplacement géographique et par emplacement Microsoft 365.

Pour en savoir plus sur ces pages, consultez [Rechercher et visualiser des données personnelles dans Priva](priva-data-profile.md).

## <a name="start-managing-risks-with-default-policies"></a>Commencer à gérer les risques avec les stratégies par défaut

La gestion des risques liés à la confidentialité commence à évaluer vos données et vous donne un aperçu des principaux scénarios de risque pour la réduction des données, la surexposition des données et les transferts de données. Ces stratégies sont activées par défaut. Vous pouvez utiliser ces stratégies pour évaluer l’emplacement de vos risques, puis activer les notifications par e-mail de l’utilisateur pour que vos utilisateurs soulever des problèmes à leur attention et guider la correction de ces risques. En outre, vous pouvez créer et personnaliser vos propres stratégies à partir des modèles de stratégie fournis. Vous pouvez adapter vos stratégies pour répondre aux besoins de conformité juridique et réglementaire de votre organisation, comme cela peut être identifié en consultation avec des conseillers juridiques. Pour en savoir plus, consultez [Créer des stratégies dans Gestion des risques liés à la confidentialité](risk-management-policies.md).

## <a name="get-started-with-subject-rights-requests"></a>Démarrage avec des demandes de droits d’objet

Demandes de droits des personnes concernées Priva automatise le processus de traitement des demandes de droits d’objet, ce qui permet d’accéder facilement aux données et aux flux de travail personnalisables qui s’intègrent aux processus métier existants. Vous pouvez facilement trouver les données pertinentes, examiner les résultats et produire des rapports. En cours de route, vous pouvez collaborer en toute sécurité avec d’autres experts de votre organisation pour effectuer la demande de droits de sujet. Vous pouvez également gérer et personnaliser vos flux de travail métier avec des modèles intégrés. Pour en savoir plus sur l’utilisation de ces fonctionnalités, consultez [En savoir plus sur Demandes de droits des personnes concernées Priva](subject-rights-requests.md).

## <a name="priva-availability"></a>disponibilité Priva

Microsoft Priva est disponible pour les clients du monde entier. Si votre organisation a approvisionné son locataire dans l’un des centres de données locaux répertoriés ci-dessous afin de répondre aux exigences de résidence des données, les solutions de Priva ne seront pas disponibles dans le volet de navigation gauche du portail de conformité Microsoft Purview :

- Norvège
- Pologne
- Qatar
- Singapour
- Afrique du Sud
- Corée du Sud
- Espagne
- Suède
- Suisse
- Émirats arabes unis

## <a name="legal-disclaimer"></a>Exclusion de responsabilité légale

[Microsoft Priva exclusion de responsabilité légale](priva-disclaimer.md)
