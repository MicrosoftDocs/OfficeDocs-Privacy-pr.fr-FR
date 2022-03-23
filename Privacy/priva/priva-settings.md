---
title: Configurer les paramètres Priva
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
- MET150
description: Découvrez les options de paramètres globaux pour Microsoft Priva.
ms.openlocfilehash: 49a6f2112e584ef72bcc0f0433b09a21ccac194c
ms.sourcegitcommit: a9ad5185174a9e8a7eea7583d257e8535c96a2ed
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/23/2022
ms.locfileid: "63746781"
---
# <a name="configure-priva-settings"></a>Configurer les paramètres Priva

Vous pouvez gérer les paramètres de Microsoft Priva en sélectionnant l’icône d’engrenage dans le coin supérieur droit de l’écran. Les options ci-après vous permettent de définir des préférences de haut niveau et de personnaliser les propriétés clés. Cette page fournit une vue d’ensemble des principales Paramètres catégories.

## <a name="anonymization"></a>Anonymisation

Vous pouvez afficher des versions rendues anonymes des noms d’utilisateur dans les fonctionnalités de gestion des risques de confidentialité pour les utilisateurs de certains rôles. La fonctionnalité d’anonymisation remplace les noms complets identifiables par une étiquette générique afin de masquer les identités de vos utilisateurs lors de l’examen des données sensibles. Cette option ne s’applique pas à la solution Demandes de droits d’objet.

## <a name="user-notification-emails"></a>Messages électroniques de notification de l’utilisateur  

Les stratégies de gestion des risques de confidentialité vous permettent de définir des paramètres pour évaluer les risques potentiels en matière de confidentialité dans votre environnement. Lorsqu’une correspondance de stratégie est détectée, la Gestion des risques de confidentialité peut envoyer un courrier électronique à vos utilisateurs avec des recommandations sur les actions correctives à prendre et un lien vers une formation sur la confidentialité. Dans **Paramètres**, vous pouvez activer ou désactiver la fonctionnalité de notification par courrier électronique de la gestion des risques de confidentialité dans son ensemble. Si la fonctionnalité de notification est désactivée Paramètres, tous les e-mails sont désactivés. Pour en savoir plus sur les stratégies, voir [Créer des stratégies dans Gestion des risques de confidentialité](risk-management-policies.md).

## <a name="teams-collaboration"></a>Collaboration des équipes  

Intégrez Microsoft Teams fonctionnalités d’accès aux demandes des droits des personnes concernées pour améliorer la collaboration avec les parties prenantes. Chaque fois qu’une demande de droits d’objet est créée, une équipe associée est créée dans Teams. Les utilisateurs peuvent être ajoutés à une équipe à partir de l’onglet Collaborateurs de la demande. Pour en savoir plus sur les demandes de droits d’objet, voir [En savoir plus sur les demandes de droits de l’objet Priva](subject-rights-requests.md).

## <a name="data-matching"></a>Correspondance de données  

Utilisez cette section pour télécharger des schémas de données qui décrivent les attributs de vos sujets de données, ce qui permet d’identifier la sujet de données correcte lors de la recherche de données personnelles dans votre environnement Microsoft 365 données. Les schémas et les packages de règles sont créés et chargés au format XML. Sous **téléchargement de données personnelles**, vous pouvez également envoyer des données personnelles qui correspond à un schéma fourni. Vous pouvez créer et télécharger votre propre fichier ou choisir de télécharger des données personnelles à partir d’Azure. Pour en savoir plus sur les demandes de droits d’objet, voir [En savoir plus sur les demandes de droits de l’objet Priva](subject-rights-requests.md).

## <a name="data-retention-periods"></a>Périodes de rétention des données

Ce paramètre est lié aux demandes de droits de l’objet Priva. Il vous permet de contrôler votre préférence pour la durée de rétention des données collectées et des rapports générés après la fermeture de la demande. Ce nombre peut être fixé à 30 ou 90 jours et s’applique à toutes les demandes de droits d’objet que vous créez. Nous vous recommandons de vérifier que vos périodes de rétention des données sont conformes aux stratégies et obligations légales de votre organisation. En savoir plus sur [la définition de la rétention des données pour les demandes de droits d’objet](subject-rights-requests-reports.md#manage-data-retention).

## <a name="data-review-tags"></a>Balises de révision des données

Les balises de révision des données peuvent être utilisées pour marquer les éléments de contenu qui sont récupérés dans une demande de droits d’objet. Cette zone de paramètres vous permet de gérer vos balises. Priva fournit trois balises par défaut : **Suivi**, **Suppression** et **Mise à jour**. Ces noms de balises ne peuvent pas être modifiés, mais vous pouvez fournir une description pour ces balises qui est significative pour votre organisation.

Priva fournit également deux balises personnalisées que vous pouvez nommer et définir pour l’utilisation de votre organisation. Ces balises sont répertoriées en tant que balise personnalisée **1** et balise **personnalisée 2** jusqu’à ce que vous modifiiez les noms.

Suivez les étapes ci-dessous pour modifier les noms et les descriptions des balises :

- Dans la page Priva **Paramètres**, sélectionnez **Balises de révision des données**.
- Recherchez la balise dans la liste à modifier et sélectionnez l’icône Modifier le crayon en dessous de son nom.
- Dans le volet volant, modifiez les champs disponibles. Pour les balises système, vous pouvez uniquement modifier la description. Pour les balises personnalisées, vous pouvez modifier le nom et la description.
- Lorsque vous avez terminé, sélectionnez **Envoyer** pour enregistrer vos modifications.

Les paramètres de balise s’appliquent à toutes les demandes de droits d’objet.

En savoir plus sur [l’application de balises lors de l’examen des données d’une demande de droits d’objet](subject-rights-requests-data-review.md#apply-tags).

**Dans Paramètres**, consultez les **balises de révision des données** pour passer en revue et gérer vos balises.
 
Ces balises peuvent être utilisées pour indiquer le contenu qui devra être davantage attentif, tel que le contenu qui devra peut-être être supprimé manuellement. Dans cette section de paramètres, vous pouvez modifier les noms et les descriptions des balises personnalisées. Vous pouvez également modifier les descriptions des balises intégrées fournies par le système. Les noms des balises système ne peuvent pas être modifiés. Pour en savoir plus sur les demandes de droits d’objet, voir [Examiner les données d’une demande de droits d’objet](subject-rights-requests-data-review.md#step-3-review-data).
