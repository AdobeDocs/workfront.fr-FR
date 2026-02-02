---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: 'Présentation du type de durée : affectation calculée'
description: Le calcul d’affectation est un type de durée que vous pouvez définir pour une tâche dans Adobe Workfront. Pour des informations générales sur les types de durée dans Workfront, voir Vue d’ensemble de la durée de la tâche et du type de durée.
author: Alina
feature: Work Management
exl-id: 5f1f6109-5d54-4c3f-9aa5-dc6ce165a1cd
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 81%

---

# Vue d’ensemble du type de durée : calcul d’affectation

<!-- Audited: 5/2025 -->

Le calcul d’affectation est un type de durée que vous pouvez définir pour une tâche dans Adobe Workfront. Pour des informations générales sur les types de durée dans Workfront, voir [Vue d’ensemble de la durée de la tâche et du type de durée](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

## Vue d’ensemble du type de durée Calcul d’affectation

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This Hub issue has a powerpoint that highlights information that is useful to users when using Calculated Assignment duration type. I don't think we can use the powerpoint, because it's old. I also don't know if the things they discuss are still relevant, since the PP is from 2015. I've closed the issue, but I'm putting a link here just in case the info is useful. https://hub.workfront.com/issue/5a9dd7d5007d02a8966014557c23cc89/updates)</p>
-->

* Lorsque vous utilisez un type de durée Calcul d’affectation, vous devez spécifier à la fois une durée et un nombre d’heures prévues pour la tâche. Workfront divise ensuite le nombre d’heures prévues par le nombre d’heures de la durée, puis par le nombre de ressources affectées à la tâche pour calculer le pourcentage d’affectation (l’allocation) pour chaque ressource. Chaque ressource aura la même valeur pour son pourcentage d’affectation. Dans ce cas, vous ne pouvez pas modifier les valeurs d’affectation de chaque ressource.
* Votre Workfront ou un administrateur de groupes peut définir le type de durée par défaut de votre système ou de votre groupe en tant qu&#39;affectation calculée. Dans ce cas, toutes les nouvelles tâches seront créées avec ce type de durée. Pour plus d’informations sur la modification de votre tâche et les préférences de problème dans le cadre de vos préférences de projet à l’échelle du système ou du groupe, voir [Configurer les préférences de tâche et de problème à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

  Dans ce cas, la tâche affiche une durée par défaut d’une journée et un nombre d’heures prévues par défaut de 0. Si la personne responsable du projet ne fixe pas de durée plus précise et ne remplit pas le champ Nombre d’heures prévues avec une estimation réaliste, les ressources apparaissent sous-affectées.

Le calcul d’affectation correspond au type de durée préféré dans les situations suivantes :

* Lorsque les affectations ont une fenêtre d&#39;activité mais ne prennent pas toute la durée allouée pour terminer leur travail. Par exemple, vous devez remettre un rapport à la personne chargée de votre supervision avant la fin de la semaine. Vous avez une durée de cinq jours, mais il ne vous faudra que 10 heures pour rédiger le document.
* Lorsqu’une seule ressource est affectée à une tâche parce que la personne responsable du projet peut estimer la durée prévue et le volume d’effort prévu, indépendamment l’un de l’autre.

  Vous pouvez utiliser le type de durée Calcul de travail pour le même résultat, mais la personne responsable du projet doit saisir un pourcentage d’allocation de la ressource afin d’affecter la valeur calculée pour le nombre d’heures prévues. Cela rend la planification des projets plus difficile et plus longue.

Le pourcentage d’allocation de chaque ressource est calculé comme suit :

```
Planned Hours / Duration / Number of Resources = Allocation Percentage for each resource
```

Par exemple, dans le scénario décrit ci-dessous, chaque tâche a une durée de 3 jours. La personne responsable du projet saisit manuellement la durée (3 jours ou 24 heures) et les heures prévues, ce qui permet de calculer le pourcentage d’allocation (ou pourcentage d’affectation) :

![Type de durée d&#39;affectation calculée](assets/calcassign-350x80.png)

## Modifier le type de durée d’une tâche en Calcul d’affectation

Pour plus d’informations sur la modification du type de durée d’une tâche, voir la section [Mettre à jour le type de durée d’une tâche](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md).

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
