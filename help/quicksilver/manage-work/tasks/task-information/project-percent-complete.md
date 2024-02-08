---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Pourcentage du projet - Aperçu complet
description: La valeur Pourcentage d’achèvement d’un projet est calculée en fonction de la durée planifiée ou des heures planifiées des tâches du projet. Votre administrateur Adobe Workfront ou un administrateur de groupe définit la valeur qui est prise en compte lors du calcul du pourcentage d’achèvement dans votre système lors de la configuration des informations dans la zone Préférences du projet. Pour plus d’informations sur la configuration des préférences du projet, voir Configuration des préférences du projet à l’échelle du système.
author: Alina
feature: Work Management
exl-id: d2395569-9fe5-42e7-a392-cff49eb519d9
source-git-commit: 816fd70642ffb7b24095602ce160421aa947e2a6
workflow-type: tm+mt
source-wordcount: '778'
ht-degree: 0%

---

# Pourcentage du projet - Aperçu complet

<!-- Audited 01/2024 -->

La valeur Pourcentage d’achèvement d’un projet est calculée en fonction de la durée ou des heures planifiées des tâches du projet. Votre administrateur Adobe Workfront ou un administrateur de groupe définit la valeur qui est prise en compte lors du calcul du pourcentage d’achèvement dans votre système lors de la configuration des informations dans la zone Préférences du projet.

