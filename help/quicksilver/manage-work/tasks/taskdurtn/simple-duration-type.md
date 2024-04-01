---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: "Présentation du type de durée : simple"
description: Le type de durée simple est un type de durée que vous pouvez définir pour une tâche dans Adobe Workfront. Pour obtenir des informations générales sur les types de durée dans Workfront, consultez Présentation de la durée de la tâche et du type de durée.
author: Alina
feature: Work Management
exl-id: 9bb472db-1448-467e-93ca-611453e1c00a
source-git-commit: 1efd7c0270fe1396345cfa6e5499e8f998297d61
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 0%

---

# Présentation du type de durée : simple

Le type de durée simple est un type de durée que vous pouvez définir pour une tâche dans Adobe Workfront. Pour obtenir des informations générales sur les types de durée dans Workfront, voir [Présentation de la durée et du type de durée de la tâche](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

## Présentation du type de durée simple

Votre administrateur Workfront ou un administrateur de groupe peut définir le type de durée par défaut de votre système ou groupe comme simple. Dans ce cas, toutes les nouvelles tâches seront créées avec ce type de durée. Pour plus d’informations sur la modification de votre tâche et les préférences des problèmes dans le cadre de vos préférences de projet au niveau du système ou du groupe, voir [Configuration des préférences de tâche et de problème à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

Les événements suivants se produisent lorsqu’une tâche a un type de durée simple :

* Les chefs de projet peuvent modifier la durée et les heures planifiées d’une tâche lors de la modification de la façon dont ces heures doivent être réparties entre les personnes désignées.

  Pour plus d’informations, voir [Mettre à jour les heures et la durée planifiées d’une tâche avec un type de durée simple](../../../manage-work/tasks/taskdurtn/update-planned-hours-duration-for-simple-duration-task.md).

  >[!IMPORTANT]
  >
  >Lorsque vous créez une tâche pour la première fois et que vous lui attribuez le Type de durée simple sans spécifier de durée, Workfront calcule la Durée de la tâche en fonction du nombre d’heures planifiées que vous indiquez pour la tâche. Si vous modifiez manuellement la Durée d’une tâche Durée simple, Workfront cesse de faire correspondre les Heures planifiées à la Durée, car cela suppose que vous souhaitiez les définir manuellement.
  >
  >Workfront calcule la durée des tâches dont la durée n&#39;a pas été modifiée manuellement à l&#39;aide de la formule suivante :
  >
  > `Task Duration = Task Planned Hours / Typical hours per work day`
  >
  >Votre administrateur Workfront définit la variable `Typical hours per work day` dans la zone Préférences du projet de la configuration de votre instance.

* Le pourcentage d’affectation est masqué et les heures d’affectation peuvent être modifiées.
* Pour tous les nouveaux clients, le type de durée au niveau du système est défini sur Simple.

## Remplacer le type de durée d’une tâche par Simple

Pour plus d’informations sur la modification du type de durée d’une tâche, voir [Mise à jour du type de durée d’une tâche](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replaced with new article linked above)</p>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Go to a task for which you want to change the Duration Type.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Task Details</strong> in the left panel, then in the Overview area double click <strong>Duration Type</strong>. </p> </li>
<li value="3"> <p>Select <strong>Simple</strong> from the drop-down menu.</p> </li>
<li value="4">Click <strong>Save</strong> <strong>Changes</strong><strong>.</strong></li>
</ol>
-->
