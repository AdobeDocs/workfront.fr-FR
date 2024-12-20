---
title: Ajout d’une miniature à un enregistrement
description: Vous pouvez modifier les informations d’enregistrement dans Adobe Workfront Planning et associer chaque enregistrement à des miniatures individuelles afin de les rendre facilement reconnaissables.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: b22c4955-c3f2-4841-a278-bb40e8890ed9
source-git-commit: 9629558bfc2c4fa7fb040bcc45534164e0d8b3b4
workflow-type: tm+mt
source-wordcount: '946'
ht-degree: 34%

---


# Ajouter une miniature à un enregistrement

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de manière générale. Il est disponible uniquement dans l’environnement Aperçu pour tous les clients. Après les versions mensuelles de Production, les mêmes fonctionnalités sont également disponibles dans l’environnement Production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation de versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

Vous pouvez associer des enregistrements à des miniatures uniques dans Adobe Workfront Planning afin de les rendre facilement reconnaissables.

Vous devez créer des types d’enregistrement avant de pouvoir commencer à créer et modifier des enregistrements.
Pour plus d’informations, consultez [Créer des types d’enregistrements](/help/quicksilver/planning/architecture/create-record-types.md).

## Conditions d’accès

<!--************double-check permissions here - asking Isk and Lilit what permissions users need for adding thumbnails-->

+++ Développez pour afficher les exigences d’accès à la planification Workfront.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

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
   <td role="rowheader"><p>Formule Adobe Workfront*</p></td> 
   <td> 
<p>L’un des projets Workfront suivants est prévu :</p> 
<ul><li>Sélectionner</li> 
<li>Principal</li> 
<li>Final</li></ul> 
<p>La planification Workfront n’est pas disponible pour les plans Workfront hérités</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Package de planification Adobe Workfront*</p></td> 
   <td> 
<p>Tous </p> 
<p>Pour plus d’informations sur les éléments inclus dans chaque plan de planification Workfront, contactez votre gestionnaire de compte Workfront. </p> 
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
   <td><p> Standard </p>
   <p>La planification Workfront n’est pas disponible pour les licences Workfront héritées</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuration du niveau d’accès</p></td> 
   <td> <p>Il n’existe aucun contrôle de niveau d’accès pour Adobe Workfront Planning.</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td>   <p>Gérer les autorisations d’un espace de travail </p>  
   <p>L’administration système a accès à tous les espaces de travail, y compris ceux qu’elle n’a pas créés.</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modèle de disposition</p></td> 
   <td> <p>Toutes les personnes, y compris les administrateurs et administratrices de Workfront, doivent se voir attribuer un modèle de mise en page incluant la zone Planning dans le menu principal. </p> </td> 
  </tr> 
</tbody> 
</table>

* Pour plus d’informations sur les exigences d’accès à Workfront, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Remarques sur les miniatures d’enregistrements

Pour faire la distinction visuelle entre les enregistrements dans une vue de tableau, vous pouvez associer une miniature unique à chaque enregistrement.

Tenez compte des points suivants :

* Une miniature est propre à un enregistrement et ne s’applique pas à tous les enregistrements du même type.
* Vous pouvez uniquement ajouter des fichiers image sous forme de miniatures.
  <!--above: when you know exactly what type of files are allowed, add the exact extensions above-->
* Vous pouvez ajouter une miniature à des enregistrements individuels dans la vue de tableau ou à partir de la page ou de la zone d’aperçu de l’enregistrement.
* Workfront télécharge automatiquement une miniature chaque fois que vous créez un enregistrement. Vous pouvez modifier cette image ultérieurement.
* Les miniatures appartiennent aux informations d’enregistrement et s’affichent dans les zones où s’affichent les enregistrements. Par exemple, les miniatures s’affichent avec les informations des enregistrements dans les zones suivantes :

   * Champ principal d’un enregistrement dans la vue de tableau
   * Barre d’enregistrement dans la vue chronologique.
   * Aperçu et page des détails de l’enregistrement.

## Ajouter une miniature à un enregistrement

Vous pouvez ajouter une miniature de la manière suivante :