Pour plus d’informations sur la configuration des préférences du projet, voir [Configuration des préférences de projet à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Le pourcentage d’achèvement d’une tâche mère est basé sur la durée ou les heures planifiées de chacune de ses sous-tâches.

De même, le pourcentage de fin d’un projet est basé sur les durées ou les heures planifiées de chaque tâche principale du projet.

Les tâches principales sont les tâches parentes et les tâches autonomes qui n&#39;ont pas d&#39;enfants.

>[!TIP]
>
>Les tâches principales ne sont pas mises en retrait dans un plan de projet.

## Comment Workfront calcule le pourcentage terminé

### Mettre à jour le pourcentage terminé sur une tâche {#update-the-percent-complete-on-a-task}

Vous pouvez modifier manuellement le pourcentage d’achèvement d’une tâche. Ce n&#39;est pas un calcul.

Workfront utilise le pourcentage d’achèvement d’une tâche individuelle pour calculer le pourcentage d’achèvement de sa tâche parent ou le pourcentage d’achèvement du projet.

Pour plus d’informations sur la mise à jour du pourcentage d’achèvement d’une tâche, voir [Afficher et mettre à jour le pourcentage d’achèvement pour les tâches](../../../manage-work/projects/updating-work-in-a-project/view-update-percent-complete-for-tasks.md).

### Comment Workfront calcule le pourcentage terminé sur une tâche parent {#how-workfront-calculates-percent-complete-on-a-parent-task}

Selon ce que votre administrateur Workfront ou de groupe a sélectionné dans les préférences du projet au niveau du système ou du groupe, le pourcentage d’achèvement d’une tâche parent est calculé en fonction de la durée ou des heures planifiées des tâches.

Examinez les scénarios suivants :

* Si le système calcule le pourcentage de réalisation sur la base des Heures planifiées, le pourcentage de réalisation de la tâche parente est calculé à l’aide de la formule suivante :

  `Parent Task Percent Complete = (((Task 1 Planned Hours * Task 1 Percent Complete) + (Task 2 Planned Hours * Task 2 Percent Complete))/Total Planned Hours of Parent)*100`

  Le total des heures planifiées du parent représente la somme de toutes les heures planifiées de chacun des enfants.

  ![](assets/project-with-tasks-percent-complete-planned-hours-calculation.png)

* Si le système calcule le pourcentage de fin en fonction de la durée, le pourcentage de fin de la tâche parente est calculé à l’aide de la formule suivante :

  `Parent Task Percent Complete = (((Task 1 Duration * Task 1 Percent Complete) + (Task 2 Duration * Task 2 Percent Complete))/ Total Duration of Parent)*100`

  ![](assets/project-with-tasks-percent-complete-duration-calculation.png)

  >[!IMPORTANT]
  >
  >La durée totale de la tâche mère est le total de toutes les durées des tâches enfants. Par exemple, une tâche parent avec deux enfants dont la durée respective est de 1 jour et de 2 jours a une durée totale de 3 jours, même lorsque les deux enfants peuvent commencer le même jour.


### Comment Workfront calcule le pourcentage terminé sur un projet {#how-workfront-calculates-percent-complete-on-a-project}

Selon ce que votre administrateur Workfront ou de groupe a sélectionné dans les préférences du projet au niveau du système ou du groupe, le pourcentage de réalisation d’un projet est calculé en fonction de la durée ou des heures planifiées des tâches principales du projet.

* Si le système calcule le pourcentage de réalisation sur la base des heures planifiées, le pourcentage de réalisation du projet est calculé à l’aide de la formule suivante :

  `Project Percent Complete =(((Task 1 Planned Hours * Task 1 Percent Complete) + (Task 2 Planned Hours * Task 2 Percent Complete))/Total Planned Hours of the Project)*100`

  Le total des heures planifiées du projet est la somme des heures planifiées de toutes les tâches principales du projet.

  ![](assets/project-with-tasks-percent-complete-planned-hours-calculation.png)

  >[!NOTE]
  >
  >La tâche 1 ou la tâche 2 ne peuvent être que des tâches parentes ou des tâches autonomes. Les tâches Heures planifiées et Pourcentage d’achèvement des tâches enfants ne sont pas utilisées dans ce calcul.

* Si le système calcule le pourcentage de réalisation sur la base de la durée, le pourcentage de réalisation du projet est calculé à l’aide de la formule suivante :

  `Project Percent Complete = (((Task 1 Duration * Task 1 Percent Complete) + (Task 2 Duration * Task 2 Percent Complete))/Duration of the Project)*100`

  >[!IMPORTANT]
  >
  >La durée du projet est le total de toutes les durées des tâches principales qui affichent un pourcentage de réalisation. Par exemple, un projet avec une tâche autonome d’une durée de 2 jours et une tâche parent d’une durée de 5 jours pour laquelle un travail a été effectué sur celle-ci aura une durée totale de 7 jours, même si les deux tâches peuvent commencer le même jour.

  ![](assets/project-with-tasks-percent-complete-duration-calculation.png)

  >[!NOTE]
  >
  >La tâche 1 ou la tâche 2 ne peuvent être que des tâches parentes ou des tâches autonomes. Les tâches Durée et Pourcentage d’achèvement des enfants ne sont pas utilisées dans ce calcul.

## Exemple de pourcentage d’achèvement sur un projet utilisant la durée

Lorsque vous utilisez la Durée des tâches pour calculer le pourcentage de réalisation d’un projet, prenez en compte l’exemple suivant :

![](assets/project-with-tasks-percent-complete-duration-calculation.png)

Les informations suivantes sont utilisées pour calculer le pourcentage de réalisation du projet

* Pourcentage d’achèvement de la tâche autonome (tâche 1 - 20 %)
* Pourcentage d’achèvement de la tâche parent (tâche 2 à 25 %)
* Durée de la tâche 1 (5 jours)
* Durée de la tâche 2 (2 jours)
* Durée du projet (7 jours)


Pour calculer le pourcentage de réalisation du projet à l’aide de la durée :

`Project Percent Complete = (((Task 1 Duration * Task 1 Percent Complete) + (Task 2 Duration * Task 2 Percent Complete))/Duration of the Project)*100`

Ou

`(((5*0.2)+(2*0.25))/7)*100= 21.43%`


<!--drafted, this was the old example:

When using the Planned Duration of the tasks to calculate the percent complete of a project, consider the following example:

percent_complete_on_project_example.png

Only the parent task (Task 1) and the standalone task (Task 8) are used to calculate the percent complete of the project.

The secondary parents of Task 1 are used to calculate the percent complete of the main parent (Task 1).

To calculate the percent complete of the main parent (Task 1), first calculate the percent complete of its secondary parents:

Task 5 Percent Complete = ((14 * 0.75 + 12 * 0.25)/(12 + 14))*100 = 51.92%

Task 2 Percent Complete = ((5 * 0.7 + 2 * 0.5)/(5 + 2))*100 = 64.29 %

Then, to calculate the percent complete of the main parent (Task 1), use the following formula:

Task 1 Percent Complete =((56 * 0.5192 + 7 * 0.6429)/63)*100 = 53.29%

To calculate the percent complete of the project, you will need to have the following numbers ready:

Task 1 Duration (63 hours) and Percent Complete (53.29%)
Task 8 Duration (100 hours) and Percent Complete (4%)
Now, to calculate the percent complete of the project, use the following formula:

Project Percent Complete =((100 * 0.04 + 63 * 0.5329))/163)*100 = 23.05%
-->