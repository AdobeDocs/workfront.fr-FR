---
title: Connecter des types d’enregistrements
description: Une façon d’indiquer comment les types d’enregistrement individuels sont associés les uns aux autres consiste à les connecter. En outre, vous pouvez connecter les types d’enregistrement Adobe Workfront Planning aux types d’objets d’autres applications afin d’améliorer l’expérience de vos utilisateurs et de garder leur focus dans une seule application.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: ae794ebe-4597-47a4-9ef3-3f4d31cb70c2
source-git-commit: 49335ec86057e4985477034558a271bf4efcab5e
workflow-type: tm+mt
source-wordcount: '2253'
ht-degree: 2%

---

<!-----
title: Connect record types
description: A way to indicate how individual record types relate to one another is to connect them. Also, you can connect Adobe Workfront Planning record types with object types from other applications to enhance your users' experience and keep their focus in one application.
hidefromtoc: yes
hide: yes
feature: Work management
role: User
author: Alina
--->

<!--update the metadata with real information when making this avilable in TOC and in the left nav-->
<!--************ THIS MIGHT NO LONGER BE A 'RELATIONSHIP' TYPE FIELD, BECAUSE THEY WILL SHOW IT IN THE CONNECTION TAB*****************************-->


# Connecter des types d’enregistrements

{{planning-important-intro}}

Vous pouvez utiliser la planification Adobe Workfront pour concevoir des espaces de travail entièrement personnalisables contenant les types d’enregistrement nécessaires dans votre entreprise. Une façon d’indiquer comment les types d’enregistrement individuels sont associés les uns aux autres consiste à les connecter. En outre, vous pouvez connecter les types d’enregistrement de Workfront Planning aux types d’objets d’autres applications afin d’améliorer l’expérience de vos utilisateurs et de garder leur focus dans une seule application.

Vous pouvez connecter des types d’enregistrement les uns aux autres ou des types d’enregistrement avec des types d’objet provenant d’autres applications.

Vous pouvez ainsi afficher les champs de l’enregistrement ou du type d’objet lié sur un enregistrement Workfront Planning.

Cet article décrit comment connecter deux types d’enregistrement dans Workfront Planning ou un type d’enregistrement à un objet d’une autre application.

Après avoir établi la connexion entre les enregistrements ou les types d’objets, vous pouvez connecter des enregistrements individuels les uns aux autres.

Pour plus d’informations sur la connexion d’un enregistrement Workfront Planning à un objet à partir d’une autre application, voir [Connexion d’enregistrements](../records/connect-records.md).

