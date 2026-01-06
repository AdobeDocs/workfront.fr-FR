---
product-previous: workfront-goals
navigation-topic: goal-management
title: Mettez à jour les objectifs dans la section Détails de l’objectif dans les objectifs Adobe Workfront
description: Vous pouvez mettre à jour les informations relatives à des objectifs individuels en accédant au panneau Détails sur l’objectif.
author: Alina
feature: Workfront Goals
exl-id: e9df0d98-05a1-4977-b7f1-426b8f5b3eae
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '576'
ht-degree: 84%

---

# Mettre à jour des objectifs dans la section Détails sur l’objectif d’Objectifs Adobe Workfront

<!--Audited for P&P only: 10/2025-->

Vous pouvez mettre à jour les informations relatives à des objectifs individuels en accédant au panneau Détails sur l’objectif.

>[!NOTE]
>
>Vous ne pouvez pas mettre à jour les objectifs dont le statut est Fermé.

## Conditions d’accès

>[!NOTE]
>
>Votre entreprise peut choisir de continuer à utiliser les objectifs Adobe Workfront si elle a déjà acheté ce package par le passé. Pour plus de détails, contactez votre représentant de compte.
>
>Adobe Workfront Goals ne peut plus être acheté.

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article. 

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr>
  <td> <p>Package Adobe Workfront</p> </td> 
   <td> 
   <p>Adobe Workfront Ultimate</p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Licence Adobe Workfront</td>
 <td>
 <p>Contributeur ou version ultérieure</p>
<p>Requête ou supérieure</p></td>
 </tr>
  <tr>
 <td role="rowheader">Configuration du niveau d’accès</td>
 <td> <p>Modifier l’accès aux Objectifs</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Autorisations d’objet</td>
 <td>
  <div>
  <p>Autorisations d’affichage ou de niveau supérieur sur l’objectif pour l’afficher</p>
  <p>Autorisations de gestion sur l’objectif pour le modifier</p>
  </div> </td>
 </tr>
<tr>
   <td role="rowheader"><p>Modèle de mise en page</p></td>
   <td> <p>Un modèle de mise en page comprenant la zone Objectifs du menu principal doit être affecté à tous les utilisateurs, y compris les administrateurs système. </p>  
</td>
  </tr>
</tbody>
</table>

