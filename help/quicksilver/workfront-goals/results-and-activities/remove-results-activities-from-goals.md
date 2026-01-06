---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Suppression des indicateurs de progression des objectifs dans Objectfs Adobe Workfront
description: Vous pouvez supprimer les résultats, les activités et les projets dans Objectifs Adobe Workfront, lorsqu’ils ne sont plus pertinents.
author: Alina
feature: Workfront Goals
exl-id: 0e064dbd-6168-47b4-98ab-b5c0481e839e
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '646'
ht-degree: 85%

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

Pour plus d’informations, consultez la section [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
 <td role="rowheader">Adobe Workfront license*</td>
 <td>
 <p>New license: Contributor or higher</p>
 Or
 <p>Current license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Product*</td>
 <td>
 <p> New product requirement, one of the following: </p>
<ul>
<li>A Select or Prime Adobe Workfront plan and an additional Adobe Workfront Goals license.</li>
<li>An Ultimate Workfront plan which includes Workfront Goals by default. </li></ul>
 <p>Or</p>
 <p>Current product requirement: A Workfront plan and an additional license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
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

{{step1-to-goals}}

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


{{step1-to-goals}}

Cela ouvre la zone Objectifs Workfront et la Liste des objectifs s’affiche par défaut.

1. Cliquez sur le nom d’un objectif duquel vous souhaitez supprimer des résultats et des activités.

   La page de l’objectif s’ouvre.
1. Cliquez sur **Indicateurs de progression** dans le panneau de gauche.
1. Sélectionnez un projet, puis cliquez sur l’icône **Déconnecter** ![Icône Déconnecter](assets/disconnect-icon.png) en haut de la liste.
1. Cliquez sur **Déconnecter** pour confirmer.

   Le projet n’est plus connecté à l’objectif. Le pourcentage terminé de l’objectif se met à jour pour exclure le projet déconnecté.

