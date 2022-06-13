---
title: Créer une demande et définir des paramètres de recherche dans les demandes de droits d’objet
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
description: Découvrez comment créer une demande de droits d’objet et définir des paramètres de recherche dans Demandes de droits des personnes concernées Microsoft Priva.
ms.openlocfilehash: 7314fefa370b24bcb215a99b67b74c13b8b27613
ms.sourcegitcommit: 3c83e8133a5a71f4e1d76a0b2981ab3ec9cd6602
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/13/2022
ms.locfileid: "66046638"
---
# <a name="create-a-request-and-define-search-settings"></a>Créer une demande et définir des paramètres de recherche

**Dans cet article** : Découvrez comment créer une demande dans Priva pour commencer à traiter une demande de droits d’objet. Comprendre les paramètres de recherche pour la récupération des données et comment affiner votre recherche.

Les utilisateurs qui détiennent un rôle dans le groupe de rôles Administrateurs de demande de droits d’objet autre que l’affichage uniquement ([voir Priva autorisations](priva-permissions.md)) peuvent créer une demande dans les demandes de droits d’objet. Un processus guidé vous guide tout au long des paramètres de recherche de données personnelles sur une personne concernée et de démarrage du processus de traitement de sa demande.

## <a name="request-types"></a>Types de demandes

Demandes de droits des personnes concernées Priva prend en charge trois types de demandes différents :

1. **Accès** : fournit un résumé des informations personnelles de la personne concernée détenues par votre organisation dans Microsoft 365.

2. **Exportation** : fournit un résumé et un fichier exporté d’éléments de contenu qui contiennent les informations personnelles de la personne concernée. Il s’agit des éléments examinés et marqués comme **inclus** lors de votre examen des données collectées par vos paramètres de recherche.

3. **Liste balisé pour le suivi** : génère un résumé de tous les fichiers qui ont été marqués lors de l’examen des données qui peuvent nécessiter une action supplémentaire en dehors de Priva. Par exemple, vous devrez peut-être faciliter la suppression des informations personnelles de la personne concernée en fonction de sa demande. Vous pouvez afficher les balises incluses et configurer des balises personnalisées pour votre organisation dans [Priva paramètres](priva-settings.md).

## <a name="getting-started-with-your-first-request"></a>Bien démarrer avec votre première demande

Lorsque vous démarrez une version d’évaluation ou un abonnement de demandes de droits d’objet, nous proposons une configuration simple et prêt à l’emploi pour votre première demande qui utilise les paramètres par défaut. Cette configuration peut vous aider à explorer le flux de travail des demandes de droits d’objet et à vous familiariser avec ses fonctionnalités.

La première fois que vous accédez à la page Demandes de droits des personnes concernées, une bannière apparaît en haut avec un bouton **Démarrage**. Lorsqu’un utilisateur sélectionne ce bouton, un volet volant s’affiche avec les informations de cet utilisateur préremplies dans les champs de nom et d’e-mail, et affiche tous les paramètres par défaut.

**Exploration des fonctionnalités de demande avec vos informations** : l’essai d’une demande de droits d’objet basée sur vos propres informations peut vous aider à vous familiariser et à vous familiariser avec le passage à chaque étape du processus. Vous verrez ce qu’une recherche par défaut génère et pouvez vous entraîner à affiner les résultats en ajustant les paramètres de recherche. Sous l’onglet **Données collectées** , vous pouvez passer en revue les éléments de la zone d’aperçu à droite et appliquer du texte, appliquer des balises, entrer des notes et marquer des éléments à inclure ou exclure pour le rapport final (pour plus d’informations sur les données de révision [d’une demande de droits d’objet](subject-rights-requests-data-review.md)).

- Vous n’avez pas besoin d’utiliser vos informations pour créer votre première demande. Si vous êtes prêt à démarrer une demande pour un sujet de données, remplacez votre nom et votre adresse e-mail par les informations de la personne concernée.

