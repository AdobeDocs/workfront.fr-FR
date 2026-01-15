---
title: Types d’enregistrements - Aperçu
description: Les types d’enregistrement sont les blocs de construction d’un espace de travail Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 1de095b3-78d9-44df-a678-51f4238deb91
source-git-commit: 5d326776b9c5b4d9d24e802375df4630508c8bd0
workflow-type: tm+mt
source-wordcount: '352'
ht-degree: 35%

---


# Vue d’ensemble des types d’enregistrement

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Contrairement à Workfront où les types d&#39;objet sont prédéfinis, dans Adobe Workfront Planning, vous pouvez créer vos propres types d&#39;objet.

Par exemple, dans Workfront, les types d’objets « Programme », « Portfolio », « Projet », « Tâche » ou « Problème » sont déjà créés.

Les types d’objets Workfront Planning sont appelés « types d’enregistrements » et n’existent que lorsque les utilisateurs les créent.

Les types d’enregistrements sont les blocs de construction d’un espace de travail Workfront Planning et vous devez tous les créer pour pouvoir les associer aux workflows et à d’autres informations.

Les types d’enregistrements sont organisés dans les espaces de travail.

Pour plus d’informations sur les espaces de travail, consultez la section [Créer des espaces de travail](/help/quicksilver/planning/architecture/create-workspaces.md).

## Vue d’ensemble des types d’enregistrement

Dans Workfront Planning, vous pouvez créer des types d’enregistrements personnalisés qui répondent aux besoins de votre entreprise.

Pour plus d’informations sur la création de types d’enregistrements, voir [Créer des types d’enregistrements](/help/quicksilver/planning/architecture/create-record-types.md).

* Lorsque vous créez un espace de travail à partir d’un modèle, les types d’enregistrement sont créés dans les sections suivantes de l’espace de travail :

   * **Types d’enregistrements opérationnels** : types d’enregistrements qui représentent des plans stratégiques, des initiatives ou des travaux planifiés. Par exemple, Campagne, Activité, Tactique, Opportunité sont des types d’enregistrements opérationnels.
   * **Taxonomies** : types d’enregistrements qui capturent des attributs sur un type d’enregistrement opérationnel. Par exemple, Région, Adresse, Audience sont des taxonomies.

  Vous pouvez renommer ou supprimer les sections et les types d’enregistrements, ou en créer d’autres.

* Lorsque vous créez un type d’enregistrement dans un espace de travail que vous avez entièrement créé, vous pouvez le placer dans n’importe quelle section que vous créez dans l’espace de travail.
* Lorsque vous créez un type d’enregistrement, seuls vous et ceux à qui vous accordez l’autorisation d’accéder à l’espace de travail et au type d’enregistrement pouvez y accéder.
* Vous devez créer un espace de travail avant de pouvoir créer des types d’enregistrement pour cet espace de travail.

  Pour connaître les limites du nombre de types d&#39;enregistrements que vous pouvez avoir dans une instance de Workfront ou un espace de travail, consultez la section [Présentation des limitations d&#39;objet Adobe Workfront Planning](/help/quicksilver/planning/general/limitations-overview.md).
* Pour utiliser des types d’enregistrements dans plusieurs espaces de travail, vous pouvez désigner des types d’enregistrements comme globaux ou connectables.

   * Les types d’enregistrements globaux peuvent être ajoutés en tant que types d’enregistrements existants à d’autres espaces de travail.
   * Les types d’enregistrements connectables peuvent être connectés à à partir d’autres espaces de travail.

  Pour plus d’informations, voir [Configuration des fonctionnalités de plusieurs espaces de travail pour les types d’enregistrements](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).


<!--

### Operational Record Type{#operational-record-type}

An operational record type is a Wrorkfront Planning record type that represents work-related objects.  

(***********insert screen shot**************)
For more information about operational record types including how to create them, see [Create record types](/help/quicksilver/planning/architecture/create-record-types.md). 

### Taxonomy{#taxonomy}

A taxonomy is a record type that captures attributes about an operational record type. 

(**********add screen shot**********)

Although creating taxonomies is identical to creating operational record types, Workfront Planning distinguishes conceptually between an operational record type and a taxonomy record type. The purpose of taxonomies is to enhance operational record types. Taxonomies should not directly represent work objects.  (***********this is no longer true, but might be later?!: A taxonomy is a record without dates, like a static list of attributes.***********) 

(********mimic what you did above for operational record types to say that we can also import taxonomies from other applications too - this will be possible later; for example Team would be a taxonomy record type, etc*************)

For example, Audience, Region, or Address can be taxonomy-type record types.  

## Similarities and differences between operational record types and taxonomies

The following table illustrates some of the similarities and differences between operational record types and taxonomies: 

| Record type and characteristic                              | Operational Record Type | Taxonomy Record Type |
|-------------------------------------------------------------|:-----------------------:|:--------------------:|
| They are part of a workspace                                |            ✓            |           ✓          |
| You can create them automatically, from a workspace template                    |            ✓            |           ✓          |
| You can create them manually, from scratch                    |            ✓            |           ✓          |
| You can create them by copying and pasting information from an external file or list                   |            ✓            |           ✓          |
| You can create by importing an Excel or CSV file                    |            ✓            |                     |
| You can create read-only record types by connecting to object types from other applications                    |            ✓            |                     |
| They represent work-related objects                         |            ✓            |                      |
| They represent attributes about work-related objects        |                         |           ✓          |
| You can create from scratch                                 |            ✓            |           ✓          |
| You can create by importing an Excel or CSV file            |            ✓            |                      |
| You can connect the record type to an object from another application|            ✓            |                      |
| You can connect to other record types               |            ✓            |                    |
| You can view their associated records in a table view       |            ✓            |           ✓          |
| You can view their associated records in a timeline view    |            ✓            |           ✓          |

-->
