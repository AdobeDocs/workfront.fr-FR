---
title: Créer des enregistrements
description: Lors de l’utilisation d’Adobe Workfront Planning, un enregistrement est une instance d’un type d’enregistrement. Vous pouvez créer des enregistrements uniques pour chaque type d’enregistrement dans le calendrier Workfront en les ajoutant manuellement à la vue de tableau, en les important à partir d’une liste, en les dupliquant ou en les créant lorsque vous les connectez à d’autres enregistrements.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: c7de4b1f-674b-424b-af64-a6df62fb738f
source-git-commit: 80d9fc7f8cf28de8dbb8f1c53835940142681906
workflow-type: tm+mt
source-wordcount: '1336'
ht-degree: 39%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Créer des enregistrements

{{planning-important-intro}}

Dans Adobe Workfront Planning, un enregistrement est une instance d’un type d’enregistrement.

Vous pouvez créer des enregistrements en effectuant l’une des opérations suivantes :

* Ajoutez-les à partir de la page de type enregistrement dans la vue de tableau.
* Copier et coller une liste d&#39;enregistrements d&#39;une liste externe
* Les dupliquer
* Créez-les au fur et à mesure que vous les connectez à partir d&#39;autres enregistrements
  <!--* Create them by submitting a request form-->

Cet article décrit comment créer des enregistrements.

Pour plus d’informations sur la gestion des enregistrements dans les vues de tableau ou de chronologie, consultez les articles suivants :

* [Gérer la vue de tableau](/help/quicksilver/planning/views/manage-the-table-view.md)
* [Gérer la vue chronologique](/help/quicksilver/planning/views/manage-the-timeline-view.md)

## Conditions d’accès

<!--Updated for GA-->

+++ Développez pour afficher les exigences d’accès à la planification Workfront.

Pour pouvoir accéder à Workfront Planning, vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Produits</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Planification d’Adobe Workfront<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Forfait Adobe Workfront*</p></td> 
   <td> 
<p>L’un des projets Workfront suivants est prévu :</p> 
<ul><li>Sélectionner</li> 
<li>Principal</li> 
<li>Final</li></ul> 
<p>La planification Workfront n’est pas disponible pour les plans Workfront hérités</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Formule de planification Adobe Workfront*</p></td> 
   <td> 
<p>N’importe quelle </p> 
<p>Pour plus d’informations sur les éléments inclus dans chaque plan de planification Workfront, voir <a href="https://business.adobe.com/products/workfront/pricing.html">Prix et package Adobe Workfront</a>. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Plateforme Adobe Workfront</p></td> 
   <td> 
<p>L’instance de Workfront de votre entreprise doit être intégrée à l’expérience unifiée Adobe pour pouvoir accéder à toutes les fonctionnalités de la planification Workfront.</p> 
<p>Pour plus d’informations, voir <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience pour Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront*</p></td> 
   <td> Standard
   <p>La planification Workfront n’est pas disponible pour les licences Workfront héritées</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuration du niveau d’accès</p></td> 
   <td> <p>Il n’existe aucun contrôle de niveau d’accès pour Adobe Workfront Planning.</p> 
   <p>Modifiez l’accès dans Workfront pour les types d’objets que vous souhaitez créer (projets et portefeuilles) lorsque vous connectez les enregistrements à ces types d’objets. </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td> <p>Gérez les autorisations de l’espace de travail auquel vous souhaitez ajouter des enregistrements. </p>  
   <p>Les équipes d’administration système ont des droits sur tous les espaces de travail, y compris ceux qu’ils n’ont pas créés.</p>
   <p>Gérez les autorisations d’accès aux objets Workfront (portfolios) pour ajouter des objets enfants (projets).</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modèle de disposition</p></td> 
   <td> <p>Tous les utilisateurs, y compris les administrateurs Workfront, doivent se voir attribuer un modèle de mise en page incluant la zone Planification dans le menu principal. </p> </td> 
  </tr> 
</tbody> 
</table>

