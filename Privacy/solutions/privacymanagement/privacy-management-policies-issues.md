---
title: Comprendre les alertes et les problèmes de gestion de la confidentialité
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
description: Découvrez comment gérer les alertes et les problèmes élevés par les correspondances de stratégie dans la gestion de la confidentialité.
ms.openlocfilehash: a5dcdc78484f664249578475326ad9d39c1cd381
ms.sourcegitcommit: 85e085eb17af8b4efd1f45207445e1b3c3679600
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/19/2021
ms.locfileid: "60478254"
---
# <a name="understand-policy-alerts-and-issues-in-privacy-management"></a>Comprendre les alertes et les problèmes de stratégie dans la gestion de la confidentialité

La gestion de la confidentialité peut contribuer à offrir une visibilité sur les découvertes importantes de vos stratégies de surexposation, de réduction des données ou de transfert de données. Dans la solution de gestion de la confidentialité, les administrateurs peuvent examiner les **alertes** concernant le contenu qui correspond à vos conditions de stratégie. La révision des alertes vous permet d’identifier les cas qui doivent être suivis. Vous pouvez le faire en créant **des problèmes.** Les problèmes donnent à vos utilisateurs un moyen structuré de réviser le contenu, d’affecter la gravité du problème et de collaborer pour résoudre les problèmes.

Si votre stratégie a été définie pour envoyer des notifications à vos utilisateurs, les propriétaires de contenu peuvent également prendre certaines mesures correctives directement à partir de ces e-mails ou de Teams. Pour plus d’informations, voir [Envoyer des notifications de stratégie aux utilisateurs.](privacy-management-policies-notifications.md)

## <a name="view-current-alerts-and-issues"></a>Afficher les alertes et problèmes actuels

La **page** Vue d’ensemble de la gestion de la confidentialité fournit une vue d’ensemble des résultats récents avec des mises à jour sur les principaux domaines de préoccupation, tels que les stratégies ayant le plus de correspondances et vos alertes de stratégie actuellement actives. Pour en savoir plus sur les informations que cet affichage fournit, voir [Rechercher et visualiser vos données.](privacy-management-data-profile.md)

Vous pouvez également accéder aux visualisations et aux détails de vos alertes et problèmes via la page **principale des stratégies.** Sélectionnez **Afficher les alertes** et **Afficher les problèmes** pour afficher les détails.

## <a name="manage-alerts"></a>Gérer des alertes

Pour évaluer vos alertes actives et spécifier les alertes qui nécessitent un suivi, accédez à votre page **Alertes.** Il fournit une liste filtrable des alertes générées par vos stratégies. Vous pouvez les examiner individuellement pour déterminer les circonstances dans lesquelles elles ont été déclenchées.

La sélection d’une alerte ouvre un volet deover avec des détails supplémentaires, tels que le nombre d’éléments correspondants et la gravité selon les paramètres de votre stratégie. Sous **l’onglet** Contenu, vous pouvez passer en revue les fichiers impliqués dans cette alerte. Ces informations peuvent fournir des informations supplémentaires sur l’événement spécifique qui a déclenché l’alerte, l’endroit où se trouvent les fichiers et les types de données personnelles impliqués. Les déclencheurs des alertes sont déterminés par les conditions spécifiques de chaque stratégie. Par exemple, une alerte peut être déclenchée sur une stratégie de transfert de données si la gestion de la confidentialité détecte un transfert entre les départements ou régions spécifiés de la stratégie.

Après avoir évalué une alerte dans la liste, vous pouvez sélectionner Créer un **problème** pour inciter vos utilisateurs à poursuivre l’examen et à prendre des mesures. Vous serez invité à nommer le problème et à ajouter les commentaires pertinents pour le contexte. Vous pouvez également ignorer les alertes ici si elles ne nécessitent pas de suivi.

## <a name="manage-issues"></a>Gérer les problèmes

Les problèmes sont créés par les administrateurs lors de l’évaluation des alertes concernant les correspondances de stratégie. Pour suivre et résoudre les problèmes indiqués, les utilisateurs peuvent visiter la page **Problèmes.** À partir de là, vous pouvez examiner les problèmes individuels, examiner les conditions d’origine, examiner les données et prendre les mesures nécessaires pour fermer le cas.

Cette page fournit la liste de tous les problèmes ouverts. Ils sont répertoriés par nom et triés par gravité pour vous aider à hiérarchiser les cas, y compris les catégories élevée, moyenne et faible, ainsi que les catégories non classées. Sélectionnez un problème dans la liste pour examiner son contenu et prendre des mesures pour le résoudre. Vous pouvez évaluer la gravité des problèmes non signés lors de l’examen.

