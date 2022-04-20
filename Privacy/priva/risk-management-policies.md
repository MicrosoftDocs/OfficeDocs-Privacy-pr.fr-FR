---
title: Créer des stratégies dans la gestion des risques liés à la confidentialité
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
description: Découvrez comment créer et personnaliser des stratégies de confidentialité pour gérer les données personnelles de votre organisation dans Microsoft 365.
ms.openlocfilehash: 2b655d778e73e2107c289988966fb491bf3ebb2e
ms.sourcegitcommit: 09ecdaded9a9f8f79587f2acb978dc53b83e5c01
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/19/2022
ms.locfileid: "64930505"
---
# <a name="create-policies-in-privacy-risk-management"></a>Créer des stratégies dans la gestion des risques liés à la confidentialité

Vous pouvez créer de nouvelles stratégies dans la gestion des risques liés à la confidentialité pour résoudre les scénarios de risque importants pour votre organisation. Pour un démarrage rapide, utilisez les modèles par défaut pour créer de nouvelles stratégies pour la surexposition des données, les transferts de données, la minimisation des données et les scénarios. Vous pouvez également personnaliser vos propres stratégies, en utilisant l’un de ces modèles comme point de départ.

Lors de la création ou de la modification de stratégies, vous pouvez configurer des notifications par e-mail ou, le cas échéant, des conseils de stratégie pour Teams pour attirer l’attention de vos utilisateurs sur les correspondances de stratégie à des fins de correction.

## <a name="create-a-policy-from-a-template"></a>Créer une stratégie à partir d’un modèle

Suivez ces étapes pour créer une stratégie à l’aide de l’un des modèles par défaut.

