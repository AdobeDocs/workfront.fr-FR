---
title: Présentation des types d’enregistrement connectés
description: Une façon d’indiquer comment les types d’enregistrements individuels sont associés les uns aux autres consiste à les connecter. En outre, vous pouvez connecter les types d’enregistrements Adobe Workfront Planning aux types d’objets d’autres applications afin d’améliorer l’expérience de vos utilisateurs et utilisatrices et de garder leur attention sur une seule application.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 1ad86cd55459d92650ac7a24c41765e579f8bb94
workflow-type: tm+mt
source-wordcount: '830'
ht-degree: 34%

---


<!--update metadata at GA-->
<!--add mini TOC when live, already added to big TOC to get the link-->

# Types d’enregistrement connectés - Aperçu

<!--REMOVE THE CONTENT BELOW FROM THE "CONNECT RECORD TYPES" ARTICLE WHEN YOU TURN THIS ARTICLE LIVE- THIS IS THE SAME CONTENT AS THERE, DUPLICATED-->

Vous pouvez indiquer que les types d’enregistrement individuels sont liés les uns aux autres ou aux objets d’autres applications en les connectant.

Cet article présente un aperçu des connexions de type enregistrement et décrit les types de connexions que vous pouvez établir entre les types d’enregistrement et d’objet.

Pour plus d’informations sur la connexion des types d’enregistrement, voir [Connexion des types d’enregistrement](/help/quicksilver/planning/architecture/connect-record-types.md).

## Remarques concernant la connexion des types d’enregistrements

La planification Workfront comprend deux étapes de connexion :

1. Tout d’abord, vous devez établir une connexion entre deux types d’enregistrement ou un type d’enregistrement et un type d’objet à partir d’une autre application. Pour plus d’informations sur la connexion des types d’enregistrement, voir [Connexion des types d’enregistrement](/help/quicksilver/planning/architecture/connect-record-types.md).
1. Deuxièmement, vous pouvez connecter des enregistrements individuels d’un type avec des enregistrements d’un autre type une fois les deux types d’enregistrements connectés. Pour plus d&#39;informations sur la connexion des enregistrements, voir [Connexion des enregistrements](/help/quicksilver/planning/records/connect-records.md).

Tenez compte des points suivants concernant la connexion des types d’enregistrement :

* Vous pouvez connecter les entités suivantes dans Adobe Workfront Planning :

   * Deux types d’enregistrement.

     Par défaut, vous pouvez connecter deux types d’enregistrement à partir du même espace de travail. Vous pouvez également configurer des types d’enregistrement pour vous connecter à des types d’enregistrement à partir d’autres espaces de travail. Pour plus d’informations, voir [Modification des types d’enregistrement](/help/quicksilver/planning/architecture/edit-record-types.md).
   * Type d’enregistrement et type d’objet d’une autre application.

* Vous pouvez connecter les types d’enregistrement de Workfront Planning aux types d’objets suivants à partir des applications suivantes :

   * Adobe Workfront :

      * Projets
      * Portefeuilles
      * Programmes
      * Entreprises
      * Groupes

   * Adobe Experience Manager Assets :

      * Images
      * Dossiers

     >[!IMPORTANT]
     >
     >Vous devez disposer d’une licence Adobe Experience Manager Assets et l’instance Workfront de votre organisation doit être intégrée à Adobe Business Platform ou à Adobe Admin Console pour connecter les enregistrements Workfront Planning à Adobe Experience Manager Assets.
     >
     >Si vous avez des questions relatives à l’intégration à Adobe Admin Console, voir les [questions fréquentes Adobe Unified Experience](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md).

* Après avoir créé des enregistrements pour les types d’enregistrements connectés, vous pouvez les lier les uns aux autres par le biais du champ d’enregistrement connecté.  Pour plus d’informations, voir [Connecter des enregistrements](/help/quicksilver/planning/records/connect-records.md).

