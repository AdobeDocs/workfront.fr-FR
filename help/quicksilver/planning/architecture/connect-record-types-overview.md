---
title: Types d’enregistrements connectés - Aperçu
description: Une façon d’indiquer comment les types d’enregistrements individuels sont associés les uns aux autres consiste à les connecter. En outre, vous pouvez connecter les types d’enregistrements Adobe Workfront Planning aux types d’objets d’autres applications afin d’améliorer l’expérience de vos utilisateurs et utilisatrices et de garder leur attention sur une seule application.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 1c04c68b-7a7f-46ae-b750-2b1f79855de4
source-git-commit: bfb0fd2956ffb9384a09882864668d5dba33a53b
workflow-type: tm+mt
source-wordcount: '1553'
ht-degree: 17%

---

# Types d’enregistrements connectés - Aperçu

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>   -->

Vous pouvez indiquer que des types d’enregistrements individuels sont liés les uns aux autres ou à des objets d’autres applications en les connectant.

Cet article présente un aperçu des connexions de type enregistrement et décrit les types de connexions que vous pouvez établir entre les types d&#39;enregistrement et d&#39;objet.

Pour plus d’informations sur la connexion des types d’enregistrements, voir [Connexion des types d’enregistrements](/help/quicksilver/planning/architecture/connect-record-types.md).

## Remarques concernant la connexion des types d’enregistrement

Dans Workfront Planning, les connexions se font en deux étapes :

1. Etablissez une connexion entre deux types d&#39;enregistrements ou un type d&#39;enregistrement et un type d&#39;objet à partir d&#39;une autre application.

   Pour plus d’informations sur la connexion des types d’enregistrements, voir [Connexion des types d’enregistrements](/help/quicksilver/planning/architecture/connect-record-types.md).

1. Connecter un enregistrement individuel d&#39;un type avec des enregistrements d&#39;un autre type après la connexion des deux types d&#39;enregistrements. Pour plus d&#39;informations sur la connexion des enregistrements, voir [Connexion des enregistrements](/help/quicksilver/planning/records/connect-records.md).

Tenez compte des points suivants concernant la connexion des types d’enregistrements :

* Vous pouvez connecter les entités suivantes dans Adobe Workfront Planning :

   * Deux types d’enregistrement.

     Par défaut, vous pouvez connecter deux types d’enregistrements à partir du même espace de travail. Vous pouvez également configurer des types d’enregistrements pour vous connecter à des types d’enregistrements d’autres espaces de travail. Pour plus d’informations, voir [Modifier les types d’enregistrements](/help/quicksilver/planning/architecture/edit-record-types.md).
   * Type d’enregistrement et type d’objet d’une autre application.

* Vous pouvez connecter des types d&#39;enregistrements Workfront Planning aux types d&#39;objets suivants à partir des applications suivantes :

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

* Après avoir créé des enregistrements pour les types d’enregistrements, vous pouvez les lier les uns aux autres par le biais du champ d’enregistrement connecté.

  Pour plus d’informations, consultez [Connecter des enregistrements](/help/quicksilver/planning/records/connect-records.md).

