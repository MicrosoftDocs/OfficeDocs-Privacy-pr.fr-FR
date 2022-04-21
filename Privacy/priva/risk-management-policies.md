---
title: Stratégies de gestion des risques liés à la confidentialité
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
description: Découvrez comment créer et gérer des stratégies dans Microsoft Priva Privacy Risk Management pour gérer les données personnelles de votre organisation dans Microsoft 365.
ms.openlocfilehash: 87671cedc8c6cba75d5ad207b52831cdd2467187
ms.sourcegitcommit: b5f7dcb73c0e3f677981e80106769cb546d00af4
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/21/2022
ms.locfileid: "65014494"
---
# <a name="privacy-risk-management-policies"></a>Stratégies de gestion des risques liés à la confidentialité

Les stratégies de gestion des risques liés à la confidentialité peuvent vous aider à résoudre les scénarios à risque qui sont importants pour votre organisation. Nos modèles de stratégie sont centrés sur la promotion de bonnes pratiques de gestion des données.  Les alertes indiquent aux administrateurs quand des correspondances de stratégie sont détectées et peuvent nécessiter une investigation plus approfondie. Les notifications par e-mail et les conseils dans Microsoft Teams aident les utilisateurs à comprendre quelles activités présentent des risques de confidentialité, permettent aux utilisateurs de résoudre immédiatement les problèmes et les orientent vers la formation à la confidentialité.

Pour un démarrage rapide, utilisez un modèle avec des paramètres par défaut pour créer de nouvelles stratégies pour la surexposition des données, les transferts de données, la minimisation des données et les scénarios. Vous pouvez également personnaliser les paramètres de modèle pour créer des stratégies qui répondent aux besoins de votre organisation.

## <a name="policy-template-types"></a>Types de modèles de stratégie

La gestion des risques liés à la confidentialité a trois modèles de stratégie conçus pour vous aider à résoudre les principaux problèmes liés à la protection des données personnelles. Chaque modèle a des paramètres par défaut que vous pouvez accepter dans le processus de configuration rapide, ou personnaliser à l’aide d’un processus guidé. Lorsque vous créez une stratégie, votre première tâche consiste à choisir l’un des trois modèles répertoriés ci-dessous :

- **Surexposition des données** : cette stratégie identifie les éléments de contenu contenant des données personnelles qui peuvent être trop largement accessibles par d’autres personnes. Lorsque des correspondances sont trouvées, vous pouvez configurer des notifications invitant les propriétaires de contenu à appliquer rapidement la protection.

- **Transferts de données** : cette stratégie peut détecter les transferts de données personnelles au-delà des limites que vous déterminez, ce qui peut impliquer des transferts en dehors de votre organisation, ou des transferts internes entre des services ou des régions géographiques. Lorsque des correspondances sont trouvées, vous pouvez configurer des notifications encourageant les expéditeurs à révoquer l’accès au contenu.

- **Réduction des données** : cette stratégie identifie les éléments de contenu contenant des données personnelles qui ont été intactes pendant de longues périodes. Lorsque des correspondances sont trouvées, vous pouvez envoyer des notifications aux propriétaires de contenu les invitant à prendre des mesures rapides pour conserver ou supprimer l’élément.

## <a name="quick-setup-using-a-template-with-default-settings"></a>Configuration rapide : utilisation d’un modèle avec les paramètres par défaut

Lors de la création d’une stratégie directement à partir d’un modèle, la plupart des paramètres sont choisis automatiquement pour vous aider à être opérationnel rapidement. Procédez comme suit pour créer une stratégie avec des paramètres par défaut à l’aide de l’un de nos modèles :

