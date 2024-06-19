---
title: Ajout d’une miniature à un enregistrement
description: Vous pouvez modifier les informations d’enregistrement dans Adobe Workfront Planning et associer chaque enregistrement à des miniatures individuelles afin de les rendre facilement reconnaissables.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: b22c4955-c3f2-4841-a278-bb40e8890ed9
source-git-commit: 8bfada77ac7b1b2a8d8fb2feec8a8167a1397cdc
workflow-type: tm+mt
source-wordcount: '779'
ht-degree: 3%

---

<!--update the metadata with real information-->

# Ajout d’une miniature à un enregistrement

{{planning-important-intro}}

Vous pouvez associer des enregistrements à des miniatures uniques dans Adobe Workfront Planning afin de les rendre facilement reconnaissables.

Vous devez créer des types d’enregistrement avant de pouvoir commencer à créer et modifier des enregistrements.
Pour plus d’informations, voir [Création de types d’enregistrement](/help/quicksilver/planning/architecture/create-record-types.md).

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
   <td role="rowheader"><p>Licence Adobe Workfront*</p></td>
   <td>
   <p>Actuel : travail ou plus élevé</p>
   <p>Nouveau : Standard</p>  
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configurations du niveau d’accès</p></td>
   <td> <p>Il n’existe aucun contrôle d’accès pour Workfront Planning </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Autorisations</p></td>
   <td> <p>Gestion des autorisations d’un espace de travail </p>  
   <p>Les administrateurs système disposent d’autorisations pour tous les espaces de travail, y compris ceux qu’ils n’ont pas créés.</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Modèle de mise en page</p></td>
   <td>  <p>Tous les utilisateurs, y compris les administrateurs de Workfront, doivent se voir attribuer un modèle de mise en page incluant la zone Planning dans le menu principal. </p> <p>Pour plus d’informations, voir <a href="/help/quicksilver/planning/access/access-overview.md">Présentation de l’accès</a>. </p>  
</td>
  </tr>

</tbody>
</table>

