---
title: Types d’enregistrements connectés - Aperçu
description: Une façon d’indiquer comment les types d’enregistrements individuels sont associés les uns aux autres consiste à les connecter. En outre, vous pouvez connecter les types d’enregistrements Adobe Workfront Planning aux types d’objets d’autres applications afin d’améliorer l’expérience de vos utilisateurs et utilisatrices et de garder leur attention sur une seule application.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 1c04c68b-7a7f-46ae-b750-2b1f79855de4
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '2020'
ht-degree: 13%

---


<!--keep the 30 limit verbiage in yellow til Jan 2026-->

# Types d’enregistrements connectés - Aperçu

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de manière générale. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Après les versions mensuelles en production, les mêmes fonctionnalités sont également disponibles dans l’environnement de production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, consultez la section [Activer ou désactiver les versions rapides pour votre entreprise](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

Vous pouvez indiquer que des types d’enregistrements individuels sont liés les uns aux autres ou à des objets d’autres applications en les connectant.

Cet article présente un aperçu des connexions de type enregistrement et décrit les types de connexions que vous pouvez établir entre les types d&#39;enregistrement et d&#39;objet.

Pour plus d’informations sur la connexion des types d’enregistrements, voir [Connexion des types d’enregistrements](/help/quicksilver/planning/architecture/connect-record-types.md).

## Remarques concernant la connexion des types d’enregistrement

Dans Workfront Planning, les connexions se font en deux étapes :

1. Etablissez une connexion entre deux types d&#39;enregistrements ou un type d&#39;enregistrement et un type d&#39;objet à partir d&#39;une autre application.

   Pour plus d’informations sur la connexion des types d’enregistrements, voir [Connexion des types d’enregistrements](/help/quicksilver/planning/architecture/connect-record-types.md).

1. Connecter un enregistrement individuel d&#39;un type avec des enregistrements d&#39;un autre type après la connexion des deux types d&#39;enregistrements. Pour plus d&#39;informations sur la connexion des enregistrements, voir [Connexion des enregistrements](/help/quicksilver/planning/records/connect-records.md).

Tenez compte des points suivants concernant la connexion des types d’enregistrements :

* <span class="preview">Dans Workfront Planning, vous pouvez avoir jusqu’à 30 champs connectés pour un type d’enregistrement.</span>

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

   * Adobe GenStudio for Performance Marketing

      * Marques

     >[!IMPORTANT]
     >
     >Vous devez disposer des éléments suivants pour vous connecter aux marques Adobe Experience Manager Assets et GenStudio :
     >* Une licence Adobe Experience Manager Assets
     >* Une licence Adobe GenStudio for Performance Marketing
     >* L’instance de Workfront de votre organisation doit être intégrée à Adobe Business Platform ou à Adobe Admin Console pour connecter les enregistrements Workfront Planning à Adobe Experience Manager Assets.
     >Pour plus d’informations sur Adobe Admin Console, consultez la [FAQ sur l’expérience unifiée Adobe](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md).

* Après avoir créé des enregistrements pour les types d’enregistrements, vous pouvez les lier les uns aux autres par le biais du champ d’enregistrement connecté.

  Pour plus d’informations, consultez [Connecter des enregistrements](/help/quicksilver/planning/records/connect-records.md).

* Lorsque vous connectez un type d’enregistrement à un autre type d’enregistrement ou à un type d’objet provenant d’une autre application, les scénarios suivants se présentent :

   * **Lorsque vous connectez deux types d&#39;enregistrements Planning** : Un champ d&#39;enregistrement lié est créé sur le type d&#39;enregistrement à partir duquel vous vous connectez. Un champ d’enregistrement lié similaire est créé sur le type d’enregistrement auquel vous vous connectez, uniquement lorsque vous activez le paramètre Créer le champ correspondant sur le type d’enregistrement lié sur l’onglet Nouvelle connexion .

     Par exemple, si vous connectez le type d’enregistrement « Campaign » au type d’enregistrement « Product », un champ d’enregistrement lié (champ de connexion) que vous nommez « Produit lié » est créé sur le type d’enregistrement Campaign. Un type d’enregistrement lié automatiquement nommé « Campagne » est créé sur le type d’enregistrement Produit .

     Par exemple, les scénarios suivants existent :

      * Lorsque vous activez le paramètre Créer le champ correspondant sur le type d’enregistrement lié et que vous connectez le type d’enregistrement « Campaign » au type d’enregistrement « Produit », un champ d’enregistrement lié (champ de connexion) que vous nommez « Produit lié » est créé sur le type d’enregistrement Campaign. Un type d’enregistrement lié automatiquement nommé « Campagne » est créé sur le type d’enregistrement Produit .
      * Lorsque vous désactivez le paramètre Créer le champ correspondant sur le type d’enregistrement lié et que vous connectez le type d’enregistrement « Campaign » au type d’enregistrement « Product », un champ d’enregistrement lié (champ de connexion) que vous nommez « Produit lié » est créé sur le type d’enregistrement Campaign. Un type d’enregistrement lié automatiquement nommé « Campaign » n’est pas créé sur le type d’enregistrement Produit .

     Pour plus d’informations, voir [Connecter les types d’enregistrements](/help/quicksilver/planning/architecture/connect-record-types.md).

   * **Lorsque vous connectez un type d’enregistrement à un type d’objet à partir d’une autre application** :

      * Un champ d’enregistrement lié est créé sur le type d’enregistrement à partir duquel vous vous connectez. Aucun champ d’enregistrement lié n’est automatiquement créé dans le type d’objet de l’autre application.
      * Les champs Enregistrements Planning ne sont pas accessibles à partir des objets Workfront.
      * Les enregistrements Planning sont visibles à partir de la section Planning de l&#39;objet Workfront. Pour plus d’informations, voir [Gérer les connexions d’enregistrement à partir d’objets Workfront](/help/quicksilver/planning/records/manage-records-in-planning-section.md).
      * Vous pouvez créer un champ personnalisé de connexion Planning et le joindre au formulaire personnalisé d’un objet Workfront. Pour plus d’informations, voir [Créer un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
      * Les champs d’enregistrement Planning sont accessibles à partir des ressources Experience Manager lorsque votre administrateur Workfront configure le mappage des métadonnées grâce à l’intégration entre Workfront et Adobe Experience Manager Assets. Pour plus d’informations, consultez [Configuration du mappage des métadonnées de ressource entre Adobe Workfront et Experience Manager Assets](https://experienceleague.adobe.com/fr/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping).
      * Les champs d’enregistrement Planning ne sont pas accessibles à partir des marques dans GenStudio for Performance Marketing.

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
     <!--* <span class="preview">You must connect record types to be able to create hierarchies in Workfront Planning. When record type connections don't exist, they are automatically created when you create a hierarchy. For information, see [Create workspace hierarchies](/help/quicksilver/planning/architecture/create-workspace-hierarchies.md).</span>-->


## Types de connexion

Après avoir établi une connexion entre deux types d&#39;enregistrements ou entre un enregistrement et un type d&#39;objet à partir d&#39;une autre application, vous pouvez ajouter des enregistrements dans les champs d&#39;enregistrement connectés.

>[!WARNING]
>
>Les options décrites dans cette section ne sont pas disponibles lors de la connexion des éléments suivants :
>
>* Deux enregistrements provenant d’espaces de travail différents
>
>* Un type d’enregistrement et des ressources Experience Manager
>
>* Un type d’enregistrement et une marque Adobe GenStudio

Vous pouvez choisir de connecter un enregistrement à plusieurs enregistrements à la fois, ou un enregistrement à la fois les uns aux autres.

Voici les types de connexion que vous pouvez choisir lors de la connexion des types d’enregistrement :

* Lorsque le paramètre **Créer le champ correspondant sur le type d’enregistrement lié** est désactivé, vous pouvez choisir parmi les options suivantes :

   * [Sélection multiple](#multi-select-connection-type)
   * [Sélection unique](#single-select-connection-type)

* Lorsque le paramètre **Créer le champ correspondant sur le type d’enregistrement lié** est activé, vous pouvez choisir parmi les options suivantes :

   * [Multiple-à-multiple](#many-to-many-connection-type)
   * [Un à plusieurs](#one-to-many-connection-type)
   * [Multiple-à-un](#many-to-one-connection-type)
   * [Un à un](#many-to-one-connection-type)

### Type de connexion à sélection multiple

![Type de connexion à sélection multiple](assets/multi-select-connection-picker.png)

Lorsque vous créez une connexion à sélection multiple entre des types d’enregistrements, vous pouvez ensuite sélectionner plusieurs enregistrements connectés dans le champ de connexion à partir du type d’enregistrement d’origine.

Par exemple, si vous créez une connexion à sélection multiple entre des campagnes et des projets, vous pouvez sélectionner plusieurs projets pour une campagne. Aucun type d’enregistrement connecté à Campaign n’est créé pour le type d’objet Projet.

Après avoir sélectionné ce type de connexion, vous ne pouvez pas le modifier après l’avoir enregistré dans l’un des types suivants :

* Sélection unique
* Un à plusieurs
* Multiple-à-un
* Un à un

### Type de connexion à sélection unique

![Type de connexion à sélection unique](assets/single-select-connection-picker.png)

Lorsque vous créez une connexion à sélection unique entre les types d’enregistrements, vous pouvez ensuite sélectionner un enregistrement dans le champ de connexion à partir du type d’enregistrement d’origine.

Par exemple, si vous créez une connexion à sélection unique entre des campagnes et des sociétés, vous pouvez sélectionner une société pour une campagne. Aucun type d’enregistrement connecté à Campaign n’est créé pour le type d’objet Société.

Après avoir sélectionné ce type de connexion, vous ne pouvez pas le modifier après l’avoir enregistré dans l’une des options suivantes :

* Un à plusieurs
* Un à un

</div>


<!--
* [Many to many](#many-to-many-connection-type)
* [One to many](#one-to-many-connection-type)
* [Many to one](#many-to-one-connection-type)
* [One to one](#many-to-one-connection-type)
-->

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
