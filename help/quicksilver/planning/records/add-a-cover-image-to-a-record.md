---
title: Ajout d’une image de couverture à un enregistrement
description: Vous pouvez personnaliser les enregistrements en ajoutant une image de couverture à la page d'enregistrement dans Adobe Workfront Planning, lors de la modification d'un enregistrement.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 93c6bc15-d945-4cfc-8e87-f5b4e6fac2f4
source-git-commit: 8546311acf722c0f4d47d4663b02ff701416894a
workflow-type: tm+mt
source-wordcount: '648'
ht-degree: 13%

---


# Ajouter une image de couverture à un enregistrement

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Vous pouvez personnaliser les enregistrements en ajoutant une image de couverture à la page d&#39;enregistrement dans Adobe Workfront Planning, lors de la modification d&#39;un enregistrement.

Pour plus d’informations sur la modification des enregistrements, voir [Modifier les enregistrements](/help/quicksilver/planning/records/edit-records.md).

Vous devez créer des types d’enregistrements avant de pouvoir commencer à créer et modifier des enregistrements.

Pour plus d’informations, consultez [Créer des types d’enregistrements](/help/quicksilver/planning/architecture/create-record-types.md).

## Conditions d’accès

+++ Développez pour afficher les conditions d’accès requises pour la fonctionnalité de cet article. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Package Adobe Workfront</p></td> 
   <td> 
<ul> 
<li><p>Tout Workfront et tout package Planning</p></li>
Ou
<li><p>Tout workflow et tout package Planning</p></li></ul>
<p>Pour plus d’informations sur les composants inclus dans chaque package Workfront Planning, contactez votre représentant de compte Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td>   <p>Autorisations de niveau Contribution ou supérieur à un espace de travail et à un type d’enregistrement  </p>  
   <p>L’administration système a accès à tous les espaces de travail, y compris ceux qu’elle n’a pas créés.</p> </td> 
  </tr>   
</tbody> 
</table>

Pour plus d’informations sur les exigences d’accès à Workfront, voir [Exigences d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   


<!--Old:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning package, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard</p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Contribute or higher permissions to a workspace and record type  </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
</tbody> 
</table> -->

## Considérations relatives aux images de couverture de page d’enregistrement

Vous pouvez personnaliser la page d&#39;un enregistrement en y ajoutant une image de couverture.

Tenez compte des points suivants :

* Une image de couverture est propre à un enregistrement et ne s’applique pas à tous les enregistrements du même type.
* Vous pouvez ajouter uniquement des fichiers image en tant qu’images de couverture.
  <!--above: when you know exactly what type of files are allowed, add the exact extensions above-->
* Vous pouvez ajouter une image de couverture à des enregistrements individuels depuis l’aperçu de l’enregistrement dans n’importe quel affichage ou à partir de la page d’enregistrement.
* Vous ne pouvez pas ajouter d’images de couverture à partir d’une vue d’enregistrement.
* Workfront charge automatiquement une image de couverture à chaque fois que vous créez un enregistrement. Vous pouvez modifier cette image ultérieurement.

## Ajouter une image de couverture à un enregistrement

Vous pouvez personnaliser un enregistrement en ajoutant une image de couverture en haut de l&#39;aperçu de l&#39;enregistrement ou de la page.

{{step1-to-planning}}

1. Cliquez sur l’espace de travail dont vous souhaitez personnaliser les enregistrements,

   Ou

   Depuis un espace de travail, développez la flèche pointant vers le bas à droite d’un nom d’espace de travail existant, recherchez un espace de travail, puis sélectionnez-le lorsqu’il s’affiche dans la liste.

   L’espace de travail et les types d’enregistrement s’affichent.

1. Cliquez sur la vignette d’un type d’enregistrement pour plus de détails.

   La page de type d’enregistrement s’ouvre.

1. Dans une vue de n’importe quel type, cliquez sur un enregistrement

   Ou

   Dans la vue du tableau, cliquez sur l’icône **Ouvrir les détails** ![Ouvrir les détails](assets/open-details-icon-in-table-name-field.png) dans la première colonne.

   L’aperçu de l’enregistrement s’ouvre dans la vue.

   ![Zone d’aperçu des détails](assets/details-box.png)


1. (Facultatif) Cliquez sur l’icône **Ouvrir dans un nouvel onglet** ![Icône Ouvrir dans un nouvel onglet](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> dans le coin supérieur droit de l’aperçu de l’enregistrement pour ouvrir la page de l’enregistrement dans un nouvel onglet.

   La page de l’enregistrement s’ouvre.

   ![Page de détails](assets/details-page.png)

1. Dans la page d’aperçu ou de détails de l’enregistrement, passez le curseur sur l’espace au-dessus du nom de l’enregistrement, puis cliquez sur **Ajouter une couverture**.

   Ou

   Pointez sur une image de couverture existante, cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) , puis cliquez sur **Télécharger**. <!--check the casing here; I logged a bug for this-->
La boîte de dialogue **Couverture d’enregistrement** s’ouvre dans l’onglet **Télécharger**.

   ![Zone d’enregistrement pour le chargement](assets/record-cover-box-for-upload.png)

1. Cliquez sur **Parcourir les images** et recherchez une image sur votre ordinateur pour la sélectionner et l’ajouter.

1. (Facultatif) Pour supprimer l’image avant de l’enregistrer, cliquez sur l’icône **Charger une nouvelle image** ![Charger une nouvelle image](assets/upload-new-image-icon.png) , puis chargez une nouvelle image.

1. (Facultatif) Cliquez sur l’onglet **Galerie**, puis cliquez sur une image dans la galerie d’images. La galerie d’images ne peut pas être modifiée.

   ![Boîte de couverture d&#39;enregistrement pour galerie](assets/record-cover-box-for-gallery.png)

1. Cliquez sur **Utiliser l’image**.

   L’image est chargée en haut de la page d’aperçu ou de détails de l’enregistrement et les modifications sont enregistrées automatiquement.

   ![Enregistrer la page avec l’image de couverture](assets/record-page-with-cover-image.png)

1. (Facultatif) Pointez sur l’image, puis cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) dans le coin inférieur droit de l’image de couverture, puis effectuez l’une des opérations suivantes :

   * Cliquez sur **Télécharger** si vous souhaitez remplacer l’image de couverture et répétez l’étape 6 pour télécharger et enregistrer une nouvelle image.
   * Cliquez sur **Repositionner**, puis utilisez l’outil **Repositionner** ![Icône de l’outil de repositionnement](assets/reposition-tool-icon.png) pour centrer l’image de couverture, puis cliquez sur **Enregistrer** lorsque vous avez terminé.
   * Cliquez sur **Supprimer** pour supprimer l’image de couverture.

   Workfront enregistre automatiquement vos modifications.
