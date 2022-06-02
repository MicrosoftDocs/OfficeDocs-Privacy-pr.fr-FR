---
title: Intégrer à Microsoft API Graph et Power Automate
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
description: Découvrez comment étendre Demandes de droits des personnes concernées Priva fonctionnalités en intégrant Microsoft API Graph et Power Automate.
ms.openlocfilehash: e4fcad2067ece3d1a6338e6d4891c59d91205a33
ms.sourcegitcommit: 9315064bf5bb9e889318e61ec5f082f36c815e1e
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/02/2022
ms.locfileid: "65851639"
---
# <a name="integrate-and-extend-through-microsoft-graph-api-and-power-automate"></a>Intégrer et étendre via Microsoft API Graph et Power Automate

Vous pouvez intégrer Demandes de droits des personnes concernées Priva à vos processus et outils métier existants à l’aide de l’API Microsoft Graph Subject Rights Request. Vous pouvez également étendre les fonctionnalités d’automatisation des demandes de droits d’objet à l’aide de flux de Power Automate intégrés pour des tâches telles que la définition de rappels de calendrier et la création de cas dans ServiceNow.

## <a name="microsoft-graph-subject-rights-requests-api"></a>API Microsoft Graph Subject Rights Requests

L’API Microsoft 365 Demande de droits d’objet offre un moyen simple mais puissant d’introduire l’automatisation dans votre stratégie de droits de sujet existante. Lorsqu’un individu demande des informations à votre organisation, nos API vous permettent de créer ces demandes dans Microsoft 365 en fonction des critères de cette demande. Vous pouvez créer la demande de droits d’objet dans Microsoft 365, suivre sa progression et accuser réception lorsque le traitement de la demande est terminé et que le contenu est prêt à être récupéré.

Nos API sont accessibles à tous pour rendre leurs solutions plus extensibles, telles que les éditeurs de logiciels indépendants, les partenaires qui cherchent à prendre en charge Microsoft 365 dans leurs solutions et les organisations qui cherchent à utiliser les API avec leurs applications métier.

Consultez la documentation complète sur [l’API Utiliser la demande de droits d’objet Microsoft Graph](/graph/api/resources/subjectrightsrequest-subjectrightsrequestapioverview).

## <a name="power-automate-templates-for-subject-rights-requests"></a>Power Automate modèles pour les demandes de droits d’objet

Microsoft Power Automate est un service de flux de travail qui automatise les actions entre les applications et les services. Les demandes de droits d’objet incluent des modèles de Power Automate intégrés pour aider les utilisateurs à gérer les demandes de droits d’objet. Les utilisateurs peuvent configurer des flux d’automatisation pour des processus tels que la création de tickets dans ServiceNow et l’ajout de rappels de calendrier sur les dates d’échéance. Pour en savoir plus sur Power Automate, consultez la [documentation Power Automate](/power-automate/getting-started).

Si vous avez acheté un abonnement Subject Rights Requests, vous n’avez pas besoin d’une licence Power Automate distincte pour utiliser les modèles de Power Automate recommandés. Ces modèles peuvent être personnalisés pour prendre en charge votre organisation et couvrir les principaux scénarios de demande de droits d’objet. Toutefois, vous pouvez avoir besoin de licences supplémentaires pour utiliser des fonctionnalités premium Power Automate dans ces modèles ou pour créer votre propre modèle.

### <a name="available-templates"></a>Modèles disponibles

- **Créez un enregistrement pour Priva cas de gestion de la confidentialité dans ServiceNow** : ce modèle est destiné aux organisations qui souhaitent utiliser leur solution ServiceNow pour suivre les cas de demande de droits d’objet. Vous serez invité à entrer les détails de votre instance ServiceNow, y compris un compte pour vous connecter à ServiceNow. Ce compte doit avoir la possibilité de créer un incident dans ServiceNow et de renseigner les détails de l’incident. Une fois connectés à votre instance, les administrateurs des demandes de droits d’objet peuvent créer un enregistrement pour le cas dans ServiceNow et, si nécessaire, peuvent personnaliser ce que le modèle remplira dans les champs sélectionnés. Pour plus d’informations sur le connecteur, consultez la [documentation du connecteur ServiceNow](/connectors/service-now/).