Pour accepter tous les paramètres et créer la demande, sélectionnez **Créer**. Le volet se ferme et vous voyez votre nouvelle demande répertoriée dans votre page **Demandes de droits** d’objet. Pour modifier l’un des paramètres par défaut avant de créer la demande, sélectionnez **Modifier les détails** de la demande, ce qui vous place dans l’Assistant [de création de la demande de droits d’objet](#create-a-request).

> [!NOTE]
> Toutes les demandes que vous créez sont comptabilisées dans votre allocation d’abonnement payant ou d’évaluation, quelles que soient les informations de la personne concernée utilisées pour la demande. La période de conservation des données standard de 30 jours s’applique après la fermeture de la demande. Découvrez comment modifier [les périodes de rétention pour les demandes de droits d’objet](subject-rights-requests-reports.md#retention-periods-for-reports-and-data).

## <a name="create-a-request"></a>Créer une demande

Suivez les étapes ci-dessous pour commencer à répondre à une demande de droits d’objet :

1. Dans le [portail de conformité Microsoft Purview](https://compliance.microsoft.com/), sélectionnez **Demandes de droits des personnes concernées Priva** dans le volet de navigation de gauche.

2. Dans le coin supérieur droit de l’écran, **sélectionnez Créer une requête**.

3. Dans la page **d’informations sur l’objet de** données, entrez le prénom et le nom et l’adresse e-mail de la personne concernée. Sélectionnez **Ajouter une résidence** pour choisir le pays de résidence de la personne concernée. Sélectionnez l’option qui identifie la façon dont la personne concernée est liée à votre organisation (par exemple, le client ou l’employé actuel), puis sélectionnez **Suivant** pour passer à l’étape suivante.

4. Dans la page **Emplacements** , choisissez l’emplacement où vous souhaitez rechercher les informations de la personne concernée. Choisissez l’un des emplacements suivants ou les deux en déplaçant le commutateur bascule d’état en regard de chaque option vers la position **On** :

   - **Exchange** : recherchez des données dans des boîtes aux lettres Exchange et dans des conversations Teams individuelles ou de groupe. Vous pouvez choisir de rechercher tous les comptes Exchange de votre organisation, ou de sélectionner **des comptes** pour sélectionner des utilisateurs individuels dans le volet volant **Exchange boîtes aux lettres**.

   - **SharePoint** : recherchez des données dans des sites SharePoint, des sites OneDrive Entreprise et des canaux Teams. Vous pouvez choisir de rechercher tous les sites SharePoint de votre organisation, ou sélectionner **Choisir des sites** pour sélectionner des utilisateurs individuels dans le volet volant **SharePoint sites**.

> [!TIP]
> Pour obtenir de l’aide sur l’identification des termes de recherche appropriés, reportez-vous aux rubriques suivantes :
> - SharePoint sites et URL : [La gestion des sites dans le centre d’administration SharePoint](/sharepoint/manage-sites-in-new-admin-center) fournit des conseils sur le tri et le filtrage des sites, ainsi que sur la recherche d’un site SharePoint. Utilisez cette option pour rechercher des URL à entrer dans le champ de recherche dans le volet de menu volant **SharePoint sites**.
> - Teams conversations et canaux : [Get-Team](/powershell/module/teams/get-team) montre comment trouver des équipes dans Microsoft Teams en fournissant des propriétés ou des informations spécifiques.
> - OneDrive sites et URL : [À propos des URL OneDrive](/onedrive/list-onedrive-urls#about-onedrive-urls) fournit des informations sur le format et les propriétés appropriés pour l’URL OneDrive d’un utilisateur. Utilisez-la pour vous aider à identifier OneDrive sites dans votre recherche.

5. Dans la page **Définir les paramètres de recherche** , vous pouvez choisir d’apporter des modifications à la recherche par défaut en choisissant parmi les différentes options de recherche avancées. C’est ici que vous pouvez également choisir d’obtenir une estimation avant que les données ne sont retournées automatiquement. Si vous choisissez l’une de ces options, lorsque vous sélectionnez **Suivant** , vous passez à des écrans supplémentaires. Pour plus d’informations, consultez [Définir les paramètres de recherche ci-dessous](#defining-search-settings) . Si vous ne souhaitez pas modifier votre recherche, laissez toutes les options vides et sélectionnez **Suivant** pour passer à l’étape suivante.

6. Dans la page **Sélectionner le type de demande** , choisissez le type de demande : **Access**, **Export** ou **Tagged list pour le suivi** ([voir les descriptions ci-dessus](#request-types)). Indiquez si la demande concerne un règlement sur la confidentialité des données. Passez en revue ou apportez des modifications à l’échéance d’achèvement, qui est par défaut de deux semaines après la date de création de la demande. Ensuite, sélectionnez **Suivant**.

7. Dans la page **Confirmer ou modifier le nom de cette demande** , vous pouvez conserver ou modifier le nom convivial fourni pour la demande, puis entrer une description facultative. Ensuite, sélectionnez **Suivant**.

8. Dans la page **Révision et fin** , passez en revue le résumé de ce que vous avez entré au cours des étapes précédentes. N’importe quel champ peut être modifié en sélectionnant le **lien Modifier** dans chaque section. Lorsque vous avez terminé, **sélectionnez Créer une requête**.

Un écran de confirmation s’affiche une fois la demande créée. Sélectionnez **Terminé** pour revenir à l’écran principal demandes de droits d’objet. La nouvelle demande est répertoriée en haut de votre liste de demandes. Sélectionnez-la dans la liste pour commencer à examiner et à parcourir les étapes de progression.

#### <a name="what-happens-after-your-request-is-created"></a>Que se passe-t-il après la création de votre demande ?

Nous allons calculer une estimation de la quantité de données qu’il s’attend à trouver en fonction de vos paramètres de recherche commence immédiatement. Visitez la page de détails de votre demande en quelques minutes à une heure pour voir les résultats de l’estimation et si la demande est passée à l’étape suivante. Votre demande passe automatiquement de **l’estimation des données** à la **récupération des données** , sauf dans les circonstances suivantes :

 - Si vous avez choisi de recevoir un esimtae de données en premier à l’étape 5, **Définissez les paramètres de recherche**, vous pourrez afficher les détails de votre recherche et apporter des modifications à votre recherche avant que toutes les données ne soient récupérées. Vous devez passer manuellement à l’étape suivante de **la récupération des données** si vous avez mis en pause l’estimation **des données**.
 
 - Si vous n’avez pas choisi de vous arrêter à l’estimation des données, mais que nous prévoyons que votre recherche générera un grand volume de données, vous verrez une barre de messages en haut de votre demande avec un lien pour modifier votre recherche avant de passer à la **récupération des données**.

Visitez [l’estimation et la récupération des données](subject-rights-requests-data-retrieval.md)pour en savoir plus sur ces étapes.

## <a name="defining-search-settings"></a>Définition des paramètres de recherche

Lorsque vous créez une demande de droits d’objet, une recherche par défaut s’exécute en fonction de vos sélections sur la page **Emplacements** de l’Assistant création. Si vous souhaitez effectuer une recherche plus ciblée ou si vous souhaitez choisir d’obtenir une estimation de vos données avant la récupération des éléments de contenu, vous pouvez effectuer ces sélections dans la page **Paramètres de recherche** de l’Assistant Création de demande.

### <a name="advanced-search-options"></a>Options de recherche avancées

- **Affiner votre recherche** : cette option vous permet de spécifier des propriétés supplémentaires pour aider à identifier la personne concernée parmi les données de votre organisation. Après avoir choisi cette option, vous êtes invité à ajouter d’autres paramètres de recherche, comme expliqué ci-dessous dans [Affiner votre recherche](#refining-your-search).
- **Inclure le contenu créé par l’objet de données** : cette option recherche le contenu qui a été créé par la personne concernée. Par exemple, les fichiers créés par la personne concernée ou chargés vers SharePoint par. La sélection de cette option peut augmenter considérablement la quantité de données retournées.
- **Inclure toutes les versions d’éléments** : si vous avez sélectionné SharePoint comme emplacement de recherche, la requête de recherche par défaut renvoie uniquement la version actuelle des éléments SharePoint. Cette case à cocher renvoie les versions actuelles et toutes les versions précédentes des éléments SharePoint, ce qui génère une quantité de données beaucoup plus importante à examiner.

> [!TIP]
> Vous pouvez choisir de charger du matériel supplémentaire pour permettre à Priva d’identifier les personnes concernées en fonction des valeurs de données exactes. Pour plus d’informations, consultez [La correspondance des données pour les demandes de droits des personnes concernées](subject-rights-requests-data-match.md).

### <a name="data-estimate"></a>Estimation des données

La **première option Obtenir une estimation** présente une estimation de la quantité de données que nous nous attendons à trouver avant que vos données ne sont récupérées automatiquement. Lorsque votre estimation est affichée sur la page de détails de la demande, vous pouvez choisir d’afficher les résultats de la recherche et d’afficher un aperçu d’un échantillon d’éléments qui ont été découverts. Si les éléments représentent les résultats attendus, vous devez sélectionner **Récupérer les données** afin de poursuivre la récupération réelle des éléments de contenu. Obtenez plus de détails sur la [phase d’estimation des données](subject-rights-requests-data-retrieval.md).

## <a name="refining-your-search"></a>Affiner votre recherche

Si vous choisissez **Affiner votre recherche** sur la page **Paramètres** de recherche, ou si vous avez suspendu à l’étape d’estimation des **données** et que vous choisissez de modifier votre requête de recherche, vous êtes invité à fournir des détails sur les attributs personnels et les conditions afin de cibler davantage vos résultats de recherche. Vous pouvez effectuer des ajouts dans l’une ou l’autre des catégories ou dans les deux catégories. Lorsque vous avez terminé d’effectuer des sélections dans cette section, la récupération des données pour la demande est basée sur vos paramètres de recherche.

Les détails décrits ci-dessous sont également ce que vous serez invité à fournir si vous avez suspendu à l’étape **d’estimation des données** et que vous choisissez de modifier votre requête de recherche. 

#### <a name="add-personal-attributes"></a>Ajouter des attributs personnels

Entrez des valeurs dans les champs de texte pour les noms, surnoms, adresses e-mail et adresses de la personne concernée. Vous pouvez ajouter d’autres identificateurs tels que la date de naissance ou le numéro de téléphone, et les champs de texte prennent en charge plusieurs entrées séparées par un point-virgule. Lorsque vous avez terminé, sélectionnez **Suivant** pour passer à la page **Conditions** .

#### <a name="conditions"></a>Conditions

Sélectionnez le bouton **Ajouter une condition** pour choisir parmi une plage de conditions pour cibler davantage votre recherche, notamment le nom de l’élément, les noms d’expéditeur et de destinataire, le type de données personnelles, et si l’élément a été partagé en externe à l’extérieur de votre organisation. Les champs de texte prennent en charge plusieurs entrées séparées par un point-virgule. Lorsque vous avez terminé, sélectionnez **Suivant** pour enregistrer vos paramètres de recherche et la progression vers le paramètre de type de requête.

## <a name="next-steps"></a>Étapes suivantes

Une fois que vous avez créé votre demande, elle apparaît dans la page de votre demande de droits d’objet. Pour en savoir plus sur la procédure de révision, consultez [Vérifier les données et collaborer sur les demandes](subject-rights-requests-data-review.md).

## <a name="legal-disclaimer"></a>Exclusion de responsabilité légale

[Microsoft Priva exclusion de responsabilité légale](priva-disclaimer.md)
