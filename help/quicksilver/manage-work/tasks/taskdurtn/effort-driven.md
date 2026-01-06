---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: 'Présentation du type de durée : piloté par l''effort'
description: « Piloté par l’effort » est un type de durée qui peut être défini pour une tâche dans Adobe Workfront. Pour des informations générales sur les types de durée dans Workfront, voir Vue d’ensemble de la durée de la tâche et du type de durée.
author: Alina
feature: Work Management
exl-id: 3c8534f7-02d0-4404-a37b-0ef6360e8efc
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '862'
ht-degree: 95%

---

# Vue d’ensemble du type de durée : « Piloté par l’effort »

« Piloté par l’effort » est un type de durée qui peut être défini pour une tâche dans Adobe Workfront. Pour des informations générales sur les types de durée dans Workfront, voir [Vue d’ensemble de la durée de la tâche et du type de durée](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

## Vue d’ensemble du type de durée « Piloté par l’effort »

Votre Workfront ou un administrateur de groupes peut définir le type de durée par défaut de votre système ou de votre groupe comme piloté par l&#39;effort. Dans ce cas, toutes les nouvelles tâches seront créées avec ce type de durée. Pour plus d’informations sur la modification de votre tâche et les préférences de problème dans le cadre de vos préférences de projet à l’échelle du système ou du groupe, voir [Configurer les préférences de tâche et de problème à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

Dans ce scénario, le risque de raccourcir arbitrairement le plan du projet existe, à moins que vous, en tant que personne responsable du projet, preniez le temps de déterminer si la tâche est réellement une tâche pilotée par l’effort.

Utilisez « Piloté par l’effort » pour ce qui suit :

* Déterminer la durée prévue en fonction du nombre de ressources disponibles pour travailler sur la tâche. La durée est égale aux nombre d’heures prévues. La durée prévue est égale au nombre d’heures prévues divisé par le nombre de personnes cessionnaires.

  Le niveau d’effort appliqué à la tâche détermine la répartition du travail et la durée.

* Suivez le nombre total d’heures passées sur une tâche lorsque plusieurs ressources sont affectées.

  Lorsque des ressources sont ajoutées, la durée prévue de la tâche diminue. (Le principe « l’union fait la force » illustre l’effet que ce type de durée a sur la durée prévue d’une tâche.)

Les sections suivantes fournissent des informations plus détaillées sur la façon dont Workfront calcule la durée prévue d’une tâche pilotée par l’effort et l’effet que l’ajout de ressources peut avoir sur la tâche avec ce type de durée.

## Vue d’ensemble de la formule du type de durée « Piloté par l’effort »

La formule de calcul de la durée prévue d’une tâche ayant un type de durée « Piloté par l’effort » dépend du pourcentage d’affectation de chaque ressource affectée à la tâche. Dans le cas d’une tâche pilotée par l’effort, Workfront calcule le nombre d’heures prévues de la tâche qui sont toujours identiques à la durée de la tâche :

```
Planned Hours (in hours) = Duration (in days)
```

Vous pouvez ajuster manuellement la durée de la tâche.

Workfront suppose qu’une journée de travail se compose de 8 heures de travail. L’administration de Workfront ou de groupes définit les heures par journée de travail avec le paramètre « Heures types par jour de travail » dans les préférences du projet dans la configuration. Pour plus d’informations sur la modification de vos préférences en matière de tâches et de problèmes dans le cadre des préférences de votre projet au niveau du système, consultez [Configurer les préférences en matière de tâches et de problèmes au niveau du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

>[!TIP]
>
>Workfront prend en compte le planning de chaque ressource affectée à la tâche afin de déterminer le pourcentage d’affectation pour chaque ressource de la tâche. Pour plus d’informations sur la création et l’affectation de plannings aux utilisateurs et aux utilisatrices, consultez la section [Créer un planning](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

Tenez compte des scénarios suivants :

* [Les ressources sont affectées à 100 % à la tâche.](#resources-are-allocated-100-to-the-task)
* [Les ressources sont affectées à la tâche selon différents pourcentages de temps.](#resources-are-allocated-for-various-percentages-of-time-to-the-task)

### Les ressources sont affectées à 100 % à la tâche. {#resources-are-allocated-100-to-the-task}

Cette formule suppose que toutes les ressources sont affectées à 100 % à la tâche.

```
Planned Duration = (Planned Hours / Number of Resources) / 8
```

Ce calcul suppose qu’une journée de travail normale se compose de 8 heures de travail. L’équation inclut cette valeur, de sorte que la durée prévue s’affiche en jours.

### Les ressources sont affectées à la tâche selon différents pourcentages de temps. {#resources-are-allocated-for-various-percentages-of-time-to-the-task}

Chaque ressource affectée pouvant avoir un niveau d’affectation unique, la formule réelle prend en compte les valeurs d’affectation suivantes :

```
Planned Duration = (Planned Hours / SUM(Percent allocation for each resource for the task)) / 8
```

Ce calcul suppose qu’une journée de travail normale se compose de 8 heures de travail. L’équation inclut cette valeur, de sorte que la durée prévue s’affiche en jours.

## Effet de l’ajout de ressources supplémentaires à une tâche

Lors de l’ajout ou de la suppression de personnes cessionnaires à une tâche avec le type de durée « Piloté par l’effort », la durée et les heures prévues ne changent pas. Toutefois, la durée prévue change.

Dans l’exemple suivant, la mesure du nombre d’heures types par jour de travail est définie sur 8 dans les préférences du projet dans la configuration du système. Comme la durée est de 3 jours, le nombre d’heures prévues est défini sur 24 (3 jours x 8 heures par journée de travail = 24 heures prévues).

>[!NOTE]
>
>Lors de l’utilisation de la contrainte de tâche « Dates fixes », la durée prévue reste la même lorsque vous ajoutez ou supprimez des personnes cessionnaires, mais la durée et les heures prévues sont ajustées. Lorsque vous utilisez une contrainte de tâche autre que des dates fixes, la durée prévue est ajustée.

Le tableau suivant illustre la modification de la durée prévue avec l’ajout de ressources à la tâche :

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th> <p><strong>Nombre de personnes cessionnaires (chacune attribuée à 100 %)</strong> </p> </th> 
   <th> <p><strong>Durée</strong> </p> </th> 
   <th> <p><strong>Nombre d’heures prévues</strong> </p> </th> 
   <th><strong>Durée prévue</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> </td> 
   <td> <p>1</p> </td> 
   <td> <p>3 jours</p> </td> 
   <td> <p>24 heures</p> <p>(3 jours x 8 heures par jour de travail = 24 heures prévues)</p> </td> 
   <td> <p>3 jours</p> <p>(24 heures prévues / 1 personne cessionnaire = 3 jours)</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> <p>2</p> </td> 
   <td> <p>3 jours</p> </td> 
   <td> <p>24 heures</p> <p>(3 jours x 8 heures par jour de travail = 24 heures prévues)</p> </td> 
   <td> <p>1,5 jour</p> <p>(24 heures prévues / 2 personnes assignées = 12 heures ou 1,5 jour)</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> <p>3</p> </td> 
   <td> <p>3 jours</p> </td> 
   <td> <p>24 heures</p> <p>(3 jours x 8 heures par jour de travail = 24 heures prévues)</p> </td> 
   <td> <p>1 jour</p> <p>(24 heures prévues / 3 personnes assignées = 8 heures ou 1 jour)</p> </td> 
  </tr> 
 </tbody> 
</table>

## Remplacer le type de durée d’une tâche par Piloté par l’effort

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
