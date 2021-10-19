---
title: Rechercher et visualiser des données personnelles dans la gestion de la confidentialité
f1.keywords:
- CSH
ms.author: v-jgriffee
author: jmgriffee
manager: laurawi
audience: Admin
ms.topic: article
ms.service: O365-seccomp
ms.localizationpriority: medium
ms.collection:
- M365-security-compliance
- M365-privacy-management
search.appverid:
- MOE150
- MET150
description: Découvrez la vue d’ensemble et le profil de données dans la gestion de la confidentialité et découvrez comment obtenir des informations sur les données personnelles dans l’environnement Microsoft 365 de votre organisation.
ms.openlocfilehash: 119dc0d3649abd35c03ea5bdfe40f7967a0d2c9d
ms.sourcegitcommit: 85e085eb17af8b4efd1f45207445e1b3c3679600
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/19/2021
ms.locfileid: "60478265"
---
# <a name="find-and-visualize-personal-data-in-privacy-management"></a>Rechercher et visualiser des données personnelles dans la gestion de la confidentialité

La gestion de la confidentialité vous permet de comprendre les données que votre organisation stocke en automatisant la découverte des biens de données personnelles et en fournissant des visualisations d’informations essentielles. Ces visualisations sont disponibles dans les pages de vue **d’ensemble** et **de profil de données.** Vous pouvez agir sur les informations ici pour renforcer la posture de confidentialité de votre organisation et réduire les risques.

