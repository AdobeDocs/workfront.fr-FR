---
product-previous: workfront-goals
navigation-topic: old-workfront-goals-articles
title: Suppression et désactivation d’objectifs dans les objectifs Adobe Workfront
description: Lorsque vous commencez à travailler sur un objectif qui n’a plus d’importance dans votre entreprise, nous vous recommandons de le désactiver au lieu de le supprimer. La désactivation d’un objectif conserve ses informations historiques et vous donne la possibilité de les réactiver ultérieurement. Cependant, il arrive que la suppression d’un objectif ait un sens, afin que votre liste d’objectifs reste précise.
author: Alina
feature: Workfront Goals
exl-id: 3089adeb-3e56-492a-82fe-536f57079b73
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '652'
ht-degree: 0%

---

# Suppression et désactivation d’objectifs dans les objectifs Adobe Workfront

Lorsque vous commencez à travailler sur un objectif qui n’a plus d’importance dans votre entreprise, nous vous recommandons de le désactiver au lieu de le supprimer. La désactivation d’un objectif conserve ses informations historiques et vous donne la possibilité de les réactiver ultérieurement. Cependant, il arrive que la suppression d’un objectif ait un sens, afin que votre liste d’objectifs reste précise.

## Exigences d’accès

<!--drafted for P&P release: 

You must have the following:

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

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Conditions préalables

Avant de pouvoir commencer, vous devez disposer des éléments suivants :

* Un modèle de mise en page qui inclut la zone Objectifs dans le menu principal.

## Désactivation des objectifs

Vous pouvez désactiver un objectif qui n’est plus pertinent et que vous souhaiterez peut-être réactiver à l’avenir.

* [Remarques concernant la désactivation des objectifs](#considerations-when-deactivating-goals)
* [Désactivation des objectifs](#deactivate-goals)

### Remarques concernant la désactivation des objectifs

Gardez à l’esprit les éléments suivants lors de la désactivation des objectifs :

* Vous pouvez uniquement désactiver les objectifs dans un état Principal. Pour plus d’informations sur l’activation d’un objectif, voir [Activation des objectifs dans les objectifs Adobe Workfront](../../workfront-goals/goal-management/activate-goals.md).

   >[!TIP]
   >
   >Vous ne pouvez pas désactiver les objectifs à l’état En création .

* Workfront arrête de calculer la progression des objectifs désactivés.
* Les objectifs inactifs ne s’affichent plus ou ne sont plus pris en compte dans la section Graphiques des objectifs Workfront. Pour plus d’informations sur les graphiques des objectifs de Workfront, voir [Consultez des graphiques pour comprendre les tendances de progression des objectifs dans les objectifs Adobe Workfront.](../../workfront-goals/goal-review-and-workfront-goals-sections/review-goal-graphs.md).

   <!--* The Check-in section. For information about the Check-in page, see [Update goal progress in Adobe Workfront Goals](../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md). -->

* Vous ne pouvez plus effectuer de mises à jour sur les objectifs désactivés.
* Vous pouvez modifier les informations relatives à l’objectif et à son alignement.
* Vous pouvez réactiver un objectif précédemment désactivé.

### Désactivation des objectifs

<!--
Deactivating goals differs depending on which environment you use.

### Deactivate goals in the Production environment


1. Go to the goal that you want to deactivate.

   For example, go to the Goal List and click the name of a goal.

   The Goal Details panel opens on the right.

   >[!TIP]
   >
   >You can open goals from any sections of Workfront Goals.

1. Click the **More icon** ![](assets/more-icon.png), then click **Deactivate**.

   ![](assets/deactivate-goal-highlighted.png)

   The goal status changes to Inactive. 

1. Click the **X** icon in the upper-right to close Goal Details.
-->

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit, puis cliquez sur **Objectifs**.

   La liste des objectifs s’affiche.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

1. (Facultatif) Modifiez vos filtres pour n’afficher que les objectifs principaux.

   Pour plus d’informations sur le filtrage des informations dans les objectifs Workfront, voir [Filtrage des informations dans les objectifs Adobe Workfront](../goal-management/filter-information-wf-goals.md).

1. Cliquez sur un principal objectif.

   La page d’objectif s’ouvre.

   ![](assets/goal-page-unshimmed.png)

1. Cliquez sur le bouton **Plus** menu ![](assets/more-icon.png) à droite du nom de l’objectif, puis cliquez sur **Désactiver**.

1. L’objectif est désactivé et son état devient inactif.

## Supprimer des objectifs

Vous pouvez supprimer des objectifs qui ne sont plus ou qui peuvent ne jamais être pertinents.

* [Remarques concernant la suppression d’objectifs](#considerations-when-deleting-goals)
* [Supprimer des objectifs](#delete-goals)

### Remarques concernant la suppression d’objectifs {#considerations-when-deleting-goals}

* Vous pouvez supprimer des objectifs dans n’importe quel état, y compris les objectifs fermés.
* Vous ne pouvez pas récupérer les objectifs supprimés.
* Les activités de barre de progression manuelle et de résultats associées à l’objectif sont également supprimées.
* Les projets associés aux objectifs ne sont pas supprimés, mais leur association à l’objectif est supprimée.

### Supprimer des objectifs

<!--
Deleting  goals differs depending on which environment you use.

#### Delete goals in the Production environment

1. Go to the goal that you want to delete.

   For example, go to the Goal List and click a goal.

   The Goal Details panel opens on the right. 

1. Click the **More icon** ![](assets/more-icon.png), then click **Delete**.

   ![](assets/delete-goal-highlighted.png)

1. Click **Yes, delete**.

   The goal is removed from the Goal List and cannot be recovered.
-->

1. Cliquez sur l’icône du menu principal ![](assets/main-menu-icon.png) dans le coin supérieur droit, puis cliquez sur **Objectifs**.

   La liste des objectifs s’affiche.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->
1. Cliquez sur le nom d’un objectif. Cela ouvre la page d’objectif.
1. Cliquez sur le bouton **Plus** menu ![](assets/more-icon.png) à droite du nom de l’objectif, puis cliquez sur **Supprimer l’objectif**, puis **Supprimer**.

   L’objectif, ses activités et ses résultats sont également supprimés et ne peuvent pas être récupérés. Les projets associés aux objectifs ou aux objectifs enfants ne sont pas supprimés.


