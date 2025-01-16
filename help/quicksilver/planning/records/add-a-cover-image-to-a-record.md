---
title: Ajout d’une image de couverture à un enregistrement
description: Vous pouvez personnaliser les enregistrements en ajoutant une image de couverture à la page d'enregistrement dans Adobe Workfront Planning, lors de la modification d'un enregistrement.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 93c6bc15-d945-4cfc-8e87-f5b4e6fac2f4
source-git-commit: ba17bd824717f61e72fb9a73c8b90fbe755e20d8
workflow-type: tm+mt
source-wordcount: '709'
ht-degree: 24%

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

+++ Développez pour afficher les exigences d’accès pour Workfront Planning.

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
<p>L’un des plans Workfront suivants :</p> 
<ul><li>Sélectionner</li> 
<li>Principal</li> 
<li>Final</li></ul> 
<p>Workfront Planning n’est pas disponible pour les plans Workfront hérités</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Package Adobe Workfront Planning*</p></td> 
   <td> 
<p>Tous </p> 
<p>Pour plus d’informations sur les composants inclus dans chaque package Workfront Planning, contactez votre gestionnaire de compte Workfront. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Plateforme Adobe Workfront</p></td> 
   <td> 
<p>L’instance de Workfront de votre organisation doit être intégrée à l’expérience unifiée Adobe pour pouvoir accéder à toutes les fonctionnalités de Workfront Planning.</p> 
<p>Pour plus d’informations, voir <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience pour Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront*</p></td> 
   <td><p> Standard</p>
   <p>Workfront Planning n’est pas disponible pour les licences Workfront héritées</p> 
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

   Dans la vue Tableau, cliquez sur l’icône **Ouvrir les détails** ![](assets/open-details-icon-in-table-name-field.png) dans la première colonne.

   L’aperçu de l’enregistrement s’ouvre dans la vue.

   ![](assets/details-box.png)

1. (Facultatif) Cliquez sur l’icône **Ouvrir dans un nouvel onglet** ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> dans le coin supérieur droit de l’aperçu de l’enregistrement pour ouvrir la page de l’enregistrement dans un nouvel onglet.

   La page de l’enregistrement s’ouvre.

   ![](assets/details-page.png)

1. Dans la page d’aperçu ou de détails de l’enregistrement, passez le curseur sur l’espace au-dessus du nom de l’enregistrement, puis cliquez sur **Ajouter une couverture**.

   Ou

   Pointez sur une image de couverture existante, cliquez sur l’![](assets/more-menu.png) de menu **Plus**, puis cliquez sur **Télécharger**. <!--check the casing here; I logged a bug for this-->
La boîte de dialogue **Couverture d’enregistrement** s’ouvre dans l’onglet **Télécharger**.

   ![](assets/record-cover-box-for-upload.png)

1. Cliquez sur **Parcourir les images** et recherchez une image sur votre ordinateur pour la sélectionner et l’ajouter.

1. (Facultatif) Pour supprimer l’image avant de l’enregistrer, cliquez sur l’icône **Télécharger une nouvelle image** ![](assets/upload-new-image-icon.png) , puis chargez une nouvelle image.

1. (Facultatif) Cliquez sur l’onglet **Galerie**, puis cliquez sur une image dans la galerie d’images. La galerie d’images ne peut pas être modifiée.

   ![](assets/record-cover-box-for-gallery.png)

1. Cliquez sur **Utiliser l’image**.

   L’image est chargée en haut de la page d’aperçu ou de détails de l’enregistrement et les modifications sont enregistrées automatiquement.

   ![](assets/record-page-with-cover-image.png)

1. (Facultatif) Pointez sur l’image, puis cliquez sur le ![](assets/more-menu.png) de menu **Plus** dans le coin inférieur droit de l’image de couverture, puis effectuez l’une des opérations suivantes :

   * Cliquez sur **Télécharger** si vous souhaitez remplacer l’image de couverture et répétez l’étape 6 pour télécharger et enregistrer une nouvelle image.
   * Cliquez sur **Repositionner**, puis utilisez l’outil **Repositionner** ![](assets/reposition-tool-icon.png) pour centrer l’image de couverture, puis cliquez sur **Enregistrer** lorsque vous avez terminé.
   * Cliquez sur **Supprimer** pour supprimer l’image de couverture.

   Workfront enregistre automatiquement vos modifications.
