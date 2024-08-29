---
product-previous: workfront-goals
navigation-topic: goal-review-and-sections
title: Gérer des objectifs dans la liste des objectifs d’Objectifs Adobe Workfront
description: Une fois que vous ou d’autres utilisateurs et utilisatrices avez créé des objectifs, vous pouvez consulter leur progression et leurs informations dans la liste des objectifs. Pour plus d’informations sur la création d’objectifs, voir Création d’objectifs dans Objectifs Adobe Workfront.
author: Alina
feature: Workfront Goals
exl-id: 2a2c1240-f796-4cb8-b8a6-2ad5853916b9
source-git-commit: d7dd5ab4e3041a100b13c5bf169747f58db0ea39
workflow-type: tm+mt
source-wordcount: '803'
ht-degree: 100%

---

# Gérer des objectifs dans la liste des objectifs d’Objectifs Adobe Workfront

<!-- printing or exporting goals is no longer possible, but see if they add it later-->

Une fois que vous ou d’autres utilisateurs et utilisatrices avez créé des objectifs, vous pouvez consulter leur progression et leurs informations dans la liste des objectifs. Pour plus d’informations sur la création d’objectifs, voir [Création d’objectifs dans Objectifs Adobe Workfront](../../workfront-goals/goal-management/create-goals.md).

## Conditions d’accès

Pour effectuer les actions décrites dans cet article, vous devez disposer de l’accès suivant :

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td> 
   <p>Pour la nouvelle structure de forfait et de licence :
  <ul><li>Un forfait Ultimate </li></ul>
   </p>
<p>Pour la structure de forfait et de licence actuelle : 
<ul><li> Un forfait Pro ou supérieur </li>
  <li>Une licence Objectifs Adobe Workfront en plus d’une licence Workfront.</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Licence Adobe Workfront*</td>
 <td>
 <p>Nouvelle licence : contributeur ou contributrice ou supérieure</p>
 Ou
 <p>Licence actuelle : demande ou supérieure</p> <p>Pour plus d’informations, voir <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Vue d’ensemble des licences Adobe Workfront</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Produit*</td>
 <td>
 <p> Nouvelle exigence de produit, une des options suivantes : </p>
<ul>
<li>Un forfait Adobe Workfront Select ou Prime et une licence Objectifs Adobe Workfront supplémentaire.</li>
<li>Un forfait Workfront Ultimate qui inclut Objectifs Workfront par défaut. </li></ul>
 <p>Ou</p>
 <p>Exigence de produit actuelle : un forfait Workfront et une licence supplémentaire pour Objectifs Adobe Workfront. </p> <p>Pour plus d’informations, consultez la section <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Exigences pour l’utilisation des Objectifs Workfront</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Niveau d’accès</td>
 <td> <p>Modifier l’accès aux Objectifs</p>  </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Autorisations d’objet</td>
 <td>
  <div>
  <p>Autorisations d’affichage ou de niveau supérieur sur l’objectif pour l’afficher</p>
  <p>Autorisations de gestion sur l’objectif pour le modifier</p>
  <p>Pour plus d’informations sur le partage des objectifs, consultez <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Partager un objectif dans les Objectifs Workfront</a>. </p>
  </div> </td>
 </tr>
 <tr>
   <td role="rowheader"><p>Modèle de disposition</p></td>
   <td> <p>Toutes les personnes, y compris les administrateurs et administratrices Workfront, doivent se voir attribuer un modèle de mise en page incluant la zone Objectifs dans le menu principal. </p>  
</td>
  </tr>
</tbody>
</table>

