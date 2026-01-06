---
product-previous: workfront-goals
navigation-topic: goal-management
title: Créer des objectifs dans les objectifs Adobe Workfront
description: Que vous soyez une personne chargée de la direction générale, une personne responsable de la gestion ou une personne contributrice, vous pouvez créer des objectifs dans les Objectifs Adobe Workfront afin d’aligner votre travail avec vos objectifs et ceux qui définissent la stratégie de votre entreprise.
author: Alina
feature: Workfront Goals
exl-id: 14bf48b6-eb0c-4b00-a1a4-0d070ccc1392
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '635'
ht-degree: 88%

---

# Créer des objectifs dans les Objectifs Adobe Workfront

<!--Audited for P&P only: 4/2025-->

Que vous soyez une personne chargée de la direction générale, une personne responsable de la gestion ou une personne contributrice, vous pouvez créer des objectifs dans les Objectifs Adobe Workfront afin d’aligner votre travail avec vos objectifs et ceux qui définissent la stratégie de votre entreprise.

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

## Des instructions relatives à la création d’objectifs.

Avant de commencer avec les Objectifs Workfront, nous vous recommandons de lire nos recommandations et instructions relatives aux bonnes pratiques de gestion des objectifs. Pour plus d’informations sur les instructions de création et de gestion des objectifs, voir [Vue d’ensemble des Objectifs Adobe Workfront](../../workfront-goals/goal-management/wf-goals-overview.md).

## Créer des objectifs

Cet article décrit comment créer un objectif stratégique dans les Objectifs Workfront. Pour plus d’informations sur la création d’un objectif de business case, voir [Créer des objectifs de business case](../../manage-work/projects/define-a-business-case/create-business-case-goals.md).

Vous pouvez créer un objectif stratégique de l’une des manières suivantes :

