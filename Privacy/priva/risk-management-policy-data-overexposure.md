---
title: Stratégies de surexposition des données dans la gestion des risques liés à la confidentialité
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
search.appverid:
- MOE150
- MET150
description: Découvrez comment créer une stratégie de surexposition des données dans Gestion des risques de confidentialité Microsoft Priva identifier et sécuriser les données personnelles qui peuvent être trop accessibles.
ms.openlocfilehash: 6efb92ed5d1b79b0fc69beebd5788062b5687269
ms.sourcegitcommit: 3c83e8133a5a71f4e1d76a0b2981ab3ec9cd6602
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/13/2022
ms.locfileid: "66046678"
---
# <a name="data-overexposure-policies-in-privacy-risk-management"></a>Stratégies de surexposition des données dans la gestion des risques liés à la confidentialité

Votre organisation peut stocker du contenu à différents niveaux d’accès, y compris des zones accessibles publiquement et d’autres qui sont restreintes. Les stratégies de surexposition des données peuvent vous aider à détecter et à gérer les situations dans lesquelles les données stockées par votre organisation ne sont pas suffisamment sécurisées. Par exemple, si l’accès à un site interne est ouvert à un trop grand nombre de personnes ou si vos paramètres d’autorisation n’ont pas été conservés, les données personnelles stockées sur ce site peuvent être vulnérables à une violation. Les stratégies de surexposition des données peuvent évaluer vos données pour ces risques et vous avertir des problèmes potentiels.

Lorsqu’une correspondance de stratégie est détectée, vous pouvez envoyer des notifications par e-mail aux utilisateurs qui incluent des options de correction pour résoudre les problèmes. Pour la surexposition des données, il s’agit notamment de rendre les éléments de contenu privés, d’avertir les propriétaires de contenu ou de marquer des éléments pour une révision ultérieure.

Notre processus de configuration de stratégie facilite la définition des conditions de stratégie. Vous disposez d’un contrôle total sur le minutage des alertes et la fréquence des e-mails qui portent l’attention des utilisateurs sur les pratiques de gestion des données sécurisées.

Il existe deux façons de créer une stratégie : à partir d’un **modèle**, qui est notre option rapide « out-of-box » à l’aide des paramètres par défaut ; ou l’option **personnalisée** , qui est un processus guidé pour définir les conditions, les alertes et les notifications.

## <a name="quick-setup-use-a-template-with-default-settings"></a>Configuration rapide : utiliser un modèle avec les paramètres par défaut

La stratégie de surexposition des données par défaut évalue les données personnelles aux trois niveaux d’accès : public, externe et interne.

Procédez comme suit pour créer une stratégie de transfert de données par défaut :

