---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: Vue d’ensemble de la durée des tâches et du type de durée
description: La durée de la tâche correspond à la différence entre sa date de début prévue et sa date d’achèvement prévue. La durée indique le délai dont dispose la tâche pour être achevée.
author: Alina
feature: Work Management
recommendations: noDisplay, noCatalog
exl-id: c81e485a-7e8c-4907-8e6c-9991681c3541
source-git-commit: b42436ad660642bd23638a8a44d9561513d748ed
workflow-type: tm+mt
source-wordcount: '1791'
ht-degree: 68%

---

# Vue d’ensemble de la durée des tâches et du type de durée

<!-- Audited: 12/2023 -->

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de manière générale. Il est disponible uniquement dans l’environnement Aperçu pour tous les clients. Après les versions mensuelles de Production, les mêmes fonctionnalités sont également disponibles dans l’environnement Production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation de versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

La durée de la tâche correspond à la différence entre sa date de début prévue et sa date d’achèvement prévue. La durée indique le délai dont dispose la tâche pour être achevée.

Le type de durée d’une tâche identifie la relation entre le nombre de ressources affectées à une tâche, l’effort total et la durée totale de la tâche.

## Vue d’ensemble de la durée de la tâche

Si les dates de début et d’achèvement effectives de la tâche ne correspondent pas au planning du projet, de la personne cessionnaire principale, ou au planning par défaut, la durée de la tâche est zéro.

>[!BEGINSHADEBOX]

**EXEMPLE**
Si un planning commence à 9 heures et se termine à 12 heures et qu’une tâche est planifiée pour commencer à 14 heures et se terminer à 16 heures, la durée de la tâche est zéro.


>[!ENDSHADEBOX]

Voici deux scénarios qui existent lors du calcul de la durée dans Adobe Workfront :