* Lorsque vous connectez un type d’enregistrement à un autre type d’enregistrement ou à un type d’objet provenant d’une autre application, les scénarios suivants se présentent :

   * **Lorsque vous connectez deux types d&#39;enregistrements Planning** : Un champ d&#39;enregistrement lié est créé sur le type d&#39;enregistrement à partir duquel vous vous connectez. Un champ d’enregistrement lié similaire est créé sur le type d’enregistrement auquel vous vous connectez <!--<span class="preview">, only when you enable the Create corresponding field on linked record type setting on the New connection tab.</span>-->.

     Par exemple, si vous connectez le type d’enregistrement « Campaign » au type d’enregistrement « Product », un champ d’enregistrement lié (champ de connexion) que vous nommez « Produit lié » est créé sur le type d’enregistrement Campaign. Un type d’enregistrement lié automatiquement nommé « Campagne » est créé sur le type d’enregistrement Produit .

     <!--<div class="preview">
        
        For example, the following scenarios exist: 
        * When you enable the Create corresponding field on linked record type setting and you connect the "Campaign" record type with the "Product" record type, a linked record field (connection field) that you name "Linked Product" is created on the Campaign record type. A linked record type automatically named "Campaign" is created on the Product record type.
        * When you disable the Create corresponding field on linked record type setting and you connect the "Campaign" record type with the "Product" record type, a linked record field (connection field) that you name "Linked Product" is created on the Campaign record type. A linked record type automatically named "Campaign" is not created on the Product record type.
        </div>-->

     Pour plus d’informations, voir [Connecter les types d’enregistrements](/help/quicksilver/planning/architecture/connect-record-types.md).

   * **Lorsque vous connectez un type d’enregistrement à un type d’objet à partir d’une autre application** :

      * Un champ d’enregistrement lié est créé sur le type d’enregistrement à partir duquel vous vous connectez. Aucun champ d’enregistrement lié n’est automatiquement créé dans le type d’objet de l’autre application.
      * Les champs Enregistrements Planning ne sont pas accessibles à partir des objets Workfront.
      * Les enregistrements Planning sont visibles à partir de l&#39;onglet Planning de l&#39;objet Workfront. Pour plus d’informations, voir [Gérer les connexions d’enregistrement à partir d’objets Workfront](/help/quicksilver/planning/records/manage-records-in-planning-section.md).
      * Vous pouvez créer un champ personnalisé de connexion Planning et le joindre au formulaire personnalisé d’un objet Workfront. Pour plus d’informations, voir [Créer un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
      * Les champs d’enregistrement Planning sont accessibles à partir des ressources Experience Manager lorsque votre administrateur Workfront configure le mappage des métadonnées grâce à l’intégration entre Workfront et Adobe Experience Manager Assets. Pour plus d’informations, consultez [Configuration du mappage des métadonnées de ressource entre Adobe Workfront et Experience Manager Assets](https://experienceleague.adobe.com/fr/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping).


   * **Lorsque vous ajoutez des champs de recherche à partir de l’enregistrement ou de l’objet auquel vous vous connectez** : en plus de créer un champ d’enregistrement lié, vous pouvez également vous connecter aux champs du type d’enregistrement ou d’objet connecté qui sont appelés champs de recherche. Un champ lié (ou de recherche) contenant des informations de l&#39;enregistrement auquel vous vous connectez s&#39;affiche sur l&#39;enregistrement auquel vous vous connectez.

     Vous pouvez connecter des champs d’autres types d’enregistrements ou des objets d’une autre application au type d’enregistrement Workfront Planning.

     Les champs liés sont en lecture seule et affichent automatiquement les informations des enregistrements connectés.

     Vous pouvez vous référer aux champs de recherche d&#39;autres types d&#39;enregistrements ou d&#39;objets dans des formules, des filtres ou des regroupements.

     Par exemple, si vous connectez le type d’enregistrement « Campagne » à un projet Workfront et que vous choisissez d’intégrer le champ Date d’achèvement prévue du projet à l’enregistrement Workfront Planning, un champ lié nommé Date d’achèvement prévue (du projet) est automatiquement créé pour la campagne. Vous ne pouvez pas modifier manuellement ce champ lié. Le champ Date d’achèvement prévue (du projet) affiche la date d’achèvement prévue des projets liés.

     >[!IMPORTANT]
     >
     >Toute personne disposant d&#39;autorisations d&#39;affichage ou supérieures pour l&#39;espace de travail peut afficher les informations dans les champs de recherche, quels que soient ses autorisations ou son niveau d&#39;accès dans l&#39;application des types d&#39;objets liés ou ses autorisations dans d&#39;autres espaces de travail.

     Les champs d’enregistrement liés sont précédés d’une icône de relation ![icône de champ de relation](assets/relationship-field-icon.png).

     Les champs liés sont précédés d’une icône qui identifie le type de champ. Par exemple, les champs liés (ou de recherche) sont précédés d’icônes indiquant qu’un champ est un nombre, un paragraphe ou une date.

     >[!TIP]
     >
     >Les informations du champ de date des objets Workfront s’affichent au format 24 heures dans Workfront Planning, quelle que soit la manière dont elles s’affichent dans Workfront.
     >
     >Par exemple, si la date de début prévue d’un projet s’affiche à 15 :00 dans Workfront, elle s’affiche à 15 :00 dans Workfront Planning dans un champ de recherche importé.


## Types de connexion

Après avoir établi une connexion entre deux types d&#39;enregistrements ou entre un enregistrement et un type d&#39;objet à partir d&#39;une autre application, vous pouvez ajouter des enregistrements dans les champs d&#39;enregistrement connectés.

>[!WARNING]
>
>Ces options ne sont pas disponibles lors de la connexion des éléments suivants :
>
>* Deux enregistrements provenant d’espaces de travail différents
>
>* Un type d’enregistrement et des ressources Experience Manager

Vous pouvez choisir de connecter un enregistrement à plusieurs enregistrements à la fois, ou un enregistrement à la fois les uns aux autres.

Selon le nombre d’enregistrements que vous pouvez ajouter à un champ d’enregistrement connecté <!--and the environment you use to create the connected fields-->, voici les types de connexion que vous pouvez choisir lors de la connexion des types d’enregistrements :

<!--replace the list of 4 connection types at the bottom of this commented-out section with this entire section, whenw e release to preview: 

<div class="preview">

* In the Preview environment: 

    * When the Create corresponding field on linked record type setting is disabled, you can choose from: 

        * [Multi-select](#multi-select-connection-type)
        * [Single-select](#single-select-connection-type)

</div>

* <span class="preview">In the Preview environment, when the Create corresponding field on linked record type setting is enabled,</span> or in the Production environment, you can choose from:

    * [Many to many](#many-to-many-connection-type)
    * [One to many](#one-to-many-connection-type)
    * [Many to one](#many-to-one-connection-type)
    * [One to one](#many-to-one-connection-type) 

<div class="preview">

### Multi-select connection type

![Multi-select connection type](assets/multi-select-connection-picker.png)

When you create a multi-select connection between record types, you can then select multiple connected records in the connection field from the original record type. 

For example, if you create a multi-select connection between campaigns and projects, you can select multiple projects for one campaign. A Campaign connected record type is not created for the Project object type.

After you select this connection type, you cannot change the connection type after you save it to any of the following types:

    * Single-select
    * One to many
    * Many to one
    * One to one

### Single-select connection type

![Single select connection type](assets/single-select-connection-picker.png)

When you create a single-select connection between record types, you can then select one record in the connection field from the original record type. 

For example, if you create a single-select connection between campaigns and companies, you can select one company for one campaign. A Campaign connected record type is not created for the Company object type.

After you select this connection type, you cannot change the connection type after you save it to any of the following:

    * One to many
    * One to one

</div>

-->

* [Multiple-à-multiple](#many-to-many-connection-type)
* [Un à plusieurs](#one-to-many-connection-type)
* [Multiple-à-un](#many-to-one-connection-type)
* [Un à un](#many-to-one-connection-type)

### Type de connexion plusieurs à plusieurs

![Sélecteur de connexion plusieurs à plusieurs](assets/many-to-many-connection-picker.png)

Lorsque vous créez une connexion multiple-à-multiple entre des types d’enregistrements, vous pouvez ensuite sélectionner plusieurs enregistrements dans le champ de connexion à partir des deux types d’enregistrements.

Par exemple, si vous créez une connexion multiple-à-multiple entre des campagnes et des projets, vous pouvez sélectionner plusieurs projets pour chaque campagne et plusieurs campagnes pour chaque projet.

Un exemple concret de relation multiple-à-multiple est la relation entre les films et les acteurs. Chaque film peut avoir plusieurs acteurs, et chaque acteur peut jouer dans plusieurs films.

Lorsque vous sélectionnez ce type de connexion, vous ne pouvez pas le modifier après l’avoir enregistré.

### Type de connexion un-à-plusieurs

![Sélecteur de connexion un à plusieurs](assets/one-to-many-connection-picker.png)


Lorsque vous créez une connexion un-à-plusieurs entre les types d’enregistrement, vous pouvez ensuite sélectionner plusieurs enregistrements dans le champ de connexion du type d’enregistrement actif, mais le champ de connexion correspondant dans le type d’enregistrement auquel vous vous connectez permettra de sélectionner un seul enregistrement. Le champ d’enregistrement connecté qui est automatiquement créé sur le deuxième type d’enregistrement est automatiquement défini sur un type de relation multiple-à-un.

Par exemple, si vous créez une connexion un-à-plusieurs entre des campagnes et des projets, vous pouvez sélectionner plusieurs projets pour chaque campagne, mais chaque projet ne peut être connecté qu’à une seule campagne.

Un exemple concret de relation un-à-plusieurs est la relation entre les bibliothèques et les livres : une bibliothèque a de nombreux livres dans son inventaire, mais un livre particulier ne peut se trouver que dans une seule bibliothèque à un moment donné.

Lorsque vous sélectionnez ce type de connexion, vous pouvez le modifier ultérieurement pour passer uniquement à un type de connexion multiple-à-multiple.

### Type de connexion multiple-à-un

![Sélecteur de connexion plusieurs à un](assets/many-to-one-connection-picker.png)


Lorsque vous créez une connexion multiple-à-un entre les types d’enregistrement, vous pouvez ensuite connecter chaque enregistrement du type d’enregistrement actif à un seul enregistrement du type d’enregistrement connecté. Le champ d’enregistrement connecté qui est automatiquement créé sur le deuxième type d’enregistrement est automatiquement défini sur un type de relation un-à-plusieurs.

Par exemple, si vous connectez des campagnes à des projets et que vous choisissez ce type de connexion, vous ne pouvez ajouter qu’un seul projet à une campagne. Cependant, vous pouvez ajouter plusieurs campagnes à un projet.

Un exemple concret d’une relation multiple-à-un est la relation entre de nombreux films et un acteur : un acteur peut être dans de nombreux films, mais chaque film ne peut avoir un acteur spécifique qu’une seule fois dans son casting.

Lorsque vous sélectionnez ce type de connexion, vous pouvez le modifier ultérieurement pour passer uniquement à un type de connexion multiple-à-multiple.

### Type de connexion un-à-un

![Sélecteur de connexion un à un](assets/one-to-one-connection-picker.png)

Lorsque vous créez une connexion un-à-un entre les types d&#39;enregistrements, dans les deux types d&#39;enregistrements, vous ne pouvez connecter chaque enregistrement qu&#39;à un seul enregistrement de l&#39;autre type d&#39;enregistrement.

Par exemple, si vous connectez des campagnes à des projets et que vous choisissez ce type de connexion, vous pouvez connecter une campagne à un projet. Un projet ne peut être connecté qu’à une seule campagne.

Un exemple réel de relation un-à-un est celui qui existe entre une personne et l’identifiant unique de son pays (comme un numéro de sécurité sociale, un identifiant de passeport, un identifiant d’identification locale) : chaque personne n’a qu’un identifiant unique pour un pays et chaque identifiant unique ne peut être associé qu’à une seule personne.

Lorsque vous sélectionnez ce type de connexion, vous pouvez le modifier ultérieurement en tout autre type de connexion.