*Pour plus d’informations, voir [Conditions d’accès requises dans la documentation de Workbench](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Points à prendre en compte concernant les miniatures d’enregistrements

Pour faire la distinction visuelle entre les enregistrements dans une vue de tableau, vous pouvez associer une miniature unique à chaque enregistrement.

Tenez compte des points suivants :

* Une miniature est propre à un enregistrement et ne s’applique pas à tous les enregistrements du même type.
* Vous pouvez uniquement ajouter des fichiers image sous forme de miniatures.
  <!--above: when you know exactly what type of files are allowed, add the exact extensions above-->
* Vous pouvez ajouter une miniature à des enregistrements individuels dans la vue de tableau ou à partir de la page ou de la zone d’aperçu de l’enregistrement.
* Workfront télécharge automatiquement une miniature chaque fois que vous créez un enregistrement. Vous pouvez modifier cette image ultérieurement.
* Les miniatures appartiennent aux informations d’enregistrement et s’affichent dans les zones où s’affichent les enregistrements. Par exemple, les miniatures s’affichent avec les informations d’enregistrement dans les zones suivantes :

   * Le champ principal d’un enregistrement dans la vue de tableau
   * La barre d’enregistrement en mode Chronologie.
   * Aperçu et page des détails de l’enregistrement.

## Ajout d’une miniature à un enregistrement

Vous pouvez ajouter une miniature de la manière suivante :

* [Ajout d’une miniature à un enregistrement à partir de la vue de tableau](#add-a-thumbnail-to-a-record-from-the-table-view)
* [Ajout d’une miniature à un enregistrement à partir de la page de détails](#add-a-thumbnail-to-a-record-from-the-details-page)

### Ajout d’une miniature à un enregistrement à partir de la vue de tableau

{{step1-to-planning}}

1. Cliquez sur l’espace de travail pour lequel vous souhaitez ajouter des miniatures, puis cliquez sur la carte de type d’enregistrement.

   Cela ouvre la page de type enregistrement.
1. Sélectionnez une vue de tableau dans la **Affichage** menu déroulant. Tous les enregistrements du type que vous avez sélectionné s&#39;affichent dans un tableau.
1. Passez la souris sur les informations du champ principal, puis cliquez sur le **Plus** menu ![](assets/more-menu.png), puis cliquez sur **Miniature**.

   ![](assets/record-more-menu-expanded.png)

   >[!TIP]
   >
   >   Le champ principal est le champ qui s’affiche dans la première colonne d’une vue de tableau. Le champ principal est toujours gelé et ne peut pas être masqué ni déplacé. L’option Miniature n’est pas disponible dans le menu Plus lorsque le champ principal est un champ de formule.

   La variable **Télécharger** s’ouvre par défaut dans la fonction **Miniature d’enregistrement** de la boîte.

   Pour plus d’informations sur le téléchargement de la miniature, voir la section [Ajout d’une miniature à un enregistrement à partir de la page de détails](#add-a-thumbnail-to-a-record-from-the-details-page) dans cet article, en commençant par l’étape 6. <!--see if this is accurate-->

<!--
   ![](assets/record-thumbnail-box-for-upload.png) 

  *****update screen shot with correct casing****

1. Drag and drop a file to add as a thumbnail
   
   Or
   
   Click **Browse images**, then browse for an image file to add. The file must be saved on your computer. 
1. (Optional) After the image uploads in the **Record thumbnail** box, use the sizing tool to crop and resize the image.
1. (Optional) Click the **Upload new image** icon ![](assets/upload-new-image-icon.png) to upload another image. 
1. (Optional) To remove a thumbnail before it is saved, click  **Remove uploaded image** icon ![](assets/remove-image-icon.png) to the right of the image. 
1. (Optional) Click the **Gallery** tab, then click an image. The gallery of images cannot be modified.

   ![](assets/record-thumbnail-box-for-gallery.png)
1. Click **Use image** to add the image as a thumbnail. 
   This closes the **Record thumbnail** box.
   The thumbnail displays in areas of Workfront Planning where the record displays. 

   >[!TIP]
   >
   >   You must enable the Thumbnail field in the table view to display thumbnails in this view. It is disabled by default.

1. (Optional) To remove the thumbnail after it is saved, hover over the primary field and click the **More** menu ![](assets/more-menu.png)> **Thumbnail** > the **Remove** icon ![](assets/remove-image-icon.png), then click **Save changes**. -->

### Ajout d’une miniature à un enregistrement à partir de la page de détails

{{step1-to-planning}}

1. Cliquez sur l’espace de travail pour lequel vous souhaitez ajouter des miniatures, puis cliquez sur la carte de type d’enregistrement.

   Cela ouvre la page de type enregistrement.
1. Dans n’importe quelle vue, cliquez sur un enregistrement pour l’ouvrir.

   La zone d’aperçu des détails s’affiche.
1. (Facultatif) Cliquez sur le **Ouvrir dans un nouvel onglet** icon ![](assets/open-details-in-a-new-tab-icon.png) dans le coin supérieur droit.

   La page de détails de l’enregistrement s’ouvre.
1. Pointez sur l’image ou l’icône de la miniature. ![](assets/record-thumbnail-icon-on-details-page.png), puis cliquez sur le bouton **Plus** menu ![](assets/more-menu.png) > **Modifier la miniature**.

   La variable **Télécharger** s’ouvre par défaut dans la fonction **Miniature d’enregistrement** de la boîte.

   ![](assets/record-thumbnail-box-for-upload.png)

1. Faites glisser et déposez un fichier à ajouter en tant que miniature.

   Ou

   Cliquez sur **Parcourir les images**, puis recherchez un fichier image à ajouter. Le fichier doit être enregistré sur votre ordinateur.

1. (Facultatif) Une fois l’image chargée dans la variable **Miniature d’enregistrement** , utilisez l’outil de dimensionnement pour recadrer et redimensionner l’image.
1. (Facultatif) Cliquez sur le **Charger une nouvelle image** icon ![](assets/upload-new-image-icon.png) pour charger une autre image.
1. (Facultatif) Cliquez sur le **Galerie** , puis cliquez sur une image. La galerie d’images ne peut pas être modifiée.

   ![](assets/record-thumbnail-box-for-gallery.png)

1. (Facultatif) Pour supprimer la miniature avant son enregistrement, cliquez sur le bouton **Supprimer** icon ![](assets/remove-image-icon.png) à droite de l’image.

1. Cliquez sur **Utiliser une image** pour ajouter l’image en tant que miniature.
Cela ferme la fenêtre **Miniature d’enregistrement** de la boîte.
La miniature s’affiche dans les zones de la planification Workfront où s’affiche l’enregistrement.

   >[!TIP]
   >
   >   Vous devez activer le champ Miniature dans la vue Tableau pour afficher les miniatures dans cette vue. Elle est désactivée par défaut.

1. (Facultatif) Pour supprimer la miniature après son enregistrement, cliquez sur un enregistrement dans n’importe quelle vue pour ouvrir la page de détails, puis survolez l’image miniature avec la souris et cliquez sur l’icône **Plus** menu ![](assets/more-menu.png)> **Supprimer** icon ![](assets/remove-image-icon.png). L’image miniature est supprimée.




<!--
### Generate a thumbnail for a record

{{step1-to-planning}}

1. Click the workspace for whose records you want to add thumbnails, then click the record type card. 

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