* Si la tâche est assignée à un utilisateur, les scénarios suivants existent en fonction de l’environnement que vous utilisez :

   * Dans l’environnement de production, Workfront utilise l’un des plannings suivants, dans cet ordre exact de calcul de la durée :

   1. Workfront prend en compte le planning de l’utilisateur ou de l’utilisatrice.
   1. Si la personne n’est pas associée à un planning, Workfront prend en compte le planning du projet.
   1. Si le projet n’est pas associé à un planning, Workfront prend en compte le planning par défaut de votre système. Pour plus d’informations sur les plannings, voir [Créer un planning](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

<div class="preview">

* Dans l’environnement Aperçu :

   1. Workfront prend en compte le planning du projet ou celui de l’utilisateur affecté à la tâche.

      L’administrateur de Workfront ou de groupe détermine le planning utilisé par Workfront lorsqu’une tâche est affectée à un utilisateur. Pour plus d’informations, voir [Configurer des préférences de projet à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   1. Si l’utilisateur ou le projet ne dispose pas de planning, Workfront utilise le planning par défaut du système.

      Les étapes sont similaires au premier scénario après avoir compris quel planning Workfront utilise pour calculer la durée.

</div>

* Si la tâche est affectée à plusieurs utilisateurs et utilisatrices :

   1. Workfront prend en compte le planning du projet ou celui de la personne cessionnaire principale.

      L’administrateur de Workfront ou de groupe détermine le planning utilisé par Workfront lorsqu’une tâche est affectée à plusieurs utilisateurs. Pour plus d’informations, voir [Configurer des préférences de projet à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   1. Si la personne désignée principale ou le projet ne dispose pas de planification, Workfront utilise la planification par défaut du système.

  Les étapes sont similaires au premier scénario après avoir compris quel planning Workfront utilise pour calculer la durée.

>[!NOTE]
>
>Lorsque vous prenez en compte les congés de la personne cessionnaire principale sur un projet, les dates prévues de la tâche peuvent s’ajuster, mais la durée de la tâche reste la même. Pour plus d’informations sur la prise en compte des congés de la personne cessionnaire principale lors de la planification d’un projet, voir [Configurer les préférences des projets à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## Unités de temps pour la durée de la tâche

Vous pouvez indiquer la durée de la tâche à la fois au moment normal et au temps écoulé entre les dates de début planifié et de fin planifiée.

Lors de la mise à jour de la durée des tâches dans une liste, vous pouvez utiliser les abréviations suivantes pour indiquer les unités de temps dans Workfront :

| Unité de temps | Abréviation |
|---|---|
| Minutes | L |
| Heures | H |
| Jours.Il s’agit du paramètre par défaut. | Dés |
| Semaines | S |
| Mois | T, MO |
| Minutes écoulées | ME |
| Heures écoulées | HE |
| Jours écoulés | JE |
| Semaines écoulées | SE |
| Mois écoulés | TE |

{style="table-layout:auto"}

>[!BEGINSHADEBOX]

**EXEMPLE**

Si vous souhaitez indiquer que la durée d’une tâche est de 3 jours écoulés, vous devez saisir &quot;3 DE&quot; dans le champ Durée d’une liste de tâches .  Vous pouvez également sélectionner l’option de votre choix pour l’unité de temps de la durée dans le menu déroulant disponible lors de la modification d’une tâche ou dans la section Détails de la tâche . Pour plus d’informations sur la modification des tâches, consultez [Modifier les tâches](../../../manage-work/tasks/manage-tasks/edit-tasks.md).


>[!ENDSHADEBOX]

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: stays QS only forever; for the pictures below: make the first one classic at preview time and the second one stays QS always. The second one is yellow >> take out at 21.2 production!!)</p>
-->

![](assets/duration-elapsed-days-tasks-nwe-350x282.png)

Tenez compte des points suivants lorsque vous indiquez la durée d’une tâche :

* Le temps écoulé est une unité de temps pour la durée d’une tâche. Il s’agit de la durée entre la date de début et la date d’achèvement prévues d’une tâche qui comprend les jours fériés, les week-ends et les jours de congé. En d’autres termes, le temps écoulé est le nombre de jours calendaires écoulés.
* Les jours représentent les jours de travail définis dans le système et configurables dans la zone Configuration . Dans la plupart des cas, une journée consiste en 8 heures.
* L’heure normale (jours ou jours de travail) prend en compte les jours fériés, les week-ends et les jours de congé et les exclut de la durée de la tâche.
* Lorsque vous indiquez la durée d’une tâche en semaines, Workfront calcule la durée en jours et heures en fonction des paramètres Type de jour de travail par semaine et Type d’heure par jour de travail définis par votre administrateur Workfront dans la zone Préférences du projet de la configuration.
* Workfront utilise la durée par défaut de 4 semaines pour un mois lors du calcul de la durée en mois.

## Vue d’ensemble du type de durée des tâches

La gestion du type de durée d’une tâche vous permet de définir des affectations de ressources cohérentes en fonction des besoins de la tâche.

Le type de durée permet de répondre aux questions suivantes :

* Quelle sera la charge de travail ?
* Quelle est l’ampleur du travail ?
* Combien de temps cela va-t-il prendre ?

![duration_type_triangle.png](assets/duration_type_triangle.png)

## Définir les types de durée

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th scope="row"><p><strong>Type de durée</strong></p></th> 
   <th scope="col"> <p><strong>Fonction</strong> </p> </th> 
   <th scope="col"> <p><strong>Effet des ressources</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <th scope="col"> <p><strong>Calcul d’affectation</strong> </p> </th> 
   <td scope="col"> <p>Calcule le pourcentage d’affectation pour chaque personne cessionnaire d’une tâche. </p> <p>Lorsque vous choisissez ce type de durée, vous pouvez saisir une durée et des heures prévues individuelles pour la tâche. Workfront divise les heures prévues par le nombre d’heures de la durée de la tâche, puis par le nombre de ressources affectées à la tâche afin de calculer l’allocation pour chaque personne cessionnaire.</p> <p>Pour plus d’informations, consultez <a href="../../../manage-work/tasks/taskdurtn/calculated-assignment.md" class="MCXref xref">Vue d’ensemble du type de durée : calcul d’affectation</a>.</p> </td> 
   <td scope="col">La durée et les heures prévues ne changent pas lors de l’ajout ou de la suppression de personnes cessionnaires dans la tâche. </td> 
  </tr> 
  <tr> 
   <th scope="col"> <p><strong>Calcul de travail</strong> </p> </th> 
   <td scope="col"> <p>Détermine les heures prévues (quantité d’effort) requises pour effectuer la tâche.</p> <p>Normalement utilisé lorsque les ressources affectées à la tâche sont allouées pour toute la durée de la tâche.</p> <p>Lorsque vous choisissez ce type de durée, vous avez la possibilité de saisir une durée spécifique pour la tâche. Workfront calcule les heures prévues pour la tâche en multipliant le nombre de jours dans la durée par le nombre d’heures de travail dans le planning et par le nombre de personnes cessionnaires pour la tâche. </p> <p>Vous avez la possibilité de modifier manuellement le pourcentage d’affectation de chaque personne cessionnaire par rapport à la tâche, ce qui réduit le nombre d’heures prévues.</p> <p>Pour plus d’informations, consultez <a href="../../../manage-work/tasks/taskdurtn/calculated-work.md" class="MCXref xref">Vue d’ensemble du type de durée : calcul de travail</a>.</p> </td> 
   <td scope="col"> <p>Les heures prévues augmentent lorsque des personnes cessionnaires sont ajoutées à la tâche. </p> <p>Les heures prévues diminuent lorsque des personnes cessionnaires sont retirées de la tâche.</p> </td> 
  </tr> 
  <tr> 
   <th scope="col"> <p><strong>Piloté par l'effort</strong></p> </th> 
   <td scope="col"> <p>Détermine les heures prévues en fonction du nombre de ressources.</p> <p>Lorsque vous choisissez ce type de durée, vous avez la possibilité de saisir une durée spécifique pour la tâche. Workfront calcule les heures prévues pour la tâche en multipliant le nombre de jours de la durée par le nombre d’heures de travail dans le planning et en divisant par le nombre de personnes cessionnaires pour la tâche. </p> <p>Vous avez la possibilité de modifier manuellement le pourcentage d’affectation de chaque personne cessionnaire pour la tâche, mais le nombre d’heures prévues reste le même.</p> <p>Pour plus d’informations, consultez <a href="../../../manage-work/tasks/taskdurtn/effort-driven.md" class="MCXref xref">Vue d’ensemble du type de durée : piloté par l’effort</a>.</p> </td> 
   <td scope="col"> <p>Les heures prévues augmentent lorsque des personnes cessionnaires sont retirées de la tâche.</p> <p>Les heures prévues diminuent lorsque des personnes cessionnaires sont ajoutées à la tâche. </p> <p>La durée ne change pas, même si un changement est apporté au nombre de personnes cessionnaires ou à leur planning. </p> <p>La durée est égale aux nombre d’heures prévues. La durée prévue est égale au nombre d’heures prévues divisé par le nombre de personnes cessionnaires.</p> </td> 
  </tr> 
  <tr> 
   <th scope="col"> <p><strong>Simple</strong> </p> </th> 
   <td scope="col"> <p>Détermine les heures prévues et la durée (identiques pour ce type de durée) en fonction du nombre d’heures allouées pour chaque personne cessionnaire. </p> <p>Workfront calcule les heures prévues en additionnant les heures allouées prévues pour chaque personne cessionnaire. </p> <p>Vous avez la possibilité de modifier manuellement le nombre d’heures allouées à chaque personne cessionnaire ; le nombre d’heures prévues et la durée changent en conséquence. Si vous choisissez un nombre total d’heures affectées pour toutes les personnes cessionnaires, ce nombre est réparti uniformément entre elles.</p> <p>Pour plus d’informations, voir la section <a href="../../../manage-work/tasks/taskdurtn/simple-duration-type.md" class="MCXref xref">Vue d’ensemble du type de durée : simple</a>.</p> </td> 
   <td scope="col"> <p>Les heures sont réparties uniformément entre les personnes cessionnaires si vous choisissez un nombre total d’heures affectées. Cependant, en tant que personne responsable de projet, vous pouvez ajuster manuellement les heures de chaque personne cessionnaire. </p> <p>Vous pouvez modifier les heures planifiées et la durée d’une tâche avec un type de durée simple, en ligne ou au niveau de la tâche. </p> <p>Si une équipe Agile est affectée à une tâche, le type de durée est automatiquement défini sur Simple et ne peut pas être modifié. La durée de la tâche d’une équipe Agile doit être supérieure à 0 minute.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Type de durée des nouvelles tâches

Le type de durée d’une nouvelle tâche correspond au type de durée configuré dans votre système. Le type de durée par défaut est Calcul d’affectation. Votre équipe d’administration Workfront ou de groupes peut mettre à jour le type de durée par défaut de votre système ou du groupe associé au projet. Pour plus d’informations, voir la section [Configurer des préférences de tâche et de problème à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

## Durée d’origine d’une tâche parent

La Durée d’origine d’une tâche est la Durée qu’une tâche avait à l’origine avant de devenir une tâche mère, en minutes.

Lorsqu’une tâche devient un parent, la durée entre la date de début prévue du premier enfant et la date d’achèvement prévue du dernier enfant est reportée sur la tâche parent et devient la durée de la tâche parent. Cela remplace la durée de la tâche originale.

Lorsque les enfants utilisent l’unité de durée des jours écoulés et que leur parent utilise l’unité de durée des jours, il peut y avoir des incohérences dans la façon dont Workfront calcule la durée de la tâche parent.

Tenez compte des points suivants :

* L’unité de durée Jours écoulés représente les jours calendaires, qui se composent toujours de 24 heures par jour.
* L’unité de durée Jours représente le jour de travail défini dans le système et peut être configuré. Dans la plupart des cas, il se compose de 8 heures par jour.
* La formule de calcul de la durée de la tâche mère est la suivante :

  `Parent task duration = Planned Completion Date of the child task that is planned to end the latest - Planned Start Date of the child task that starts the earliest`

* Lors du calcul de la durée de la tâche mère, le système calcule d&#39;abord la durée selon la formule ci-dessus, puis applique le planning.


Pour plus d’informations, voir [Présentation de la tâche Durée d’origine et Heures planifiées originales](/help/quicksilver/manage-work/tasks/task-information/task-original-duration-and-original-planned-hours.md).

## Modifier le type de durée d’une tâche

Pour plus d’informations sur la modification du type de durée d’une tâche, voir la section [Mettre à jour le type de durée d’une tâche](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md).
