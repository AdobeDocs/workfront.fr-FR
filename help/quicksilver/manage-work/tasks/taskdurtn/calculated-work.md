---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: 'Vue d''ensemble du type de durée : Travail calculé'
description: Le calcul de travail est un type de durée que vous pouvez définir pour une tâche dans Adobe Workfront. Pour des informations générales sur les types de durée dans Workfront, voir Vue d’ensemble de la durée de la tâche et du type de durée.
author: Alina
feature: Work Management
exl-id: f521c2f5-8d58-44c0-af18-6940ad0950ea
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '568'
ht-degree: 92%

---

# Vue d’ensemble du type de durée : calcul de travail

Le calcul de travail est un type de durée que vous pouvez définir pour une tâche dans Adobe Workfront. Pour des informations générales sur les types de durée dans Workfront, voir [Vue d’ensemble de la durée de la tâche et du type de durée](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

## Vue d’ensemble du type de durée Calcul de travail

Le calcul de travail détermine la quantité de travail (nombre d’heures prévues) nécessaire pour que la tâche soit terminée. Nous vous recommandons d’utiliser le type durée Calcul de travail lorsque les ressources affectées à la tâche sont allouées pour toute la durée de la tâche.

Votre Workfront ou un administrateur de groupes peut définir le type de durée par défaut de votre système ou de votre groupe comme Travail calculé. Dans ce cas, toutes les nouvelles tâches seront créées avec ce type de durée. Pour plus d’informations sur la modification de votre tâche et les préférences de problème dans le cadre de vos préférences de projet à l’échelle du système ou du groupe, voir [Configurer les préférences de tâche et de problème à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

À mesure que des ressources sont ajoutées à une tâche, la personne responsable du projet peut s’attendre à une augmentation de l’effort prévu. Pour illustrer cela, une réunion de planification d’une heure avec trois ressources représente un nombre total de trois heures de travail requises, et une réunion de planification d’une heure avec dix ressources représente dix heures de travail requises. Cela suppose que chaque ressource est affectée à la tâche avec une affectation de 100 %.

## Examiner la formule de calcul du travail requis lors de l’utilisation du type de durée Calcul de travail

Lorsque vous utilisez le type de durée Calcul de travail sur une tâche, Workfront calcule la quantité de travail pour chaque tâche à l’aide des deux formules suivantes. Les formules diffèrent selon le pourcentage de temps consacré à chaque ressource et le nombre de ressources affectées à chaque tâche :

* Formule simplifiée : en supposant qu’une ressource soit affectée à la tâche et qu’elle soit affectée à la tâche pour 100 % de son temps disponible, la valeur Travail requis pour chaque tâche est calculée à l’aide de la formule suivante :

```
Work Required (Planned Hours) = (Duration of the task in hours) x (The number of resources assigned to the task)
```

* Formule complexe : si vous attribuez chaque ressource avec différentes affectations, la formule prend en compte ces affectations et tient compte de ces variations :

```
Work Required (Planned Hours) = SUM[(Duration of the task in hours) x (Percent allocated towards tasks for each resource)]
```

## Examiner l’effet de l’ajout ou de la suppression de ressources de la tâche

Lors de l’ajout ou de la suppression de personnes cessionnaires à une tâche avec le type de durée Calcul de travail, la durée peut être modifiée manuellement. Lorsque des personnes cessionnaires sont ajoutées ou supprimées de la tâche, le nombre d’heures prévues change.

Dans l’exemple suivant, la mesure Heures habituelles par journée de travail est définie sur 8 dans les préférences du projet dans Configuration. Chaque tâche a une durée d’un jour. À mesure que le nombre de personnes cessionnaires change, le nombre d’heures prévues change en fonction du nombre de personnes cessionnaires pour une tâche donnée :

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Nombre de personnes cessionnaires (affectées à 100 % chacune)</strong> </p> </th> 
   <th> <p><strong>Durée</strong> </p> </th> 
   <th> <p><strong>Nombre d’heures prévues</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>1</p> </td> 
   <td> <p>1 jour</p> </td> 
   <td> <p>8 heures</p> <p>(1 jour x 8 heures par jour de travail x 1 personne cessionnaire = 8 heures prévues)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>2</p> </td> 
   <td> <p>1 jour</p> </td> 
   <td> <p>16 heures</p> <p>(1 jour x 8 heures par jour de travail x 2 personnes cessionnaires = 16 heures prévues)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>3</p> </td> 
   <td> <p>1 jour</p> </td> 
   <td> <p>24 heures</p> <p>(1 jour x 8 heures par jour de travail x 3 personnes cessionnaires = 24 heures prévues)</p> </td> 
  </tr> 
 </tbody> 
</table>

Dans ce cas, chaque personne cessionnaire est affectée à 100 % à la tâche de Calcul de travail.

![Type de durée de travail calculée](assets/calcwork-350x71.png)

## Modifier le type de durée d’une tâche en Calcul de travail

Pour plus d’informations sur la modification du type de durée d’une tâche, voir [Mettre à jour le type de durée d’une tâche](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replaced with new article linked above)</p>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Go to a task for which you want to change the Duration Type.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Task Details</strong> in the left panel, then in the Overview area double click <strong>Duration Type</strong>. </p> </li>
<li value="3">Select <strong>Calculated Work</strong> from the drop-down menu.</li>
<li value="4">Click <strong>Save</strong> <strong>Changes</strong>.</li>
</ol>
-->
