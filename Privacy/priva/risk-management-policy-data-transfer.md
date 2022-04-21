---
title: Stratégies de transfert de données dans la gestion des risques liés à la confidentialité
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
description: Découvrez comment créer une stratégie de gestion des données dans Microsoft Priva Privacy Risk Management pour endiguer les transferts de données personnelles au sein ou en dehors de votre organisation.
ms.openlocfilehash: 6d491a7a65035aa1e3a405f36ef30b95f9c29245
ms.sourcegitcommit: b5f7dcb73c0e3f677981e80106769cb546d00af4
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/21/2022
ms.locfileid: "65014483"
---
# <a name="data-transfer-policies-in-privacy-risk-management"></a>Stratégies de transfert de données dans la gestion des risques liés à la confidentialité

## <a name="whats-new"></a>Nouveautés
Les stratégies de transfert de données peuvent désormais détecter quand les éléments contenant des données personnelles sont transférés en dehors de votre organisation. Les transferts externes sont le scénario de transfert par défaut lorsque vous créez une stratégie de transfert de données à l’aide de [l’option de configuration rapide](#quick-setup-use-a-template-with-default-settings). Cela n’impactera pas ou ne modifiera pas les paramètres des stratégies de transfert de données que vous avez déjà créées.

## <a name="overview"></a>Présentation

Le transfert de données personnelles présente des risques, en particulier lorsqu’ils sont transférés en dehors de votre organisation ou envoyés entre certains services ou emplacements géographiques au sein de votre organisation. Par exemple, si les données sont envoyées via des e-mails non chiffrés ou à des destinataires non autorisés, les données peuvent ne plus être sécurisées. Les activités de transfert de données comme celles-ci peuvent avoir un impact réglementaire ou violer les pratiques de confidentialité de l’organisation établies.

Les stratégies de transfert de données dans Privacy Risk Management vous permettent de surveiller les transferts de données personnelles en dehors de votre organisation, ainsi que les transferts internes entre différents services ou pays ou régions. Lorsqu’une correspondance de stratégie est détectée, vous pouvez envoyer des notifications par e-mail aux utilisateurs qui leur permettent d’effectuer des actions correctives directement dans l’e-mail, comme rendre les éléments de contenu privés, informer les propriétaires de contenu ou marquer des éléments pour une révision ultérieure.

Notre processus de configuration de stratégie facilite la définition des conditions de stratégie. Vous disposez d’un contrôle total sur le minutage des alertes et la fréquence des e-mails et des conseils en cours dans Microsoft Teams qui portent l’attention des utilisateurs sur les pratiques de gestion des données sécurisées.

Il existe deux façons de créer une stratégie : à partir d’un **modèle**, qui est notre option rapide « out-of-box » à l’aide des paramètres par défaut ; ou l’option **personnalisée** , qui est un processus guidé pour définir les conditions, les alertes et les notifications.

## <a name="quick-setup-use-a-template-with-default-settings"></a>Configuration rapide : utiliser un modèle avec les paramètres par défaut

La stratégie de transfert de données par défaut détecte quand des données personnelles sont envoyées à des destinataires en dehors de votre organisation. Par exemple, il apparaît lorsqu’un utilisateur de votre organisation envoie un e-mail Exchange à un destinataire externe dans les champs **À**, **Cc** ou **Cci**.

Procédez comme suit pour créer une stratégie de transfert de données par défaut :

1. Dans le [Centre de conformité Microsoft 365](https://compliance.microsoft.com/), recherchez Priva Privacy Risk Management dans le volet de navigation de gauche et sélectionnez **Stratégies**.

2. Sélectionnez **Créer une stratégie** dans le coin supérieur droit de l’écran, qui affiche un volet volant répertoriant toutes les options de création de stratégie.

3. Dans la zone **Transferts de données** , sélectionnez **Créer**.

4. Un volet volant contient les détails de la stratégie. La sélection des **paramètres d’affichage** affiche les [paramètres par défaut](#default-data-transfer-policy-settings). Vous pouvez modifier les paramètres à partir d’ici, ce qui vous permet d’accéder au processus guidé décrit ci-dessous. Pour continuer à créer votre stratégie à l’aide des paramètres par défaut, entrez simplement un nom descriptif, puis **sélectionnez Créer une stratégie**.

Votre stratégie sera créée et vous la trouverez dans votre page **Polices** . Il commence en [mode test](risk-management-policies.md#testing-a-policy) pour vous permettre de surveiller ses performances avant de l’activer.

#### <a name="default-data-transfer-policy-settings"></a>Paramètres de stratégie de transfert de données par défaut

Une stratégie de transfert de données créée à partir du modèle détecte :
- Lorsque des données personnelles au sein de votre organisation sont transférées ou partagées avec un destinataire ou un emplacement en dehors de votre organisation.
- Lorsque des données personnelles sont partagées en externe à partir de l’un de ces emplacements au sein de votre organisation :
    - **Exchange**. Exemple : envoi d’un e-mail contenant des données personnelles à une adresse e-mail de destinataire en dehors de votre organisation.
    - **OneDrive** et **SharePoint**. Exemples : envoi d’un lien vers un fichier ou un site qui contient des données personnelles à une personne externe à votre organisation ; copie ou déplacement d’un fichier vers un emplacement OneDrive ou SharePoint situé en dehors de votre organisation.
    - **Teams**. Exemple : envoi d’un message de conversation Teams contenant des données personnelles à un destinataire en dehors de votre organisation.
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

Effectuez les étapes ci-dessous pour créer une stratégie de transfert de données :

1. Dans le [Centre de conformité Microsoft 365](https://compliance.microsoft.com/), recherchez Priva Privacy Risk Management dans le volet de navigation de gauche et sélectionnez **Stratégies**.

2. Sélectionnez le bouton **Créer une stratégie** en haut à droite de votre écran, qui affiche un volet volant répertoriant toutes les options de création de stratégie.

3. Dans la zone **Personnalisée** , sélectionnez **Créer**.

4. Dans la page **Nom et type** , sélectionnez le modèle de stratégie **de transfert de données** . Entrez un nom de stratégie qui vous aidera à l’identifier facilement à partir de votre liste sur la page **Stratégies** , puis entrez une description facultative, puis sélectionnez **Suivant**.

5. Dans la page **Données à surveiller** , choisissez le type de données personnelles que votre stratégie doit surveiller. Il existe deux options :
    - **Groupes de classification** : regroupements de types d’informations sensibles utilisés pour détecter du contenu lié à des données personnelles ou à des réglementations spécifiques. Si vous sélectionnez cette option, vous devez sélectionner **+Ajouter des groupes de classification** pour choisir un ou plusieurs groupes dans la liste fournie.
    - **Types d’informations sensibles individuels** : sélectionnez cette option pour choisir parmi une liste de [types d’informations sensibles individuels](/microsoft-365/compliance/sensitive-information-type-entity-definitions).

    En savoir plus sur [le choix des données à surveiller](risk-management-policies.md#choose-data-to-monitor). Lorsque vous avez terminé de sélectionner les données à surveiller, sélectionnez **Suivant**.

6. Dans la page **Utilisateurs et groupes** , choisissez les utilisateurs de votre organisation auxquels la stratégie s’appliquera. Vous pouvez sélectionner tous les utilisateurs individuels et tous les groupes de distribution Office 365, ou vous pouvez sélectionner des utilisateurs et des groupes spécifiques. En savoir plus sur [le choix des utilisateurs et des groupes](risk-management-policies.md#choose-users-and-groups). Lorsque vous avez terminé, sélectionnez **Suivant**.

7. Dans la page **Emplacements**, sélectionnez tous les emplacements de données dans Microsoft 365 que vous souhaitez que la stratégie couvre. Choisissez parmi Exchange comptes de messagerie, comptes OneDrive, Teams messages de conversation et de canal, ainsi que des sites SharePoint.

    Dans SharePoint vous pouvez désigner tous les sites ou sites spécifiques. Si vous sélectionnez **Des sites spécifiques SharePoint**, vous pouvez entrer l’URL du site dans le champ URL. Vous pouvez également sélectionner **+Choisir des sites**, puis, dans le volet volant, cochez la case à gauche du nom du site que vous souhaitez sélectionner.

    En savoir plus sur [le choix des emplacements](risk-management-policies.md#choose-locations). Lorsque vous avez terminé de sélectionner des emplacements, sélectionnez **Suivant**.

8. Dans la page **Conditions** , sélectionnez le type de condition de transfert de données détecté par la stratégie :
    - **Transferts en dehors de votre organisation** : détecte les transferts d’utilisateurs ou de groupes au sein de votre organisation vers des utilisateurs externes ou invités en dehors de votre organisation.
    - **Transferts entre les services de votre organisation** : pour cette option, vous allez sélectionner un service expéditeur et un service de destinataire. Choisissez des départements dans les listes des volets volants qui s’affichent, puis sélectionnez **Ajouter**.
    - **Transferts entre les limites ou les régions du pays** : pour cette option, vous allez sélectionner une région d’expéditeur et une région de destinataire. Choisissez vos pays ou régions désignés dans les volets volants qui s’affichent, puis sélectionnez **Ajouter**.

9. Dans la page Résultats, décidez s’il faut informer les utilisateurs lorsqu’ils correspondent aux conditions **définies** par la stratégie. Vous pouvez choisir l’une des options suivantes ou les deux, ou ne choisir ni l’une ni l’autre en laissant les cases à cocher vides :
    - **Astuces envoyés dans Microsoft Teams** : les conseils de gestion des données s’affichent dans l’instance de Teams d’un utilisateur lorsqu’il a effectué une action qui correspond aux conditions de la stratégie. Vous devez ajouter une URL pour votre formation de confidentialité préférée, qui apparaîtra également dans l’info-bulle.
    - **Notifications par e-mail** : les utilisateurs reçoivent une notification par e-mail lorsque leurs actions correspondent aux conditions de stratégie. Les e-mails contiennent des instructions pour prendre des mesures de correction directement à partir de l’e-mail, ainsi qu’un lien vers la formation à la confidentialité. Vous allez désigner la fréquence des e-mails et l’URL de votre formation de confidentialité préférée.
     
    En savoir plus sur la configuration [des notifications utilisateur](risk-management-notifications.md). Lorsque vous avez terminé de sélectionner les résultats, sélectionnez **Suivant**.

10. Dans la page **Alertes** , utilisez le bouton bascule pour activer les alertes qu’un administrateur verra sur la page **Alertes** dans la section **Stratégies** de la gestion des risques de confidentialité. Vous allez indiquer la fréquence à laquelle les alertes sont générées, les seuils de correspondance avant la génération des alertes et la gravité des alertes. En savoir plus sur [la définition d’alertes pour les correspondances de stratégie](risk-management-policies.md#set-alerts). Lorsque vous avez terminé, sélectionnez **Suivant**.

11. Dans la page **Mode** , déterminez si vous souhaitez ou non exécuter votre stratégie en mode test lorsque vous la créez pour la première fois, ce qui signifie qu’aucune alerte ou notification n’est envoyée. Pour conserver votre stratégie en mode test, ce que nous vous recommandons, sélectionnez le commutateur bascule vers la position **Activé** . En savoir plus sur le [test d’une stratégie](risk-management-policies.md#testing-a-policy).

> [!NOTE]
> Si vous **basculez l’option Exécuter en mode test** vers la position **Désactivée** , *votre stratégie s’active* lorsque vous avez terminé de la créer. Cela signifie que toutes les alertes ou notifications utilisateur que vous avez configurées commencent à générer une fois qu’une correspondance est détectée.

12. Dans la page **Terminer** , passez en revue vos choix. Sélectionnez **Modifier** sous l’une des sections pour ajuster les paramètres. Lorsque vous êtes satisfait des paramètres de votre stratégie, sélectionnez **Envoyer** pour créer la stratégie.

Après quelques secondes, vous verrez une confirmation que la stratégie a été créée. Sélectionnez **Terminé** dans la page de confirmation, qui vous amène à la page **Stratégies** où vous verrez la nouvelle stratégie en haut du tableau.

## <a name="next-steps"></a>Prochaines étapes

Pour plus d’informations sur la modification et la gestion des stratégies, consultez [les stratégies de gestion des risques de confidentialité](risk-management-policies.md) .
