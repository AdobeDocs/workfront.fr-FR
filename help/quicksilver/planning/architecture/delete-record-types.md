---
title: Supprimer types d’enregistrements
description: Vous pouvez supprimer des types d’enregistrement lorsqu’ils ne sont plus pertinents. La suppression des types d’enregistrement supprime également toutes les informations associées aux types d’enregistrement, telles que leurs enregistrements, champs et vues.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 70fd3887-3871-45b5-9c21-f57da63662aa
source-git-commit: 7d37481fc5b468f6f8ea1fce6ccd7ae064f00251
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 53%

---


<!--keep the global record type reference in yellow till January 2026-->

# Supprimer des types d’enregistrements

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Vous pouvez supprimer des types d’enregistrement lorsqu’ils ne sont plus pertinents.

Cependant, la suppression des types d’enregistrement supprime également toutes les informations associées aux types d’enregistrement. Pour plus d’informations, consultez la section [Remarques concernant la suppression de types d’enregistrement](#considerations-when-deleting-record-types) de cet article.

Pour plus d’informations sur les types d’enregistrements, voir [&#x200B; Présentation des types d’enregistrements &#x200B;](/help/quicksilver/planning/architecture/overview-of-record-types.md).

<!-- last sentence might need to be deleted when we can recover or replace deleted record types-->

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès. 

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
<li>Prime</li> 
<li>Ultimate</li></ul> 
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
<p>L’instance de Workfront de votre organisation doit être intégrée à l’expérience unifiée Adobe pour pouvoir accéder à Workfront Planning.</p> 
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
   <td>   <p>Gestion des autorisations relatives à un espace de travail et à un type d’enregistrement</p>  
   <p>L’administration système a accès à tous les espaces de travail, y compris ceux qu’elle n’a pas créés.</p></td> 
  </tr> 
</tbody> 
</table>

* Pour plus d’informations sur les exigences d’accès à Workfront, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   


## Remarques concernant la suppression de types d’enregistrement

<!--check this and ensure these are still true - some things might change with / after closed beta-->

* Vous ne pouvez supprimer que les types d’enregistrement des espaces de travail pour lesquels vous disposez d’autorisations de gestion.
* La suppression des types d’enregistrement supprime les informations suivantes qui leur sont associées :

   * Tous les enregistrements de ce type
   * Tous les champs associés au type d’enregistrement
   * Toutes les vues (y compris les filtres, les regroupements et les critères de tri) du type d’enregistrement
* Le type d’enregistrement est supprimé pour toutes les personnes accédant à l’espace de travail.
* La suppression des types d’enregistrements et leurs informations associées est irréversible.
* Il est recommandé de recréer les champs et les enregistrements associés au type d’enregistrement que vous souhaitez supprimer sur un autre type d’enregistrement avant de les supprimer.

<!--

<div class="preview">

* You cannot delete a global record type that has been added to other workspaces. 
   
   You must first delete it from the secondary workspaces where it's been added, before you can delete it from its original workspace. 

   Deleting a global record type from their secondary workspaces only remove them, their records, and that workspace's fields from the secondary workspace. It does not delete the global record type from its original workspace.

   For information, see the section "Delete a global record type from a secondary workspace" in the article [Add existing record types from another workspace](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md). 

</div>
-->

## Supprimer des types d’enregistrements

{{step1-to-planning}}

1. Cliquez sur l’espace de travail dont vous souhaitez supprimer les types d’enregistrements,

   Ou

   Depuis un espace de travail, développez la flèche pointant vers le bas à droite d’un nom d’espace de travail existant, recherchez un espace de travail, puis sélectionnez-le lorsqu’il s’affiche dans la liste.

   L’espace de travail et les types d’enregistrement s’affichent.
1. Utilisez l’une des méthodes suivantes :

   * Pointez sur la carte de type d’enregistrement, cliquez sur le menu **Plus**, puis **Supprimer**.
   * Cliquez sur la carte du type d’enregistrement à supprimer, puis, dans la page du type d’enregistrement, cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) à droite du nom du type d’enregistrement, puis cliquez sur **Supprimer**.

   ![Confirmation de suppression définitive du type d’enregistrement](assets/permanently-delete-record-type-confirmation.png)

   <!--[!TIP]
   >
   ><span class="preview">You cannot delete global record types added to other workspaces. First, delete the global record types form their secondary workspaces before deleting them from the original workspace.</span>-->


1. Saisissez **delete** dans la zone de confirmation, puis cliquez sur **Supprimer définitivement**. Cette opération n’est pas sensible à la casse.

   Le type d&#39;enregistrement sélectionné, ainsi que ses champs, les enregistrements associés et les vues sont supprimés et ne peuvent pas être récupérés.