* Lorsque vous connectez un type d’enregistrement à un autre type d’enregistrement ou à un type d’objet provenant d’une autre application, les scénarios suivants se présentent :

   * **Lorsque vous connectez deux types d’enregistrements Planning** : un champ d’enregistrement lié est créé sur le type d’enregistrement à partir duquel vous vous connectez. Un champ d’enregistrement lié similaire est créé sur le type d’enregistrement auquel vous vous connectez.

     Par exemple, si vous connectez le type d’enregistrement &quot;Campagne&quot; au type d’enregistrement &quot;Produit&quot;, un champ d’enregistrement lié (champ de connexion) que vous nommez &quot;Produit lié&quot; est créé dans le type d’enregistrement Campaign. Un type d’enregistrement lié automatiquement nommé &quot;Campaign&quot; est créé sur le type d’enregistrement Produit .

   * **Lorsque vous connectez un type d&#39;enregistrement à un type d&#39;objet à partir d&#39;une autre application** :

      * Un champ d’enregistrement lié est créé sur le type d’enregistrement à partir duquel vous vous connectez. Aucun champ d’enregistrement lié n’est automatiquement créé sur le type d’objet de l’autre application.
      * La planification des champs d’enregistrement n’est pas accessible à partir des objets Workfront.
      * La planification des champs d’enregistrement est accessible à partir des ressources Experience Manager lorsque votre administrateur Workfront configure le mappage des métadonnées par le biais de l’intégration entre Workfront et Adobe Experience Manager Assets. Pour plus d’informations, voir [Configuration du mappage des métadonnées de ressource entre Adobe Workfront et Experience Manager Assets](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=fr).
      * Les enregistrements de planification sont visibles à partir de l’onglet Planification de l’objet Workfront. Pour plus d’informations, voir [Gestion des enregistrements dans la section Planification des objets Adobe Workfront](/help/quicksilver/planning/records/manage-records-in-planning-section.md).

   * **Lorsque vous ajoutez des champs de recherche à partir de l’enregistrement ou de l’objet auquel vous vous connectez** : en plus de créer un champ d’enregistrement lié, vous pouvez également vous connecter à des champs à partir de l’enregistrement ou du type d’objet connecté qui sont appelés champs de recherche. Un champ lié (ou de recherche) contenant des informations de l’enregistrement auquel vous vous connectez s’affiche sur l’enregistrement à partir duquel vous vous connectez.

     Vous pouvez connecter des champs d’autres types d’enregistrement ou d’objets d’une autre application au type d’enregistrement de Workfront Planning.

     Les champs liés sont en lecture seule et affichent automatiquement les informations des enregistrements connectés.

     Vous pouvez vous référer aux champs de recherche d’autres types d’enregistrement ou d’objets dans des formules, des filtres ou des regroupements.

     Par exemple, si vous connectez le type d’enregistrement « Campagne » à un projet Workfront et que vous choisissez d’intégrer le champ Date d’achèvement prévue du projet à l’enregistrement Workfront Planning, un champ lié nommé Date d’achèvement prévue (du projet) est automatiquement créé pour la campagne. Vous ne pouvez pas modifier manuellement ce champ lié. Le champ Date d’achèvement prévue (du projet) affiche la date d’achèvement prévue des projets liés.

     >[!IMPORTANT]
     >
     >Toute personne disposant d’autorisations de vue ou supérieures sur l’espace de travail peut afficher les informations dans les champs de recherche, indépendamment de ses autorisations ou de son niveau d’accès dans l’application des types d’objets liés ou de ses autorisations dans d’autres espaces de travail.

     Les champs d’enregistrement liés sont précédés d’une icône de relation ![](assets/relationship-field-icon.png).

     Les champs liés sont précédés d’une icône qui identifie le type de champ. Par exemple, les champs liés (ou recherche) sont précédés d’icônes indiquant qu’un champ est un nombre, un paragraphe ou une date.

<!--## Connection types

After you establish a connection between two record types or between a record and an object type from another application, you can add records in the connected record fields. 

Depending on how many records you can add to a connected record field, the following are the connection types you can choose from when connecting record types: 

* [Many to many](#many-to-many-connection-type)
* [One to many](#one-to-many-connection-type)
* [Many to one](#many-to-one-connection-type)
* [One to one](#many-to-one-connection-type)

>[!WARNING]
>
>These options are not available when connecting the following: 
>* Two records from different workspaces
>
>* A record type and Experience Manager assets

### Many-to-many connection type

![](assets/many-to-many-connection-picker.png)

When you create a many-to-many connection between record types, you can then select multiple records in the connection field from both record types. 

For example, if you create a many-to-many connection between campaigns and projects, you can select multiple projects for each campaign, and multiple campaigns for each project. 

A real-life example of a many-to-many relationship type is the relationship between movies and actors. Each movie can have multiple actors, and each actor can play in multiple movies. 

When you select this connection type, you cannot change the connection type after you save it. 

### One-to-many connection type

![](assets/one-to-many-connection-picker.png)


When you create a one-to-many connection between record types, you can then select multiple records in the connection field in the current record type, but the corresponding connection field in the record type you connect to will allow selecting only one record. The connected record field that is automatically created on the second record type is automatically set to a many-to-one relationship type. 

For example, if you create a one-to-many connection between campaigns and projects, you can select multiple projects for each campaign, but each project can be connected to only one campaign.

A real-life example of a one-to-many relationship type is the relationship between libraries and books: a library has many books in its inventory; but one particular book can only be in one library at a given point in time. 

When you select this connection type, you can later change it only to a many-to-many connection type. 

### Many-to-one connection type

![](assets/many-to-one-connection-picker.png)


When you create a many-to-one connection between record types, you can then connect each record in the current record type with only one record from the connected record type. The connected record field that is automatically created on the second record type is automatically set to a one-to-many relationship type. 

For example, if you connect campaigns with projects and you choose this type of connection, you can add only one project to a campaign. But you can add multiple campaigns to one project. 

A real-life example of a many-to-one relationship type is the relationship between many movies and one actor: one actor can be in many movies, but each movie can only have a specific actor once in its cast. 

When you select this connection type, you can later change it only to a many-to-many connection type.

### One-to-one connection type

![](assets/one-to-one-connection-picker.png)

When you create a one-to-one connection between record types, in both record types you can connect each record only with one record from the other record type.

For example, if you connect campaigns with projects and you choose this type of connection, you can connect one campaign with one project. One project can be connected only to one campaign. 

A real-life example of a one-to-one relationship is the one existing between a person and their country's unique identifier (like a Social Security Number, Passport ID, local identification ID): each person has only one unique identifier for a country and each unique identifier can be linked to only one person. 

When you select this connection type, you can later change it to any other connection type. 

-->



