---
title: 'Automatiser les tâches dans les demandes de droits d’objet '
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
description: Découvrez comment utiliser Microsoft Power Automate pour vous aider à automatiser les tâches essentielles pour les demandes de droits d’objet dans Priva.
ms.openlocfilehash: ec9edde16b60c2326ca899e587dfe5dc7a1e32f5
ms.sourcegitcommit: 09ecdaded9a9f8f79587f2acb978dc53b83e5c01
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/19/2022
ms.locfileid: "64930495"
---
# <a name="automate-tasks-in-subject-rights-requests"></a>Automatiser les tâches dans les demandes de droits d’objet 

Microsoft Power Automate est un service de flux de travail qui automatise les actions entre les applications et les services. Lorsque vous activez Power Automate flux pour les demandes de droits d’objet Microsoft Priva, vous pouvez automatiser des tâches importantes pour les cas et les utilisateurs, telles que la création de tickets dans ServiceNow ou l’ajout de rappels de calendrier sur les dates d’échéance. Pour en savoir plus sur Power Automate, visitez leur [site de documentation](/power-automate/getting-started).

Les clients disposant d’abonnements Subject Rights Requests n’ont pas besoin d’une autre licence Power Automate pour utiliser les modèles de Power Automate recommandés pour Priva. Ces modèles peuvent être personnalisés pour prendre en charge votre organisation et couvrir les principaux scénarios de demande de droits d’objet. Si vous choisissez d’utiliser des fonctionnalités premium Power Automate dans ces modèles, créez un modèle personnalisé à l’aide du connecteur de conformité Microsoft 365 ou utilisez des modèles Power Automate pour d’autres domaines de conformité dans Microsoft 365, vous aurez peut-être besoin de davantage de licences Power Automate.

## <a name="create-a-new-power-automate-flow-from-a-template"></a>Créer un flux de Power Automate à partir d’un modèle

1. Dans le [portail de conformité Microsoft Purview](https://compliance.microsoft.com/), accédez à la section Priva de la navigation et sélectionnez **Priva Subject Rights Requests**.
1. Ouvrez la demande de droits d’objet avec laquelle vous souhaitez travailler dans la liste, puis sélectionnez **Automatiser**, puis **Gérez Power Automate flux**. Le volet de menu volant Flux s’ouvre.
1. Utilisez l’option **Nouveau** et choisissez le modèle que vous souhaitez utiliser parmi les options disponibles. À partir de là, suivez les invites de l’Assistant pour terminer la configuration. Les options varient en fonction de votre type de modèle.

Après avoir enregistré une instance du modèle, vous devez l’exécuter à partir de la page de détails de la demande de droits d’objet afin que l’instance de flux ait le contexte et l’ID appropriés. Ouvrez la demande, revenez au menu **Automatiser** , sélectionnez le modèle, puis sélectionnez **Exécuter le flux**. Vous pouvez voir vos activités passées en sélectionnant **Afficher l’activité d’exécution de flux**.

### <a name="power-automate-templates-in-priva"></a>modèles Power Automate dans Priva

- **Créer un enregistrement pour le cas de gestion de la confidentialité dans ServiceNow** : ce modèle est destiné aux organisations qui souhaitent utiliser leur solution ServiceNow pour suivre les cas de demande de droits d’objet. Vous serez invité à entrer les détails de votre instance ServiceNow, y compris un compte pour vous connecter à ServiceNow. Ce compte doit avoir la possibilité de créer un incident dans ServiceNow et de renseigner les détails de l’incident. Une fois connectés à votre instance, les administrateurs des demandes de droits d’objet peuvent créer un enregistrement pour le cas dans ServiceNow et, si nécessaire, peuvent personnaliser ce que le modèle remplira dans les champs sélectionnés. Pour plus d’informations sur le connecteur, consultez la [page de référence du connecteur ServiceNow](/connectors/service-now/).
- **Créez un rappel de calendrier** : ce modèle permet de définir des rappels de date d’échéance dans votre calendrier Outlook pour les demandes de droits d’objet. L’outil remplira certains détails pour vous à partir des propriétés de la demande, telles que le nom de la demande et sa date d’échéance. Vous pouvez ajouter des détails descriptifs, spécifier des destinataires et ajuster d’autres paramètres avancés.
- **Obtenir des fichiers par balise pour une demande de droits d’objet** : ce modèle vous permet de rechercher des fichiers pour votre demande de droits d’objet qui ont reçu une balise spécifique. Vous pouvez modifier le flux pour effectuer des actions personnalisées ou afficher la liste des fichiers retournés à exploiter pour les processus ou outils internes.

## <a name="share-a-power-automate-flow"></a>Partager un flux de Power Automate

En partageant un flux Power Automate, vous pouvez ajouter un autre propriétaire et lui permettre de modifier, mettre à jour et supprimer le flux. Tous les propriétaires peuvent également accéder à l’historique des exécutions et ajouter ou supprimer d’autres propriétaires. Pour partager un flux, ouvrez la demande de droits d’objet avec laquelle vous souhaitez travailler, sélectionnez **Automatiser**, puis **sélectionnez Gérer Power Automate flux**. Dans ce volet, vous pouvez sélectionner un flux existant, puis utiliser l’option Partager pour ajouter un utilisateur ou un groupe.

Ce volet vous donne également la possibilité de gérer les connexions incorporées aux services utilisés dans le flux Power Automate. La modification de ces paramètres peut affecter votre capacité à exécuter le flux.

## <a name="edit-or-delete-power-automate-flow"></a>Modifier ou supprimer Power Automate flux

Pour ajuster les détails d’un flux de Power Automate, ouvrez la demande de droits d’objet, sélectionnez **Automatiser**, puis **sélectionnez Gérer Power Automate flux**. Dans ce volet, vous pouvez sélectionner un flux existant pour afficher les détails. Utilisez Modifier dans n’importe quelle section pour modifier les propriétés, puis enregistrez.

Pour supprimer entièrement le flux, utilisez l’option **Supprimer** . Il supprime le flux pour tous les propriétaires et le désinstalle pour tous les utilisateurs. Les instances de flux précédentes continueront à s’exécuter pour éviter la perte de données. Vous pouvez confirmer votre choix avant la fin de la suppression.

## <a name="legal-disclaimer"></a>Exclusion de responsabilité légale

[Exclusion de responsabilité légale de Microsoft Priva](priva-disclaimer.md)
