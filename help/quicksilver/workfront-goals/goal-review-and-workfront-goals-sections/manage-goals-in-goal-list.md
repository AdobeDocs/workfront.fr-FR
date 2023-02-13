---
product-previous: workfront-goals
navigation-topic: goal-review-and-sections
title: Gestion des objectifs dans la liste des objectifs d’Adobe Workfront
description: Une fois que vous ou d’autres utilisateurs avez créé des objectifs, vous pouvez consulter leur progression et leurs informations dans la liste des objectifs. Pour plus d’informations sur la création d’objectifs, voir Création d’objectifs dans les objectifs Adobe Workfront.
author: Alina
feature: Workfront Goals
exl-id: 2a2c1240-f796-4cb8-b8a6-2ad5853916b9
source-git-commit: afc2124a7fd0d9d52c04be1c174fdba314beec7a
workflow-type: tm+mt
source-wordcount: '779'
ht-degree: 2%

---

# Gestion des objectifs dans la liste des objectifs d’Adobe Workfront

<!-- printing or exporting goals is no longer possible, but see if they add it later-->

Une fois que vous ou d’autres utilisateurs avez créé des objectifs, vous pouvez consulter leur progression et leurs informations dans la liste des objectifs. Pour plus d’informations sur la création d’objectifs, voir [Création d’objectifs dans les objectifs Adobe Workfront](../../workfront-goals/goal-management/create-goals.md).

## Exigences d’accès

<!--drafted - replace the table below with this one when P&P releases: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
  <tr>
   <td role="rowheader">Adobe Workfront plan*</td>
   <td>
   <p>Current plan: Select or higher</p>
   Or
   <p>Legacy plan: Pro or higher</p>
   
   </td>
  </tr>
  <tr>
   <td role="rowheader">Adobe Workfront license*</td>
   <td>
   <p>Current license: Contributor or higher</p>
   Or
   <p>Legacy license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
  </tr>
  <tr>
   <td role="rowheader">Product</td>
   <td>
   <p> Current product requirement: If you have the Select or Prime Adobe Workfront plan, you must also buy an additional Adobe Workfront Goals license.  Workfront Goals are included in the Ultimate Workfront Plan.</p>
   Or
   <p>Legacy product requirement: You must purchase an additional license for the Adobe Workfront Goals to access functionality described in this article. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
  </tr>
  <tr>
   <td role="rowheader">Access level*</td>
   <td> <p>Edit access to Goals</p> <p><b>NOTE</b><p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see:</p>
     <ul>
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a> </p> </li>
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Grant access to Adobe Workfront Goals</a></span> </p> </li>
     </ul> </p> </td>
  </tr>
  <tr data-mc-conditions="">
   <td role="rowheader">Object permissions</td>
   <td>
    <div>
     <p>View or higher permissions to the goal to view it</p>
     <p>Manage permissions to the goal to edit it</p>
     <p>For information about sharing goals, see <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Workfront Goals</a>. </p>
    </div> </td>
  </tr>
 </tbody>
</table>
-->

Vous devez disposer des accès suivants pour effectuer les actions décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Pro ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Requête ou supérieure</p> <p>Pour plus d’informations, voir <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Présentation des licences Adobe Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td> <p>Pour accéder aux fonctionnalités décrites dans cet article, vous devez acheter une licence supplémentaire pour les objectifs d’Adobe Workfront. </p> <p>Pour plus d’informations, voir <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Conditions requises pour utiliser les objectifs Workfront</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Niveau d’accès*</td> 
   <td> <p>Affichage ou accès supérieur aux objectifs</p> <p><b>NOTE</b><p>Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir :</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Accorder l’accès aux objectifs Adobe Workfront</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> 
    <div> 
     <p>Affichage ou autorisations supérieures sur les objectifs</p> 
     <p>Pour plus d’informations sur le partage des objectifs, voir <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Partage d’un objectif dans les objectifs Workfront</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

*Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Conditions préalables

Avant de pouvoir commencer, vous devez disposer des éléments suivants :

* Un modèle de mise en page qui inclut la zone Objectifs dans le menu principal.

## Gestion des objectifs dans la liste des objectifs

Vous pouvez afficher et gérer les objectifs dans les sections suivantes des objectifs de Workfront :

* Liste d’objectifs
* Alignement des objectifs

Chaque section affiche des objectifs dans des formats légèrement différents. La section que vous utilisez dépend de l’objectif que vous souhaitez atteindre lorsque vous travaillez avec des objectifs.

