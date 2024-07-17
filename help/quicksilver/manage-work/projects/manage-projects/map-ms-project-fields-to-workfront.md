---
product-area: projects
navigation-topic: manage-projects
title: Mapper des champs Microsoft Project à des projets Adobe Workfront
description: Les projets dans Adobe Workfront et Microsoft Project sont généralement compatibles. Cet article décrit comment les champs de projet les plus courants des deux applications se mappent les uns aux autres.
author: Alina
feature: Work Management
exl-id: 381eb6ad-8084-406b-90f9-44460b58a04c
source-git-commit: c566eb094e96abca6073554433434822c567bc34
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 8%

---

# Mapper des champs Microsoft Project à des projets Adobe Workfront

Les projets dans Adobe Workfront et Microsoft Project sont généralement compatibles. Les deux applications vous permettent d’effectuer les opérations suivantes :

* Exportation de projets à partir de Microsoft Project et importation dans Workfront
* Exportez des projets à partir de Workfront et importez-les dans Microsoft Project. 

Pour plus d’informations sur l’importation de projets de Microsoft Project dans Workfront, voir [Importation d’un projet à partir d’un projet Microsoft](../../../manage-work/projects/create-projects/import-project-from-ms-project.md).

Pour plus d’informations sur l’exportation d’un projet à partir de Workfront pour l’importer dans le projet Microsoft, voir [Exportation d’un projet vers le projet Microsoft](../../../manage-work/projects/manage-projects/export-project-to-ms-project.md).

Lors de ces importations de données, il est important de comprendre comment les informations se transforment d’une application à l’autre. La plupart du temps, vous devrez apporter des modifications manuelles au projet, une fois l’importation terminée. 

## Présentation du mapping des champs

>[!NOTE]
>
>Les dates prévues ne correspondent pas toujours entre les deux systèmes. Les écarts peuvent être pris en compte par la planification et les différences de préférences système entre Workfront et Microsoft Project. Ces écarts de dates peuvent également entraîner des différences dans l’effort, la durée et le pourcentage de réussite.

| **Champ de projet Microsoft** | **Champ Workfront** |
|---|---|
| Titre du projet | Nom du projet |
| Dates de début et de fin | Dates de début et de fin planifiées |
| Nom de la tâche | Nom de la tâche |
| Durée de la tâche | Durée planifiée de la tâche |
| Tâche | Heures planifiées de la tâche |
| Tâche % terminée | Task % Complete (selon la durée de la tâche) |
| Tâche % terminée | Tâche % terminée (en fonction des heures planifiées de la tâche) |
| Début et fin planifiés | Dates de début et de fin planifiées |
| Début et fin réels | Dates de début et de fin réelles |
| Resource Name | Affectation de tâche |
| Unités d&#39;affectation | Pourcentage d’affectation |
| Note de tâche | Description de la tâche |
| Tâche antérieure | Tâche antérieure |

## Présentation des données non incluses

Un certain nombre de champs de projet ne sont pas importés ou exportés depuis Workfront.

Ces champs comprennent, sans s’y limiter, les éléments suivants :

* Pièces jointes du document
* Champs personnalisés (au niveau du projet ou de la tâche)
* Notes Workfront
* Problèmes
* Un décalage négatif dans les tâches avec une relation de prédécesseur Début/Fin (les tâches sont importées sans retard)
* Affectations
* Contraintes de tâche

  >[!NOTE]
  >
  >Comme les contraintes ne correspondent pas entre le projet Microsoft et Workfront, assurez-vous qu’il existe des relations de prédécesseur entre les tâches. Dans le cas contraire, les dates de début et de fin planifiées des tâches peuvent ne pas être exactes dans le projet importé. 
