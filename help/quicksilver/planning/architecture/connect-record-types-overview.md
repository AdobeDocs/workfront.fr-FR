---
title: Présentation des types d’enregistrement connectés
description: Une façon d’indiquer comment les types d’enregistrements individuels sont associés les uns aux autres consiste à les connecter. En outre, vous pouvez connecter les types d’enregistrements Adobe Workfront Planning aux types d’objets d’autres applications afin d’améliorer l’expérience de vos utilisateurs et utilisatrices et de garder leur attention sur une seule application.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 1c04c68b-7a7f-46ae-b750-2b1f79855de4
source-git-commit: e82cf1b586ea3b08f419802bd1e88c6567b61b95
workflow-type: tm+mt
source-wordcount: '1522'
ht-degree: 21%

---

# Types d’enregistrement connectés - Aperçu

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de manière générale. Il est disponible uniquement dans l’environnement Aperçu pour tous les clients. Après les versions mensuelles de Production, les mêmes fonctionnalités sont également disponibles dans l’environnement Production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, consultez la section [Activer ou désactiver les versions rapides pour votre entreprise](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

Vous pouvez indiquer que les types d’enregistrement individuels sont liés les uns aux autres ou aux objets d’autres applications en les connectant.

Cet article présente un aperçu des connexions de type enregistrement et décrit les types de connexions que vous pouvez établir entre les types d’enregistrement et d’objet.

Pour plus d’informations sur la connexion des types d’enregistrement, voir [Connexion des types d’enregistrement](/help/quicksilver/planning/architecture/connect-record-types.md).

## Remarques concernant la connexion des types d’enregistrement

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

* Après avoir créé des enregistrements pour les types d’enregistrements connectés, vous pouvez les lier les uns aux autres par le biais du champ d’enregistrement connecté.  Pour plus d’informations, consultez [Connecter des enregistrements](/help/quicksilver/planning/records/connect-records.md).

* Lorsque vous connectez un type d’enregistrement à un autre type d’enregistrement ou à un type d’objet provenant d’une autre application, les scénarios suivants se présentent :

   * **Lorsque vous connectez deux types d’enregistrements Planning** : un champ d’enregistrement lié est créé sur le type d’enregistrement à partir duquel vous vous connectez. Un champ d’enregistrement lié similaire est créé dans le type d’enregistrement auquel vous vous connectez.

     Par exemple, si vous connectez le type d’enregistrement &quot;Campagne&quot; au type d’enregistrement &quot;Produit&quot;, un champ d’enregistrement lié (champ de connexion) que vous nommez &quot;Produit lié&quot; est créé dans le type d’enregistrement Campaign. Un type d’enregistrement lié automatiquement nommé &quot;Campaign&quot; est créé sur le type d’enregistrement Produit .

   * **Lorsque vous connectez un type d&#39;enregistrement à un type d&#39;objet à partir d&#39;une autre application** :

      * Un champ d’enregistrement lié est créé sur le type d’enregistrement à partir duquel vous vous connectez. Aucun champ d’enregistrement lié n’est automatiquement créé dans le type d’objet de l’autre application.
      * La planification des champs d’enregistrement n’est pas accessible à partir des objets Workfront.
      * Les enregistrements de planification sont visibles à partir de l’onglet Planification de l’objet Workfront. Pour plus d’informations, voir [Gestion des enregistrements dans la section Planification des objets Adobe Workfront](/help/quicksilver/planning/records/manage-records-in-planning-section.md).
      * <span class="preview">Vous pouvez créer un champ personnalisé Planification de la connexion et le joindre au formulaire personnalisé d’un objet Workfront. Pour plus d’informations, voir [Création d’un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md). </span>
      * La planification des champs d’enregistrement est accessible à partir des ressources Experience Manager lorsque votre administrateur Workfront configure le mappage des métadonnées par le biais de l’intégration entre Workfront et Adobe Experience Manager Assets. Pour plus d’informations, voir [Configuration du mappage des métadonnées de ressource entre Adobe Workfront et Experience Manager Assets](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=fr).


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

## Types de connexion

Après avoir établi une connexion entre deux types d’enregistrements ou entre un type d’enregistrement et d’objet à partir d’une autre application, vous pouvez ajouter des enregistrements dans les champs d’enregistrement connectés.

Selon le nombre d’enregistrements que vous pouvez ajouter à un champ d’enregistrement connecté, voici les types de connexions parmi lesquels vous pouvez choisir lors de la connexion des types d’enregistrement :

* [Multiple-à-multiple](#many-to-many-connection-type)
* [Un-à-multiple](#one-to-many-connection-type)
* [Multiple-à-un](#many-to-one-connection-type)
* [Un-à-un](#many-to-one-connection-type)

>[!WARNING]
>
>Ces options ne sont pas disponibles lors de la connexion des éléments suivants :
>
>* Deux enregistrements provenant de différents espaces de travail
>
>* Type d’enregistrement et ressources Experience Manager

### Type de connexion multiple-à-multiple

![](assets/many-to-many-connection-picker.png)

Lorsque vous créez une connexion de type &quot;plusieurs à plusieurs&quot; entre des types d’enregistrement, vous pouvez ensuite sélectionner plusieurs enregistrements dans le champ de connexion à partir des deux types d’enregistrement.

Par exemple, si vous créez une connexion de type &quot;plusieurs à plusieurs&quot; entre des campagnes et des projets, vous pouvez sélectionner plusieurs projets pour chaque campagne et plusieurs campagnes pour chaque projet.

Un exemple réel d&#39;un type de relation multiple-à-multiple est la relation entre les films et les acteurs. Chaque film peut avoir plusieurs acteurs, et chaque acteur peut jouer dans plusieurs films.

Lorsque vous sélectionnez ce type de connexion, vous ne pouvez pas le modifier après l’avoir enregistré.

### Type de connexion un-à-multiple

![](assets/one-to-many-connection-picker.png)


Lorsque vous créez une connexion un-à-multiple entre les types d’enregistrement, vous pouvez ensuite sélectionner plusieurs enregistrements dans le champ de connexion du type d’enregistrement actif, mais le champ de connexion correspondant dans le type d’enregistrement auquel vous vous connectez permettra de sélectionner un seul enregistrement. Le champ d’enregistrement connecté automatiquement créé sur le deuxième type d’enregistrement est automatiquement défini sur un type de relation multiple-à-un.

Par exemple, si vous créez une connexion un-à-multiple entre des campagnes et des projets, vous pouvez sélectionner plusieurs projets pour chaque campagne, mais chaque projet ne peut être connecté qu’à une seule campagne.

Un exemple réel d&#39;un type de relation de type &quot;un à plusieurs&quot; est la relation entre les bibliothèques et les livres : une bibliothèque a de nombreux livres dans son inventaire ; mais un livre particulier ne peut se trouver que dans une seule bibliothèque à un moment donné.

Lorsque vous sélectionnez ce type de connexion, vous ne pouvez le changer plus tard que pour un type de connexion multiple-à-multiple.

### Type de connexion multiple-à-un

![](assets/many-to-one-connection-picker.png)


Lorsque vous créez une connexion multiple-à-un entre les types d’enregistrement, vous pouvez ensuite connecter chaque enregistrement du type d’enregistrement actif à un seul enregistrement du type d’enregistrement connecté. Le champ d’enregistrement connecté automatiquement créé dans le deuxième type d’enregistrement est automatiquement défini sur un type de relation un-à-multiple.

Par exemple, si vous connectez des campagnes à des projets et que vous choisissez ce type de connexion, vous ne pouvez ajouter qu’un seul projet à une campagne. Vous pouvez toutefois ajouter plusieurs campagnes à un seul projet.

Un exemple réel d&#39;un type de relation multiple-à-un est la relation entre de nombreux films et un acteur : un acteur peut être dans de nombreux films, mais chaque film ne peut avoir qu&#39;un acteur spécifique une fois dans sa diffusion.

Lorsque vous sélectionnez ce type de connexion, vous ne pouvez le changer plus tard que pour un type de connexion multiple-à-multiple.

### Type de connexion un-à-un

![](assets/one-to-one-connection-picker.png)

Lorsque vous créez une connexion un-à-un entre les types d’enregistrement, dans les deux types d’enregistrement, vous ne pouvez connecter chaque enregistrement qu’à un seul enregistrement de l’autre type.

Par exemple, si vous connectez des campagnes à des projets et que vous choisissez ce type de connexion, vous pouvez connecter une campagne à un seul projet. Un projet ne peut être connecté qu’à une seule campagne.

Un exemple réel de relation un-à-un est celui existant entre une personne et l&#39;identifiant unique de son pays (comme un numéro de sécurité sociale, un passeport, un identifiant d&#39;identification local) : chaque personne n&#39;a qu&#39;un seul identifiant unique pour un pays et chaque identifiant unique ne peut être associé qu&#39;à une seule personne.

Lorsque vous sélectionnez ce type de connexion, vous pouvez le modifier ultérieurement en tout autre type de connexion.
