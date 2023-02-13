---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: '''Présentation du type de durée : Attribution calculée"'
description: L’affectation calculée est un type de durée que vous pouvez définir pour une tâche dans Adobe Workfront. Pour obtenir des informations générales sur les types de durée dans Workfront, consultez Présentation de la durée de la tâche et du type de durée.
author: Alina
feature: Work Management
exl-id: 5f1f6109-5d54-4c3f-9aa5-dc6ce165a1cd
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '478'
ht-degree: 0%

---

# Présentation du type de durée : Attribution calculée

L’affectation calculée est un type de durée que vous pouvez définir pour une tâche dans Adobe Workfront. Pour obtenir des informations générales sur les types de durée dans Workfront, voir [Présentation de la durée et du type de durée de la tâche](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

## Présentation du type de durée d’affectation calculée

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This Hub issue has a powerpoint that highlights information that is useful to users when using Calculated Assignment duration type. I don't think we can use the powerpoint, because it's old. I also don't know if the things they discuss are still relevant, since the PP is from 2015. I've closed the issue, but I'm putting a link here just in case the info is useful. https://hub.workfront.com/issue/5a9dd7d5007d02a8966014557c23cc89/updates)</p>
-->

* Lorsque vous utilisez un type de durée d’affectation calculée, vous devez spécifier une durée et un nombre d’heures planifiées pour la tâche. Workfront divise ensuite le montant des heures planifiées par le nombre d’heures dans la durée, puis par le nombre de ressources affectées à la tâche pour calculer le pourcentage d’affectation (calcule l’affectation) pour chaque ressource. Chaque ressource aura également la même valeur pour son pourcentage d’allocation. Dans ce cas, vous ne pouvez pas modifier les valeurs d’attribution de chaque ressource.
* Votre administrateur Workfront ou un administrateur de groupe peut définir le type de durée par défaut de votre système ou groupe comme affectation calculée. Dans ce cas, toutes les nouvelles tâches seront créées avec ce type de durée. Pour plus d’informations sur la modification de votre tâche et les préférences des problèmes dans le cadre de vos préférences de projet au niveau du système ou du groupe, voir [Configuration des préférences de tâche et de problème à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

   Dans ce cas, la tâche a par défaut une durée d’un jour et une valeur par défaut de 0 heure planifiée. À moins que le chef de projet ne définisse une durée plus précise et ne renseigne le champ Heures planifiées avec une estimation réaliste, les ressources apparaissent sous-affectées.

L’affectation calculée est le type de durée préféré dans les situations suivantes :

* Lorsque les affectations disposent d’une fenêtre d’activité, mais ne prennent pas toute la durée allouée pour terminer leur travail. Par exemple, vous devez envoyer un rapport à votre superviseur d’ici la fin de la semaine. Vous avez une durée de cinq jours, mais vous ne devrez attendre que dix heures pour rédiger le document.
* Lorsqu’une seule ressource est affectée à une tâche, car le chef de projet peut estimer la durée planifiée et le volume d’effort planifié indépendamment l’un de l’autre.

   Vous pouvez utiliser le type Durée de travail calculée pour le même résultat, mais le chef de projet doit saisir une allocation de pourcentage pour la ressource afin d’affecter la valeur calculée pour les Heures planifiées. Cela rend la planification du projet plus difficile et plus chronophage.

Le pourcentage d&#39;allocation pour chaque ressource est calculé comme suit :

```
Planned Hours / Duration / Number of Resources = Allocation Percentage for each resource
```

Par exemple, dans le scénario décrit ci-dessous, chaque tâche a une durée de 3 jours. Le chef de projet saisit manuellement la durée (3 jours ou 24 heures) et les heures planifiées. Par conséquent, le pourcentage d’affectation (ou pourcentage d’affectation) est calculé comme suit :

![](assets/calcassign-350x80.png)

## Remplacer le type de durée d’une tâche par affectation calculée

Pour plus d’informations sur la modification du type de durée d’une tâche, voir [Mise à jour du type de durée d’une tâche](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replaced with new article linked above)</p>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Go to a task for which you want to change the Duration Type.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Task Details</strong> in the left panel, then in the Overview area double click <strong>Duration Type</strong>. </p> </li>
<li value="3">Select <strong>Calculated Assignment</strong> from the drop-down menu.</li>
<li value="4">Click <strong>Save</strong> <strong>Changes</strong>.</li>
</ol>
-->
