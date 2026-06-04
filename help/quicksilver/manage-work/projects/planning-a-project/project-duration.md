---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Présentation de la durée du projet
description: Adobe Workfront calcule la durée d’un projet en prenant en compte la date de début de la tâche la plus ancienne et la date d’achèvement de la tâche la plus récente et compte le nombre de jours entre ces deux dates.
author: Alina
feature: Work Management
exl-id: b558eaad-669b-4079-b61a-07df227edfa2
TQID: https://experienceleague.adobe.com/1j0nj2W5f7FtgIk46G3ePFA-zwt7VAyV9fQWKm2kZJ4
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: ce22a157-dd2c-405f-b740-c2f204bb4c1aid: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 254
ht-degree: 96%

---

# Vue d’ensemble de la durée du projet

Adobe Workfront calcule la durée d’un projet en prenant en compte la date de début de la tâche la plus ancienne et la date d’achèvement de la tâche la plus récente et compte le nombre de jours entre ces deux dates.

## Durée du projet

La durée du projet est calculée selon la formule suivante :

```
Project Duration = Completion Date of the latest task - Start Date of the earliest task
```

>[!NOTE]
>
>La durée des problèmes liés au projet n’affecte pas la durée du projet.

La durée du projet compte le nombre de jours entre les deux dates de la tâche en fonction du planning associé au projet ou des utilisateurs et utilisatrices affectés aux tâches. Pour plus d’informations sur la planification utilisée par Workfront pour calculer la durée, voir [Vue d’ensemble des plannings](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/schedules-overview.md).

## Types de durée de projet

Il existe deux types de durée de projet, voici les formules par lesquelles Workfront les calcule :

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Check these formulas? Should they be divided by the hours per day?!) </p>
-->

* **Durée prévue** :

  ```
  Project Planned Duration = Planned Completion Date of the latest task - Planned Start Date of the earliest task / Typical hour per day
  ```

* **Durée effective** :

  ```
  Project Actual Duration = Actual Completion Date of the latest task - Actual Start Date of the earliest task / Typical hour per day
  ```

## Localiser la durée du projet

Vous pouvez localiser les durées prévues et effectives du projet dans les zones suivantes de Workfront :

* . Dans la zone Détails du projet, dans la section Vue d’ensemble.

  Pour plus d’informations sur le sous-onglet Vue d’ensemble d’un projet, voir l’article [Gérer les informations dans la zone Vue d’ensemble du projet](../../../manage-work/projects/manage-projects/understand-project-overview-area.md).

* Dans un rapport de projet, en incluant les champs Durée ou Durée effective dans le rapport.

  Pour plus d’informations sur la création de rapports, voir l’article [Créer un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