- **Ajoutez un rappel de calendrier pour effectuer le suivi d’un Priva cas de gestion de la confidentialité** : ce modèle permet de définir des rappels de date d’échéance dans votre calendrier Outlook pour les demandes de droits d’objet. L’outil remplira certains détails pour vous à partir des propriétés de la demande, telles que le nom de la demande et sa date d’échéance. Vous pouvez ajouter des détails descriptifs, spécifier des destinataires et ajuster d’autres paramètres avancés.

- **Obtenir des fichiers par balise pour une demande de droits d’objet Priva** : ce modèle vous permet de rechercher des fichiers pour votre demande de droits d’objet qui ont reçu une balise spécifique. Vous pouvez modifier le flux pour effectuer des actions personnalisées ou afficher la liste des fichiers retournés à utiliser pour les processus ou outils internes.

### <a name="create-a-new-power-automate-flow-from-a-template"></a>Créer un flux de Power Automate à partir d’un modèle

1. Dans le [portail de conformité Microsoft Purview](https://compliance.microsoft.com/), sélectionnez **Demandes de droits des personnes concernées Priva** dans le volet de navigation gauche.

2. Recherchez la demande de droits d’objet sur laquelle vous souhaitez travailler et sélectionnez-la dans la liste pour ouvrir sa page de détails.

3. Dans le coin supérieur droit, sélectionnez **Automatiser**, puis **Sélectionnez Gérer Power Automate flux** pour ouvrir le volet de menu volant des flux.

4. Sélectionnez **Nouveau** et choisissez le modèle que vous souhaitez utiliser parmi les options disponibles. À partir de là, suivez les invites pour personnaliser et ajouter des étapes pour terminer la génération du flux. Les options varient en fonction du modèle que vous utilisez (voir les types de modèles ci-dessous).

5. Lorsque vous avez terminé, sélectionnez **Enregistrer**.

Après avoir enregistré une instance du modèle, vous devez l’exécuter à partir de la page de détails de la demande afin que l’instance de flux ait le contexte et l’ID appropriés. Ouvrez la demande, revenez au menu **Automatiser** , sélectionnez le modèle, puis sélectionnez **Exécuter le flux**. Vous pouvez voir vos activités passées en sélectionnant **Afficher l’activité d’exécution de flux**.

### <a name="share-a-power-automate-flow"></a>Partager un flux de Power Automate

Le partage d’un flux Power Automate vous permet d’ajouter un autre propriétaire et de le modifier, de le mettre à jour et de le supprimer. Tous les propriétaires peuvent accéder à l’historique des exécutions et ajouter ou supprimer d’autres propriétaires. 

Pour partager un flux, ouvrez la demande de droits d’objet avec laquelle vous souhaitez travailler, sélectionnez **Automatiser**, puis **sélectionnez Gérer Power Automate flux**. Dans ce volet, vous pouvez sélectionner un flux existant, puis utiliser l’option **Partager** pour ajouter un utilisateur ou un groupe.

Ce volet vous donne également la possibilité de gérer les connexions incorporées aux services utilisés dans le flux Power Automate. La modification de ces paramètres peut affecter votre capacité à exécuter le flux.

### <a name="edit-or-delete-power-automate-flow"></a>Modifier ou supprimer Power Automate flux

Pour ajuster les détails d’un flux Power Automate, sélectionnez **Automatiser** dans le coin supérieur droit de la page de détails d’une demande, puis **sélectionnez Gérer Power Automate flux**.

Dans le volet **Power Automate flux**, sélectionnez le flux que vous souhaitez modifier, puis **sélectionnez Modifier** dans la barre de commandes pour modifier ou ajouter des étapes. Lorsque vous avez terminé, **sélectionnez Enregistrer**.

Pour supprimer un flux, sélectionnez-le dans la liste du volet **Power Automate flux**, puis **sélectionnez Supprimer** dans la barre de commandes. Le flux sera supprimé pour tous les propriétaires et désinstallé pour tous les utilisateurs. Les instances de flux précédentes continueront à s’exécuter pour éviter la perte de données. Vous serez invité à confirmer avant la fin de la suppression.

## <a name="legal-disclaimer"></a>Exclusion de responsabilité légale

[Microsoft Priva exclusion de responsabilité légale](priva-disclaimer.md)
