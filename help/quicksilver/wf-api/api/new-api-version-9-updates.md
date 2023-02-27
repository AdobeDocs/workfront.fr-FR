---
content-type: api
navigation-topic: api-navigation-topic
title: Mises à jour de l’API version 9
description: Ressources mises à jour
author: Becky
feature: Workfront API
exl-id: 51892846-d93f-4363-8416-4118fb2ef84d
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 47%

---

# Mises à jour de l’API version 9

## Ressources mises à jour

Les ressources existantes suivantes ont été mises à jour avec cette version de l’API Adobe Workfront. Pour afficher les ressources nouvelles de la version 9, vous pouvez accéder à [Nouveautés de l’API version 9](../../wf-api/api/new-api-version-9.md) et [Nouveautés de l’API version 9 (suite)](../../wf-api/api/new-api-version-9-continue.md). Les modifications apportées à une ressource sont indiquées de la manière suivante :

* Les ajouts sont simplement répertoriés
* Les suppressions sont indiquées par un texte barré.
* Les modifications sont signalées dans la note suivant le tableau

### AgileWork

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| `opTaskID`<sup>2</sup> |  |  |  |  |  |  |
| `taskID`<sup>2</sup> |  |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

¹ Indicateur supprimé : REPORTABLE\
² Indicateur supprimé : NOT_GROUPABLE

### Approbation

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| `storyBoardOrder` | `agileWork` |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

Affectation

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
|  |  |  |  | `assignUserToRoleOnProjects`<sup>1</sup> |  |  |
|  |  |  |  | `assignUserToRoleOnTasks`<sup>1</sup> |  |  |
|  |  |  |  | `swapUsersOnProjects`<sup>1</sup> |  |  |
|  |  |  |  | `swapUsersOnTasks`<sup>1</sup> |  |  |

{style=&quot;table-layout:auto&quot;}

¹ Champ ajouté : lockToRole

### CustomerPreferences

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| `name`<sup>1</sup> |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Modifications apportées aux valeurs possibles

### Heure

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| `days` |  |  |  |  |  |  |
| `workHoursPerDay` |  |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

### Itération

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
|  |  |  |  | `moveIssues` |  |  |

{style=&quot;table-layout:auto&quot;}

### LayoutTemplates

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| `groupID` | `group` |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

### Note

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| `html` |  |  |  |  |  |  |
| `json` |  |  |  |  |  |  |
| `richTextNoteID` |  |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

### TâcheOp

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| `color` | `agileWork` |  |  | `convertToProject` |  |  |
| `isReady` |  |  |  | `convertToTask` |  |  |
| `storyBoardOrder` |  |  |  | `linkExternalObject` |  |  |
|  |  |  |  | `unlinkExternalObject` |  |  |

{style=&quot;table-layout:auto&quot;}

### ResourceBudget

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| `ID` |  |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

¹ Indicateur supprimé : REPORTABLE

### Planification

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| `homeGroupID` | `homeGroup` |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

### Tâche

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
|  | `agileWork` |  |  | `convertToProject` |  |  |
|  |  |  |  | `linkExternalObject` |  |  |
|  |  |  |  | `unlinkExternalObject` |  |  |

{style=&quot;table-layout:auto&quot;}

### Équipe

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| `includeIssues` |  |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

### TimesheetProfile

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| `groupID` | `group` |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

### UIFilter

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
|  |  |  |  |  | `filtersForObjCode` |  |

{style=&quot;table-layout:auto&quot;}

### UIView

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
|  |  |  |  |  | `viewsForObjCode` |  |

{style=&quot;table-layout:auto&quot;}

### Utilisateur

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| `logTimeInDays` |  |  |  |  |  |  |
| `workHoursPerDay` |  |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

### Travail

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| `storyBoardOrder` | `agileWork` |  |  | `getWFHomeObjects` |  |  |
