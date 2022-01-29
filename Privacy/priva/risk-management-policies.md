---
title: Créer des stratégies dans la gestion des risques de confidentialité
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
description: Découvrez comment créer et personnaliser des stratégies de confidentialité pour la gestion des données personnelles de votre organisation dans Microsoft 365.
ms.openlocfilehash: ce8f2d5e6728bcd01a99775450668c002c9cb59e
ms.sourcegitcommit: f145dff5e387a8e26db2f3a2c7de125978fbacc9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/28/2022
ms.locfileid: "62249032"
---
# <a name="create-policies-in-privacy-risk-management"></a>Créer des stratégies dans la gestion des risques de confidentialité

Vous pouvez créer de nouvelles stratégies dans la Gestion des risques de confidentialité pour résoudre les scénarios de risque importants pour votre organisation. Pour un démarrage rapide, utilisez les modèles par défaut pour créer de nouvelles stratégies pour la surexposion de données, les transferts de données, ainsi que la réduction et les scénarios de données. Vous pouvez également personnaliser vos propres stratégies, en utilisant l’un de ces modèles comme point de départ.

Lors de la création ou de la modification de stratégies, vous pouvez configurer des notifications par courrier électronique ou, le cas besoin, des conseils de stratégie pour Teams afin d’attirer l’attention de vos utilisateurs sur les correspondances de stratégie afin de les mettre à jour.

## <a name="create-a-policy-from-a-template"></a>Créer une stratégie à partir d’un modèle

Suivez ces étapes pour créer une stratégie à l’aide de l’un des modèles par défaut.

