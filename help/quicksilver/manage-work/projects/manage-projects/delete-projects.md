---
title: Suppression de projets
product-area: projects
navigation-topic: manage-projects
description: Vous pouvez supprimer un projet si celui-ci et ses données ne sont plus nécessaires.
author: Alina
feature: Work Management
exl-id: a0e80c4d-29a8-4bf8-aa19-0c2d493236c6
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '854'
ht-degree: 1%

---

# Suppression de projets

Vous pouvez supprimer un projet si celui-ci et ses données ne sont plus nécessaires.

Au lieu de supprimer un projet, nous vous recommandons de le modifier et de définir le statut Terminé ou Mort. Cette opération supprime de la liste des tâches d’un utilisateur toutes les tâches en cours liées au projet, mais enregistre toutes les données associées au projet.

## Exigences d’accès

<!-- drafted for P&P:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront plan*</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront license*</p> </td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Access level configurations*</strong> </td> 
   <td> <p>Edit access to Projects with ability to Create <span>and Delete</span> projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Object permissions</strong> </p> </td> 
   <td> <p>Edit access to Projects, Tasks,&nbsp;Issues with ability to Delete projects, tasks, and issues</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Les étapes de cet article doivent être les suivantes :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modifier l’accès aux projets, tâches, problèmes avec la possibilité de supprimer des projets, des tâches et des problèmes</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérez les autorisations liées au projet, aux tâches et aux problèmes du projet avec la possibilité de supprimer le projet, les tâches et les problèmes. </p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.
Vous pouvez supprimer un projet dans une liste de projets ou au niveau du projet.

## Comprendre le processus de suppression de projets

* [Restrictions relatives à la suppression de projets](#limitations-for-deleting-projects)
* [Impact de la suppression de projets](#the-impact-of-deleting-projects)

### Restrictions relatives à la suppression de projets  {#limitations-for-deleting-projects}

* Les éléments supprimés restent dans la Corbeille pendant 30 jours et ne peuvent être récupérés que par l’administrateur de Workfront.

   Pour plus d’informations sur la restauration d’objets, voir l’article [Restauration des éléments supprimés](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

* Si le projet comporte des tâches ou des problèmes avec les heures enregistrées, l’administrateur de Workfront ou de groupe doit autoriser la suppression de ces tâches en configurant les préférences de tâche et de problème dans votre instance Workfront pour que vous puissiez supprimer le projet qui contient les tâches.

   Pour plus d’informations sur l’activation de la suppression de tâches, de problèmes ou de projets pour lesquels des heures sont enregistrées, voir la section &quot;Suppression&quot; dans [Configuration des préférences de tâche et de problème à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Quicksilver,QuicksilverOrClassic.Draft mode">(NOTE: this bullet stays in NWE only forever)</p>
  -->

### Impact de la suppression de projets {#the-impact-of-deleting-projects}

* Lorsque vous supprimez un projet, vous avez un impact sur d’autres objets liés au projet.

   Les objets suivants associés à un projet sont également supprimés lorsque vous supprimez un projet :

   * Documents

      Vous ne pouvez pas supprimer un projet qui comporte un document joint qui a été extrait. Pour plus d’informations sur l’extraction de documents, voir [Extraction de documents](../../../documents/managing-documents/check-out-documents.md).

   * Tâches
   * Sous-tâches
   * Événements
   * Notes
   * Approbations
   * Frais

* Selon la manière dont votre administrateur Workfront configure les préférences Projet, Tâche ou Suppression de problème dans la feuille de temps et les préférences Heure de votre instance Workfront, les heures consignées pour les tâches, les problèmes ou le projet sont gérées de l’une des manières suivantes lors de la suppression du projet :

   * Les heures restent sur la feuille de temps comme heure générale.
   * Les heures sont supprimées et seront restaurées si le projet est un jour restauré.

   Pour plus d’informations sur la configuration des préférences de suppression pour les heures de connexion aux problèmes, voir [Configuration des préférences de feuille de temps et d’heure](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

* Si le projet que vous supprimez est lié à une initiative dans le planificateur de scénario Workfront :

   * L&#39;initiative reste sur le plan, mais le lien vers le projet est supprimé.
   * Si le projet que vous supprimez est lié à la seule initiative publiée d’un plan, l’indication que le plan a été publié est également supprimée.
   * Si vous récupérez un projet supprimé, le projet est récupéré, mais son lien avec l’initiative n’est pas restauré et la zone du planificateur de scénario ne s’affiche plus dans les détails du projet.

      Le planificateur de scénario n’est disponible que dans la nouvelle expérience Adobe Workfront et nécessite une licence supplémentaire. Pour plus d’informations sur le planificateur de scénario Workfront, voir [Présentation du planificateur de scénarios](../../../scenario-planner/scenario-planner-overview.md).

      Pour plus d’informations sur les projets liés aux initiatives dans le planificateur de scénario, voir [Mettre à jour ou créer des projets en publiant des initiatives dans le planificateur de scénarios](../../../scenario-planner/publish-scenarios-update-projects.md).

* Si le projet est également une activité pour un objectif dans les objectifs de Workfront :

   * Le projet est supprimé de l’objectif. La progression indiquée sur l’objectif par le projet est également supprimée.

   * Si vous récupérez le projet supprimé, le projet est également restauré en tant qu’activité de l’objectif.

      Cela nécessite une licence supplémentaire. Pour plus d’informations sur les objectifs de Workfront, voir [Présentation des objectifs d’Adobe Workfront](../../../workfront-goals/goal-management/wf-goals-overview.md).

      Pour plus d’informations sur l’association de projets à des objectifs, voir [Ajout de projets aux objectifs dans les objectifs Adobe Workfront](../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).

## Supprimer un projet dans une liste

Vous pouvez supprimer des projets d’une liste de projets.

1. Accédez à une liste de projets ou à un rapport de projet.
1. Sélectionnez le projet à supprimer, puis cliquez sur **Supprimer** en haut de la liste.

1. Cliquez sur **Oui, la supprimer** pour confirmer la suppression.

   Le projet est supprimé et stocké dans la Corbeille pendant 30 jours. Votre administrateur Workfront peut le restaurer à partir de la Corbeille pendant cette période.

## Suppression d’un projet au niveau du projet

1. Accédez au projet que vous souhaitez supprimer.
1. Cliquez sur le bouton **Plus** icon ![](assets/qs-more-menu.png).

1. Cliquez sur **Supprimer le projet**.

1. Cliquez sur **Oui, supprimez-le**.

   Le projet est supprimé et stocké dans la Corbeille pendant 30 jours. Votre administrateur Workfront peut le restaurer à partir de la Corbeille pendant cette période.

## Restauration des projets supprimés

Un administrateur système ou de groupe peut restaurer les projets dans les 30 jours suivant leur suppression, comme décrit dans l’article . [Restauration des éléments supprimés](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).
