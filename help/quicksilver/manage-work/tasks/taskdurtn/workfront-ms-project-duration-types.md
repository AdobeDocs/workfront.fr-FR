---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: Types de durée dans Adobe Workfront et Microsoft Project
description: Les types de durée disponibles dans Adobe Workfront sont différents de leurs équivalents dans Microsoft Project, appelés types de tâche. Cela peut parfois créer de la confusion lors de l’export ou de l’import de projets entre Workfront et Microsoft Project.
author: Alina
feature: Work Management
exl-id: 986ecf91-693d-4ee1-bc56-355a2819ae41
TQID: https://experienceleague.adobe.com/avh0ZuYJpsf7Ed5HiWuLkxEA-0PD-1iFvzHmWvpDZiI
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b91c0848-76c4-4da4-8b81-3aade0518dd0id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 257
ht-degree: 78%

---

# Types de durée dans Adobe Workfront et Microsoft Project

Les types de durée disponibles dans Adobe Workfront sont différents de leurs équivalents dans Microsoft Project, appelés types de tâche. Cela peut parfois créer de la confusion lors de l’export ou de l’import de projets entre Workfront et Microsoft Project.

Pour plus d’informations sur l’importation et l’exportation de projets entre Workfront et Microsoft Project, consultez les articles suivants :

* [Exporter un projet vers Microsoft Project](../../../manage-work/projects/manage-projects/export-project-to-ms-project.md)
* [Importer un projet à partir de Microsoft Project](../../../manage-work/projects/create-projects/import-project-from-ms-project.md)

## Types de durée dans les projets Workfront et Microsoft

Workfront comporte quatre types de durée de tâche :

* Simple
* Piloté par l&#39;effort
* Calcul de travail
* Calcul d&#39;affectation

Pour plus d’informations, voir [Vue d’ensemble de la durée de tâche et du type de durée](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

Ces types de durée ne sont pas reconnus par Microsoft Project. Actuellement, le projet Microsoft comporte trois types de tâches similaires aux types de durée dans Workfront :

* Unités fixes
* Travail fixe
* Durée fixe

## Le type de durée change lors de l’exportation de Workfront vers MS Project

Lors de l’export de projets de Workfront vers Microsoft Project, les tâches pilotées par l’effort deviennent un travail fixe. Les tâches simples, le calcul de travail et le calcul d’affectation deviennent des unités fixes.

## Le type de durée change lors de l&#39;importation de MS Project vers Workfront

Lors de l’import de projets de Microsoft Project dans Workfront, les unités fixes deviennent des tâches pilotées par l’effort. Le travail fixe et la durée fixe reçoivent le type de durée par défaut que votre administrateur ou administratrice Workfront a sélectionné pour votre système. Pour plus d’informations, voir [Configurer les préférences de tâche et de problème à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

<!--
<note type="warning">
When a task has Calculated Work as the Duration Type and the default Duration Type in Setup is set as Calculated Assignment, then MS Project assignment allocations will be lost during the import.
 
(drafting this because it is misleading)
 
</note>
-->
