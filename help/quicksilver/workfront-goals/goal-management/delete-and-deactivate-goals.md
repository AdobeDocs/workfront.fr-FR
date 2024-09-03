---
product-previous: workfront-goals
navigation-topic: old-workfront-goals-articles
title: Supprimer et désactiver des objectifs dans Objectifs Adobe Workfront
description: Lorsque vous commencez à travailler sur un objectif et qu’il n’est plus pertinent pour votre organisation, nous vous recommandons de le désactiver au lieu de le supprimer. La désactivation d’un objectif permet de conserver son historique et vous donne la possibilité de le réactiver ultérieurement. Cependant, il peut arriver que la suppression d’un objectif soit judicieuse, afin que votre liste d’objectifs reste exacte.
author: Alina
feature: Workfront Goals
exl-id: 3089adeb-3e56-492a-82fe-536f57079b73
source-git-commit: d7dd5ab4e3041a100b13c5bf169747f58db0ea39
workflow-type: tm+mt
source-wordcount: '668'
ht-degree: 100%

---

# Supprimer et désactiver des objectifs dans Objectifs Adobe Workfront

Lorsque vous commencez à travailler sur un objectif et qu’il n’est plus pertinent pour votre organisation, nous vous recommandons de le désactiver au lieu de le supprimer. La désactivation d’un objectif permet de conserver son historique et vous donne la possibilité de le réactiver ultérieurement. Cependant, il peut arriver que la suppression d’un objectif soit judicieuse, afin que votre liste d’objectifs reste exacte.

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
 <p> Nouvelle exigence de produit, une des options suivantes : </p>
<ul>
<li>Un forfait Adobe Workfront Select ou Prime et une licence Objectifs Adobe Workfront supplémentaire.</li>
<li>Un forfait Workfront Ultimate qui inclut Objectifs Workfront par défaut. </li></ul>
 <p>Ou</p>
 <p>Exigence de produit actuelle : un forfait Workfront et une licence supplémentaire pour Objectifs Adobe Workfront. </p> <p>Pour plus d’informations, consultez la section <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Exigences pour l’utilisation des Objectifs Workfront</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader"><p>Niveau d’accès</p></td>
 <td> <p>Modifier l’accès aux Objectifs</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Autorisations d’objet</td>
 <td>
  <div>
  <p>Autorisations d’affichage ou de niveau supérieur sur l’objectif pour l’afficher</p>
  <p>Autorisations de gestion sur l’objectif pour le modifier</p>
  <p>Pour plus d’informations sur le partage des objectifs, voir <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Partager un objectif dans Objectifs Workfront</a>. </p>
  </div> </td>
 </tr>
 <tr>
   <td role="rowheader"><p>Modèle de mise en page</p></td>
   <td> <p>Toutes les personnes, y compris les administrateurs et administratrices Workfront, doivent se voir attribuer un modèle de mise en page incluant la zone Objectifs dans le menu principal. </p>  
</td>
  </tr>
</tbody>
</table>

*Pour plus d’informations, voir [Conditions d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Désactiver des objectifs

Vous pouvez désactiver un objectif qui n’est plus pertinent et que vous souhaiterez peut-être réactiver à l’avenir.

* [Points à prendre en compte lors de la désactivation des objectifs](#considerations-when-deactivating-goals)
* [Désactiver des objectifs](#deactivate-goals)

### Points à prendre en compte lors de la désactivation des objectifs

N’oubliez pas les points suivants lorsque vous désactivez des objectifs :

* Vous ne pouvez désactiver que les objectifs ayant un statut actif. Pour plus d’informations sur l’activation d’un objectif, voir [Activer des objectifs dans Objectifs Adobe Workfront](../../workfront-goals/goal-management/activate-goals.md).

  >[!TIP]
  >
  >Vous ne pouvez pas désactiver les objectifs ayant un statut Brouillon.

* Workfront arrête de calculer la progression des objectifs désactivés.
* Les objectifs inactifs ne s’affichent plus et ne sont plus pris en compte dans la section Graphiques d’Objectifs Workfront. Pour plus d’informations sur les graphiques d’Objectifs Workfront, voir [Réviser des graphiques pour comprendre les tendances de progression des objectifs dans Objectifs Adobe Workfront](../../workfront-goals/goal-review-and-workfront-goals-sections/review-goal-graphs.md).

  <!--* The Check-in section. For information about the Check-in page, see [Update goal progress in Adobe Workfront Goals](../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md). -->

* Vous ne pouvez plus effectuer de mises à jour sur les objectifs désactivés.
* Vous pouvez modifier les informations relatives à l’objectif et à son alignement.
* Vous pouvez réactiver un objectif précédemment désactivé.

### Désactiver des objectifs

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

   Pour plus d’informations sur le filtrage des informations dans les Objectifs Workfront, voir [Filtrer des informations dans les Objectifs Adobe Workfront](../goal-management/filter-information-wf-goals.md).

1. Cliquez sur un objectif actif.

   La page de l’objectif s’ouvre.

   ![](assets/goal-page-unshimmed.png)

1. Cliquez sur le menu **Plus** ![](assets/more-icon.png) à droite du nom de l’objectif, puis cliquez sur **Désactiver**.

1. L’objectif est désactivé et son statut devient inactif.

## Supprimer des objectifs

Vous pouvez supprimer les objectifs qui ne sont plus pertinents ou qui pourraient ne jamais l’être.

* [Points à prendre en compte lors de la suppression d’objectifs](#considerations-when-deleting-goals)
* [Supprimer des objectifs](#delete-goals)

### Points à prendre en compte lors de la suppression d’objectifs {#considerations-when-deleting-goals}

* Vous pouvez supprimer des objectifs quel que soit leur statut, y compris des objectifs clôturés.
* Vous ne pouvez pas récupérer les objectifs supprimés.
* Les résultats et les activités de la barre de progression manuelle liés à l’objectif sont également supprimés.
* Les projets associés à des objectifs ne sont pas supprimés, mais leur association avec l’objectif en question est supprimée.

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
1. Cliquez sur le nom d’un objectif. La page de l’objectif s’ouvre.
1. Cliquez sur le menu **Plus** ![](assets/more-icon.png) à droite du nom de l’objectif, puis cliquez sur **Supprimer l’objectif**, puis sur **Supprimer**.

   L’objectif, ses activités et ses résultats sont également supprimés et ne peuvent pas être récupérés. Les projets associés à l’objectif ou aux objectifs enfants ne sont pas supprimés.


