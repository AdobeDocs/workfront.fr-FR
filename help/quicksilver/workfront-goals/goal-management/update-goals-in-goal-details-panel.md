---
product-previous: workfront-goals
navigation-topic: goal-management
title: Mise à jour des objectifs dans le panneau Détails de l’objectif dans les objectifs Adobe Workfront
description: Vous pouvez mettre à jour les informations relatives à des objectifs individuels en accédant au panneau Détails de l’objectif .
author: Alina
feature: Workfront Goals
exl-id: e9df0d98-05a1-4977-b7f1-426b8f5b3eae
source-git-commit: 024c612d46848c55529e902a00d481588d261584
workflow-type: tm+mt
source-wordcount: '654'
ht-degree: 9%

---

# Mettre à jour des objectifs dans la section Détails de l’objectif dans Objectifs Adobe Workfront

<!--drafted for the goal redesign:
- change the title for Production to Update goals in the Goal details section in Adobe Workfront Goals. 
- update the description in the metadata above
-->

Vous pouvez mettre à jour les informations relatives à des objectifs individuels en accédant au panneau Détails de l’objectif .

>[!NOTE]
>
>Vous ne pouvez pas mettre à jour les objectifs dont l’état est Fermé.


## Conditions d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td> 
   <p>Pour le nouveau plan et la nouvelle structure de licence :
  <ul><li>Un plan ultime </li>
  Ou
  <li>Une licence supplémentaire pour les objectifs Adobe Workfront pour les plans Prime ou Select Adobe Workfront. </li></ul> </p>
<p>Pour le plan actuel et la structure de licence : 
<ul><li> A Pro ou version ultérieure </li>
  <li>Une licence Adobe Workfront Goals en plus d’une licence Workfront.</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Licence Adobe Workfront*</td>
 <td>
 <p>Nouvelle licence : contributeur ou contributrice ou supérieure</p>
 Ou
 <p>Licence actuelle : demande ou supérieure</p> <p>Pour plus d’informations, voir <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Présentation des licences Adobe Workfront</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Produit*</td>
 <td>
 <p> Nouvelle exigence de produit, l’une des options suivantes : </p>
<ul>
<li>Un forfait Select ou Prime Adobe Workfront et une licence Adobe Workfront Goals supplémentaire.</li>
<li>Un plan Workfront Ultimate qui inclut par défaut les objectifs de Workfront. </li></ul>
 <p>Ou</p>
 <p>Exigences actuelles du produit : formule Workfront et licence supplémentaire pour les objectifs Adobe Workfront. </p> <p>Pour plus d’informations, consultez la section <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Exigences pour l’utilisation des Objectifs Workfront</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Niveau d’accès*</td>
 <td> <p>Modifier l’accès aux objectifs</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Autorisations d’objet</td>
 <td>
  <div>
  <p>Afficher ou des autorisations supérieures à l’objectif pour l’afficher</p>
  <p>Gérer les autorisations sur l’objectif pour le modifier</p>
  <p>Pour plus d’informations sur le partage des objectifs, consultez <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Partager un objectif dans les Objectifs Workfront</a>. </p>
  </div> </td>
 </tr>
 <tr>
   <td role="rowheader"><p>Modèle de mise en page</p></td>
   <td> <p>Tous les utilisateurs, y compris les administrateurs de Workfront, doivent se voir attribuer un modèle de mise en page incluant la zone Objectifs dans le menu principal. </p>  
</td>
  </tr>
</tbody>
</table>

*Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Mise à jour des objectifs dans la section Détails des objectifs

Vous pouvez accéder à un objectif individuel à partir d’une liste d’objectifs.

<!--

Updating goals in the Goal Details panel differs depending on where you access the goal from. 

### Update goals in the Goal Details panel in the Production environment

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   This opens the Goals area in Workfront. 

1. Click the name of a goal in the Goal List, then click the name of a goal.

   This opens the Goal Details panel on the right.
   ![](assets/goal-details-summary-tab-350x294.png)

   >[!TIP]
   >
   >You can also click the name of a goal in the Goal Alignment, Check-in, or Pulse sections. 
   >
   ><!-- drafted for goal redesign:
   >Add this to the TIP above with goal redesign: 
   >
   >The Check-in and Pulse sections have been removed from the Preview environment.
   >