1. Dans le [portail de conformité Microsoft Purview](https://compliance.microsoft.com/), accédez à la section Priva Privacy Risk Management et sélectionnez **Stratégies**.
1. Sélectionnez **Créer une stratégie**.
1. Choisissez le type de modèle souhaité. Un volet volant contenant des informations sur le modèle s’ouvre.
1. Pour passer en revue les paramètres par défaut du modèle, notamment les types de données, les emplacements de données et les conditions qui déclenchent les correspondances de stratégie, sélectionnez **Paramètres d’affichage**.
     - Vous avez ici la possibilité de sélectionner **Modifier les paramètres** pour apporter des modifications. Cela vous dirigera vers l’Assistant pour la personnalisation des paramètres.
1. Si vous êtes prêt à utiliser les paramètres par défaut, donnez un nom descriptif à votre stratégie, puis **sélectionnez Créer une stratégie.**

Lors de la création d’une stratégie directement à partir d’un modèle, de nombreux paramètres sont choisis automatiquement pour vous. Il démarre également en mode test par défaut, ce qui signifie qu’aucune alerte ou notification n’est générée. Si vous êtes prêt à activer entièrement votre stratégie après l’avoir exécutée en mode test et passé en revue les résultats de la stratégie, vous pouvez la trouver dans votre liste de stratégies et modifier la stratégie pour la désactiver.

## <a name="create-a-custom-policy"></a>Créer une stratégie personnalisée

Pour prendre un contrôle précis des paramètres d’une stratégie, vous pouvez créer une stratégie personnalisée à l’aide de l’un des modèles existants comme base de référence. Priva fournit un Assistant pour vous guider tout au long de ces étapes.

Tous les types de stratégies suivent ce flux de base. Certains paramètres et options changeront en fonction de la stratégie choisie.

1. Dans le [portail de conformité Microsoft Purview](https://compliance.microsoft.com/), accédez à la section Priva Privacy Risk Management et sélectionnez **Stratégies**.
1. Sélectionnez **Créer une stratégie**.
1. Choisissez l’option **Personnalisée** pour commencer à utiliser l’Assistant.
1. Choisissez votre type de modèle de base : **surexposition des données,** **transferts de données** ou **réduction des données**. Chacune d’elles vous donnera certaines options lors de la création de la stratégie.
1. Nommez et décrivez votre stratégie. Nous vous recommandons d’utiliser des noms clairs et descriptifs pour identifier vos stratégies, car ces noms apparaîtront plus loin dans les alertes relatives aux correspondances de stratégie.
1. Passez à l’Assistant et choisissez les paramètres souhaités. Les options suivantes sont disponibles : 
    - **Données à surveiller** : sélectionnez le type de données personnelles que votre stratégie surveillera.
    - **Utilisateurs et groupes** : appliquez votre stratégie à tous les utilisateurs ou utilisateurs sélectionnés.
    - **Emplacements** : appliquez votre stratégie à des zones sélectionnées dans Microsoft 365.
    - **Conditions** : définissez les conditions de votre stratégie. Ces options varient en fonction de votre type de stratégie.
    - **Résultats** : définissez les résultats lorsqu’une correspondance de stratégie est trouvée, par exemple les notifications utilisateur.
    - **Alertes** : déterminez la fréquence des alertes aux administrateurs lorsqu’une correspondance de stratégie est trouvée.
    - **Mode** : choisissez d’exécuter ou non votre stratégie en mode test.
1. Une fois tous les paramètres terminés, passez en revue vos choix, apportez les modifications souhaitées, puis sélectionnez **Envoyer** pour créer la stratégie.

## <a name="learn-about-key-settings-for-all-policies"></a>En savoir plus sur les paramètres clés pour toutes les stratégies

### <a name="choose-data-to-monitor"></a>Choisir les données à surveiller

Lors de la modification ou de la configuration d’un type de stratégie personnalisée, vous êtes invité à sélectionner les types de données que votre stratégie doit surveiller. Les options sont les suivantes :

- **Groupes de classification** : liste pouvant faire l’objet d’une recherche d’ensembles de données basés sur des réglementations de confidentialité clés, telles que le RGPD ou l’HIPAA. Affichez les détails d’un groupe pour voir les types d’informations sensibles qu’il couvre. Sélectionnez un ou plusieurs de ces ensembles pour les utiliser tels qu’ils sont.
- **Types d’informations sensibles individuels** : en choisissant vous-même des types d’informations sensibles spécifiques, tels que les numéros de sécurité sociale ou les informations de permis de conduire, vous pouvez personnaliser votre propre groupe ou groupe de données à rechercher. Cet Assistant vous permet de sélectionner dans la liste complète des types d’informations sensibles dans Gestion des risques liés à la confidentialité. Chaque type d’informations a ses propres propriétés. Utilisez le bouton d’informations à côté de l’un d’eux pour obtenir des détails et des notes sur les paramètres recommandés. Si vous créez plusieurs groupes, l’Assistant vous permet d’appliquer des opérateurs booléens pour les associer et définir leur ordre des opérations.

Si vous sélectionnez dans les groupes de classification existants, vous ne pouvez pas également sélectionner des types individuels ou créer vos propres groupes. Pour plus de flexibilité, choisissez des types d’informations sensibles individuels. Pour utiliser les normes les plus courantes, choisissez parmi les groupes de classification.

### <a name="set-user-email-notifications"></a>Définir les notifications par e-mail des utilisateurs

Avec [les notifications par e-mail](risk-management-notifications.md), vous pouvez envoyer des notifications sur les correspondances de stratégie directement à vos propriétaires de contenu. Ces e-mails récapitulent les données à examiner et les actions possibles à prendre, telles que la mise en privé des documents, leur conservation dans les fichiers, la création de rapports sur les correspondances de faux positifs et l’ajout de notes pour une référence ultérieure. Ces e-mails incluent également des liens pour les destinataires de formation sur la façon de gérer ces cas. La fourniture de ces liens est nécessaire et doit pointer vers votre propre documentation interne sur les processus et les meilleures pratiques.

Les notifications peuvent être activées pour des stratégies individuelles lors de la création d’une stratégie personnalisée ou lors de la modification d’une stratégie. Définissez vos préférences dans la section **Résultats** .

Les paramètres requis incluent la fréquence de vos notifications et votre lien vers la formation à la confidentialité.

Les paramètres facultatifs incluent certains champs personnalisables pour vos e-mails. Sélectionnez l’option **Aperçu et modifier la messagerie de notification** pour ouvrir un volet volant qui affiche un exemple de notification. Ici, vous pouvez modifier la ligne d’objet de l’e-mail, l’en-tête et le texte du corps, ainsi que le nom d’affichage et l’URL de votre formation de confidentialité.

Notez que la fonctionnalité globale de gestion des risques liés à la confidentialité pour envoyer des notifications par e-mail est contrôlée dans **Paramètres**. Elle est activée par défaut. La désactivation de ce paramètre arrête tous les e-mails même si les notifications ont été configurées au niveau d’une stratégie individuelle.

## <a name="learn-about-settings-for-data-minimization-policies"></a>En savoir plus sur les paramètres des stratégies de minimisation des données

Les stratégies de réduction des données se concentrent sur l’âge de votre contenu et sur la durée de sa dernière modification. La surveillance des données personnelles qui sont toujours conservées dans du contenu plus ancien et inutilisé peut vous aider à mieux gérer vos données stockées et à réduire les risques. Ce paramètre est géré sur l’écran **Conditions** .

Par défaut, les stratégies de réduction des données recherchent du contenu contenant des données personnelles qui ont été créées ou modifiées pour la dernière fois il y a au moins 30 jours. Lors de la modification ou de la création d’une stratégie personnalisée, vous pouvez sélectionner d’autres délais prédéfinis.

## <a name="learn-about-settings-for-data-transfer-policies"></a>En savoir plus sur les paramètres des stratégies de transfert de données

Les stratégies de transfert de données vous permettent de surveiller les transferts de données personnelles en dehors de votre organisation, ainsi que les transferts internes entre différents services ou pays ou régions. Dans l’écran **Conditions** , vous pouvez choisir les types de transferts que la gestion des risques liés à la confidentialité doit rechercher.

Par défaut, les stratégies de transfert de données détectent quand les données personnelles de votre organisation sont transférées ou partagées avec un destinataire ou un emplacement en dehors de votre organisation. Lors de la modification ou de la création d’une stratégie personnalisée, vous pouvez choisir le type de transfert, puis effectuer des sélections pour les régions ou services de l’expéditeur et du destinataire.

Les stratégies de transfert de données prennent également en charge la fourniture de conseils et de recommandations de stratégie à vos utilisateurs dans Teams, afin qu’ils puissent rester informés des meilleures pratiques de gestion des données. Cette option peut être activée sur l’écran **Résultats** .

## <a name="learn-about-settings-for-data-overexposure-policies"></a>En savoir plus sur les paramètres des stratégies de surexposition des données

Votre organisation peut stocker du contenu à différents niveaux d’accès, y compris des zones accessibles publiquement et d’autres qui sont restreintes. Dans l’écran **Conditions** , vous pouvez choisir de demander à Privacy Risk Management de rechercher une surexposition potentielle des données pour le contenu stocké à l’un des niveaux d’accès suivants :

- **Public** : toute personne disposant d’un lien peut afficher ce contenu.
- **Externe** : des personnes spécifiques en dehors de l’organisation ont accès.
- **Interne** : les utilisateurs de votre organisation ont accès.

Par défaut, les stratégies de surexposition des données évaluent les trois niveaux d’accès. Lors de la modification ou de la création d’une stratégie personnalisée, vous pouvez choisir l’ensemble ou l’un de ces niveaux.

## <a name="next-steps"></a>Étapes suivantes

Pour plus d’informations sur la façon de gérer vos stratégies et d’apporter des modifications après leur création, consultez [Gérer les stratégies](risk-management-policies-manage.md).

## <a name="legal-disclaimer"></a>Exclusion de responsabilité légale

[Exclusion de responsabilité légale de Microsoft Priva](priva-disclaimer.md)
