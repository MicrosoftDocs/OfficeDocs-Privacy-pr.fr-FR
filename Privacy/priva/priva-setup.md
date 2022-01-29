---
title: Mise en place de Priva
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
description: Découvrez comment configurer Microsoft Priva pour votre organisation, définir des rôles et des autorisations et configurer des paramètres importants.
ms.openlocfilehash: 62e28361b57dd866b95ce566616473ed1a71e4ad
ms.sourcegitcommit: f145dff5e387a8e26db2f3a2c7de125978fbacc9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/28/2022
ms.locfileid: "62248967"
---
# <a name="get-started-with-priva"></a>Mise en place de Priva

Si vous êtes prêt à commencer à utiliser Microsoft Priva pour vous aider à identifier et réduire les risques de confidentialité, suivez ces étapes pour configurer les conditions préalables et commencer à explorer les informations sur la confidentialité.

## <a name="step-1-confirm-subscriptions-and-licensing"></a>Étape 1 : Confirmer les abonnements et les licences

Priva est disponible dans le [Centre de conformité Microsoft 365](https://compliance.microsoft.com/) et peut être acheté par des organisations titulaires des licences suivantes :

- Microsoft 365 E3, E5, A3, A5
- Office 365 E1, E3, E5, A1, A3, A5

Priva propose des options de licence pour deux solutions différentes : Priva Privacy Risk Management et Priva Subject Rights Requests. Ceux-ci peuvent être achetés individuellement ou ensemble. Lorsque vous obtenez des licences pour les demandes de droits d’objet, vous pouvez choisir le niveau de licence approprié pour le nombre de demandes que vous devez gérer. Vous pouvez acheter des demandes supplémentaires à tout moment.

Pour obtenir des instructions détaillées sur les licences, consultez [instructions relatives aux licences Microsoft 365 pour la sécurité et la conformité](/office365/servicedescriptions/microsoft-365-service-descriptions/microsoft-365-tenantlevel-services-licensing-guidance/microsoft-365-security-compliance-licensing-guidance#privacy-management).

> [!Note]
> Priva n’est pas disponible pour les clients modérés, Cloud de la communauté du secteur public élevés ou du département de la Défense (DoD) du gouvernement américain Community (Cloud de la communauté du secteur public).

### <a name="get-free-trial-license"></a>Obtenir une licence d’essai gratuite

Une licence d’essai gratuite est disponible pour la mise en place de Priva. Pour en savoir plus sur l’éligibilité et sur la façon de participer, consultez la version d’essai [gratuit de Priva](priva-trial.md).

## <a name="step-2-enable-the-microsoft-365-audit-log"></a>Étape 2 : Activer le journal d Microsoft 365 d’audit

Microsoft 365 journaux d’audit sont un résumé de toutes les activités au sein de votre organisation. Les stratégies de gestion des risques de confidentialité peuvent utiliser ces activités pour générer des informations sur les stratégies.

Les journaux d’audit de votre organisation sont peut-être déjà allumés. Si vous devez commencer à les utiliser pour la première fois, voir Activer ou désactiver la recherche dans le journal [d’audit](/microsoft-365/compliance/turn-audit-log-search-on-or-off) pour obtenir des instructions pas à pas pour activer l’audit. Une fois l’audit activé, le message qui apparaît indique que le journal d’audit est en cours de préparation et que vous pourrez effectuer une recherche environ deux heures après la fin de la préparation. Vous n'avez à faire cette action qu'une seule fois. Pour plus d’informations sur l’utilisation Microsoft 365 journal d’audit, voir [Rechercher dans le journal d’audit](/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).

## <a name="step-3-set-user-permissions-and-assign-roles"></a>Étape 3 : Définir des autorisations utilisateur et attribuer des rôles

Priva utilise un modèle d’autorisation de contrôle d’accès basé sur un rôle (RBAC). Seuls les utilisateurs affectés à un rôle peuvent accéder à Priva, et les actions autorisées par chaque utilisateur sont limitées par type de rôle.

Votre administrateur global dispose des autorisations pour accéder à Priva et affecter d’autres utilisateurs à des rôles. Ils peuvent se connecter et définir des autorisations utilisateur dans le [Centre de conformité Microsoft 365](https://compliance.microsoft.com/) pour Priva. Pour un démarrage rapide, le groupe de rôles Gestion de la confidentialité dispose des autorisations pour accéder à toutes les fonctionnalités de Priva. Ce groupe peut être adapté aux organisations où la même personne peut effectuer toutes les tâches. D’autres rôles de confidentialité vous permettent de prendre un contrôle plus granulaire et d’affecter des utilisateurs à des fonctions ou fonctionnalités sélectionnées.

Pour en savoir plus sur les groupes de rôles et sur la façon d’accorder l’accès, voir [Définir des autorisations utilisateur et attribuer des rôles dans Priva](priva-permissions.md).

## <a name="step-4-start-finding-and-visualizing-your-data"></a>Étape 4 : Commencer à trouver et à visualiser vos données

Une fois que vous vous êtes connectez à Priva, la page **Vue d’ensemble s’affiche** . Cette page fournit des informations dynamiques sur l’évolution des données personnelles dans votre environnement Microsoft 365 pour vous aider à identifier rapidement les problèmes, à identifier les indicateurs de risque et à prendre des mesures pour résoudre les problèmes. Votre vue d’ensemble doit être remplie avec les informations initiales dans les 24 premières heures de l’inscription. À mesure que vous continuez d’utiliser Priva, la page de vue d’ensemble s’actualise pour continuer à fournir les informations actuelles.

Pour obtenir des informations supplémentaires sur vos données au fil du temps, **votre page de** profil de données fournit davantage de visualisations et d’analyses et vous offre une vue globale des données de votre organisation par emplacement géographique et par emplacement Microsoft 365 données.

Pour en savoir plus sur ces pages, voir [Rechercher et visualiser des données personnelles dans Priva](priva-data-profile.md).

## <a name="step-5-start-managing-risks-with-default-policies"></a>Étape 5 : Commencer à gérer les risques avec les stratégies par défaut

La gestion des risques de confidentialité commence à évaluer vos données et vous donne un coup d’œil aux principaux scénarios de risque pour la réduction des données, la surexposation des données et les transferts de données. Ces stratégies sont désactivées par défaut. Vous pouvez utiliser ces stratégies pour évaluer vos risques, puis activer les notifications par courrier électronique de vos utilisateurs afin de les attirer vers leur attention et d’orienter la correction de ces risques. En outre, vous pouvez créer et personnaliser vos propres stratégies à partir des modèles de stratégie fournis. Vous pouvez adapter vos stratégies pour répondre aux besoins de conformité juridique et réglementaire de votre organisation, comme cela peut être identifié en consultation avec un conseiller juridique. Pour plus d’informations, voir [Créer des stratégies dans Gestion des risques de confidentialité](risk-management-policies.md).

## <a name="step-6-get-started-with-subject-rights-requests"></a>Étape 6 : Prendre en premier les demandes de droits d’objet

Les demandes de droits de l’objet priva automatisent le processus d’traitement des demandes de droits de l’objet, ce qui permet d’accéder facilement aux données et aux flux de travail personnalisables qui s’intègrent aux processus métiers existants. Vous pouvez facilement trouver les données pertinentes, examiner les résultats et produire des rapports. En cours de route, vous pouvez collaborer en toute sécurité avec d’autres experts de votre organisation pour finalisation de la demande de droits d’objet. Vous pouvez également gérer et personnaliser vos flux de travail d’entreprise avec des modèles intégrés. Pour en savoir plus sur l’utilisation de ces fonctionnalités, voir [En savoir plus sur les demandes de droits de l’objet Priva](subject-rights-requests.md).

## <a name="legal-disclaimer"></a>Clause d’exclusion de responsabilité légale

[Clause d’exclusion de responsabilité légale Microsoft Priva](priva-disclaimer.md)
