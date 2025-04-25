---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: Supprimer l’alignement des objectifs dans les objectifs Adobe Workfront
description: Vous pouvez supprimer l’alignement entre deux objectifs s’il n’est plus logique qu’ils soient connectés.
author: Alina
feature: Workfront Goals
exl-id: a6196356-ca11-4759-9cff-64850a60208e
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 88%

---

# Supprimer l’alignement des objectifs dans Objectifs Adobe Workfront

<!--Audited P&P only: 4/2025-->

Vous pouvez supprimer l’alignement entre deux objectifs s’il n’est plus logique qu’ils soient connectés.

Pour plus d’informations sur l’alignement des objectifs, consultez les articles suivants :

* [Aligner les objectifs en les connectant dans Objectifs Adobe Workfront](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md)
* [Aligner les objectifs en convertissant les résultats et les activités en objectifs](../../workfront-goals/goal-alignment/align-goals-by-converting-results-activities.md)

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

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
 <p>Nouvelle licence : contributeur ou contributrice ou niveau supérieur</p>
 Ou
 <p>Licence actuelle : demande ou niveau supérieur</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Produit*</td>
 <td>
   <p> Nouvelle exigence de produit : Workfront</p>
   Ou
   <p>Configuration requise actuelle du produit : en plus d’une licence Workfront, vous devez acheter une licence pour les objectifs Adobe Workfront. </p> <p>Pour plus d’informations, consultez la section <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Exigences pour l’utilisation des Objectifs Workfront</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Niveau d’accès</td>
 <td> <p>Modifier l’accès aux Objectifs</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Autorisations d’objet</td>
 <td>
  <p>Autorisations d’affichage ou de niveau supérieur sur l’objectif pour l’afficher</p>
  <p>Autorisations de gestion sur l’objectif pour le modifier</p>
  <p>Pour plus d’informations sur le partage des objectifs, voir <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Partager un objectif dans Objectifs Workfront</a>. </p>
  </td>
 </tr>
   <td role="rowheader"><p>Modèle de mise en page</p></td>
   <td> <p>Toutes les personnes, y compris les administrateurs et administratrices Workfront, doivent se voir attribuer un modèle de mise en page incluant la zone Objectifs dans le menu principal. </p>  
</td>
  </tr>
</tbody>
</table>

*Pour plus d’informations, voir [Conditions d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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
