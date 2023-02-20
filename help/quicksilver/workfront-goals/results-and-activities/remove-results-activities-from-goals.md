---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Suppression des indicateurs de progression des objectifs dans les objectifs Adobe Workfront
description: Vous pouvez supprimer les résultats, les activités et les projets des objectifs d’Adobe Workfront, lorsqu’ils ne sont plus pertinents.
author: Alina
feature: Workfront Goals
exl-id: 0e064dbd-6168-47b4-98ab-b5c0481e839e
source-git-commit: fb538c6511514eedf81f4b9be452d5f87e3f7577
workflow-type: tm+mt
source-wordcount: '703'
ht-degree: 0%

---

# Suppression des indicateurs de progression des objectifs dans les objectifs Adobe Workfront

<!-- for goal redesign PRODUCTION RELEASE: Should this article be called "Remove or disconnect progress indicators from goals" when this is available to ALL progress indicators (including "disconnect goals")-- if yes, updte the title everywhere else where this is linked?
-->

Vous pouvez supprimer les résultats, les activités et les projets des objectifs s’ils ne sont plus pertinents.

Pour plus d’informations sur la création d’objectifs et l’ajout de résultats et d’activités à ces objectifs, consultez les articles suivants :

* [Création d’objectifs dans les objectifs Adobe Workfront](../../workfront-goals/goal-management/create-goals.md)
* [Ajout d’activités aux objectifs dans les objectifs Adobe Workfront](../../workfront-goals/results-and-activities/add-activities-to-goals.md)
* [Ajout de résultats aux objectifs dans les objectifs Adobe Workfront](../../workfront-goals/results-and-activities/add-results-to-goals.md)
* [Modification des résultats et des activités dans les objectifs Adobe Workfront](../../workfront-goals/results-and-activities/edit-results-and-activities.md)

Les objectifs peuvent également être alignés sur les objectifs parents, en devenant des objectifs enfants. Les objectifs pour les enfants sont également des indicateurs de progression des objectifs parents.

Vous pouvez supprimer l’alignement entre les objectifs en supprimant la connexion entre eux. Pour plus d’informations, voir [Suppression de l’alignement d’objectif dans les objectifs Adobe Workfront](../goal-alignment/remove-goal-alignment.md).

## Exigences d’accès

<!--drafted - replace the table below with this one when P&P releases: 

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

*Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Conditions préalables

Avant de pouvoir commencer, vous devez disposer des éléments suivants :

* Un modèle de mise en page qui inclut la zone Objectifs dans le menu principal.
* Objectif avec des résultats, des activités ou des projets.

## Considérations relatives à la suppression des résultats, des activités et de la déconnexion des projets des objectifs

* Vous ne pouvez supprimer des résultats et des activités que des objectifs principaux.
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

