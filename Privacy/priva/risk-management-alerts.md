---
title: Examiner et corriger les alertes dans gestion des risques liés à la confidentialité
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
- M365-priva-privacy-risk-management
search.appverid:
- MOE150
- MET150
description: Découvrez comment gérer les alertes et les problèmes déclenchés par les correspondances de stratégie dans Microsoft Priva Privacy Risk Management.
ms.openlocfilehash: a770a7b8d77e2d7792fc4ea8c68914dc62b48a27
ms.sourcegitcommit: 0e68501654f702d8b8b694ae696bb8bd7fa7cea6
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/07/2022
ms.locfileid: "65268327"
---
# <a name="investigate-and-remediate-alerts-in-privacy-risk-management"></a>Examiner et corriger les alertes dans gestion des risques liés à la confidentialité

Microsoft Priva peut vous aider à fournir une visibilité sur les découvertes importantes de vos stratégies de surexposition, de réduction des données ou de transfert de données. Dans la solution Gestion des risques liés à la confidentialité, les administrateurs peuvent passer en revue **les alertes** concernant le contenu qui correspond à vos conditions de stratégie. L’examen des alertes vous permet d’identifier les cas qui nécessitent un suivi. Pour ce faire, vous pouvez créer **des problèmes**. Les problèmes offrent à vos utilisateurs un moyen structuré de passer en revue le contenu, d’attribuer la gravité du problème et de travailler en collaboration pour résoudre les problèmes.

Si votre stratégie a été configurée pour envoyer des notifications à vos utilisateurs, les propriétaires de contenu peuvent également prendre certaines mesures correctives directement à partir de ces e-mails ou de Teams. Pour en savoir plus, consultez [Envoyer des notifications utilisateur dans Gestion des risques liés à la confidentialité](risk-management-notifications.md).

## <a name="view-current-alerts-and-issues"></a>Afficher les alertes et les problèmes actuels

La page **Vue d’ensemble** de Priva fournit une vue d’ensemble des résultats récents avec des mises à jour sur les principaux domaines d’intérêt, tels que les stratégies avec le plus de correspondances et vos alertes de stratégie actuellement actives. Pour en savoir plus sur les informations fournies par cette vue, consultez [Rechercher et visualiser des données personnelles dans Priva](priva-data-profile.md).

Vous pouvez également accéder aux visualisations et aux détails sur vos alertes et problèmes via la page **Stratégies** principale. Sélectionnez **Afficher les alertes** et **afficher les problèmes** pour afficher les détails.

## <a name="manage-alerts"></a>Gérer des alertes

Pour évaluer vos alertes actives et spécifier celles qui nécessitent un suivi, accédez à votre page **Alertes** . Il fournit une liste filtrable des alertes générées par vos stratégies. Vous pouvez les examiner individuellement pour déterminer les circonstances dans lesquelles elles ont été déclenchées.

La sélection d’une alerte ouvre un volet de basculement avec des détails supplémentaires, tels que le nombre d’éléments correspondants et la gravité, selon les paramètres de votre stratégie. Sous l’onglet **Contenu** , vous pouvez examiner les fichiers impliqués dans cette alerte. Ces informations peuvent fournir des informations supplémentaires sur l’événement spécifique qui a déclenché l’alerte, l’endroit où résident les fichiers et les types de données personnelles impliqués. Les déclencheurs d’alertes sont déterminés par les conditions spécifiques de chaque stratégie. Par exemple, une alerte peut être déclenchée sur une stratégie de transfert de données si Priva détecte un transfert entre les départements ou régions spécifiés de la stratégie.

Après avoir évalué n’importe quelle alerte dans la liste, vous pouvez sélectionner **Créer un problème** pour demander à vos utilisateurs d’approfondir l’examen et l’action. Vous serez invité à nommer le problème et à ajouter des commentaires pertinents pour le contexte. Vous pouvez également ignorer les alertes ici si elles ne nécessitent pas de suivi.

## <a name="manage-issues"></a>Gérer les problèmes

Les problèmes sont créés par les administrateurs lors de l’évaluation des alertes sur les correspondances de stratégie. Pour suivre et résoudre les problèmes indiqués, les utilisateurs peuvent visiter la page **Problèmes** . À partir de là, vous pouvez examiner des problèmes individuels, examiner les conditions d’incitation, examiner les données et prendre les mesures nécessaires pour fermer l’affaire.

Cette page fournit la liste de tous les problèmes ouverts. Ils sont répertoriés par nom et triés par gravité pour vous aider à hiérarchiser les cas, y compris les catégories élevée, moyenne et basse, ainsi que les cas non attribués. Sélectionnez un problème dans la liste pour passer en revue son contenu et prendre des mesures pour le résoudre. Vous pouvez attribuer une évaluation de gravité aux problèmes non attribués lors de l’examen.

