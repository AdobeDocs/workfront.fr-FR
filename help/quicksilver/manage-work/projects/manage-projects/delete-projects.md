---
title: Supprimer des projets
product-area: projects
navigation-topic: manage-projects
description: Vous pouvez supprimer un projet si celui-ci et ses données ne sont plus nécessaires. Au lieu de supprimer un projet, nous vous recommandons de le modifier et de définir le statut Terminé ou Mort. Cette opération supprime de la liste des tâches d’un utilisateur toutes les tâches en cours liées au projet, mais enregistre toutes les données associées au projet.
author: Alina
feature: Work Management
exl-id: a0e80c4d-29a8-4bf8-aa19-0c2d493236c6
recommendations: noDisplay, noCatalog
source-git-commit: 84c5772d130be78d9f9b9aef342c57183d5ec985
workflow-type: tm+mt
source-wordcount: '908'
ht-degree: 7%

---

# Supprimer des projets

<!--Audited: 01/2024-->

Vous pouvez supprimer un projet si celui-ci et ses données ne sont plus nécessaires.

Au lieu de supprimer un projet, nous vous recommandons de le modifier et de définir le statut Terminé ou Mort. Cette opération supprime de la liste des tâches d’un utilisateur toutes les tâches en cours liées au projet, mais enregistre toutes les données associées au projet.

Vous pouvez supprimer un projet dans une liste de projets ou au niveau du projet.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Forfait Adobe Workfront</p> </td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td> <p>Licence Adobe Workfront*</p> </td> 
   <td> <p>Licence actuelle : formule </p> 
   Ou
   <p>Nouvelle licence : Standard </p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Configuration du niveau d’accès</td> 
   <td> <p>Modification de l’accès aux projets avec possibilité de créer et de supprimer des projets</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Autorisations d’objet </p> </td> 
   <td> <p>Modifier l’accès aux projets, tâches, problèmes avec la possibilité de supprimer des projets, des tâches et des problèmes</p> </td> 
  </tr> 
 </tbody> 
</table>

* Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront. Pour plus d’informations sur les exigences d’accès, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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
   * Problèmes
   * Mises à jour
   * Approbations
   * Frais
   * Risques
   * Niveaux de référence
   * Informations de cas d’entreprise
   * Informations sur la file d’attente
   * Taux de facturation
   * Enregistrements de facturation

     Vous ne pouvez pas supprimer un projet dont l’état est Facturé pour les enregistrements de facturation. Pour plus d’informations, consultez [Créer des enregistrements de facturation](../../projects/project-finances/create-billing-records.md).

* Selon la manière dont votre administrateur Workfront configure les préférences Projet, Tâche ou Suppression d’un problème dans les préférences Frise chronologique et Heures de votre instance Workfront, les heures consignées pour les tâches, les problèmes ou le projet sont traitées de l’une des manières suivantes lors de la suppression du projet :

   * Les heures restent sur la feuille de temps comme heure générale.
   * Les heures sont supprimées et seront restaurées si le projet est un jour restauré.

  Pour plus d’informations sur la configuration des préférences de suppression pour les heures de connexion aux problèmes, voir [Configuration des préférences de feuille de temps et d’heure](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

* Si le projet que vous supprimez est lié à une initiative dans le planificateur de scénario Workfront :

   * L&#39;initiative reste sur le plan, mais le lien vers le projet est supprimé.
   * Si le projet que vous supprimez est lié à la seule initiative publiée d’un plan, l’indication que le plan a été publié est également supprimée.
   * Si vous récupérez un projet supprimé, le projet est récupéré, mais son lien avec l’initiative n’est pas restauré et la zone du planificateur de scénario ne s’affiche plus dans les détails du projet.

     Le planificateur de scénario nécessite une licence supplémentaire. Pour plus d’informations sur le planificateur de scénario Workfront, voir [Présentation du planificateur de scénarios](../../../scenario-planner/scenario-planner-overview.md).

     Pour plus d’informations sur les projets liés aux initiatives dans le planificateur de scénario, voir [Mettre à jour ou créer des projets en publiant des initiatives dans le planificateur de scénarios](../../../scenario-planner/publish-scenarios-update-projects.md).

* Si le projet est également une activité pour un objectif dans les objectifs de Workfront :

   * Le projet est supprimé de l’objectif. La progression indiquée sur l’objectif par le projet est également supprimée.

   * Si vous récupérez le projet supprimé, le projet est également restauré en tant qu’activité de l’objectif.

     Cela nécessite une licence supplémentaire. Pour plus d’informations sur les objectifs de Workfront, voir [Présentation des objectifs d’Adobe Workfront](../../../workfront-goals/goal-management/wf-goals-overview.md).

     Pour plus d’informations sur l’association de projets à des objectifs, voir [Ajout de projets aux objectifs dans les objectifs Adobe Workfront](../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).

## Supprimer un projet dans une liste

Vous pouvez supprimer des projets d’une liste de projets.

1. Accédez à une liste de projets ou à un rapport de projet.
1. Sélectionnez le ou les projets que vous souhaitez supprimer, puis cliquez sur le bouton **Supprimer** icon ![](assets/delete-icon.png) en haut de la liste.

1. Cliquez sur **Oui, la supprimer** pour confirmer la suppression.

   Les projets sont supprimés et stockés dans la Corbeille pendant 30 jours. Votre administrateur Workfront peut alors restaurer les projets supprimés de la Corbeille.

## Suppression d’un projet au niveau du projet

1. Accédez au projet que vous souhaitez supprimer.
1. Cliquez sur le bouton **Plus** icon ![](assets/qs-more-menu.png) à droite du nom du projet, puis cliquez sur **Supprimer le projet**.

   ![](assets/more-icon-expanded-delete-project-highlighted.png)

1. Cliquez sur **Oui, supprimez-le**.

   Le projet est supprimé et stocké dans la Corbeille pendant 30 jours. Votre administrateur Workfront peut le restaurer à partir de la Corbeille pendant cette période.

## Restauration des projets supprimés

Un administrateur système ou de groupe peut restaurer les projets dans les 30 jours suivant leur suppression, comme décrit dans l’article . [Restauration des éléments supprimés](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).
