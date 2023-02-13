---
product-previous: workfront-goals
navigation-topic: goal-management
title: Fermer et rouvrir les objectifs dans les objectifs Adobe Workfront
description: Vous pouvez fermer un objectif lorsque vous souhaitez indiquer que vous l’avez terminé ou que vous n’y travaillez plus car il est devenu obsolète.
author: Alina
feature: Workfront Goals
exl-id: bbb549c1-aea6-4f5e-8a6b-01fc04cf06ef
source-git-commit: afc2124a7fd0d9d52c04be1c174fdba314beec7a
workflow-type: tm+mt
source-wordcount: '908'
ht-degree: 0%

---

# Fermer et rouvrir les objectifs dans les objectifs Adobe Workfront

Vous pouvez fermer un objectif lorsque vous souhaitez indiquer les éléments suivants :

* L&#39;objectif est atteint, soit parce que vous l&#39;avez atteint, soit parce que la période s&#39;est écoulée.
* Vous n&#39;y travaillez plus et ne prévoyez pas de le faire dans un avenir immédiat.

Vous pouvez rouvrir les objectifs qui ont été fermés lorsqu’ils redeviennent pertinents.

## Exigences d’accès

<!--drafted for P&P release: 

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
   <td> <p>Modifier l’accès aux objectifs ou plus</p> <p><b>NOTE</b><p>Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir :</p> 
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

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Conditions préalables

Avant de pouvoir commencer, vous devez disposer des éléments suivants :

* Un modèle de mise en page qui inclut la zone Objectifs dans le menu principal.

## Remarques concernant la fermeture ou la réouverture d’objectifs

* Vous devez avoir accès à Modifier les objectifs dans votre niveau d’accès avant de pouvoir fermer et rouvrir les objectifs. Pour plus d’informations sur l’octroi de l’accès aux Objectifs, voir [Accorder l’accès aux objectifs Adobe Workfront](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).
* Vous ne pouvez fermer que les principaux objectifs. Vous ne pouvez pas fermer les objectifs dont l’état est En création.

   Pour plus d’informations sur les états d’objectif, voir [Présentation de l’état des objectifs dans les objectifs Adobe Workfront](../../workfront-goals/goal-management/goal-status-overview.md).

* Fermer les objectifs bloque sa progression et vous permet d’évaluer vos performances dans leur réalisation.

   >[!CAUTION]
   >
   >Lorsque vous classez un objectif qui a des objectifs principaux, son avancement change après la fin pour indiquer l’avancement des objectifs principaux. Pour plus d’informations sur l’alignement des objectifs, voir [Alignement des objectifs en les connectant aux objectifs Adobe Workfront](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).

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

1. (Facultatif) Modifiez vos filtres pour n’afficher que les objectifs principaux.

   Pour plus d’informations sur le filtrage des informations dans les objectifs Workfront, voir [Filtrage des informations dans les objectifs Adobe Workfront](../goal-management/filter-information-wf-goals.md).
1. Cliquez sur un principal objectif.

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
1. Cliquez sur le bouton **Plus** menu ![](assets/more-icon.png) à droite du nom de l’objectif, puis **Réouvrir** > **Réouvrir**.

   Les événements suivants se produisent :
   * Le but est maintenant ouvert et a un statut Principal.
   * La progression de l&#39;objectif est recalculée à partir de la date courante.
   * Toutes les notes de fermeture sont supprimées de la page Détails de l’objectif . Les notes de fermeture supprimées ne peuvent pas être récupérées.

1. (Facultatif) Modifiez à nouveau vos filtres pour n’afficher que les objectifs principaux.

   Les objectifs que vous avez ouverts s’affichent à l’écran.

