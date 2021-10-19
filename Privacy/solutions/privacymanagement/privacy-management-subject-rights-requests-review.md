---
title: Examiner les données et collaborer sur les demandes de droits de l’objet dans la gestion de la confidentialité
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
description: Découvrez comment examiner les données des demandes des droits de l’objet collectées par la gestion de la confidentialité et collaborer sur la réalisation de la demande.
ms.openlocfilehash: 7f0754007c70ef7836abf13ec0dbd50e9d9c8958
ms.sourcegitcommit: 85e085eb17af8b4efd1f45207445e1b3c3679600
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/19/2021
ms.locfileid: "60478251"
---
# <a name="review-data-and-collaborate-on-subject-rights-requests"></a>Examiner les données et collaborer sur des demandes de droits d’objet

Une fois que vous avez créé une demande de droits d’objet[(en](privacy-management-subject-rights-requests-create.md)savoir plus), la gestion de la confidentialité utilise vos entrées sur votre sujet pour rechercher des correspondances dans l’environnement Microsoft 365 de votre organisation. Une fois ces données compilées, vous pouvez passer en revue les résultats, faire des choix sur les informations à inclure et, si nécessaire, des informations. Ces étapes peuvent être prises en charge par plusieurs utilisateurs via l’interface de gestion de la confidentialité.

## <a name="step-1-review-request-details-and-monitor-progress"></a>Étape 1 : Examiner les détails de la demande et surveiller l’avancement

