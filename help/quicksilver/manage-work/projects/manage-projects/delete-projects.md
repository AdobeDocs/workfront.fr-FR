---
title: Supprimer projets
product-area: projects
navigation-topic: manage-projects
description: Vous pouvez supprimer un projet si celui-ci et ses données ne sont plus nécessaires. Au lieu de supprimer un projet, nous vous recommandons de le modifier et de changer son statut sur Terminé ou Inactif. Cette opération supprime de la liste de tâches d’un utilisateur ou d’une utilisatrice toutes les tâches en cours liées au projet, mais enregistre toutes les données qui y sont associées.
author: Alina
feature: Work Management
exl-id: a0e80c4d-29a8-4bf8-aa19-0c2d493236c6
recommendations: noDisplay, noCatalog
source-git-commit: ba5089fd02ca099d25ce0d3c2c2c039c2c6e2fe2
workflow-type: tm+mt
source-wordcount: '1067'
ht-degree: 79%

---

# Supprimer des projets

<!--Audited: 07/2024-->

Vous pouvez supprimer un projet si celui-ci et ses données ne sont plus nécessaires.

Au lieu de supprimer un projet, nous vous recommandons de le modifier et de changer son statut sur Terminé ou Inactif. Cette opération supprime de la liste de tâches d’un utilisateur ou d’une utilisatrice toutes les tâches en cours liées au projet, mais enregistre toutes les données qui y sont associées.

Vous pouvez supprimer un projet dans une liste de projets ou au niveau du projet.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Package Adobe Workfront</p> </td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td> <p>Licence Adobe Workfront</p> </td> 
   <td> <p>Standard</p>
   <p>Plan</p> 
   </td> 
  </tr> 
    <td>Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès aux projets avec la possibilité de créer et de supprimer des projets</p> </td> 
  </tr> 
    <td> <p>Autorisations d’objet</p> </td> 
   <td> <p>Modifier l’accès aux projets, tâches et problèmes avec la possibilité de supprimer des projets, des tâches et des problèmes</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront plan</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront license*</p> </td> 
   <td> <p>New license: Standard </p>
   <p>Current license: Plan </p> 
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Access level configuration</td> 
   <td> <p>Edit access to Projects with ability to Create and Delete projects</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Object permissions </p> </td> 
   <td> <p>Edit access to Projects, Tasks, Issues with ability to Delete projects, tasks, and issues</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Comprendre le processus de suppression de projets

