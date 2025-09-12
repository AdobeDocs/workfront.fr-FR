---
title: Vues d’enregistrements en double
description: Si vous souhaitez conserver plusieurs versions d'une vue et apporter de légères modifications entre les versions, vous pouvez dupliquer une vue dans Adobe Workfront Planning. Cet article décrit comment dupliquer une vue.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 441a53d1-ad39-41b7-93fe-2ae1836476c9
source-git-commit: bfb0fd2956ffb9384a09882864668d5dba33a53b
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 35%

---

# Dupliquer les vues d’enregistrement

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->


{{planning-important-intro}}

Si vous souhaitez conserver plusieurs versions d&#39;une vue et apporter de légères modifications entre les versions, vous pouvez dupliquer une vue dans Adobe Workfront Planning.

La duplication d’une vue crée des copies identiques d’une vue existante.

Les autorisations de partage de la vue d’origine ne sont pas transférées à la vue dupliquée.

La duplication des vues est identique pour tous les types de vues dans Workfront Planning.

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
   <td><p> Standard </p>
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
   <td>   <p>Gérer les autorisations pour une vue</p>  
   <p>Autorisations d’affichage d’une vue pour modifier temporairement les paramètres d’affichage ou la dupliquer.</p> </td> 
  </tr> 
</tbody> 
</table>

* Pour plus d’informations sur les exigences d’accès à Workfront, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

## Dupliquer une vue d’enregistrement

{{step1-to-planning}}

1. Cliquez sur la vignette d’un espace de travail.

   L’espace de travail s’ouvre et les types d’enregistrements s’affichent sous forme de cartes.

1. Cliquez sur la vignette d’un type d’enregistrement pour plus de détails.

   La page de type d’enregistrement s’ouvre.
Par défaut, tous les enregistrements du type sélectionné s&#39;affichent dans la vue de tableau.

1. Pointez sur l’onglet de la vue à dupliquer, puis cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) à droite du nom de la vue, puis cliquez sur **Dupliquer**.

   ![Menu Afficher plus sur une vue d’enregistrement](assets/view-more-menu-with-duplicate-option.png)

   <!--at preview release, replace the step above with this one: 
    1. Depending on which environment you use, do the following: 
    * In the Production environment, hover over one the of the view's names in the view tab, then click **More** ![More menu](assets/more-menu.png) to the left of the view name, then click **Duplicate**. 
    * <span class="preview">In the Preview environment, click the dropdown icon ![Dropdown icon](assets/drop-down-icon.png) next to the current view name, hover over the name of a view, click **More**, then **Duplicate**.</span>-->
   La vue est dupliquée et le nom de la nouvelle vue suit le modèle suivant : `Original view's name (Copy)`. Le nouvel onglet de vue s’affiche à la fin de tous les onglets de vue.
