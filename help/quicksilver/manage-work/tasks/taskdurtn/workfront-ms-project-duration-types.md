---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: Types de durée dans Adobe Workfront et Microsoft Project
description: Les types de durée disponibles dans Adobe Workfront sont différents de leurs équivalents dans les projets Microsoft, appelés Types de tâche. Cela peut parfois être déroutant lors de l’exportation ou de l’importation de projets entre Workfront et Microsoft Project.
author: Alina
feature: Work Management
exl-id: 986ecf91-693d-4ee1-bc56-355a2819ae41
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 11%

---

# Types de durée dans Adobe Workfront et Microsoft Project

Les types de durée disponibles dans Adobe Workfront sont différents de leurs équivalents dans les projets Microsoft, appelés Types de tâche. Cela peut parfois être déroutant lors de l’exportation ou de l’importation de projets entre Workfront et Microsoft Project.

Pour plus d’informations sur l’importation et l’exportation de projets entre Workfront et Microsoft Project, reportez-vous aux articles suivants :

* [Exporter un projet vers un projet Microsoft](../../../manage-work/projects/manage-projects/export-project-to-ms-project.md)
* [Importer un projet depuis Microsoft Project](../../../manage-work/projects/create-projects/import-project-from-ms-project.md)

## Types de durée dans les projets Workfront et Microsoft

Workfront comporte quatre types de durée de tâche :

* Simple
* Piloté par l&#39;effort
* Calcul de travail
* Calcul d&#39;affectation

Pour plus d’informations, voir [Présentation de la durée de la tâche et du type de durée](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

Ces types de durée ne sont pas reconnus par le projet Microsoft. Actuellement, le projet Microsoft comporte trois types de tâche similaires aux types de durée dans Workfront :

* Unités fixes
* Travail fixe
* Durée fixe

## Le type de durée change lors de l’exportation de Workfront vers un projet MS

Lors de l’exportation de projets de Workfront vers le projet Microsoft, les tâches pilotées par l’effort deviennent un travail fixe. Les tâches simples, calculées et l’affectation calculée deviennent des unités fixes.

## Le type de durée change lors de l’importation de MS Project vers Workfront

Lors de l’importation de projets de Microsoft Project dans Workfront, les unités fixes deviennent pilotées par l’effort. Le travail fixe et la durée fixe reçoivent le type de durée par défaut que votre administrateur Workfront a sélectionné pour votre système. Pour plus d’informations, voir [Configuration de la tâche à l’échelle du système et des préférences de problème](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

<!--
<note type="warning">
When a task has Calculated Work as the Duration Type and the default Duration Type in Setup is set as Calculated Assignment, then MS Project assignment allocations will be lost during the import.
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(drafting this because it is misleading)
</MadCap:conditionalText>
</note>
-->
