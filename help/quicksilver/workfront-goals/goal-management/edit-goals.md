---
product-previous: workfront-goals
navigation-topic: goal-management
title: Modifier les objectifs dans Adobe Workfront Objectifs
description: Vous pouvez modifier les objectifs existants de n’importe quelle période et dans n’importe quel statut.
author: Alina
feature: Workfront Goals
exl-id: 74db534c-6897-40c2-bea9-a9d30a40f61c
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '563'
ht-degree: 80%

---

# Modifier des objectifs dans Objectifs Adobe Workfront

<!--Audited for P&P only: 10/2025-->

Vous pouvez modifier les objectifs existants de n’importe quelle période et dans n’importe quel statut.

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
 <p>Or</p>
  <p>Current product requirement: In addition to a Workfront license, you must purchase a license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Access level</td>
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

## Considérations sur la modification des objectifs

* Vous ne pouvez pas modifier les objectifs dont le statut est Clos.
* Vous pouvez modifier les objectifs de n’importe quelle période.

  Vous pouvez modifier les informations suivantes pour un objectif passé :

   * Nom
   * Période
   * Statut

     >[!TIP]
     >
     >Si l’objectif est Clos, sa réouverture recalcule le pourcentage d’avancement. Vous ne pouvez pas modifier un objectif clos.

   * Description
   * Résultats et activités

## Modifier des objectifs

<!--
Editing goals differs depending on what environment you use.

### Edit goals in the Production environment

1. Go to a goal that you want to edit and click the goal name to open the **Goal Details** panel. 
1. Click the **More icon** ![More icon](assets/more-icon.png), then click **Edit**.

   ![Edit goal](assets/edit-goal-highlighted.png)

1. Update the name of the goal in the **Goal** field. 
1. Select a time period when the goal should be completed.

   Select from the following predefined options:

   * The current year
   * The quarters of the current year
   * The next two years
   * The quarters of the next two years

   Or

   Click **Define custom dates** to select a custom time frame. 

1. (Conditional) Select a start and an end date for your goal, if you clicked **Define custom dates**.

   
   <p>(NOTE: these fields don't yet have a name) </p>
   

   >[!CAUTION]
   >
   >You cannot create a goal with custom dates in the past.

1. (Optional) Click **Reset custom dates** to return to the predefined options.

   >[!TIP]
   >
   >We recommend that everyone in your organization selects the same time frames for similar goals or goals that are aligned. This provides better alignment between goals and ensures that everyone's work supports your larger organization-wide strategy.

1. Click the **Owner** field and select a new owner for the goal, if you want to indicate someone else as the owner of the goal. 
1. (Conditional) Start typing the name of a user, team, group, or the name of your organization in the **Owner** field, then select it when it displays in the list. You can have only one owner for a goal. 
1. Update the **Description** of the goal, then click **Save**.

-->

{{step1-to-goals}}

Une liste d’objectifs s’affiche.

1. Cliquez sur un objectif.\
   La page de l’objectif s’affiche.

   ![Page d’objectif](assets/goal-page-unshimmed.png)

1. Effectuez l’une des opérations suivantes pour modifier les informations relatives à l’objectif :
   * Cliquez sur les champs qui s’affichent dans l’en-tête de l’objectif pour les mettre à jour. Tous les champs de l’en-tête ne sont pas modifiables.
   * Cliquez sur l’icône **Plus** ![Plus](assets/more-icon.png) à droite du nom de l’objectif, puis cliquez sur **Modifier**.
   * Cliquez sur **Détails de l’objectif** dans le panneau de gauche, puis cliquez sur l’icône **Modifier** ![Modifier](assets/edit-icon.png) dans le coin supérieur droit, puis cliquez sur **Tout modifier**. Commencez à mettre à jour les champs de la section Détails sur l’objectif.

     >[!IMPORTANT]
     >
     >Les champs qui s’affichent dans les zones mentionnées ci-dessus ne sont pas tous modifiables. Workfront calcule certains champs et ceux-ci sont en lecture seule.

1. (Le cas échéant) En fonction de ce que vous avez sélectionné à l’étape précédente, mettez à jour les informations suivantes sur l’objectif :

   * Mettez à jour les informations suivantes dans l’en-tête de l’objectif, puis appuyez sur Entrée pour enregistrer vos modifications :
      * **Nom de l’objectif** : cliquez sur le nom de l’objectif et commencez à saisir un nouveau nom.
      * **Personne propriétaire** : cliquez sur le nom de la personne propriétaire et commencez à taper le nom d’une personne, d’une équipe, d’un groupe ou de votre entreprise, puis sélectionnez-le lorsqu’il s’affiche dans la liste. Vous ne pouvez avoir qu’une seule personne propriétaire pour un objectif.
   * Mettez à jour les informations suivantes dans la case Modifier l’objectif, puis cliquez sur **Enregistrer** :
      * **Nom de l’objectif**
      * **Période** : cliquez pour mettre à jour la période de l’objectif.\
        Ou\
        Sélectionnez **Activer des dates personnalisées** pour indiquer les dates de **Début** et de **Fin** de l’objectif.

        >[!TIP]
        >
        >Désélectionnez **Activer les dates personnalisées** pour revenir à la période originale de l’objectif.

      * **Personne propriétaire de l’objectif**
      * **Description** : ajoutez ou mettez à jour des informations sur l’objectif.
   * Mettez à jour ou révisez les informations dans la section Détails sur l’objectif. Pour plus d’informations, voir [Mettre à jour les objectifs dans la section Détails sur l’objectif dans Objectifs Adobe Workfront](../goal-management/update-goals-in-goal-details-panel.md).

   <!-- (should you update the title here after changing it at production??? - change it to Update goals in the goal Details section)-->

1. (Facultatif) Cliquez sur **Indicateurs de progression** dans le panneau de gauche pour ajouter des résultats, des activités ou des projets à l’objectif. En ajoutant des indicateurs de progression, vous vous assurez de pouvoir suivre l’évolution de l’objectif.
Pour plus d’informations, consultez les articles suivants :
   * [Ajouter des activités aux objectifs dans Objectifs Adobe Workfront](../results-and-activities/add-activities-to-goals.md)
   * [Ajoutez des résultats aux objectifs dans Objectifs Adobe Workfront](../results-and-activities/add-results-to-goals.md).
   * [Ajoutez des projets aux objectifs dans Objectifs Adobe Workfront](../results-and-activities/connect-projects-to-goals-overview.md).

</div>
