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
ms.openlocfilehash: a6f2fe55600d6cc3018c9d15f05a6d9e459a1486
ms.sourcegitcommit: 3c83e8133a5a71f4e1d76a0b2981ab3ec9cd6602
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/13/2022
ms.locfileid: "66046598"
---
# <a name="configure-priva-settings"></a>Configurer les paramètres Priva

Vous pouvez gérer les paramètres de Microsoft Priva en sélectionnant l’icône d’engrenage dans le coin supérieur droit de l’écran. Les options disponibles ici vous permettent de définir des préférences générales et de personnaliser les propriétés de clé. Cette page fournit une vue d’ensemble des principales catégories de Paramètres.

## <a name="anonymization"></a>Anonymisation

Vous pouvez afficher des versions anonymes des noms d’utilisateur dans les fonctionnalités de gestion des risques de confidentialité pour les utilisateurs de certains rôles. La fonctionnalité d’anonymisation remplace les noms d’affichage identifiables par une étiquette générique afin de masquer les identités de vos utilisateurs tout en examinant les données sensibles. Cette option ne s’applique pas à la solution Demandes de droits d’objet.

## <a name="user-notification-emails"></a>E-mails de notification utilisateur  

Les stratégies de gestion des risques liés à la confidentialité vous permettent de définir des paramètres pour évaluer les risques potentiels en matière de confidentialité dans votre environnement. Lorsqu’une correspondance de stratégie est détectée, la gestion des risques liés à la confidentialité peut envoyer un e-mail à vos utilisateurs avec des recommandations sur les mesures correctives à prendre et un lien vers la formation à la confidentialité. Dans **Paramètres**, vous pouvez activer ou désactiver la fonctionnalité de notification par e-mail de la gestion des risques de confidentialité dans son ensemble. Si la fonctionnalité de notification est désactivée dans Paramètres, tous les e-mails sont désactivés. Pour en savoir plus sur les stratégies, consultez [Créer des stratégies dans Gestion des risques liés à la confidentialité](risk-management-policies.md).

## <a name="teams-collaboration"></a>Collaboration des équipes  

Intégrez Microsoft Teams fonctionnalités à Demandes de droits des personnes concernées Priva pour améliorer la collaboration avec les parties prenantes. Si vous cochez la case pour **activer Microsoft Teams fonctionnalités pour les demandes de droits d’objet**, vous créez automatiquement un canal Teams associé pour chaque requête. Les utilisateurs peuvent être ajoutés au canal Teams à partir de l’onglet **Collaborateurs** de la demande.

L’activation de cette fonctionnalité appliquera Teams fonctionnalités à toutes les demandes. Si vous décochez la case, ces fonctionnalités seront désactivées pour toutes les demandes. En savoir plus sur [la collaboration pendant le processus d’examen des données](subject-rights-requests-data-review.md#collaboration-for-data-review).

## <a name="data-matching"></a>Correspondance des données  

Utilisez cette section pour charger des schémas de données qui décrivent les attributs de vos sujets de données, ce qui vous aidera à identifier la personne concernée lors de la recherche de données personnelles dans votre environnement Microsoft 365. Les schémas et les packages de règles sont créés et chargés au format XML. Sous **Chargement de données personnelles**, vous pouvez également envoyer des données personnelles qui correspondent à un schéma fourni. Vous pouvez créer et charger votre propre fichier ou choisir de charger des données personnelles à partir d’Azure. En savoir plus sur la [correspondance des données pour les demandes de droits d’objet](subject-rights-requests-data-match.md).

## <a name="data-retention-periods"></a>Périodes de rétention des données

Ce paramètre est lié à Demandes de droits des personnes concernées Priva. Il vous permet de contrôler votre préférence pour la durée pendant laquelle vous souhaitez conserver les données collectées et les rapports générés après la fermeture de la demande. Il peut être défini sur 30 ou 90 jours et s’applique à toutes les demandes de droits d’objet que vous créez. Nous vous recommandons de vérifier que vos périodes de conservation des données sont conformes aux stratégies et obligations légales de votre organisation. En savoir plus sur [la conservation des données pour les demandes de droits d’objet](subject-rights-requests-reports.md#retention-periods-for-reports-and-data).

## <a name="data-review-tags"></a>Balises de révision des données

Les balises de révision des données peuvent être utilisées pour marquer les éléments de contenu récupérés dans une demande de droits d’objet. Cette zone de paramètres vous permet de gérer vos balises. Priva fournit trois balises par défaut : **Suivi**, **Suppression** et **Mise à jour**. Ces noms de balises ne peuvent pas être modifiés, mais vous pouvez fournir une description de ces balises significative pour votre organisation.

Priva fournit également deux balises personnalisées que vous pouvez nommer et définir pour l’utilisation de votre organisation. Vous verrez ces balises répertoriées en tant que **Balise personnalisée 1** et **Balise personnalisée 2** jusqu’à ce que vous modifiiez les noms.

Suivez les étapes ci-dessous pour modifier les noms et descriptions des balises :

- Dans la page Priva **Paramètres**, sélectionnez **Balises de révision des données**.
- Recherchez la balise dans la liste à modifier, puis sélectionnez l’icône **Modifier** le crayon en regard de son nom.
- Dans le volet volant, apportez vos modifications dans les champs disponibles. Pour les balises système, vous pouvez uniquement modifier la description. Pour les balises personnalisées, vous pouvez modifier le nom et la description.
- Lorsque vous avez terminé, **sélectionnez Envoyer** pour enregistrer vos modifications.

Les paramètres de balise s’appliquent à toutes les demandes de droits d’objet.

En savoir plus sur [l’application de balises lors de l’examen des données pour une demande de droits d’objet](subject-rights-requests-data-review.md#apply-tags).