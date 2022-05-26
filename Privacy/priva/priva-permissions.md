---
title: Définir des autorisations utilisateur et attribuer des rôles dans Microsoft Priva
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
- M365-priva-subject-rights-requests
search.appverid:
- MOE150
- MET150
description: Découvrez comment configurer Microsoft Priva autorisations et affecter des utilisateurs à des groupes de rôles.
ms.openlocfilehash: eca08327e2db909475dbf4c072b8f6843de3d57b
ms.sourcegitcommit: 3c27ecf7c86c8a3db38cae8819fc090eed192b4f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/25/2022
ms.locfileid: "65678221"
---
# <a name="set-user-permissions-and-assign-roles-in-microsoft-priva"></a>Définir des autorisations utilisateur et attribuer des rôles dans Microsoft Priva

Pour autoriser les membres de votre organisation à utiliser Microsoft Priva, affectez-les aux groupes de rôles appropriés dans le portail de conformité Microsoft Purview.

> [!NOTE]
> La plupart des rôles Priva sont actuellement désignés comme « gestion de la confidentialité ». Consultez la liste complète ci-dessous. Les rôles spécifiques à Priva n’apparaissent pas dans Azure Active Directory.

## <a name="sign-in-and-set-permissions"></a>Se connecter et définir des autorisations

1. Accédez au [portail de conformité Microsoft Purview](https://compliance.microsoft.com/) et sélectionnez **Autorisations** dans le volet de navigation de gauche.  
2. Dans la liste **déroulante Microsoft Purview solutions**, sélectionnez **Rôles**. La liste complète des groupes de rôles s’affiche.
3. Recherchez le groupe de rôles auquel vous souhaitez ajouter un ou plusieurs utilisateurs (voir les descriptions de groupe de rôles ci-dessous) et cochez la case à gauche du nom du groupe.
4. Dans le volet volant de ce groupe, sous l’en-tête **Membres** , **sélectionnez Modifier**.  
5. Dans le volet de menu volant, **sélectionnez Choisir des membres** dans le volet de navigation gauche. Une autre fenêtre de menu volant s’affiche.
6. Sélectionnez **+ Ajouter** pour choisir un ou plusieurs utilisateurs à ajouter au groupe.  
7. Cochez la case en regard des noms que vous souhaitez ajouter, puis sélectionnez le bouton **Ajouter** en bas.  
8. Lorsque vous avez terminé d’affecter des utilisateurs, sélectionnez **Terminé**, puis **Enregistrer**, puis **Fermer**.

## <a name="learn-more-about-role-groups-and-roles"></a>En savoir plus sur les groupes de rôles et les rôles

Selon la structure de votre équipe, vous avez des options pour affecter des utilisateurs à des groupes de rôles spécifiques afin de gérer différents ensembles de fonctionnalités Priva. Les membres doivent être affectés à des groupes de rôles en fonction des tâches qu’ils doivent accomplir et du niveau d’accès aux fichiers approprié. Chaque groupe de rôles comprend un ou plusieurs rôles. Ces rôles peuvent se rapporter à des tâches Priva spécifiques ou à des fonctions clés activées ou restreintes pour les membres de ce groupe. Différents utilisateurs peuvent donc avoir différents niveaux de visibilité et d’accès à certaines fonctionnalités Priva.

Les groupes de rôles peuvent être personnalisés si nécessaire. Pour éviter toute perte accidentelle d’accès, nous vous recommandons de créer une copie du groupe de rôles existant que vous souhaitez personnaliser, d’attribuer un nom identifiable à la copie, d’apporter et de vérifier vos modifications au nouveau groupe et d’y affecter des personnes selon les besoins.

## <a name="privacy-management-role-group"></a>Groupe de rôles Gestion de la confidentialité

Ce groupe contient tous les rôles d’autorisation Priva dans un seul groupe. Ce groupe de rôles peut être adapté aux organisations où la même personne peut effectuer toutes les tâches. La fourniture de l’appartenance à ce groupe de rôles accordera à ce compte un accès complet à toutes les fonctionnalités de Priva pour lesquelles vous détenez une licence.

Nous vous recommandons de vous assurer qu’il y a toujours au moins un membre actif de ce groupe.

Les rôles sont les suivants :

- Gestion des cas  
- Visionneuse de contenu de classification des données  
- Visionneuse de liste de classification des données  
- Administration de gestion de la confidentialité  
- Analyse de la gestion de la confidentialité  
- Enquête sur la gestion de la confidentialité  
- Contribution permanente à la gestion de la confidentialité  
- Contribution temporaire à la gestion de la confidentialité  
- Visionneuse de gestion de la confidentialité  
- Demande de droits de sujet Administration  
- cas View-Only

## <a name="privacy-management-administrators-role-group"></a>Groupe de rôles Administrateurs de la gestion de la confidentialité

Les membres de ce groupe de rôles ont un large accès aux fonctions Priva, notamment la création, la lecture, la mise à jour et la suppression de stratégies de gestion des risques de confidentialité, de demandes de droits d’objet, d’autorisations et de paramètres.

Les rôles sont les suivants :

- Gestion des cas  
- Administration de gestion de la confidentialité  
- cas View-Only

## <a name="privacy-management-analysts-role-group"></a>Groupe de rôles Analystes de gestion de la confidentialité

Les membres de ce groupe de rôles agissent en tant qu’analystes de cas. Ils peuvent examiner les correspondances de stratégie, afficher les métadonnées de fichier et prendre des mesures de correction. Ce groupe ne peut pas accéder aux fichiers complets via l’Explorateur de contenu.

Les rôles sont les suivants :

- Gestion des cas  
- Visionneuse de liste de classification des données  
- Analyse de la gestion de la confidentialité  
- cas View-Only

### <a name="privacy-management-investigators-role-group"></a>Groupe de rôles Investigateurs de gestion de la confidentialité

Les membres de ce groupe agissent en tant qu’enquêteurs de données. Ils peuvent examiner les correspondances de stratégie, afficher le contenu du fichier associé et prendre des mesures de correction. Ce groupe peut accéder aux fichiers via l’Explorateur de contenu.

Les rôles sont les suivants :

- Gestion des cas  
- Visionneuse de contenu de classification des données  
- Visionneuse de liste de classification des données  
- Enquête sur la gestion de la confidentialité  
- cas View-Only

## <a name="privacy-management-viewer-role-group"></a>Groupe de rôles Visionneuse de gestion de la confidentialité

Les membres de ce groupe peuvent afficher des informations analytiques dans Priva, telles que la vue d’ensemble, le profil de données et les rapports de demande d’objet.

Les rôles sont les suivants :

- Visionneuse de gestion de la confidentialité

## <a name="subject-rights-request-administrators-role-group"></a>Groupe de rôles Administrateurs de demande de droits d’objet

Les membres de ce groupe ont un accès complet pour administrer et créer des demandes de droits d’objet.

Les rôles sont les suivants :

- Demande de droits de sujet Administration

## <a name="privacy-management-contributors-role-group"></a>Groupe de rôle Contributeurs à la gestion de la confidentialité

Les membres de ce groupe ont accès aux demandes de droits d’objet pour lesquelles ils ont été ajoutés en tant que collaborateurs.  

Les rôles sont les suivants :

- Contribution temporaire à la gestion de la confidentialité  
- Contribution permanente à la gestion de la confidentialité

## <a name="legal-disclaimer"></a>Exclusion de responsabilité légale

[Microsoft Priva exclusion de responsabilité légale](priva-disclaimer.md)