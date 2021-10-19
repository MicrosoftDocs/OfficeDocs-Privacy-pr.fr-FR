---
title: Gérer la correspondance des données pour les demandes de droits de l’objet dans la gestion de la confidentialité
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
description: Découvrez comment télécharger des informations supplémentaires sur la gestion de la confidentialité sur vos personnes à l’aide de données.
ms.openlocfilehash: 00a902705336d766993e805d78609a48334b2bf6
ms.sourcegitcommit: 85e085eb17af8b4efd1f45207445e1b3c3679600
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/19/2021
ms.locfileid: "60478272"
---
# <a name="manage-data-matching-for-subject-rights-requests"></a>Gérer la correspondance des données pour les demandes de droits d’objet

Grâce à la correspondance des données, les organisations peuvent activer la gestion de la confidentialité pour identifier les personnes liées aux données en fonction des valeurs de données fournies exactes. Cela peut vous aider à améliorer la précision de la recherche du contenu de la sujet de données qui correspond à ces valeurs de données à la fois pour votre personnel interne et pour les utilisateurs externes avec qui vous interagissez. Il simplifie également la nécessité de fournir des champs manuellement lors de la création des demandes de droits d’objet, et fournit du contexte dans les demandes de droits de l’objet et pour la vignette Vue d’ensemble qui présente vos éléments avec le plus de contenu de sujet de données. Pour en savoir plus sur cette vue, voir [Rechercher et visualiser vos données.](privacy-management-data-profile.md#items-with-the-most-data-subject-content)

Pour utiliser la fonctionnalité de correspondance de données, vous devez être membre du groupe de rôles Gestion de la confidentialité. À partir de la gestion de  la confidentialité dans [le Centre de conformité Microsoft 365,](https://compliance.microsoft.com/)sélectionnez Paramètres dans la partie supérieure de navigation, puis correspondance **de données.** À partir de là, vous devrez définir le schéma de données personnelles et fournir un téléchargement de données personnelles, comme illustré ci-dessous. Notez que vous pouvez ajouter des éléments et supprimer des éléments que vous ajoutez via l’interface utilisateur. Toutefois, vous ne pouvez pas modifier un élément en place à partir de l’interface utilisateur pour le moment.

## <a name="prepare-for-data-import"></a>Préparer l’importation de données

Avant de définir le schéma ou de télécharger des données, vous devez identifier la source de vos informations de sujet de données. Le format de fichier requis est .csv, qui peut être lu par une application telle que Microsoft Excel. Structurez cette exportation de sorte que vos en-têtes de colonne apparaissent sur la première ligne. Ces en-têtes doivent inclure les noms des attributs de votre schéma de données personnelles. Vérifiez le format des données dans chaque champ. Si l’une des données contient des virgules, entourez ces valeurs de guillemets doubles pour vous assurer qu’elles ne seront pas séparées.

## <a name="define-the-personal-data-schema"></a>Définir le schéma de données personnelles

Le schéma de données personnelles décrit les attributs de vos sujets de données. Télécharger ce schéma sur le premier onglet de la zone des paramètres de correspondance de données. Les fichiers requis incluent un fichier XML **de** schéma de données personnelles et un fichier XML **de package** de règles.

### <a name="personal-data-schema-xml"></a>XML de schéma de données personnelles

Le fichier de schéma de données personnelles est un fichier XML qui définit les noms de colonne attendus.

- Nommez ce fichier de *schémapdm.xml*.
- Définissez chaque nom de colonne à l’aide de la balise Nom du champ, comme dans l’exemple ci-dessous.
- Utilisez searchable = « true » pour les champs que vous souhaitez rechercher, jusqu’à un maximum de cinq champs. Au moins l’un de vos noms de champ doit pouvoir faire l’être. Exemple de syntaxe `\<Field name="" searchable=""/>` : .
- Le schéma de données personnelles possède une section de balise DataStore. Quatre champs obligatoires doivent être mappés à vos noms de champs : primaryKeyField, upnField, firstNameField, lastNameField.

Par exemple, le fichier XML suivant définit un exemple de schéma, avec cinq champs spécifiés comme utilisables dans une recherche : PatientID, MRN, SSN, Téléphone et DOB. Le champ primaryKeyField est mappé sur PatientID, upnField est mappé sur MRN, firstNameField est mappé sur FirstName et lastNameField est mappé sur LastName.

Vous pouvez copier, modifier et utiliser notre exemple.

 ```xml
<PdmSchema xmlns="http://schemas.microsoft.com/office/2020/pdm">
      <DataStore name="Patientrecords" description="Schema for patient records" version="1" primaryKeyField="PatientID" upnField="MRN" firstNameField="FirstName" lastNameField="LastName">
            <Field name="PatientID" searchable="true"/>
            <Field name="MRN" searchable="true" />
            <Field name="FirstName" />
            <Field name="LastName" />
            <Field name="SSN" searchable="true" />
            <Field name="Phone" searchable="true" />
            <Field name="DOB" searchable="true" />
            <Field name="Gender" />
            <Field name="Address" />
      </DataStore>
</PdmSchema>
 ```

### <a name="rule-package-xml"></a>XML de package de règles

Lorsque vous définissez votre package de règles, veillez à référencer correctement votre fichier de schéma de données personnelles créé ci-dessus : pdm.xml. Dans l’exemple de package de règles XML suivant, les champs suivants doivent être personnalisés pour créer votre type sensible de correspondance de données :

- **RulePack id**  &  **ID PrivacyMatch**: utiliser new-GUID pour générer un GUID.
- **Datastore : ce** champ spécifie le magasin de données de recherche de correspondance de données personnelles à utiliser. Indiquez le nom datastore défini d’un schéma de données personnelles configuré.
- **idMatch**: ce champ pointe vers l’élément principal de la correspondance de données personnelles.
  - **Correspond :** spécifie le champ à utiliser dans la recherche exacte. Fournissez un nom de champ utilisable dans une recherche à partir du schéma de données personnelles.
  - **Classification**: ce champ spécifie la correspondance de type sensible qui déclenche la recherche de correspondance de données personnelles. Vous pouvez fournir le nom ou le GUID d’un type d’informations sensibles intégré ou personnalisé. Afin d’éviter les problèmes de performances, si vous utilisez un type d’informations sensibles personnalisé en tant qu’élément classification dans la correspondance de données personnelles, n’utilisez pas un type d’informations sensibles personnalisé qui correspondra à un grand pourcentage de contenu (par exemple, « n’importe quel nombre » ou « tout mot de cinq lettres »). Nous vous recommandons d’ajouter des mots clés de prise en charge ou d’inclure la mise en forme dans la définition du type d’informations sensibles de classification personnalisé.
- **Correspondance**: ce champ pointe vers des preuves supplémentaires trouvées à proximité d’idMatch.
  - **Correspondances**: indiquez un nom de champ quelconque dans le schéma de données personnelles de DataStore.
- **Ressource**: cette section spécifie le nom et la description du type sensible dans plusieurs paramètres régionaux.
  - **idRef**: fournir un GUID pour l’ID ExactMatch.
  - **Nom & descriptions :** personnaliser selon les besoins.

Dans notre exemple de fichier XML de package de règles ci-dessous, nous faisons référence au fichier pdm.xml exemple de fichier de l’étape précédente qui crée le fichier XML de schéma de données personnelles :

- **Datastore**: le nom de dataStore fait référence au fichier de schéma que nous avons créé précédemment : dataStore = « PatientRecords ».
- **idMatch**: la valeur idMatch fait référence à un champ utilisable dans une recherche répertorié dans le fichier pdm.xml que nous avons créé précédemment : idMatch correspond à = « SSN ».
  - **Classification**: la valeur de classification fait référence à un type d’informations sensibles existant ou personnalisé : classification = « Numéro de sécurité sociale (SSN) des États-Unis ». (en l’occurrence, nous utilisons le type d’informations sensibles existant pour le numéro de sécurité sociale aux États-Unis).

Créez un package de règles au format XML (avec codage Unicode), comme dans l’exemple de code suivant. Vous pouvez copier, modifier et utiliser cet exemple.

 ```xml
<RulePackage xmlns="http://schemas.microsoft.com/office/2020/pdm">
  <RulePack id="fd098e03-1796-41a5-8ab6-198c93c62b21">
    <Version build="0" major="2" minor="0" revision="0" />
    <Publisher id="eb553734-8306-44b4-9ad5-c388ad970528" />
    <Details defaultLangCode="en-us">
      <LocalizedDetails langcode="en-us">
        <PublisherName>IP DLP</PublisherName>
        <Name>Health Care PDM Rulepack</Name>
        <Description>This rule package contains the Personal Data Match sensitive type for health care sensitive types.</Description>
      </LocalizedDetails>
    </Details>
  </RulePack>
  <Rules>
    <PrivacyMatch id = "E1CC861E-3FE9-4A58-82DF-4BD259EAB381" patternsProximity = "300" dataStore ="PatientRecords" recommendedConfidence = "65" >
      <Pattern confidenceLevel="65">
        <idMatch matches = "SSN" classification = "U.S. Social Security Number (SSN)" />
      </Pattern>
      <Pattern confidenceLevel="75">
        <idMatch matches = "SSN" classification = "U.S. Social Security Number (SSN)" />
        <Any minMatches ="3" maxMatches ="6">
          <match matches="PatientID" />
          <match matches="MRN"/>
          <match matches="FirstName"/>
          <match matches="LastName"/>
          <match matches="Phone"/>
          <match matches="DOB"/>
        </Any>
      </Pattern>
    </PrivacyMatch>
    <LocalizedStrings>
      <Resource idRef="E1CC861E-3FE9-4A58-82DF-4BD259EAB381">
        <Name default="true" langcode="en-us">Patient SSN Exact Match.</Name>
        <Description default="true" langcode="en-us">PDM Sensitive type for detecting Patient SSN.</Description>
      </Resource>
    </LocalizedStrings>
  </Rules>
</RulePackage>
 ```

## <a name="upload-personal-data"></a>Télécharger données personnelles
Après avoir défini le schéma de données  personnelles, vous pouvez effectuer le chargement des données personnelles sous le deuxième onglet de la page des paramètres de correspondance de données. Lorsque vous **sélectionnez Ajouter,** choisissez le schéma personnel que vous avez défini à la première étape, puis téléchargez le fichier contenant les données personnelles.

Vous pouvez charger ces données personnelles en choisissant un fichier local ou en fournissant une URL SAS à un emplacement Stockage Microsoft Azure existant contenant votre fichier de données personnelles.
Si vous avez préparé un fichier en tant que première étape de ce processus qui est conforme au schéma créé, vous pouvez utiliser ce fichier pour le chargement.

## <a name="legal-disclaimer"></a>Clause d’exclusion de responsabilité légale

[Clause d’exclusion de responsabilité légale de gestion de la confidentialité](privacy-management-disclaimer.md)
