---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: "Présentation du type de durée : piloté par l’effort"
description: Effort Driven est un type de durée que vous pouvez définir pour une tâche dans Adobe Workfront. Pour des informations générales sur les types de durée dans Workfront, voir Vue d’ensemble de la durée de la tâche et du type de durée.
author: Alina
feature: Work Management
exl-id: 3c8534f7-02d0-4404-a37b-0ef6360e8efc
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '862'
ht-degree: 12%

---

# Vue d’ensemble du type de durée : piloté par l’effort

Effort Driven est un type de durée que vous pouvez définir pour une tâche dans Adobe Workfront. Pour des informations générales sur les types de durée dans Workfront, voir [Vue d’ensemble de la durée de la tâche et du type de durée](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

## Présentation du type de durée pilotée par l’effort

Votre administrateur Workfront ou un administrateur de groupe peut définir le type de durée par défaut de votre système ou groupe comme piloté par Effort.Dans ce cas, toutes les nouvelles tâches seront créées avec ce type de durée. Pour plus d’informations sur la modification de votre tâche et les préférences de problème dans le cadre de vos préférences de projet à l’échelle du système ou du groupe, voir [Configurer les préférences de tâche et de problème à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

Dans ce scénario, il existe un risque de raccourcir arbitrairement le plan du projet, à moins que vous, en tant que chef de projet, preniez le temps de déterminer si la tâche est réellement une tâche pilotée par l’effort.

Utilisez Effort Driven pour :

* Déterminez la durée planifiée en fonction du nombre de ressources disponibles pour travailler sur la tâche. La durée est égale aux heures planifiées. La durée planifiée est égale au nombre d’heures planifiées divisé par le nombre de personnes désignées.

  Le niveau d&#39;effort appliqué à la tâche détermine la division du travail et la durée.

* Trackez le nombre total d’heures passées sur une tâche lorsque plusieurs ressources sont affectées.

  Lorsque des ressources sont ajoutées, la Durée planifiée de la tâche diminue. (Le principe &quot;plusieurs mains font un travail léger&quot; illustre l’effet que ce type de durée a sur la durée planifiée d’une tâche.)

Les sections suivantes fournissent des informations plus détaillées sur la façon dont Workfront calcule la durée planifiée d’une tâche pilotée par l’effort et l’effet que l’ajout de ressources a sur la tâche avec ce type de durée.

## Présentation de la formule Type de durée pilotée par l’effort

La formule de calcul de la Durée planifiée d’une tâche avec un Type de durée de l’effort piloté dépend du pourcentage d’affectation de chaque ressource affectée à la tâche. Dans le cas d’une tâche pilotée par l’effort, Workfront calcule les Heures planifiées de la tâche et elles sont toujours identiques à la Durée de la tâche :

```
Planned Hours (in hours) = Duration (in days)
```

Vous pouvez ajuster manuellement la Durée de la tâche.

Workfront suppose qu’il y a 8 heures de travail par jour. L’administrateur de Workfront ou de groupe définit les heures par jour de travail avec le paramètre Heures par jour de travail standard dans les préférences du projet dans Configuration. Pour plus d’informations sur la modification de votre tâche et les préférences de problème dans le cadre de vos préférences de projet au niveau du système, voir [ Configuration des préférences de tâche et de problème à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

>[!TIP]
>
>Workfront prend en compte le planning de chaque ressource affectée à la tâche afin de déterminer le pourcentage d’allocation pour chaque ressource de la tâche. Pour plus d’informations sur la création et l’affectation de plannings aux utilisateurs, voir [Création d’un planning](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

Examinez les scénarios suivants :

* [Les ressources sont affectées à 100 % à la tâche](#resources-are-allocated-100-to-the-task)
* [Les ressources sont affectées à divers pourcentages de temps à la tâche.](#resources-are-allocated-for-various-percentages-of-time-to-the-task)

### Les ressources sont affectées à 100 % à la tâche {#resources-are-allocated-100-to-the-task}

Cette formule suppose que toutes les ressources sont affectées à 100 % à la tâche.

```
Planned Duration = (Planned Hours / Number of Resources) / 8
```

Ce calcul suppose que le nombre d’heures par jour est de 8. L’équation inclut cette valeur, de sorte que la durée planifiée s’affiche en jours.

### Les ressources sont affectées à divers pourcentages de temps à la tâche. {#resources-are-allocated-for-various-percentages-of-time-to-the-task}

Chaque ressource affectée pouvant avoir un niveau d’affectation unique, la formule réelle prend en compte ces valeurs d’affectation :

```
Planned Duration = (Planned Hours / SUM(Percent allocation for each resource for the task)) / 8
```

Ce calcul suppose que le nombre d’heures par jour est de 8. L’équation inclut cette valeur, de sorte que la durée planifiée s’affiche en jours.

## Effet de l’ajout de ressources supplémentaires à une tâche

Lors de l’ajout ou de la suppression de personnes désignées dans une tâche avec le type de durée pilotée par l’effort, la durée et les heures planifiées ne changent pas. Toutefois, la durée planifiée change.

Dans l’exemple suivant, la mesure Heures par jour de travail standard est définie sur 8 dans les préférences du projet dans la configuration du système. Comme la durée est de 3 jours, les Heures planifiées sont définies sur 24 (3 jours x 8 heures par jour de travail = 24 Heures planifiées).

>[!NOTE]
>
>Lors de l’utilisation de la contrainte de tâche Dates fixes , la durée planifiée reste la même lorsque vous ajoutez ou supprimez des personnes désignées ; à la place, la durée et les heures planifiées sont ajustées. Lorsque vous utilisez une contrainte de tâche autre que des dates fixes, la durée planifiée est ajustée.

Le tableau suivant illustre la modification de la durée planifiée avec l’ajout de ressources à la tâche :

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th> <p><strong>Nombre de cessionnaires (chacun 100 % alloué)</strong> </p> </th> 
   <th> <p><strong>Durée</strong> </p> </th> 
   <th> <p><strong>Nombre d’heures prévues</strong> </p> </th> 
   <th><strong>Durée prévue</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> </td> 
   <td> <p>1</p> </td> 
   <td> <p>3 jours</p> </td> 
   <td> <p>24 heures</p> <p>(3 jours x 8 heures par jour de travail = 24 heures planifiées)</p> </td> 
   <td> <p>3 jours</p> <p>(24 heures planifiées / 1 cessionnaire = 3 jours)</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> <p>2</p> </td> 
   <td> <p>3 jours</p> </td> 
   <td> <p>24 heures</p> <p>(3 jours x 8 heures par jour de travail = 24 heures planifiées)</p> </td> 
   <td> <p>1,5 jour</p> <p>(24 heures planifiées / 2 cessionnaires = 12 heures ou 1,5 jour)</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> <p>3</p> </td> 
   <td> <p>3 jours</p> </td> 
   <td> <p>24 heures</p> <p>(3 jours x 8 heures par jour de travail = 24 heures planifiées)</p> </td> 
   <td> <p>1 jour</p> <p>(24 heures planifiées / 3 cessionnaires = 8 heures ou 1 jour)</p> </td> 
  </tr> 
 </tbody> 
</table>

## Remplacer le type de durée d’une tâche par Basé sur l’effort

Pour plus d’informations sur la modification du type de durée d’une tâche, voir [Mettre à jour le type de durée d’une tâche](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replaced with new article linked above)</p>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Go to a task for which you want to change the Duration Type.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Task Details</strong> in the left panel, then in the Overview area click <strong>Duration Type</strong>. </p> </li>
<li value="3"> <p>Select <strong>Effort Driven</strong> from the drop-down menu.</p> </li>
<li value="4">Click <strong>Save</strong><strong>Changes</strong>.</li>
</ol>
-->
