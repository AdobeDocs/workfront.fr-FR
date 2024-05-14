---
title: Présentation des types d’enregistrement
description: Les types d’enregistrement sont les blocs de construction d’un espace de travail Adobe Workfront Planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 1de095b3-78d9-44df-a678-51f4238deb91
source-git-commit: b2ec979cf9aa2431c8c908440c227758d9dab521
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Présentation des types d’enregistrement

{{maestro-important-intro}}

Contrairement à Workfront où les types d’objets sont prédéfinis, dans Adobe Workfront Planning, vous pouvez créer vos propres types d’objets. Par exemple, dans Workfront, les types d’objets Programme, Portfolio, Projet, Tâche ou Problème sont déjà créés.

Les types d’objets de la planification Workfront sont appelés &quot;types d’enregistrement&quot; et vous pouvez tous les créer et les personnaliser. Les types d’enregistrement sont les blocs de création d’un espace de travail de planification Workfront. Pour plus d’informations sur les espaces de travail, voir [Créer des espaces de travail](../architecture/create-workspaces.md).

## Présentation du type d’enregistrement

Dans la planification Workfront, vous pouvez créer des types d’enregistrements personnalisés qui répondent aux besoins de votre entreprise.

* Lorsque vous créez un espace de travail à partir d’un modèle, les types d’enregistrement sont créés dans les sections suivantes de l’espace de travail :

   * [Types d’enregistrement opérationnels](#operational-record-type): type d’enregistrement qui représente les plans stratégiques, les initiatives ou les travaux planifiés. Par exemple, Campaign, Activity, Tactique, Opportunity peuvent être des types d&#39;enregistrements opérationnels.
   * [Taxonomies](#taxonomy): types d’enregistrements qui capturent des attributs sur un type d’enregistrement opérationnel. Par exemple, Région, Adresse, Audience peuvent être des taxonomies.

* Lorsque vous créez un type d’enregistrement dans un espace de travail que vous avez entièrement créé, vous pouvez le placer dans n’importe quelle section que vous créez dans l’espace de travail.
* Lorsque vous créez un type d’enregistrement, seuls vous et ceux que vous autorisez à accéder à l’espace de travail pouvez afficher le type d’enregistrement.
* Vous devez créer un espace de travail avant de pouvoir créer des types d’enregistrement pour l’espace de travail.
* Un espace de travail peut contenir un total de 1 000 types d’enregistrement, quel que soit le nombre de sections de l’espace de travail. Cela inclut les types d’enregistrements que vous créez de A à Z ou qui sont créés lors de l’utilisation d’un modèle.


<!--

### Operational Record Type{#operational-record-type}

An operational record type is a Maestro record type that represents work-related objects.  

(***********insert screen shot**************)
For more information about operational record types including how to create them, see [Create record types](../architecture/create-record-types.md). 

### Taxonomy{#taxonomy}

A taxonomy is a record type that captures attributes about an operational record type. 

(**********add screen shot**********)

For more information about taxonomy record types, see [Create a taxonomy](../architecture/create-a-taxonomy.md). 

Although creating taxonomies is identical to creating operational record types, Maestro distinguishes conceptually between an operational record type and a taxonomy record type. The purpose of taxonomies is to enhance operational record types. Taxonomies should not directly represent work objects.  (***********this is no longer true, but might be later?!: A taxonomy is a record without dates, like a static list of attributes.***********) 

(********mimic what you did above for operational record types to say that we can also import taxonomies from other applications too - this will be possible later; for example Team would be a taxonomy record type, etc*************)

For example, Audience, Region, or Address can be taxonomy-type record types.  

For more information, see [Create a taxonomy](../architecture/create-a-taxonomy.md). 

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
| You can connect to other Maestro record types               |            ✓            |                    |
| You can view their associated records in a table view       |            ✓            |           ✓          |
| You can view their associated records in a timeline view    |            ✓            |           ✓          |

-->