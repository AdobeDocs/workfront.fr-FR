---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: Supprimer l’alignement des objectifs dans les objectifs Adobe Workfront
description: Vous pouvez supprimer l’alignement entre deux objectifs s’il n’est plus logique qu’ils soient connectés.
author: Alina
feature: Workfront Goals
exl-id: a6196356-ca11-4759-9cff-64850a60208e
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 77%

---

# Supprimer l’alignement des objectifs dans Objectifs Adobe Workfront

<!--Audited P&P only: 4/2025-->

Vous pouvez supprimer l’alignement entre deux objectifs s’il n’est plus logique qu’ils soient connectés.

Pour plus d’informations sur l’alignement des objectifs, consultez les articles suivants :

* [Aligner les objectifs en les connectant dans Objectifs Adobe Workfront](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md)
* [Aligner les objectifs en convertissant les résultats et les activités en objectifs](../../workfront-goals/goal-alignment/align-goals-by-converting-results-activities.md)

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
  <td> <p>Package Adobe Workfront</p> </td> 
   <td> 
   <p>Adobe Workfront Ultimate</p>
   </td> 
  </tr> 
 <tr>
 <td role="rowheader">Licence Adobe Workfront</td>
 <td>
 <p>Contributeur ou version ultérieure</p>
 <p>Requête ou supérieure</p> </td>
 </tr>
  <tr>
 <td role="rowheader">Niveau d’accès</td>
 <td> <p>Modifier l’accès aux Objectifs</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Autorisations d’objet</td>
 <td>
  <p>Autorisations d’affichage ou de niveau supérieur sur l’objectif pour l’afficher</p>
  <p>Autorisations de gestion sur l’objectif pour le modifier</p>

</td>
 </tr>
   <td role="rowheader"><p>Modèle de mise en page</p></td>
   <td> <p>Un modèle de mise en page comprenant la zone Objectifs du menu principal doit être affecté à tous les utilisateurs, y compris les administrateurs système. </p>  
</td>
  </tr>
</tbody>
</table>

Pour plus d’informations, consultez la section [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
 <p>Current license: Request or higher</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Product*</td>
 <td>
   <p> New product requirement: Workfront</p>
   Or
   <p>Current product requirement: In addition to a Workfront license, you must purchase a license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Access level</td>
 <td> <p>Edit access to Goals</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Object permissions</td>
 <td>
  <p>View or higher permissions to the goal to view it</p>
  <p>Manage permissions to the goal to edit it</p>
  <p>For information about sharing goals, see <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Workfront Goals</a>. </p>
  </td>
 </tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Goals area in the Main Menu. </p>  
</td>
  </tr>
</tbody>
</table>-->

## Conditions préalables

Vous devez disposer des éléments suivants avant de pouvoir démarrer :

* Objectif parent auquel est associé au moins un objectif enfant. Les objectifs enfants sont les indicateurs de progression de l’objectif.

## Considérations relatives à la suppression de l’alignement des objectifs

Tenez compte des points suivants lorsque vous supprimez l’alignement entre deux objectifs :

* L’objectif parent doit être associé à un autre objectif, activité ou résultat pour rester actif.
* Vous ne pouvez pas supprimer un objectif enfant aligné d’un objectif parent s’il s’agit du seul indicateur de progression de l’objectif parent.
* L’objectif enfant devient un objectif autonome lorsque vous supprimez son alignement sur l’objectif parent.

## Supprimer l’alignement d’objectif

<!--
Removing goal alignment differs depending on which environment you use.

### Remove goal alignment in the Production environment


1. Go to a child goal aligned to a parent goal. 
1. Click the goal name to open the **Goal Details** panel. 
1. Click the **gear icon** ![Gear icon](assets/gear-icon-settings.png) next to the parent goal, then click **Remove alignment**.

   ![Reove alignment](assets/edit-remove-alignment-350x88.png)

   The goal becomes a standalone goal and its progress no longer influences the progress of the original parent goal. 

1. (Optional) Click **Undo** in the lower-left corner of the screen if you want to revert this change and keep the goals aligned. 
1. (Optional) Add activities and results to either goals to indicate their progress. For information about adding activities and results, see the following articles:

   * [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md) 
   * [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md)
-->

1. Accédez à la zone **Objectifs** dans Workfront et cliquez sur le nom d’un objectif pour ouvrir la page de l’objectif.
1. Dans la page de l’objectif d’un objectif parent, cliquez sur **Indicateurs de progression** dans le panneau de gauche.

   ![Supprimer l’alignement des objectifs](assets/remove-goal-alignment-from-list-unshimmed.png)

1. Dans le regroupement **Type : Objectif** sélectionnez un objectif, puis cliquez sur l’icône **Déconnecter** ![Icône Déconnecter](assets/disconnect-goal-to-remove-alignment-icon-unshimmed.png) en haut de la liste.

   La boîte Déconnecter s’affiche.

1. Cliquez sur **Déconnecter** pour déconnecter l’objectif sélectionné de son parent.

   L’objectif devient un objectif autonome et n’est plus répertorié comme indicateur de progression de l’objectif d’origine. La progression de l’objectif déconnecté n’a plus d’incidence sur la progression de l’objectif initial.

   Un message de réussite s’affiche dans le coin supérieur droit de la page pour confirmer que l’objectif a été déconnecté.
