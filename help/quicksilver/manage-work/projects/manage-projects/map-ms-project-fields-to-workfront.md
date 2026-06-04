---
product-area: projects
navigation-topic: manage-projects
title: Mappage des champs de projet Microsoft aux projets Adobe Workfront
description: Les projets dans Adobe Workfront et Microsoft Project sont généralement compatibles. Cet article décrit comment les champs de projet les plus courants des deux applications se mappent les uns aux autres.
author: Alina
feature: Work Management
exl-id: 381eb6ad-8084-406b-90f9-44460b58a04c
TQID: https://experienceleague.adobe.com/WdFf5O8kKyY43PsHLEINDaLzsEa0idHZPNz83O12bTI
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 396
ht-degree: 84%

---

# Mapper des champs Microsoft Project à des projets Adobe Workfront

Les projets dans Adobe Workfront et Microsoft Project sont généralement compatibles. Les deux applications vous permettent d’effectuer les opérations suivantes :

* Exporter des projets à partir de Microsoft Project et les importer dans Workfront
* Exporter des projets à partir de Workfront et les importer dans Microsoft Project.

Pour plus d’informations sur l’import de projets de Microsoft Project dans Workfront, voir [Importer un projet à partir de Microsoft Project](../../../manage-work/projects/create-projects/import-project-from-ms-project.md).

Pour plus d’informations sur l’export d’un projet à partir de Workfront pour l’importer dans Microsoft Project, voir [Exporter un projet vers Microsoft Project](../../../manage-work/projects/manage-projects/export-project-to-ms-project.md).

Lors de ces imports de données, il est important de comprendre comment les informations se transforment d’une application à l’autre. La plupart du temps, vous devrez apporter des modifications manuelles au projet, une fois l’import terminé.

## Vue d’ensemble du mapping des champs

>[!NOTE]
>
>Les dates prévues ne correspondent pas toujours entre les deux systèmes. Les écarts peuvent être pris en compte par le planning et les différences de préférences système entre Workfront et Microsoft Project. Ces incohérences de date peuvent également entraîner des différences d’effort, de durée et de pourcentage d’achèvement.

| **Champ Microsoft Project** | **Champ Workfront** |
|---|---|
| Titre du projet | Nom du projet |
| Dates de début et de fin | Dates de début et de fin prévues |
| Nom de la tâche | Nom de la tâche |
| Durée de la tâche | Durée prévue de la tâche |
| Travail de la tâche | Nombre d’heures prévues de la tâche |
| % de tâche terminé | Pourcentage terminé de la tâche (selon la durée de la tâche) |
| % de travail de tâche terminé | Pourcentage terminé de la tâche (selon le nombre d’heures prévues de la tâche) |
| Début et fin planifiés | Dates de début et de fin prévues |
| Début et fin réels | Dates de début et d&#39;achèvement effectives |
| Nom de la ressource | Affectation de la tâche |
| Unités d’affectation | Pourcentage d’attribution d’affectation |
| Note de la tâche | Description de la tâche |
| Tâche antérieure | Tâche antérieure |

## Vue d’ensemble des données non incluses

Un certain nombre de champs de projet ne sont ni importés ni exportés depuis Workfront.

Ces champs comprennent, sans s’y limiter, les éléments suivants :

* Pièces jointes du document
* Champs personnalisés (au niveau du projet ou de la tâche)
* Notes Workfront
* Problèmes
* Décalage négatif dans les tâches avec une relation antérieure Démarrer/Terminer (les tâches sont importées sans le décalage)
* Affectations
* Contraintes de tâche

  >[!NOTE]
  >
  >Comme les contraintes ne correspondent pas entre Microsoft Project et Workfront, assurez-vous qu’il existe des relations antérieures entre les tâches. Dans le cas contraire, les dates de début et d’achèvement prévues des tâches peuvent ne pas être exactes dans le projet importé.