1. Dans le [centre de conformité Microsoft Purview](https://compliance.microsoft.com/), recherchez Priva Privacy Risk Management dans le volet de navigation de gauche et sélectionnez **Stratégies**.

2. Sélectionnez **Créer une stratégie** dans le coin supérieur droit de l’écran, qui affiche un volet volant répertoriant toutes les options de création de stratégie.

3. Recherchez le type de stratégie que vous souhaitez créer et, dans sa carte, **sélectionnez Créer**.

4. Un volet volant contient les détails de la stratégie. La sélection des **paramètres d’affichage** affiche les paramètres par défaut. Vous pouvez modifier les paramètres à partir d’ici, ce qui vous permet d’accéder au processus guidé décrit ci-dessous. Pour continuer à créer votre stratégie à l’aide des paramètres par défaut, entrez simplement un nom descriptif, puis **sélectionnez Créer une stratégie**.

Votre stratégie sera créée et vous la trouverez dans la page **Stratégies** .

La stratégie commence à s’exécuter en mode test, ce qui signifie qu’aucune alerte ou notification n’est générée et que vous pouvez surveiller ses performances. Lorsque vous êtes prêt à activer votre stratégie, sélectionnez-la et modifiez-la pour l’activer.

## <a name="custom-setup-guided-process-to-choose-all-settings"></a>Configuration personnalisée : processus guidé pour choisir tous les paramètres

L’option de stratégie personnalisée est un processus guidé pour la création d’une stratégie. Vous allez commencer par choisir un modèle, puis parcourir chaque paramètre pour personnaliser votre stratégie. Les instructions ci-dessous fournissent des détails sur les paramètres de base qui s’appliquent à chacun des trois types de stratégie. Lorsque les paramètres diffèrent par type de stratégie, nous allons établir un lien vers des instructions spécifiques.

Suivez les étapes ci-dessous pour créer une stratégie :

1. Dans le [Centre de conformité Microsoft 365](https://compliance.microsoft.com/), recherchez Priva Privacy Risk Management dans le volet de navigation gauche. Dans le menu déroulant, sélectionnez **Stratégies**.

2. Sélectionnez **Créer une stratégie**.

3. Choisissez l’option **Personnalisée** pour créer votre stratégie à l’aide de l’Assistant Création de stratégie dans Gestion des risques liés à la confidentialité.

4. Choisissez le type de stratégie : **surexposition des données,** **transferts de données** ou **réduction des données**.

5. Donnez un nom descriptif à votre stratégie pour vous aider à l’identifier dans votre liste de stratégies. Fournissez une description facultative, puis sélectionnez **Suivant**.

6. Les étapes suivantes vous permettent de définir tous les paramètres de stratégie. Pour plus d’informations, vous pouvez accéder aux descriptions de cet article. Les options suivantes sont disponibles : 
    - [**Données à surveiller**](#choose-data-to-monitor) : sélectionnez le type de données personnelles que votre stratégie surveillera.
    - [**Utilisateurs et groupes**](#choose-users-and-groups) : appliquez votre stratégie à tous les utilisateurs ou utilisateurs sélectionnés.
    - [**Emplacements**](#choose-locations) : appliquez votre stratégie à des zones sélectionnées dans Microsoft 365.
    - [**Conditions**](#set-conditions) : définissez les conditions de votre stratégie. Ces options varient en fonction de votre type de stratégie.
    - [**Résultats**](#define-outcomes-user-email-notifications-and-tips) : définissez les résultats lorsqu’une correspondance de stratégie est trouvée, par exemple les notifications par e-mail de l’utilisateur.
    - [**Alertes**](#set-alerts) : déterminez la fréquence des alertes aux administrateurs lorsqu’une correspondance de stratégie est trouvée.
    - [**Mode**](#testing-a-policy) : choisissez d’exécuter ou non votre stratégie en mode test.
7. Une fois tous les paramètres terminés, passez en revue vos choix, apportez les modifications souhaitées, puis sélectionnez **Envoyer** pour créer la stratégie.

Après quelques secondes, vous verrez une confirmation que la stratégie a été créée. Sélectionnez **Terminé** dans la page de confirmation, qui vous amène à la page **Stratégies** où vous verrez la nouvelle stratégie en haut du tableau.

Les sections ci-dessous fournissent des détails supplémentaires sur chaque paramètre de stratégie.

## <a name="choose-data-to-monitor"></a>Choisir les données à surveiller

Lors de la création ou de la modification d’une stratégie, nous vous demandons de sélectionner les types de données que la stratégie doit surveiller. Il existe deux options :

- **Groupes de classification** : liste de regroupements de types d’informations sensibles pouvant faire l’objet d’une recherche ; par exemple, un groupe basé sur l’Australia Health Records Act ou un groupe basé sur des informations d’identification personnelle des États-Unis, telles qu’un numéro de passeport américain.

- **Types d’informations sensibles individuels** : liste de types d’informations sensibles pouvant faire l’objet d’une recherche ; par exemple, les numéros de sécurité sociale ou les numéros de permis de conduire.

Si vous sélectionnez dans les groupes de classification existants, vous ne pouvez pas non plus sélectionner des types individuels ou créer vos propres groupes. Pour plus de flexibilité, choisissez des types d’informations sensibles individuels. Pour utiliser les normes les plus courantes, choisissez parmi les groupes de classification. En savoir plus sur chaque type de données ci-dessous.

### <a name="classification-groups"></a>Groupes de classification

Les groupes de classification sont des regroupements de [types d’informations sensibles](/microsoft-365/compliance/sensitive-information-type-entity-definitions) utilisés pour détecter du contenu lié à des données personnelles ou à des réglementations spécifiques.

Lorsque vous sélectionnez cette option dans la page **Données à surveiller** , vous devez sélectionner **+Ajouter des groupes de classification** et choisir un ou plusieurs groupes dans la liste qui s’affiche dans un volet de menu volant.

### <a name="individual-sensitive-information-types"></a>Types d’informations sensibles individuels

En choisissant des [types d’informations sensibles](/microsoft-365/compliance/sensitive-information-type-entity-definitions) spécifiques, tels que les numéros de sécurité sociale ou les informations de permis de conduire, vous pouvez personnaliser votre propre groupe ou groupe de données à rechercher. Vous pouvez effectuer une sélection dans la liste complète des types d’informations sensibles dans Gestion des risques liés à la confidentialité. Chaque type d’informations a ses propres propriétés.

Lorsque vous sélectionnez cette option sur la page **Données à surveiller** , un sélecteur s’affiche avec **la valeur par défaut** répertoriée comme nom pour le groupe de types d’informations sensibles que vous sélectionnez. Conservez ou modifiez ce nom de groupe, puis sélectionnez **Ajouter** pour sélectionner un ou plusieurs types d’informations sensibles dans la liste complète dans Gestion des risques de confidentialité. Chaque type d’informations a ses propres propriétés et paramètres recommandés, que vous pouvez découvrir en sélectionnant l’icône d’informations à droite du menu déroulant Confiance après avoir ajouté le type d’informations. Vous pouvez également modifier le nombre d’instances pour chaque type d’informations sensibles. Ce paramètre désigne le nombre d’instances uniques de chaque type d’informations sensibles que votre stratégie doit détecter.

Si vous créez plusieurs groupes, l’Assistant vous permet de sélectionner la façon dont les groupes doivent se connecter (relation « et » ou « ou ») et de définir leur ordre des opérations.

## <a name="choose-users-and-groups"></a>Choisir des utilisateurs et des groupes

Vous avez deux options pour déterminer quels utilisateurs une stratégie couvrira : tous les utilisateurs et groupes, ou des utilisateurs et des groupes spécifiques.

- **Tous les utilisateurs et groupes** : cette option applique la stratégie à tous les utilisateurs et groupes Office 365 de votre organisation.

- **Utilisateurs ou groupes spécifiques** : cette option vous permet de sélectionner des utilisateurs individuels, des groupes Office 365 individuels ou une combinaison des deux.
  - **Pour choisir des utilisateurs** : **sélectionnez Choisir des utilisateurs** et, dans le volet de menu volant, recherchez un utilisateur en entrant une adresse e-mail dans la zone de recherche. Ou recherchez l’utilisateur dans la liste et cochez la case à gauche de son nom. Vous pouvez sélectionner jusqu’à 100 utilisateurs. Lorsque vous avez terminé, **sélectionnez Ajouter.**
  - **Pour choisir des groupes** : **sélectionnez Choisir des groupes** et, dans le volet volant, cochez la case à gauche de chaque nom de groupe. Vous pouvez sélectionner jusqu’à dix groupes. Lorsque vous avez terminé, **sélectionnez Ajouter**.

Après avoir désigné des utilisateurs et des groupes, sélectionnez **Suivant** pour passer à l’étape suivante.

## <a name="choose-locations"></a>Choisir des emplacements

Dans cette étape, vous allez indiquer où, dans votre environnement Microsoft 365, vous souhaitez que la stratégie recherche des correspondances de données personnelles. Les options d’emplacement dépendent du type de stratégie, et vous pouvez en sélectionner plusieurs. Chacun des emplacements est expliqué ci-dessous.

- **Exchange** : la stratégie identifie les correspondances dans les comptes Exchange des utilisateurs, qui incluent du contenu dans le corps des e-mails et dans les pièces jointes envoyées ou reçues par Exchange boîtes aux lettres.

- **OneDrive** : la stratégie identifie les correspondances dans les fichiers stockés dans le compte OneDrive Entreprise des utilisateurs.

- **Teams** : la stratégie identifie les correspondances dans les messages des utilisateurs dans Teams canaux et conversations.

- **SharePoint** : la stratégie identifie les correspondances dans les fichiers stockés dans les sites SharePoint des utilisateurs. Lorsque vous sélectionnez cette option, vous choisissez entre les options suivantes :
    - **Tous les sites SharePoint** : cette sélection couvre tous les sites de tous les utilisateurs de votre organisation.

    - **Sites SharePoint spécifiques** : cette sélection vous demande de désigner des sites spécifiques auxquels la stratégie doit s’appliquer. Vous pouvez entrer l’URL d’un site spécifique directement dans la zone URL, puis sélectionner le signe pour l’ajouter **+** à votre liste de sites. Vous pouvez également sélectionner **Choisir des sites** et, dans le volet volant, rechercher et sélectionner dans la liste des sites auxquels vous avez accès. Cochez la case qui s’affiche lorsque vous pointez sur le site que vous souhaitez sélectionner. Après avoir effectué vos sélections, sélectionnez **Ajouter**.  Tous les sites que vous avez choisis sont répertoriés en bas de la page **Emplacements** .
    
    > [!TIP]
    > Si vous avez besoin d’aide pour identifier les sites SharePoint dans votre organisation, [visitez Gérer les sites dans le centre d’administration SharePoint](/sharepoint/manage-sites-in-new-admin-center).

Une fois que vous avez terminé de désigner des emplacements, sélectionnez **Suivant**.

## <a name="set-conditions"></a>Définir les conditions

Les conditions de détection des correspondances de stratégie diffèrent en fonction du modèle de stratégie.

- **Surexposition des données** : reportez-vous à l’étape de conditions dans les [instructions d’installation personnalisée de la stratégie d’exposition des données](risk-management-policy-data-overexposure.md#custom-setup-guided-policy-creation-process).
- **Transferts de données** : reportez-vous à l’étape des conditions dans les [instructions d’installation personnalisée de la stratégie de transfert de données](risk-management-policy-data-transfer.md#custom-setup-guided-policy-creation-process).
- **Réduction des données** : reportez-vous à l’étape de conditions dans les [instructions d’installation personnalisée de la stratégie de réduction des données](risk-management-policy-data-minimization.md#custom-setup-guided-policy-creation-process).

## <a name="define-outcomes-user-email-notifications-and-tips"></a>Définir les résultats : notifications et conseils par e-mail de l’utilisateur

Les paramètres de résultats sont gérés dans la page **Résultats** de l’Assistant Création de stratégie. Sur cette page, vous pouvez choisir d’envoyer une notification par e-mail aux utilisateurs lorsqu’ils effectuent une action qui correspond aux conditions d’une stratégie.

Les stratégies de transfert de données ont une option supplémentaire pour afficher des conseils aux utilisateurs dans Teams lorsque leurs actions génèrent une correspondance de stratégie. Ces conseils incluent des liens vers la formation sur la confidentialité, que vous fournissez, ainsi que des mécanismes de correction des risques potentiels.

Ces notifications peuvent être des opportunités utiles pour empêcher l’escalade des problèmes et pour renforcer les compétences et la confiance des utilisateurs dans l’adoption de pratiques de gestion des données sécurisées.

Consultez [les notifications utilisateur dans Privacy Risk Management](risk-management-notifications.md) pour en savoir plus sur l’utilisation des notifications utilisateur.

## <a name="set-alerts"></a>Définir des alertes

Les alertes aident les administrateurs à savoir quand un événement utilisateur correspond aux conditions d’une stratégie. La configuration des alertes est facultative et vous contrôlez la fréquence à laquelle les alertes sont générées, le seuil qui doit être atteint avant qu’une alerte soit générée et la gravité de l’alerte. Les alertes sont affichées dans la carte **Alertes** de la page **Stratégies** . En savoir plus sur [l’affichage, l’examen et la correction des alertes](risk-management-alerts.md).

#### <a name="turn-on-alerts"></a>Activer les alertes

Vous pouvez activer les alertes lorsque vous créez une stratégie pour la première fois, ou la modifier ultérieurement pour les activer. Dans la page **Alertes** de l’Assistant Création de stratégie, définissez le bouton bascule **Créer des alertes** sur la position **Activé** .

#### <a name="alert-frequency-and-thresholds"></a>Fréquence et seuils d’alerte
Après avoir activé les alertes, déterminez la fréquence à laquelle elles seront générées.

- **Alerte chaque fois qu’une correspondance de stratégie se produit** : la sélection de cette option peut générer un nombre élevé d’alertes.
- **Alerte lorsqu’un seuil spécifique est atteint** : vous définissez des seuils en fonction du nombre et de la fréquence des événements utilisateur détectés.

#### <a name="alert-severity-level"></a>Niveau de gravité de l’alerte
Sélectionnez un niveau de gravité faible, moyen ou élevé. Nous suggérons à votre organisation de définir ce que chaque niveau représente pour vous.

## <a name="testing-a-policy"></a>Test d’une stratégie

Lorsque vous créez une stratégie, le paramètre par défaut consiste à la démarrer en mode test. Cela signifie qu’une fois la stratégie créée :

- Aucune alerte n’est générée. Toutefois, vous verrez des insights sur la page de détails de la stratégie lorsque des correspondances sont détectées, y compris les types de données détectés et leurs emplacements.

- Aucune notification par e-mail de l’utilisateur n’est envoyée lorsque des correspondances de stratégie sont détectées. Toutefois, vous verrez des insights sur la page de détails de la stratégie montrant les utilisateurs associés aux correspondances de stratégie.

Le mode test vous permet de rechercher les correspondances des 30 derniers jours d’activité utilisateur. À l’aide de ces insights, vous pouvez évaluer le comportement de la stratégie et examiner les types d’alertes qui peuvent être générées lorsque la stratégie est activée.

Nous vous recommandons de tester votre stratégie pendant au moins cinq jours pour vous aider à comprendre le type et le volume des correspondances qu’elle générera. Vous pouvez [modifier la stratégie](#edit-a-policy) pendant qu’elle est en mode test afin de surveiller la façon dont les modifications affectent ses performances avant de l’activer. Par exemple, vous pouvez constater que la stratégie est trop large et que ses conditions doivent être ajustées. Vous pouvez également vous rendre compte, en fonction de l’activité, qu’elle détecte que les alertes ne seront pas générées dans un laps de temps utile pour vous.

La page de détails de la stratégie indique le nombre de jours d’exécution du test. Vous verrez combien de correspondances ont été trouvées par emplacement, combien d’événements utilisateur correspondant aux conditions de la stratégie ont été détectés et les types de données personnelles détectés par les correspondances de stratégie.

> [!NOTE]
> Si vous **basculez l’option Exécuter en mode test** vers la position **Désactivée** , *votre stratégie s’active* lorsque vous avez terminé de la créer. Cela signifie que toutes les alertes ou notifications utilisateur que vous avez configurées commencent à se générer lorsque des correspondances sont détectées.

Lorsque vous êtes satisfait des paramètres de votre stratégie et que vous êtes prêt à l’activer, sélectionnez le bouton bleu **Activer la stratégie** . La stratégie est désormais active et génère toutes les alertes et notifications utilisateur que vous configurez.

## <a name="turn-on-a-policy"></a>Activer une stratégie

Vous pouvez définir une stratégie à activer dès que vous avez terminé de la créer. Cela n’est pas recommandé, car il est préférable de surveiller les performances et les paramètres en mettant la stratégie en mode test avant de l’activer (voir [Test d’une stratégie](#testing-a-policy)).

Si vous avez créé votre stratégie en mode test, vous pouvez l’activer rapidement en procédant comme suit :

1. Dans votre page **Stratégies** , recherchez la stratégie et sélectionnez son nom pour ouvrir sa page de détails.
2. Dans la carte **d’état de** la stratégie, sélectionnez **Activer la stratégie**.

La stratégie est désormais active et génère toutes les alertes et notifications utilisateur que vous configurez.

## <a name="turn-off-a-policy"></a>Désactiver une stratégie

Vous pouvez désactiver une stratégie à tout moment en sélectionnant **Désactiver la stratégie** dans le coin supérieur droit de la page de détails d’une stratégie. Lorsqu’une stratégie est désactivée, elle ne détecte pas les correspondances ou ne génère pas d’alertes ou de notifications par e-mail. La désactivation d’une stratégie ne supprime pas une stratégie. Vous pouvez réactiver une stratégie en sélectionnant **Activer la stratégie** dans le coin supérieur droit de la page de détails de la stratégie.

## <a name="view-details-and-activity-from-the-policy-details-page"></a>Afficher les détails et l’activité à partir de la page des détails de la stratégie

Chaque stratégie a une page de détails montrant les activités détectées par la stratégie et des insights pour vous aider à résoudre les risques.

Une fois votre stratégie créée, sélectionnez son nom dans le tableau de la page **Stratégies** principale. L’onglet **Vue d’ensemble** de la page détails de la stratégie vous indique l’état de votre stratégie, fournit des insights sur vos données et met en évidence les correspondances de stratégie. Ici, vous pouvez afficher des détails sur des correspondances de stratégie spécifiques et en savoir plus sur les étapes suivantes. Si votre stratégie s’exécute en mode test, les étapes suivantes recommandées s’affichent sur cette page et un bouton pour activer la stratégie.

Lorsque la stratégie est activée, vous pouvez continuer à consulter sa page de détails de stratégie pour afficher des insights continus sur les domaines problématiques, la gravité et les tendances des alertes, ainsi que les actions correctives prises.

### <a name="overview-tab"></a>Onglet Overview

Sous l’onglet **Vue d’ensemble** de la page de détails de la stratégie, vous trouverez des détails sur ce que la stratégie détecte en ce qui concerne les types et les emplacements des données et l’activité des utilisateurs. Les informations sur la page de détails de la stratégie sont décrites ci-dessous. Après avoir activé une stratégie, la sortie des données peut prendre jusqu’à 48 heures.

#### <a name="policy-status"></a>État de la stratégie

La carte d’état de stratégie indique si votre stratégie se trouve dans l’un des trois états suivants : **Test**, **Activé** ou **Désactivé**.

**Test** : cette section indique le nombre de jours pendant lesquels votre stratégie a été en mode test, ce qui signifie qu’elle recherche des correspondances de stratégie en fonction des conditions que vous avez définies, mais ne génère pas d’alertes ou de notifications utilisateur. Nous vous fournirons une recommandation lorsqu’il sera temps d’activer votre stratégie. Vous pouvez l’activer à tout moment en sélectionnant le bouton **Activer** la stratégie sur cette carte.

**Activé** : lorsque votre stratégie est activée, la carte d’état affiche des métriques qui mettent en évidence le moment où une action corrective s’est produite après qu’une stratégie correspond à la génération d’alertes et de notifications utilisateur.

- **Actions de l’utilisateur :** cette métrique indique le nombre d’actions de correction effectuées par les utilisateurs lorsqu’ils sont invités à envoyer un e-mail de notification sur le nombre total de notifications envoyées. Par exemple, 8/10 représenterait que sur 10 notifications d’utilisateur envoyées, les utilisateurs ont effectué une action de correction dans 8 instances.

- **Taux de résolution des utilisateurs** : cette métrique est la vitesse à laquelle les actions de correction sont effectuées par les utilisateurs en fonction du nombre de notifications générées. Si le pourcentage est faible, vous pouvez [modifier le contenu de l’e-mail](risk-management-notifications.md#preview-and-customize-email-content) ou examiner attentivement les correspondances pour déterminer si la stratégie détecte l’activité prévue.

- **Actions d’administration effectuées** : cette métrique indique le nombre d’actions de correction effectuées par les administrateurs lorsqu’une alerte est générée par la stratégie. En savoir plus sur [la façon d’effectuer des actions sur les alertes](risk-management-alerts.md#manage-alerts).

- **Taux de résolution des** administrateurs : cette métrique correspond au taux auquel les actions de correction sont effectuées par les administrateurs en fonction du nombre d’alertes.

#### <a name="matches-by-location"></a>Correspond par emplacement

La carte **Correspondances par emplacement** affiche le nombre d’éléments de contenu détectés par la stratégie en fonction de l’emplacement Microsoft 365.

#### <a name="user-notifications"></a>Notifications à l’utilisateur

La carte de **notifications utilisateur** affiche un graphique à barres montrant le nombre d’e-mails de notification utilisateur qui ont été générés par la stratégie si ces fonctionnalités sont activées.

#### <a name="matches-by-user"></a>Correspond par utilisateur

Les **correspondances par carte d’utilisateur** répertorient les principaux utilisateurs dont les actions ont déclenché une correspondance de stratégie. Vous verrez le nombre d’événements détectés par la stratégie pour chaque utilisateur, ainsi que le nombre d’actions de correction effectuées à partir des notifications par e-mail. Sélectionnez **Afficher tous les utilisateurs** de cette carte pour passer en revue la liste complète des utilisateurs détectés par la stratégie.

#### <a name="matches-by-data-type"></a>Correspond par type de données

La carte **Correspondances par type de données** affiche les types de données personnelles détectées par les correspondances de stratégie et la quantité de chaque type. Le graphique à secteurs montre visuellement si un certain type de données personnelles, par exemple des numéros de sécurité sociale ou des numéros de carte de crédit, est principalement représenté dans les scénarios à risque que vous essayez d’identifier.

> [!TIP]
> Lorsque vous examinez de manière holistique les emplacements, les types de données et le nombre d’utilisateurs impliqués dans les correspondances de stratégie, vous pouvez avoir une meilleure idée des types de mesures de formation et de protection des données nécessaires pour aider votre organisation à sécuriser les données personnelles qu’elle stocke.

### <a name="matched-items-tab"></a>Onglet Éléments mis en correspondance

L’onglet **Éléments mis** en correspondance affiche une liste de tous les éléments de contenu correspondant à une condition définie dans la stratégie. Dans cette vue, vous pouvez sélectionner un élément à partir de sa ligne pour l’afficher en préversion dans la fenêtre à droite de la liste d’éléments.

Dans la fenêtre d’aperçu, vous trouverez les onglets suivants qui fournissent des détails sur chaque élément :
- **Source** : affiche les données personnelles qui ont déclenché la correspondance.
- Détails : affiche le propriétaire du contenu (utilisateur de votre organisation) pour l’élément, l’emplacement Microsoft 365 de l’élément, le nombre de types de données personnelles au sein de l’élément et les types de données **personnelles** spécifiques.
- **Activités de fichier** : affiche toute étiquette ou classification appliquée à l’élément.
- **Historique des corrections** : affiche des informations sur les actions de correction effectuées par les utilisateurs ou les administrateurs sur l’élément.

## <a name="edit-a-policy"></a>Modifier une stratégie

Vous pouvez modifier les paramètres d’une stratégie à tout moment, que ce soit en mode test ou activé. Vous pouvez mettre à jour la plupart des paramètres de stratégie, notamment remettre une stratégie en mode test après l’avoir activée. Les seuls paramètres que vous ne pouvez pas modifier sont le modèle de stratégie et le nom de la stratégie.

Pour modifier une stratégie, suivez les étapes ci-dessous :

1. Dans le [Centre de conformité Microsoft 365](https://compliance.microsoft.com/), recherchez Priva Privacy Risk Management dans le volet de navigation gauche. Dans le menu déroulant, sélectionnez **Stratégies**.

2. Sélectionnez la stratégie que vous souhaitez modifier à partir de sa ligne dans la page **Stratégies** , qui affiche la page de détails de cette stratégie.

3. Dans la page des détails de la stratégie, sélectionnez la commande **Modifier** dans le coin supérieur droit de la page. Cette action vous permettra de créer des stratégies dans Gestion des risques liés à la confidentialité.

4. Procédez comme suit pour accéder aux paramètres que vous souhaitez modifier. Vous pouvez modifier tous les paramètres à l’exception du modèle de stratégie et du nom de la stratégie. Sélectionnez **Suivant** pour passer à chaque étape suivante.

5. Dans la page **Terminer** , passez en revue vos paramètres, puis **sélectionnez Envoyer** pour enregistrer les modifications que vous avez apportées.

## <a name="delete-a-policy"></a>Suppression d’une stratégie

Si vous devez supprimer une stratégie de gestion des risques de confidentialité existante, recherchez-la dans la liste de la page **Stratégies** , sélectionnez le menu d’action (points de suspension verticaux), puis choisissez l’action **Supprimer la stratégie** . Vous pouvez également ouvrir la page de détails de la stratégie et sélectionner **Supprimer** dans le coin supérieur droit.

Vous serez invité à confirmer votre choix avant que la suppression soit définitive et que la stratégie soit définitivement supprimée. La suppression d’une stratégie n’affecte aucun fichier précédemment évalué par la stratégie, et les problèmes et alertes générés par la stratégie sont toujours répertoriés dans les pages **Alertes** et **problèmes** .

## <a name="next-steps"></a>Prochaines étapes

Une fois que votre stratégie est activée et commence à générer des alertes, vous devez commencer à comprendre les risques qu’elles peuvent présenter à votre organisation. Découvrez comment gérer les alertes, examiner les événements et prendre des mesures correctives dans la gestion des risques liés à la confidentialité en visitant [Examiner et corriger les alertes](risk-management-alerts.md).

## <a name="legal-disclaimer"></a>Exclusion de responsabilité légale

[Exclusion de responsabilité légale de Microsoft Priva](priva-disclaimer.md)
