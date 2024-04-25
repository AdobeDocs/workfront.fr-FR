---
product-previous: workfront-goals
navigation-topic: goal-management
title: Modifier des objectifs dans Objectifs Adobe Workfront
description: Vous pouvez modifier des objectifs existants à partir de n’importe quelle période et dans n’importe quel état.
author: Alina
feature: Workfront Goals
exl-id: 74db534c-6897-40c2-bea9-a9d30a40f61c
source-git-commit: 09e34ecdfeec531ebbaaba4fb8682496c53d86bf
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 11%

---

# Modifier des objectifs dans Objectifs Adobe Workfront

Vous pouvez modifier des objectifs existants à partir de n’importe quelle période et dans n’importe quel état.

## Conditions d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr>
 <td role="rowheader">Forfait Adobe Workfront</td>
 <td>
 <p>N’importe quelle</p>

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
 <td role="rowheader">Niveau d’accès</td>
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
      * **Nom de l’objectif**: cliquez sur le nom de l’objectif et commencez à saisir un nouveau nom.
      * **Propriétaire**: cliquez sur le nom du propriétaire, puis commencez à saisir le nom d’un utilisateur, d’une équipe, d’un groupe ou de votre société, puis sélectionnez-le lorsqu’il s’affiche dans la liste. Vous ne pouvez avoir qu&#39;un seul propriétaire pour un objectif.
   * Mettez à jour les informations suivantes dans la zone Modifier l’objectif , puis cliquez sur **Enregistrer**:
      * **Nom de l’objectif**
      * **Période**: cliquez sur pour mettre à jour la période de l’objectif.\
        Ou\
        Sélectionner **Activation des dates personnalisées** pour spécifier des dates pour le **Début** et **Dates de fin**.

        >[!TIP]
        >
        >Désélectionner **Activation des dates personnalisées** pour revenir à la période d’origine de l’objectif.

      * **Propriétaire de l’objectif**
      * **Description**: ajoutez ou mettez à jour des informations sur l’objectif.
   * Mettez à jour ou passez en revue les informations dans la section Détails de l’objectif . Pour plus d’informations, voir [Mise à jour des objectifs dans la section Détails des objectifs d’Adobe Workfront](../goal-management/update-goals-in-goal-details-panel.md).

   <!-- (should you update the title here after changing it at production??? - change it to Update goals in the goal Details section)-->

1. (Facultatif) Cliquez sur **Indicateurs de progression** dans le panneau de gauche pour ajouter des résultats, des activités ou des projets à l’objectif. L’ajout d’indicateurs de progression vous permet de suivre la progression de l’objectif.
Pour plus d’informations, voir les articles suivants :
   * [Ajouter des activités aux objectifs dans Objectifs Adobe Workfront](../results-and-activities/add-activities-to-goals.md)
   * [Ajout de résultats aux objectifs dans les objectifs Adobe Workfront](../results-and-activities/add-results-to-goals.md).
   * [Ajout de projets aux objectifs dans les objectifs Adobe Workfront](../results-and-activities/connect-projects-to-goals-overview.md).

</div>
