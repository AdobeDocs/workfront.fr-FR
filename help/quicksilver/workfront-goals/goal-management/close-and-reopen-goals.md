---
product-previous: workfront-goals
navigation-topic: goal-management
title: Fermer et rouvrir desobjectifs dans Objectifs Adobe Workfront
description: Vous pouvez fermer un objectif lorsque vous souhaitez indiquer que vous l’avez terminé ou que vous n’y travaillez plus car il est devenu obsolète.
author: Alina
feature: Workfront Goals
exl-id: bbb549c1-aea6-4f5e-8a6b-01fc04cf06ef
source-git-commit: 024c612d46848c55529e902a00d481588d261584
workflow-type: tm+mt
source-wordcount: '949'
ht-degree: 6%

---

# Fermer et rouvrir desobjectifs dans Objectifs Adobe Workfront

Vous pouvez fermer un objectif lorsque vous souhaitez indiquer les éléments suivants :

* L&#39;objectif est atteint, soit parce que vous l&#39;avez atteint, soit parce que la période s&#39;est écoulée.
* Vous n&#39;y travaillez plus et ne prévoyez pas de le faire dans un avenir immédiat.

Vous pouvez rouvrir les objectifs qui ont été fermés lorsqu’ils redeviennent pertinents.

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

## Remarques concernant la fermeture ou la réouverture d’objectifs

* Vous devez avoir accès à Modifier les objectifs dans votre niveau d’accès avant de pouvoir fermer et rouvrir les objectifs. Pour plus d’informations sur l’octroi de l’accès aux Objectifs, voir [Accorder l’accès aux objectifs Adobe Workfront](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).
* Vous ne pouvez fermer que les objectifs actifs. Vous ne pouvez pas fermer les objectifs dont l’état est En création.

  Pour plus d’informations sur les états d’objectif, voir [Présentation de l’état des objectifs dans les objectifs Adobe Workfront](../../workfront-goals/goal-management/goal-status-overview.md).

* Fermer les objectifs bloque sa progression et vous permet d’évaluer vos performances dans leur réalisation.

  >[!CAUTION]
  >
  >Lors de la fermeture d’un objectif avec des objectifs de contribution actifs, sa progression change après la fermeture pour indiquer la progression des objectifs actifs de contribution. Pour plus d’informations sur l’alignement des objectifs, voir [Alignement des objectifs en les connectant aux objectifs Adobe Workfront](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).

* Mettez à jour les indicateurs de progression de l’objectif avant de fermer l’objectif pour vous assurer que l’objectif se termine avec une valeur de progression exacte. Si tous les indicateurs de progression ont été atteints, le pourcentage d’objectif terminé doit être de 100 % et votre objectif a été atteint. Pour plus d’informations sur la mise à jour de vos objectifs, voir [Mise à jour de la progression de l’objectif dans les objectifs Adobe Workfront](../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md).
* Conservez les commentaires finaux comme une mise à jour des objectifs que vous fermez. Pour plus d’informations sur l’ajout de commentaires aux objectifs, voir [Gestion des commentaires d’objectif dans les objectifs Adobe Workfront](../../workfront-goals/goal-management/manage-goal-comments.md).
* Vous ne pouvez plus mettre à jour la progression des résultats et des activités sur un objectif que vous fermez.
* Vous pouvez rouvrir un objectif fermé si vous souhaitez continuer à travailler dessus.
* Si l’objectif n’a pas été atteint, pensez à copier la plupart de ses informations sur la prochaine période (trimestre ou année). Il s’agit d’une excellente option pour les objectifs qui sont identiques d’une période à l’autre ou pour les objectifs sur lesquels vous devrez peut-être encore travailler au cours de la prochaine période. Pour plus d’informations sur la copie d’objectifs, voir [Copie d’objectifs dans les objectifs Adobe Workfront](../../workfront-goals/goal-management/copy-goals.md). Vous pouvez également mettre à jour la période sur l’objectif au lieu de la copier dans une autre période.
* Workfront supprime les commentaires d’un objectif fermé lorsque vous le rouvrez. Si vous devez conserver les commentaires, nous vous recommandons de copier l’objectif fermé, y compris les résultats qui lui sont associés, plutôt que de le rouvrir.


## Fermer les objectifs

<!--
Closing goals differs depending on what environment you use. 

### Close goals in the Production environment

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   The Goal List opens. 

