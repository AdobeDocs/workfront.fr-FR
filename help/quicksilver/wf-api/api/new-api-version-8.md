---
content-type: api
navigation-topic: api-navigation-topic
title: Nouveautés de l’API version 8
description: Il s’agit d’une liste des ressources nouvelles de l’API version 9. Pour obtenir la liste des mises à jour apportées aux ressources de la version 8, consultez Mises à jour de l’API version 8 .
author: Becky
feature: Workfront API
exl-id: 90fefaa6-d387-4cdb-8aea-9a939fe2ac26
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 32%

---

# Nouveautés de l’API version 8

## Nouvelles ressources

Il s’agit d’une liste des ressources nouvelles de l’API version 9. Pour obtenir la liste des mises à jour apportées aux ressources de la version 8, consultez la page [Mises à jour de l’API version 8](../../wf-api/api/new-api-version-8-updates.md)

**AgileWork**

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| backlogOrder | client |   |   | bulkCopy  |   | COPY |
| color | itération  |   |   |   |   | COUNT |
| customerID | lastUpdatedBy |   |   |   |   | SUPPRIMER |
| estimation | opTask |   |   |   |   | MODIFIER |
| ID | projet |   |   |   |   | GET  |
| isReady | storyboardParent |   |   |   |   | RAPPORT |
| iterationID | tâche |   |   |   |   | SEARCH |
| lastUpdateDate | équipe |   |   |   |   |   |
| lastUpdatedByID |   |   |   |   |   |   |
| name |   |   |   |   |   |   |
| opTaskID |   |   |   |   |   |   |
| parentStoryBoardOrder |   |   |   |   |   |   |
| projectID |   |   |   |   |   |   |
| storyBoardOrder |   |   |   |   |   |   |
| storyBoardParentID |   |   |   |   |   |   |
| taskID  |   |   |   |   |   |   |
| TeamID |   |   |   |   |   |   |
| type |   |   |   |   |   |   |
| uiObjCode |   |   |   |   |   |   |
| uiObjectID |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### APIVersionMetadata

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| deprecationRelease |   |   |   |   |   | COUNT  |
| removeRelease |   |   |   |   |   | GET |
| versionName |   |   |   |   |   | RAPPORT |
|   |   |   |   |   |   | SEARCH |

{style=&quot;table-layout:auto&quot;}

**KanbanBoard**

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | AJOUTER |
| name |   |   |   |   |   | COUNT |
|   |   |   |   |   |   | SUPPRIMER |
|   |   |   |   |   |   | MODIFIER |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | RAPPORT |
|   |   |   |   |   |   | SEARCH |

{style=&quot;table-layout:auto&quot;}

### ProofApprovalStatus

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   |   |
| proofApprovalStatusID |   |   |   |   |   |   |
| proofApprovalStatusLabel |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

**ProofFileMetadata**

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| documentVersionID | documentVersion |   |   |   |   |   |
| fileIndex |   |   |   |   |   |   |
| fileName |   |   |   |   |   |   |
| ID |   |   |   |   |   |   |
| isURL |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

**ResourceBudgetedHour**

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| allocationDate |   |   |   |   |   | AJOUTER |
| recordsHours |   |   |   |   |   | COUNT |
| scheduledBudgetedHours |   |   |   |   |   | SUPPRIMER |
| projectID |   |   |   |   |   | MODIFIER |
| roleID |   |   |   |   |   | GET |
| userID |   |   |   |   |   | RAPPORT |
|   |   |   |   |   |   | SEARCH |

{style=&quot;table-layout:auto&quot;}

### ResourcePlannerFilter

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | AJOUTER |
| name |   |   |   |   |   | COUNT |
|   |   |   |   |   |   | SUPPRIMER |
|   |   |   |   |   |   | MODIFIER |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | RAPPORT |
|   |   |   |   |   |   | SEARCH |

{style=&quot;table-layout:auto&quot;}

**RichTextNote**

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | COUNT |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | RAPPORT |
|   |   |   |   |   |   | SEARCH |

{style=&quot;table-layout:auto&quot;}

### S&#39;abonner

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
|  ID |   |   |   | addSubscribers | subscribers | AJOUTER |
|   |   |   |   | removeSubscribers |   | COUNT  |
|   |   |   |   | subscribes |   | SUPPRIMER |
|   |   |   |   | se désabonne |   | GET |
|   |   |   |   |   |   | RAPPORT |
|   |   |   |   |   |   | SEARCH |

{style=&quot;table-layout:auto&quot;}

### UserRole

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| roleID | rôle |   |   |   |   |   |
| timePercentage | user |   |   |   |   |   |
| userID |   |   |   |   |   |   |
