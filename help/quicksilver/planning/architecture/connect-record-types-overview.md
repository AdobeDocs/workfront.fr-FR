---
title: Connexion aux types d’enregistrement - Aperçu
description: Une façon d’indiquer comment les types d’enregistrements individuels sont associés les uns aux autres consiste à les connecter. En outre, vous pouvez connecter les types d’enregistrements Adobe Workfront Planning aux types d’objets d’autres applications afin d’améliorer l’expérience de vos utilisateurs et utilisatrices et de garder leur attention sur une seule application.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: d5d517a0c9a1292c37e66db07f7ed17d0a9a59e1
workflow-type: tm+mt
source-wordcount: '1021'
ht-degree: 36%

---


<!--update metadata at GA-->
<!--add mini TOC when live, already added to big TOC to get the link-->

# Connexion aux types d’enregistrement - Aperçu

<!--REMOVE THE CONTENT BELOW FROM THE "CONNECT RECORD TYPES" ARTICLE WHEN YOU TURN THIS ARTICLE LIVE- THIS IS THE SAME CONTENT AS THERE, DUPLICATED-->

Vous pouvez indiquer que les types d’enregistrement individuels sont liés les uns aux autres ou aux objets d’autres applications en les connectant.

Cet article présente la manière dont les types d’enregistrement se connectent et décrit les types de connexions que vous pouvez établir entre les types d’enregistrement et d’objet.

Pour plus d’informations sur la connexion des types d’enregistrement, voir [Connexion des types d’enregistrement](/help/quicksilver/planning/architecture/connect-record-types.md).

## Remarques concernant la connexion des types d’enregistrements

* Vous pouvez connecter les entités suivantes dans Adobe Workfront Planning :

   * Deux types d’enregistrements

     Les types d’enregistrements doivent appartenir au même espace de travail.
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

* Après avoir créé des enregistrements individuels pour un type d’enregistrement, vous pouvez sélectionner les enregistrements à connecter dans le champ de type d’enregistrement lié. Pour plus d’informations, voir [Connecter des enregistrements](/help/quicksilver/planning/records/connect-records.md).

* Lorsque vous connectez un type d’enregistrement à un autre type d’enregistrement ou à un type d’objet provenant d’une autre application, les scénarios suivants se présentent :

   * **Lorsque vous reliez deux types d’enregistrements** : un champ d’enregistrement lié est créé dans le type d’enregistrement à partir duquel vous établissez la connexion. Un champ d’enregistrement lié similaire est créé sur le type d’enregistrement auquel vous vous connectez.

     Par exemple, si vous connectez le type d’enregistrement &quot;Campagne&quot; au type d’enregistrement &quot;Produit&quot;, un champ d’enregistrement lié que vous nommez &quot;Produit lié&quot; est créé dans le type d’enregistrement Campaign. Un type d’enregistrement lié automatiquement nommé &quot;Campaign&quot; est créé sur le type d’enregistrement Produit .

   * **Lorsque vous connectez un type d&#39;enregistrement à un type d&#39;objet à partir d&#39;une autre application** :

      * Un champ d’enregistrement lié est créé sur le type d’enregistrement à partir duquel vous vous connectez. Aucun champ d’enregistrement lié n’est automatiquement créé sur le type d’objet de l’autre application.

      * La planification des champs d’enregistrement n’est pas accessible à partir des objets Workfront.
      * La planification des champs d’enregistrement est accessible à partir des ressources Experience Manager lorsque votre administrateur Workfront configure le mappage des métadonnées par le biais de l’intégration entre Workfront et Adobe Experience Manager Assets. Pour plus d’informations, voir [Configuration du mappage des métadonnées de ressource entre Adobe Workfront et Experience Manager Assets](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=fr).

   * **Lorsque vous ajoutez des champs liés (ou de recherche) à partir de l’enregistrement ou de l’objet auquel vous vous connectez** : un champ lié (ou de recherche) avec des informations de l’enregistrement auquel vous vous connectez s’affiche sur l’enregistrement à partir duquel vous vous connectez.

     Vous pouvez connecter des champs d’autres types d’enregistrement ou d’objets d’une autre application au type d’enregistrement de Workfront Planning.

     Les champs liés sont en lecture seule et affichent automatiquement les informations des enregistrements ou des objets connectés lorsque vous connectez les enregistrements ou les objets.

     Par exemple, si vous connectez le type d’enregistrement « Campagne » à un projet Workfront et que vous choisissez d’intégrer le champ Date d’achèvement prévue du projet à l’enregistrement Workfront Planning, un champ lié nommé Date d’achèvement prévue (du projet) est automatiquement créé pour la campagne. Vous ne pouvez pas modifier manuellement ce champ lié. Le champ Date d’achèvement prévue (du projet) affiche la date d’achèvement prévue des projets liés.

     >[!IMPORTANT]
     >
     >Toute personne disposant d’autorisations d’affichage ou supérieures sur l’espace de travail peut afficher les informations dans les champs liés, indépendamment de ses autorisations ou de son niveau d’accès dans l’application des types d’objets liés.