### <a name="review-issue-details"></a>Examiner les détails du problème

Les pages de détails du problème vous guident tout au long du processus de résolution des risques de confidentialité identifiés et de gestion des fichiers indiqués.

Les onglets des pages de détails du problème fournissent des informations sur les alertes et le contenu associés, notamment :

- **Vue d’ensemble** : affiche des informations essentielles sur le problème. Consultez l’état actuel du problème et les prochaines actions recommandées à entreprendre. Vous pouvez également voir une vue d’ensemble du contenu, de la stratégie associée, des détails sur l’alerte et la chronologie. La chronologie indique où vous êtes dans la récupération de contenu. Le contenu téléchargé sera conservé temporairement pour révision.
- **Alertes** : liste détaillée des alertes associées au problème.
- **Contenu** : liste filtrable des éléments de contenu associés. Sélectionnez un élément pour afficher des détails à son sujet, y compris les activités qui se sont produites et son historique de correction, si quelqu’un a déjà pris des mesures dans Priva pour gérer les données. Vous pouvez également choisir d’effectuer de nouvelles actions de correction.
- **Remarques** : sélectionnez cette option pour ajouter ou afficher des notes pour votre équipe sur le problème.
- **Collaborateurs** : affichez et gérez la liste des collaborateurs qui peuvent contribuer à résoudre ce problème.

### <a name="share-the-issue"></a>Partager le problème

L’ajout de personnes en tant que collaborateurs vous permet de partager le problème avec d’autres membres de votre entreprise via un canal Microsoft Teams sécurisé, un e-mail d’entreprise ou en partageant un lien directement vers la page du problème dans Priva. Ces options sont disponibles sous le bouton **Partager** . Lors du partage via Teams, vous êtes invité à sélectionner parmi les équipes disponibles dans votre organisation, à sélectionner le canal spécifique et à laisser un message sur le problème, qui sera partagé avec le canal spécifié.

## <a name="review-content-and-remediate-issues"></a>Examiner le contenu et corriger les problèmes

Pour passer en revue le contenu associé à un problème, choisissez l’action **Vérifier le contenu** si vous y êtes invité ou ouvrez l’onglet **Contenu** . Sélectionnez n’importe quel fichier de la liste pour l’afficher dans son intégralité. Vous pouvez voir ici des détails sur le fichier, toutes les activités enregistrées et son historique de correction, si des étapes précédentes ont été prises pour gérer ce fichier. Sélectionnez **Corriger** pour effectuer une ou plusieurs des actions répertoriées ci-dessous.

- **Notifier le propriétaire** : informez le propriétaire du contenu du problème détecté.

- **Appliquer une étiquette de rétention** : ajoutez une étiquette pour cet élément qui peut la conserver, la supprimer ou la conserver, puis la supprimer après une heure spécifiée. [En savoir plus sur les étiquettes de rétention](/microsoft-365/compliance/retention).

- **Appliquer une étiquette de confidentialité** : ajoutez une étiquette pour cet élément qui identifie sa sensibilité et, éventuellement, ajoutez une protection qui inclut les marquages visuels et le chiffrement. [En savoir plus sur les étiquettes de confidentialité](/microsoft-365/compliance/sensitivity-labels).

- **Marquer comme non une correspondance** : identifiez un résultat de recherche comme faux positif pour supprimer l’élément de contenu de la considération.

- **Supprimer** (pour les stratégies de réduction des données uniquement) : utilisez cette option pour une suppression réversible des données. L’élément est déplacé dans le dossier ou la corbeille d’éléments supprimés (Exchange, SharePoint, OneDrive) ou supprimé avec une option de récupération (Teams messages). La suppression peut être inversée dans un laps de temps défini, en fonction des paramètres du service.

- **Rendre privé** (pour la surexposition des données et les stratégies de transfert de données uniquement) : supprimez l’accès ouvert pour cet élément de contenu.

Chaque option vous invite à laisser des commentaires et toute autre information de support nécessaire pour le propriétaire du contenu avant de confirmer votre choix.

Une fois que toutes les étapes de correction ont été effectuées (y compris toutes les actions que vous jugez recommandées en plus des options disponibles dans Priva) et que le problème est prêt à se fermer, utilisez le bouton **Résoudre** et ajoutez vos commentaires finaux avant de l’envoyer.

## <a name="legal-disclaimer"></a>Exclusion de responsabilité légale

[Exclusion de responsabilité légale de Microsoft Priva](priva-disclaimer.md)
