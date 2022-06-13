---
title: Générer des rapports et fermer une requête
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
description: Découvrez comment gérer les packages de données créés par Microsoft Priva pour les demandes de droits d’objet et traiter la demande à la personne concernée.
ms.openlocfilehash: 44113c480f81e6ef885de3649d9e04810c776d7c
ms.sourcegitcommit: 3c83e8133a5a71f4e1d76a0b2981ab3ec9cd6602
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/13/2022
ms.locfileid: "66046688"
---
# <a name="generate-reports-and-close-a-request"></a>Générer des rapports et fermer une requête

**Dans cet article** : Comprendre le type de rapports générés dans les demandes de droits des personnes concernées. Découvrez les périodes de rétention des données collectées et trouvez des instructions pour fournir des résultats à la personne concernée et fermer la demande.

Une fois que vous avez terminé votre examen des données pour une demande de droits d’objet, l’étape suivante consiste à générer les rapports nécessaires pour répondre à la demande. Priva crée des rapports et collecte les fichiers marqués comme **Include** pendant le processus de révision des données. Les fichiers sélectionnés à partir de ces packages de données peuvent être envoyés à votre sujet de données pour terminer leur demande.

## <a name="understanding-reports"></a>Présentation des rapports

Une fois que vous avez sélectionné **Terminer la révision** dans l’étape **De révision des données** de la demande de droits d’objet, les rapports finaux de la demande commencent à être générés automatiquement. Sous l’onglet **Rapports** de la page détails des demandes de droits d’objet, la colonne **État** indique quand la génération du rapport est **en cours** et quand un rapport est **prêt à être téléchargé**. La création des rapports peut prendre jusqu’à 30 minutes.

