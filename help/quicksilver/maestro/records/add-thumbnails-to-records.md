---
title: Ajout d’une miniature à un enregistrement
description: Vous pouvez modifier les informations d’enregistrement dans Adobe Workfront Planning et associer chaque enregistrement à des miniatures individuelles afin de les rendre facilement reconnaissables.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: b22c4955-c3f2-4841-a278-bb40e8890ed9
source-git-commit: 1369269bcb64bd32f26603608782dc996b079cb9
workflow-type: tm+mt
source-wordcount: '536'
ht-degree: 5%

---

<!--update the metadata with real information-->

# Ajout d’une miniature à un enregistrement

{{planning-important-intro}}

Vous pouvez associer des enregistrements à des miniatures uniques dans Adobe Workfront Planning afin de les rendre facilement reconnaissables.

Vous devez créer des types d’enregistrement avant de pouvoir commencer à créer et modifier des enregistrements.
Pour plus d’informations, voir [Création de types d’enregistrement](../architecture/create-record-types.md).

## Conditions d’accès

<!--************double-check permissions here - asking Isk and Lilit what permissions users need for adding thumbnails-->

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
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Accord Adobe Workfront</p></td>
   <td>
<p>Votre entreprise doit être inscrite à l’étape d’accès anticipé pour la planification Workfront </p>
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
   <td> <p>Il n’existe aucun contrôle d’accès pour Workfront Planning </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Autorisations</p></td>
   <td> <p>Attribution ou autorisations supérieures à un espace de travail </p>  
   <p>Les administrateurs système disposent d’autorisations pour tous les espaces de travail, y compris ceux qu’ils n’ont pas créés.</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Modèle de mise en page</p></td>
   <td>  <p>Tous les utilisateurs, y compris les administrateurs de Workfront, doivent se voir attribuer un modèle de mise en page incluant la zone Planning dans le menu principal. </p> <p>Pour plus d’informations, voir <a href="/help/quicksilver/maestro/access/access-overview.md">Présentation de l’accès</a>. </p>  
</td>
  </tr>

</tbody>
</table>

## Points à prendre en compte concernant les miniatures d’enregistrements

Pour faire la distinction visuelle entre les enregistrements dans une vue de tableau, vous pouvez associer une miniature unique à chaque enregistrement.

Tenez compte des points suivants :

* Vous pouvez uniquement ajouter des fichiers image sous forme de miniatures.
  <!--above: when you know exactly what type of files are allowed, add the exact extensions above-->
* Vous pouvez ajouter une miniature à des enregistrements individuels dans la vue de tableau.
* Les miniatures appartiennent aux informations d’enregistrement et s’affichent dans les vues où s’affichent les enregistrements. Par exemple, les miniatures s’affichent avec les informations d’enregistrement dans les zones suivantes :

   * Le champ principal d’un enregistrement dans la vue de tableau
   * La barre d’enregistrement en mode Chronologie.
* Vous ne pouvez pas ajouter de miniatures d’enregistrement à partir de la page de l’enregistrement ou d’un autre type de vue.
* Les miniatures ne s’affichent pas sur la page de l’enregistrement.

## Ajout d’une miniature à un enregistrement

{{step1-to-maestro}}

1. Sélectionnez l’espace de travail pour lequel vous souhaitez ajouter des miniatures, puis cliquez sur la carte de type d’enregistrement.

   Cela ouvre la page de type enregistrement.
1. Sélectionnez une vue de tableau dans la **Affichage** menu déroulant. Tous les enregistrements du type que vous avez sélectionné s&#39;affichent dans un tableau.
1. Passez la souris sur les informations du champ principal, puis cliquez sur le **Plus** menu ![](assets/more-menu.png), puis cliquez sur **Miniature**.

   ![](assets/record-more-menu-expanded.png)

   >[!TIP]
   >
   >   Le champ principal est le champ qui s’affiche dans la première colonne d’une vue de tableau. Le champ principal est toujours gelé et ne peut pas être masqué ni déplacé.

   La variable **Miniature d’enregistrement** s’ouvre.

   ![](assets/record-thumbnail-box-for-upload.png)

   <!--update screen shot with correct casing-->

