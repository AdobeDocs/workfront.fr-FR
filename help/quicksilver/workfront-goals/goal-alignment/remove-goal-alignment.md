---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: Supprimer l’alignement des objectifs dans Objectifs Adobe Workfront
description: Vous pouvez supprimer l’alignement entre deux objectifs s’il n’est plus logique qu’ils soient connectés.
author: Alina
feature: Workfront Goals
exl-id: a6196356-ca11-4759-9cff-64850a60208e
source-git-commit: 09e34ecdfeec531ebbaaba4fb8682496c53d86bf
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 18%

---

# Supprimer l’alignement des objectifs dans Objectifs Adobe Workfront

Vous pouvez supprimer l’alignement entre deux objectifs s’il n’est plus logique qu’ils soient connectés.

Pour plus d’informations sur l’alignement des objectifs, consultez les articles suivants :

* [Alignement des objectifs en les connectant aux objectifs Adobe Workfront](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md)
* [Alignement des objectifs en convertissant les résultats et les activités en objectifs](../../workfront-goals/goal-alignment/align-goals-by-converting-results-activities.md)

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
 <p>Licence actuelle : demande ou supérieure</p> </td>
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
  <p>Afficher ou des autorisations supérieures à l’objectif pour l’afficher</p>
  <p>Gérer les autorisations sur l’objectif pour le modifier</p>
  <p>Pour plus d’informations sur le partage des objectifs, consultez <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Partager un objectif dans les Objectifs Workfront</a>. </p>
  </td>
 </tr>
   <td role="rowheader"><p>Modèle de mise en page</p></td>
   <td> <p>Tous les utilisateurs, y compris les administrateurs de Workfront, doivent se voir attribuer un modèle de mise en page incluant la zone Objectifs dans le menu principal. </p>  
</td>
  </tr>
</tbody>
</table>

*Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Conditions préalables

Vous devez disposer des éléments suivants avant de commencer :

* Objectif parent auquel est associé au moins un objectif enfant. Les objectifs pour les enfants sont les indicateurs de progrès de l&#39;objectif.

## Considérations relatives à la suppression de l’alignement des objectifs

Tenez compte des points suivants lorsque vous supprimez l’alignement entre deux objectifs :

* L’objectif parent doit être associé à un autre objectif, activité ou résultat pour rester actif.
* Vous ne pouvez pas supprimer un objectif enfant aligné d’un objectif parent s’il s’agit du seul indicateur de progression de l’objectif parent.
* L’objectif enfant devient un objectif autonome lorsque vous supprimez son alignement sur l’objectif parent.

## Supprimer l’alignement d’objectif

<!--
Removing goal alignment differs depending on which environment you use.

### Remove goal alignment in the Production environment


1. Go to a child goal aligned to a parent goal. 
1. Click the goal name to open the **Goal Details** panel. 
1. Click the **gear icon** ![](assets/gear-icon-settings.png) next to the parent goal, then click **Remove alignment**.

   ![](assets/edit-remove-alignment-350x88.png)

   The goal becomes a standalone goal and its progress no longer influences the progress of the original parent goal. 

1. (Optional) Click **Undo** in the lower-left corner of the screen if you want to revert this change and keep the goals aligned. 
1. (Optional) Add activities and results to either goals to indicate their progress. For information about adding activities and results, see the following articles:

   * [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md) 
   * [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md)
-->

1. Accédez au **Objectifs** dans Workfront et cliquez sur le nom d’un objectif pour ouvrir la page de l’objectif.
1. Dans la page de l’objectif d’un objectif parent, cliquez sur **Indicateurs de progression** dans le panneau de gauche.

   ![](assets/remove-goal-alignment-from-list-unshimmed.png)

1. Dans le **Type : Objectif** regroupement, sélectionnez un objectif, puis cliquez sur le bouton **Déconnecter** icon ![](assets/disconnect-goal-to-remove-alignment-icon-unshimmed.png) en haut de la liste.

   La zone Déconnecter s’affiche.

1. Cliquez sur **Déconnecter** pour déconnecter l’objectif sélectionné de son parent.

   L’objectif devient un objectif autonome et n’est plus répertorié comme indicateur de progression de l’objectif d’origine. La progression de l’objectif déconnecté n’a plus d’incidence sur la progression de l’objectif initial.

   Un message de réussite s’affiche dans le coin supérieur droit de la page pour confirmer que l’objectif a été déconnecté.