### <a name="review-issue-details"></a>Examiner les détails du problème

Les pages de détails des problèmes vous guident tout au long du processus de gestion des risques de confidentialité identifiés et de gestion des fichiers indiqués.

Les onglets des pages de détails des problèmes fournissent des informations sur les alertes et le contenu associés, notamment :

- **Vue d’ensemble**: présente les informations essentielles sur le problème. Consultez l’état actuel du problème et les actions recommandées suivantes à prendre. Vous pouvez également voir une vue d’ensemble du contenu, de la stratégie associée, des détails sur l’alerte et de la chronologie. La chronologie indique où vous vous trouvez pour récupérer du contenu. Le contenu téléchargé sera temporairement conservé pour révision.
- **Alertes**: liste détaillée des alertes associées au problème.
- **Contenu**: liste filtrable des éléments de contenu associés. Sélectionnez n’importe quel élément pour afficher des détails à son sujet, y compris les activités qui se sont produites et son historique de correction, si quelqu’un a déjà pris des mesures dans la gestion de la confidentialité pour gérer les données. Vous pouvez également choisir de prendre de nouvelles mesures correctives.
- **Remarques**: choisissez d’ajouter ou d’afficher des notes concernant le problème pour votre équipe.
- **Collaborateurs :** affichez et gérez la liste des collaborateurs qui peuvent contribuer à la résolution de ce problème.

### <a name="share-the-issue"></a>Partager le problème

L’ajout de personnes en tant que collaborateurs vous permet de partager le problème avec d’autres membres de votre entreprise via un canal Microsoft Teams sécurisé, un courrier électronique de l’entreprise ou en partageant un lien directement vers la page du problème dans la gestion de la confidentialité. Ces options sont disponibles sous le **bouton** Partager. Lors du partage via Teams, vous serez invité à sélectionner les équipes disponibles dans votre organisation, à sélectionner le canal spécifique et à laisser un message sur le problème, qui sera partagé avec le canal spécifié.

## <a name="review-content-and-remediate-issues"></a>Examiner le contenu et résoudre les problèmes

Pour examiner le contenu associé à  un problème, choisissez l’action Examiner le contenu si vous y êtes invité ou ouvrez **l’onglet** Contenu. Sélectionnez n’importe quel fichier de la liste pour l’afficher dans son intégralité. Vous pouvez y voir des détails sur le fichier, les activités sur l’enregistrement et son historique de correction, si des étapes précédentes ont été prises pour gérer ce fichier.

Utilisez le **bouton Corriger pour** prendre vos propres décisions de gestion des données pour ce contenu dans la gestion de la confidentialité. La sélection du bouton vous permet de choisir parmi une ou plusieurs actions de correction. Les options suivantes sont disponibles : 

**Toutes les stratégies**

- **Notifier le propriétaire**: informer le propriétaire du contenu du problème détecté.
- **Appliquer une étiquette de rétention**: ajoutez une étiquette sur la rétention des données pour cet élément. [En savoir plus sur les étiquettes de rétention.](/microsoft-365/compliance/create-apply-retention-labels)
- **Appliquer une étiquette de niveau de sensibilité**: ajoutez une étiquette sur la sensibilité des données de cet élément. [En savoir plus sur les étiquettes de sensibilité.](/microsoft-365/compliance/sensitivity-labels)
- **Marquer comme n’étant pas une correspondance**: identifiez un résultat de recherche comme faux positif pour supprimer l’élément de contenu de la considération.

**Réduction des données**

- **Supprimer**: utilisez cette option pour une suppression possible des données. Le contenu est déplacé dans le dossier des éléments supprimés ou dans la bac de recyclage (Exchange, SharePoint, OneDrive) ou supprimé avec une option de récupération (Teams messages). La suppression peut être annulée dans un laps de temps donné, en fonction des paramètres du service.

**Surexposation de données et transfert de données**

- **Rendre privé**: supprimez l’accès ouvert pour cet élément de contenu.

Chaque option vous invite à laisser des commentaires et toute autre information de prise en charge nécessaire pour le propriétaire du contenu avant de confirmer votre choix.

Une fois que toutes les mesures correctives ont été prises (y compris les actions que vous jugez conseillées en plus des options disponibles dans la gestion de la confidentialité) et que le problème est prêt à se fermer, utilisez le bouton Résoudre et ajoutez vos commentaires finaux avant de l’envoyer. 

## <a name="legal-disclaimer"></a>Clause d’exclusion de responsabilité légale

[Clause d’exclusion de responsabilité légale de gestion de la confidentialité](privacy-management-disclaimer.md)
