---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Supprimer des indicateurs de progression des objectifs dans Objectifs Adobe Workfront
description: Vous pouvez supprimer les résultats, les activités et les projets des objectifs d’Adobe Workfront, lorsqu’ils ne sont plus pertinents.
author: Alina
feature: Workfront Goals
exl-id: 0e064dbd-6168-47b4-98ab-b5c0481e839e
source-git-commit: 024c612d46848c55529e902a00d481588d261584
workflow-type: tm+mt
source-wordcount: '748'
ht-degree: 9%

---

# Supprimer des indicateurs de progression des objectifs dans Objectifs Adobe Workfront

<!-- for goal redesign PRODUCTION RELEASE: Should this article be called "Remove or disconnect progress indicators from goals" when this is available to ALL progress indicators (including "disconnect goals")-- if yes, updte the title everywhere else where this is linked?
-->

Vous pouvez supprimer les résultats, les activités et les projets des objectifs s’ils ne sont plus pertinents.

Pour plus d’informations sur la création d’objectifs et l’ajout de résultats et d’activités à ces objectifs, consultez les articles suivants :

* [Création d’objectifs dans les objectifs Adobe Workfront](../../workfront-goals/goal-management/create-goals.md)
* [Ajout d’activités aux objectifs dans les objectifs Adobe Workfront](../../workfront-goals/results-and-activities/add-activities-to-goals.md)
* [Ajout de résultats aux objectifs dans les objectifs Adobe Workfront](../../workfront-goals/results-and-activities/add-results-to-goals.md)
* [Modifier des résultats et des activités dans Objectifs Adobe Workfront](../../workfront-goals/results-and-activities/edit-results-and-activities.md)

Les objectifs peuvent également être alignés sur les objectifs parents, en devenant des objectifs enfants. Les objectifs pour les enfants sont également des indicateurs de progression des objectifs parents.

Vous pouvez supprimer l’alignement entre les objectifs en supprimant la connexion entre eux. Pour plus d’informations, voir [Suppression de l’alignement d’objectif dans les objectifs Adobe Workfront](../goal-alignment/remove-goal-alignment.md).

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
 <tr>
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

## Conditions préalables

Un objectif doit être associé aux résultats, aux activités ou aux projets.

## Considérations relatives à la suppression des résultats, des activités et de la déconnexion des projets des objectifs

* Vous ne pouvez supprimer des résultats et des activités que des objectifs actifs.
* Vous pouvez supprimer des résultats et des activités d’un objectif en les supprimant. Les résultats et activités supprimés ne peuvent pas être récupérés.
* Lorsque vous supprimez le résultat ou l’activité d’un objectif, la progression du résultat supprimé ou de l’activité affecte la progression globale de l’objectif.
* Vous ne pouvez pas supprimer un projet d’un objectif, mais vous pouvez le déconnecter de l’objectif. En déconnectant le projet de l’objectif, le pourcentage de réalisation du projet n’affecte plus la progression de l’objectif.

  Pour plus d’informations sur la manière dont les projets affectent la progression des objectifs, voir [Ajout de projets aux objectifs dans les objectifs Adobe Workfront](../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).

* Vous ne pouvez pas supprimer un résultat ou une activité d’un objectif et vous ne pouvez pas déconnecter un objectif ou un projet enfant, s’il s’agit du dernier indicateur de progression de l’objectif.
* Si un projet est supprimé de la zone Projets et qu’il s’agit du dernier indicateur de progression d’un objectif, l’objectif devient inactif.

## Supprimer des résultats et des activités des objectifs

Vous supprimez des résultats et des activités d’un objectif en les supprimant. La suppression des résultats et des activités d’un objectif est identique.

<!--
How you delete results and activities differs depending on the environment you use.

### Delete results and activities in the Production environment


1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   This opens the Workfront Goals area and the Goal List displays by default. 

1. Click the name of a goal you want to remove results and activities from.

   This opens the Goal Details panel on the right.

1. Click **Results** to remove results or **Activities** to remove activities. 

1. Click the **gear icon** ![](assets/settings-gear-icon.png) to the right of the result or activity name, then click **Delete** > **Yes, delete**.

   ![](assets/delete-result-goal-details-350x108.png)

   The result or activity is deleted and cannot be recovered. The percent complete of the goal updates to exclude the deleted activity or result.

-->

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit, puis cliquez sur **Objectifs**.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->
   Cela ouvre la zone Objectifs de Workfront et la Liste des objectifs s’affiche par défaut.

1. Cliquez sur le nom d’un objectif duquel vous souhaitez supprimer des résultats et des activités.

   Cela ouvre la page d’objectif.

1. Cliquez sur **Indicateurs de progression** dans le panneau de gauche.

1. Sélectionnez un résultat ou une activité, puis cliquez sur le bouton **Supprimer** icon ![](assets/delete-icon.png) en haut de la liste.

1. Cliquez sur **Supprimer** pour confirmer la suppression. Le résultat ou l&#39;activité est supprimé et ne peut pas être récupéré. Le pourcentage de fin de l’objectif est mis à jour pour exclure l’activité ou le résultat supprimé.


## Suppression de projets des objectifs

<!--
Dsconnecting projects from goals differs depending on the environment you use.

### Disconnect projects from goals in the Production environment


1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   This opens the Workfront Goals area and the Goal List displays by default. 

1. Click the name of a goal you want to remove results and activities from.

   This opens the Goal Details panel on the right.

1. Click the **right-pointing arrow** to the left of the Activities sections to expand it. 
1. Click the **gear icon** ![](assets/settings-gear-icon.png) to the right of the project name, then click **Disconnect**.

   ![](assets/disconnect-project-goal-details-350x94.png)

   The project is disconnected from the goal. The percent complete of the goal updates to exclude the percent complete of the disconnected project.
-->


1. Cliquez sur le bouton **Menu Principal** dans le coin supérieur droit, puis cliquez sur **Objectifs**.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   Cela ouvre la zone Objectifs de Workfront et la Liste des objectifs s’affiche par défaut.

1. Cliquez sur le nom d’un objectif duquel vous souhaitez supprimer des résultats et des activités.

   Cela ouvre la page d’objectif.
1. Cliquez sur **Indicateurs de progression** dans le panneau de gauche.
1. Sélectionnez un projet, puis cliquez sur le bouton **Déconnecter** icon ![](assets/disconnect-icon.png) en haut de la liste.
1. Cliquez sur **Déconnecter** pour confirmer.

   Le projet n’est plus connecté à l’objectif. Le pourcentage d’achèvement de l’objectif se met à jour pour exclure le projet déconnecté.

