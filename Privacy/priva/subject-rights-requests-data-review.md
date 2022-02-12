---
title: Examiner les données d’une demande de droits d’objet
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
description: Découvrez comment examiner les données des demandes des droits de l’objet collectées par Microsoft Priva et collaborer sur la réalisation de la demande.
ms.openlocfilehash: d8420667d3ad9bd2e42a1d6fc34b4681d7166452
ms.sourcegitcommit: 1f3f2757f456628ec904bc3df985b00ffba8f892
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/11/2022
ms.locfileid: "62542842"
---
# <a name="review-data-for-a-subject-rights-request"></a>Examiner les données d’une demande de droits d’objet

Une fois que vous avez créé une demande de droits d’objet [(en](subject-rights-requests-create.md) savoir plus) dans Microsoft Priva, la solution Demandes de droits d’objet utilise vos entrées pour rechercher des correspondances sur votre sujet de données dans l’environnement Microsoft 365 de votre organisation. Une fois ces données compilées, vous pouvez passer en revue les résultats, faire des choix sur les informations à inclure et, le cas échéant, fournir des informations. Ces étapes peuvent être prises en compte par plusieurs utilisateurs via l’interface Priva.

## <a name="step-1-review-request-details-and-monitor-progress"></a>Étape 1 : Examiner les détails de la demande et surveiller l’avancement

