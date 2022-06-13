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
description: Découvrez comment examiner les données de demande de droits d’objet collectées par Microsoft Priva et collaborer à l’exécution de la demande.
ms.openlocfilehash: 0182be22efe224481625c121dc98ebe1d96a06ec
ms.sourcegitcommit: 3c83e8133a5a71f4e1d76a0b2981ab3ec9cd6602
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/13/2022
ms.locfileid: "66046628"
---
# <a name="review-data-for-a-subject-rights-request"></a>Examiner les données d’une demande de droits d’objet

**Dans cet article** : Découvrez comment passer en revue les données collectées pour une demande de droits d’objet à l’aide d’outils de rédaction, de balises de fichier. Découvrez comment utiliser la fonctionnalité de collaboration, qui inclut un canal Teams dédié.

Une fois que les données ont été collectées pour une demande de droits d’objet, l’étape suivante consiste à passer en revue les éléments de contenu, à décider quels éléments inclure ou exclure dans le cadre de la demande, et à rétablir les informations si nécessaire.

## <a name="tasks-for-completing-the-data-review"></a>Tâches pour terminer la révision des données

À ce stade, vos contributeurs doivent examiner les résultats sous l’onglet **Données collectées**. Un canal Teams est automatiquement configuré pour faciliter l’examen du contenu par toutes les parties prenantes. Pour plus d’informations, consultez [Collaboration pour la révision des données](#collaboration-for-data-review) ci-dessous. Les tâches essentielles pour l’étape de révision des données sont décrites ci-dessous.

#### <a name="mark-items-as-include-or-exclude-and-add-notes"></a>Marquer des éléments comme Inclure ou Exclure et ajouter des notes

Passez en revue la liste des éléments identifiés retournés par votre recherche. Si vous décidez que l’élément doit être inclus dans le rapport final à l’objet de données, **sélectionnez Inclure** dans la barre de commandes en haut de la liste des éléments. Vous pouvez également sélectionner le bouton **Inclure** bleu dans la zone de révision de contenu à droite de la liste des éléments. Lorsque vous **sélectionnez Inclure**, un volet volant s’affiche avec une option permettant d’ajouter des notes. Lorsque vous avez terminé, **sélectionnez Envoyer** pour enregistrer l’état de révision de l’élément en tant **qu’Inclure**.

Si l’élément n’appartient pas à la demande, **sélectionnez Exclure** dans la barre de commandes ou le bouton **Exclure** dans la zone de révision de contenu. L’exclusion d’un élément signifie qu’il ne sera pas inclus dans les [rapports finaux générés pour la personne concernée](subject-rights-requests-reports.md).

> [!NOTE]
> Si vous **marquez** un élément comme Exclu, vous devez ajouter une note pour justifier pourquoi il ne concerne pas la demande de droits d’objet. Les notes sont à des fins internes et ne sont pas incluses dans les rapports finaux.

Si le contenu semble être un faux positif, sélectionnez **Non une correspondance** et, dans le volet de menu volant, **sélectionnez Confirmer**. Cette action exclut le fichier de vos rapports finaux et signale l’élément comme quelque chose qui n’aurait pas dû être détecté dans la recherche.

#### <a name="apply-tags"></a>Apply tags

Les balises peuvent être utilisées pour vous aider à identifier les éléments qui nécessitent une attention supplémentaire. Priva fournit trois balises par défaut ( **Suivi**, **Suppression** et **Mise à jour** ) pour lesquelles vous pouvez définir une description. Priva fournit également deux balises personnalisées que vous pouvez nommer et décrire.

Par exemple, si vous déterminez lors de l’examen des données qu’un élément de contenu n’a pas besoin d’être conservé par votre organisation, vous pouvez appliquer la balise **Supprimer** , puis exporter une liste de tous les fichiers étiquetés afin de pouvoir revenir en arrière et supprimer les éléments identifiés lorsque vous avez terminé la demande.

Les cinq balises que vous gérez dans **Paramètres** s’appliquent à toutes vos demandes de droits d’objet.

**Pour ajouter ou supprimer des balises :**

- Sélectionnez l’élément dans la liste sous l’onglet **Données collectées** de la demande.
- Dans la zone d’aperçu de l’élément à droite de la liste, sélectionnez le bouton **Appliquer les balises** sur la ligne inférieure. Vous pouvez également sélectionner les trois points à droite du nom de l’élément et sélectionner l’option **Appliquer des balises** .
- Un volet volant s’affiche avec la liste des balises. Cochez la case en regard de l’une des balises que vous souhaitez appliquer à l’élément. La décochage d’une case à cocher supprime la balise.
- Lorsque vous avez terminé, **sélectionnez Enregistrer**, qui enregistre vos sélections de balises et ferme le volet volant.

**Pour ajouter des balises personnalisées ou mettre à jour les descriptions des balises :**
- Dans la page Demandes de droits d’objet, sélectionnez **Paramètres** dans le coin supérieur droit de votre écran pour accéder à vos paramètres de Priva.
- Accédez à la page **Balises de révision des données** , puis sélectionnez la balise pour entrer une description et, pour les balises personnalisées, un nom. En savoir plus sur [les paramètres de balise](priva-settings.md#data-review-tags).

**Pour exporter une liste d’éléments marqués :**
- Accédez à la page **Données collectées** dans une demande de droits d’objet.
- Au-dessus de la liste des éléments, sélectionnez la commande **Exporter** .
- Un fichier Excel est téléchargé et affiche les propriétés de tous les éléments collectés par la recherche de la requête. Recherchez la colonne **Étiquettes** pour identifier et trier les éléments par balise.

#### <a name="use-the-annotate-command-to-redact-text"></a>Utiliser la commande Annotate pour rétablir le texte
La commande **Annotate** dans la zone de révision de contenu vous permet de créer des balisages inline et de rétablir les données dans un élément de contenu. Par exemple, si vous devez inclure un fichier pour une personne qui contient également les informations personnelles d’un autre sujet de données, vous pouvez utiliser la **rédaction** de zone sous le bouton Dessin dans la barre de commandes pour noircir toutes les informations qui ne concernent pas la personne qui a effectué la demande. Une fois vos modifications terminées, **sélectionnez Inclure** pour ajouter le fichier supprimé à la demande. L’annotation crée une copie du fichier, qui est stockée dans votre objet blob Azure. Le fichier d’origine reste inchangé et stocké à son emplacement d’origine.

#### <a name="enter-notes-about-a-file"></a>Entrer des notes sur un fichier
Pour ajouter ou passer en revue des notes sur un élément, sélectionnez l’élément dans sa ligne et accédez à l’onglet **Notes** de fichier dans la zone de révision de contenu à droite. Vous pouvez également utiliser l’option **Ajouter une note de fichier** pour créer un commentaire. Pour passer en revue ou ajouter des notes au niveau du cas global, accédez à l’onglet **Notes** principal ci-dessus et utilisez **ajouter une note de cas**. Ces notes seront visibles pour les utilisateurs qui travaillent sur la demande, mais ne seront pas incluses dans le rapport final ou partagées avec la personne concernée.

## <a name="collaboration-for-data-review"></a>Collaboration pour la révision des données

Les administrateurs de demandes de droits d’objet peuvent afficher toutes les demandes. Vous pouvez ajouter d’autres utilisateurs pour collaborer sur une demande, ce qui leur donnera accès à l’affichage de cette demande et utilisera les données collectées dans celle-ci pour faciliter le déplacement de la demande vers l’achèvement.

Lorsque vous créez une demande, un canal de Teams dédié est automatiquement créé pour permettre aux parties prenantes de discuter de la demande et de partager en toute sécurité les entrées et les contributions. L’onglet **Collaborateurs** de la page détails de la demande affiche tous les collaborateurs qui peuvent afficher et contribuer à la demande et à n’importe quel canal Teams associé.

Pour ajouter d’autres collaborateurs, **sélectionnez Ajouter un collaborateur**, commencez à taper le nom de l’utilisateur, sélectionnez le nom une fois qu’il apparaît, puis **sélectionnez Ajouter**.

Pour démarrer une conversation Teams, n’importe quel collaborateur peut sélectionner **Conversation avec des collaborateurs** en haut à droite de la page de détails de la demande. Cette action ouvre Teams et vous place dans le canal **Général** pour le site d’équipe de votre demande de droits d’objet.

Vous pouvez modifier le comportement par défaut de la création de canaux Teams pour les demandes de droits d’objet en accédant à Priva **Paramètres** dans le coin supérieur droit de la demande de droits de l’objet. Sélectionnez **Teams collaboration**, puis décochez la case sur la page pour désactiver Teams fonctionnalités pour toutes les requêtes relatives aux droits d’objet.

La commande **Partager** en haut à droite de la page de détails d’une requête crée un lien partageable qui accède directement à la demande dans Priva. Donnez ce lien aux collaborateurs afin qu’ils puissent accéder à la demande à laquelle vous les avez ajoutés.

## <a name="complete-the-review"></a>Terminer la révision

Lorsque tous les éléments ont été examinés et que vous avez défini leur état **comme Inclure**, **Exclure** ou **Ne pas correspondre,** il est temps de fermer l’étape de révision. Tous les collaborateurs d’une demande peuvent terminer la révision.

Sélectionnez le bouton **Terminer la révision** dans le coin supérieur droit de la demande. Un volet de menu volant affiche un résumé des données et ajoute toutes les notes associées. Ces notes sont destinées à la conservation des enregistrements internes et ne sont pas partagées avec la personne concernée.

Sélectionnez **Terminer la révision** dans le volet de menu volant pour terminer l’étape de révision. Cette action prépare la demande pour les étapes finales du processus : génération de rapports et fermeture de la demande. Les résumés de vos décisions seront fournis ultérieurement sous l’onglet **Rapports** .

## <a name="next-steps"></a>Étapes suivantes
Découvrez comment générer le rapport final et travailler à l’achèvement de la demande dans [Générer des rapports et fermer une demande](subject-rights-requests-reports.md).

## <a name="legal-disclaimer"></a>Exclusion de responsabilité légale

[Microsoft Priva exclusion de responsabilité légale](priva-disclaimer.md)