1. On the Summary tab, click the **More icon** ![](assets/more-icon.png), then click any of the following options:

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

   ![](assets/goal-details-updates-tab-350x280.png)

1. (Optional) Deselect any of the following options if you want to not display them in the Updates tab.&nbsp;They are selected by default: 

   | Option |Description  |
   |---|---|
   | Progress Updates |Displays information about the history of progress updates on results and activities.  |
   | Comments |Displays comments made by users on the goal.  |
   | Editing History |Displays information about creating and updating the goal, results, and activities.  |

1. (Optional) Click **Details** under a progress or an editing history update to display additional information about the update.

   ![](assets/update-details-in-updates-tab-expanded-highlighted-350x139.png)

-->



1. Cliquez sur le nom d’un objectif dans la liste des objectifs, puis sur le nom d’un objectif.

   Cela ouvre la fenêtre **Détails de l’objectif** sur la gauche.

   ![](assets/goal-page-unshimmed.png)

1. Cliquez sur le bouton **Icône Modifier** ![](assets/edit-icon.png) dans le coin supérieur droit, puis cliquez sur **Tout modifier** ou **Présentation**

   Ou

   Commencez à saisir des informations dans l’un des champs modifiables de la section Détails de l’objectif . La section devient modifiable.

   >[!IMPORTANT]
   >
   >Tous les champs qui s’affichent dans la section Détails de l’objectif ne peuvent pas être modifiés. Workfront calcule certains champs et ils sont en lecture seule.

1. Mettez à jour ou consultez les champs suivants :

   * **Description**: ajoutez ou mettez à jour des informations sur l’objectif.
   * **Progression**: indique le pourcentage de l’objectif atteint jusqu’à présent. Vous ne pouvez pas mettre à jour manuellement la progression d’un objectif. Le progrès de l&#39;objectif est le calcul de tous les indicateurs de progrès.
   * **Condition**: indique si l’objectif est nouveau et n’a pas encore été mis à jour, s’il est sur la cible d’être terminé à temps ou s’il est en retard. Vous ne pouvez pas mettre à jour la condition d’un objectif. La condition de l’objectif est automatiquement calculée par Worfront.\
     Pour plus d’informations sur la condition et la progression de l’objectif, voir
     [Présentation de la progression et de la condition des objectifs dans les objectifs Adobe Workfront](../goal-management/calculate-goal-progress.md).
   * **État**: vous ne pouvez pas mettre à jour manuellement l’état d’un objectif. Pour plus d’informations, voir [Présentation de l’état des objectifs dans les objectifs Adobe Workfront](../goal-management/goal-status-overview.md).
   * **Propriétaire de l’objectif**: cliquez sur pour mettre à jour le nom du propriétaire de l’objectif. Commencez à saisir le nom d’un utilisateur, d’une équipe, d’un groupe ou du nom de votre organisation, puis sélectionnez-le lorsqu’il s’affiche dans la liste. Vous ne pouvez avoir qu&#39;un seul propriétaire pour un objectif.
   * **Objectif parent**: commencez à saisir le nom d’un objectif que vous souhaitez définir comme parent de l’objectif que vous avez sélectionné. La progression de l’objectif sélectionné met automatiquement à jour la progression de l’objectif parent.

     >[!TIP]
     >
     >Vous ne pouvez pas mettre à jour les informations suivantes sur un objectif parent :
     >    * Période de l’objectif parent
     >    * Progression de l’objectif parent
     >    * Propriétaire de l’objectif parent.
     >      
     >Vous devez mettre à jour ces informations sur l’objectif parent lui-même.

   * **Période**: cliquez sur pour mettre à jour la période de l’objectif.\
     Ou\
     Sélectionner **Activation des dates personnalisées** pour spécifier des dates pour le **Début** et **Dates de fin**.
   * **Notes de fermeture**: ce champ n’est visible que pour les objectifs dont l’état est Fermé. Les objectifs fermés ne peuvent pas être modifiés. La réouverture d’un objectif fermé supprime définitivement les notes de fin.


