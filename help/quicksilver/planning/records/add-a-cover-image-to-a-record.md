---
title: Ajout d’une image de couverture à un enregistrement
description: Vous pouvez personnaliser des enregistrements en ajoutant une image de couverture à la page d’enregistrement dans Adobe Workfront Planning, lors de la modification d’un enregistrement.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 93c6bc15-d945-4cfc-8e87-f5b4e6fac2f4
source-git-commit: cf42511263ec1cffd90d1e4bdcd43521b7fe6a30
workflow-type: tm+mt
source-wordcount: '699'
ht-degree: 23%

---


# Ajouter une image de couverture à un enregistrement

{{planning-important-intro}}

Vous pouvez personnaliser des enregistrements en ajoutant une image de couverture à la page d’enregistrement dans Adobe Workfront Planning, lors de la modification d’un enregistrement.

Pour plus d&#39;informations sur la modification des enregistrements, voir [Modifier les enregistrements](/help/quicksilver/planning/records/edit-records.md).

Vous devez créer des types d’enregistrement avant de pouvoir commencer à créer et modifier des enregistrements.

Pour plus d’informations, voir [Créer des types d’enregistrements](/help/quicksilver/planning/architecture/create-record-types.md).

## Conditions d’accès

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
   <td><p> Standard</p>
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
   <p>Les équipes d’administration système ont des droits sur tous les espaces de travail, y compris ceux qu’ils n’ont pas créés.</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modèle de disposition</p></td> 
   <td> <p>Toutes les personnes, y compris les administrateurs et administratrices de Workfront, doivent se voir attribuer un modèle de mise en page incluant la zone Planning dans le menu principal. </p> </td> 
  </tr> 
</tbody> 
</table>

* Pour plus d’informations sur les exigences d’accès à Workfront, consultez les [Conditions d’accès requises dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


<!--

OLD: 
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
   <td> <p>There are no access controls for Workfront Planning </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td>  <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Planning area in the Main Menu. </p> <p>For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>

 </tbody>
</table>

*For more information, see [Access requirements in Workfornt documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

-->

## Considérations relatives aux images de couverture de page d’enregistrement

Vous pouvez personnaliser la page d’un enregistrement en y ajoutant une image de couverture.

Tenez compte des points suivants :

* Une image de couverture est propre à un enregistrement et ne s’applique pas à tous les enregistrements du même type.
* Vous pouvez uniquement ajouter des fichiers image comme images de couverture.
  <!--above: when you know exactly what type of files are allowed, add the exact extensions above-->
* Vous pouvez ajouter une image de couverture à des enregistrements individuels à partir de l’aperçu de l’enregistrement dans n’importe quelle vue ou à partir de la page d’enregistrement.
* Vous ne pouvez pas ajouter d’images de couverture à partir d’une vue d’enregistrement.
* Workfront télécharge automatiquement une image de couverture chaque fois que vous créez un enregistrement. Vous pouvez modifier cette image ultérieurement.

## Ajouter une image de couverture à un enregistrement

Vous pouvez personnaliser un enregistrement en ajoutant une image de couverture en haut de l’aperçu de l’enregistrement ou de la page.

{{step1-to-planning}}

1. Cliquez sur l&#39;espace de travail dont vous souhaitez personnaliser les enregistrements,

   Ou

   Dans un espace de travail, développez la flèche pointant vers le bas située à droite du nom d’un espace de travail existant, recherchez un espace de travail, puis sélectionnez-le lorsqu’il s’affiche dans la liste.

   L’espace de travail et les types d’enregistrement s’affichent.

1. Cliquez sur une carte de type d’enregistrement.

   La page du type d’enregistrement s’ouvre.

1. Dans une vue quel que soit le type, cliquez sur un enregistrement.

   Ou

   Dans la vue table, cliquez sur l&#39;icône **Ouvrir les détails** ![](assets/open-details-icon-in-table-name-field.png) dans la première colonne.

   L’aperçu de l’enregistrement s’ouvre dans la vue.

   ![](assets/details-box.png)

1. (Facultatif) Cliquez sur l’icône **Ouvrir dans un nouvel onglet** ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> dans le coin supérieur droit de l’aperçu de l’enregistrement pour ouvrir la page de l’enregistrement dans un nouvel onglet.

   La page de l’enregistrement s’ouvre.

   ![](assets/details-page.png)

1. Dans l’aperçu de l’enregistrement ou la page, cliquez sur **Ajouter une couverture**


   Ou

   Pointez sur une image de couverture existante, cliquez sur le menu **Plus** ![](assets/more-menu.png) , puis sur **Télécharger**. <!--check the casing here; I logged a bug for this-->
La zone **Record cover** s’ouvre dans l’onglet **Upload**.

   ![](assets/record-cover-box-for-upload.png)

1. Cliquez sur **Parcourir les images** et rechercher une image sur votre ordinateur pour la sélectionner et l&#39;ajouter.

1. (Facultatif) Pour supprimer l’image avant qu’elle ne soit enregistrée, cliquez sur l’icône **Télécharger une nouvelle image** ![](assets/upload-new-image-icon.png) et téléchargez une nouvelle image.

1. (Facultatif) Cliquez sur l’onglet **Galerie** , puis cliquez sur une image dans la galerie d’images. La galerie d’images ne peut pas être modifiée.

   ![](assets/record-cover-box-for-gallery.png)

1. Cliquez sur **Utiliser l&#39;image**.

   L’image est téléchargée en haut de l’aperçu de l’enregistrement ou de la page et les modifications sont enregistrées automatiquement.

   ![](assets/record-page-with-cover-image.png)

1. (Facultatif) Pointez sur l’image, puis cliquez sur le menu **Plus** ![](assets/more-menu.png) dans le coin inférieur droit de l’image de couverture, puis effectuez l’une des opérations suivantes :

   * Cliquez sur **Télécharger** si vous souhaitez remplacer l’image de couverture et répétez l’étape 6 pour télécharger et enregistrer une nouvelle image.
   * Cliquez sur **Reposition** et utilisez l’outil **Reposition** ![](assets/reposition-tool-icon.png) pour centrer l’image de couverture, puis cliquez sur **Enregistrer** lorsque vous avez terminé.
   * Cliquez sur **Supprimer** pour supprimer l’image de couverture.

   Workfront enregistre automatiquement vos modifications.