* [Créer un objectif à partir de zéro](#create-a-goal-from-scratch)
* [Copier un objectif existant](#copy-an-existing-goal)
* [Convertir un résultat ou une activité en objectif](#convert-a-result-or-activity-to-a-goal)

### Créer un objectif à partir de zéro {#create-a-goal-from-scratch}

<!--
Creating goals differs depending on what environment you use.

#### Create a goal from scratch in the Production environment 


1. Click the **Main Menu** icon ![Main Menu icon](assets/main-menu-icon.png) in the upper right corner, then click **Goals**.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -)

   The Goal List displays.

1. (Conditional) Click **Goal List**, **Graphs**, **Pulse**, or **Check-in** in the left pane, then click **Add Goal** in the upper-right corner of the page. The Add Goal box displays.

   ![Add goal box](assets/add-goal-box-350x235.png)

   >[!TIP]
   >
   >You can add a goal from any section in Workfront Goals. The process for creating a goal is identical regardless of the section you choose to add the goal from.

1. Start typing what you want to achieve in the **Goal** field. This is the name of the goal and a required field. 
1. Select a time period when the goal should be executed in the **Period** drop-down menu. This is a pre-filled field. The default is the current quarter.

   Select from the following predefined options:

   * The current year
   * The quarters of the current year
   * The next two years
   * The quarters of the next two years

   Or

   Click **Define custom dates** to select a custom time frame. 

1. (Conditional) Select a **Start date** and an **End date** for your goal, if you clicked **Define custom dates**.

   >[!TIP]
   >
   >* You can create a goal with dates in any time period, including up to 2 years in the past. 
   >* When defining custom dates, they are constrained by the initial date you selected. So if you select quarter and then custom dates, you can't go beyond that quarter.

1. (Optional) Click **Reset custom dates** to return to the predefined options.

   >[!TIP]
   >
   >We recommend that everyone in your organization selects the same timeframes for similar goals or goals that are aligned. This provides better alignment between goals and ensures that everyone's work supports your over-arching strategy.

1. (Optional) Click your name in the **Owner** field, if you want to indicate someone else as the owner of the goal. By default, you are the owner of goals you create. 
1. Start typing the name of a user, team, group, or the name of your organization in the **Owner** field, then select it when it displays in the list. You can have only one owner for a goal. 
1. (Optional) Enter a **Description** for the goal. This field is optional. 
1. Click **Save**.

   The status of the new goal is Draft.

   >[!IMPORTANT]
   >
   >You must associate a goal with a progress indicator to activate it and start working on it. 
   >
   >Do at least one of the following to be able to activate a goal: 
   >
   >* Add a Result
   >
   >  For information about adding results, see [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md).
   >   
   >* Add an Activity
   >   
   >  For information about adding activities, see [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md). 
   >   
   >* Align another goal to it
   >   
   >  For information about aligning goals, see [Align goals by connecting them in Adobe Workfront Goals](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).

1. Click the **X** icon in the upper-right of the Goal Details panel to close it.

-->

{{step1-to-goals}}

La liste des objectifs s’affiche.

1. Cliquez sur **Nouvel objectif**.

   La zone Nouvel objectif s’affiche.

   ![Nouvelle zone d’objectif](assets/new-goal-box-unshimmed.png)

1. Renseignez les champs suivants :
   * **Nom de l’objectif** : saisissez un nom pour l’objectif. Champ obligatoire.
   * **Période** : sélectionnez un trimestre ou une année prédéfini(e) dans le champ déroulant **Période**.

     Ou

     Sélectionnez l’option **Activer les dates personnalisées**, puis une **Date de début** et une **Date de fin** pour l’objectif.

     Les années précédentes, actuelle et suivantes, ainsi que leurs trimestres respectifs, sont répertoriés comme des options prédéfinies dans le champ déroulant Période.

     La période de l’objectif indique la période pendant laquelle vous prévoyez que l’objectif se termine.

   * **Personne propriétaire de l’objectif** : commencez à saisir le nom d’un utilisateur ou d’une utilisatrice, d’une équipe, d’un groupe ou de votre organisation pour indiquer qui est le propriétaire de l’objectif. Par défaut, vous êtes la personne propriétaire de l’objectif.
   * **Description** : informations complémentaires sur l’objectif.
1. Cliquez sur **Créer l’objectif**.

   Le nouvel objectif est répertorié dans la liste des objectifs et a le statut de **Brouillon**.

   Vous devez associer un objectif à un indicateur de progression pour l’activer et commencer à travailler.

   Effectuez au moins l’une des opérations suivantes pour préparer l’activation d’un objectif :
   * Ajouter un résultat

     Pour plus d’informations sur l’ajout de résultats, voir [Ajouter des résultats aux objectifs dans les Objectifs Adobe Workfront](../results-and-activities/add-results-to-goals.md).
   * Ajouter une activité

     Pour plus d’informations sur l’ajout d’activités, voir [Ajouter des activités aux objectifs dans les Objectifs Adobe Workfront](../results-and-activities/add-activities-to-goals.md).
   * Aligner un autre objectif sur celui-ci

     Pour plus d’informations sur l’alignement des objectifs, voir [Aligner des objectifs en les connectant entre les uns aux autres dans les Objectifs Adobe Workfront](../goal-alignment/align-goals-by-connecting-them.md).


### Copier un objectif existant {#copy-an-existing-goal}

Vous pouvez créer un objectif en copiant un objectif existant.

Pour plus d’informations sur la copie d’objectifs, voir [Copier des objectifs dans les Objectifs Adobe Workfront](../../workfront-goals/goal-management/copy-goals.md).

### Convertir un résultat ou une activité en objectif {#convert-a-result-or-activity-to-a-goal}

Vous pouvez créer un objectif en convertissant le résultat ou l’activité d’un objectif existant en objectif. Le nouvel objectif s’aligne sur l’objectif d’origine.

Pour plus d’informations sur la conversion des résultats et des activités en objectifs, voir [Aligner des objectifs en convertissant les résultats et les activités en objectifs](../../workfront-goals/goal-alignment/align-goals-by-converting-results-activities.md).