Pour commencer, consultez la section gestion de la confidentialité du [Centre de conformité Microsoft 365](https://compliance.microsoft.com/) et affichez les pages suivantes :

- **Vue** d’ensemble : fournit une vue d’ensemble des données de votre organisation dans Microsoft 365. Les administrateurs de confidentialité peuvent surveiller les tendances et les activités, identifier et examiner les risques potentiels impliquant des données personnelles et se baser sur des activités clés telles que la gestion des stratégies ou les actions de demande de droits de l’objet.
- **Profil de** données : fournit un instantané des données personnelles que votre organisation stocke dans Microsoft 365. Cette page vous permet de visualiser l’emplacement des données personnelles, les types les plus répandus dans votre organisation et le nombre de types différents dans les différents emplacements de votre environnement Microsoft 365. Vous pouvez également explorer les données personnelles à partir de cet emplacement.

À mesure que vos données changent et que la gestion de la confidentialité effectue de nouvelles conclusions, les informations affichées sur ces pages sont mises à jour. Notez que la représentation des nouvelles données dans les graphiques peut prendre jusqu’à 24 heures.

## <a name="explore-the-overview-page"></a>Explorer la page vue d’ensemble

La page de présentation se compose de trois sections principales. Les vignettes en haut de la page fournissent des statistiques récentes essentielles sur vos données. La section Informations clés fournit des opportunités d’enquête sur les tendances et domaines d’intérêt clés. Pour plus d’informations sur votre environnement de données, consultez les graphiques de courbe de tendance. Pour en savoir plus sur ces domaines, consultez les sections ci-dessous.

![Exemple de page de présentation.](../../media/privacy-management-overview.png)

### <a name="top-tiles"></a>Vignettes principales

#### <a name="policy-matches-over-past-7-days"></a>Correspondances de stratégie au cours des 7 derniers jours

Lorsque des stratégies sont définies dans le cadre de la gestion de la confidentialité, vos données sont évaluées en fonction de vos stratégies pour certaines conditions qui peuvent présenter des risques de confidentialité. Les correspondances de stratégie indiquent des découvertes de données qui peuvent avoir besoin d’un examen ou d’une correction plus approfondis. Cette vignette indique le nombre de correspondances de stratégie qui se sont produites au cours des sept derniers jours. Les correspondances seront surfacen es ici, que les stratégies soient actives ou en cours d’exécution en mode test, afin que vous pouvez voir les résultats de toutes vos stratégies actives. La sélection de cette vignette vous permet d’afficher une vue filtrée de la **page** Stratégies de gestion de la confidentialité, montrant les stratégies qui ont fait l’effet d’une correspondance au cours des sept derniers jours.

#### <a name="items-with-personal-data"></a>Éléments avec des données personnelles

Pour voir les fonctionnalités de découverte automatisée de la solution de gestion de la confidentialité au travail, consultez la vignette **Éléments avec des données personnelles.** Cette vignette indique le nombre de nouveaux éléments contenant des données personnelles en fonction de vos paramètres qui ont été découverts dans l’environnement Microsoft 365 de votre organisation au cours des sept derniers jours. La sélection de cette vignette charge une vue des 100 éléments les plus récents découverts.

#### <a name="subject-rights-requests"></a>Demandes de droits de l’objet

La page vue d’ensemble comprend une vignette qui indique le nombre de demandes de droits d’objet créées au cours des sept derniers jours. Une deuxième vignette, le cas échéant, indique le nombre de demandes en retard en fonction des échéances que vous avez désignées et peut avoir besoin d’une attention immédiate. La sélection de ces vignettes permettra aux utilisateurs ayant les autorisations appropriées d’accès à la page de demande de droits de l’objet de la gestion de la confidentialité.

### <a name="key-insights"></a>Informations clés

#### <a name="content-items-with-the-most-personal-data"></a>Éléments de contenu avec les données les plus personnelles

Le contenu qui contient une grande quantité de données personnelles peut présenter un risque d’exposition plus élevé. Vous pouvez examiner ces éléments pour vous assurer qu’ils sont couverts par une stratégie de gestion de la confidentialité. Pour attirer votre attention sur ces éléments, la page vue d’ensemble fournit une vue d’ensemble de vos éléments de contenu qui contiennent les données les plus personnelles en fonction de vos paramètres. Vous pouvez y voir le nombre de types de données personnelles uniques détectés, le nombre de propriétaires de contenu uniques qui ont été identifiés et le nombre de personnes qui ont été identifiées en fonction des paramètres de correspondance des données pour les demandes de droits d’objet.

Sélectionnez **Afficher le résumé** pour un affichage récapitulatif des éléments trouvés. Vous pouvez également choisir **d’explorer ces** résultats pour afficher un aperçu des fichiers individuels. Cet affichage affiche un maximum de 100 éléments. Les utilisateurs du groupe de rôles Gestion de la confidentialité peuvent sélectionner des fichiers pour passer en revue les détails et déterminer la pertinence, et exporter la liste au format .csv pour référence.

#### <a name="policies-with-the-most-matches-in-the-last-week"></a>Stratégies ayant le plus de correspondances au cours de la semaine dernière

Cet aperçu présente les stratégies les plus fréquemment mise en correspondance au cours des sept derniers jours, que ce soit en mode « On » ou « Testing ». Il permet d’illustrer les performances de vos stratégies et les effets du travail en cours lorsque vos utilisateurs de gestion de la confidentialité affinent leurs comportements de confidentialité.

Sélectionnez **Afficher le résumé** pour un résumé des 10 principales stratégies associées et des propriétaires de contenu du contenu associé. Vous verrez également le nombre de notifications utilisateur envoyées en raison de ces correspondances de stratégie et le nombre d’actions de l’utilisateur prises. Sélectionnez **Examiner** pour afficher la page des stratégies dans la gestion de la confidentialité, filtrée pour afficher les stratégies dans l’affichage récapitulatif. Cette vue d’investigation affiche des statistiques pour la durée de vie complète de la stratégie. Sélectionnez-le pour voir des détails tels que le moment où les éléments qui ont été détectés ont été détectés initialement.

#### <a name="users-with-the-most-policy-matched-in-the-last-week"></a>Utilisateurs ayant le plus de correspondances de stratégie au cours de la semaine dernière

Cette information traite également des correspondances à partir de stratégies en mode « Test » ou « En cours ». Il vous permet d’afficher un résumé des utilisateurs ayant le plus de correspondances de stratégies au cours de la semaine dernière et des stratégies correspondantes. Cela inclut les totaux des propriétaires de contenu uniques, les notifications envoyées à ces utilisateurs et le nombre d’actions prises à partir de ces notifications. La sélection **de l’examen** vous permet d’afficher la page des stratégies, filtrée pour afficher les stratégies dans l’affichage récapitulatif. Dans la vue d’investigation, vous ne trouverez pas d’informations utilisateur, mais vous pouvez sélectionner une stratégie pour afficher les détails de stratégie liés à ces correspondances.

#### <a name="items-with-the-most-data-subject-content"></a>Éléments ayant le plus de contenu de sujet de données

Cet aperçu fait référence aux informations de la fonctionnalité de correspondance de données dans les demandes de droits de l’objet et présente les éléments de contenu découverts dans Microsoft 365 qui contiennent le plus de sujets de données. Pour en savoir plus sur ce paramètre, voir [Gérer les demandes de droits d’objet.](privacy-management-subject-rights-requests.md)

Ces éléments peuvent vous aider à confirmer votre configuration de correspondance de données et à atténuer les risques de confidentialité liés à ces éléments. Sélectionnez **Afficher le résumé** pour un affichage récapitulatif. Sélectionnez **Explorer** pour obtenir une vue détaillée de 100 de ces éléments au plus. Ici, vous pouvez afficher un aperçu de ces éléments et déterminer la pertinence et exporter la liste au .csv format.

### <a name="trendline-graphs"></a>Graphiques de courbe de tendance

Pour obtenir des visualisations dynamiques des tendances trouvées dans les données de votre organisation, consultez les graphiques de courbe de tendance. Ces graphiques peuvent être filtrés par caractéristiques telles que la durée, le type de données ou les emplacements des données. Utilisez les dropdowns fournies pour ajuster votre affichage. Le fait de pointer sur des lignes dans le graphique vous permet de voir les statistiques relatives à ce point spécifique dans le temps.

Les résultats liés aux stratégies incluent les données des stratégies en mode « Test » et « En cours ». Si aucune stratégie d’un type particulier n’est active, les graphiques associés n’indiquent aucun résultat.

#### <a name="active-policy-alerts"></a>Alertes de stratégie active

Cette zone affiche un instantané des alertes actives déclenchées par des correspondances de stratégie. Au fil du temps, cette vue peut vous aider à détecter plus facilement des anomalies telles que des pics de volume importants. Sélectionnez **Afficher les alertes** pour accéder à la page des stratégies dans la gestion de la confidentialité, où vous pouvez examiner plus en détail les alertes et créer des problèmes pour la correction.

#### <a name="personal-data-found-in-organization"></a>Données personnelles trouvées dans l’organisation

Ce graphique montre les tendances du nombre de données personnelles correspondant à vos paramètres qui ont été découvertes au fil du temps dans votre environnement Microsoft 365 et où elles se trouvent. Il commence à être rempli une fois que la gestion de la confidentialité a été en cours d’exécution pendant suffisamment de temps et après que du contenu avec des données personnelles a été trouvé dans SharePoint, OneDrive, Teams et/ou Exchange.

#### <a name="data-transfers-detected-in-organization"></a>Transferts de données détectés dans l’organisation

Ce graphique est lié aux stratégies de transfert de données. Il fournit une vue d’ensemble du déplacement des données au sein de votre organisation, soit entre les services, soit entre les régions pour les organisations multigéogé.

#### <a name="unused-personal-data"></a>Données personnelles inutilisées

Ce graphique est lié aux stratégies de réduction des données. Il fournit des informations sur la façon dont votre organisation stocke du contenu contenant des données personnelles et sur la façon dont vos stratégies peuvent améliorer votre gestion de ces données au fil du temps.

#### <a name="overexposed-personal-data"></a>Données personnelles surexposées

Ce graphique est lié aux stratégies de surexpossure des données. Il peut vous aider à identifier les comportements de partage au sein de votre organisation et les emplacements où le contenu avec des données personnelles peut être surexposé, par exemple en étant partagé publiquement, partagé avec un utilisateur externe ou partagé largement au sein de votre organisation.

#### <a name="subject-rights-requests-by-regulation"></a>Demandes de droits de l’objet par réglementation

Cet affichage fournit des informations sur les réglementations les plus répandues qui pilotent vos demandes de droits d’objet au fil du temps. La légende de ce graphique montre les noms des réglementations les plus récentes. Le fait de pointer sur les lignes de tendance indique le nombre total de demandes de droits d’objet ouvertes pour cette réglementation pendant l’heure sélectionnée.

#### <a name="subject-rights-requests-by-status"></a>Demandes de droits de l’objet par état

Ce graphique indique comment votre organisation se porte sur l’exécution des demandes de droits d’objet, décomposées en demandes actives, fermées ou en **retard.** Les résultats de cette recherche peuvent vous aider à indiquer où vous pouvez tirer parti de l’allocation de ressources supplémentaires pour fermer vos demandes et vos objectifs de réunion.

### <a name="additional-data-views"></a>Affichages de données supplémentaires

#### <a name="subject-rights-requests-at-a-glance"></a>Demandes de droits de l’objet en un coup d’œil

Cette vue fournit une vue d’ensemble des demandes de droits d’objet actives, y compris le temps restant à effectuer les demandes avant leur échéance. Il récapitule le nombre total de demandes dont vous avez, le nombre d’entre elles sont actives et le nombre de demandes fermées. Sélectionnez **Afficher toutes les demandes** pour aller à la page de demande des droits de l’objet, où vous pouvez afficher d’autres détails et travailler sur les demandes actives pour les faire passer à la fin.

#### <a name="subject-rights-requests-by-residency"></a>Demandes de droits d’objet par résidence

Cet affichage de carte vous permet de visualiser votre volume de demandes de droits d’objet par résidence des personnes qui en sont à l’objet. Le survol d’une bulle identifiera la région et le total des demandes de droits d’objet ouvertes pour le compte des résidents.

## <a name="explore-the-data-profile-page"></a>Explorer la page de profil de données

La page de profil de données dans la gestion de la confidentialité fournit une vue instantanée des données personnelles que votre organisation stocke Microsoft 365 et où elles se trouve. Il fournit également des informations sur les types de données que vous stockez. Les vignettes principales sont les suivantes.

![Exemple de page de profil de données.](../../media/privacy-management-dataprofile.png)

### <a name="personal-data-type-instances-detected-in-microsoft-365"></a>Instances de type de données personnelles détectées dans Microsoft 365

Cette vignette vous permet de visualiser la quantité de données personnelles présentes dans votre environnement Microsoft 365 en fonction de vos paramètres et de la façon dont ces données sont distribuées entre Exchange, OneDrive, SharePoint et Teams.

Le graphique à barres indique le nombre approximatif d’instances de type de données personnelles uniques trouvées dans votre contenu. Des exemples de types de données peuvent inclure des éléments tels que des numéros de carte de crédit et des numéros de sécurité sociale. Par conséquent, un fichier découvert qui contient trois numéros de carte de crédit et un numéro de sécurité sociale contiendrait deux types de données personnelles uniques et quatre instances. La partie inférieure de cette vignette affiche les types de données personnelles uniques dans chaque Microsoft 365'emplacement. Il offre une vue d’ensemble de la diversité des types de données personnelles détectés dans le contenu de votre organisation.

### <a name="top-personal-data-types-across-your-organization"></a>Principaux types de données personnelles au sein de votre organisation

Cette vignette fournit un instantané des principaux types de données personnelles détectés dans votre environnement, ainsi que des informations sur le nombre d’éléments contenant ce type de données personnelles et sur les emplacements.

### <a name="personal-data-type-instances-by-region"></a>Instances de type de données personnelles par région

Pour les environnements multigé géographiques, cette vignette regroupe au niveau régional les instances de type de données personnelles trouvées dans votre contenu, en fonction des régions dans lesquelles ce contenu est hébergé. Pour les organisations à région unique, cette vignette affiche un point représentant votre emplacement Microsoft 365 région. Le fait de pointer sur des points sur la carte indique le nombre approximatif d’instances de type de données personnelles découvertes dans cette région.

### <a name="exploring-content"></a>Exploration de contenu

La sélection **d’Explorer** sur n’importe quelle vignette de profil de données ouvre l’explorateur de contenu. Pour l’instant, vous ne pouvez pas rechercher un élément de contenu spécifique et vous ne verrez pas Teams données dans cet affichage. Cela signifie que les nombres dans l’explorateur de contenu peuvent ne pas correspondre aux nombres affichés sur la page de profil de données, étant donné que la page de profil de données Teams contenu. Les administrateurs de confidentialité qui souhaitent obtenir des informations supplémentaires sur leurs données de confidentialité peuvent le faire ici en fonction du type de données personnelles (type d’informations sensibles) ou de l’emplacement (Exchange, OneDrive ou SharePoint).

## <a name="legal-disclaimer"></a>Clause d’exclusion de responsabilité légale

[Clause d’exclusion de responsabilité légale de gestion de la confidentialité](privacy-management-disclaimer.md)
