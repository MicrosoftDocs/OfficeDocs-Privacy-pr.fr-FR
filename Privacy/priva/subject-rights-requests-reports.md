---
title: Générer des rapports et répondre à une demande de droits d’objet
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
description: Découvrez comment gérer les packages de données créés par Microsoft Priva pour les demandes de droits d’objet et comment satisfaire la demande à la personne à l’origine du traitement des données.
ms.openlocfilehash: a72dfb53e4f642cd2c567896c854af2beaedd416
ms.sourcegitcommit: beeb693075ef692e95d679f366301df8517b2ac3
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/23/2022
ms.locfileid: "63765517"
---
# <a name="generate-reports-and-fulfill-a-subject-rights-request"></a>Générer des rapports et répondre à une demande de droits d’objet

Une fois que vous avez terminé votre révision des données pour une demande de droits d’objet dans Microsoft Priva, vous pouvez passer à la demande. Priva crée des rapports et collecte les fichiers marqués comme **Include** pendant le processus de révision des données. Les fichiers sélectionnés à partir de ces packages de données peuvent être envoyés à votre objet de données pour terminer leur demande. Priva prend également en charge l’exploitation Microsoft 365 l’API des demandes de droits de sujet pour introduire des fonctionnalités d’automatisation.

## <a name="understanding-reports"></a>Comprendre les rapports

Une fois que **vous avez sélectionné Révision complète à** l’étape **Examiner** les données de la demande de droits de l’objet, les rapports finaux de la demande commenceront à être générés automatiquement. Sous **l’onglet Rapports** de la page détails des demandes de droits  de l’objet, la colonne État  indique quand la génération du rapport est en cours et quand un rapport est prêt **à être téléchargé**. La création des rapports peut prendre jusqu’à 30 minutes.

