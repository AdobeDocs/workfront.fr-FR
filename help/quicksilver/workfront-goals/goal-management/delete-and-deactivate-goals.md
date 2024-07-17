---
product-previous: workfront-goals
navigation-topic: old-workfront-goals-articles
title: Supprimer et désactiver des objectifs dans Objectifs Adobe Workfront
description: Lorsque vous commencez à travailler sur un objectif qui n’a plus d’importance dans votre entreprise, nous vous recommandons de le désactiver au lieu de le supprimer. La désactivation d’un objectif conserve ses informations historiques et vous donne la possibilité de les réactiver ultérieurement. Cependant, il arrive que la suppression d’un objectif ait un sens, afin que votre liste d’objectifs reste précise.
author: Alina
feature: Workfront Goals
exl-id: 3089adeb-3e56-492a-82fe-536f57079b73
source-git-commit: 024c612d46848c55529e902a00d481588d261584
workflow-type: tm+mt
source-wordcount: '684'
ht-degree: 11%

---

# Supprimer et désactiver des objectifs dans Objectifs Adobe Workfront

Lorsque vous commencez à travailler sur un objectif qui n’a plus d’importance dans votre entreprise, nous vous recommandons de le désactiver au lieu de le supprimer. La désactivation d’un objectif conserve ses informations historiques et vous donne la possibilité de les réactiver ultérieurement. Cependant, il arrive que la suppression d’un objectif ait un sens, afin que votre liste d’objectifs reste précise.

## Conditions d’accès

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
 <td role="rowheader"><p>Niveau d’accès</p></td>
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
   <td role="rowheader"><p>Modèle de disposition</p></td>
   <td> <p>Tous les utilisateurs, y compris les administrateurs de Workfront, doivent se voir attribuer un modèle de mise en page incluant la zone Objectifs dans le menu principal. </p>  
</td>
  </tr>
</tbody>
</table>

*Pour plus d’informations, voir [Conditions d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Désactivation des objectifs

Vous pouvez désactiver un objectif qui n’est plus pertinent et que vous souhaiterez peut-être réactiver à l’avenir.

* [Remarques concernant la désactivation des objectifs](#considerations-when-deactivating-goals)
* [Désactivation des objectifs](#deactivate-goals)

### Remarques concernant la désactivation des objectifs

Gardez à l’esprit les éléments suivants lors de la désactivation des objectifs :

* Vous pouvez uniquement désactiver les objectifs à l’état Actif . Pour plus d’informations sur l’activation d’un objectif, voir [Activation des objectifs dans les objectifs Adobe Workfront](../../workfront-goals/goal-management/activate-goals.md).

  >[!TIP]
  >
  >Vous ne pouvez pas désactiver les objectifs à l’état En création .

* Workfront arrête de calculer la progression des objectifs désactivés.
* Les objectifs inactifs ne s’affichent plus ou ne sont plus pris en compte dans la section Graphiques des objectifs Workfront. Pour plus d’informations sur les graphiques des objectifs de Workfront, voir [Révision des graphiques pour comprendre les tendances de progression des objectifs dans les objectifs Adobe Workfront](../../workfront-goals/goal-review-and-workfront-goals-sections/review-goal-graphs.md).

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

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit, puis sur **Objectifs**.

   La liste des objectifs s’affiche.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

1. (Facultatif) Modifiez vos filtres pour n’afficher que les objectifs actifs.

   Pour plus d’informations sur le filtrage des informations dans les objectifs Workfront, voir [Filtrage des informations dans les objectifs Adobe Workfront](../goal-management/filter-information-wf-goals.md).

1. Cliquez sur un objectif actif.

   La page d’objectif s’ouvre.

   ![](assets/goal-page-unshimmed.png)

1. Cliquez sur le menu **Plus** ![](assets/more-icon.png) situé à droite du nom de l’objectif, puis cliquez sur **Désactiver**.

1. L’objectif est désactivé et son état devient inactif.

## Supprimer des objectifs

Vous pouvez supprimer des objectifs qui ne sont plus ou qui peuvent ne jamais être pertinents.

* [Considérations relatives à la suppression d’objectifs](#considerations-when-deleting-goals)
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

1. Cliquez sur l’icône du menu principal ![](assets/main-menu-icon.png) dans le coin supérieur droit, puis sur **Objectifs**.

   La liste des objectifs s’affiche.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->
1. Cliquez sur le nom d’un objectif. Cela ouvre la page d’objectif.
1. Cliquez sur le menu **Plus** ![](assets/more-icon.png) situé à droite du nom de l’objectif, puis cliquez sur **Supprimer l’objectif**, puis sur **Supprimer**.

   L’objectif, ses activités et ses résultats sont également supprimés et ne peuvent pas être récupérés. Les projets associés aux objectifs ou aux objectifs enfants ne sont pas supprimés.