1. Dans le [portail de conformité Microsoft Purview](https://compliance.microsoft.com/), recherchez Gestion des risques de confidentialité Priva dans le volet de navigation de gauche et sélectionnez **Stratégies**.

2. Sélectionnez **Créer une stratégie** dans le coin supérieur droit de l’écran, qui affiche un volet volant répertoriant toutes les options de création de stratégie.

3. Dans la zone **Surexposition des données** , sélectionnez **Créer**.

4. Un volet volant contient les détails de la stratégie. La sélection des **paramètres d’affichage** affiche les paramètres par défaut. Vous pouvez modifier les paramètres à partir d’ici, ce qui vous permet d’accéder au processus guidé décrit ci-dessous. Pour continuer à créer votre stratégie à l’aide des paramètres par défaut, entrez simplement un nom descriptif, puis **sélectionnez Créer une stratégie**.

Votre stratégie sera créée et vous la trouverez dans votre page **Polices** . Il commence en [mode test](risk-management-policies.md#testing-a-policy) pour vous permettre de surveiller ses performances avant de l’activer.

#### <a name="default-data-overexposure-policy-settings"></a>Paramètres de stratégie de surexposition des données par défaut

Une stratégie de surexposition des données créée à partir du modèle détecte :

- Lorsqu’un utilisateur fournit un accès trop large aux éléments contenant des données personnelles stockées dans le OneDrive ou le SharePoint de votre organisation. Par exemple, la stratégie détecte le partage de données personnelles des manières suivantes :
    - Par le biais d’un lien auquel toute personne du public peut accéder
    - Via un lien ou en raison d’autorisations qui permettent à tous les membres de l’organisation d’accéder à
    - Octroi de droits d’accès à des utilisateurs externes ou à des invités pour OneDrive ou SharePoint fichiers
- Types de données basés sur les [groupes de classification suivants](risk-management-policies.md#classification-groups) :
    - Règlement général de l’UE sur la protection des données (RGPD)
    - Informations d’identification personnelle des États-Unis
    - US Patriot Act
    - Loi sur la notification de violation de l’État des États-Unis
    - Us Gramm-Leach-Bliley Act (GLBA)
    - Us Health Insurance Portability and Accountability Act (HIPAA)
    - Australia Health Records Act (HRIP)
    - Australia Privacy Act
    - Informations d’identification personnelle au Japon
    - Japan Protection of Personal Information

## <a name="custom-setup-guided-policy-creation-process"></a>Configuration personnalisée : processus de création de stratégie guidée

L’option de stratégie personnalisée est un processus guidé permettant de créer une stratégie en définissant des conditions, en désignant la gravité et la fréquence des alertes et en activant les notifications par e-mail de l’utilisateur.

Effectuez les étapes ci-dessous pour créer une stratégie de surexposition des données :

1. Dans le [portail de conformité Microsoft Purview](https://compliance.microsoft.com/), recherchez Gestion des risques de confidentialité Priva dans le volet de navigation de gauche et sélectionnez **Stratégies**.

2. Sélectionnez le bouton **Créer une stratégie** en haut à droite de votre écran, qui affiche un volet volant répertoriant toutes les options de création de stratégie.

3. Dans la zone **Personnalisée** , sélectionnez **Créer**.

4. Dans la page **Nom et type** , sélectionnez le modèle de stratégie de **surexposition des données** . Entrez un nom de stratégie qui vous aidera à l’identifier facilement à partir de votre liste sur la page **Stratégies** , puis entrez une description facultative, puis sélectionnez **Suivant**.

5. Dans la page **Données à surveiller** , choisissez le type de données personnelles que votre stratégie doit surveiller. Il existe deux options :
    - **Groupes de classification** : regroupements de types d’informations sensibles utilisés pour détecter du contenu lié à des données personnelles ou à des réglementations spécifiques. Si vous sélectionnez cette option, vous devez sélectionner **+Ajouter des groupes de classification** pour choisir un ou plusieurs groupes dans la liste fournie.
    - **Types d’informations sensibles individuels** : sélectionnez cette option pour choisir parmi une liste de [types d’informations sensibles individuels](/microsoft-365/compliance/sensitive-information-type-entity-definitions).

    En savoir plus sur [le choix des données à surveiller](risk-management-policies.md#choose-data-to-monitor). Lorsque vous avez terminé de sélectionner les données à surveiller, sélectionnez **Suivant**.

6. Dans la page **Utilisateurs et groupes** , choisissez les utilisateurs de votre organisation auxquels la stratégie s’appliquera. Vous pouvez sélectionner tous les utilisateurs individuels et tous les groupes de distribution Office 365, ou vous pouvez sélectionner des utilisateurs et des groupes spécifiques. En savoir plus sur [le choix des utilisateurs et des groupes](risk-management-policies.md#choose-users-and-groups). Lorsque vous avez terminé, sélectionnez **Suivant**.

7. Dans la page **Emplacements**, sélectionnez tous les emplacements de données dans Microsoft 365 que vous souhaitez que la stratégie couvre. Choisissez parmi OneDrive comptes et sites SharePoint.

    Dans SharePoint vous pouvez désigner tous les sites ou sites spécifiques. Si vous sélectionnez **Des sites spécifiques SharePoint**, vous pouvez entrer l’URL du site dans le champ URL. Vous pouvez également sélectionner **+Choisir des sites**, puis, dans le volet volant, cochez la case à gauche du nom du site que vous souhaitez sélectionner.

    En savoir plus sur [le choix des emplacements](risk-management-policies.md#choose-locations). Lorsque vous avez terminé de sélectionner des emplacements, sélectionnez **Suivant**.

8. Dans la page **Conditions** , sélectionnez le type de condition de surexposition des données détectée par la stratégie :
    - **Public** : toute personne disposant d’un lien peut accéder au contenu.
    - **Externe** : des personnes spécifiques en dehors de l’organisation ont accès.
    - **Interne** : tous les utilisateurs de votre organisation ont accès.
    
    La sélection de plusieurs niveaux d’accès élargit l’étendue des données et peut générer des quantités significativement plus importantes d’alertes et de notifications utilisateur.

    Cochez la case en regard de vos choix, puis sélectionnez **Suivant**.

9. Dans la page Résultats, décidez s’il faut informer les utilisateurs lorsqu’ils correspondent aux conditions **définies** par la stratégie. Si vous cochez la case des notifications par e-mail, les utilisateurs reçoivent une notification par e-mail lorsque leurs actions correspondent aux conditions de stratégie. Les e-mails contiennent des instructions pour prendre des mesures de correction directement à partir de l’e-mail, ainsi qu’un lien vers la formation à la confidentialité. Vous allez désigner la fréquence des e-mails et l’URL de votre formation de confidentialité préférée.
     
    En savoir plus sur la configuration [des notifications utilisateur](risk-management-notifications.md). Lorsque vous avez terminé de sélectionner les résultats, sélectionnez **Suivant**.

10. Dans la page **Alertes** , utilisez le bouton bascule pour activer les alertes qu’un administrateur verra sur la page **Alertes** dans la section **Stratégies** de la gestion des risques de confidentialité. Vous allez indiquer la fréquence à laquelle les alertes sont générées, les seuils de correspondance avant la génération des alertes et la gravité des alertes. En savoir plus sur [la définition d’alertes pour les correspondances de stratégie](risk-management-policies.md#set-alerts). Lorsque vous avez terminé, sélectionnez **Suivant**.

11. Dans la page **Mode** , déterminez si vous souhaitez ou non exécuter votre stratégie en mode test lorsque vous la créez pour la première fois, ce qui signifie qu’aucune alerte ou notification n’est envoyée. Pour conserver votre stratégie en mode test, ce que nous vous recommandons, sélectionnez le commutateur bascule vers la position **Activé** . En savoir plus sur le [test d’une stratégie](risk-management-policies.md#testing-a-policy).

> [!NOTE]
> Si vous **basculez l’option Exécuter en mode test** vers la position **Désactivée** , *votre stratégie s’active* lorsque vous avez terminé de la créer. Cela signifie que toutes les alertes ou notifications utilisateur que vous avez configurées commencent à générer une fois qu’une correspondance est détectée.

12. Dans la page **Terminer** , passez en revue vos choix. Sélectionnez **Modifier** sous l’une des sections pour ajuster les paramètres. Lorsque vous êtes satisfait des paramètres de votre stratégie, sélectionnez **Envoyer** pour créer la stratégie.

Après quelques secondes, vous verrez une confirmation que la stratégie a été créée. Sélectionnez **Terminé** dans la page de confirmation, qui vous amène à la page **Stratégies** où vous verrez la nouvelle stratégie en haut du tableau.

## <a name="next-steps"></a>Étapes suivantes

Pour plus d’informations sur la modification et la gestion des stratégies, consultez [les stratégies de gestion des risques de confidentialité](risk-management-policies.md) .