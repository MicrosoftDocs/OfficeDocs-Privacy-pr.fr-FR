---
title: Envoyer des notifications utilisateur dans Gestion des risques liés à la confidentialité
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
description: Découvrez comment informer les propriétaires de contenu des correspondances de stratégie trouvées par Microsoft Priva Privacy Risk Management et comment ils peuvent utiliser ces notifications par e-mail pour résoudre les problèmes.
ms.openlocfilehash: 8969e1cd4d5859102b18bd46723d1be6e85d35f6
ms.sourcegitcommit: b5f7dcb73c0e3f677981e80106769cb546d00af4
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/21/2022
ms.locfileid: "65014374"
---
# <a name="user-notifications-in-privacy-risk-management"></a>Notifications utilisateur dans Gestion des risques liés à la confidentialité

Lorsque vous configurez une stratégie dans Privacy Risk Management, vous pouvez choisir d’avertir les utilisateurs lorsque leurs actions répondent aux conditions que vous avez définies dans la stratégie. Il existe deux types de notifications : les e-mails, qui sont disponibles pour les trois types de stratégie, et les conseils qui apparaissent dans Teams, qui sont disponibles uniquement pour le type de stratégie de transfert de données. Lorsque vous créez ou modifiez une stratégie, vous pouvez décider d’activer ces notifications, de leur fréquence d’envoi et de personnaliser leur contenu.

L’envoi de notifications aux utilisateurs peut être un composant important pour aider votre organisation à atteindre ses objectifs de confidentialité. Les notifications sont conçues pour :

- Sensibiliser immédiatement les utilisateurs quand leurs actions peuvent exposer des données personnelles à des risques de confidentialité.
- Fournissez des méthodes de correction directement dans les e-mails, afin que les utilisateurs puissent prendre des mesures rapides pour protéger les données à risque.
- Dirigez les utilisateurs vers les recommandations en matière de confidentialité et les meilleures pratiques de votre organisation.

Informer les utilisateurs des problèmes potentiels en ce moment et leur permettre de corriger les problèmes et d’actualiser leurs compétences peuvent être des outils puissants pour créer des pratiques de gestion des données solides au sein de votre organisation.

Passez en revue les sections ci-dessous pour vous aider à préparer et gérer les notifications utilisateur pour les correspondances de stratégie.

## <a name="prepare-training-content-for-notifications"></a>Préparer le contenu de la formation pour les notifications

Un lien vers la formation à la confidentialité est requis si vous choisissez d’envoyer des notifications utilisateur lorsque des correspondances de stratégie sont détectées. L’accès aux directives de confidentialité de votre organisation vous permet de tenir vos utilisateurs informés de vos propres bonnes pratiques et stratégies. Il peut également donner le contexte pour les actions de correction suggérées dans l’e-mail et aider vos utilisateurs à se préparer à de bonnes décisions de gestion des données à l’avenir.

Avant de configurer votre stratégie, choisissez l’URL d’entraînement que vous souhaitez inclure. Un lien peut être fourni par stratégie. Nous vous recommandons donc de choisir des références spécifiques à chaque scénario.

## <a name="set-user-email-notifications"></a>Définir les notifications par e-mail des utilisateurs

Vous pouvez configurer des notifications par e-mail pour tous les types de stratégies lorsque vous créez une stratégie ou modifiez une stratégie existante. Ces paramètres se trouvent dans la page **Résultats** de l’Assistant Création de stratégie. [Visitez Définir les résultats : notifications utilisateur et conseils](risk-management-policies.md#define-outcomes-user-email-notifications-and-tips) pour obtenir les instructions complètes.

> [!NOTE]
> La capacité globale de Privacy Risk Management à envoyer des notifications par e-mail est contrôlée dans Priva **Paramètres**. Elle est activée par défaut. La désactivation de ce paramètre arrête tous les e-mails même si les notifications ont été configurées au niveau d’une stratégie individuelle. En savoir plus sur [les paramètres d’e-mail de notification utilisateur](priva-settings.md#user-notification-emails).

## <a name="send-notifications-in-teams"></a>Envoyer des notifications dans Teams

Pour les stratégies de transfert de données, vous pouvez choisir aux utilisateurs de recevoir des conseils et des recommandations de stratégie dans des canaux Teams sécurisés lorsqu’une correspondance de stratégie est détectée. Ces conseils informent les utilisateurs sur l’utilisation responsable des données personnelles. Astuces inclut également des liens vers la formation associée.

Pour en savoir plus sur la configuration de ces notifications, consultez [Définir les résultats : notifications utilisateur et conseils](risk-management-policies.md#define-outcomes-user-email-notifications-and-tips).

## <a name="preview-and-customize-email-content"></a>Afficher un aperçu et personnaliser le contenu de l’e-mail

Lorsque les utilisateurs reçoivent des notifications par e-mail sur les correspondances de stratégie, ils peuvent suivre les invites dans les e-mails pour prendre immédiatement des mesures correctives. Par exemple, si une stratégie de surexposition de données trouve une correspondance pour des données personnelles qui peuvent être trop largement accessibles, l’e-mail de notification inclut un lien vers l’élément de contenu afin que l’utilisateur puisse le consulter, ainsi que des boutons permettant à l’utilisateur de marquer l’élément comme privé ou de conserver son niveau d’accès actuel. Les actions suggérées seront pertinentes pour chaque type de stratégie.

Vous pouvez afficher un aperçu du contenu de l’e-mail et apporter vos propres modifications lors de l’ajustement de ce paramètre dans le processus de création ou de modification de la stratégie. Pour afficher un aperçu et modifier le contenu de votre e-mail de notification, suivez les étapes ci-dessous :

1. Créez ou modifiez votre stratégie en démarrant les étapes décrites dans le [processus de création de stratégie guidé](risk-management-policies.md#custom-setup-guided-process-to-choose-all-settings).

2. À l’étape **Résultats** du processus, sélectionnez la zone en regard **d’Envoyer un e-mail de notification aux utilisateurs lorsqu’une correspondance de stratégie se produit**.

3. Sélectionnez le bouton **Aperçu et modifier l’e-mail de notification** qui apparaît sous la case à cocher de l’e-mail de notification.

4. Un volet de menu volant s’affiche avec des champs de texte préremplis avec le contenu de messagerie par défaut. Vous pouvez modifier n’importe quel ou tous les champs, y compris : la ligne d’objet de l’e-mail, l’en-tête de corps, le contenu du corps, le nom complet de la formation à la confidentialité et l’URL d’entraînement. L’aperçu de l’e-mail se trouve en bas du volet de menu volant, et il change à mesure que vous apportez des modifications au texte par défaut. Lorsque vous êtes satisfait du contenu de l’e-mail, **sélectionnez Enregistrer** pour enregistrer vos paramètres. Pour ignorer les modifications apportées à l’e-mail par défaut, sélectionnez le **X** dans le coin supérieur droit du volet volant pour le fermer et revenir au contenu par défaut.

5. De retour sur la page **Résultats** , sélectionnez **Suivant**. Passez en revue l’Assistant et, lorsque vous arrivez à la page **de fin** finale, passez en revue vos paramètres et **sélectionnez Envoyer**.

Vos paramètres de notification sont désormais en vigueur pour cette stratégie. Si votre stratégie est en test, les notifications ne seront pas envoyées. Si votre stratégie est activée, des notifications sont envoyées. Afficher plus de détails sur [la création et la gestion des stratégies](risk-management-policies.md).


## <a name="legal-disclaimer"></a>Exclusion de responsabilité légale

[Exclusion de responsabilité légale de Microsoft Priva](priva-disclaimer.md)
