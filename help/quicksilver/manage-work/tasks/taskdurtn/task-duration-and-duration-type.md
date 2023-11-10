---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: Présentation de la durée et du type de durée de la tâche
description: La durée de la tâche correspond à la différence entre la date de fin planifiée et la date de début planifiée de la tâche. La durée indique la période disponible pour que la tâche soit terminée.
author: Alina
feature: Work Management
recommendations: noDisplay, noCatalog
exl-id: c81e485a-7e8c-4907-8e6c-9991681c3541
source-git-commit: 48f46abab1958325aba6832b85247dc2c80f4e80
workflow-type: tm+mt
source-wordcount: '1380'
ht-degree: 2%

---

# Présentation de la durée et du type de durée de la tâche

La durée de la tâche correspond à la différence entre la date de fin planifiée et la date de début planifiée de la tâche. La durée indique la période disponible pour que la tâche soit terminée.

Le Type de durée d’une tâche identifie la relation entre le nombre de ressources affectées à une tâche, l’effort total et la Durée totale de la tâche.

## Présentation de la durée de la tâche

>[!NOTE]
>
>Lorsque vous prenez en compte le temps de pause du Principal cessionnaire sur un projet, les dates prévues de la tâche peuvent s’ajuster, mais la durée de la tâche reste la même. Pour plus d’informations sur la prise en compte du temps de pause du Principal cessionnaire lors de la planification d’un projet, voir  [Configuration des préférences de projet à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Si les dates de début et de fin réelles de la tâche ne correspondent pas au planning du projet, de la personne désignée principale ou au planning par défaut, la durée de la tâche est zéro.

**Exemple :** Si un planning commence à 9 heures et se termine à 12 heures et qu’une tâche est planifiée pour commencer à 14 heures et se terminer à 16 heures, la durée de la tâche est zéro.

Voici deux scénarios qui existent lors du calcul de la durée dans Adobe Workfront.

* Si la tâche est assignée à un utilisateur, Workfront utilise l’un des plannings suivants, dans cet ordre précis pour calculer la durée :

   1. Workfront prend en compte le planning de l’utilisateur.
   1. Si l’utilisateur n’est pas associé à un planning, Workfront prend en compte le planning du projet.
   1. Si le projet n’est pas associé à une planification, Workfront prend en compte le planning par défaut de votre système. Pour plus d’informations sur les plannings, voir [Création d’un planning](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* Si la tâche est affectée à plusieurs utilisateurs :

  Workfront prend en compte le planning du projet ou celui de la personne désignée principale.

  Votre administrateur Workfront détermine le planning utilisé par Workfront lorsqu’une tâche est affectée à plusieurs utilisateurs. Pour plus d’informations, voir [Configuration des préférences de projet à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

  Les étapes sont similaires au premier scénario après avoir compris quel planning Workfront utilise pour calculer la durée.

## Unités de temps pour la durée de la tâche

Vous pouvez indiquer la durée de la tâche à la fois au moment normal et au temps écoulé entre les dates de début planifié et de fin planifiée.

Lors de la mise à jour de la Durée des tâches dans une liste, vous pouvez utiliser les abréviations suivantes pour indiquer les unités de temps dans Workfront :

| Unité de temps | Abréviation |
|---|---|
| Minutes | L |
| Heures | h |
| Jours. Il s’agit du paramètre par défaut. | Dés |
| Semaines | S |
| Mois | M |
| Minutes écoulées | EM |
| Heures écoulées | EH |
| Jours écoulés | ED |
| Semaines écoulées | EW |
| Mois écoulés | ET |

{style="table-layout:auto"}

**Exemple :** Si vous souhaitez indiquer que la durée d’une tâche est de 3 jours écoulés, vous devez saisir &quot;3 DE&quot; dans le champ Durée d’une liste de tâches .  Vous pouvez également sélectionner l’option de votre choix pour l’unité de temps de la durée dans le menu déroulant disponible lors de la modification d’une tâche ou dans la section Détails de la tâche . Pour plus d’informations sur la modification des tâches, voir [Modifier les tâches](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: stays QS only forever; for the pictures below: make the first one classic at preview time and the second one stays QS always. The second one is yellow >> take out at 21.2 production!!)</p>
-->

![](assets/duration-elapsed-days-tasks-nwe-350x282.png)

Tenez compte des points suivants lorsque vous indiquez la durée d’une tâche :

* Le temps écoulé est une unité de temps pour la durée d’une tâche. Il s’agit de l’heure entre la date de début planifiée et la date de fin planifiée d’une tâche qui comprend les jours fériés, les week-ends et les heures de congé. En d&#39;autres termes, le temps écoulé est le passage des jours calendaires.
* Le temps régulier prend en compte les jours fériés, les week-ends et les jours de congé et les exclut de la Durée de la tâche.

* Lorsque vous indiquez la durée d’une tâche en semaines, Workfront calcule la durée en jours et heures en fonction des paramètres Type de jour de travail par semaine et Type d’heure par jour de travail définis par votre administrateur Workfront dans la zone Préférences du projet de la configuration.
* Workfront utilise la durée par défaut de 4 semaines pour un mois lors du calcul de la durée en mois.

## Présentation du type de durée de tâche

La gestion du type de durée d’une tâche vous permet de définir des affectations de ressources cohérentes en fonction des besoins de la tâche.

Le type de durée permet de répondre aux questions suivantes :

* À quel point allons-nous être occupés ?
* Quelle est la taille du travail ?
* Combien de temps cela va-t-il prendre ?

![duration_type_triangle.png](assets/duration-type-triangle-350x245.png)

## Définition des types de durée

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th scope="row">Type de durée </th> 
   <th scope="col"> <p><strong>Fonction</strong> </p> </th> 
   <th scope="col"> <p><strong>Comment les ressources l’affectent</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <th scope="col"> <p><strong>Calcul d'affectation</strong> </p> </th> 
   <td scope="col"> <p>Calcule le pourcentage d’allocation pour chaque personne désignée pour une tâche. </p> <p>Lorsque vous choisissez ce type de durée, vous pouvez saisir une durée et des heures planifiées individuelles pour la tâche. Workfront divise les Heures planifiées par le nombre d’heures qu’il y a à l’intérieur de la Durée de la tâche, puis par le nombre de ressources affectées à la tâche pour calculer l’allocation pour chaque personne désignée.</p> <p>Pour plus d’informations, voir <a href="../../../manage-work/tasks/taskdurtn/calculated-assignment.md" class="MCXref xref">Présentation du type de durée : Attribution calculée</a>.</p> </td> 
   <td scope="col">La durée et les heures planifiées ne changent pas lors de l’ajout ou de la suppression de personnes désignées dans la tâche. </td> 
  </tr> 
  <tr> 
   <th scope="col"> <p><strong>Calcul de travail</strong> </p> </th> 
   <td scope="col"> <p>Détermine les heures planifiées (quantité de travail) requises pour terminer la tâche.</p> <p>Normalement utilisé lorsque les ressources affectées à la tâche sont allouées pour toute la durée de la tâche.</p> <p>Lorsque vous choisissez ce type de durée, vous avez la possibilité de saisir une durée spécifique pour la tâche. Workfront calcule les Heures planifiées de la tâche en multipliant le nombre de jours dans la durée par le nombre d’heures de travail dans le planning et par le nombre de personnes désignées pour la tâche. </p> <p>Vous avez la possibilité de modifier manuellement le pourcentage d’affectation de chaque personne désignée par rapport à la tâche, ce qui réduit le nombre d’heures planifiées.</p> <p>Pour plus d’informations, voir <a href="../../../manage-work/tasks/taskdurtn/calculated-work.md" class="MCXref xref">Présentation du type de durée : travail calculé</a>.</p> </td> 
   <td scope="col"> <p>Les heures planifiées augmentent lorsque les personnes désignées sont ajoutées à la tâche. </p> <p>Les heures planifiées diminuent lorsque les personnes désignées sont retirées de la tâche.</p> </td> 
  </tr> 
  <tr> 
   <th scope="col"> <p>Piloté par l'effort</p> </th> 
   <td scope="col"> <p>Détermine les Heures planifiées en fonction du nombre de ressources.</p> <p>Lorsque vous choisissez ce type de durée, vous avez la possibilité de saisir une durée spécifique pour la tâche. Workfront calcule les Heures planifiées de la tâche en multipliant le nombre de jours dans la Durée par le nombre d’heures de travail dans le planning et en divisant cela par le nombre de personnes désignées pour la tâche. </p> <p>Vous avez la possibilité de modifier manuellement le pourcentage d’affectation de chaque personne désignée par rapport à la tâche, mais le nombre d’heures planifiées reste le même.</p> <p>Pour plus d’informations, voir <a href="../../../manage-work/tasks/taskdurtn/effort-driven.md" class="MCXref xref">Présentation du type de durée : piloté par l’effort</a>.</p> </td> 
   <td scope="col"> <p>Les heures planifiées augmentent lorsque les personnes désignées sont retirées de la tâche.</p> <p>Les heures planifiées diminuent lorsque des personnes désignées sont ajoutées à la tâche. </p> <p>La durée ne change pas, quel que soit le nombre de personnes désignées ou leur planning. </p> <p>La durée est égale aux heures planifiées. La durée planifiée est égale au nombre d’heures planifiées divisé par le nombre de personnes désignées.</p> </td> 
  </tr> 
  <tr> 
   <th scope="col"> <p><strong>Simple</strong> </p> </th> 
   <td scope="col"> <p>Détermine les heures planifiées et la durée (identiques pour ce type de durée) en fonction du nombre d’heures pendant lesquelles chaque personne désignée est allouée. </p> <p>Workfront calcule les Heures planifiées en additionnant les heures allouées prévues pour chaque personne désignée. </p> <p>Vous avez la possibilité de modifier manuellement le nombre d’heures alloué à chaque personne désignée, ainsi que le nombre d’heures planifiées et le montant de la durée, qui changent en conséquence. Si vous choisissez un nombre total d’heures allouées pour tous les cessionnaires, ce nombre est réparti uniformément entre chaque cessionnaire.</p> <p>Pour plus d’informations, voir <a href="../../../manage-work/tasks/taskdurtn/simple-duration-type.md" class="MCXref xref">Présentation du type de durée : simple</a>.</p> </td> 
   <td scope="col"> <p>Les heures sont réparties uniformément entre les personnes désignées si vous choisissez un nombre total d’heures allouées. Cependant, en tant que chef de projet, vous pouvez ajuster manuellement les heures de chaque responsable. </p> <p>Vous pouvez modifier les heures planifiées et la durée d’une tâche avec un type de durée simple intégré ou au niveau de la tâche. </p> <p>Si une équipe agile est affectée à une tâche, le type de durée est automatiquement défini sur Simple et ne peut pas être modifié. La durée de la tâche d’une équipe agile doit être supérieure à 0 minute.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Type de durée des nouvelles tâches

Le type de durée d’une nouvelle tâche correspond au type de durée configuré dans votre système. Le type de durée par défaut est Attribution calculée. Votre administrateur Workfront ou un administrateur de groupe peut mettre à jour le type de durée par défaut de votre système ou du groupe associé au projet. Pour plus d’informations, voir [Configuration des préférences de tâche et de problème à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

## Modification du type de durée d’une tâche

Pour plus d’informations sur la modification du type de durée d’une tâche, voir [Mise à jour du type de durée d’une tâche](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md).
