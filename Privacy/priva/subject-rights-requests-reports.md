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
ms.openlocfilehash: 8a6a41188de78508401b0dfffb3d7cdefb2320a5
ms.sourcegitcommit: 4965df24fdc907f7a6e397f2c78019aaf72c7580
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/17/2022
ms.locfileid: "63564444"
---
# <a name="generate-reports-and-fulfill-a-subject-rights-request"></a>Générer des rapports et répondre à une demande de droits d’objet

Une fois que vous avez terminé votre révision des données pour une demande de droits d’objet dans Microsoft Priva, vous pouvez passer à la demande d’exécution. Priva crée des rapports et collecte les fichiers marqués pour **Inclure** pendant le processus de révision des données. Les fichiers sélectionnés à partir de ces packages de données peuvent être envoyés à votre objet de données pour terminer leur demande. Priva prend également en charge l’exploitation Microsoft 365 l’API des demandes de droits de sujet pour introduire des fonctionnalités d’automatisation.

## <a name="understanding-reports"></a>Comprendre les rapports

Une fois que **vous avez sélectionné Révision complète à** l’étape **Examiner** les données de la demande de droits de l’objet, les rapports finaux de la demande commenceront à être générés automatiquement. Sous **l’onglet Rapports** de la page détails des demandes de droits  de l’objet, la colonne État  indique quand la génération du rapport est en cours et quand un rapport est prêt **à être téléchargé**. La création des rapports peut prendre jusqu’à 30 minutes.

Les rapports sont divisés en deux sections :
1. **Rapports pour la sujet de données** : ces rapports contiennent des informations qui peuvent être renvoyées à la sujet des données dans le cadre de l’traitement des demandes. C’est ici que se trouve le **package** de données contenant des fichiers que vous pouvez envoyer à la sujet des données.
   > [!IMPORTANT]
   > Un package de données est généré uniquement si vous marquez des éléments **comme Étant inclus** pendant la révision des données.

   > [!IMPORTANT]
   > Un package de données sera uniquement généré pour les types de demandes **d’exportation** et **d’accès** . Un package de données ne sera pas généré pour une liste marquée **pour une demande de** suivi. Examiner les détails sur les [types de demande de droits d’objet](subject-rights-requests-create.md#use-the-subject-rights-request-creation-wizard).

2. **Rapports pour une utilisation interne** : ces rapports sont pour les enregistrements internes de votre organisation liés à la demande de droits de l’objet. Elles incluent un journal d’audit et une liste de tous les fichiers à qui vous avez appliqué des balises pendant la révision des données afin de suivre ou de prendre des mesures supplémentaires.

## <a name="prepare-final-reports-for-the-data-subject"></a>Préparer les rapports finux pour la sujet de données

Le package de données de demande de droits de l’objet est généré en tant que fichier zip. La générer peut prendre jusqu’à 30 minutes. Lorsqu’il est prêt, ouvrez votre demande de droits d’objet à partir de la page des  demandes de droits d’objet, ouvrez l’onglet Rapports, recherchez votre téléchargement et ouvrez le fichier zip.

Le package de données contient un large éventail de fichiers. Les fichiers en dehors du dossier Azure sont fournis à titre de référence et doivent être utilisés principalement par les administrateurs. Les documents clés de votre sujet de données sont contenus dans le **dossier Azure** .

Nous vous recommandons d’examiner attentivement le contenu de ce dossier et d’envoyer uniquement les fichiers nécessaires à votre personne à l’étude. Vous devez évaluer votre réponse pour vous assurer qu’elle est adaptée aux exigences de la loi applicable.

### <a name="azure-folder-contents"></a>Contenu du dossier Azure

Ouvrez ce dossier, puis ouvrez **AEDExport.zip** fichier. Les contenus sont les suivants :

- Le **Extracted_text_files** contient du texte extrait des fichiers natifs (si pris en charge).
- Le **dossier NativeFiles** contient tous les éléments **inclus** dans leur format de fichier natif.
- Les fichiers rédigés sont dans le **dossier NativeFiles** et ont le suffixe « _burn.pdf ».
- Les fichiers exportés sont renommés à l’aide d’identificateurs uniques pour protéger les données personnelles. Vous pouvez faire référence aux noms uniques avec les noms de fichier d’origine à l’aide **Export_load_file.csv.** Étant donné que les noms de fichiers d’origine peuvent inclure des informations sensibles, vous devez suivre vos stratégies qui s’appliquent à ces informations.

Après avoir passé en revue le contenu de votre fichier zip, modifiez-le selon vos besoins pour supprimer le contenu que vous ne souhaitez pas inclure dans le package final. Une fois terminé, envoyez-le en toute sécurité à votre sujet de données.

## <a name="integrate-with-partner-solutions"></a>Intégration avec des solutions partenaires

Vous pouvez intégrer la solution Demandes des droits de l’objet Priva à vos processus et outils d’entreprise existants à l’aide de l’API Microsoft 365 droits de l’objet. L’utilisation de l’API vous offre un moyen simple mais puissant d’introduire l’automatisation dans votre stratégie de droits d’objet.

Lorsque des personnes responsables des données demandent des informations à votre organisation, nos API peuvent vous aider à créer ces demandes dans Microsoft 365 en fonction des critères uniques de la demande. Vous pouvez créer la demande de droits d’objet dans Microsoft 365, suivre la progression de la demande tout au long de ses étapes et reconnaître que la demande a terminé le traitement et que le contenu est prêt à être récupéré. Nos API sont accessibles à tous pour rendre leurs solutions plus extensibles : qu’il s’agit des isv, des partenaires pour prendre en charge les Microsoft 365 dans leurs solutions ou pour les organisations à utiliser avec leurs applications métier.

Pour en savoir plus, [consultez l’API de demande de droits Graph Microsoft](/graph/api/resources/subjectrightsrequest-subjectrightsrequestapioverview).

## <a name="manage-data-retention"></a>Gérer la rétention des données

Les rapports générés par le biais de cet outil et les données associées, telles que les fichiers annotés enregistrés dans Azure, sont stockés pendant une durée spécifiée. La période de rétention des données est définie dans Priva **Paramètres** et s’applique à toutes les demandes de droits de l’objet. Pour afficher ou modifier vos périodes de rétention des données, suivez les étapes ci-dessous :

1. À partir de n’importe où dans les demandes des droits de l’objet **Priva**, sélectionnez Paramètres (icône d’engrenage) dans le coin supérieur droit de votre écran.
2. **Sélectionnez les périodes de rétention des données** dans le navigation de gauche.
3. Dans le menu déroulant, sélectionnez 30 jours ou 90 jours comme période de rétention.

Assurez-vous que les périodes de rétention de données que vous avez choisies sont conformes aux stratégies et obligations légales de votre organisation.

## <a name="legal-disclaimer"></a>Clause d’exclusion de responsabilité légale

[Clause d’exclusion de responsabilité légale Microsoft Priva](priva-disclaimer.md)
