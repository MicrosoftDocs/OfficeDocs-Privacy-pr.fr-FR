---
title: Flux de travail pour les demandes de droits d’objet
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
description: Comprendre les étapes du flux de travail et la page des détails de la demande dans Demandes de droits des personnes concernées Microsoft Priva.
ms.openlocfilehash: 794176260f6377862d34a66dc71cef1e811188b9
ms.sourcegitcommit: fe651dab4c89e67b21d37531c04e3996b7af1138
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/14/2022
ms.locfileid: "66060086"
---
# <a name="understand-the-workflow-and-request-details-pages"></a>Comprendre les pages de détails du flux de travail et des demandes

**Dans cet article** : Découvrez les étapes de progression à mesure que vous créez et traitez une demande. Découvrez comment utiliser les insights et les fonctionnalités de la page de détails de chaque requête.

Lorsque vous [créez une demande](subject-rights-requests-create.md) dans la solution Demandes de droits des personnes concernées, les informations que vous fournissez sont utilisées pour rechercher des correspondances sur votre sujet de données dans l’environnement Microsoft 365 de votre organisation. Les éléments correspondants sont conformes pour vous permettre de passer en revue, de faire des choix sur ce qu’il faut inclure et de rétablir les informations si nécessaire. Plusieurs utilisateurs peuvent collaborer sur ces étapes dans l’interface Demandes de droits d’objet. La page [Vue d’ensemble](#overview-tab) de la demande fournit l’état des étapes de progression et des conseils sur les étapes à suivre.

## <a name="progress-stages-for-requests"></a>Étapes de progression des demandes

Chaque requête passe par plusieurs étapes. Certaines étapes progressent automatiquement, et d’autres sont avancées manuellement après la fin de certaines étapes, telles que l’examen des fichiers.

- **Estimation des données** : avant de récupérer les données, Priva estime la quantité de données qu’elle s’attend à trouver. Selon la quantité de données, la demande peut ou non passer automatiquement à l’étape suivante de récupération des données. Vous pouvez définir une demande pour qu’elle s’interrompe à l’étape de l’estimation avant de collecter des données ; en savoir plus sur [l’estimation et la récupération des données](subject-rights-requests-data-retrieval.md).

- **Récupérer des données** : tous les fichiers, e-mails, conversations, images et autres éléments de contenu sont regroupés. Une fois cette étape terminée, la demande passe automatiquement à l’étape suivante de l’examen des données. En savoir plus sur [l’estimation et la récupération des données](subject-rights-requests-data-retrieval.md).

- **Passer en revue les données** : les collaborateurs examinent toutes les données collectées, déterminent celles qui se rapportent à la demande et effectuent des tâches telles que la rédaction de fichiers et l’ajout de notes de cas. En savoir plus sur [la révision des données pour une demande de droits d’objet](subject-rights-requests-data-review.md). Une fois la révision des données terminée, vous passez manuellement à l’étape suivante pour générer des rapports.

- **Générer des rapports** : une fois la révision des données terminée, un utilisateur passe manuellement à cette étape. Priva génère les rapports finaux, qui incluent le package de données à partager avec la personne concernée, et les rapports internes pour les enregistrements de votre organisation. En savoir plus sur [la génération de rapports](subject-rights-requests-reports.md).

- **Fermez la demande** : lorsque tout le travail est terminé, fermez la demande pour indiquer qu’elle est considérée comme terminée. En savoir plus sur [la génération de rapports](subject-rights-requests-reports.md) afin que vous puissiez traiter et fermer la demande.

## <a name="understanding-the-request-details-page"></a>Présentation de la page de détails de la demande

Sélectionnez **Demandes de droits des personnes concernées Priva** dans le volet de navigation gauche du portail de conformité Microsoft Purview pour accéder aux demandes créées par votre organisation et afficher leur état. Les cartes d’état de la page principale demandes de droits d’objet, affichées ci-dessous, indiquent le nombre de demandes actives, fermées et en retard, ainsi que les principaux types de demandes. Le tableau sous les cartes d’état répertorie toutes les demandes créées par votre organisation, avec la demande la plus récente en haut.

**Page principale des demandes de droits d’objet :** 
![ Page principale demandes de droits d’objet.](../media/priva-srr-overview.png)

Pour ouvrir la page de détails d’une demande, sélectionnez le nom de la demande dans la table. Ici, vous pouvez en savoir plus sur les propriétés de la demande, les résultats de la recherche et l’état de la demande. La page de détails, affichée ci-dessous, deviendra votre hub pour travailler et collaborer sur la gestion des fichiers trouvés, la création de rapports et d’exportations et la réalisation de la demande.

**Page de détails d’une demande :**
![ Page de détails de la demande de droits d’objet.](../media/priva-srr-detailspage.png)

### <a name="overview-tab"></a>Onglet Overview

L’onglet **Vue d’ensemble** de la page détails de la demande fournit des détails sur la demande, un indicateur de progression montrant votre étape actuelle et des informations clés sur les données trouvées. Cette page contient des cartes d’état individuelles expliquées ci-dessous.

##### <a name="details"></a>Détails

La carte **Détails affiche des** informations de base pour vous orienter vers la demande, telles que son échéance, la date de création, la description et la réglementation relative à la confidentialité associée.

##### <a name="progress"></a>Progression

La carte **progression** répertorie chaque étape du processus : Estimation des données, Récupération des données, Examiner les données, Générer des rapports et Fermer la demande. Un cercle bleu rempli en regard de l’étape indique l’étape sur laquelle vous êtes actuellement. Une coche dans le cercle bleu signifie que l’étape est terminée. Un cercle vide signifie que l’étape n’a pas encore démarré.

##### <a name="data-estimate-summary"></a>Résumé de l’estimation des données

La carte **récapitulative d’estimation** des données s’affiche lorsque la demande est suspendue à [l’étape d’estimation des données](subject-rights-requests-data-retrieval.md#data-estimate). Il indique l’emplacement et le nombre d’éléments que votre recherche doit récupérer.

##### <a name="total-number-of-items-found"></a>Nombre total d’éléments trouvés

Le **nombre total d’éléments trouvés** affiche le nombre d’éléments de contenu trouvés et leur emplacement dans Microsoft 365.

##### <a name="priority-items-to-review"></a>Éléments de priorité à examiner

La vignette **Éléments de priorité à examiner** affiche les éléments que vous souhaiterez peut-être hiérarchiser au démarrage de votre révision. La vignette affiche un nombre d’éléments appartenant aux catégories suivantes :
- **Confidentiel** : ces éléments ont une [étiquette de confidentialité Microsoft](/microsoft-365/compliance/sensitivity-labels) qui leur est appliquée. Par exemple, un document Word avec une étiquette « Hautement confidentiel ». 
- **Données multi-personnes** : ces éléments contiennent les données personnelles de plusieurs personnes. Si vous souhaitez inclure ces éléments dans le package de données final, vous devez rétablir les données non pertinentes dans les fichiers. Obtenez [des détails sur l’examen des données](subject-rights-requests-data-review.md). Pour Priva identifier les éléments contenant des données multi-personnes, votre organisation doit configurer la [correspondance des données pour les demandes de droits des personnes concernées](subject-rights-requests-data-match.md).

**Comment localiser vos éléments prioritaires :**

Tout d’abord, vérifiez que vous avez activé votre vue de ces éléments dans votre table d’éléments **collectées** par les données en suivant les étapes ci-dessous :

- Sous l’onglet **Données collectées** , sélectionnez **Personnaliser les colonnes** en haut de la liste des éléments.
- Dans le volet volant **Modifier les colonnes** , placez une vérification en regard des **types De priorité**.
- Sélectionnez **Appliquer**. Votre liste d’éléments aura désormais une colonne **de types De priorité** .

Vous pouvez maintenant identifier les éléments de priorité et les trouver en triant la colonne **de type Priority** pour regrouper des types similaires.

### <a name="data-collected-tab"></a>Onglet Données collectées

Lorsque tous les éléments correspondant à vos paramètres de recherche ont été identifiés, ils sont collectés et présentés sous l’onglet **Données collectées** . À côté de la liste des éléments se trouve un écran d’aperçu permettant de passer en revue chaque élément, d’effectuer des actions et de marquer les éléments comme inclus ou exclus dans le cadre de la demande. En savoir plus sur [l’étape de révision et de collaboration des données](subject-rights-requests-data-review.md).

### <a name="notes-tab"></a>Onglet Notes

L’onglet **Notes** permet aux collaborateurs d’entrer des notes sur le travail effectué sur la demande. Ces notes sont visibles par toutes les personnes qui travaillent sur la demande, mais ne seront pas incluses dans le rapport final ou partagées avec la personne concernée.

### <a name="collaborators-tab"></a>Onglet Collaborateurs

L’onglet Collaborateurs affiche tous les utilisateurs qui ont été invités à collaborer sur les données collectées, ainsi que tous les canaux Teams associés pour la demande. Le créateur de la requête est automatiquement répertorié en tant que collaborateur. Invitez de nouveaux collaborateurs en sélectionnant la commande **Ajouter un collaborateur** et en entrant le nom d’un utilisateur pour le sélectionner dans une liste. En savoir plus sur la [collaboration pour la révision des données](subject-rights-requests-data-review.md#collaboration-for-data-review)

### <a name="reports-tab"></a>Onglet Rapports

L’onglet **Rapports** affiche tous les rapports générés automatiquement lorsque vous passez à l’étape **Générer des rapports** . Les rapports sont séparés en deux catégories : les rapports à partager avec la personne concernée et les rapports destinés à l’utilisation interne de votre organisation. Obtenez des détails sur [l’utilisation des rapports](subject-rights-requests-reports.md).

### <a name="history-tab"></a>Onglet Historique

**L’onglet Historique** récapitule les événements de niveau supérieur pour la demande, y compris les modifications de l’étape de progression et les agrégats pour le nombre d’éléments inclus, exclus et supprimés.

## <a name="next-steps"></a>Prochaines étapes

Visitez [Créer une demande de droits d’objet](subject-rights-requests-create.md) pour savoir comment être indiqué avec votre première demande.

## <a name="legal-disclaimer"></a>Exclusion de responsabilité légale

[Microsoft Priva exclusion de responsabilité légale](priva-disclaimer.md)