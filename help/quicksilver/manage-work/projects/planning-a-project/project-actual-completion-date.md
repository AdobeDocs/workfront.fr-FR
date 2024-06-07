---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Vue d’ensemble de la date d’achèvement effective du projet
description: Les projets, tâches et problèmes ont une date d’achèvement réelle dans Adobe Workfront. Il s’agit de la date à laquelle le projet, la tâche ou le problème ont été marqués comme étant terminés.
author: Alina
feature: Work Management
exl-id: 0baba359-a61d-43d7-8336-1f45c7f34374
source-git-commit: c593eab154a0942995b1f913e7189450913faac0
workflow-type: tm+mt
source-wordcount: '489'
ht-degree: 2%

---

# Vue d’ensemble de la date d’achèvement effective du projet

Les projets, tâches et problèmes ont une date d’achèvement réelle dans Adobe Workfront. Il s’agit de la date à laquelle le projet, la tâche ou le problème ont été marqués comme étant terminés.

## Dates d’achèvement réelles

La date de fin réelle représente la date et l’heure réelles auxquelles le travail est terminé. Lorsqu’une tâche ou un problème est marqué comme Terminé ou Terminé, Workfront définit automatiquement la date du changement d’état de l’élément comme Date d’achèvement réelle de la tâche ou du problème. Si cette date ne reflète pas exactement le moment où la tâche ou le problème a été réellement terminé, vous pouvez modifier manuellement la date de fin réelle.

Par exemple, vous pouvez marquer une tâche ou un problème Terminé le lundi, mais vous savez que le travail a été terminé le vendredi précédent. Après avoir marqué la tâche ou le problème comme terminé, vous pouvez mettre à jour manuellement la date d’achèvement réel de la tâche ou de l’émission à la date du vendredi précédent pour refléter la fin réelle.

Vous ne pouvez pas modifier manuellement la date de fin réelle d’un projet, mais vous pouvez modifier manuellement l’état d’un projet, ce qui peut déclencher une modification de sa date de fin réelle.

La date d’achèvement réelle d’un projet est définie comme suit :

* En mettant manuellement à jour l’état du projet : si le mode d’achèvement du projet est défini sur Manuel et que vous modifiez manuellement l’état du projet sur Terminé, la date d’achèvement réel du projet est mise à jour à la date et à l’heure de la dernière tâche terminée.
* Automatiquement, lorsque la dernière tâche du projet se termine : si le mode d’achèvement du projet est défini sur Automatique et que vous marquez la dernière tâche comme Terminée ou mettez à jour la date d’achèvement réelle de la dernière tâche, la date d’achèvement réelle du projet est également mise à jour avec cette date.

  Pour plus d’informations sur la définition du mode d’exécution d’un projet, voir l’article . [Modification de projets](../../../manage-work/projects/manage-projects/edit-projects.md).

  >[!NOTE]
  >
  >Workfront utilise la date d’achèvement réelle de la tâche du projet qui s’est terminée en dernier en tant que date d’achèvement réel pour l’ensemble du projet.

Un administrateur Workfront ou de groupe détermine si Workfront utilise la date d’aujourd’hui ou la date d’achèvement planifiée d’une tâche ou un problème lorsqu’ils sont définis sur Terminé ou Fermé. Pour plus d’informations sur la définition des préférences de tâche et de problème, voir [Configuration des préférences de tâche et de problème à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

<!--this statement is confusing, not sure what it is referring to, so I am drafting this for now: The value for the Actual Completion Date is always what is considered the current date and time.-->



## Localisation des dates de fin réelles

La date d’achèvement réelle se trouve dans les zones suivantes de Workfront :

* Zones Projet, Tâche et Détails du problème
* Boîtes Modifier le projet, la tâche et le problème
* Zone Projet, Tâche et Mises à jour du problème en tant que mise à jour du système.
* Listes ou rapports de projet, de tâche ou de problème.

Pour plus d’informations sur la création de rapports, voir l’article [Création d’un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
