---
title: Supprimer enregistrements
description: Vous pouvez supprimer des enregistrements que vous ou une autre personne avez créés.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 3f7a3667-8a9f-462a-b706-cf15850a0d1c
source-git-commit: fd8e5d3baf6af0dbdd1275494fad54b204abd1a5
workflow-type: tm+mt
source-wordcount: '701'
ht-degree: 52%

---


# Supprimer des enregistrements

<!--take Preview and Production references out at release-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Vous pouvez supprimer des enregistrements qui ne sont plus pertinents dans Adobe Workfront Planning. Vous pouvez récupérer les enregistrements supprimés pendant 30 jours après leur suppression. Pour plus d’informations sur la récupération des enregistrements supprimés, voir [ Récupérer les enregistrements supprimés ](/help/quicksilver/planning/records/restore-deleted-records.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès.

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
<p>Pour plus d’informations sur les éléments inclus dans chaque plan de planification Workfront, contactez votre gestionnaire de compte Workfront. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Plateforme Adobe Workfront</p></td> 
   <td> 
<p>L’instance de Workfront de votre entreprise doit être intégrée à l’expérience unifiée Adobe pour pouvoir accéder à toutes les fonctionnalités de Workfront Planning.</p> 
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
   <td>   <p>Autorisations de niveau Contributeur ou supérieur à un espace de travail <!--<span class="preview">and record type</span>--> </a> </p>  
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

## Considérations sur la suppression des enregistrements

* Vous pouvez supprimer des enregistrements que vous ou une autre personne avez créés.
* Vous ne pouvez pas récupérer les enregistrements supprimés dans l’environnement de production. Vous pouvez récupérer les enregistrements supprimés dans l’environnement de Prévisualisation.
* Lorsque des enregistrements supprimés sont liés à d’autres enregistrements, ces enregistrements liés restent intacts, bien que les informations de l’enregistrement supprimé soient éliminées.
* Vous ne pouvez pas supprimer des enregistrements des vues Chronologie ou Calendrier.

## Supprimer des enregistrements

Vous pouvez supprimer un enregistrement à partir des zones suivantes :

* [À partir de la page de l’enregistrement](#delete-a-record-from-the-records-page)
* [À partir de la vue de tableau d’un type d’enregistrement](#delete-a-record-from-the-record-type-table-view)

### Supprimer un enregistrement à partir de la page de l’enregistrement

{{step1-to-planning}}

1. Cliquez sur l’espace de travail dont vous souhaitez supprimer les enregistrements.

   L’espace de travail s’ouvre et les types d’enregistrements s’affichent sous forme de cartes.

1. Cliquez sur la vignette d’un type d’enregistrement pour plus de détails.

   La page du type d’enregistrement s’ouvre.
1. Utilisez l’une des méthodes suivantes :

   * À partir d’une vue en tableau, cliquez sur le nom d’un enregistrement.
   * Dans la vue en tableau, pointez sur le nom d’un enregistrement, puis cliquez sur le menu **Plus** ![](assets/more-menu.png), puis sur **Vue**.

     ![](assets/contextual-menu-for-record-row.png)
   * Dans une vue de chronologie, cliquez sur une barre d’un enregistrement.

   La page de l’enregistrement s’ouvre.

1. Cliquez sur le menu **Plus** ![](assets/more-menu.png) à droite du nom de l’enregistrement, cliquez sur **Supprimer**, puis à nouveau sur **Supprimer** pour confirmer.

   ![](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed-->
L’enregistrement est supprimé.
1. (Facultatif et conditionnel) Si vous supprimez l&#39;enregistrement dans l&#39;environnement Aperçu, accédez à la vue Tableau de la page d&#39;enregistrement, puis cliquez sur l&#39;icône **Annuler** ![](assets/undo-icon.png) dans le coin supérieur droit de la vue, puis cliquez sur **Récemment supprimé** pour récupérer les enregistrements supprimés.

Pour plus d’informations sur la récupération des enregistrements supprimés, voir [ Récupérer les enregistrements supprimés ](/help/quicksilver/planning/records/restore-deleted-records.md).

### Supprimer un enregistrement de la vue en tableau d’un type enregistrement

{{step1-to-planning}}

1. Cliquez sur l’espace de travail dont vous souhaitez supprimer les enregistrements.

   L’espace de travail s’ouvre et les types d’enregistrements s’affichent sous forme de cartes.

1. Cliquez sur la vignette d’un type d’enregistrement pour plus de détails.

   La page de type d’enregistrement s’ouvre.
1. (Conditionnel) Dans le menu déroulant **Afficher** situé dans le coin supérieur gauche du tableau, sélectionnez une vue de tableau. Il s’agit de la vue par défaut, sauf si vous avez visualisé le type d’enregistrement dans la vue Chronologique lors de votre dernier accès.

   Les enregistrements associés au type d’enregistrement sélectionné s’affichent dans la vue Tableau.
1. Utilisez l’une des méthodes suivantes :

   * Cliquez avec le bouton droit de la souris sur une ligne d’enregistrement, puis cliquez sur **Supprimer**.
   * Cliquez sur le ![](assets/more-menu.png) de menu **Plus** à droite du nom de l’enregistrement, puis cliquez sur **Supprimer**.

     ![](assets/contextual-menu-for-record-row.png)

   * Cliquez sur l’icône **Ouvrir les détails** ![](assets/open-details-icon-in-table-name-field.png) pour ouvrir la boîte contenant les informations détaillées de l’enregistrement, cliquez sur **Plus** ![](assets/more-menu.png) à droite du nom de l’enregistrement, puis sur **Supprimer**.

   L’enregistrement est supprimé.

1. (Facultatif) Effectuez l’une des opérations suivantes pour annuler ou rétablir la suppression d’un enregistrement :

   * Cliquez sur l&#39;icône **Annuler** ![](assets/undo-icon.png), puis **Récemment supprimé** pour récupérer les enregistrements supprimés. Pour plus d’informations sur la récupération des enregistrements supprimés, voir [ Récupérer les enregistrements supprimés ](/help/quicksilver/planning/records/restore-deleted-records.md).
   * Utilisez les raccourcis clavier suivants pour annuler ou rétablir la suppression d’un enregistrement :

      * Ctrl + Z (⌘ + Z pour Mac) pour annuler la suppression d’un enregistrement
      * Ctrl+Maj+Z (⌘+Maj+Z pour Mac) pour rétablir la suppression de l’enregistrement.




