---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Suppression des indicateurs de progression des objectifs dans Objectfs Adobe Workfront
description: Vous pouvez supprimer les résultats, les activités et les projets dans Objectifs Adobe Workfront, lorsqu’ils ne sont plus pertinents.
author: Alina
feature: Workfront Goals
exl-id: 0e064dbd-6168-47b4-98ab-b5c0481e839e
source-git-commit: 45c71a8106bdb8eeaa38f2fb83ff0312e48183d0
workflow-type: tm+mt
source-wordcount: '739'
ht-degree: 93%

---

# Suppression des indicateurs de progression des objectifs dans Objectfs Adobe Workfront

<!-- for goal redesign PRODUCTION RELEASE: Should this article be called "Remove or disconnect progress indicators from goals" when this is available to ALL progress indicators (including "disconnect goals")-- if yes, updte the title everywhere else where this is linked?
-->

Vous pouvez supprimer les résultats, les activités et les projets des objectifs s’ils ne sont plus pertinents.

Pour plus d’informations sur la création d’objectifs et l’ajout de résultats et d’activités à ces objectifs, consultez les articles suivants :

* [Créer des objectifs dans Objectifs Adobe Workfront](../../workfront-goals/goal-management/create-goals.md)
* [Ajout d’activités aux objectifs dans Objectifs Adobe Workfront](../../workfront-goals/results-and-activities/add-activities-to-goals.md)
* [Ajout de résultats aux objectifs dans Objectifs Adobe Workfront](../../workfront-goals/results-and-activities/add-results-to-goals.md)
* [Modification des résultats et des activités dans Objectifs Adobe Workfront](../../workfront-goals/results-and-activities/edit-results-and-activities.md)

Les objectifs peuvent également être alignés sur les objectifs parents et devenir des objectifs enfants. Les objectifs enfants sont également des indicateurs de progression des objectifs parents.

Vous pouvez supprimer l’alignement entre les objectifs en supprimant la connexion entre eux. Pour plus d’informations, consultez [Supprimer l’alignement d’objectif dans Objectifs Adobe Workfront](../goal-alignment/remove-goal-alignment.md).

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
 <p>Licence actuelle : demande ou niveau supérieur</p> <p>Pour plus d’informations, voir <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Vue d’ensemble des licences Adobe Workfront</a>.</p> </td>
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
 <td role="rowheader">Niveau d’accès</td>
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

## Conditions préalables

Un objectif doit être associé à des résultats, des activités ou des projets.

## Considérations relatives à la suppression des résultats, des activités et de la déconnexion des projets des objectifs

* Vous ne pouvez supprimer des résultats et des activités que des objectifs actifs.
* Vous pouvez supprimer des résultats et des activités d’un objectif en les supprimant. Les résultats et activités supprimés ne peuvent pas être récupérés.
* Lorsque vous supprimez le résultat ou l’activité d’un objectif, la progression du résultat ou de l’activité supprimé affecte la progression globale de l’objectif.
* Vous ne pouvez pas supprimer un projet d’un objectif, mais vous pouvez le déconnecter de l’objectif. En déconnectant le projet de l’objectif, le pourcentage d’achèvement du projet n’affecte plus la progression de l’objectif.

  Pour plus d’informations sur la manière dont les projets affectent la progression des objectifs, consultez [Ajouter des projets aux objectifs dans Objectifs Adobe Workfront](../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).

* Vous ne pouvez pas supprimer un résultat ou une activité d’un objectif et vous ne pouvez pas déconnecter un objectif ou un projet enfant s’il s’agit du dernier indicateur de progression de l’objectif.
* Si un projet est supprimé de la zone Projets et qu’il s’agit du dernier indicateur de progression d’un objectif, l’objectif devient inactif.

## Supprimer des résultats et des activités des objectifs

Vous supprimez des résultats et des activités d’un objectif en les supprimant. La suppression des résultats et des activités d’un objectif est identique.

<!--
How you delete results and activities differs depending on the environment you use.

### Delete results and activities in the Production environment


1. Click the **Main Menu** icon ![Main Menu icon](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   This opens the Workfront Goals area and the Goal List displays by default. 

1. Click the name of a goal you want to remove results and activities from.

   This opens the Goal Details panel on the right.

1. Click **Results** to remove results or **Activities** to remove activities. 

1. Click the **gear icon** ![Gear icon](assets/settings-gear-icon.png) to the right of the result or activity name, then click **Delete** > **Yes, delete**.

   ![Delete result](assets/delete-result-goal-details-350x108.png)

   The result or activity is deleted and cannot be recovered. The percent complete of the goal updates to exclude the deleted activity or result.

-->

1. Cliquez sur l’icône **Menu principal** ![icône du menu principal](assets/main-menu-icon.png) dans le coin supérieur droit, puis cliquez sur **Objectifs**.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->
   Cela ouvre la zone Objectifs Workfront et la Liste des objectifs s’affiche par défaut.

1. Cliquez sur le nom d’un objectif duquel vous souhaitez supprimer des résultats et des activités.

   La page de l’objectif s’ouvre.

1. Cliquez sur **Indicateurs de progression** dans le panneau de gauche.

1. Sélectionnez un résultat ou une activité, puis cliquez sur l&#39;icône **Supprimer** ![Icône Supprimer](assets/delete-icon.png) en haut de la liste.

1. Cliquez sur **Supprimer** pour confirmer la suppression. Le résultat ou l’activité est supprimé et ne peut pas être récupéré. Le pourcentage terminé de l’objectif est mis à jour pour exclure l’activité ou le résultat supprimé.


## Supprimer des projets dans des objectifs

<!--
Dsconnecting projects from goals differs depending on the environment you use.

### Disconnect projects from goals in the Production environment


1. Click the **Main Menu** icon ![Main Menu icon](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   This opens the Workfront Goals area and the Goal List displays by default. 

1. Click the name of a goal you want to remove results and activities from.

   This opens the Goal Details panel on the right.

1. Click the **right-pointing arrow** to the left of the Activities sections to expand it. 
1. Click the **gear icon** ![Gear icon](assets/settings-gear-icon.png) to the right of the project name, then click **Disconnect**.

   ![Disconnect](assets/disconnect-project-goal-details-350x94.png)

   The project is disconnected from the goal. The percent complete of the goal updates to exclude the percent complete of the disconnected project.
-->


1. Cliquez sur l’icône **Menu Principal** dans le coin supérieur droit, puis cliquez sur **Objectifs**.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   Cela ouvre la zone Objectifs Workfront et la Liste des objectifs s’affiche par défaut.

1. Cliquez sur le nom d’un objectif duquel vous souhaitez supprimer des résultats et des activités.

   La page de l’objectif s’ouvre.
1. Cliquez sur **Indicateurs de progression** dans le panneau de gauche.
1. Sélectionnez un projet, puis cliquez sur l’icône **Déconnecter** ![Icône Déconnecter](assets/disconnect-icon.png) en haut de la liste.
1. Cliquez sur **Déconnecter** pour confirmer.

   Le projet n’est plus connecté à l’objectif. Le pourcentage terminé de l’objectif se met à jour pour exclure le projet déconnecté.