*Pour plus d’informations, voir [Conditions d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Gérer les objectifs dans la liste des objectifs

Vous pouvez afficher et gérer les objectifs dans les sections suivantes des Objectifs Workfront :

* Liste d’objectifs
* Alignement des objectifs

Chaque section affiche des objectifs dans des formats légèrement différents. La section que vous utilisez dépend de l’objectif que vous souhaitez atteindre lorsque vous travaillez avec des objectifs.

Pour plus d’informations, voir [Vue d’ensemble des sections sur les Objectifs Adobe Workfront](../../workfront-goals/goal-review-and-workfront-goals-sections/overview-of-wf-goals-sections.md).

Cet article décrit comment passer en revue les objectifs dans la liste des objectifs.

Tenez compte des points suivants lorsque vous passez en revue la liste des objectifs :

* Vous pouvez afficher les objectifs que vous ou toute autre personne de votre entreprise avez créés dans la liste des objectifs. Pour pouvoir modifier les objectifs, vous devez disposer des autorisations de gestion.

<!--

### Manage the Goal List in the Production environment

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner, then click **Goals**.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   The Goal List section displays by default. You can view goals regardless of their status, period, or owner, by default.

   The list of goals contains the following columns with information about each goal, result, or activity: 

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> 
       <div> 
        <p role="rowheader">Name </p> 
       </div> </td> 
      <td>The name of the goal, result, or activity.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Owner</td> 
      <td>The name of the goal, result, or activity owner. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Period</td> 
      <td>The time period for which the goal is scheduled.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Progress </td> 
      <td> <p>The progress indicator for the goal includes the following:</p> 
       <ul> 
      <li> <p>The progress label. </p> <p>For information, see <a href="../../workfront-goals/goal-management/calculate-goal-progress.md" class="MCXref xref">Overview of goal progress and condition in Adobe Workfront Goals</a>. </p> </li> 
      <li> <p>The percent complete of the goal, activity, or result. </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Status (includes alignment icon)</p> <p> <img src="assets/alignment-icon-large.png"> </p> </td> 
      <td> <p>The status of the goal which can be one of the following:</p> 
       <ul> 
        <li>Active</li> 
        <li>Draft</li> 
        <li>Inactive</li> 
        <li>Closed</li> 
       </ul> <p>For information about goal status, see <a href="../../workfront-goals/goal-management/goal-status-overview.md" class="MCXref xref">Goal status overview in Adobe Workfront Goals</a>. </p> <p>The alignment icon appears on goals that are aligned to other goals. For information about aligning goals, see <a href="../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md" class="MCXref xref">Align goals by connecting them in Adobe Workfront Goals</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Use the filters in the upper-right corner of the goal list to select only goals that are important to you. For information about using filters in Workfront Goals, see [Filter information in Adobe Workfront Goals](../../workfront-goals/goal-management/filter-information-wf-goals.md)
1. Click any of the fields in the column headers to sort it by that field.

   An arrow displays to the right of the field by which the list is sorted.

   ![](assets/goal-list-with-goal-expanded-+-result-+-activity-350x117.png)

1. (Optional) Click the field in the column again to sort the same column in a descending order. 
1. Click the right-pointing arrow to the left of the goal name to expand a goal

   Or

   Click the right-pointing arrow ![](assets/right-pointing-arrow.png) in the header of the list to expand all the goals in the list and view additional information about each goal, including any of the following:

   * Results names, owners, and progress

     For information about results, see [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md).
   
   * Activity names, owners, and progress

     For information about activities, see [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md).

1. Click the name of a goal to open the **Goal Details** panel on the right and review more information about the goal as well as manage it. For information about reviewing individual goals, see [Update goals in the Goal details section in Adobe Workfront Goals](../../workfront-goals/goal-management/update-goals-in-goal-details-panel.md).
1. (Optional) Expand the **Goals per page** drop-down menu and select from the following options to display additional goals:

   * 20  
      
      This is the default selection. 
   * 50
   * 100

1. Click **Print** to export a list of goals, results, and activities to a .pdf file.

   >[!TIP]
   >
   >* When printing a list of goals, the file produced contains only the information displayed on the screen. Items eliminated by filtering a list of goals do not display in the .pdf file.
   >* When you do not expand the goals in the list before printing the list, the .pdf file displays only goals without their results and activities.

   For more information, see [Print the Goal List in Adobe Workfront Goals](../../workfront-goals/goal-management/print-the-goal-list.md). 

1. Click the **Alignment icon** ![](assets/align-icon.png) next to an aligned to open the goal's card in the Goal Alignment section. For more information, see [Navigate the Goal Alignment section in Adobe Workfront Goals](../../workfront-goals/goal-alignment/navigate-goal-alignment-chart.md).
-->

Pour gérer les objectifs dans la liste des objectifs :

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit, puis cliquez sur **Objectifs**.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   La section Liste des objectifs s’affiche par défaut. Par défaut, vous pouvez afficher les objectifs, quel que soit leur statut, leur période ou leur propriétaire.

   La liste des objectifs contient les champs suivants avec des informations sur chaque objectif :

   * **Nom** : nom de l’objectif.
   * **Propriétaire** : nom de la personne propriétaire de l’objectif.
   * **Période** : période pour laquelle l’objectif est planifié.
   * **Statut** : le statut de l’objectif peut être l’un des suivants :
      * Actif
      * Brouillon
      * Inactif
      * Fermé

     Pour plus d’informations sur le statut des objectifs, consultez la section [Vue d’ensemble du statut des objectifs dans les Objectifs Adobe Workfront](../goal-management/goal-status-overview.md).

     L’icône d’alignement s’affiche sur les objectifs alignés sur d’autres objectifs. Pour plus d’informations sur l’alignement des objectifs, voir [Aligner des objectifs en les connectant dans les Objectifs Adobe Workfront](../goal-alignment/align-goals-by-connecting-them.md).

   * **Condition** : représentation visuelle de la progression de l’objectif au cours de la période allouée à l’objectif.

     La condition d’un objectif peut être l’une des suivantes :

      * Nouveau
      * Dans les temps
      * En danger
      * En difficulté

     Pour plus d’informations sur les conditions des objectifs, voir [Vue d’ensemble de la progression et de la condition des objectifs dans les Objectifs Adobe Workfront](../goal-management/calculate-goal-progress.md).

   * **Progression** : indicateur de progression de l’objectif sous forme de valeur en pourcentage. La couleur de l’indicateur de progression correspond à la couleur de la condition de l’objectif.

     Pour plus d’informations, voir [Calculer la progression de l’objectif dans les Objectifs Adobe Workfront](../goal-management/calculate-goal-progress.md).

1. Cliquez sur l’icône Filtrer ![](assets/filter-icon.png) dans le coin supérieur droit de la liste des objectifs et appliquez des filtres pour n’afficher que les objectifs qui vous semblent importants.

   Pour plus d’informations sur l’utilisation de filtres dans Objectifs Workfront, voir [Filtrer des informations dans les Objectifs Adobe Workfront](../goal-management/filter-information-wf-goals.md).

1. Cliquez sur l’un des champs des en-têtes de colonne pour trier la liste en fonction de ce champ.
Une flèche s’affiche à droite du champ par lequel la liste est triée.

1. (Facultatif) Cliquez de nouveau sur le champ de la colonne pour trier la même colonne par ordre décroissant.
1. Cliquez sur le nom d’un objectif pour ouvrir la page de l’objectif.
1. Sélectionnez un objectif dans la liste, puis cliquez sur l’une des options suivantes en haut de la liste :
   * Icône **Modifier** ![](assets/edit-icon.png) pour modifier des informations sur l’objectif. Pour plus d’informations, voir [Modifier les objectifs dans les Objectifs Adobe Workfront](../goal-management/edit-goals.md).
   * Icône **Partager** ![](assets/share-icon.png) pour partager l’objectif avec d’autres personnes. Pour plus d’informations, voir [Partager un objectif dans les Objectifs Adobe Workfront](../workfront-goals-settings/share-a-goal.md).
   * Icône **Ouvrir l’alignement** ![](assets/align-icon-unshimmed.png) pour ouvrir la zone Alignement de l’objectif. Cette option s’affiche uniquement lorsque l’objectif sélectionné est aligné sur un autre objectif.
   * Icône **Supprimer** ![](assets/delete-icon.png) pour supprimer l’objectif. Cliquez sur **Supprimer** pour confirmer.  Pour plus d’informations, voir la section [Supprimer et désactiver des objectifs dans les Objectifs Adobe Workfront](../goal-management/delete-and-deactivate-goals.md).