* Les champs d’enregistrement liés sont précédés d’une icône de relation ![](assets/relationship-field-icon.png).

  Les champs liés sont précédés d’une icône qui identifie le type de champ. Par exemple, les champs liés (ou recherche) sont précédés d’icônes indiquant qu’un champ est un nombre, un paragraphe ou une date.

* Les champs de recherche sont précédés d’une icône qui indique le type d’information affiché dans le champ.

## Types de connexion

Après avoir établi une connexion entre deux types d’enregistrements ou entre un type d’enregistrement et d’objet à partir d’une autre application, vous pouvez ajouter des enregistrements dans les champs d’enregistrement connectés.

Selon le nombre d’enregistrements que vous pouvez ajouter à une connexion, voici les types de connexions parmi lesquels vous pouvez choisir lors de la connexion des types d’enregistrements :

* [Un à plusieurs](#one-to-many-connection-type)
* [Un à un](#many-to-one-connection-type)
* [Beaucoup à un](#many-to-one-connection-type)
* [Beaucoup à plusieurs](#many-to-many-connection-type)

<!-- add screen shots for each type of connection below-->

### Type de connexion un-à-multiple

Lorsque vous sélectionnez le type de connexion un-à-multiple entre les types d’enregistrement, vous pouvez ensuite connecter un enregistrement à plusieurs enregistrements auxquels vous vous connectez.

Par exemple, si vous connectez des campagnes à des projets, vous pouvez connecter une campagne à plusieurs projets. Mais un projet ne peut être connecté qu&#39;à une seule campagne.

Lorsque vous sélectionnez ce type de connexion, vous ne pouvez le changer plus tard que pour un type de connexion multiple-à-multiple.

### Type de connexion un-à-un

Lorsque vous sélectionnez le type de connexion un-à-un entre les types d’enregistrement, vous pouvez ensuite connecter un enregistrement à un autre enregistrement auquel vous vous connectez.

Par exemple, si vous connectez des campagnes à des projets, vous pouvez connecter une campagne à un seul projet. Un projet ne peut être connecté qu’à une seule campagne.

Lorsque vous sélectionnez ce type de connexion, vous pouvez le modifier ultérieurement en tout autre type de connexion.

### Type de connexion multiple-à-un

Lorsque vous sélectionnez le type de connexion multiple-à-un entre les types d’enregistrement, vous pouvez ensuite connecter plusieurs enregistrements avec un seul enregistrement auquel vous vous connectez.

Par exemple, si vous connectez des campagnes à des projets, vous pouvez connecter plusieurs campagnes à un seul projet. Un projet peut être connecté à plusieurs opérations.

Lorsque vous sélectionnez ce type de connexion, vous ne pouvez le changer plus tard que pour un type de connexion multiple-à-multiple.

### Type de connexion multiple-à-multiple

Lorsque vous sélectionnez le type de connexion multiple-à-multiple entre les types d’enregistrement, vous pouvez ensuite connecter de nombreux enregistrements à plusieurs enregistrements auxquels vous vous connectez.

Par exemple, si vous connectez des campagnes à des projets, vous pouvez connecter plusieurs campagnes à plusieurs projets. Vous pouvez également connecter plusieurs projets à plusieurs campagnes.

Lorsque vous sélectionnez ce type de connexion, vous ne pouvez pas le modifier après l’avoir enregistré.