1. (Optional) Modify your filters to display only goals that are active.

   For information about filtering information in Workfront Goals, see [Filter information in Adobe Workfront Goals](../../workfront-goals/goal-management/filter-information-wf-goals.md). 

1. Click an active goal.

   The Goal Details panel displays on the right. 

1. (Optional and recommended) Click the **Updates** tab and add an update in the **Comment here** field about the reason you are closing the goal, then click **Post**. 

1. Click the **More icon** ![](assets/more-icon.png) to the right of the goal name, then click **Close** > **Close Goal**.

   This closes the goal and saves the current progress on the goal and its results and activities.

   >[!IMPORTANT]
   >
   >If the goal has contributing goals that are still active, the progress of the goal continues to update based on the progress of the aligned goals.
   >
   >
   >![](assets/closing-goals-with-active-aligned-goals-warning-350x71.png)   >
   >

1. (Optional) Modify your filters again to display only closed goals. The goals you closed display on the screen.
-->

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) > **Objectifs** dans le coin supérieur droit.

   La liste des objectifs s’affiche.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

1. (Facultatif) Modifiez vos filtres pour n’afficher que les objectifs actifs.

   Pour plus d’informations sur le filtrage des informations dans les objectifs Workfront, voir [Filtrage des informations dans les objectifs Adobe Workfront](../goal-management/filter-information-wf-goals.md).
1. Cliquez sur un objectif actif.

   La page d’objectif s’ouvre.

   ![](assets/goal-page-unshimmed.png)
1. Cliquez sur le bouton **Plus** menu ![](assets/more-icon.png) à droite du nom de l’objectif, puis cliquez sur **Fermer**.

   L’objectif se ferme et vous recevez une confirmation dans le coin supérieur droit de l’écran.

   ![](assets/goal-close-confirmation-with-add-closing-notes-link.png)

1. (Facultatif) Dans la zone de confirmation, cliquez sur **Ajout de notes de fermeture** pour ajouter des commentaires sur cet objectif et les raisons pour lesquelles vous devez le fermer.
1. Ajoutez des notes de fin, puis cliquez sur **Ajout de notes**.

   ![](assets/add-closing-notes-box-unshimmed.png)

   Les commentaires s’affichent dans la section Détails de l’objectif de la page de l’objectif, dans la zone Notes de fermeture .

   >[!NOTE]
   >
   >Workfront supprime les notes de fermeture si vous rouvrez ultérieurement un objectif fermé.


## Réouverture des objectifs

Vous pouvez rouvrir les objectifs fermés si vous décidez qu’ils sont redevenus pertinents et que vous devez continuer à mettre à jour leur progression.

<!--
Reopening goals differs depending on what environment you use.

### Reopen goals in the Production environment

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   The Goal List opens. 

1. (Optional) Modify your filters to display only goals that are closed.

   For information about filtering information in Workfront Goals, see [Filter information in Adobe Workfront Goals](../../workfront-goals/goal-management/filter-information-wf-goals.md).


1. Click a closed goal.

   This opens the Goal Details panel on the right. 

1. Click the **More icon** ![](assets/more-icon.png) to the right of the goal name, then click **Reopen** > **Reopen**.

   This reopens the goal and places it in a status of Active. The progress of the goal is recalculated starting with the current date. 

1. (Optional) Modify your filters again to display only active goals. The goals you opened display on the screen.

-->

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png)> **Objectifs** dans le coin supérieur droit.

   La liste des objectifs s’affiche.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

1. (Facultatif) Modifiez vos filtres pour n’afficher que les objectifs fermés.

   Pour plus d’informations sur le filtrage des informations dans les objectifs Workfront, voir [Filtrage des informations dans les objectifs Adobe Workfront](../goal-management/filter-information-wf-goals.md).
1. Cliquez sur le nom d’un objectif fermé.

   La page d’objectif s’ouvre.
1. Cliquez sur le bouton **Plus** menu ![](assets/more-icon.png) à droite du nom du goal, puis **Réouvrir** > **Réouvrir**.

   Les événements suivants se produisent :
   * L’objectif est maintenant ouvert et a l’état Actif.
   * La progression de l&#39;objectif est recalculée à partir de la date courante.
   * Toutes les notes de fermeture sont supprimées de la page Détails de l’objectif . Les notes de fermeture supprimées ne peuvent pas être récupérées.

1. (Facultatif) Modifiez à nouveau vos filtres pour n’afficher que les objectifs actifs.

   Les objectifs que vous avez ouverts s’affichent à l’écran.