Pour voir les résultats initiaux de votre recherche, allez dans la zone de gestion de la confidentialité du Centre de conformité Microsoft 365 et [ouvrez](https://compliance.microsoft.com/) **les demandes de droits de l’objet.** Vous pouvez trouver la liste de toutes les demandes de droits d’objet ouvertes sur cette page principale.

Sélectionnez votre demande dans la liste pour voir les détails de la demande. Ici, vous pouvez en savoir plus sur les propriétés de la demande, les résultats de la recherche et l’état de la demande. Cette page devient votre hub pour travailler et collaborer sur la gestion des fichiers trouvés, la création de rapports et d’exportation et la réalisation de la demande.

Les vignettes de la page de détails de la demande sont les suivantes :

- **Détails :** détails essentiels sur la demande, y compris sa date d’échéance et de demande, sa description et la réglementation de confidentialité associée.
- **Progression**: chronologie indiquant les étapes terminées et les tâches à terminer.
- Statistiques sur votre étape de progression actuelle. Cette vignette peut afficher des informations telles qu’un résumé d’estimation des données, le nombre d’éléments trouvés dans votre recherche et leur emplacement dans Microsoft 365 ou l’état de vos exportations.
- **Éléments de priorité à réviser**: cette vignette affiche des informations sur les éléments importants détectés par la gestion de la confidentialité. Par exemple, il peut s’agir d’informations confidentielles portant déjà une étiquette de confidentialité Microsoft ou d’éléments avec des données sur plusieurs personnes qui peuvent nécessiter une action. Cela permettra aux administrateurs de savoir où commencer leur révision. Les éléments de priorité se trouvent sous Données collectées en filtrant par la colonne « Types de priorité ».

### <a name="understand-progress-stages"></a>Comprendre les étapes de progression

Les demandes de droits de l’objet sont soumises à plusieurs étapes. Certains progressent automatiquement à mesure que la gestion de la confidentialité effectue l’évaluation des données, tandis que d’autres avancent lorsque les administrateurs et les collaborateurs des droits de l’objet effectuent les étapes essentielles telles que la révision, la sélection et la révision de fichiers.

Étant donné que les demandes peuvent avoir besoin d’être travaillées au fil du temps ou par plusieurs collaborateurs, la gestion de la confidentialité fournit des mises à jour continues sur l’état et des conseils sur les étapes à suivre. Ces mises à jour peuvent être vues sur la page de présentation de la demande de droits d’objet.

1. **Estimation des données**: après la création d’une demande, la gestion de la confidentialité identifie les éléments qui incluent des correspondances potentielles avec votre personne objet de données et prend note de leurs emplacements dans Microsoft 365. Une fois l’estimation des données effectuée, vous avancerez automatiquement pour récupérer les **données,** sauf s’il existe des erreurs ou si votre demande est définie pour être suspendue ici pour révision par l’administrateur.
   - Votre demande peut être définie pour exiger une révision de l’administrateur à ce stade. Si votre administrateur détermine que les résultats initiaux de votre requête de recherche semblent satisfaisants, vous pouvez continuer à récupérer des données. Si vous souhaitez apporter des modifications avant de poursuivre, vous pouvez d’abord modifier votre requête de recherche. Pour plus d’informations, voir l’étape 2. Vous ne pourrez pas modifier votre requête de recherche une fois la phase de récupération des données initiée.
   - Si votre requête de recherche renvoie une estimation de données importante, ce qui signifie qu’elle dépasse le seuil recommandé de la gestion de la confidentialité pour la taille ou le nombre de fichiers, vous pouvez essayer de réviser votre recherche pour affiner son étendue. Notez que les fichiers associés à un élément correspondant (par exemple, les pièces jointes d’un e-mail) peuvent être comptabilisés dans votre total. Les estimations de données dépassant le maximum d’estimation de données de grande taille nécessiteront une révision de la recherche pour continuer.
1. **Récupérer des** données : cette étape indique que la gestion de la confidentialité est en cours de récupération de vos données. Une fois l’analyse terminée, elle avance automatiquement pour passer **en revue les données.**
1. **Examiner les** données : à ce stade, vos  collaborateurs doivent passer en revue les résultats sous l’onglet Données collectées et effectuer toutes les tâches applicables, telles que la rédaction, l’application de balises et l’ajout de notes. Lorsque vous avez terminé l’avis, sélectionnez **Terminer l’avis.**
1. **Générer des rapports**: vos rapports sont générés à ce stade. Lorsque vous avez terminé, vous pouvez les trouver sous **l’onglet Rapports.** Vos fichiers terminés peuvent être exportés pour révision et remise finales à la personne qui a effectué la demande.

## <a name="step-2-optional-view-and-edit-search-queries"></a>Étape 2 (facultative) : afficher et modifier les requêtes de recherche

Pour afficher des informations détaillées sur la recherche de données derrière une demande de droits d’objet, sélectionnez **Afficher les détails de la** requête de recherche. Cela ouvre un volet récapitulant la requête et affichant d’autres détails sur ce qui a été trouvé.

Vous avez la possibilité d’afficher **un aperçu** des résultats de recherche pour voir le type de contenu qui sera renvoyé pour cette requête. Si vous souhaitez modifier les propriétés de cette recherche et que vous n’avez pas commencé la phase Récupérer les données, vous pouvez utiliser l’option Modifier la requête **de recherche.**

L’Assistant Modifier la requête de recherche offre la possibilité de modifier ou d’ajouter des propriétés pour l’identification de la personne objet de données, vos filtres et conditions de recherche, ainsi que les emplacements dans lesquels rechercher des données (y compris Exchange, SharePoint, OneDrive et/ou Teams). Utilisez ces options pour atteindre le niveau de spécificité souhaité. Vous pouvez passer en revue la version finale de votre nouvelle requête avant d’atteindre **Enregistrer.**

Lorsque vous avez terminé de modifier votre requête de recherche, une nouvelle recherche s’exécute pour remplacer vos résultats de recherche précédents. Cela réinitialise votre état dans la section **Progression** à la première étape, **l’estimation des données.** La nouvelle recherche peut prendre jusqu’à 60 minutes. Une fois l’analyse effectuée, vous verrez les résultats mis à jour sur la page de détails de la demande.

## <a name="step-3-review-data"></a>Étape 3 : Examiner les données

À ce stade, vos collaborateurs doivent passer en revue les résultats sous **l’onglet Données collectées.** Les tâches essentielles sont les suivantes :

1. Examinez la liste des éléments identifiés et choisissez s’il faut inclure chaque fichier dans vos résumés et/ou exporter. Si vous n’avez pas besoin d’inclure une correspondance signalée, sélectionnez l’option « Exclure ». Si le contenu semble être un faux positif, vous pouvez choisir « Ne correspond pas » pour exclure le fichier de vos rapports finux et pointer l’élément comme un élément qui n’aurait pas dû être choisi par la demande. Pour définir l’état d’un élément, utilisez le menu d’action (ellipses verticales) en dehors de son nom et sélectionnez le choix souhaité. Si vous y êtes invité, ajoutez une note de référence interne pour expliquer votre décision. Les remarques sont requises lors de l’exclusion de fichiers.
1. Utilisez **l’option Appliquer des balises** pour vous aider à identifier les éléments qui doivent être à l’attention. Les balises disponibles incluent les options fournies par le système, par exemple le marquage d’un élément pour le suivi, et peuvent inclure des balises personnalisées telles que définies dans les paramètres globaux.
1. Utilisez **Annotate pour** créer des marques de texte inline ou pour redessiner des données dans un fichier sélectionné. Par exemple, si vous avez besoin d’inclure un fichier pour une personne qui contient également les informations personnelles d’autres personnes, vous pouvez utiliser l’action de zone **(sous** le bouton Dessin dans la barre de commandes) pour faire noircir toutes les informations qui ne concernent pas la personne qui a effectué la demande. Lorsque vos modifications sont terminées, **sélectionnez Inclure** pour ajouter le fichier rédigé à la demande. L’annotation crée une copie du fichier, de sorte que rien dans le fichier d’origine ne soit modifié et reste à son emplacement d’origine. La copie est stockée dans votre objet blob Azure.
1. Pour passer en revue les notes d’un élément, sélectionnez-le et sélectionnez **l’onglet Notes de** fichier. Vous pouvez également utiliser l’option **Ajouter une note de fichier** pour créer un commentaire. Pour passer en revue ou ajouter des notes à un niveau de cas global, rendez-vous dans l’onglet **Notes** principal ci-dessus et utilisez **la note de cas d’ajout.** Ces notes sont visibles pour les utilisateurs qui travaillent sur la demande, mais ne sont pas incluses dans le rapport final ou partagées avec la sujet des données.
1. Lorsque tous les éléments ont été révisés et que leurs statuts sont définies, sélectionnez **Terminer la révision.** Cela permet d’ouvrir un volet de survol dans lequel vous pouvez passer en revue un résumé des données et ajouter des notes pertinentes. Ces notes sont pour la conservation d’enregistrement interne et ne sont pas partagées avec la sujet de données.
1. Sélectionnez à nouveau Terminer l’avis pour continuer. Les résumés de vos décisions seront fournis ultérieurement sous l’onglet **Rapports.**

### <a name="collaborate-on-data-review"></a>Collaborer sur la révision des données

La gestion de la confidentialité prend en charge la collaboration Microsoft Teams pour permettre à votre groupe de travailler ensemble sur des demandes de droits d’objet. Lorsque vous créez une demande, un canal Teams est automatiquement créé et associé à votre demande par défaut. Ici, vous pouvez discuter de la demande et partager en toute sécurité les entrées et les contributions. Pour participer à la conversation, ouvrez votre demande et utilisez l’option **Conversation avec des** collaborateurs. Cela vous ouvre Microsoft Teams et vous place dans le canal Général pour le site d’équipe de votre demande de droits d’objet.

Pour consulter la liste des collaborateurs actifs qui peuvent afficher et contribuer à votre site d’équipe, dans votre demande de droits d’objet, ouvrez **l’onglet** Collaborateurs. Pour ajouter des utilisateurs supplémentaires afin de collaborer sur cette demande, sélectionnez l’option **Ajouter un collaborateur.**

Pour modifier le comportement par défaut de la génération de sites Teams lors de la création d’une demande de droits d’objet, sélectionnez **Paramètres** dans le mode de navigation supérieur et sélectionnez **Teams collaboration** pour modifier le paramètre.

Vous pouvez également  utiliser l’option Partager en haut à droite dans une demande de droit d’objet pour mettre en boucle des personnes par Teams ou par courrier électronique, ou pour copier le lien vers la page dans la gestion de la confidentialité. Le partage via Teams vous permet de sélectionner un site et un canal Teams existants disponibles pour votre compte, où il publiera un lien vers ce cas, ainsi que tout message que vous fournissez.

## <a name="step-4-close-the-request"></a>Étape 4 : Fermer la demande

Lorsque vous avez effectué toutes les actions nécessaires pour résoudre votre demande de droits d’objet, sélectionnez **Fermer la demande.** Cela crée le rapport final, qui sera chiffré et mis à disposition dans l’onglet **Rapports.** L’achèvement peut prendre un certain temps en fonction du nombre de fichiers dans la demande.

## <a name="next-steps"></a>Étapes suivantes
Pour en savoir plus sur l’working with reports and completing subject rights requests, see [Fulfill subject rights requests](privacy-management-subject-rights-requests-fulfill.md).

## <a name="legal-disclaimer"></a>Clause d’exclusion de responsabilité légale

[Clause d’exclusion de responsabilité légale de gestion de la confidentialité](privacy-management-disclaimer.md)
