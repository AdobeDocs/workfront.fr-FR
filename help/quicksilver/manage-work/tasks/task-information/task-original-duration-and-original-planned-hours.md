---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Présentation de la tâche Durée initiale et Heures planifiées initiales
description: Dans le cadre de la planification d’un projet, vous devez déterminer les valeurs des heures planifiées et de la durée (ou de la durée planifiée) de chaque tâche du projet.
author: Alina
feature: Work Management
exl-id: 96d77d9f-3d5f-457e-a4ad-10edc371a991
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 1%

---

# Présentation de la tâche Durée initiale et Heures planifiées initiales

Dans le cadre de la planification d’un projet, vous devez déterminer les valeurs des heures planifiées et de la durée (ou de la durée planifiée) de chaque tâche du projet.

Pour plus d’informations sur les heures planifiées pour les tâches, voir [Présentation des heures planifiées](../../../manage-work/tasks/task-information/planned-hours.md).

Pour plus d’informations sur la durée d’une tâche, voir [Présentation de la durée et du type de durée de la tâche](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

Vous pouvez voir ces valeurs dans l’onglet Détails de la tâche ou lors de la modification d’une tâche.

Si vous créez une vue pour une liste de tâches ou un rapport de tâches, vous pouvez également voir les champs Heures planifiées d’origine et Durée d’origine pour les tâches.

## Travail requis à l&#39;origine

Les Heures planifiées initiales d’une tâche représentent le nombre d’Heures planifiées qu’une tâche avait à l’origine avant de devenir une tâche parent. Lorsqu’une tâche devient une tâche parent, les Heures planifiées des tâches enfants sont cumulées à la tâche parent pour indiquer les Heures planifiées du parent.

En affichant le champ Heures planifiées d’origine dans un rapport de tâche ou une liste, vous pouvez voir le nombre d’heures planifiées d’origine avant que la tâche n’hérite du nombre d’heures planifiées de ses enfants.

>[!NOTE]
>
>Lorsque vous créez une tâche, le nombre d’heures initialement planifiées est nul. Si la tâche devient une tâche parente, la valeur de ce champ est renseignée avec le nombre d’ Heures planifiées de la tâche avant qu’elle ne soit remplacée par un parent. Cette valeur reste dans ce champ même si la tâche revient à une tâche autonome.

## Durée originale

La Durée d’origine d’une tâche est la Durée qu’une tâche avait à l’origine avant de devenir une tâche mère, en minutes. Lorsqu’une tâche devient parent, la Durée entre la Date de début planifiée du premier enfant et la Date de fin planifiée du dernier enfant est cumulée à la tâche parent et devient la Durée de la tâche parent. Cette opération remplace la Durée de la tâche d’origine.

En affichant le champ Durée d’origine dans un rapport ou une liste de tâches, vous pouvez voir le nombre de jours d’origine de la durée de la tâche avant qu’elle n’hérite de la durée de ses enfants.

>[!NOTE]
>
>Lorsque vous créez une tâche, la durée d’origine est zéro. Si la tâche devient une tâche parente, la valeur de ce champ est renseignée avec la Durée de la tâche avant qu’elle ne soit remplacée par un parent. Cette valeur reste dans ce champ même si la tâche revient à une tâche autonome. Cette valeur s’affiche en minutes.

## Exemple

Par exemple, lorsque deux tâches sont des tâches autonomes, leur durée d’origine et leurs heures planifiées originales sont nulles.

![original_scheduled_hours_and_duration_without_parent.png](assets/original-planned-hours-and-duration-without-parent-350x38.png)

Lorsque la première tâche devient le parent de la seconde tâche, les champs Durée d’origine et Heures planifiées d’origine sont renseignés avec les valeurs de la Durée et Heures planifiées de la tâche avant qu’elle ne devienne parent. La Durée d’origine s’affiche en minutes. La Durée et les Heures planifiées de l’enfant deviennent la Durée et les Heures planifiées du parent.

![original_and_scheduled_hours_with_a_parent_task.png](assets/original-and-planned-hours-with-a-parent-task-350x38.png)

Lorsque le parent redevient une tâche autonome, la durée et les heures planifiées reviennent aux valeurs d’origine, tandis que la durée d’origine et les heures planifiées d’origine restent renseignées. Ils ne reviennent pas à zéro.

![original_duration_and_scheduled_hours_after_reversion_of_a_parent.png](assets/original-duration-and-planned-hours-after-reversal-of-a-parent-350x39.png)
