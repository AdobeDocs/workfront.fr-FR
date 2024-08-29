---
product-previous: workfront-goals
navigation-topic: goal-management
title: Mettre à jour des objectifs dans le panneau Détails sur l’objectif dans Objectifs Adobe Workfront
description: Vous pouvez mettre à jour les informations relatives à des objectifs individuels en accédant au panneau Détails sur l’objectif.
author: Alina
feature: Workfront Goals
exl-id: e9df0d98-05a1-4977-b7f1-426b8f5b3eae
source-git-commit: d7dd5ab4e3041a100b13c5bf169747f58db0ea39
workflow-type: tm+mt
source-wordcount: '638'
ht-degree: 100%

---

# Mettre à jour des objectifs dans la section Détails de l’objectif dans Objectifs Adobe Workfront

<!--drafted for the goal redesign:
- change the title for Production to Update goals in the Goal details section in Adobe Workfront Goals. 
- update the description in the metadata above
-->

Vous pouvez mettre à jour les informations relatives à des objectifs individuels en accédant au panneau Détails sur l’objectif.

>[!NOTE]
>
>Vous ne pouvez pas mettre à jour les objectifs dont le statut est Fermé.


## Conditions d’accès

Vous devez disposer des éléments suivants :

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
 <td role="rowheader">Niveau d’accès*</td>
 <td> <p>Modifier l’accès aux Objectifs</p> </td>
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

## Mettre à jour des objectifs dans la section Détails sur l’objectif

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

   Cela ouvre la section **Détails sur l’objectif** sur la gauche.

   ![](assets/goal-page-unshimmed.png)

1. Cliquez sur l’**icône Modifier** ![](assets/edit-icon.png) dans le coin supérieur droit, puis sur **Tout modifier** ou **Vue d’ensemble**.

   Ou

   Commencez à saisir des informations dans l’un des champs modifiables de la section Détails sur l’objectif. La section devient modifiable.

   >[!IMPORTANT]
   >
   >Tous les champs qui s’affichent dans la section Détails sur l’objectif ne peuvent pas être modifiés. Workfront calcule certains champs et ceux-ci sont en lecture seule.

1. Mettez à jour ou vérifiez les champs suivants :

   * **Description** : ajoutez ou mettez à jour des informations sur l’objectif.
   * **Progression** : indique le pourcentage de l’objectif atteint jusqu’à présent. Vous ne pouvez pas mettre à jour manuellement la progression d’un objectif. La progression de l’objectif est le calcul de tous les indicateurs de progression.
   * **Condition** : indique si l’objectif est nouveau et n’a pas encore été mis à jour, s’il est sur le point d’être terminé à temps ou s’il est en retard. Vous ne pouvez pas mettre à jour la condition d’un objectif. La condition de l’objectif est automatiquement calculée par Workfront.\
     Pour plus d’informations sur la condition et la progression de l’objectif, voir
     [Vue d’ensemble de la progression et de la condition des objectifs dans Objectifs Adobe Workfront](../goal-management/calculate-goal-progress.md).
   * **Statut** : vous ne pouvez pas mettre à jour manuellement le statut d’un objectif. Pour plus d’informations, voir [Vue d’ensemble des statuts des objectifs dans Objectifs Adobe Workfront](../goal-management/goal-status-overview.md).
   * **Personne propriétaire de l’objectif** : cliquez pour mettre à jour le nom de la personne propriétaire de l’objectif. Commencez à saisir le nom d’une personne, d’une équipe, d’un groupe ou le nom de votre organisation, puis sélectionnez-le lorsqu’il s’affiche dans la liste. Vous ne pouvez avoir qu’une seule personne propriétaire pour un objectif.
   * **Objectif parent** : commencez à saisir le nom d’un objectif que vous souhaitez définir comme parent de l’objectif que vous avez sélectionné. La progression de l’objectif sélectionné met automatiquement à jour la progression de l’objectif parent.

     >[!TIP]
     >
     >Vous ne pouvez pas mettre à jour les informations suivantes sur un objectif parent :
     >    * Période de l’objectif parent
     >    * Progression de l’objectif parent
     >    * Personne propriétaire de l’objectif parent
     >      
     >Vous devez mettre à jour ces informations sur l’objectif parent lui-même.

   * **Période** : cliquez pour mettre à jour la période de l’objectif.\
     Ou\
     Sélectionnez **Activer les dates personnalisées** pour indiquer les dates de **Début** et de **Fin** de l’objectif.
   * **Notes finales** : ce champ n’est visible que pour les objectifs dont le statut est Fermé. Les objectifs fermés ne peuvent pas être modifiés. La réouverture d’un objectif fermé supprime définitivement les notes finales.


