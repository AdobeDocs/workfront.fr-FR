---
product-previous: workfront-goals
navigation-topic: goal-management
title: Modifier les objectifs dans les objectifs Adobe Workfront
description: Vous pouvez modifier des objectifs existants à partir de n’importe quelle période et dans n’importe quel état.
author: Alina
feature: Workfront Goals
exl-id: 74db534c-6897-40c2-bea9-a9d30a40f61c
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 1%

---

# Modifier les objectifs dans les objectifs Adobe Workfront

Vous pouvez modifier des objectifs existants à partir de n’importe quelle période et dans n’importe quel état.

## Exigences d’accès

<!--drafted - for P&P releases: 

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

Vous devez disposer des éléments suivants :

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
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modifier l’accès aux objectifs ou plus</p> <p><b>NOTE</b>

<p>Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir :</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Accorder l’accès aux objectifs Adobe Workfront</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> 
    <div> 
     <p>Gérer les autorisations pour l’objectif</p> 
     <p>Pour plus d’informations sur le partage des objectifs, voir <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Partage d’un objectif dans les objectifs Workfront</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

*Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Conditions préalables

Avant de pouvoir commencer, vous devez disposer des éléments suivants :

* Un modèle de mise en page qui inclut la zone Objectifs dans le menu principal.
* Vous avez créé les objectifs que vous souhaitez modifier ou vous disposez des autorisations de gestion pour eux.

## Observations relatives à la modification des objectifs

* Vous ne pouvez pas modifier des objectifs dont l’état est Fermé.
* Vous pouvez modifier des objectifs à partir de n’importe quelle période.

   Vous pouvez modifier les informations suivantes pour un objectif antérieur :

   * Nom
   * Période
   * Statut

      >[!TIP]
      >
      >Si l’objectif est Fermé, la réouverture recalcule le pourcentage de progression terminé. Vous ne pouvez pas modifier un objectif fermé.

   * Description
   * Résultats et activités

## Modifier les objectifs

<!--
Editing goals differs depending on what environment you use.

### Edit goals in the Production environment

1. Go to a goal that you want to edit and click the goal name to open the **Goal Details** panel. 
1. Click the **More icon** ![](assets/more-icon.png), then click **Edit**.

   ![](assets/edit-goal-highlighted.png)

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

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png), puis cliquez sur **Objectifs**.\
   Une liste d’objectifs s’affiche.
1. Cliquez sur un objectif.\
   La page d’objectif s’affiche.

   ![](assets/goal-page-unshimmed.png)

1. Pour modifier les informations de l’objectif, effectuez l’une des opérations suivantes :
   * Cliquez sur les champs qui s&#39;affichent dans l&#39;en-tête de l&#39;objectif pour les mettre à jour. Tous les champs de l’en-tête ne sont pas modifiables.
   * Cliquez sur le bouton **Icône Plus** ![](assets/more-icon.png) à droite du nom de l’objectif, puis cliquez sur **Modifier**.
   * Cliquez sur **Détails de l’objectif** dans le panneau de gauche, puis cliquez sur l’icône **Icône Modifier** ![](assets/edit-icon.png) dans le coin supérieur droit, puis cliquez sur **Tout modifier**. Commencez à mettre à jour les champs dans la section Détails de l’objectif .

      >[!IMPORTANT]
      >
      >Tous les champs qui s&#39;affichent dans les zones mentionnées ci-dessus ne peuvent pas être modifiés. Workfront calcule certains champs et ils sont en lecture seule.

1. (Conditionnel) Selon ce que vous avez sélectionné à l’étape précédente, mettez à jour les informations suivantes sur l’objectif :

   * Mettez à jour les informations suivantes dans l’en-tête de l’objectif, puis appuyez sur Entrée pour enregistrer vos modifications :
      * **Nom de l’objectif**: Cliquez sur le nom de l’objectif et commencez à saisir un nouveau nom.
      * **Propriétaire**: Cliquez sur le nom du propriétaire et commencez à saisir le nom d’un utilisateur, d’une équipe, d’un groupe ou de votre société, puis sélectionnez-le lorsqu’il s’affiche dans la liste. Vous ne pouvez avoir qu&#39;un seul propriétaire pour un objectif.
   * Mettez à jour les informations suivantes dans la zone Modifier l’objectif , puis cliquez sur **Enregistrer**:
      * **Nom de l’objectif**
      * **Période**: Cliquez pour mettre à jour la période de l’objectif.\
         Ou\
         Sélectionner **Activation des dates personnalisées** pour spécifier des dates pour le **Début** et **Dates de fin**.

         >[!TIP]
         >
         >Désélectionner **Activation des dates personnalisées** pour revenir à la période d’origine de l’objectif.

      * **Propriétaire de l’objectif**
      * **Description**: Ajoutez ou mettez à jour des informations sur l’objectif.
   * Mettez à jour ou passez en revue les informations dans la section Détails de l’objectif . Pour plus d’informations, voir [Mise à jour des objectifs dans la section Détails de l’objectif dans les objectifs Adobe Workfront](../goal-management/update-goals-in-goal-details-panel.md).

   <!-- (should you update the title here after changing it at production??? - change it to Update goals in the goal Details section)-->

1. (Facultatif) Cliquez sur **Indicateurs de progression** dans le panneau de gauche pour ajouter des résultats, des activités ou des projets à l’objectif. L’ajout d’indicateurs de progression vous permet de suivre la progression de l’objectif.
Pour plus d’informations, voir les articles suivants :
   * [Ajout d’activités aux objectifs dans les objectifs Adobe Workfront](../results-and-activities/add-activities-to-goals.md)
   * [Ajout de résultats aux objectifs dans les objectifs Adobe Workfront](../results-and-activities/add-results-to-goals.md).
   * [Ajout de projets aux objectifs dans les objectifs Adobe Workfront](../results-and-activities/connect-projects-to-goals-overview.md).

</div>