Les rapports sont divisés en deux sections :
1. **Rapports pour la personne concernée** : ces rapports contiennent des informations qui peuvent être retournées à la personne concernée dans le cadre de l’exécution de la demande. C’est là que vous trouverez le **package de données** contenant les fichiers à envoyer à la personne concernée.
   > [!IMPORTANT]
   > Un package de données ne sera généré que si vous **marquez** des éléments comme Inclus pendant votre révision des données.

   > [!IMPORTANT]
   > Un package de données ne sera généré que pour **les types de demandes d’exportation** et **d’accès** . Un package de données ne sera pas généré pour une **liste balisé pour la demande de suivi** . Passez en revue les détails sur les [types de demandes de droits d’objet](subject-rights-requests-create.md#request-types).

2. **Rapports à des fins d’utilisation interne** : ces rapports concernent les enregistrements internes de votre organisation liés à la demande de droits d’objet. Ils incluent un journal d’audit et une liste de tous les fichiers auxquels vous avez appliqué des balises pendant la révision des données afin de suivre ou de prendre des mesures supplémentaires.

> [!NOTE]
> Lorsque des rapports sont générés, l’organisation termine la demande en envoyant les rapports appropriés de manière sécurisée à la personne concernée afin de répondre à la demande de droits de l’objet. Si la personne concernée a demandé la suppression de ses données, il incombe à l’organisation d’identifier les éléments à supprimer et d’effectuer la suppression.

## <a name="data-package"></a>Package de données

Le package de données de demande de droits d’objet contient des éléments marqués comme **Include** pendant la phase de révision des données du processus. Le package de données est généré sous forme de fichier zip. Lorsqu’il est prêt à être téléchargé, sélectionnez la ligne du rapport sous l’onglet **Rapports** de la page de détails de la demande de droits d’objet. Un panneau volant s’ouvre avec un bouton permettant de **télécharger** le rapport. Les instructions suivantes sur les actions **à suivre** dans le panneau volant fournissent une référence rapide pour savoir comment utiliser le contenu.

Lorsque vous êtes prêt à télécharger le package de données, **sélectionnez Télécharger**, recherchez votre téléchargement, puis ouvrez le fichier zip téléchargé.

### <a name="contents-of-the-data-package"></a>Contenu du package de données

Le fichier zip du package de données contient les éléments suivants :

- Un dossier nommé **Azure** : ce dossier contient les éléments clés de votre sujet de données. Consultez l’explication détaillée ci-dessous.
- Fichiers en dehors du dossier **Azure** : il peut s’agir de deux feuilles de calcul nommées **Résultats** et **Résumé**. Ces fichiers en dehors du dossier Azure sont fournis pour référence et doivent être utilisés principalement par les administrateurs de votre organisation.

Lorsque Priva identifie et récupère des fichiers pour une demande de droits d’objet, les fichiers qu’il exporte dans ce processus sont renommés à l’aide d’identificateurs uniques pour protéger les données personnelles. Vous pouvez référencer les noms uniques avec les noms de fichiers d’origine à l’aide du fichier **Export_load_file.csv** . Étant donné que les noms de fichiers d’origine peuvent inclure des informations sensibles, vous devez suivre vos stratégies qui s’appliquent à ces informations.

> [!NOTE]
> Nous vous recommandons d’examiner attentivement le contenu de ce dossier et d’envoyer uniquement les fichiers nécessaires à votre sujet de données. Vous devez évaluer votre réponse pour vous assurer qu’elle est adaptée aux exigences de la loi applicable.

### <a name="azure-folder-contents"></a>Contenu du dossier Azure

Ouvrez le dossier **Azure** , puis ouvrez le fichier **AEDExport.zip** , qui contient un autre dossier de fichiers avec un nom long composé de chiffres et de lettres. Ouvrez le dossier avec le nom long pour afficher le contenu décrit ci-dessous :

- **Extracted_text_files** dossier : contient du texte extrait des fichiers natifs (lorsque cela est pris en charge).
- **Dossier NativeFiles** : contient tous les éléments marqués lors de la révision des données comme **Inclus**, dans leur format de fichier natif. Chaque élément de ce dossier reçoit un nom de fichier unique pour protéger les données personnelles. Vous pouvez faire référence à ces noms uniques avec leur nom de fichier d’origine à l’aide du fichier Export_load_file.csv, expliqué ci-dessous.
  - Les fichiers qui ont été rédigés à l’aide de la fonction **Annotate** pendant le processus de révision des données se trouvent dans le dossier **NativeFiles** et ont le suffixe « _burn.pdf ».
- **Export_load_file.csv** fichier : contient les noms de fichiers d’origine afin que vous puissiez les référencer avec les noms de fichiers uniques fournis dans le dossier NativeFiles.
- **Fichier texte récapitulatif** : fournit un résumé des types de fichiers dans le package de données, du nombre de fichiers et de leur taille.

##### <a name="what-to-do-with-the-folder-contents"></a>Que faire avec le contenu du dossier

Ouvrez le dossier **Azure** et les fichiers zip comme expliqué ci-dessus. Votre tâche suivante consiste à passer en revue les éléments, à déterminer ce qu’il faut envoyer à la personne concernée et à modifier le contenu du fichier zip si nécessaire.

Par exemple, pour une demande d’exportation où la personne concernée souhaite recevoir une copie de tous les éléments contenant leurs données personnelles détenues par l’organisation, vous devez examiner attentivement les éléments du dossier **NativeFiles** et supprimer tout élément que vous ne souhaitez pas renvoyer à la personne concernée.

Pour une demande d’accès où la personne concernée souhaite recevoir un résumé de toutes ses informations personnelles détenues par l’organisation, vous devez vous concentrer sur le fichier texte **résumé** .

Modifiez le fichier zip pour supprimer tout contenu que vous ne souhaitez pas inclure dans le package final. Une fois l’opération terminée, envoyez le fichier zip de manière sécurisée à la personne concernée qui a effectué la demande de droits d’objet.

## <a name="audit-log"></a>Journal d’audit

Le journal d’audit est un fichier CSV qui fournit un enregistrement de la progression des étapes pour chaque demande de droits d’objet. Il répertorie chaque étape du processus, ainsi que la date et l’heure terminées, ainsi que le nom d’utilisateur de la personne qui a effectué l’étape.

## <a name="tagged-files-reports"></a>Rapports de fichiers balisés

Les rapports **étiquetés en tant que fichiers étiquetés comme... sont des** fichiers CSV qui répertorient les éléments de contenu auxquels les balises ont été appliquées pendant le processus de révision des données. Les balises sont utilisées pour marquer les éléments de contenu pour une attention ou une action supplémentaire de l’organisation. En savoir plus sur [les paramètres des balises](priva-settings.md#data-review-tags).

## <a name="retention-periods-for-reports-and-data"></a>Périodes de rétention pour les rapports et les données

Les rapports générés par les demandes de droits d’objet et les données associées, telles que les fichiers annotés enregistrés dans Azure, sont stockés pendant une durée spécifiée. La période de rétention par défaut est de 30 jours à partir de la date à laquelle une demande de droits d’objet est fermée.

La période de rétention des données est définie dans Priva **Paramètres** et s’applique à toutes les demandes de droits de l’objet. Pour afficher ou modifier votre période de rétention des données, suivez les étapes ci-dessous :

1. N’importe où dans Demandes de droits des personnes concernées Priva, sélectionnez **Paramètres** (l’icône d’engrenage) dans le coin supérieur droit de votre écran.
2. Sélectionnez **les périodes de rétention des données** dans le volet de navigation gauche.
3. Dans le menu déroulant **Données collectées et rapports** , sélectionnez 30 jours ou 90 jours comme période de rétention.
4. Sélectionnez **Enregistrer** pour enregistrer vos paramètres.

Veillez à vérifier que les périodes de rétention des données que vous avez choisies sont conformes aux stratégies et obligations légales de votre organisation.

## <a name="close-the-request"></a>Fermer la demande

Une fois que vous avez effectué toutes les actions nécessaires liées à la demande de droits d’objet, marquez la demande comme fermée en sélectionnant **Fermer la demande** dans le coin supérieur droit de la page de détails de la demande. Une demande fermée signifie qu’elle n’est plus active et indique qu’aucun travail supplémentaire n’est nécessaire pour répondre à la demande d’origine de la personne concernée à votre organisation.

Les demandes fermées ne peuvent pas être rouvertes, mais vous pouvez revenir à la demande pour afficher les détails et les notes de la demande. Les rapports de la demande sont conservés en fonction de la [période de rétention](#retention-periods-for-reports-and-data) établie.

## <a name="legal-disclaimer"></a>Exclusion de responsabilité légale

[Microsoft Priva exclusion de responsabilité légale](priva-disclaimer.md)
