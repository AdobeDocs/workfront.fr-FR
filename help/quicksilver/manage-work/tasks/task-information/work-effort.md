---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Vue d’ensemble de l’effort de travail
description: Vue d’ensemble de l’effort de travail
author: Alina
feature: Work Management
exl-id: 70f51e4b-43cc-427a-99e4-ebb056bb1070
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '1488'
ht-degree: 97%

---

# Vue d’ensemble de l’effort de travail

<!--Audited: 01/2024-->

<!--
(NOTE: Linked to the UI >> in the Project/ Template edit box > Tasks area> Learn more)
-->

En tant que personne gestionnaire de projet, vous pouvez choisir comment estimer la quantité de travail nécessaire à l’exécution des tâches dans un projet. Estimez la quantité de travail nécessaire à l’exécution des tâches à l’aide de l’un des indicateurs suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Heures prévues</td> 
   <td> <p> Saisie numérique manuelle ou calcul Adobe Workfront affichant le nombre d’heures nécessaires pour que les ressources affectées à une tâche la terminent. </p> <p>Tenez compte des points suivants concernant le nombre d’heures prévues : </p> 
    <ul> 
     <li>Il s’agit de la méthode par défaut. </li> 
     <li>Vous pouvez mettre à jour manuellement le nombre d’heures prévues uniquement pour les tâches dont le type de durée est Calcul d’affectation ou Simple. </li> 
    </ul> <p>Pour plus d’informations sur le nombre d’heures prévues, consultez la section <a href="../../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref">Vue d’ensemble du nombre d’heures prévues</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Effort de travail </td> 
   <td> <p>Libellé manuel qui définit si l’utilisateur ou l’utilisatrice doit fournir un effort de travail quotidien faible, moyen ou important pour terminer une tâche. <!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
       The level of effort is estimated to be a percentage of the daily amount of working time. (NOTE: keep this drafted. Vazgen said it's not needed, but waiting for feedback from users)
      </MadCap:conditionalText>
     --> </p> <p>Tenez compte des points suivants concernant l’effort de travail :</p> 
    <ul> 
     <li>Ce champ est disponible uniquement pour les tâches dont le type de durée est Simple. </li> 
     <li>Vous pouvez activer l’utilisation de ce libellé et définir le pourcentage de temps de travail qui lui est associé au niveau du projet. </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Cet article décrit l’effort de travail et explique comment l’utiliser pour estimer la quantité de travail pour vos tâches.

>[!NOTE]
>
>Le nombre d’heures prévues et l’effort de travail s’influencent mutuellement. La mise à jour du nombre d’heures prévues peut mettre à jour l’effort de travail, et la mise à jour de l’effort de travail peut mettre à jour le nombre d’heures prévues de la tâche.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Standard</p>
   <p>Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès aux projets et tâches</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations de gestion d’un projet et de ses tâches</p>  </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, consultez la section [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current: Plan </p>
   Or
   <p>New: Standard </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configuration</td> 
   <td> <p>Edit access to Projects and Tasks</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a project and its tasks</p>  </td> 
  </tr> 
 </tbody> 
</table>-->

## Observations relatives à l’utilisation de l’option Effort de travail

* Lorsque les tâches d’un projet comportent 0 heure prévue et que vous activez le paramètre Utiliser l’effort de travail pour calculer automatiquement le nombre d’heures prévues des tâches dans le projet, le niveau d’effort de travail par défaut associé est moyen. Le nombre d’heures prévues est automatiquement mis à jour pour les tâches dont le type de durée est Simple. Pour plus d’informations, consultez la section [Niveaux d’effort de travail](#levels-of-work-effort) dans cet article.
* Lorsque les tâches d’un projet comportent des heures prévues supérieures à 0 et que vous activez le paramètre Utiliser l’effort de travail pour calculer automatiquement le nombre d’heures prévues des tâches dans le projet, le niveau d’effort de travail est mis à jour en fonction du nombre d’heures prévues sans modifier le nombre d’heures prévues des tâches dont le type de durée est Simple. Pour plus d’informations, consultez la section [Calcul de l’effort de travail en fonction du nombre d’heures prévues dans Workfront](#how-workfront-calculates-work-effort-based-on-planned-hours) dans cet article.
* Lorsque les tâches d’un projet comportent 0 heure prévue et que vous activez le paramètre Utiliser l’effort de travail pour calculer automatiquement le nombre d’heures prévues des tâches dans le projet, puis que vous mettez à jour le niveau d’effort de travail de Moyen à Faible ou Important, les heures prévues sont également mises à jour. Pour plus d’informations, consultez la section [Calcul des heures prévues en fonction de l’effort de travail dans Workfront](#how-workfront-calculates-planned-hours-based-on-work-effort) dans cet article.
* Lorsque vous modifiez des tâches en ligne et que vous modifiez simultanément les champs Nombre d’heures prévues et Effort de travail d’une tâche, le nombre d’heures prévues est mis à jour avec la valeur que vous indiquez, tandis que l’effort de travail est calculé en fonction de votre nombre d’heures prévues mis à jour.
* Lorsque vous mettez à jour la valeur Effort de travail d’une tâche, la durée ne se calcule plus automatiquement en fonction du nombre d’heures prévues. Pour plus d’informations sur le calcul de la durée des tâches dont le type de durée est Simple, consultez la section [Vue d’ensemble du type de durée : Simple](../../../manage-work/tasks/taskdurtn/simple-duration-type.md).
* Lorsque vous modifiez le type de durée d’une tâche de Simple à n’importe quel autre type, le champ Effort de travail est masqué dans la tâche. Le nombre d’heures prévues reste inchangé.
* Vous ne pouvez pas mettre à jour le niveau d’effort de travail dans une tâche parent. Le niveau d’effort de travail d’une tâche parent est automatiquement calculé en fonction du nombre d’heures prévues des tâches, qui est un cumul de toutes les tâches enfants. Pour plus d’informations sur les tâches parents, consultez la section [Créer des sous-tâches](../../../manage-work/tasks/create-tasks/create-subtasks.md).

## Activer l’utilisation de l’effort de travail au lieu du nombre d’heures prévues

1. Accédez à un projet et cliquez sur le menu **Plus** ![icône Plus](assets/more-icon.png), puis sur **Modifier**.
1. Cliquez sur **Paramètres de la tâche**, puis sélectionnez l’option **Utiliser l’option Effort de travail pour calculer automatiquement les heures planifiées de la tâche**. Cette option est désélectionnée par défaut.

   ![Travail sur les projets](assets/nwe-work-effort-on-projects-350x182.png)

   Pour plus d’informations sur l’activation de l’utilisation de l’effort de travail sur un projet, voir la section « Paramètres des tâches » dans l’article [Modifier des projets](../../../manage-work/projects/manage-projects/edit-projects.md).

1. Cliquez sur **Tâches** dans le panneau de gauche, puis cliquez sur le nom d’une tâche pour y accéder.
1. Cliquez sur le menu **Plus** ![icône Plus](assets/more-icon.png), puis sur **Modifier**. Assurez-vous que la tâche possède un type de durée Simple.

   >[!TIP]
   >
   >Vous pouvez également mettre à jour l’effort de travail d’une tâche dans la section Détails de la tâche.

1. Dans la zone **Vue d’ensemble**, cliquez sur le menu déroulant Effort de travail pour corriger la quantité d’effort nécessaire pour accomplir la tâche.

   ![Tâche sur la page Modifier la tâche](assets/work-effort-on-edit-task-page-350x239.png)

   Pour plus d’informations sur la mise à jour du champ Effort de travail sur une tâche, consultez les articles suivants :

   * Section « Vue d’ensemble » de l’article [Modifier les tâches](../../../manage-work/tasks/manage-tasks/edit-tasks.md)
   * [Gérer des informations sur la tâche dans la zone Vue d’ensemble des détails de la tâche](../../../manage-work/tasks/manage-tasks/task-information-in-overview.md)

## Niveaux d’effort de travail {#levels-of-work-effort}

En tant que perosnne gestionnaire de projet, vous pouvez identifier trois niveaux d’effort de travail pour vos projets. Chaque niveau d’effort correspond à un pourcentage du temps quotidien dont les personnes ont besoin pour accomplir la tâche.

Lorsque vous définissez le niveau d’effort de travail, vous devez vous poser la question suivante : « Combien de temps une personne affectée à cette tâche doit-elle y consacrer quotidiennement pour la réaliser dans les délais ? »

Le tableau suivant illustre les niveaux possibles d’effort de travail et les pourcentages correspondants par défaut. En tant que gestionnaire de projet, vous pouvez adapter les pourcentages aux besoins de votre organisation. Vous effectuez cette opération lorsque vous modifiez un projet. Pour plus d’informations sur la modification des projets, voir [Modifier les projets](../../../manage-work/projects/manage-projects/edit-projects.md).

En tant qu’administrateur ou administratrice Workfront, vous définissez les Heures habituelles par journée de travail dans la zone Préférences du projet de la Configuration. Il s’agit du nombre d’heures quotidien considéré comme temps de travail. Pour plus d’informations sur la configuration des préférences de projet pour votre instance de Workfront, voir [Configurer les préférences de projet à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

>[!NOTE]
>
>Dans les exemples ci-dessous, nous supposons que l’administrateur ou l’administratrice Workfront a fixé les Heures habituelles par journée de travail à 8 heures.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Niveau d’effort de travail</td> 
   <td>Valeurs en pourcentage</td> 
  </tr> 
  <tr> 
   <td>Petite </td> 
   <td>Un petit niveau d’effort pour accomplir une tâche est défini comme 25 % des Heures habituelles par journée de travail. Cela signifie qu’une tâche à laquelle est attribué ce niveau d’effort de travail devrait prendre jusqu’à 2 heures par jour pour être accomplie en une journée. <code>(0.25*8=2)</code></td> 
  </tr> 
  <tr> 
   <td>Moyen</td> 
   <td> <p>Un niveau d’effort moyen pour accomplir une tâche est défini comme 50 % des Heures habituelles par journée de travail. Cela signifie qu’une tâche à laquelle est attribué ce niveau d’effort de travail doit prendre plus de 2 heures et moins de 6 heures pour être accomplie en une journée. <code>(0.50*80=4)</code> </p> <p>Note : lorsque le paramètre Utiliser l’effort de travail pour calculer automatiquement le nombre d’heures prévues d’une tâche est activé sur le projet, il s’agit du paramètre par défaut pour une tâche, si la tâche avait 0 heure prévue avant que ce paramètre ne soit activé. Le nombre d’heures prévues de la tâche est alors mis à jour à 4 heures. </p> </td> 
  </tr> 
  <tr> 
   <td>Grande</td> 
   <td>Un grand niveau d’effort pour l’accomplissement d’une tâche est défini comme 75 % des Heures habituelles par journée de travail. Cela signifie qu’une tâche à laquelle est attribué ce niveau d’effort de travail devrait prendre 6 heures ou plus pour être accomplie en une journée. <code>(0.75*8=6)</code></td> 
  </tr> 
 </tbody> 
</table>

## Calcul du nombre d’heures prévues en fonction de l’effort de travail par Workfront {#how-workfront-calculates-planned-hours-based-on-work-effort}

Lorsque vous activez le paramètre Utiliser l’option Effort de travail pour calculer automatiquement les heures planifiées de la tâche sur un projet, Workfront calcule le nombre d’heures prévues pour une tâche avec un type de durée Simple en utilisant la formule suivante :

```
Task Planned Hours = Number of days in task Duration * Work Effort percentage * Typical hours per work day
```

Par exemple, une tâche d’une durée de 3 jours et d’un effort de travail moyen compte 12 heures prévues,

```
Planned Hours = 3*4=12
```

avec une valeur des Heures habituelles par journée de travail de 8 heures.

>[!TIP]
>
>Lorsqu’une tâche est affectée à plusieurs ressources, le nombre d’heures prévues est réparti de manière égale entre chaque ressource pour chaque jour de la durée de la tâche.

## Calcul de l’effort de travail sur la base du nombre d’heures prévues par Workfront {#how-workfront-calculates-work-effort-based-on-planned-hours}

Lorsque vous activez le paramètre Utiliser l’option Effort de travail pour calculer automatiquement les heures planifiées de la tâche sur un projet et que vous avez déjà des heures prévues sur la tâche ou que vous modifiez le nombre d’heures prévues sur la tâche, Workfront met à jour la valeur de l’effort de travail.

Workfront utilise la formule suivante pour mettre à jour le niveau d’effort de travail en fonction du nombre d’heures prévues :

```
Work Effort level = Task Planned Hours / Duration / Typical hours per work day
```

Par exemple, si vous avez une tâche d’une durée de 2 jours et que vous mettez à jour le nombre d’heures prévues de 8 à 20 heures, l’effort de travail pour la tâche passe de Moyen à Grand :

```
Work Effort level = 20 / 2 / 8 = 125 % = Large
```

## Localiser l’effort de travail pour les tâches et les projets

* [Effort de travail pour les projets](#work-effort-for-projects)
* [Effort de travail pour les tâches](#work-effort-for-tasks)

### Effort de travail pour les projets {#work-effort-for-projects}

Vous pouvez localiser la section Effort de travail d’un projet dans la zone suivante :

* La zone Paramètres de la tâche dans la zone Modifier le projet

### Effort de travail pour les tâches {#work-effort-for-tasks}

Vous pouvez localiser le champ Effort de travail d’une tâche dans les zones suivantes :

* La zone Vue d’ensemble dans la zone Modifier la tâche
* Dans la zone Vue d’ensemble de la section Détails de la tâche, dans la zone Temps de travail
* Une liste de tâches ou un rapport