* Pour plus d’informations sur les exigences d’accès à Workfront, consultez les [Conditions d’accès requises dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

<!--OLD info: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p>
   <p>Current: Plan</p>  
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> <p>There are no access controls for Adobe Workfront Planning </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Contribute or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>

 </tbody>
</table>

*For more information, see [Access requirements for Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). -->

+++


## Créez des enregistrements en les ajoutant à un type d&#39;enregistrement <!--in a record type table (I don't think you can create them elsewhere right now)-->

Vous pouvez créer des enregistrements dans la vue de tableau d’une page de type d’enregistrement.

Pour plus d’informations sur la modification des informations d’enregistrement, voir [Modifier des enregistrements](/help/quicksilver/planning/records/edit-records.md).

{{step1-to-planning}}

1. Cliquez sur l&#39;espace de travail dans lequel vous souhaitez ajouter des enregistrements.

   L’espace de travail s’ouvre et les types d’enregistrement s’affichent sous forme de cartes.

1. Cliquez sur une carte de type d’enregistrement. Pour plus d’informations sur la création d’un type d’enregistrement, voir [Créer des types d’enregistrement](/help/quicksilver/planning/architecture/create-record-types.md).

   La page de type d’enregistrement s’ouvre dans la dernière vue à laquelle vous avez accédé. Par défaut, une page de type d’enregistrement s’ouvre dans la vue de tableau.
Tous les enregistrements du type sélectionné s&#39;affichent dans la vue.

1. (Conditionnel) Selon la vue que vous affichez, effectuez l’une des opérations suivantes :

   * Dans la vue Tableau :

      * Cliquez sur **Nouvel enregistrement** dans la dernière ligne du tableau.

      * Cliquez sur **Maj+Entrée** sur votre clavier depuis n’importe quelle colonne ou ligne du tableau. Une ligne vide est alors ajoutée sous l’enregistrement à partir duquel vous commencez.
      * Passez la souris sur le champ principal d’un enregistrement, cliquez sur le menu **Plus** ![](assets/more-menu.png) situé à droite du champ, puis cliquez sur **Insérer un enregistrement au-dessus** ou **Insérer un enregistrement en dessous**.

     ![](assets/adding-a-new-campaign-in-table-row.png)

   * Dans n’importe quelle vue :

      * Cliquez sur **Nouvel enregistrement** dans le coin supérieur droit de la page. La boîte d’aperçu des enregistrements s’ouvre.

     Workfront télécharge automatiquement une miniature et une image de couverture vers chaque nouvel enregistrement. Vous pourrez modifier ces images ultérieurement. Pour plus d’informations, voir les articles suivants :

      * [Ajouter une image de couverture à un enregistrement](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md)
      * [Ajouter une miniature à un enregistrement](/help/quicksilver/planning/records/add-thumbnails-to-records.md)

1. Commencez à saisir des informations sur le nouvel enregistrement dans les champs que vous voyez dans la zone d’aperçu.

   >[!NOTE]
   >
   >  * Il n’existe aucun champ obligatoire pour les enregistrements. Nous vous recommandons toutefois d’ajouter des informations pour le champ principal d’un enregistrement, car il est utile d’identifier les enregistrements lors de la liaison d’enregistrements. Pour plus d’informations sur les champs principaux, voir [Gestion de la vue de table](/help/quicksilver/planning/views/manage-the-table-view.md) et [Présentation des champs de Principal](/help/quicksilver/planning/fields/primary-field-overview.md).
   >
   >  * Les champs qui font référence à d’autres types d’enregistrement ou à des champs calculés sont en lecture seule.

1. (Conditionnel) Lors de l’ajout d’enregistrements dans le tableau, continuez à ajouter des informations sur chaque ligne, puis cliquez sur **Entrée** sur votre clavier pour enregistrer vos modifications.

   Ou

   Cliquez sur le nom du nouvel enregistrement ou sur l’icône **Ouvrir les détails** ![](assets/open-details-icon-in-table-name-field.png) à gauche du nom de l’enregistrement. Un aperçu contenant les informations détaillées de l’enregistrement s’ouvre dans le tableau.

   >[!TIP]
   >
   >Vous ne pouvez accéder à l’icône **Ouvrir les détails** qu’à partir du champ nom de l’enregistrement lorsque le champ Nom est un champ principal.

1. Commencez à modifier les informations de l’enregistrement dans l’aperçu de l’enregistrement. Workfront enregistre automatiquement vos modifications.
1. (Facultatif) Cliquez sur l’icône **Ouvrir dans un nouvel onglet** ![](assets/open-details-in-a-new-tab-icon.png) dans le coin supérieur droit de l’aperçu de l’enregistrement pour ouvrir la page de l’enregistrement dans un nouvel onglet. Continuez à modifier l’enregistrement sur la page d’enregistrement. Pour plus d’informations, voir [Modifier des enregistrements](/help/quicksilver/planning/records/edit-records.md).

1. (Facultatif) Utilisez les raccourcis clavier suivants pour annuler ou rétablir l’ajout de nouveaux enregistrements ou de leurs informations lors de leur ajout dans la vue de tableau :

   * Ctrl+Z (⌘+Z pour Mac) pour annuler une modification
   * Ctrl+Maj+Z (⌘+Maj+Z pour Mac) pour rétablir une modification

<!-- this is not possible anymore: 

## Create records by connecting them from another application

You can import records from other applications by linking them to existing records. This creates a linked record for the other application's connected object. 

1. Create a record type, as described in the [Create record types](/help/quicksilver/planning/architecture/create-record-types.md).

1. Create records for the record type you created in the previous step. For information, see the section [Create records by manually adding them to a record type](#create-records-by-manually-adding-them-to-a-record-type) in this article. 

1. Create a connection to an object type from another application for the record type you created. For information, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md).

1. Add objects from another application to the records you created above using the linked record field you created in the previous step. For information, see [Connect records](/help/quicksilver/planning/records/connect-records.md). 

    The following items are created in Workfront Planning:

    * A read-only record type that refers to the other application's record type you linked to in the connected record field. 

      For example, if you connect a Planning record type to Workfront project, a read-only record type named "Workfront project" is created in the same workspace. You can access the read-only Workfront record types from the table view of the Planning records you're linking from. 
   
-->

## Créer des enregistrements en les copiant et en les collant depuis une liste externe

1. Commencez à créer des enregistrements dans la vue Tableau, comme décrit dans la section [Créer des enregistrements en les ajoutant manuellement à un type d’enregistrement](#create-records-by-manually-adding-them-to-a-record-type) dans cet article.

   Assurez-vous que la vue de tableau contient les colonnes (ou les champs) que vous souhaitez renseigner avec les nouvelles informations d’enregistrement.

1. Cliquez sur **Nouveau &lt; Nom du type d’enregistrement >** dans la dernière ligne du tableau pour ajouter autant de nouvelles lignes au tableau que vous souhaitez.

   Par exemple, ajoutez 10 lignes à la vue de tableau si vous souhaitez coller les informations relatives à 10 nouveaux enregistrements d’une autre application.

1. Dans une autre application, créez une liste d’enregistrements à importer.

   Vous pouvez par exemple utiliser une feuille de calcul Excel pour créer votre liste.

   La liste doit contenir des informations sous forme de tableau.

   >[!TIP]
   >
   > Les colonnes de la liste doivent contenir des informations sur les champs existants que vous avez dans Workfront.
   >
   > Assurez-vous que les champs de votre choix ont déjà été créés dans Workfront et que les informations de votre feuille s’affichent au format correct qui correspond à celui de chaque champ de Workfront.

1. Dans une autre application, sélectionnez plusieurs lignes et colonnes, puis collez les informations dans la vue de tableau de type enregistrement, en commençant par le premier nouvel enregistrement.

   Les informations suivantes sont importées dans la zone Workfront Planning :

   * Les lignes contiennent les nouveaux enregistrements.
   * Les colonnes renseignent les informations des champs des enregistrements.

## Créer des enregistrements en les dupliquant

Pour plus d&#39;informations sur la duplication d&#39;enregistrements, voir [Duplication d&#39;enregistrements](/help/quicksilver/planning/records/copy-or-duplicate-records.md).

## Créer des enregistrements lors de leur connexion

Vous pouvez créer des enregistrements ou des objets Workfront lorsque vous les connectez à partir d&#39;autres enregistrements.

Vous devez disposer des éléments suivants avant de pouvoir ajouter de nouveaux enregistrements ou des objets Workfront en les connectant à partir d’enregistrements existants :

* Types d’enregistrement connectés. Pour plus d’informations, voir [Connecter des types d’enregistrement](/help/quicksilver/planning/architecture/connect-record-types.md).
* Enregistrements connectés. Pour plus d’informations, voir [Connecter des enregistrements](/help/quicksilver/planning/records/connect-records.md).
* Accès et autorisations corrects dans Workfront Planning et Workfront, comme décrit dans la section [Exigences d’accès](#access-requirements) de cet article.

>[!NOTE]
>
>La création de projets et de portefeuilles Workfront lorsque vous les connectez aux enregistrements de planification Workfront est similaire à la création d’enregistrements de planification lorsque vous les connectez à partir d’autres enregistrements.

Pour créer des enregistrements lors de leur connexion à partir d&#39;autres enregistrements :

1. Commencez à connecter les enregistrements de la planification Workfront, comme décrit dans l’article [Connecter des enregistrements](/help/quicksilver/planning/records/connect-records.md).
1. (Conditionnel) Si vous ne parvenez pas à trouver un enregistrement en essayant de l’ajouter à partir du champ d’enregistrement connecté d’un autre enregistrement, recherchez un enregistrement, puis cliquez sur **+ Ajouter**. Le bouton **+ Ajouter** est suivi du nom du type d’enregistrement à partir duquel vous vous connectez.

   ![](assets/add-button-to-create-records-in-context-highlighted.png)

   L’enregistrement est créé et ajouté au champ d’enregistrement connecté.
1. (Facultatif) Accédez à la vue table du type d’enregistrement dont vous avez créé l’enregistrement. Un nouvel enregistrement s’affiche dans la dernière ligne de la vue.
1. (Facultatif) Commencez à ajouter des informations pour le nouvel enregistrement dans la vue de tableau.
Ou
Cliquez sur son nom pour ouvrir la page de détails et y ajouter des informations.

<!--
## Create records by submitting a request form

After someone creates a request form for a record type and shares a link to it with you, you can submit a request which creates a record for that record type. 

For information, see [Create and manage a request form in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

Both Workfront users and users external to your organization can submit requests to Planning record types and create records, if they have a link to the request form.

For information, see [Submit Adobe Workfront Planning requests to create records](/help/quicksilver/planning/requests/submit-requests.md). -->