* [Ajout d’une miniature à un enregistrement à partir de la vue de tableau](#add-a-thumbnail-to-a-record-from-the-table-view)
* [Ajout d’une miniature à un enregistrement à partir de la page de détails](#add-a-thumbnail-to-a-record-from-the-details-page)

### Ajout d’une miniature à un enregistrement à partir de la vue de tableau

{{step1-to-planning}}

1. Cliquez sur l’espace de travail pour lequel vous souhaitez ajouter des miniatures, puis cliquez sur la carte de type d’enregistrement.

   Cela ouvre la page du type d’enregistrement.
1. Sélectionnez une vue de tableau dans le menu déroulant **Vue**. Tous les enregistrements du type que vous avez sélectionné s’affichent dans un tableau.
1. Pointez sur les informations du champ principal, puis cliquez sur le menu **Plus** ![](assets/more-menu.png), et enfin sur **Miniature**.

   ![](assets/record-more-menu-expanded.png)

   >[!TIP]
   >
   >   Le champ principal est le champ qui s’affiche dans la première colonne d’une vue de tableau. Le champ principal est toujours gelé et ne peut pas être masqué ni déplacé. L’option Miniature n’est pas disponible dans le menu Plus lorsque le champ principal est un champ de formule.

   L’onglet **Télécharger** s’ouvre par défaut dans la zone **Miniature des enregistrements**.

   Pour plus d’informations sur le téléchargement de la miniature, reportez-vous à la section [Ajout d’une miniature à un enregistrement à partir de la page de détails](#add-a-thumbnail-to-a-record-from-the-details-page) de cet article, en commençant par l’étape 6. <!--see if this is accurate-->

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

   Cela ouvre la page du type d’enregistrement.
1. Dans n’importe quelle vue, cliquez sur un enregistrement pour l’ouvrir.

   La zone d’aperçu des détails s’affiche.
1. (Facultatif) Cliquez sur l’icône **Ouvrir dans un nouvel onglet** ![](assets/open-details-in-a-new-tab-icon.png) dans le coin supérieur droit.

   La page de détails de l’enregistrement s’ouvre.

1. (Conditionnel) Dans l’aperçu de l’enregistrement ou la page, passez la souris sur l’image miniature ou l’icône ![](assets/record-thumbnail-icon-on-details-page.png), puis cliquez sur le menu **Plus** ![](assets/more-menu.png) > **Modifier la miniature** dans l’environnement de production.

   Ou

   <span class="preview"> Pointez sur l’espace situé au-dessus du nom de l’enregistrement, puis cliquez sur **Ajouter une miniature** ou **Modifier la miniature** dans l’environnement de prévisualisation.</span>

   L’onglet **Télécharger** s’ouvre par défaut dans la zone **Miniature des enregistrements**.

   ![](assets/record-thumbnail-box-for-upload.png)

1. Faites glisser et déposez un fichier à ajouter en tant que miniature.

   Ou

   Cliquez sur **Parcourir les images**, puis recherchez un fichier image à ajouter. Le fichier doit être enregistré sur votre ordinateur.

1. (Facultatif) Une fois l’image téléchargée dans la zone **Record thumbnail**, utilisez l’outil de dimensionnement pour recadrer et redimensionner l’image.
1. (Facultatif) Cliquez sur l&#39;icône **Télécharger une nouvelle image** ![](assets/upload-new-image-icon.png) pour télécharger une autre image.
1. (Facultatif) Cliquez sur l’onglet **Galerie** , puis sur une image. La galerie d’images ne peut pas être modifiée.

   ![](assets/record-thumbnail-box-for-gallery.png)

1. (Facultatif) Pour supprimer la miniature avant qu’elle ne soit enregistrée, cliquez sur l’icône **Supprimer** ![](assets/remove-image-icon.png) située à droite de l’image.

1. Cliquez sur **Utiliser l’image** pour ajouter l’image en tant que miniature.
Cela ferme la boîte **Record thumbnail**.
La miniature s’affiche dans les zones de la planification Workfront où s’affiche l’enregistrement.

   >[!TIP]
   >
   >   Vous devez activer le champ Miniature dans la vue Tableau pour afficher les miniatures dans cette vue. Elle est désactivée par défaut.

1. (Facultatif) Pour supprimer la miniature après son enregistrement, cliquez sur un enregistrement dans n’importe quelle vue pour ouvrir la page de détails, puis survolez l’image miniature avec la souris et cliquez sur l’icône **Plus** ![](assets/more-menu.png)> **Supprimer** ![](assets/remove-image-icon.png) . L’image miniature est supprimée.




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