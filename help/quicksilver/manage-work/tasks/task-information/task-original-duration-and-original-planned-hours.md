---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Vue d’ensemble de la durée initiale de la tâche et des heures prévues à l’origine
description: Dans le cadre de la planification d’un projet, vous devez déterminer les valeurs du nombre d’heures prévues et de la durée (ou durée prévue) de chaque tâche du projet.
author: Alina
feature: Work Management
exl-id: 96d77d9f-3d5f-457e-a4ad-10edc371a991
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '578'
ht-degree: 100%

---

# Vue d’ensemble de la durée initiale de la tâche et des heures prévues à l’origine

Dans le cadre de la planification d’un projet, vous devez déterminer les valeurs du nombre d’heures prévues et de la durée (ou durée prévue) de chaque tâche du projet.

Pour plus d’informations sur le nombre d’heures prévues des tâches, voir [Vue d’ensemble du nombre d’heures prévues](../../../manage-work/tasks/task-information/planned-hours.md).

Pour plus d’informations sur la durée des tâches, voir [Vue d’ensemble de la durée des tâches et du type de durée](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

Vous pouvez consulter ces valeurs dans l’onglet Détails de la tâche ou lors de la modification d’une tâche.

Si vous créez une vue pour une liste de tâches ou un rapport de tâches, vous pouvez également voir les champs Nombre d’heures prévues initial et Durée d’origine pour les tâches.

## Nombre d’heures prévues à l’origine

Le nombre d’heures prévues initial d’une tâche représente le nombre d’heures prévues qu’une tâche avait à l’origine avant de devenir une tâche parent. Lorsqu’une tâche devient une tâche parent, le nombre d’heures prévues des tâches enfants est reporté sur la tâche parent afin d’indiquer le nombre d’heures prévues de la tâche parent.

En affichant le champ Nombre d’heures prévues initial dans un rapport ou une liste de tâches, vous pouvez voir le nombre initial d’heures prévues avant que la tâche n’hérite du nombre d’heures prévues de ses tâches enfants.

>[!NOTE]
>
>Lorsque vous créez une tâche, le nombre d’heures prévues initial est égal à zéro. Si la tâche devient une tâche parent, la valeur de ce champ est remplie avec le nombre d’heures prévues de la tâche avant qu’elle ne devienne une tâche parent. Cette valeur reste dans ce champ même lorsque la tâche redevient une tâche autonome.

## Durée originale

La durée initiale d’une tâche est la durée que la tâche avait à l’origine avant de devenir une tâche parent, en minutes. Lorsqu’une tâche devient un parent, la durée entre la date de début prévue du premier enfant et la date d’achèvement prévue du dernier enfant est reportée sur la tâche parent et devient la durée de la tâche parent. Cela remplace la durée de la tâche originale.

En affichant le champ Durée initiale dans un rapport ou une liste de tâches, vous pouvez voir le nombre original de jours pour la durée de la tâche avant qu’elle n’hérite de la durée de ses tâches enfants.

>[!NOTE]
>
>Lorsque vous créez une tâche, la durée initiale est égale à zéro. Si la tâche devient une tâche parent, la valeur de ce champ est remplie avec la durée de la tâche avant qu’elle ne devienne une tâche parent. Cette valeur reste dans ce champ même lorsque la tâche redevient une tâche autonome. Cette valeur s’affiche en minutes.

## Exemple

Par exemple, lorsque deux tâches sont autonomes, leur durée initiale et leur nombre d’heures prévues initial ont nuls.

![original_planned_hours_and_duration_without_parent.png](assets/original-planned-hours-and-duration-without-parent-350x38.png)

Lorsque la première tâche devient le parent de la seconde, les champs Durée initiale et Nombre d’heures prévues initial sont remplis avec les valeurs de la Durée et du Nombre d’heures prévues de la tâche avant qu’elle ne devienne le parent. La durée initiale est affichée en minutes. La durée et le nombre d’heures prévues de l’enfant deviennent la durée et le nombre d’heures prévues du parent.

![original_and_planned_hours_with_a_parent_task.png](assets/original-and-planned-hours-with-a-parent-task-350x38.png)

Lorsque le parent redevient une tâche autonome, la durée et le nombre d’heures prévues reprennent leurs valeurs d’origine, tandis que la durée et le nombre d’heures prévues d’lrigine restent renseignées. Ils ne reviennent pas à zéro.

![original_duration_and_planned_hours_after_reversal_of_a_parent.png](assets/original-duration-and-planned-hours-after-reversal-of-a-parent-350x39.png)