Pour plus d’informations, voir [Présentation des sections Objectifs d’Adobe Workfront](../../workfront-goals/goal-review-and-workfront-goals-sections/overview-of-wf-goals-sections.md).

Cet article décrit comment passer en revue les objectifs dans la liste des objectifs.

Tenez compte des points suivants lors de la révision de la liste des objectifs :

* Vous pouvez afficher les objectifs que vous ou toute autre personne de votre entreprise avez créés dans la liste des objectifs. Pour pouvoir les modifier, vous devez disposer des autorisations Gérer sur les objectifs.

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

Pour gérer les objectifs dans la liste des objectifs :

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png)  dans le coin supérieur droit, puis cliquez sur **Objectifs**.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   La section Liste des objectifs s’affiche par défaut. Par défaut, vous pouvez afficher les objectifs, quel que soit leur statut, point ou propriétaire.

   La liste des objectifs contient les champs suivants avec des informations sur chaque objectif :

   * **Nom**: Nom de l’objectif.
   * **Propriétaire**: Nom du propriétaire de l’objectif.
   * **Période**: Période pour laquelle l’objectif est planifié.
   * **État**: L’état de l’objectif peut être l’un des suivants :
      * Actif
      * Brouillon
      * Inactif
      * Fermé

      Pour plus d’informations sur l’état de l’objectif, voir [Présentation de l’état des objectifs dans les objectifs Adobe Workfront](../goal-management/goal-status-overview.md).

      L’icône d’alignement s’affiche sur les objectifs alignés sur d’autres objectifs. Pour plus d’informations sur l’alignement des objectifs, voir [Alignement des objectifs en les connectant aux objectifs Adobe Workfront](../goal-alignment/align-goals-by-connecting-them.md).

   * **Condition**: Une représentation visuelle de la progression de l’objectif au cours de la période allouée à l’atteinte de l’objectif.

      La condition d’un objectif peut être l’une des suivantes :

      * Nouveau
      * Dans les temps
      * En danger
      * En difficulté

      Pour plus d’informations sur les conditions d’objectif, voir [Présentation de la progression et de la condition des objectifs dans les objectifs Adobe Workfront](../goal-management/calculate-goal-progress.md).

   * **Progression**: Indicateur de progression de l’objectif sous forme de valeur en pourcentage. La couleur de l’indicateur de progression correspond à la couleur de la condition de l’objectif.

      Pour plus d’informations, voir [Calculer la progression de l’objectif dans les objectifs Adobe Workfront](../goal-management/calculate-goal-progress.md).



1. Cliquez sur l’icône Filtrer ![](assets/filter-icon.png) dans le coin supérieur droit de la liste des objectifs et appliquez des filtres pour n’afficher que les objectifs importants pour vous.

   Pour plus d’informations sur l’utilisation de filtres dans les objectifs Workfront, voir [Filtrage des informations dans les objectifs Adobe Workfront](../goal-management/filter-information-wf-goals.md).

1. Cliquez sur l’un des champs des en-têtes de colonne pour trier la liste en fonction de ce champ.
Une flèche s’affiche à droite du champ de tri de la liste.

1. (Facultatif) Cliquez de nouveau sur le champ de la colonne pour trier la même colonne dans un ordre décroissant.
1. Cliquez sur le nom d’un objectif pour ouvrir la page de l’objectif.
1. Sélectionnez un objectif dans la liste, puis cliquez sur l’une des options suivantes en haut de la liste :
   * **Modifier** icon ![](assets/edit-icon.png) pour modifier des informations sur l’objectif. Pour plus d’informations, voir [Modifier les objectifs dans les objectifs Adobe Workfront](../goal-management/edit-goals.md).
   * **Partager** icon ![](assets/share-icon.png) partager le but avec d&#39;autres personnes. Pour plus d’informations, voir [Partage d’un objectif dans les objectifs Adobe Workfront](../workfront-goals-settings/share-a-goal.md).
   * **Alignement des ouvertures** icon ![](assets/align-icon-unshimmed.png) pour ouvrir la zone Alignement de l’objectif . Cette option s’affiche uniquement lorsque l’objectif sélectionné est aligné sur un autre objectif.
   * **Supprimer** icon ![](assets/delete-icon.png) pour supprimer l’objectif, puis cliquez sur **Supprimer** pour confirmer.  Pour plus d’informations, voir [Suppression et désactivation d’objectifs dans les objectifs Adobe Workfront](../goal-management/delete-and-deactivate-goals.md).