1. Dans la [Centre de conformité Microsoft 365](https://compliance.microsoft.com/), sélectionnez Stratégies **dans la** section Gestion des risques pour la confidentialité.
1. Sélectionnez **Créer une stratégie**.
1. Choisissez le type de modèle souhaité. Cela permet d’ouvrir un volet volant avec des informations sur le modèle.
1. Pour passer en revue les paramètres par défaut du modèle, y compris les types de données, les emplacements de données et les conditions qui déclenchent des correspondances de stratégie, sélectionnez **Paramètres d’affichage**.
     - Vous avez la possibilité ici de sélectionner **Modifier les paramètres** pour apporter des modifications. Cela vous dirigera vers l’Assistant pour la personnalisation des paramètres.
1. Si vous êtes prêt à choisir les paramètres par défaut, donnez un nom descriptif à votre stratégie et sélectionnez **Créer une stratégie.**

Lorsque vous créez une stratégie directement à partir d’un modèle, de nombreux paramètres sont automatiquement choisis. Il démarre également en mode test par défaut, ce qui signifie qu’aucune alerte ou notification n’est générée. Si vous êtes prêt à activer entièrement votre stratégie après l’avoir exécute en mode test et passé en revue les résultats de la stratégie, vous pouvez la trouver dans votre liste de stratégies et modifier la stratégie pour l’activer.

## <a name="create-a-custom-policy"></a>Créer une stratégie personnalisée

Pour prendre un contrôle granulaire des paramètres d’une stratégie, vous pouvez créer une stratégie personnalisée à l’aide de l’un des modèles existants comme base. Priva fournit un Assistant pour vous guider tout au long de ces étapes.

Tous les types de stratégie suivent ce flux de base. Certains paramètres et options changent en fonction de la stratégie que vous avez choisie.

1. Dans la [Centre de conformité Microsoft 365](https://compliance.microsoft.com/), sélectionnez Stratégies **dans la** section Gestion des risques pour la confidentialité.
1. Sélectionnez **Créer une stratégie**.
1. Choisissez **l’option** Personnalisée pour commencer à utiliser l’Assistant.
1. Choisissez votre type de modèle de référence : **surexposion de données,** **transferts de données ou** réduction **des données**. Chacune d’elles vous offre certaines options lors de la création de la stratégie.
1. Nommez et décrivez votre stratégie. Nous vous recommandons d’utiliser des noms clairs et descriptifs pour identifier vos stratégies, car ces noms apparaîtront ultérieurement dans les alertes concernant les correspondances de stratégie.
1. Continuez à l’aide de l’Assistant et choisissez les paramètres souhaités. Les options suivantes sont disponibles : 
    - **Données à surveiller :** sélectionnez le type de données personnelles que votre stratégie surveillera.
    - **Utilisateurs et groupes** : appliquez votre stratégie à tous les utilisateurs ou utilisateurs sélectionnés.
    - **Emplacements** : appliquez votre stratégie aux zones sélectionnées dans Microsoft 365.
    - **Conditions** : définissez les conditions de votre stratégie. Ces options varient en fonction de votre type de stratégie.
    - **Résultats :** définissez les résultats lorsqu’une correspondance de stratégie est trouvée, telles que les notifications de l’utilisateur.
    - **Alertes :** déterminez la fréquence des alertes pour les administrateurs lorsqu’une correspondance de stratégie est trouvée.
    - **Mode** : choisissez d’abord d’exécuter ou non votre stratégie en mode test.
1. Lorsque tous les paramètres sont terminés, examinez vos choix, az les modifications souhaitées, puis sélectionnez **Envoyer pour créer** la stratégie.

## <a name="learn-about-key-settings-for-all-policies"></a>En savoir plus sur les paramètres clés de toutes les stratégies

### <a name="choose-data-to-monitor"></a>Choisir les données à surveiller

Lors de la modification ou de la configuration d’un type de stratégie personnalisée, vous serez invité à sélectionner les types de données que votre stratégie doit surveiller. Les options sont les suivantes :

- **Groupes de classification** : liste d’ensembles de données utilisables dans une recherche en fonction des principales réglementations en matière de confidentialité, telles que le R GDPR ou la LOI AMÉRICAINE. Afficher les détails d’un groupe pour voir les types d’informations sensibles qu’il couvre. Sélectionnez un ou plusieurs de ces ensembles pour les utiliser tels qu’ils sont.
- Types d’informations sensibles individuels : en choisissant vous-même des types d’informations sensibles spécifiques, tels que des numéros de sécurité sociale ou des informations de permis de conduire, vous pouvez personnaliser votre propre groupe ou groupe de données à rechercher. Cet Assistant vous permet de sélectionner dans la liste complète des types d’informations sensibles dans la gestion des risques de confidentialité. Chaque type d’informations possède ses propres propriétés. Utilisez le bouton d’informations à côté de l’un d’eux pour obtenir des détails et des remarques sur les paramètres recommandés. Si vous créez plusieurs groupes, l’Assistant vous permet d’appliquer des opérateurs booléens pour les relier et définir leur ordre d’opération.

Si vous sélectionnez à partir des groupes de classification existants, vous ne pouvez pas également sélectionner des types individuels ou créer vos propres groupes. Pour une plus grande flexibilité, choisissez des types d’informations sensibles individuels. Pour utiliser les normes les plus courantes, choisissez parmi les groupes de classification.

### <a name="set-user-email-notifications"></a>Définir les notifications par courrier électronique de l’utilisateur

Avec [les notifications par courrier](risk-management-notifications.md) électronique, vous pouvez envoyer des notifications concernant les correspondances de stratégie directement à vos propriétaires de contenu. Ces e-mails résument les données qui doivent être examinées et les actions possibles à effectuer, telles que la possibilité de rendre les documents privés, de les conserver dans un fichier, de signaler les correspondances faux positifs et d’ajouter des notes pour référence ultérieure. Ces e-mails incluent également des liens pour les destinataires de formation sur la façon de gérer ces cas. La fourniture de ces liens est requise et doit pointer vers votre propre documentation interne sur les processus et les meilleures pratiques.

Les notifications peuvent être activées pour des stratégies individuelles lors de la création d’une stratégie personnalisée ou lors de la modification d’une stratégie. Définissez vos préférences dans la section **Résultats** .

Les paramètres requis incluent la fréquence de vos notifications et votre lien vers la formation à la confidentialité.

Les paramètres facultatifs incluent certains champs personnalisables pour vos e-mails. Sélectionnez **l’option Aperçu et modifier le courrier de notification** pour ouvrir un volet volant qui affiche un exemple de notification. Ici, vous pouvez modifier la ligne d’objet de l’e-mail, l’en-tête et le corps du texte, ainsi que le nom d’affichage et l’URL de votre formation sur la confidentialité.

Notez que la fonctionnalité globale de gestion des risques de confidentialité pour envoyer des notifications par courrier électronique est contrôlée **dans Paramètres**. Elle est activée par défaut. La mise hors service de ce paramètre arrête tous les e-mails, même si les notifications ont été configurées à un niveau de stratégie individuel.

## <a name="learn-about-settings-for-data-minimization-policies"></a>En savoir plus sur les paramètres des stratégies de réduction des données

Les stratégies de réduction des données se concentrent sur l’âge de votre contenu et la durée depuis sa dernière modification. La surveillance des données personnelles qui sont toujours conservées dans du contenu ancien et inutilisé peut vous aider à mieux gérer vos données stockées et à réduire les risques. Ce paramètre est géré dans **l’écran Conditions** .

Par défaut, les stratégies de réduction des données recherchent le contenu contenant des données personnelles qui ont été créées ou modifiées pour la dernière fois il y a au moins 60 jours. Lors de la modification ou de la création d’une stratégie personnalisée, vous pouvez choisir parmi d’autres périodes prédéfinis.

## <a name="learn-about-settings-for-data-transfer-policies"></a>En savoir plus sur les paramètres des stratégies de transfert de données

Les stratégies de transfert de données vous permettent de surveiller les données transférées entre certaines régions du monde ou entre les différents services de votre organisation. Dans **l’écran Conditions** , vous pouvez choisir les types de transferts que la Gestion des risques de confidentialité doit rechercher.

Par défaut, les stratégies de transfert de données recherchent les transferts entre l’Amérique du Nord et d’autres régions. Lors de la modification ou de la création d’une stratégie personnalisée, vous pouvez choisir le type de transfert, puis effectuer des sélections pour les régions ou départements de l’expéditeur et du destinataire.

Les stratégies de transfert de données offrent également des conseils et des recommandations de stratégie à vos utilisateurs dans Teams, afin qu’ils restent informés des meilleures pratiques de gestion des données. Vous pouvez le faire sur **l’écran Résultats** .

## <a name="learn-about-settings-for-data-overexposure-policies"></a>En savoir plus sur les paramètres des stratégies de surexpossure des données

Votre organisation peut stocker du contenu à différents niveaux d’accès, y compris des zones accessibles au public et d’autres qui sont restreintes. Dans **l’écran Conditions** , vous pouvez choisir que la Gestion des risques de confidentialité recherche les données potentielles surexposées pour le contenu stocké à l’un des niveaux d’accès suivants :

- **Public** : toute personne ayant un lien peut afficher ce contenu.
- **Externe :** des personnes spécifiques extérieures à l’organisation ont accès.
- **Interne :** les utilisateurs de votre organisation ont accès.

Par défaut, les stratégies de surexpossure des données évaluent les trois niveaux d’accès. Lors de la modification ou de la création d’une stratégie personnalisée, vous pouvez choisir l’ensemble ou l’un de ces niveaux.

## <a name="next-steps"></a>Prochaines étapes

Pour plus d’informations sur la façon de gérer vos stratégies et d’apporter des modifications après leur création, voir [Gérer les stratégies](risk-management-policies-manage.md).

## <a name="legal-disclaimer"></a>Clause d’exclusion de responsabilité légale

[Clause d’exclusion de responsabilité légale Microsoft Priva](priva-disclaimer.md)
