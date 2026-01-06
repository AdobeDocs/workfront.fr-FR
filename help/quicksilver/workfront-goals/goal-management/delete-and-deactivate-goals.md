---
product-previous: workfront-goals
navigation-topic: old-workfront-goals-articles
title: Supprimer et désactiver les objectifs dans Adobe Workfront Objectifs
description: Lorsque vous commencez à travailler sur un objectif et qu’il n’est plus pertinent pour votre organisation, nous vous recommandons de le désactiver au lieu de le supprimer. La désactivation d’un objectif permet de conserver son historique et vous donne la possibilité de le réactiver ultérieurement. Cependant, il peut arriver que la suppression d’un objectif soit judicieuse, afin que votre liste d’objectifs reste exacte.
author: Alina
feature: Workfront Goals
exl-id: 3089adeb-3e56-492a-82fe-536f57079b73
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '590'
ht-degree: 81%

---

# Supprimer et désactiver des objectifs dans Objectifs Adobe Workfront

<!--Audited for P&P only: 10/2025-->

Lorsque vous commencez à travailler sur un objectif et qu’il n’est plus pertinent pour votre organisation, nous vous recommandons de le désactiver au lieu de le supprimer. La désactivation d’un objectif permet de conserver son historique et vous donne la possibilité de le réactiver ultérieurement. Cependant, il peut arriver que la suppression d’un objectif soit judicieuse, afin que votre liste d’objectifs reste exacte.

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

1. Click the **More icon** ![More icon](assets/more-icon.png), then click **Deactivate**.

   ![Deactivate goal](assets/deactivate-goal-highlighted.png)

   The goal status changes to Inactive. 

1. Click the **X** icon in the upper-right to close Goal Details.
-->

{{step1-to-goals}}

La liste des objectifs s’affiche.


1. (Facultatif) Modifiez vos filtres pour n’afficher que les objectifs actifs.

   Pour plus d’informations sur le filtrage des informations dans les Objectifs Workfront, voir [Filtrer des informations dans les Objectifs Adobe Workfront](../goal-management/filter-information-wf-goals.md).

1. Cliquez sur un objectif actif.

   La page de l’objectif s’ouvre.

   ![Page d’objectif](assets/goal-page-unshimmed.png)

1. Cliquez sur le menu **Plus** ![Icône Plus](assets/more-icon.png) à droite du nom de l’objectif, puis cliquez sur **Désactiver**.

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

1. Click the **More icon** ![More icon](assets/more-icon.png), then click **Delete**.

   ![Delete goal](assets/delete-goal-highlighted.png)

1. Click **Yes, delete**.

   The goal is removed from the Goal List and cannot be recovered.
-->

{{step1-to-goals}}

La liste des objectifs s’affiche.

1. Cliquez sur le nom d’un objectif. La page de l’objectif s’ouvre.
1. Cliquez sur le menu **Plus** ![Icône Plus](assets/more-icon.png) à droite du nom de l’objectif, puis cliquez sur **Supprimer l’objectif** et **Supprimer**.

   L’objectif, ses activités et ses résultats sont également supprimés et ne peuvent pas être récupérés. Les projets associés à l’objectif ou aux objectifs enfants ne sont pas supprimés.


