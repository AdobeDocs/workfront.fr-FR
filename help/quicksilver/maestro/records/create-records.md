---
title: Créer des enregistrements
description: Lors de l’utilisation des fonctionnalités de planification d’Adobe Workfront, un enregistrement est une instance d’un type d’enregistrement. Vous devez créer des types d’enregistrement avant de pouvoir créer des enregistrements individuels. La création d'enregistrements de taxonomie est identique à la création d'enregistrements opérationnels.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: c7de4b1f-674b-424b-af64-a6df62fb738f
source-git-commit: b795ceccb3f72eb64269062823199be9c8511860
workflow-type: tm+mt
source-wordcount: '809'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Créer des enregistrements

{{maestro-important-intro}}

Dans les fonctionnalités de planification d’Adobe Workfront, un enregistrement est une instance d’un type d’enregistrement.

Vous pouvez avoir les types d’enregistrements suivants :

* **Enregistrements opérationnels**: ils représentent des objets liés au travail. Par exemple, pour un enregistrement opérationnel appelé &quot;Campagne&quot;, vous pouvez avoir nommé des enregistrements tels que &quot;Newsletter mensuelle&quot; ou &quot;Solde d’été&quot;.
* **Enregistrements de taxonomie**: ils représentent des attributs qui peuvent être associés à des enregistrements opérationnels. Par exemple, pour un type d’enregistrement de taxonomie appelé &quot;Canal&quot;, vous pouvez avoir nommé des taxonomies telles que &quot;Email&quot;, &quot;Social Media&quot; ou &quot;Publicité&quot;.

La création d&#39;enregistrements opérationnels est identique à la création d&#39;enregistrements de taxonomie.

Vous pouvez créer des enregistrements en effectuant l’une des opérations suivantes :

* Création manuelle de ces types d’enregistrement
  <!-- not possible anymore: * Connect them to records from other applications-->
* Créez des enregistrements en copiant et en collant des informations à partir d’une liste externe.

Cet article décrit comment créer des enregistrements. Pour plus d’informations sur la gestion des enregistrements dans les vues de tableau ou de chronologie, consultez les articles suivants :

* [Gestion de la vue de tableau](/help/quicksilver/maestro/views/manage-the-table-view.md)
* [Gestion du mode Chronologie](/help/quicksilver/maestro/views/manage-the-timeline-view.md)

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

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
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Accord Adobe Workfront</p></td>
   <td>
<p>Votre entreprise doit être inscrite au programme bêta fermé des fonctionnalités de planification d’Adobe Workfront. Contactez le représentant de votre compte pour en savoir plus sur cette nouvelle offre. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Formule Adobe Workfront</p></td>
   <td>
<p>Quelconque</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licence Adobe Workfront</p></td>
   <td>
   <p>Quelconque</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Paramétrages du niveau d'accès</p></td>
   <td> <p>Il n’existe aucun contrôle d’accès pour les fonctionnalités de planification Adobe Workfront </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Autorisations</p></td>
   <td> <p>Attribution ou autorisations supérieures à un espace de travail</a> </p>  
   <p>Les administrateurs système disposent d’autorisations pour tous les espaces de travail, y compris ceux qu’ils n’ont pas créés.</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Modèle de mise en page</p></td>
   <td> <p>L’administrateur de Workfront ou de groupe doit ajouter la zone Maestro à votre modèle de mise en page. Pour plus d’informations, voir <a href="../access/access-overview.md">Présentation de l’accès</a>. </p>  
</td>
  </tr>

</tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Créer des enregistrements en les ajoutant manuellement à un type d’enregistrement <!--in a record type table (I don't think you can create them elsewhere right now)-->

Vous pouvez créer des enregistrements dans la vue table d’une page de type enregistrement.

Pour plus d’informations sur la modification des informations d’enregistrement, voir [Modifier des enregistrements](/help/quicksilver/maestro/records/edit-records.md).

{#step1-to-maestro}

L’espace de travail que vous avez consulté pour la dernière fois s’ouvre par défaut. Pour plus d’informations sur la création d’espaces de travail, voir [Créer des espaces de travail](../architecture/create-workspaces.md).
1. Cliquez sur une carte de type enregistrement. Pour plus d’informations sur la création d’un type d’enregistrement, voir [Création de types d’enregistrement](../architecture/create-record-types.md).

   La page de type enregistrement s’ouvre dans la vue à laquelle vous avez accédé la dernière fois. Par défaut, une page de type enregistrement s’ouvre dans la vue de tableau.
Tous les enregistrements du type sélectionné s&#39;affichent en mode Tableau.

1. (Conditionnel) Si la page de type enregistrement ne s’ouvre pas dans la vue de tableau, cliquez sur le bouton **Affichage** , puis sélectionnez une **Vue Tableau** ![](assets/table-view-icon.png) ou cliquez sur **Créer une vue > Tableau** pour créer une vue de tableau.

<!--Replace the above with this when we release the tabbed views: 
1. (Conditional) If the record type page does not open in the table view, click the tab of a table view, or click **+ View** to create a table view. -->

1. Pour ajouter de nouveaux enregistrements, cliquez sur **Nouvel enregistrement** dans la dernière ligne du tableau ;

   Ou

   Cliquez sur **Maj + Entrée** sur votre clavier à partir de n’importe quelle colonne ou ligne du tableau. Ceci ajoute une ligne vide.

   ![](assets/adding-a-new-campaign-in-table-row.png)

1. Commencez à saisir des informations sur le nouvel enregistrement dans la nouvelle ligne.

   >[!NOTE]
   >
   >  * Il n’existe aucun champ obligatoire pour les enregistrements. Nous vous recommandons toutefois d’ajouter un Nom pour l’enregistrement, car il est utile d’identifier les enregistrements lors de la liaison d’enregistrements.
   >
   >  * Les champs qui font référence à d’autres types d’enregistrement ou à des champs calculés sont en lecture seule.

1. Continuez à ajouter des informations sur chaque ligne, puis cliquez sur **Entrée** sur votre clavier pour enregistrer vos modifications.

<!--Or 
    
    Click the new record's name or the **Open details** icon ![](assets/open-details-icon-in-table-name-field.png) to the left of the record name. The **Details** box opens in the table. 

      >[!TIP]
      >
      >    You can access the Details box only from the name field of the record when the Name field is a primary field. 

  1. Start editing the record's information in the Details box. Workfront automatically saves your changes. 
  1. (Optional) Click the **Open in new tab** icon ![](assets/open-details-in-a-new-tab-icon.png) in the upper-right corner of the Details box to open the record's **Details** page in a new tab. Continue editing the record on the Details page.
    -->

1. (Facultatif) Utilisez les raccourcis clavier suivants pour annuler ou rétablir l’ajout de nouveaux enregistrements :

   * Ctrl + Z (⌘ + Z pour Mac) pour annuler une modification.
   * Ctrl + Maj + Z (⌘ + Maj + Z pour Mac) pour rétablir la modification

<!-- this is not possible anymore: 

## Create records by connecting them from another application

You can import records from other applications by linking them to existing records. This creates a linked record for the other application's connected object. 

1. Create a record type, as described in the [Create record types](../architecture/create-record-types.md).

1. Create records for the record type you created in the previous step. For information, see the section [Create records by manually adding them to a record type](#create-records-by-manually-adding-them-to-a-record-type) in this article. 

1. Create a connection to an object type from another application for the record type you created. For information, see [Connect record types](../architecture/connect-record-types.md).

1. Add objects from another application to the records you created above using the linked record field you created in the previous step. For information, see [Connect records](../records/connect-records.md). 

    The following items are created in Maestro:

    * A read-only Maestro record type that refers to the other application's record type you linked to in the connected record field. 

      For example, if you connect a Maestro record type to Workfront project, a read-only record type named "Workfront project" is created in the same workspace. You can access the read-only Workfront record types from the table view of the Maestro records you're linking from. 
   
-->

## Créer des enregistrements en copiant et collant des informations à partir d’une liste externe

1. Commencez à créer des enregistrements dans la vue Tableau, comme décrit dans la section [Créer des enregistrements en les ajoutant manuellement à un type d’enregistrement](#create-records-by-manually-adding-them-to-a-record-type) dans cet article.

   Assurez-vous que la vue de tableau contient les colonnes (ou les champs) que vous souhaitez renseigner avec les nouvelles informations d’enregistrement.

1. Cliquez sur **Nouveau &lt; Nom du type d’enregistrement >** dans la dernière ligne du tableau pour ajouter autant de nouvelles lignes que vous souhaitez que vos nouveaux enregistrements soient.

   Par exemple, ajoutez 10 lignes à la vue de tableau si vous souhaitez coller les informations relatives à 10 nouveaux enregistrements d’une autre application.

1. Dans une autre application, créez une liste d&#39;enregistrements à importer.

   Vous pouvez par exemple utiliser une feuille de calcul Excel pour créer votre liste.

   La liste doit contenir des informations sous forme de tableau.

   >[!TIP]
   >
   > Les colonnes de la liste doivent contenir des informations sur les champs existants que vous avez dans Workfront.
   >
   > Assurez-vous que les champs de votre choix ont déjà été créés dans Workfront et que les informations de votre feuille s’affichent au format correct qui correspond à celui de chaque champ de Workfront.

1. Dans une autre application, sélectionnez plusieurs lignes et colonnes, puis collez les informations dans la vue table de type enregistrement, en commençant par le premier nouvel enregistrement.

   Les informations suivantes sont importées dans la zone des fonctionnalités de planification de Workfront :

   * Les lignes contiennent les nouveaux enregistrements
   * Les colonnes renseignent les informations des champs des enregistrements.
