---
title: Correspondance des données pour les demandes de droits d’objet
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
description: Découvrez comment charger des informations supplémentaires sur vos sujets de données dans Microsoft Priva.
ms.openlocfilehash: 90ee0e8e21d25954c11113992cbb7ece847c85ab
ms.sourcegitcommit: 6b88d22d0250cbb9a4ba1f71665f29cb67939851
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65059738"
---
# <a name="data-matching-for-subject-rights-requests"></a>Correspondance des données pour les demandes de droits d’objet

Avec la correspondance des données, les organisations peuvent permettre à Microsoft Priva d’identifier les personnes concernées en fonction des valeurs de données exactes fournies. Cela peut aider à augmenter la précision de la localisation du contenu de la personne concernée qui correspond à ces valeurs de données à la fois pour votre personnel interne et pour les utilisateurs externes avec lesquels vous interagissez. Il simplifie également la nécessité de fournir manuellement des champs lors de la création de la demande de droits d’objet, et fournit le contexte dans les demandes de droits d’objet et pour la vignette Vue d’ensemble qui présente vos éléments avec le contenu de la personne concernée la plus élevée. Pour en savoir plus sur cette vue, consultez [Rechercher et visualiser des données personnelles dans Priva](priva-data-profile.md#items-with-the-most-data-subject-content).

Pour utiliser la fonctionnalité de correspondance des données, vous devez être membre du groupe de rôles Gestion de la confidentialité. À partir de Priva dans le [portail de conformité Microsoft Purview](https://compliance.microsoft.com/), sélectionnez **Paramètres** dans le volet de navigation supérieur, puis **correspondance des données**. À partir de là, vous devez définir le schéma de données personnelles et fournir un chargement de données personnelles comme indiqué ci-dessous. Notez que vous pouvez ajouter des éléments et supprimer des éléments que vous ajoutez, mais que vous ne pouvez pas modifier un élément.

## <a name="prepare-for-data-import"></a>Préparer l’importation de données

Avant de définir le schéma ou de charger des données, vous devez identifier la source des informations de votre sujet de données. Le format de fichier requis est .csv, qui peut être lu par une application telle que Microsoft Excel. Structurez cette exportation pour que vos en-têtes de colonne apparaissent dans la première ligne. Ces en-têtes doivent inclure les noms des attributs de votre schéma de données personnelles. Vérifiez le format des données dans chaque champ. Si l’une des données contient des virgules, entourez ces valeurs de guillemets doubles pour vous assurer qu’elles ne seront pas analysées dans des champs distincts.

## <a name="define-the-personal-data-schema"></a>Définir le schéma de données personnelles

La première étape de la configuration de la correspondance des données consiste à définir le schéma de données personnelles, qui décrit les attributs de vos sujets de données. Vous allez charger ce schéma dans le premier onglet de la zone des paramètres correspondant aux données. Les fichiers requis incluent un fichier XML **de schéma de données personnelles** et un fichier XML de **package de règles** .

### <a name="personal-data-schema-xml"></a>XML de schéma de données personnelles

Le fichier de schéma de données personnelles est un fichier XML qui définit les noms de colonnes attendus.

- Nommez ce fichier de schéma *pdm.xml*.
- Définissez chaque nom de colonne à l’aide de la balise Nom du champ, comme indiqué dans l’exemple ci-dessous.
- Utilisez searchable = « true » pour les champs que vous souhaitez rechercher, jusqu’à un maximum de cinq champs. Au moins un de vos noms de champs doit être consultable. Exemple de syntaxe : `\<Field name="" searchable=""/>`.
- Le schéma de données personnelles comporte une section d’étiquette DataStore. Quatre champs obligatoires doivent être mappés à vos noms de champs : primaryKeyField, upnField, firstNameField, lastNameField.

Par exemple, le fichier XML suivant définit un exemple de schéma, avec cinq champs spécifiés comme pouvant faire l’objet d’une recherche : PatientID, MRN, SSN, Téléphone et DOB. PrimaryKeyField est mappé à PatientID, upnField est mappé à MRN, firstNameField est mappé à FirstName et lastNameField est mappé à LastName.

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

### <a name="rule-package-xml"></a>Code XML du package de règles

Lorsque vous configurez votre package de règles, veillez à référencer correctement votre fichier de schéma de données personnelles créé ci-dessus : pdm.xml. Dans l’exemple de package de règles XML suivant, les champs suivants doivent être personnalisés pour créer votre type sensible de correspondance de données :

- **ID** &  RulePack **ID PrivacyMatch** : utilisez new-GUID pour générer un GUID.
- **Magasin de** données : ce champ spécifie le magasin de données de recherche de correspondance de données personnelles à utiliser. Indiquez le nom de magasin de données défini d’un schéma de données personnelles configuré.
- **idMatch** : ce champ pointe vers l’élément principal pour la correspondance des données personnelles.
  - **Correspondances** : spécifie le champ à utiliser dans la recherche exacte. Fournissez un nom de champ pouvant faire l’objet d’une recherche à partir du schéma de données personnelles.
  - **Classification** : ce champ spécifie la correspondance de type sensible qui déclenche la recherche de correspondance de données personnelles. Vous pouvez fournir le nom ou le GUID d’un type d’informations sensibles intégré ou personnalisé. Pour éviter de provoquer des problèmes de performances, si vous utilisez un type d’informations sensibles personnalisé comme élément Classification dans la correspondance des données personnelles, n’utilisez pas un type d’informations sensibles personnalisé qui correspond à un grand pourcentage de contenu (par exemple, « n’importe quel nombre » ou « mot de cinq lettres »). Nous vous recommandons d’ajouter des mots clés de prise en charge ou d’inclure la mise en forme dans la définition du type d’informations sensibles de classification personnalisée.
- **Correspondance** : ce champ pointe vers des preuves supplémentaires trouvées à proximité d’idMatch.
  - **Correspondances** : indiquez n’importe quel nom de champ dans le schéma de données personnelles pour DataStore.
- **Ressource** : cette section spécifie le nom et la description du type sensible dans plusieurs paramètres régionaux.
  - **idRef** : fournissez le GUID pour l’ID ExactMatch.
  - **Nom & descriptions** : personnalisez en fonction des besoins.

Dans notre exemple XML de package de règles ci-dessous, nous référençant le fichier pdm.xml exemple de fichier de l’étape précédente qui crée le XML de schéma de données personnelles :

- **Magasin de** données : le nom du magasin de données fait référence au fichier de schéma que nous avons créé précédemment : dataStore = « PatientRecords ».
- **idMatch** : la valeur idMatch fait référence à un champ pouvant faire l’objet d’une recherche répertorié dans le fichier pdm.xml que nous avons créé précédemment : idMatch correspond à « SSN ».
  - **Classification** : la valeur de classification fait référence à un type d’informations sensibles existant ou personnalisé : classification = « U.S. Social Security Number (SSN) ». (en l’occurrence, nous utilisons le type d’informations sensibles existant pour le numéro de sécurité sociale aux États-Unis).

Créez un package de règles au format XML (avec encodage Unicode), comme dans l’exemple de code suivant. Vous pouvez copier, modifier et utiliser cet exemple.

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

## <a name="sensitive-info-types"></a>Types d’informations sensibles

La deuxième étape de la configuration de la correspondance des données consiste à créer des types d’informations sensibles uniques pour la correspondance de données personnelles (PDM). [Les types d’informations sensibles (SIT) sont des](/microsoft-365/compliance/sensitive-information-type-learn-about) classifieurs basés sur des modèles qui détectent des informations sensibles telles que la Sécurité sociale ou les numéros de carte de crédit. La configuration d’un type d’informations sensibles PDM vous permet d’utiliser des valeurs de données exactes plutôt que des valeurs génériques pour détecter les correspondances. Pour commencer cette étape, sélectionnez **Créer un type d’informations sensibles PDM** pour démarrer l’Assistant Création.

## <a name="upload-personal-data"></a>Télécharger données personnelles

Après avoir défini le schéma de données personnelles et les types d’informations sensibles, la troisième étape consiste à charger des données personnelles. Accédez à l’onglet **Chargement de données personnelles** , **sélectionnez Ajouter**, puis choisissez le schéma personnel que vous avez défini à la première étape, puis chargez le fichier contenant les données personnelles.

Vous pouvez charger ces données personnelles en choisissant un fichier local ou en fournissant une URL SAS à un emplacement Stockage Microsoft Azure existant contenant votre fichier de données personnelles.
Si vous avez préparé un fichier comme première étape de ce processus conforme au schéma créé, vous pouvez utiliser ce fichier pour le chargement.

## <a name="legal-disclaimer"></a>Exclusion de responsabilité légale

[Exclusion de responsabilité légale de Microsoft Priva](priva-disclaimer.md)