Pour un exemple de connexion des types d’enregistrement, voir [Exemple de connexion de types d&#39;enregistrements et d&#39;enregistrements](../architecture/example-connect-record-types-and-records.md).

<!--ensure this last linked article is right; the title and the link should have changed-->

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Produit</p> </td>
   <td>
   <p> Adobe Workfront</p> <p>Pour connecter les types d’enregistrements Adobe Workfront Planning à Experience Manager Assets, vous devez disposer d’une licence Adobe Experience Manager Assets et l’instance de Workfront de votre entreprise doit être intégrée à l’expérience unifiée de l’Adobe. Pour plus d’informations, voir <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe d’une expérience unifiée pour Workfront</a>.</p> </td>
  </tr>  
 <td role="rowheader"><p>Accord Adobe Workfront</p></td>
   <td>
<p>Votre entreprise doit être inscrite au programme bêta fermé d’Adobe Workfront Planning. Contactez le représentant de votre compte pour en savoir plus sur cette nouvelle offre. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Forfait Adobe Workfront</p></td>
   <td>
<p>N’importe quelle</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licence Adobe Workfront</p></td>
   <td>
   <p>N’importe quelle</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configurations du niveau d’accès</p></td>
   <td> <p>Il n’existe aucun contrôle de niveau d’accès pour Adobe Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Modèle de mise en page</p></td>
   <td> <p>L’administrateur de Workfront ou de groupe doit ajouter la zone Planning dans votre modèle de mise en page. Pour plus d’informations, voir <a href="../access/access-overview.md">Présentation de l’accès</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Autorisations</p></td>
   <td> <p>Gestion des autorisations d’un espace de travail</a> </p>  
   <p>Les administrateurs système disposent d’autorisations pour tous les espaces de travail, y compris ceux qu’ils n’ont pas créés.
</td>
  </tr>
 </tbody>
</table>

<!--Maybe enable this at GA - but planing is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->


## Considérations sur la connexion des types d’enregistrement

* Vous pouvez connecter les entités suivantes dans Adobe Workfront Planning :

   * Deux types d’enregistrement

     Les types d’enregistrement doivent appartenir au même espace de travail.
   * Type d’enregistrement et type d’objet d’une autre application.

* Vous pouvez connecter les types d’objets suivants à partir des applications suivantes à l’aide des types d’enregistrement de Workfront Planning :

   * ADOBE WORKFRONT :

      * Projets
      * Portefeuilles
      * Programmes
      * Entreprises
      * Groupes

   * ADOBE EXPERIENCE MANAGER ASSETS :

      * Images
      * Dossiers

     >[!IMPORTANT]
     >
     >Vous devez disposer d’une licence Adobe Experience Manager Assets et l’instance de Workfront de votre entreprise doit être intégrée à Adobe Business Platform ou à Adobe Admin Console pour connecter les enregistrements Workfront Planning à Adobe Experience Manager Assets.
     >
     >Si vous avez des questions sur l’intégration à Adobe Admin Console, reportez-vous à la section [FAQ sur l’expérience unifiée Adobe](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md).

* Après avoir créé des enregistrements individuels pour un type d&#39;enregistrement, vous pouvez sélectionner les enregistrements auxquels vous vous connectez à partir du champ type d&#39;enregistrement associé. Pour plus d’informations, voir [Connexion d’enregistrements](../records/connect-records.md).

* Après avoir connecté un type d’enregistrement à un autre type d’enregistrement ou à un type d’objet d’une autre application, les scénarios suivants existent :

   * **Lorsque vous connectez deux types d’enregistrements**: un champ d’enregistrement lié est créé sur le type d’enregistrement à partir duquel vous vous connectez. Un champ d’enregistrement lié similaire est créé sur le type d’enregistrement auquel vous vous connectez.

     Par exemple, si vous connectez le type d’enregistrement &quot;Campagne&quot; au type d’enregistrement &quot;Produit&quot;, un champ d’enregistrement lié que vous nommez &quot;Produit lié&quot; est créé sur le type d’enregistrement Campaign et un type d’enregistrement lié automatiquement nommé &quot;Campagne&quot; est créé sur le type d’enregistrement Produit .

   * **Lorsque vous connectez un type d’enregistrement à un type d’objet d’une autre application**: un champ d’enregistrement lié est créé sur le type d’enregistrement à partir duquel vous vous connectez. Aucun champ d’enregistrement lié n’est automatiquement créé sur le type d’objet de l’autre application.

     Un nouveau type d’enregistrement en lecture seule de la planification Workfront est créé pour l’objet de l’autre application uniquement lorsque les objets réels sont connectés aux enregistrements de la planification Workfront.

     Pour plus d’informations, voir [Connexion d’enregistrements](../records/connect-records.md).

   * **Lorsque vous ajoutez des champs de recherche de l’enregistrement ou de l’objet auquel vous vous connectez.**: vous pouvez connecter des champs de l’objet de l’autre application au type d’enregistrement de la planification Workfront. Il s’agit de champs liés ou de recherche. Les champs liés affichent automatiquement les informations des enregistrements ou des objets connectés lorsque vous connectez les enregistrements ou les objets. Les champs de recherche liés sont toujours en lecture seule et renseignent automatiquement les valeurs des enregistrements ou objets connectés.

     Par exemple, si vous associez le type d’enregistrement &quot;Campagne&quot; à un projet Workfront et que vous choisissez d’importer le champ Date de fin planifiée du projet dans l’enregistrement de planification Workfront, un champ lié appelé Date de fin planifiée (à partir du projet) est automatiquement créé pour la campagne. Vous ne pouvez pas modifier manuellement ce champ lié. Le champ Date d’achèvement planifiée (à partir du projet) affiche la Date d’achèvement planifiée des projets liés.

     >[!IMPORTANT]
     >
     >    Toute personne disposant d’autorisations de vue ou supérieures sur l’espace de travail peut afficher les informations dans les champs liés, indépendamment de ses autorisations ou de son niveau d’accès dans l’application des types d’objets liés.

* Les champs d’enregistrement liés sont précédés d’une icône de relation ![](assets/relationship-field-icon.png).

  Les champs liés sont précédés d’une icône qui identifie le type de champ. Par exemple, des icônes qui indiquent qu’un champ est un nombre, un paragraphe ou une date.

## Connecter des types d’enregistrements

<!--when changes here, also update the article for "Connect records"-->

{{step1-to-maestro}}

L’espace de travail du dernier accès doit s’ouvrir par défaut.

1. (Facultatif) Développez la flèche pointant vers le bas située à droite du nom d’un espace de travail existant, puis sélectionnez l’espace de travail duquel vous souhaitez connecter les types d’enregistrement.
1. Cliquez sur la carte d’un type d’enregistrement pour ouvrir la page de type d’enregistrement.
1. Cliquez sur le bouton **+** dans le coin supérieur droit du tableau, puis cliquez sur l’icône **Nouvelle connexion** .

   ![](assets/new-connection-tab-with-workfront-aem-options.png)

1. Dans le **Type d’enregistrement** , recherchez un type d’enregistrement ou sélectionnez l’une des options suivantes :

   * Un autre type d’enregistrement dans la section de l’espace de travail que vous avez sélectionné

     >[!TIP]
     >
     >Seuls les types d’enregistrement de l’espace de travail sélectionné sont disponibles pour la connexion.
     > 
     >Si vous ne disposez pas d’autres types d’enregistrement dans l’espace de travail sélectionné, la section espace de travail ne s’affiche pas.

   * A **Projet, Portfolio, Programme, Société**, ou **Groupe** de la **Types d’objet Workfront** .
   * **Experience Manager Assets** de la **Adobe d’applications** .

   ![](assets/new-connection-tab-fields-with-another-record-selected.png)


1. Mettez à jour les informations suivantes :

   * **Nom**: nom du champ connecté, tel qu’il apparaîtra dans la vue de tableau ou dans la page d’enregistrement du type d’enregistrement d’origine. Cela crée la colonne des enregistrements liés dans la vue table du type d&#39;enregistrement d&#39;origine ou du champ d&#39;enregistrement lié pour les enregistrements d&#39;origine.

   >[!TIP]
   >
   >Nous vous recommandons d’inclure le nom de l’enregistrement auquel vous êtes lié dans le nom du champ d’enregistrement connecté afin de capturer le type d’enregistrement du nouveau champ. Le nom de l&#39;enregistrement lié n&#39;est pas visible dans le nouveau champ d&#39;enregistrement lié ou ses champs liés.

   * **Description**: informations supplémentaires sur le champ d’enregistrement connecté. La description d’un champ s’affiche lorsque vous placez le pointeur de la souris sur la colonne du champ dans un tableau.
   * **Autoriser plusieurs enregistrements**: sélectionnez cette option pour indiquer que vous autorisez les utilisateurs à ajouter plusieurs enregistrements lorsque le champ de type d’enregistrement associé s’affiche sur les enregistrements originaux. Cette option est sélectionnée par défaut.
   * **Sélectionner les champs de recherche**: sélectionnez cette option pour ajouter des champs à partir du type d’enregistrement sélectionné. Les champs de recherche sont des champs associés à l’enregistrement ou au type d’objet auquel vous créez un lien. Leur liaison affiche des informations sur l’enregistrement ou l’objet auquel vous créez un lien dans l’enregistrement que vous souhaitez. Cette option est sélectionnée par défaut.

1. (Conditionnel et facultatif) Si vous avez choisi de connecter un objet Workfront, sélectionnez une **Formulaire personnalisé** de la **Lier uniquement les objets correspondant à ces critères** . Seuls les objets auxquels sont attachés les formulaires personnalisés sélectionnés peuvent être associés au type d’enregistrement sélectionné. Vous pouvez sélectionner plusieurs formulaires.

   ![](assets/workfront-project-connection-selection.png)

   >[!NOTE]
   >
   > Vous devez créer des formulaires personnalisés dans Workfront pour les objets sélectionnés avant qu’ils ne s’affichent dans cette liste.

1. (Conditionnel) Si vous avez choisi de vous connecter à Experience Manager Assets, sélectionnez un référentiel dans le **Référentiel Experience Manager** dans le menu déroulant **Lier des ressources du référentiel suivant** . Il s’agit d’un champ obligatoire. Seuls les référentiels auxquels vous avez accès dans Experience Manager Assets s’affichent dans ce champ.

   <!--replace the screen shot below when they fix the permissions info icon bug-->

   ![](assets/aem-assets-connection-selection.png)

1. Cliquez sur **Créer**.

1. (Conditionnel) Si vous avez sélectionné l’option **Sélectionner un champ de recherche** , le paramètre **Ajouter des champs de recherche** s’ouvre.

   Cliquez sur le bouton **+** pour ajouter des champs à partir de la fonction **Champs non sélectionnés** zone.

   Ou

   Cliquez sur le bouton **-** pour supprimer des champs de la fonction **Champs sélectionnés** area

   ![](assets/add-lookup-fields-for-another-maestro-record-type-box.png)

   Les valeurs des champs connectés sont renseignées automatiquement une fois que vous avez lié des enregistrements ou des objets.

   >[!IMPORTANT]
   >
   >    Toute personne disposant d’autorisations de vue ou supérieures sur l’espace de travail peut afficher les informations dans les champs liés, indépendamment de ses autorisations ou de son niveau d’accès dans l’application des types d’objets liés.


1. (Facultatif) Cliquez sur **Ignorer** et n’ajoutez aucun champ de l’enregistrement ou de l’objet lié. La variable **Nom** de l’enregistrement lié est le seul champ visible dans la vue de table de l’enregistrement d’origine.

1. (Facultatif et conditionnel) Si vous choisissez de lier un champ de type nombre, devise, pourcentage ou date, sélectionnez également une valeur d’agrégateur. Les valeurs des champs liés s&#39;affichent soit séparés par des virgules, soit sous la forme d&#39;une valeur agrégée selon l&#39;agrégateur que vous choisissez, lorsque les utilisateurs sélectionnent plusieurs enregistrements liés dans le champ d&#39;enregistrement lié.

   ![](assets/aggregator-drop-down-for-number-linked-field.png)

   >[!NOTE]
   >
   > Les agrégateurs ne sont pas disponibles lors de la connexion des types d’enregistrement à Experience Manager Assets.

   Sélectionnez l’une des options suivantes :

   * **Aucun**: affiche les valeurs provenant de plusieurs enregistrements séparés par des virgules. Il s’agit de la sélection par défaut.
   * **MAX**: affiche la valeur la plus élevée parmi toutes les valeurs issues de plusieurs enregistrements sélectionnés dans le champ d’enregistrement lié.
   * **MIN**: affiche la valeur la plus basse de toutes les valeurs provenant de plusieurs enregistrements sélectionnés dans le champ d’enregistrement lié.
   * **SUM**: affiche le total de toutes les valeurs provenant de plusieurs enregistrements sélectionnés dans le champ d’enregistrement lié.
   * **AVG**: affiche la moyenne de toutes les valeurs provenant de plusieurs enregistrements sélectionnés dans le champ d’enregistrement lié.
   * **UNIQUE**: supprime les doublons des valeurs de champ de recherche et affiche uniquement les valeurs uniques. Cette option n’est pas disponible pour les types de champ suivants :
      * Paragraphe
      * Case à cocher
      * Personnes

   >[!NOTE]
   >
   >Vous pouvez, par exemple, lier l’enregistrement de produit (enregistrement lié) de l’enregistrement Campaign (enregistrement d’origine) et le nommer &quot;champ de produit&quot;. Vous pouvez également choisir de lier le champ Budget de l’enregistrement de produit à partir de l’enregistrement de campagne et de l’appeler &quot;Budget produit&quot;. Si vous avez le droit de sélectionner plusieurs enregistrements dans le &quot;champ Produit&quot;, vous pouvez sélectionner le Produit 1 dont le budget est de 100 000 € et le Produit 2 dont le budget est de 110 000 €, et le Produit 3 dont le budget est de 100 000 €. Vous pouvez afficher les informations budgétaires suivantes dans le champ lié à partir de l’enregistrement d’origine, en fonction de l’agrégateur choisi :
   >
   >* **Aucun**: 100 000 $, 110 000 $, 100 000 $
   >* **MAX**: 110 000 $
   >* **MIN**: 100 000 $
   >* **SUM**: 310 000 $
   >* **AVG**: 103 000,33 $
   >* **UNIQUE**: 100 000 $
   >

1. (Facultatif) Utilisez la variable **search** icon ![](assets/search-icon.png) pour rechercher un champ.

1. Cliquez sur **Ajouter des champs** pour enregistrer vos modifications.

   Les éléments suivants sont ajoutés :

   * Champ d’enregistrement lié sur le type d’enregistrement à partir duquel vous créez une liaison. Le champ enregistrement lié affiche les enregistrements individuels du type d’enregistrement lié, une fois que vous les avez ajoutés manuellement. Pour plus d’informations sur l’ajout d’enregistrements, voir [Connexion d’enregistrements](/help/quicksilver/maestro/records/connect-records.md). Le nom du champ d’enregistrement lié est le nom que vous avez sélectionné à l’étape 6. <!--accurate-->

   * Champ(s) lié(s) qui affiche les informations des champs de l’enregistrement ou des types d’objets liés après l’ajout manuel des enregistrements ou des objets dans le champ d’enregistrement lié. Les champs liés ne sont créés que lorsque la variable **Sélectionner les champs de recherche** est sélectionné lors de la création de la connexion. Les champs liés sont automatiquement nommés selon ce modèle :

     `<Name of the original field on the linked record> (from <Name of your linked field>)`

     Par exemple, si vous avez lié un type d’enregistrement Campaign avec un type d’enregistrement Program et que vous nommez le champ d’enregistrement associé au Programme &quot;Informations sur le programme&quot;, puis que vous choisissez d’afficher également le champ Budget du programme dans la vue de table de la campagne, le champ lié est automatiquement nommé `Budget (from Program information)` dans la vue tableau de la campagne.

   * Lorsque vous liez des types d’enregistrement les uns aux autres, un champ d’enregistrement lié est également ajouté au type d’enregistrement auquel vous êtes associé. Le nom du champ d’enregistrement lié sur le type d’enregistrement lié est le nom du type d’enregistrement à partir duquel vous créez un lien.

     Par exemple, si vous associez le type d’enregistrement &quot;Produit&quot; du type d’enregistrement &quot;Campagne&quot; et que vous nommez le champ connecté de la campagne &quot;Produit lié&quot;, un champ d’enregistrement lié &quot;Campagne&quot; est créé pour le type d’enregistrement Produit .

     >[!TIP]
     >
     > Un champ d’enregistrement lié n’est pas créé pour les objets d’une autre application vers le type d’enregistrement que vous associez dans Workfront Planning.

1. (Facultatif et conditionnel) Depuis la vue du tableau du type d’enregistrement d’origine ou de l’enregistrement lié, cliquez sur la flèche pointant vers le bas dans l’en-tête des champs d’enregistrement liés, puis cliquez sur l’une des options suivantes :

   * **Champ Modifier**: vous pouvez uniquement mettre à jour la variable **Nom** et la variable **Description** informations du champ.
   * **Modifier les champs de recherche**: ajoutez ou supprimez l’un des champs de l’enregistrement lié.

   ![](assets/edit-field-and-lookup-fields-drop-down-menu-in-table-column.png)

   Pour ajouter ou supprimer des champs de recherche, suivez les instructions des étapes 10 à 14 ci-dessus. <!--ensure these step numbers stay accurate-->

   >[!NOTE]
   >
   > Vous ne pouvez pas ajouter de champs de recherche appartenant à des types d’enregistrement que vous liez à des types d’objets provenant d’une autre application.
   >
   > Par exemple, vous ne pouvez pas ajouter le champ de recherche &quot;État de la campagne&quot; à un projet Workfront auquel vous créez un lien à partir des campagnes.

1. (Facultatif) Cliquez sur la flèche pointant vers le bas dans l’en-tête d’un champ d’enregistrement lié ou dans l’en-tête d’un champ de recherche à partir du type d’enregistrement à partir duquel vous liez, puis cliquez sur . **Supprimer**.

   Le champ d’enregistrement ou le champ de recherche sont supprimés. Si vous supprimez un champ d’enregistrement, les champs de recherche associés à l’enregistrement lié sont également supprimés.
