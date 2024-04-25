---
product-previous: workfront-goals
navigation-topic: goal-management
title: Créer des objectifs dans Objectifs Adobe Workfront
description: Que vous soyez PDG, responsable ou contributeur individuel, vous pouvez créer des objectifs dans les objectifs d’Adobe Workfront afin d’aligner votre travail avec vos objectifs et les objectifs qui définissent la stratégie de votre entreprise.
author: Alina
feature: Workfront Goals
exl-id: 14bf48b6-eb0c-4b00-a1a4-0d070ccc1392
source-git-commit: 09e34ecdfeec531ebbaaba4fb8682496c53d86bf
workflow-type: tm+mt
source-wordcount: '680'
ht-degree: 13%

---

# Créer des objectifs dans Objectifs Adobe Workfront

Que vous soyez PDG, responsable ou contributeur individuel, vous pouvez créer des objectifs dans les objectifs d’Adobe Workfront afin d’aligner votre travail avec vos objectifs et les objectifs qui définissent la stratégie de votre entreprise.

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
<td role="rowheader">Niveau d’accès*</td>
<td> <p>Modifier l’accès aux objectifs</p> </td>
</tr>
<tr data-mc-conditions="">
<td role="rowheader">Autorisations d’objet</td>
<td>
<p>Afficher ou des autorisations supérieures à l’objectif pour l’afficher</p>
<p>Gérer les autorisations sur l’objectif pour le modifier</p>
<p>Pour plus d’informations sur le partage des objectifs, consultez <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Partager un objectif dans les Objectifs Workfront</a>. </p>
</td>
</tr>
<tr>
   <td role="rowheader"><p>Modèle de mise en page</p></td>
   <td> <p>Tous les utilisateurs, y compris les administrateurs de Workfront, doivent se voir attribuer un modèle de mise en page incluant la zone Objectifs dans le menu principal. </p>  
</td>
  </tr>
</tbody>
</table>

*Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Instructions relatives à la création d’objectifs

Avant de commencer avec les objectifs de Workfront, nous vous recommandons de lire nos recommandations et instructions relatives aux bonnes pratiques en matière de gestion efficace des objectifs. Pour plus d’informations sur les consignes de création et de gestion des objectifs, voir [Présentation des objectifs d’Adobe Workfront](../../workfront-goals/goal-management/wf-goals-overview.md).

## Créer des objectifs

Cet article décrit comment créer un objectif stratégique dans les objectifs de Workfront. Pour plus d’informations sur la création d’un objectif de Business Case, voir [Créer des objectifs de Business Case](../../manage-work/projects/define-a-business-case/create-business-case-goals.md).

Vous pouvez créer un objectif stratégique de l’une des manières suivantes :

* [Créer un objectif à partir de zéro](#create-a-goal-from-scratch)
* [Copier un objectif existant](#copy-an-existing-goal)
* [Convertir un résultat ou une activité en objectif](#convert-a-result-or-activity-to-a-goal)

### Créer un objectif à partir de zéro {#create-a-goal-from-scratch}

<!--
Creating goals differs depending on what environment you use.

#### Create a goal from scratch in the Production environment 


1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper right corner, then click **Goals**.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -)

   The Goal List displays.

1. (Conditional) Click **Goal List**, **Graphs**, **Pulse**, or **Check-in** in the left pane, then click **Add Goal** in the upper-right corner of the page. The Add Goal box displays.

   ![](assets/add-goal-box-350x235.png)

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

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit, puis cliquez sur **Objectifs**.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   La liste des objectifs s’affiche.
1. Cliquez sur **Nouvel objectif**.

   La zone Nouveau but s’affiche.

   ![](assets/new-goal-box-unshimmed.png)

1. Renseignez les champs suivants :
   * **Nom de l’objectif**: saisissez un nom pour l’objectif. Champ obligatoire.
   * **Période**: sélectionnez un trimestre ou une année prédéfini dans la variable **Période** champ déroulant

     Ou

     Sélectionnez la variable **Activation des dates personnalisées** , puis sélectionnez une **Début** et **Date de fin** pour l’objectif.

     Les années précédentes, en cours et suivantes, ainsi que leurs trimestres respectifs, sont répertoriés comme des options prédéfinies dans le champ déroulant Période .

     La période de l’objectif indique la période pendant laquelle vous prévoyez que l’objectif se termine.

   * **Propriétaire de l’objectif**: commencez à saisir le nom d’un utilisateur, d’une équipe, d’un groupe ou de votre organisation pour indiquer qui est le propriétaire de l’objectif. Par défaut, vous êtes sélectionné en tant que propriétaire de l’objectif.
   * **Description**: saisissez des informations supplémentaires sur l’objectif.
1. Cliquez sur **Créer un objectif**.

   Le nouvel objectif est répertorié dans la liste Objectif et a le statut de **Version préliminaire**.

   Vous devez associer un objectif à un indicateur de progression pour l’activer et commencer à travailler dessus.

   Effectuez au moins l’une des opérations suivantes pour préparer l’activation d’un objectif :
   * Ajouter un résultat

     Pour plus d’informations sur l’ajout de résultats, voir [Ajout de résultats aux objectifs dans les objectifs Adobe Workfront](../results-and-activities/add-results-to-goals.md).
   * Ajout d’une activité

     Pour plus d’informations sur l’ajout d’activités, voir [Ajout d’activités aux objectifs dans les objectifs Adobe Workfront](../results-and-activities/add-activities-to-goals.md).
   * Aligner un autre objectif dessus

     Pour plus d’informations sur l’alignement des objectifs, voir [Alignement des objectifs en les connectant aux objectifs Adobe Workfront](../goal-alignment/align-goals-by-connecting-them.md).


### Copier un objectif existant {#copy-an-existing-goal}

Vous pouvez créer un objectif en copiant un objectif existant.

Pour plus d’informations sur la copie d’objectifs, voir [Copie d’objectifs dans les objectifs Adobe Workfront](../../workfront-goals/goal-management/copy-goals.md).

### Convertir un résultat ou une activité en objectif {#convert-a-result-or-activity-to-a-goal}

Vous pouvez créer un objectif en convertissant le résultat ou l’activité d’un objectif existant en objectif. Le nouvel objectif s’aligne sur l’objectif d’origine.

Pour plus d’informations sur la conversion des résultats et des activités en objectifs, voir [Alignement des objectifs en convertissant les résultats et les activités en objectifs](../../workfront-goals/goal-alignment/align-goals-by-converting-results-activities.md).