Pour plus d’informations, voir [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> 
   <p>For the new plan and license structure:
  <ul><li>An Ultimate plan </li></ul>
   </p>
<p>For the current plan and license structure: 
<ul><li> A Pro or higher </li>
  <li>An Adobe Workfront Goals license in addition to a Workfront license.</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront license*</td>
 <td>
 <p>New license: Contributor or higher</p>
 Or
 <p>Current license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Product*</td>
 <td>
  <p> New product requirement: Workfront</p>
  Or
  <p>Current product requirement: In addition to a Workfront license, you must purchase a license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Access level*</td>
 <td> <p>Edit access to Goals</p> </td>
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
 <tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Goals area in the Main Menu. </p>  
</td>
  </tr>
</tbody>
</table>-->

## Mettre à jour des objectifs dans la section Détails sur l’objectif

Vous pouvez accéder à un objectif individuel à partir d’une liste d’objectifs.

<!--

Updating goals in the Goal Details panel differs depending on where you access the goal from. 

### Update goals in the Goal Details panel in the Production environment

1. Click the **Main Menu** icon ![Main Menu icon](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   This opens the Goals area in Workfront. 

1. Click the name of a goal in the Goal List, then click the name of a goal.

   This opens the Goal Details panel on the right.
   ![Goal details summary](assets/goal-details-summary-tab-350x294.png)

   >[!TIP]
   >
   >You can also click the name of a goal in the Goal Alignment, Check-in, or Pulse sections. 
   >
   ><!-- drafted for goal redesign:
   >Add this to the TIP above with goal redesign: 
   >
   >The Check-in and Pulse sections have been removed from the Preview environment.
   >

1. On the Summary tab, click the **More icon** ![More icon](assets/more-icon.png), then click any of the following options:

   1. **Edit**. For information about editing goals, see [Edit goals in Adobe Workfront Goals](../../workfront-goals/goal-management/edit-goals.md).
   1. **Copy**. For information about copying goals, see [Copy goals in Adobe Workfront Goals](../../workfront-goals/goal-management/copy-goals.md).
   1. **Activate**. This option is available only for drafted and inactive goals.

      For information about activating goals, see [Access and open goals in Adobe Workfront Goals](../../workfront-goals/goal-management/access-goals-in-wf-goals.md). 
   
   1. **Close**, then click**Close Goal**. This option is available only for active goals.

      For information about closing goals, see [Close and reopen goals in Adobe Workfront Goals](../../workfront-goals/goal-management/close-and-reopen-goals.md). 
   
   1. **Deactivate**. This option is available only for active goals. This deactivates the goal immediately.

      For information about deactivating goals, see [Delete and deactivate goals in Adobe Workfront Goals](../../workfront-goals/goal-management/delete-and-deactivate-goals.md).
   
   1. **Delete**, then click **Yes, Delete**.

      For information about deleting goals, see [Delete and deactivate goals in Adobe Workfront Goals](../../workfront-goals/goal-management/delete-and-deactivate-goals.md).

      >[!NOTE]
      >
      >Deleted goals cannot be recovered.

   1. **Reopen**, then click **Reopen**. This option is available only for closed goals that are from a current time period.

      For information about reopening goals, see [Close and reopen goals in Adobe Workfront Goals](../../workfront-goals/goal-management/close-and-reopen-goals.md). 
   
   1. (Conditional) If you clicked any of the options between steps a-i above except Delete or Reopen, click **Save**.    
   
      (!--ensure this is accurate)--)

1. Click **Align to another goal** in the upper-right of the Summary tab, then specify the name of a goal in the **Align to** **another goal** field that you want to align the current goal to. The current goal becomes the child of the goal you align it to. For information about child and parent goals, see [Align goals by connecting them in Adobe Workfront Goals](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md). 
1. Click **Add results**. Results drive the progress of your goal. For information about adding results, see [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md).

1. Click **Add activities**. Activities drive the progress of your goal. For information about adding activities, see [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md). 

1. Click the **Updates** tab. Here, you can view goal comments and review the entire editing history of the goal, activities, and results, to understand who changed what and when.

   ![Goal details updates](assets/goal-details-updates-tab-350x280.png)

1. (Optional) Deselect any of the following options if you want to not display them in the Updates tab. They are selected by default: 

   | Option |Description  |
   |---|---|
   | Progress Updates |Displays information about the history of progress updates on results and activities.  |
   | Comments |Displays comments made by users on the goal.  |
   | Editing History |Displays information about creating and updating the goal, results, and activities.  |

1. (Optional) Click **Details** under a progress or an editing history update to display additional information about the update.

   ![Details in update tab](assets/update-details-in-updates-tab-expanded-highlighted-350x139.png)

-->



1. Cliquez sur le nom d’un objectif dans la liste des objectifs, puis sur le nom d’un objectif.

   Cela ouvre la section **Détails sur l’objectif** sur la gauche.

   ![Page d’objectif](assets/goal-page-unshimmed.png)

1. Cliquez sur l’icône **Modifier** ![Modifier](assets/edit-icon.png) dans le coin supérieur droit, puis cliquez sur **Modifier tout** ou **Aperçu**

   Ou

   Commencez à saisir des informations dans l’un des champs modifiables de la section Détails sur l’objectif. La section devient modifiable.

   >[!IMPORTANT]
   >
   >Tous les champs qui s’affichent dans la section Détails sur l’objectif ne peuvent pas être modifiés. Workfront calcule certains champs et ceux-ci sont en lecture seule.

1. Mettez à jour ou vérifiez les champs suivants :

   * **Description** : ajoutez ou mettez à jour des informations sur l’objectif.
   * **Progression** : indique le pourcentage de l’objectif atteint jusqu’à présent. Vous ne pouvez pas mettre à jour manuellement la progression d’un objectif. La progression de l’objectif est le calcul de tous les indicateurs de progression.
   * **Condition** : indique si l’objectif est nouveau et n’a pas encore été mis à jour, s’il est dans les temps ou s’il est en retard. Vous ne pouvez pas mettre à jour la condition d’un objectif. La condition de l’objectif est automatiquement calculée par Workfront.\
     Pour plus d’informations sur la condition et la progression de l’objectif, voir
     [Vue d’ensemble de la progression et de la condition des objectifs d’Objectifs Adobe Workfront](../goal-management/calculate-goal-progress.md).
   * **Statut** : vous ne pouvez pas mettre à jour manuellement le statut d’un objectif. Pour plus d’informations, voir [Vue d’ensemble des statuts des objectifs dans Objectifs Adobe Workfront](../goal-management/goal-status-overview.md).
   * **Personne propriétaire de l’objectif** : cliquez dessus pour mettre à jour le nom de la personne propriétaire de l’objectif. Commencez à saisir le nom d’une personne, d’une équipe, d’un groupe ou du nom de votre organisation, puis sélectionnez-le lorsqu’il s’affiche dans la liste. Vous ne pouvez avoir qu’une seule personne propriétaire pour un objectif.
   * **Objectif parent** : commencez à saisir le nom d’un objectif que vous souhaitez définir comme parent de l’objectif que vous avez sélectionné. La progression de l’objectif sélectionné met automatiquement à jour la progression de l’objectif parent.

     >[!TIP]
     >
     >Vous ne pouvez pas mettre à jour les informations suivantes sur un objectif parent :
     >    * Période de l’objectif parent
     >    * Progression de l’objectif parent
     >    * Personne propriétaire de l’objectif parent.
     >      
     >Vous devez mettre à jour ces informations sur l’objectif parent lui-même.

   * **Période** : cliquez pour mettre à jour la période de l’objectif.\
     Ou\
     Sélectionnez **Activer des dates personnalisées** pour indiquer les dates de **Début** et de **Fin** de l’objectif.
   * **Notes finales** : ce champ n’est visible que pour les objectifs dont le statut est Fermé. Les objectifs fermés ne peuvent pas être modifiés. La réouverture d’un objectif fermé supprime définitivement les notes finales.


