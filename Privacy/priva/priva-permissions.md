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
description: Découvrez comment configurer des autorisations Microsoft Priva et attribuer des utilisateurs à des groupes de rôles.
ms.openlocfilehash: bcc2e108f10e427e55034621f2f8b5c40e6d9184
ms.sourcegitcommit: f145dff5e387a8e26db2f3a2c7de125978fbacc9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/28/2022
ms.locfileid: "62248972"
---
# <a name="set-user-permissions-and-assign-roles-in-microsoft-priva"></a>Définir des autorisations utilisateur et attribuer des rôles dans Microsoft Priva

Pour accorder aux membres de votre organisation les autorisations d’utiliser Microsoft Priva, affectez-les aux groupes de rôles appropriés dans le Centre de conformité Microsoft 365.

> [!NOTE]
> La plupart des rôles Priva sont actuellement désignés comme « gestion de la confidentialité ». Pour obtenir une liste complète, voir ci-dessous. Les rôles spécifiques à Priva n’apparaissent pas dans Azure Active Directory.

## <a name="sign-in-and-set-permissions"></a>Se connectez et définissez des autorisations

1. Go to the [Centre de conformité Microsoft 365](https://compliance.microsoft.com/) and select **Permissions** in the left navigation.  
2. Sous la **dropdown du Centre de** conformité, sélectionnez **Rôles**. La liste complète des groupes de rôles s’affiche.
3. Recherchez le groupe de rôles auquel vous souhaitez ajouter un ou plusieurs utilisateurs, puis cochez la case à gauche du nom du groupe.
4. Dans le volet volant de ce groupe, sélectionnez **Modifier** sous **l’en-tête Membres** .  
5. **Sélectionnez Choisir les membres**. Une autre fenêtre volante s’affiche.
6. **Sélectionnez + Ajouter** pour choisir un ou plusieurs utilisateurs à ajouter au groupe.  
7. Cochez la case en regard des noms que vous souhaitez ajouter, puis sélectionnez le **bouton Ajouter en** bas.  
8. Lorsque vous avez terminé d’affecter des utilisateurs, sélectionnez **Terminé**, puis **Enregistrer**, puis **Fermer**.

## <a name="learn-more-about-role-groups-and-roles"></a>En savoir plus sur les groupes de rôles et les rôles

Selon la structure de votre équipe, vous avez la possibilité d’affecter des utilisateurs à des groupes de rôles spécifiques pour gérer différents ensembles de fonctionnalités Priva. Les membres doivent être affectés à des groupes de rôles en fonction des tâches qu’ils doivent accomplir et du niveau d’accès approprié aux fichiers. Chaque groupe de rôles comprend un ou plusieurs rôles. Ces rôles peuvent concerner des tâches Priva spécifiques ou des fonctions clés qui sont activées ou restreintes pour les membres de ce groupe. Par conséquent, différents utilisateurs peuvent avoir différents niveaux de visibilité et d’accès à certaines fonctionnalités priva.

Les groupes de rôles peuvent être personnalisés si nécessaire. Pour éviter toute perte accidentelle d’accès, nous vous recommandons de créer une copie du groupe de rôles existant que vous souhaitez personnaliser, d’attribuer un nom identifiable à la copie, d’apporter et de vérifier vos modifications au nouveau groupe et d’y affecter des personnes selon le cas.

## <a name="privacy-management-role-group"></a>Groupe de rôles Gestion de la confidentialité

Ce groupe contient tous les rôles d’autorisation Priva dans un seul groupe. Ce groupe de rôles peut être adapté aux organisations où la même personne peut effectuer toutes les tâches. L’appartenance à ce groupe de rôles accordera à ce compte un accès total à toutes les fonctionnalités de Priva pour lesquelles vous disposez d’une licence.

Nous vous recommandons de vous assurer qu’il existe toujours au moins un membre actif de ce groupe.

Les rôles sont les suivants :

- Gestion des cas  
- Visionneuse de contenu de classification des données  
- Visionneuse de listes de classification des données  
- Administrateur de la gestion de la confidentialité  
- Analyse de la gestion de la confidentialité  
- Examen de la gestion de la confidentialité  
- Contribution permanente à la gestion de la confidentialité  
- Contribution temporaire à la gestion de la confidentialité  
- Visionneuse de la gestion de la confidentialité  
- Administrateur des demandes de droits de l’objet  
- View-Only Case

## <a name="privacy-management-administrators-role-group"></a>Groupe de rôles Administrateurs de la gestion de la confidentialité

Les membres de ce groupe de rôles ont un large accès aux fonctions Priva, notamment la création, la lecture, la mise à jour et la suppression des stratégies de gestion des risques de confidentialité, des demandes de droits de l’objet, des autorisations et des paramètres.

Les rôles sont les suivants :

- Gestion des cas  
- Administrateur de la gestion de la confidentialité  
- View-Only Case

## <a name="privacy-management-analysts-role-group"></a>Groupe de rôles Analystes de la gestion de la confidentialité

Les membres de ce groupe de rôles agissent en tant qu’analystes de cas. Ils peuvent examiner les correspondances de stratégie, afficher les métadonnées des fichiers et prendre des mesures correctives. Ce groupe ne peut pas accéder aux fichiers complets via l’Explorateur de contenu.

Les rôles sont les suivants :

- Gestion des cas  
- Visionneuse de listes de classification des données  
- Analyse de la gestion de la confidentialité  
- View-Only Case

### <a name="privacy-management-investigators-role-group"></a>Groupe de rôles Enquêteurs de la gestion de la confidentialité

Les membres de ce groupe agissent en tant qu’enquêteurs de données. Ils peuvent examiner les correspondances de stratégie, afficher le contenu du fichier associé et prendre des mesures correctives. Ce groupe peut accéder aux fichiers via l’Explorateur de contenu.

Les rôles sont les suivants :

- Gestion des cas  
- Visionneuse de contenu de classification des données  
- Visionneuse de listes de classification des données  
- Examen de la gestion de la confidentialité  
- View-Only Case

## <a name="privacy-management-viewer-role-group"></a>Groupe de rôles Visionneuse de gestion de la confidentialité

Les membres de ce groupe peuvent afficher des informations analytiques dans Priva, telles que la vue d’ensemble, le profil de données et les rapports de demande d’objet.

Les rôles sont les suivants :

- Visionneuse de la gestion de la confidentialité

## <a name="subject-rights-request-administrators-role-group"></a>Groupe de rôles Administrateurs des demandes de droits de l’objet

Les membres de ce groupe ont un accès total pour administrer et créer des demandes de droits d’objet.

Les rôles sont les suivants :

- Administrateur des demandes de droits de l’objet

## <a name="privacy-management-contributors-role-group"></a>Groupe de rôles Contributeurs à la gestion de la confidentialité

Les membres de ce groupe ont accès aux demandes de droits d’objet pour lesquelles ils ont été ajoutés en tant que collaborateur.  

Les rôles sont les suivants :

- Contribution temporaire à la gestion de la confidentialité  
- Contribution permanente à la gestion de la confidentialité

## <a name="legal-disclaimer"></a>Clause d’exclusion de responsabilité légale

[Clause d’exclusion de responsabilité légale Microsoft Priva](priva-disclaimer.md)