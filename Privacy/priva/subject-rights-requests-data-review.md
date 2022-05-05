---
title: Examiner les données d’une demande de droits d’objet
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
description: Découvrez comment examiner les données de demande de droits d’objet collectées par Microsoft Priva et collaborer à la réalisation de la demande.
ms.openlocfilehash: 3a1211d391ee196ad431fe19ab9134386c9803a4
ms.sourcegitcommit: 6b88d22d0250cbb9a4ba1f71665f29cb67939851
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65059758"
---
# <a name="review-data-for-a-subject-rights-request"></a>Examiner les données d’une demande de droits d’objet

Après avoir créé une demande de droits d’objet ([en savoir plus](subject-rights-requests-create.md)) dans Microsoft Priva, la solution Demandes de droits d’objet utilise vos entrées pour rechercher des correspondances sur votre sujet de données dans l’environnement Microsoft 365 de votre organisation. Une fois que ces données ont été compilées, vous pouvez examiner les résultats, faire des choix sur ce qu’il faut inclure et répéter des informations si nécessaire. Ces étapes peuvent être collaborées par plusieurs utilisateurs via l’interface Priva.

## <a name="step-1-review-request-details-and-monitor-progress"></a>Étape 1 : Examiner les détails de la demande et surveiller la progression

Pour afficher les résultats initiaux de votre recherche, accédez à la zone Priva du [portail de conformité Microsoft Purview](https://compliance.microsoft.com/) et **ouvrez les demandes de droits** d’objet. Vous trouverez la liste de toutes les demandes de droits d’objet ouvertes sur cette page principale.

Sélectionnez votre demande dans la liste pour afficher les détails de la demande. Ici, vous pouvez en savoir plus sur les propriétés de la demande, les résultats de la recherche et l’état de la demande. Cette page deviendra votre hub pour travailler et collaborer sur la gestion des fichiers trouvés, la création de rapports et d’exportations et la réalisation de la demande.

L’onglet **Vue d’ensemble** de la page détails de votre demande fournit des détails sur la demande, un indicateur de progression montrant votre étape actuelle et des informations clés sur les données trouvées. Les vignettes de cette page sont les suivantes :

##### <a name="details"></a>Détails

La carte **Détails affiche des** informations de base pour vous orienter vers la demande, telles que l’échéance, la date de création, la description et la réglementation en matière de confidentialité liées à la demande.

##### <a name="progress"></a>Progression

La carte **progression** répertorie chaque étape du processus : Estimation des données, Récupération des données, Examiner les données, Générer des rapports et Fermer la demande. Un cercle bleu rempli en regard de l’étape indique l’étape sur laquelle vous êtes actuellement. Une coche dans le cercle bleu signifie que l’étape est terminée, et le cercle non rempli signifie que l’étape n’a pas encore démarré.

##### <a name="total-number-of-items-found"></a>Nombre total d’éléments trouvés

Statistiques sur votre phase de progression actuelle. Cette vignette peut afficher des informations telles qu’un résumé de l’estimation des données, le nombre d’éléments trouvés dans votre recherche et leurs emplacements dans Microsoft 365, ou l’état de vos exportations.

##### <a name="priority-items-to-review"></a>Éléments de priorité à examiner

La vignette **Éléments de priorité à examiner** affiche les éléments que vous souhaiterez peut-être hiérarchiser au démarrage de votre révision. La vignette affiche un nombre d’éléments appartenant aux catégories suivantes :
- **Confidentiel** : il s’agit d’éléments auxquels une [étiquette de confidentialité Microsoft](/microsoft-365/compliance/sensitivity-labels) est appliquée. Par exemple, un document Word avec une étiquette « Hautement confidentiel ». 
- **Données multi-personnes** : ces éléments contiennent les données personnelles de plusieurs personnes. Si vous souhaitez inclure ces éléments dans le package de données final, vous devez rétablir les données non pertinentes dans les fichiers. Consultez [l’étape 3 : Passez en revue les données](#step-3-review-data) ci-dessous pour plus d’informations. Notez que pour que Priva identifie les éléments contenant des données multi-personnes, votre organisation doit configurer la [correspondance des données pour les demandes de droits d’objet](subject-rights-requests-data-match.md).

**Comment localiser vos éléments prioritaires :**

Tout d’abord, vérifiez que vous avez activé votre vue de ces éléments dans votre table d’éléments **collectées** par les données en suivant les étapes ci-dessous :

- Sous l’onglet **Données collectées** , sélectionnez **Personnaliser les colonnes** en haut de la liste des éléments.
- Dans le volet volant **Modifier les colonnes** , placez une vérification en regard des **types De priorité**.
- Sélectionnez **Appliquer**. Votre liste d’éléments aura désormais une colonne **de types De priorité** .

Vous pouvez maintenant identifier les éléments de priorité et les trouver en triant la colonne **de type Priority** pour regrouper des types similaires.

### <a name="understand-progress-stages"></a>Comprendre les étapes de progression

Les demandes de droits d’objet passent par plusieurs étapes. Certains états progressent automatiquement et d’autres étapes avancent lorsque les administrateurs et les contributeurs de demandes de droits d’objet effectuent des étapes essentielles telles que l’examen des fichiers.

Étant donné que les demandes peuvent avoir besoin d’être travaillées au fil du temps ou par plusieurs contributeurs, Priva fournit des mises à jour continues sur l’état et des conseils sur les prochaines étapes à suivre. Ces mises à jour peuvent être affichées sous l’onglet **Vue d’ensemble** de la page de détails d’une demande de droits d’objet.

#### <a name="data-estimate"></a>Estimation des données
Une fois que vous avez créé une demande, Priva commence immédiatement à rechercher des correspondances potentielles avec la personne concernée dans votre environnement Microsoft 365. Une fois que nous avons identifié tous les éléments que nous pensons correspondre à vos critères, vous verrez l’estimation dans la carte **de résumé de l’estimation des données** dans la page **Vue d’ensemble** de la demande. La quantité de données dans l’étendue de votre recherche affecte la durée nécessaire pour terminer l’estimation.

Votre demande passe automatiquement à l’étape suivante de la récupération des données, où tous les éléments de contenu sont regroupés afin que les parties prenantes puissent collaborer sur la révision des données. Dans certains cas, nous suspendons l’estimation des données avant de passer à la récupération et vous informons des prochaines étapes à suivre avant de continuer.

Vous pouvez également choisir de suspendre automatiquement à l’étape de l’estimation des données lorsque vous créez pour la première fois une demande de droits d’objet. Pendant le processus de création, **sélectionnez la première option Obtenir une estimation** pendant l’étape **Des paramètres de** recherche. Passez en revue les détails de [l’étape des paramètres de recherche](subject-rights-requests-create.md#define-search-settings).

#### <a name="pause-in-data-estimate-for-large-search-results"></a>Suspendre l’estimation des données pour les résultats de recherche volumineux

Priva remarquera si votre estimation des données est prévue pour retourner un grand nombre d’éléments à examiner (plus de 10 000 éléments). L’estimation s’interrompt afin que vous puissiez afficher un aperçu des résultats et décider s’il faut [modifier votre requête de recherche](subject-rights-requests-create.md#refine-your-search) pour cibler des emplacements ou des conditions plus spécifiques, ou continuer à récupérer les éléments identifiés.  Nous allons vous montrer à l’écran le nombre d’éléments et le volume de données correspondant à votre recherche. Vous disposez d’une ou des deux options suivantes dans une barre de messages en haut de votre écran :

- Un bouton **Modifier la requête de recherche** vous permet d’accéder directement aux paramètres de recherche de la requête pour définir des paramètres plus stricts et générer une nouvelle estimation.
- Tant que votre requête de recherche ne dépasse pas 300 000 éléments, vous verrez également une option pour **récupérer des données**. Cela vous permet de choisir de ne pas modifier votre recherche et de continuer à collecter les données.

#### <a name="retrieve-data"></a>Récupérer des données
L’étape de récupération des données est celle où tous les fichiers, e-mails, conversations, images et autres éléments de contenu contenant les données personnelles de la personne concernée sont récupérés et regroupés dans un conteneur de stockage d’objets blob Azure à des fins de révision. La récupération des données peut prendre quelques minutes ou beaucoup plus longtemps en fonction du volume de données. Une fois cette étape terminée, la demande passe automatiquement à l’étape suivante de **la révision des données**.

#### <a name="review-data"></a>Passer en revue les données
 À ce stade, vos contributeurs doivent examiner les résultats sous l’onglet **Données collectées** et effectuer toutes les tâches applicables, telles que la rédaction, l’application de balises et l’ajout de notes. Lorsque vous avez terminé la révision, sélectionnez **Terminer la révision**.

#### <a name="generate-reports"></a>Générer des rapports
Vos rapports sont générés à ce stade. Une fois l’opération terminée, celles-ci se trouvent sous l’onglet **Rapports** . Vos fichiers finis peuvent être exportés pour révision finale et remise à la personne concernée qui a effectué la demande.

#### <a name="close-the-request"></a>Fermer la demande
Une demande fermée indique que tous les travaux ont été effectués pour répondre à cette demande de droits d’objet. Toutes les données collectées et les rapports seront conservés en fonction de vos [paramètres de rétention des données](priva-settings.md#data-retention-periods).

## <a name="step-2-optional-view-and-edit-search-queries"></a>Étape 2 (facultatif) : afficher et modifier les requêtes de recherche

Pour afficher des informations détaillées sur la recherche de données derrière une demande de droits d’objet, sélectionnez **Afficher les détails de la requête de recherche**. Cela ouvre un volet résumant la requête et affichant des détails supplémentaires sur ce qui a été trouvé.

Vous avez ici la possibilité **d’afficher la préversion des résultats de la recherche** pour voir quel type de contenu sera retourné pour cette requête. Si vous souhaitez modifier les propriétés de cette recherche et que vous n’avez pas commencé la phase Récupérer des données, vous pouvez utiliser l’option **Modifier la requête de recherche** .

Le processus guidé de requête de recherche de modification vous permet de modifier ou d’ajouter des propriétés pour l’identification de la personne concernée, vos filtres et conditions de recherche, ainsi que les emplacements dans lesquels rechercher des données (y compris Exchange, SharePoint, OneDrive et/ou Teams). Utilisez ces options pour atteindre le niveau de spécificité souhaité. Vous pouvez passer en revue la version finale de votre nouvelle requête avant d’appuyer sur **Enregistrer**.

Lorsque vous avez terminé de modifier votre requête de recherche, une nouvelle recherche s’exécute pour remplacer vos résultats de recherche précédents. Cela réinitialise votre état dans la section **Progression** à la première étape, **Estimation des données**. La nouvelle recherche peut prendre jusqu’à 60 minutes. Une fois l’opération terminée, les résultats mis à jour s’affichent sur la page de détails de la demande.

## <a name="step-3-review-data"></a>Étape 3 : Examiner les données

À ce stade, vos contributeurs doivent examiner les résultats sous l’onglet **Données collectées**. Un canal Teams est automatiquement configuré pour faciliter l’examen du contenu par toutes les parties prenantes. Pour plus d’informations [, consultez Collaborer sur la révision des données](#collaborate-on-data-review) . Les tâches essentielles pour l’étape de révision des données sont décrites ci-dessous.

#### <a name="mark-items-as-include-or-exclude-and-add-notes"></a>Marquer des éléments comme Inclure ou Exclure et ajouter des notes

Passez en revue la liste des éléments identifiés retournés par votre recherche. Si vous décidez que l’élément doit être inclus dans le rapport final à l’objet de données, **sélectionnez Inclure** dans la barre de commandes en haut de la liste des éléments. Vous pouvez également sélectionner le bouton **Inclure** bleu dans la zone de révision de contenu à droite de la liste des éléments. Lorsque vous **sélectionnez Inclure**, un volet volant s’affiche avec une option permettant d’ajouter des notes. Lorsque vous avez terminé, **sélectionnez Envoyer** pour enregistrer l’état de révision de l’élément en tant **qu’Inclure**.

Si l’élément n’appartient pas à la demande, **sélectionnez Exclure** dans la barre de commandes ou le bouton **Exclure** dans la zone de révision de contenu. L’exclusion d’un élément signifie qu’il ne sera pas inclus dans les [rapports finaux générés pour la personne concernée](subject-rights-requests-reports.md).

> [!NOTE]
> Si vous **marquez** un élément comme Exclu, vous devez ajouter une note pour justifier pourquoi il ne concerne pas la demande de droits d’objet. Les notes sont à des fins internes et ne sont pas incluses dans les rapports finaux.

Si le contenu semble être un faux positif, sélectionnez **Non une correspondance** et, dans le volet de menu volant, **sélectionnez Confirmer**. Cette action exclut le fichier de vos rapports finaux et signale l’élément comme quelque chose qui n’aurait pas dû être détecté dans la recherche.

#### <a name="apply-tags"></a>Apply tags

Les balises peuvent être utilisées pour vous aider à identifier les éléments qui nécessitent une attention supplémentaire. Priva fournit trois balises par défaut ( **suivi**, **suppression** et **mise à jour** ) pour lesquelles vous pouvez définir une description. Priva fournit également deux balises personnalisées que vous pouvez nommer et décrire.

Par exemple, si vous déterminez lors de l’examen des données qu’un élément de contenu n’a pas besoin d’être conservé par votre organisation, vous pouvez appliquer la balise **Supprimer** , puis exporter une liste de tous les fichiers étiquetés afin de pouvoir revenir en arrière et supprimer les éléments identifiés lorsque vous avez terminé la demande.

Les cinq balises que vous gérez dans **Paramètres** s’appliquent à toutes vos demandes de droits d’objet.

**Pour ajouter ou supprimer des balises :**

- Sélectionnez l’élément dans la liste sous l’onglet **Données collectées** de la demande.
- Dans la zone d’aperçu de l’élément à droite de la liste, sélectionnez le bouton **Appliquer les balises** sur la ligne inférieure. Vous pouvez également sélectionner les trois points à droite du nom de l’élément et sélectionner l’option **Appliquer des balises** .
- Un volet volant s’affiche avec la liste des balises. Cochez la case en regard de l’une des balises que vous souhaitez appliquer à l’élément. La désélation d’une case à cocher supprime la balise.
- Lorsque vous avez terminé, **sélectionnez Enregistrer**, qui enregistre vos sélections de balises et ferme le volet volant.

**Pour ajouter des balises personnalisées ou mettre à jour les descriptions des balises :**
- Dans la page Demandes de droits de l’objet, sélectionnez **Paramètres** dans le coin supérieur droit de votre écran pour accéder à vos paramètres Priva.
- Accédez à la page **Balises de révision des données** , puis sélectionnez la balise pour entrer une description et, pour les balises personnalisées, un nom. En savoir plus sur [les paramètres de balise](priva-settings.md#data-review-tags).

**Pour exporter une liste d’éléments marqués :**
- Accédez à la page **Données collectées** dans une demande de droits d’objet.
- Au-dessus de la liste des éléments, sélectionnez l’icône de flèche vers le bas qui indique **Exporter** lorsque vous pointez dessus.
- Un fichier Excel est téléchargé et affiche les propriétés de tous les éléments collectés par la recherche de la requête. Recherchez la colonne **Étiquettes** pour identifier et trier les éléments par balise.

#### <a name="use-the-annotate-command-to-redact-text"></a>Utiliser la commande Annotate pour rétablir le texte
La commande **Annotate** dans la zone de révision de contenu vous permet de créer des balisages inline et de rétablir les données dans un élément de contenu. Par exemple, si vous devez inclure un fichier pour une personne qui contient également les informations personnelles d’un autre sujet de données, vous pouvez utiliser la **rédaction** de zone sous le bouton Dessin dans la barre de commandes pour noircir toutes les informations qui ne concernent pas la personne qui a effectué la demande. Une fois vos modifications terminées, **sélectionnez Inclure** pour ajouter le fichier supprimé à la demande. L’annotation crée une copie du fichier, qui est stockée dans votre objet blob Azure. Le fichier d’origine reste inchangé et stocké à son emplacement d’origine.

#### <a name="enter-notes-about-a-file"></a>Entrer des notes sur un fichier
Pour ajouter ou passer en revue des notes sur un élément, sélectionnez l’élément dans sa ligne et accédez à l’onglet **Notes** de fichier dans la zone de révision de contenu à droite. Vous pouvez également utiliser l’option **Ajouter une note de fichier** pour créer un commentaire. Pour passer en revue ou ajouter des notes au niveau du cas global, accédez à l’onglet **Notes** principal ci-dessus et utilisez **ajouter une note de cas**. Ces notes seront visibles pour les utilisateurs qui travaillent sur la demande, mais ne seront pas incluses dans le rapport final ou partagées avec la personne concernée.

#### <a name="complete-the-review"></a>Terminer la révision

Lorsque tous les éléments ont été examinés et que vous avez défini leur état **comme Inclure**, **Exclure** ou **Ne pas correspondre,** il est temps de fermer l’étape de révision en sélectionnant le bouton  **Terminer la révision** dans le coin supérieur droit de la demande. Un volet de menu volant affiche un résumé des données et ajoute toutes les notes associées. Ces notes sont destinées à la conservation des enregistrements internes et ne sont pas partagées avec la personne concernée.

Sélectionnez **Terminer la révision** dans le volet de menu volant pour terminer l’étape de révision. Les résumés de vos décisions seront fournis ultérieurement sous l’onglet **Rapports** .

### <a name="collaborate-on-data-review"></a>Collaborer sur la révision des données

Priva prend en charge la collaboration via Microsoft Teams pour permettre à votre groupe de travailler ensemble sur les demandes de droits de l’objet. Lorsque vous créez une demande, un canal Teams est automatiquement créé et associé à votre demande par défaut. Ici, vous pouvez discuter de la demande et partager en toute sécurité les entrées et les contributions. Pour participer à la conversation, ouvrez votre demande et utilisez l’option **Conversation avec collaborateurs** . Cela ouvre Microsoft Teams et vous place dans le canal Général pour le site d’équipe de votre demande de droits d’objet.

Pour passer en revue la liste des collaborateurs actifs qui peuvent afficher et contribuer à votre site d’équipe, ouvrez l’onglet **Collaborateurs** dans votre demande de droits d’objet. Pour ajouter des utilisateurs supplémentaires pour collaborer sur cette demande, sélectionnez l’option **Ajouter un collaborateur**.

Pour modifier le comportement par défaut de la génération de sites Teams lors de la création d’une demande de droits d’objet, accédez à **Paramètres** dans la navigation supérieure et sélectionnez **Teams collaboration** pour modifier le paramètre.

Vous pouvez également utiliser l’option **Partager** en haut à droite d’une demande de droit de l’objet pour connecter des personnes via Teams ou e-mail, ou pour copier le lien vers la page de Priva. Le partage via Teams vous permet de sélectionner un site et un canal Teams existants disponibles pour votre compte, où il publiera un lien vers ce cas avec n’importe quel message que vous fournissez.

## <a name="step-4-close-the-request"></a>Étape 4 : Fermer la demande

Une fois que vous avez effectué toutes les actions nécessaires pour résoudre votre demande de droits d’objet, sélectionnez **Fermer la demande**. Cela crée le rapport final, qui se trouve sous **l’onglet Rapports**. La saisie semi-automatique peut prendre un certain temps en fonction du nombre de fichiers dans la demande.

## <a name="next-steps"></a>Prochaines étapes
Pour en savoir plus sur l’utilisation des rapports et l’exécution des demandes de droits des personnes concernées, consultez [Générer des rapports et répondre à une demande de droits de sujet](subject-rights-requests-reports.md).

## <a name="legal-disclaimer"></a>Exclusion de responsabilité légale

[Exclusion de responsabilité légale de Microsoft Priva](priva-disclaimer.md)