Pour voir les résultats initiaux de votre recherche, rendez-vous dans la zone Priva du [Centre de conformité Microsoft 365 et ouvrez](https://compliance.microsoft.com/) **les demandes de droits de l’objet**. Vous pouvez trouver la liste de toutes les demandes de droits d’objet ouvertes sur cette page principale.

Sélectionnez votre demande dans la liste pour voir les détails de la demande. Ici, vous pouvez en savoir plus sur les propriétés de la demande, les résultats de la recherche et l’état de la demande. Cette page deviendra votre hub pour travailler et collaborer sur la gestion des fichiers trouvés, la création de rapports et d’exportation et la réalisation de la demande.

Les vignettes de la page de détails de la demande sont les suivantes :

- **Détails :** détails essentiels sur la demande, y compris son échéance et sa date de demande, sa description et la réglementation de confidentialité associée.
- **Progression :** chronologie indiquant les étapes terminées et les tâches à terminer.
- Statistiques sur votre étape de progression actuelle. Cette vignette peut afficher des informations telles qu’un résumé d’estimation des données, le nombre d’éléments trouvés dans votre recherche et leur emplacement dans Microsoft 365 ou l’état de vos exportations.
- **Éléments de priorité à réviser** : cette vignette affiche des informations sur les éléments importants détectés par Priva pour vous. Par exemple, il peut s’agir d’informations confidentielles portant déjà une étiquette de confidentialité Microsoft ou d’éléments avec des données sur plusieurs personnes qui peuvent nécessiter une action. Cela permettra aux administrateurs de savoir où commencer leur révision. Les éléments de priorité se trouvent sous Données collectées par filtrage par la colonne « Types de priorités ».

### <a name="understand-progress-stages"></a>Comprendre les étapes de progression

Les demandes de droits de l’objet sont soumises à plusieurs étapes. Certaines progressent automatiquement au fil de l’évaluation des données par Priva, tandis que d’autres avancent lorsque les administrateurs et les collaborateurs des droits de l’objet effectuent les étapes essentielles telles que la révision, la sélection et la révision de fichiers.

Étant donné que les demandes peuvent avoir besoin d’être travaillées au fil du temps ou par plusieurs collaborateurs, Priva fournit des mises à jour continues sur l’état et des conseils sur les prochaines étapes à suivre. Ces mises à jour peuvent être vues sur la page de présentation de la demande de droits d’objet.

#### <a name="data-estimate"></a>Estimation des données
Une fois que vous avez créé une demande, Priva commence immédiatement à chercher des correspondances potentielles avec la sujet de données dans votre Microsoft 365 de données. Une fois que nous avons identifié tous les éléments qui correspondent à vos critères, vous verrez l’estimation dans  la carte récapitulatif d’estimation des données sur la page Vue d’ensemble de **la** demande. La quantité de données dans l’étendue de votre recherche aura une incidence sur le temps qu’il faudra pour effectuer l’estimation.

Votre demande passe automatiquement à l’étape suivante de récupération des données, dans laquelle tous les éléments de contenu sont rassemblés afin que vos parties prenantes peuvent collaborer sur leur révision des données. Toutefois, dans certains cas, nous suspendons l’estimation des données avant de passer à la récupération et vous informons des étapes suivantes à suivre avant de poursuivre.

Vous pouvez également choisir de suspendre automatiquement à l’étape d’estimation des données lorsque vous créez une demande de droits d’objet pour la première fois. Pendant le processus de création, sélectionnez l’option Obtenir une estimation **en premier** lors de **l’étape Paramètres de** recherche. Examinez les détails de [l’étape des paramètres de recherche](subject-rights-requests-create.md#define-search-settings).

#### <a name="pause-in-data-estimate-for-large-search-results"></a>Suspendre l’estimation des données pour les résultats de recherche importants

Priva remarque si votre estimation des données est projetée pour renvoyer une grande quantité d’éléments à réviser (plus de 10 000 éléments). L’estimation sera suspendue afin que vous pouvez afficher un aperçu des résultats et [](subject-rights-requests-create.md#refine-your-search) décider s’il faut modifier votre requête de recherche pour cibler des emplacements ou des conditions plus spécifiques, ou continuer à récupérer les éléments identifiés.  Nous vous montrerons à l’écran le nombre d’éléments et le volume de données qui correspondent à votre recherche. Vous avez l’une des options suivantes ou les deux dans une barre de messages en haut de l’écran :

- Un **bouton Modifier la** requête de recherche vous permet d’entrer directement dans les paramètres de recherche de la demande pour définir des paramètres plus stricts et générer une nouvelle estimation.
- Tant que votre requête de recherche ne compte pas plus de 300 000 éléments, vous verrez également une option pour récupérer **des données**. Cela vous permet de choisir de ne pas modifier votre recherche et de continuer à collecter les données.

#### <a name="retrieve-data"></a>Récupérer des données
L’étape de récupération des données se produit lorsque tous les fichiers, messages électroniques, conversations, images et autres éléments de contenu contenant les données personnelles de la sujet de données sont récupérés et rassemblés dans un conteneur de stockage d’objets blob Azure pour révision. La récupération des données peut prendre quelques minutes ou beaucoup plus en fonction du volume de données. Lorsque cette étape est terminée, la demande passe automatiquement à l’étape suivante des données **de révision**.

#### <a name="review-data"></a>Examiner les données
 À ce stade, vos collaborateurs doivent passer en revue les résultats sous l’onglet Données collectées et effectuer toutes les tâches applicables, telles que la rédaction, l’application de balises et l’ajout de notes. Lorsque vous avez terminé l’avis, sélectionnez **Terminer l’avis**.

#### <a name="generate-reports"></a>Générer des rapports
Vos rapports sont générés à ce stade. Lorsque vous avez terminé, vous pouvez les trouver sous **l’onglet Rapports** . Vos fichiers terminés peuvent être exportés pour révision et remise finales à la personne qui a effectué la demande.

#### <a name="close-the-request"></a>Fermer la demande
Une demande fermée indique que tout le travail a été effectué pour répondre à cette demande de droits d’objet. Toutes les données collectées et les rapports seront conservés en fonction de vos [paramètres de rétention des données](priva-settings.md#data-retention-periods).

## <a name="step-2-optional-view-and-edit-search-queries"></a>Étape 2 (facultative) : afficher et modifier les requêtes de recherche

Pour afficher des informations détaillées sur la recherche de données derrière une demande de droits d’objet, sélectionnez **Afficher les détails de la requête de recherche**. Cela ouvre un volet récapitulant la requête et affichant d’autres détails sur ce qui a été trouvé.

Vous avez la possibilité ici d’afficher **un aperçu** des résultats de recherche pour voir le type de contenu qui sera renvoyé pour cette requête. Si vous souhaitez modifier les propriétés de cette recherche et que vous n’avez pas commencé la phase Récupérer les données, vous pouvez utiliser l’option Modifier la requête **de recherche** .

Le processus guidé de modification de requête de recherche vous permet de modifier ou d’ajouter des propriétés pour l’identification de la sujet de données, vos filtres et conditions de recherche, ainsi que les emplacements dans lesquels rechercher des données (y compris Exchange, SharePoint, OneDrive et/ou Teams). Utilisez ces options pour atteindre le niveau de spécificité souhaité. Vous pouvez passer en revue la version finale de votre nouvelle requête avant d’atteindre **Enregistrer**.

Lorsque vous avez terminé de modifier votre requête de recherche, une nouvelle recherche s’exécute pour remplacer vos résultats de recherche précédents. Cela réinitialise votre état dans la section **Progression** à la première étape, **Estimation des données**. La nouvelle recherche peut prendre jusqu’à 60 minutes. Une fois l’analyse effectuée, vous verrez les résultats mis à jour sur la page de détails de la demande.

## <a name="step-3-review-data"></a>Étape 3 : Examiner les données

À ce stade, vos collaborateurs doivent passer en revue les résultats sous **l’onglet Données collectées** . Les tâches essentielles sont les suivantes :

1. Examinez la liste des éléments identifiés et choisissez s’il faut inclure chaque fichier dans vos résumés et/ou exporter. Si vous n’avez pas besoin d’inclure une correspondance signalée, sélectionnez l’option « Exclure ». Si le contenu semble être un faux positif, vous pouvez choisir « Ne correspond pas » pour exclure le fichier de vos rapports finux et pointer l’élément comme un élément qui n’aurait pas dû être choisi par la demande. Pour définir l’état d’un élément, utilisez le menu d’action (ellipses verticales) en dehors de son nom et sélectionnez le choix souhaité. Si vous y êtes invité, ajoutez une note de référence interne pour expliquer votre décision. Les remarques sont requises lors de l’exclusion de fichiers.
1. Utilisez **l’option Appliquer des balises** pour vous aider à identifier les éléments qui doivent être à l’attention. Les balises disponibles incluent les options fournies par le système, par exemple le marquage d’un élément pour le suivi, et peuvent inclure des balises personnalisées telles que définies dans les paramètres globaux.
1. Utilisez **Annotate pour** créer des marques de texte inline ou pour redessiner des données dans un fichier sélectionné. Par exemple, si vous avez besoin d’inclure un fichier pour une personne qui contient également les informations personnelles d’autres personnes, vous pouvez utiliser l’action de **zone (sous** le bouton Dessin dans la barre de commandes) pour faire noircir toutes les informations qui ne concernent pas la personne qui a effectué la demande. Lorsque vos modifications sont terminées, **sélectionnez Inclure** pour ajouter le fichier rédigé à la demande. L’annotation crée une copie du fichier, de sorte que rien dans le fichier d’origine ne soit modifié et reste à son emplacement d’origine. La copie est stockée dans votre objet blob Azure.
1. Pour passer en revue les notes d’un élément, sélectionnez-le et sélectionnez **l’onglet Notes de** fichier. Vous pouvez également utiliser l’option **Ajouter une note de fichier** pour créer un commentaire. Pour passer en revue ou ajouter des notes à un niveau de cas global, rendez-vous dans l’onglet **Notes** principal ci-dessus et utilisez **ajouter une note de cas**. Ces notes sont visibles pour les utilisateurs qui travaillent sur la demande, mais ne sont pas incluses dans le rapport final ou partagées avec la sujet des données.
1. Une fois que tous les éléments ont été révisés et que leurs statuts ont été définies, sélectionnez **Terminer la révision**. Cela permet d’ouvrir un volet de survol dans lequel vous pouvez passer en revue un résumé des données et ajouter des notes pertinentes. Ces notes sont pour la conservation d’enregistrement interne et ne sont pas partagées avec la sujet de données.
1. Sélectionnez à nouveau Terminer l’avis pour continuer. Les résumés de vos décisions seront fournis ultérieurement sous l’onglet **Rapports** .

### <a name="collaborate-on-data-review"></a>Collaborer à la révision des données

Priva prend en charge la collaboration par Microsoft Teams pour permettre à votre groupe de travailler ensemble sur des demandes de droits d’objet. Lorsque vous créez une demande, un canal Teams est automatiquement créé et associé à votre demande par défaut. Ici, vous pouvez discuter de la demande et partager en toute sécurité les entrées et les contributions. Pour participer à la conversation, ouvrez votre demande et utilisez l’option **Conversation avec des** collaborateurs. Cela vous ouvre Microsoft Teams et vous place dans le canal Général pour le site d’équipe de votre demande de droits d’objet.

Pour consulter la liste des collaborateurs actifs qui peuvent afficher et contribuer à votre site d’équipe, dans votre demande de droits d’objet, ouvrez **l’onglet** Collaborateurs. Pour ajouter des utilisateurs supplémentaires à cette demande, sélectionnez l’option **Ajouter un collaborateur**.

Pour modifier le comportement par défaut de la génération de sites Teams lors de la création d’une demande de droits d’objet, sélectionnez **Paramètres** dans le mode de navigation supérieur et sélectionnez **Teams collaboration** pour modifier le paramètre.

Vous pouvez également utiliser **l’option Partager** en haut à droite au sein d’une demande d’objet droit pour mettre en boucle des personnes par Teams ou par courrier électronique, ou pour copier le lien vers la page dans Priva. Le partage via Teams vous permet de sélectionner un site et un canal Teams existants disponibles pour votre compte, où il publiera un lien vers ce cas, ainsi que tout message que vous fournissez.

## <a name="step-4-close-the-request"></a>Étape 4 : Fermer la demande

Lorsque vous avez effectué toutes les actions nécessaires pour résoudre votre demande de droits d’objet, sélectionnez **Fermer la demande**. Cela crée le rapport final, qui se trouve sous l’onglet **Rapports**. L’achèvement peut prendre un certain temps en fonction du nombre de fichiers dans la demande.

## <a name="next-steps"></a>Prochaines étapes
Pour en savoir plus sur l’emploi de rapports et la réalisation de demandes de droits d’objet, voir [Générer des rapports et répondre à une demande de droits d’objet](subject-rights-requests-reports.md).

## <a name="legal-disclaimer"></a>Clause d’exclusion de responsabilité légale

[Clause d’exclusion de responsabilité légale Microsoft Priva](priva-disclaimer.md)
