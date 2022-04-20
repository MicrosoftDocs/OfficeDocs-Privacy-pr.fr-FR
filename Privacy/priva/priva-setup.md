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
ms.openlocfilehash: e88145dc999e210f36a8dc82e1bc9996bc15bb88
ms.sourcegitcommit: 09ecdaded9a9f8f79587f2acb978dc53b83e5c01
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/19/2022
ms.locfileid: "64930555"
---
# <a name="get-started-with-priva"></a>Démarrer avec Priva

Si vous êtes prêt à commencer à utiliser Microsoft Priva pour obtenir de l’aide pour identifier et atténuer les risques de confidentialité, suivez ces étapes pour configurer les prérequis et commencer à explorer les insights de confidentialité.

## <a name="step-1-confirm-subscriptions-and-licensing"></a>Étape 1 : Confirmer les abonnements et les licences

Priva est disponible dans le [portail de conformité Microsoft Purview](https://compliance.microsoft.com/) et peut être acheté par les organisations disposant des licences suivantes :

- Microsoft 365 E3, E5, A3, A5
- Office 365 E1, E3, E5, A1, A3, A5

Priva propose des options de licence pour deux solutions différentes : Priva Privacy Risk Management et Priva Subject Rights Requests. Ceux-ci peuvent être achetés individuellement ou ensemble. Lorsque vous obtenez des licences pour les demandes de droits d’objet, vous pouvez choisir le niveau de licence approprié pour le nombre de demandes que vous devez gérer. Vous pouvez acheter des demandes supplémentaires à tout moment.

Pour obtenir des instructions détaillées sur les licences, consultez [instructions relatives aux licences Microsoft 365 pour la sécurité et la conformité](/office365/servicedescriptions/microsoft-365-service-descriptions/microsoft-365-tenantlevel-services-licensing-guidance/microsoft-365-security-compliance-licensing-guidance#microsoft-priva).

> [!Note]
> Priva n’est pas disponible pour les clients us government Community (Cloud de la communauté du secteur public) Moderate, Cloud de la communauté du secteur public High ou Department of Defense (DoD).

### <a name="get-free-trial-license"></a>Obtenir une licence d’évaluation gratuite

Une licence d’essai gratuite est disponible pour la prise en main de Priva. Pour en savoir plus sur l’éligibilité et sur la façon de participer, consultez [Découvrir la version d’évaluation gratuite de Priva](priva-trial.md).

## <a name="step-2-enable-the-microsoft-365-audit-log"></a>Étape 2 : Activer le journal d’audit Microsoft 365

Microsoft 365 journaux d’audit sont un récapitulatif de toutes les activités au sein de votre organisation. Les stratégies de gestion des risques de confidentialité peuvent utiliser ces activités pour générer des insights de stratégie.

Il se peut que les journaux d’audit soient déjà activés dans votre organisation. Si vous devez commencer à les utiliser pour la première fois, consultez [Activer ou désactiver la recherche dans le journal d’audit](/microsoft-365/compliance/turn-audit-log-search-on-or-off) pour obtenir des instructions pas à pas pour activer l’audit. Une fois l’audit activé, le message qui apparaît indique que le journal d’audit est en cours de préparation et que vous pourrez effectuer une recherche environ deux heures après la fin de la préparation. Vous n'avez à faire cette action qu'une seule fois. Pour plus d’informations sur l’utilisation du journal d’audit Microsoft 365, consultez [Rechercher dans le journal d’audit](/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).

## <a name="step-3-set-user-permissions-and-assign-roles"></a>Étape 3 : Définir des autorisations utilisateur et attribuer des rôles

Priva utilise un modèle d’autorisation de contrôle d’accès en fonction du rôle (RBAC). Seuls les utilisateurs auxquels un rôle est attribué peuvent accéder à Priva, et les actions autorisées par chaque utilisateur sont limitées par type de rôle.

Votre administrateur général dispose des autorisations nécessaires pour accéder à Priva et affecter d’autres utilisateurs à des rôles. Ils peuvent se connecter et définir des autorisations utilisateur dans le [portail de conformité Microsoft Purview](https://compliance.microsoft.com/) pour Priva. Pour commencer rapidement, le groupe de rôles Gestion de la confidentialité dispose des autorisations nécessaires pour accéder à toutes les fonctionnalités de Priva. Ce groupe peut être adapté aux organisations où la même personne peut effectuer toutes les tâches. D’autres rôles de confidentialité vous permettent de prendre un contrôle plus précis et d’affecter des utilisateurs à des fonctionnalités ou des fonctions sélectionnées.

Pour en savoir plus sur les groupes de rôles et sur la façon d’accorder l’accès, consultez [Définir les autorisations utilisateur et attribuer des rôles dans Priva](priva-permissions.md).

## <a name="step-4-start-finding-and-visualizing-your-data"></a>Étape 4 : Commencer à rechercher et à visualiser vos données

Une fois connecté à Priva, la page **Vue d’ensemble** s’affiche. Cette page fournit des insights dynamiques sur l’évolution des données personnelles dans votre environnement Microsoft 365 pour vous aider à identifier rapidement les problèmes, à identifier les indicateurs de risque et à prendre des mesures pour résoudre les problèmes. Votre vue d’ensemble doit être renseignée avec les informations initiales dans les 24 premières heures suivant l’inscription. Au fur et à mesure que vous continuerez à utiliser Priva, la page de vue d’ensemble s’actualisera pour continuer à fournir des informations actuelles.

Pour plus d’informations sur vos données au fil du temps, votre page **Profil** de données fournit davantage de visualisations et d’analyses et vous donne une vue holistique des données de votre organisation par emplacement géographique et par emplacement Microsoft 365.

Pour en savoir plus sur ces pages, consultez [Rechercher et visualiser des données personnelles dans Priva](priva-data-profile.md).

## <a name="step-5-start-managing-risks-with-default-policies"></a>Étape 5 : Commencer à gérer les risques avec les stratégies par défaut

La gestion des risques liés à la confidentialité commence à évaluer vos données et vous donne un aperçu des principaux scénarios de risque pour la réduction des données, la surexposition des données et les transferts de données. Ces stratégies sont activées par défaut. Vous pouvez utiliser ces stratégies pour évaluer l’emplacement de vos risques, puis activer les notifications par e-mail de l’utilisateur pour que vos utilisateurs soulever des problèmes à leur attention et guider la correction de ces risques. En outre, vous pouvez créer et personnaliser vos propres stratégies à partir des modèles de stratégie fournis. Vous pouvez adapter vos stratégies pour répondre aux besoins de conformité juridique et réglementaire de votre organisation, comme cela peut être identifié en consultation avec des conseillers juridiques. Pour en savoir plus, consultez [Créer des stratégies dans Gestion des risques liés à la confidentialité](risk-management-policies.md).

## <a name="step-6-get-started-with-subject-rights-requests"></a>Étape 6 : Démarrage avec des demandes de droits d’objet

Priva Subject Rights Requests automatise le processus de traitement des demandes de droits d’objet, ce qui permet d’accéder facilement aux données et aux flux de travail personnalisables qui s’intègrent aux processus métier existants. Vous pouvez facilement trouver les données pertinentes, examiner les résultats et produire des rapports. En cours de route, vous pouvez collaborer en toute sécurité avec d’autres experts de votre organisation pour effectuer la demande de droits de sujet. Vous pouvez également gérer et personnaliser vos flux de travail métier avec des modèles intégrés. Pour en savoir plus sur l’utilisation de ces fonctionnalités, consultez [Learn about Priva Subject Rights Requests](subject-rights-requests.md).

## <a name="legal-disclaimer"></a>Exclusion de responsabilité légale

[Exclusion de responsabilité légale de Microsoft Priva](priva-disclaimer.md)
