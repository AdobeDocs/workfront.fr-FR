---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: Types de durée dans Adobe Workfront et Microsoft Project
description: Les types de durée disponibles dans Adobe Workfront sont différents de leurs équivalents dans Microsoft Project, appelés types de tâche. Cela peut parfois créer de la confusion lors de l’export ou de l’import de projets entre Workfront et Microsoft Project.
author: Alina
feature: Work Management
exl-id: 986ecf91-693d-4ee1-bc56-355a2819ae41
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 100%

---

# Types de durée dans Adobe Workfront et Microsoft Project

Les types de durée disponibles dans Adobe Workfront sont différents de leurs équivalents dans Microsoft Project, appelés types de tâche. Cela peut parfois créer de la confusion lors de l’export ou de l’import de projets entre Workfront et Microsoft Project.

Pour plus d’informations sur l’import et l’export de projets entre Workfront et Microsoft Project, voir les articles suivants :

* [Exporter un projet vers Microsoft Project](../../../manage-work/projects/manage-projects/export-project-to-ms-project.md)
* [Importer un projet à partir de Microsoft Project](../../../manage-work/projects/create-projects/import-project-from-ms-project.md)

## Types de durée dans Workfront et Microsoft Project

Workfront comporte quatre types de durée de tâche :

* Simple
* Piloté par l&#39;effort
* Calcul de travail
* Calcul d&#39;affectation

Pour plus d’informations, voir [Vue d’ensemble de la durée de tâche et du type de durée](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

Ces types de durée ne sont pas reconnus par Microsoft Project. Actuellement, Microsoft Project comporte trois types de tâche similaires aux types de durée dans Workfront :

* Unités fixes
* Travail fixe
* Durée fixe

## Le type de durée change lors de l’export de Workfront vers MS Project.

Lors de l’export de projets de Workfront vers Microsoft Project, les tâches pilotées par l’effort deviennent un travail fixe. Les tâches simples, le calcul de travail et le calcul d’affectation deviennent des unités fixes.

## Le type de durée change lors de l’import à partir de MS Project vers Workfront

Lors de l’import de projets de Microsoft Project dans Workfront, les unités fixes deviennent des tâches pilotées par l’effort. Le travail fixe et la durée fixe reçoivent le type de durée par défaut que votre administrateur ou administratrice Workfront a sélectionné pour votre système. Pour plus d’informations, voir [Configurer les préférences de tâche et de problème à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

<!--
<note type="warning">
When a task has Calculated Work as the Duration Type and the default Duration Type in Setup is set as Calculated Assignment, then MS Project assignment allocations will be lost during the import.
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(drafting this because it is misleading)
</MadCap:conditionalText>
</note>
-->
