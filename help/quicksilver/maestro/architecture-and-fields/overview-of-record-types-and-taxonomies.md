---
title: Présentation des types d’enregistrement et des taxonomies
description: Les types d’enregistrement sont les blocs de création d’un espace de travail Maestro.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 1de095b3-78d9-44df-a678-51f4238deb91
source-git-commit: b02c81873d84946f8db54bcf9a1a464de38781de
workflow-type: tm+mt
source-wordcount: '542'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Présentation des types d’enregistrement et des taxonomies

>[!IMPORTANT]
>
>Les informations de cet article se rapportent à Adobe Maestro, une nouvelle offre d’Adobe.
>
>Actuellement, Adobe Maestro fait partie d’un programme bêta ouvert à un nombre limité de clients.
>
>Pour plus d’informations sur l’inscription au programme bêta de Maestro, contactez le représentant de votre compte.
>
>Pour plus d’informations, voir [Présentation d’Adobe Maestro](../maestro-overview.md).

Contrairement à Workfront où les types d’objets sont prédéfinis, dans Adobe Maestro, vous pouvez créer vos propres types d’objets. Par exemple, dans Workfront, les types d’objets Programme, Portfolio, Projet, Tâche ou Problème sont déjà créés.

Les types d’objets Maestro sont appelés &quot;types d’enregistrement&quot;. Les types d’enregistrement sont les blocs de création d’un espace de travail Maestro. Pour plus d’informations sur les espaces de travail, voir [Créer des espaces de travail](../architecture-and-fields/create-workspaces.md).

## Présentation du type d’enregistrement

Dans Maestro, vous pouvez créer des types d’enregistrements personnalisés qui répondent aux besoins de votre entreprise.

* Voici les types d’enregistrements Maestro :

   * [Type d’enregistrement opérationnel](#operational-record-type): type d’enregistrement qui représente les plans stratégiques, les initiatives ou les travaux planifiés. Par exemple, Campaign, Activity, Tactique, Opportunity peuvent être des types d&#39;enregistrements opérationnels.
   * [Taxonomie](#taxonomy): types d’enregistrements qui capturent des attributs sur un type d’enregistrement opérationnel. Par exemple, Région, Adresse, Audience peuvent être des taxonomies.

* Lorsque vous créez un type d’enregistrement, tout le monde dans votre entreprise peut le visualiser, le modifier ou le supprimer. <!--this will change with access levels and permissions-->
* Vous devez créer un espace de travail avant de pouvoir créer des types d’enregistrement pour l’espace de travail.
* Vous pouvez avoir un total cumulé de 1 000 types d’enregistrements opérationnels et taxonomies dans un espace de travail. Cela inclut les types d’enregistrement ou les taxonomies que vous créez de toutes pièces ou que vous importez à partir d’autres systèmes.

### Type d’enregistrement opérationnel{#operational-record-type}

Un type d’enregistrement opérationnel est un type d’enregistrement Maestro qui représente des objets liés au travail.

![](assets/operational-record-type-blank.png)

Pour plus d’informations sur les types d’enregistrements opérationnels, y compris sur la façon de les créer, voir [Création de types d’enregistrement](../architecture-and-fields/create-record-types.md).

### Taxonomie{#taxonomy}

Une taxonomie est un type d’enregistrement qui capture les attributs d’un type d’enregistrement opérationnel.

![](assets/taxonomy-record-type-blank.png)

Pour plus d’informations sur les types d’enregistrement de taxonomie, voir [Création d’une taxonomie](../architecture-and-fields/create-a-taxonomy.md).

Bien que la création de taxonomies soit identique à la création de types d&#39;enregistrements opérationnels, Maestro fait la distinction conceptuelle entre un type d&#39;enregistrement opérationnel et un type d&#39;enregistrement de taxonomie. L&#39;objectif des taxonomies est d&#39;améliorer les types de dossiers opérationnels. Les taxonomies ne devraient pas représenter directement des objets de travail.  <!--this is no longer true, but might be later?!: A taxonomy is a record without dates, like a static list of attributes.-->

<!--mimic what you did above for operational record types to say that we can also import taxonomies from other applications too - this will be possible later; for example Team would be a taxonomy record type, etc -->

Par exemple, Audience, Région ou Adresse peuvent être des types d’enregistrement de type taxonomie.

Pour plus d’informations, voir [Création d’une taxonomie](../architecture-and-fields/create-a-taxonomy.md).

## Similarités et différences entre les types d’enregistrements opérationnels et les taxonomies

Le tableau suivant illustre certaines similitudes et différences entre les types d&#39;enregistrements opérationnels et les taxonomies :

| Type d’enregistrement et caractéristique | Type d’enregistrement opérationnel | Type d’enregistrement de taxonomie |
|-------------------------------------------------------------|:-----------------------:|:--------------------:|
| Ils font partie d’un espace de travail | ✓ | ✓ |
| Vous pouvez les créer automatiquement à partir d&#39;un modèle d&#39;espace de travail. | ✓ | ✓ |
| Vous pouvez les créer manuellement, à partir de zéro | ✓ | ✓ |
| Vous pouvez les créer en copiant et en collant des informations à partir d’un fichier ou d’une liste externe | ✓ | ✓ |
| Vous pouvez créer en important un fichier Excel ou CSV. | ✓ |                     |
| Vous pouvez créer des types d’enregistrement en lecture seule en vous connectant aux types d’objets d’autres applications. | ✓ |                     |
| Elles représentent des objets liés au travail. | ✓ |                      |
| Elles représentent des attributs sur les objets liés au travail. |                         | ✓ |
| Vous pouvez créer entièrement | ✓ | ✓ |
| Vous pouvez créer en important un fichier Excel ou CSV. | ✓ |                      |
| Vous pouvez connecter le type d’enregistrement à un objet à partir d’une application tierce. | ✓ |                      |
| Vous pouvez vous connecter à d’autres types d’enregistrements Maestro | ✓ |                    |
| Vous pouvez afficher les enregistrements associés dans une vue de tableau. | ✓ | ✓ |
| Vous pouvez afficher les enregistrements associés dans une vue chronologique. | ✓ | ✓ |