Les rapports sont divisés en deux sections :
1. **Rapports pour la sujet de données** : ces rapports contiennent des informations qui peuvent être renvoyées à la sujet des données dans le cadre de l’traitement des demandes. C’est ici que se trouve le **package** de données contenant des fichiers que vous pouvez envoyer à la sujet des données.
   > [!IMPORTANT]
   > Un package de données est généré uniquement si vous marquez des éléments **comme Étant inclus** pendant la révision des données.

   > [!IMPORTANT]
   > Un package de données sera uniquement généré pour les types de demandes **d’exportation** et **d’accès** . Un package de données ne sera pas généré pour une liste marquée **pour une demande de** suivi. Examiner les détails sur les [types de demande de droits d’objet](subject-rights-requests-create.md#use-the-subject-rights-request-creation-wizard).

2. **Rapports pour une utilisation interne** : ces rapports sont pour les enregistrements internes de votre organisation liés à la demande de droits de l’objet. Elles incluent un journal d’audit et une liste de tous les fichiers à qui vous avez appliqué des balises pendant la révision des données afin de suivre ou de prendre des mesures supplémentaires.

> [!NOTE]
> Lorsque des rapports sont générés, l’organisation termine la demande en envoyant les rapports appropriés de manière sécurisée à la personne objet de données afin de répondre à la demande de droits de l’objet. Si la sujet des données a demandé la suppression de ses données, il incombe à l’organisation d’identifier les éléments à suppression et d’effectuer la suppression.

## <a name="data-package"></a>Package de données

Le package de données de demande de droits de l’objet contient des éléments marqués comme **Étant inclus** pendant la phase de révision des données du processus. Le package de données est généré en tant que fichier zip. Lorsqu’il est prêt pour le téléchargement, sélectionnez la ligne du rapport sous l’onglet **Rapports** de la page détails de la demande de droits de l’objet. Un panneau volant s’ouvre avec un bouton pour **télécharger** le rapport. Les **instructions suivantes sur** les étapes à suivre dans le panneau volant fournissent une référence rapide sur l’emploi du contenu.

Lorsque vous êtes prêt à télécharger le package de données, sélectionnez **Télécharger**, recherchez votre téléchargement, puis ouvrez le fichier zip téléchargé.

### <a name="contents-of-the-data-package"></a>Contenu du package de données

Le fichier zip du package de données contient les éléments suivants :

- Un dossier nommé **Azure** : ce dossier contient les documents clés pour votre sujet de données. Consultez l’explication détaillée ci-dessous.
- Fichiers en dehors du **dossier Azure** : il peut s’agir de deux feuilles de calcul nommées **Résultats** et **Résumé**. Ces fichiers en dehors du dossier Azure sont fournis à titre de référence et doivent être utilisés principalement par les administrateurs de votre organisation.

Lorsque Priva identifie et récupère des fichiers pour une demande de droits d’objet, les fichiers qu’il exporte dans ce processus sont renommés à l’aide d’identificateurs uniques pour protéger les données personnelles. Vous pouvez faire référence aux noms uniques avec les noms de fichier d’origine à l’aide **Export_load_file.csv** fichier. Étant donné que les noms de fichiers d’origine peuvent inclure des informations sensibles, vous devez suivre vos stratégies qui s’appliquent à ces informations.

> [!NOTE]
> Nous vous recommandons d’examiner attentivement le contenu de ce dossier et d’envoyer uniquement les fichiers nécessaires à votre personne à l’étude. Vous devez évaluer votre réponse pour vous assurer qu’elle est adaptée aux exigences de la loi applicable.

### <a name="azure-folder-contents"></a>Contenu du dossier Azure

Ouvrez **le dossier Azure** , puis ouvrez **le fichierAEDExport.zip** , qui contient un autre dossier de fichiers avec un nom long composé de chiffres et de lettres. Ouvrez le dossier avec le nom long pour révéler le contenu décrit ci-dessous :

- **Extracted_text_files** dossier : contient du texte extrait des fichiers natifs (si pris en charge).
- **Dossier NativeFiles** : contient tous les éléments marqués lors de la révision des données comme **Inclus**, dans leur format de fichier natif. Un nom de fichier unique est attribué à chaque élément de ce dossier pour protéger les données personnelles. Vous pouvez faire référence à ces noms uniques avec leur nom de fichier d’origine à l’aide Export_load_file.csv fichier, expliqué ci-dessous.
  - Les fichiers qui ont été rédigés à l’aide de la fonction **Annotate** pendant le processus de révision des données se classent dans le dossier **NativeFiles** et ont le suffixe « _burn.pdf ».
- **Export_load_file.csv** : contient les noms de fichiers d’origine afin que vous pouvez les référencer de manière croisée avec les noms de fichiers uniques fournis dans le dossier NativeFiles.
- **Fichier texte** récapitulatif : fournit un résumé des types de fichiers dans le package de données, du nombre de fichiers et de leur taille.

##### <a name="what-to-do-with-the-folder-contents"></a>Que faire avec le contenu du dossier

Ouvrez **le dossier Azure** et les fichiers zip, comme expliqué ci-dessus. Votre tâche suivante consiste à examiner les éléments, à déterminer ce qu’il faut envoyer à la sujet des données et à modifier le contenu du fichier zip si nécessaire.

Par exemple, pour une demande d’exportation dans laquelle la personne responsable des données souhaite recevoir une copie de tous les éléments contenant leurs données personnelles détenues par l’organisation, vous pouvez examiner attentivement les éléments du dossier **NativeFiles** et supprimer tout élément que vous ne souhaitez pas renvoyer à la personne à l’origine du problème.

Pour une demande d’accès dans laquelle la personne responsable des données souhaite recevoir un résumé de toutes ses informations personnelles détenues par l’organisation, vous pouvez  vous concentrer sur le fichier texte Résumé.

Modifiez le fichier zip pour supprimer le contenu que vous ne souhaitez pas inclure dans le package final. Une fois terminé, envoyez le fichier zip de manière sécurisée à la personne qui a effectué la demande de droits d’objet.

## <a name="audit-log"></a>Journal d’audit

Le journal d’audit est un fichier CSV qui fournit un enregistrement de la progression des étapes pour chaque demande de droits d’objet. Il répertorie chaque étape du processus, ainsi que la date et l’heure terminées, ainsi que le nom d’utilisateur de la personne qui a terminé l’étape.

## <a name="tagged-files-reports"></a>Rapports de fichiers marqués

Les rapports étiquetés comme fichiers marqués comme **...** sont des fichiers CSV qui résentent les éléments de contenu pour lesquels des balises ont été appliquées au cours du processus de révision des données. Les balises sont utilisées pour baliser les éléments de contenu pour une attention ou une action supplémentaire de l’organisation. En savoir plus sur [les paramètres des balises](priva-settings.md#data-review-tags).

## <a name="retention-periods-for-reports-and-data"></a>Périodes de rétention pour les rapports et les données

Les rapports générés par les demandes de droits de l’objet et les données associées, telles que les fichiers annotés enregistrés dans Azure, sont stockés pendant une durée spécifiée. La période de rétention par défaut est de 30 jours à partir de la date à laquelle une demande de droits d’objet est fermée.

La période de rétention des données est définie dans Priva **Paramètres** et s’applique à toutes les demandes de droits de l’objet. Pour afficher ou modifier votre période de rétention des données, suivez les étapes ci-dessous :

1. À partir de n’importe où dans les demandes des droits de l’objet **Priva**, sélectionnez Paramètres (icône d’engrenage) dans le coin supérieur droit de votre écran.
2. **Sélectionnez les périodes de rétention des données** dans le navigation de gauche.
3. Dans le menu déroulant Données **collectées et** rapports, sélectionnez 30 jours ou 90 jours comme période de rétention.
4. **Sélectionnez Enregistrer** pour enregistrer vos paramètres.

Assurez-vous que les périodes de rétention de données que vous avez choisies sont conformes aux stratégies et obligations légales de votre organisation.

## <a name="integrate-with-partner-solutions"></a>Intégration avec des solutions partenaires

Vous pouvez intégrer la solution Demandes des droits de l’objet Priva à vos processus et outils d’entreprise existants en tirant parti de l Microsoft 365 API de demande de droits de l’objet. Cela vous offre un moyen simple mais puissant d’introduire l’automatisation dans votre stratégie de droits d’objet.

Lorsque des personnes responsables des données demandent des informations à votre organisation, vous pouvez tirer parti de nos API pour créer ces demandes dans Microsoft 365 en fonction des critères personnalisés pour cette demande. Vous pouvez créer la demande de droits d’objet dans Microsoft 365, suivre la progression de la demande tout au long de ses étapes et reconnaître que la demande a terminé le traitement et que le contenu est prêt à être récupéré. Nos API sont accessibles à tous pour rendre leurs solutions plus extensibles : qu’il s’agit des isv, des partenaires pour prendre en charge les Microsoft 365 dans leurs solutions ou pour les organisations à utiliser avec leurs applications métier.

Pour en savoir plus, [consultez l’API de demande de droits Graph Microsoft](/graph/api/resources/subjectrightsrequest-subjectrightsrequestapioverview).

## <a name="legal-disclaimer"></a>Clause d’exclusion de responsabilité légale

[Clause d’exclusion de responsabilité légale Microsoft Priva](priva-disclaimer.md)
