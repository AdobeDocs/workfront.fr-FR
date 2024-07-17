---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Vue d’ensemble de la durée du projet
description: Adobe Workfront calcule la Durée d’un projet en prenant en compte la Date de début de la première tâche et la Date de fin de la dernière tâche et comptabilise le nombre de jours entre les deux dates.
author: Alina
feature: Work Management
exl-id: b558eaad-669b-4079-b61a-07df227edfa2
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 3%

---

# Vue d’ensemble de la durée du projet

Adobe Workfront calcule la Durée d’un projet en prenant en compte la Date de début de la première tâche et la Date de fin de la dernière tâche et comptabilise le nombre de jours entre les deux dates.

## Durée du projet

La Durée du projet est calculée selon la formule suivante :

```
Project Duration = Completion Date of the latest task - Start Date of the earliest task
```

>[!NOTE]
>
>La durée des problèmes sur le projet n’a aucune incidence sur la durée du projet.

La durée du projet compte le nombre de jours entre les deux dates de la tâche, en fonction du planning associé au projet ou des utilisateurs affectés aux tâches. Pour plus d’informations sur la planification utilisée par Workfront pour calculer la durée, voir [Aperçu des planifications](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/schedules-overview.md).

## Types de durée du projet

Il existe deux types de durée du projet et les formules selon lesquelles Workfront les calcule :

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Check these formulas? Should they be divided by the hours per day?!) </p>
-->

* **Durée planifiée** : 

  ```
  Project Planned Duration = Planned Completion Date of the latest task - Planned Start Date of the earliest task / Typical hour per day
  ```

* **Durée réelle** : 

  ```
  Project Actual Duration = Actual Completion Date of the latest task - Actual Start Date of the earliest task / Typical hour per day
  ```

## Localisation de la durée du projet

Vous pouvez localiser les Durée planifiée et Durée réelle du projet dans les zones suivantes de Workfront :

* . Dans la zone Détails du projet, dans la section Aperçu .

  Pour plus d’informations sur le sous-onglet Aperçu d’un projet, consultez l’article [Gérer les informations dans la zone Aperçu du projet](../../../manage-work/projects/manage-projects/understand-project-overview-area.md).

* Dans un rapport Projet , en incluant les champs Durée ou Durée réelle dans le rapport.

  Pour plus d’informations sur la création de rapports, consultez l’article [Créer un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