* [Restrictions relatives à la suppression de projets](#limitations-for-deleting-projects)
* [Impact de la suppression de projets](#the-impact-of-deleting-projects)

### Limites de suppression de projets  {#limitations-for-deleting-projects}

* Les éléments supprimés seront déplacés vers la Corbeille pendant 30 jours et ne pourront être récupérés que par l’administrateur ou administratrice système.

  Pour plus d’informations sur la restauration d’objets, voir l’article [Restaurer des éléments supprimés](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

* Si le projet a des tâches ou des problèmes avec des heures consignées, l’administrateur ou administratrice Workfront ou de groupes doit autoriser la suppression de ces tâches en configurant les préférences de tâches et de problèmes dans votre instance Workfront pour que vous puissiez supprimer le projet qui contient les tâches.

  Pour plus d’informations sur l’activation de la suppression de tâches, de problèmes ou de projets pour lesquels des heures sont consignées, voir la section « Suppression » dans [Configurer les préférences de tâches et de problèmes à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Quicksilver,QuicksilverOrClassic.Draft mode">(NOTE: this bullet stays in NWE only forever)</p>
  -->

### Impact de la suppression de projets {#the-impact-of-deleting-projects}

* La suppression d’un projet a un impact sur les autres objets liés à ce projet.

  Les objets suivants associés à un projet sont également supprimés lorsque vous supprimez un projet :

   * Documents

     Vous ne pouvez pas supprimer un projet auquel est joint un document qui a été extrait. Pour plus d’informations sur l’extraction de documents, voir [Extraire des documents](../../../documents/managing-documents/check-out-documents.md).

   * Tâches
   * Sous-tâches
   * Problèmes
   * Mises à jour
   * Approbations
   * Frais
   * Risques
   * Niveaux de référence
   * Informations sur le business case
   * Informations sur les détails de la file d’attente
   * Taux de facturation
   * Enregistrements de facturation

     Vous ne pouvez pas supprimer un projet dont le statut est Facturé pour les enregistrements de facturation. Pour plus d’informations, voir [Créer des enregistrements de facturation](../../projects/project-finances/create-billing-records.md).

* Selon la manière dont votre administrateur ou administratrice Workfront configure les préférences de suppression de projet, tâche ou problème dans les préférences de feuilles de temps et heures de votre instance Workfront, les heures enregistrées pour les tâches, les problèmes ou le projet sont traitées de l’une des manières suivantes lors de la suppression du projet :

   * Les heures restent sur la feuille de temps comme heures générales.
   * Les heures sont supprimées et seront restaurées si le projet est un jour restauré.

  Pour plus d’informations sur la configuration des préférences de suppression pour les heures enregistrées relatives aux problèmes, voir [Configurer des préférences de feuille de temps et heures](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

* Si le projet que vous supprimez est lié à une initiative dans le planificateur de scénarios Workfront :

   * L’initiative reste sur le plan, mais le lien vers le projet est supprimé.
   * Si le projet que vous supprimez est lié à la seule initiative publiée d’un plan, l’indication que le plan a été publié est également supprimée.
   * Si vous récupérez un projet supprimé, le projet est récupéré, mais son lien avec l’initiative n’est pas restauré et la zone du planificateur de scénarios ne s’affiche plus dans les détails du projet.

     Le planificateur de scénarios nécessite une licence supplémentaire. Pour plus d’informations sur le planificateur de scénarios Workfront, voir [Vue d’ensemble du planificateur de scénarios](../../../scenario-planner/scenario-planner-overview.md).

     Pour plus d’informations sur les projets liés aux initiatives dans le planificateur de scénarios, voir [Mettre à jour ou créer des projets en publiant des initiatives dans le planificateur de scénarios](../../../scenario-planner/publish-scenarios-update-projects.md).

* Si le projet est également une activité pour un objectif dans les Objectifs Workfront :

   * Le projet est supprimé de l’objectif. La progression indiquée sur l’objectif par le projet est également supprimée.

   * Si vous récupérez le projet supprimé, le projet est également restauré en tant qu’activité de l’objectif.

     Cela nécessite une licence supplémentaire. Pour plus d’informations sur les Objectifs Workfront, voir [Vue d’ensemble des Objectifs Adobe Workfront](../../../workfront-goals/goal-management/wf-goals-overview.md).

     Pour plus d’informations sur l’association de projets à des objectifs, voir [Ajouter des projets aux objectifs dans les Objectifs Adobe Workfront](../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).

## Supprimer un projet dans une liste

Vous pouvez supprimer des projets d’une liste de projets.

1. Accédez à une liste de projets ou à un rapport de projet.
1. Sélectionnez le ou les projets à supprimer, puis cliquez sur l’icône **Supprimer** ![Icône Supprimer](assets/delete-icon.png) en haut de la liste.

1. Cliquez sur **Oui, supprimer** pour confirmer la suppression.

   Les projets sont supprimés et stockés dans la corbeille pendant 30 jours. Votre administrateur ou administratrice Workfront peut restaurer les projets supprimés de la corbeille durant cette période.

## Supprimer un projet au niveau du projet

1. Accédez au projet que vous souhaitez supprimer.
1. Cliquez sur l’icône **Plus** ![Menu Plus](assets/qs-more-menu.png) à droite du nom du projet, puis cliquez sur **Supprimer le projet**.

   ![Menu Plus développé](assets/more-icon-expanded-delete-project-highlighted.png)

1. Cliquez sur **Oui, supprimer**.

   Le projet est supprimé et stocké dans la corbeille pendant 30 jours. Votre administrateur ou administratrice Workfront peut le restaurer à partir de la corbeille pendant cette période.

## Supprimer un projet de la page des enregistrements connectés d&#39;un enregistrement Workfront Planning

>[!NOTE]
>
>Les informations de cette section font référence à Adobe Workfront Planning, une fonctionnalité supplémentaire d’Adobe Workfront.
>
>Pour obtenir la liste des conditions requises pour accéder à Workfront Planning, consultez [Présentation de l&#39;accès à Adobe Workfront Planning](/help/quicksilver/planning/access/access-overview.md).
> 
>Pour obtenir des informations générales sur Workfront Planning, voir [Prise en main d’Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).

Pour pouvoir accéder aux projets et les supprimer d’une page d’enregistrements connectés Workfront Planning, vous devez disposer des éléments suivants :

* Types d’enregistrements Planning connectés aux projets Workfront. Pour plus d’informations, consultez la section [Connecter des types d’enregistrements](/help/quicksilver/planning/architecture/connect-record-types.md).
* Enregistrements de planification. Pour plus d’informations, voir [Créer des enregistrements](/help/quicksilver/planning/records/create-records.md).
* Page Enregistrements connectés qui affiche les projets connectés à un enregistrement Planning. Pour plus d’informations, voir [Ajouter une page Enregistrements connectés à un enregistrement](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md).

Pour supprimer un enregistrement d&#39;une page d&#39;enregistrements connectée :

1. Sur la page Enregistrements connectés qui affiche les projets connectés à un enregistrement, passez la souris sur le nom d’un projet et cliquez sur l’icône **Plus** ![Icône Plus](assets/more-icon.png)

   Ou

   Sélectionnez un ou plusieurs projets dans la liste. Remarquez la barre bleue en bas de la liste des projets.

1. Cliquez sur **Supprimer**, puis sur **Supprimer** pour confirmer.

   Les projets sont supprimés et placés dans la corbeille de Workfront.

## Restauration des projets supprimés

Un administrateur ou administratrice système ou de groupes peut restaurer les projets dans les 30 jours suivant leur suppression, comme décrit dans l’article [Restaurer des éléments supprimés](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).
