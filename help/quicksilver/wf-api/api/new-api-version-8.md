---
content-type: api
navigation-topic: api-navigation-topic
title: Nouveautés de l’API version 8
description: Il s’agit d’une liste des ressources nouvelles de l’API version 9. Pour obtenir la liste des mises à jour apportées aux ressources de la version 8, consultez Mises à jour de l’API version 8.
author: Becky
feature: Workfront API
role: Developer
exl-id: 90fefaa6-d387-4cdb-8aea-9a939fe2ac26
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 100%

---

# Nouveautés de l’API version 8

## Nouvelles ressources

Il s’agit d’une liste des ressources nouvelles de l’API version 9. Pour obtenir la liste des mises à jour apportées aux ressources de la version 8, consultez la page [Mises à jour de l’API version 8](../../wf-api/api/new-api-version-8-updates.md)

**AgileWork**

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| backlogOrder | customer |   |   | bulkCopy |   | COPY |
| color | iteration |   |   |   |   | COUNT |
| customerID | lastUpdatedBy |   |   |   |   | SUPPRIMER |
| estimate | opTask |   |   |   |   | MODIFIER |
| ID | projet |   |   |   |   | GET |
| isReady | storyboardParent |   |   |   |   | REPORT |
| iterationID | tâche |   |   |   |   | SEARCH |
| lastUpdateDate | équipe |   |   |   |   |   |
| lastUpdatedByID |   |   |   |   |   |   |
| name |   |   |   |   |   |   |
| opTaskID |   |   |   |   |   |   |
| parentStoryBoardOrder |   |   |   |   |   |   |
| projectID |   |   |   |   |   |   |
| storyBoardOrder |   |   |   |   |   |   |
| storyBoardParentID |   |   |   |   |   |   |
| taskID |   |   |   |   |   |   |
| teamID |   |   |   |   |   |   |
| type |   |   |   |   |   |   |
| uiObjCode |   |   |   |   |   |   |
| uiObjectID |   |   |   |   |   |   |

{style="table-layout:auto"}

### APIVersionMetadata

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| deprecationRelease |   |   |   |   |   | COUNT |
| removalRelease |   |   |   |   |   | GET |
| versionName |   |   |   |   |   | REPORT |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

**KanbanBoard**

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | ADD |
| name |   |   |   |   |   | COUNT |
|   |   |   |   |   |   | SUPPRIMER |
|   |   |   |   |   |   | EDIT |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | REPORT |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

### ProofApprovalStatus

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   |   |
| proofApprovalStatusID |   |   |   |   |   |   |
| proofApprovalStatusLabel |   |   |   |   |   |   |

{style="table-layout:auto"}

**ProofFileMetadata**

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| documentVersionID | documentVersion |   |   |   |   |   |
| fileIndex |   |   |   |   |   |   |
| fileName |   |   |   |   |   |   |
| ID |   |   |   |   |   |   |
| isURL |   |   |   |   |   |   |

{style="table-layout:auto"}

**ResourceBudgetedHour**

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| allocationDate |   |   |   |   |   | ADD |
| budgetedHours |   |   |   |   |   | COUNT |
| plannedBudgetedHours |   |   |   |   |   | SUPPRIMER |
| projectID |   |   |   |   |   | EDIT |
| roleID |   |   |   |   |   | GET |
| userID |   |   |   |   |   | REPORT |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

### ResourcePlannerFilter

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | ADD |
| name |   |   |   |   |   | COUNT |
|   |   |   |   |   |   | SUPPRIMER |
|   |   |   |   |   |   | EDIT |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | REPORT |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

**RichTextNote**

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | COUNT |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | REPORT |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

### S&#39;abonner

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| ID |   |   |   | addSubscribers | subscribers | ADD |
|   |   |   |   | removeSubscribers |   | COUNT |
|   |   |   |   | subscribes |   | SUPPRIMER |
|   |   |   |   | unsubscribes |   | GET |
|   |   |   |   |   |   | REPORT |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

### UserRole

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| roleID | Rôle |   |   |   |   |   |
| timePercentage | utilisateur |   |   |   |   |   |
| userID |   |   |   |   |   |   |