1. Dans le **Télécharger** , faites glisser et déposez un fichier à ajouter en tant que miniature ou cliquez sur **Sélectionner pour charger**, puis recherchez un fichier image à ajouter. Le fichier doit être enregistré sur votre ordinateur.
1. (Facultatif) Utilisez l’outil de dimensionnement pour recadrer et redimensionner l’image.
1. Cliquez sur **Utiliser une image** pour ajouter l’image en tant que miniature.
Cela ferme la fenêtre **Miniature d’enregistrement** de la boîte.
1. (Conditionnel) Si vous disposez au moins des autorisations de contribution à la vue de tableau, cliquez sur **Champs** dans le coin supérieur droit de la vue du tableau.
1. Sélectionnez la variable **Miniature** pour afficher la miniature. Cette option est désélectionnée par défaut.

   ![](assets/thumbnail-toggle-in-fields-menu-deselected.png)

   La miniature s’affiche à gauche de la valeur du champ principal.
1. (Facultatif et conditionnel) Si vous ne disposez pas des autorisations de contributeur ou d’une autorisation ultérieure pour l’affichage, sélectionnez une nouvelle vue dans la **Affichage** ou créer une vue.
1. (Facultatif) Pour supprimer la miniature, passez la souris sur le champ principal et cliquez sur le bouton **Plus** menu ![](assets/more-menu.png)> **Miniature** > le **Supprimer** icon ![](assets/remove-image-icon.png), puis cliquez sur **Enregistrer les modifications**.

<!--
Replace the section above with the following when we release generate thumbnails:

## Add a thumbnail to a record

You can add a thumbnail to a record in the following ways:

* Upload a file from your computer
* Generate an image with a prompt

### Upload a thumbnail to a record

{{step1-to-maestro}}

1. Select the workspace for whose records you want to add thumbnails, then click the record type card. 

   This opens the record type page. 
1. Select a table view from the **View** drop-down menu. All records of the type you selected display in a table. 
1. Hover over the primary field information, click the **More** menu ![](assets/more-menu.png), then click **Thumbnail**. 

   ![](assets/record-more-menu-expanded.png)

      >[!TIP]
      >
      >   The primary field is the field that displays in the first column of a table view. The primary field is always frozen and cannot be hidden or relocated. 

   The **Record thumbnail** box opens.

   ![](assets/record-thumbnail-box-for-upload.png) 

1. Click the **Upload** tab, and drag and drop a file to add as a thumbnail
   Or
   Click **Select to upload**, then browse for an image file to add. The file must be saved on your computer. 
1. (Optional) Use the sizing tool to crop and resize the image.
1. Click **Use image** to add the image as a thumbnail. 
   This closes the **Record thumbnail** box.
1. (Conditional) If you have at least Contribute permissions to the table view, click **Fields** in the upper-right corner of the table view. 
1. Select the **Thumbnail** toggle to display the thumbnail. This is deselected by default. 

   ![](assets/thumbnail-toggle-in-fields-menu-deselected.png)

   The thumbnail displays to the left of the primary field value. 
1. (Optional and conditional) If you do not have Contribute or higher permissions to the view, select a new view from the **View** drop-down menu, or create a view. 
1. (Optional) To remove the thumbnail, hover over the primary field and click the **More** menu ![](assets/more-menu.png)> **Thumbnail** > the **Remove** icon ![](assets/remove-image-icon.png), then click **Save changes**.

### Generate a thumbnail for a record

{{step1-to-maestro}}

1. Select the workspace for whose records you want to add thumbnails, then click the record type card. 

   This opens the record type page. 
1. Select a table view from the **View** drop-down menu. All records of the type you selected display in a table. 
1. Hover over the primary field information, click the **More** menu ![](assets/more-menu.png), then click **Thumbnail**. 

   ![](assets/record-more-menu-expanded.png)

      >[!TIP]
      >
      >   The primary field is the field that displays in the first column of a table view. The primary field is always frozen and cannot be hidden or relocated. 

   The **Record thumbnail** box opens.

(*************** update the screenshot below*************)
   ![](assets/record-thumbnail-box-for-upload.png) 

1. Click the **Generate** tab, and type a prompt describing the type of image you want to add in the space provided. 
1. Click **Generate**. 

   A set of four suggested images displays. 

1. Click an image to select it, then click **Use image**. 

   The Record thumbnail box closes and the thumbnail is attached to the record. All users who can view the records can now see the selected thumbnail. 
1. (Optional) Click the **More** menu ![](assets/more-menu.png) to the right of the record name in the table view, then click **Thumbnail**. 

   The generated image opens in the **Upload** tab where you can modify or remove it, as described in the section [Upload a thumbnail to a record](#upload-a-thumbnail-to-a-record) in this article. 
-->