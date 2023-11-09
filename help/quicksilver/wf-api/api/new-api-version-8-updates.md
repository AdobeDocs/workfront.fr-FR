---
content-type: api
navigation-topic: api-navigation-topic
title: Mises à jour de l’API version 8
description: Affichez les mises à jour de l’API version 8.
author: Becky
feature: Workfront API
role: Developer
exl-id: c6d7d2d2-cd21-4ca8-a5a0-afe3669dc959
source-git-commit: ae80999fc7ea7e35097560aa99baa435bcd31b74
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 28%

---

# Mises à jour de l’API version 8

## Ressources mises à jour

Les ressources existantes suivantes ont été mises à jour avec cette version de l’API Adobe Workfront. Pour afficher les ressources qui sont nouvelles de la version 8, voir [Nouveautés de l’API version 8](../../wf-api/api/new-api-version-8.md). Les modifications apportées à une ressource sont indiquées de la manière suivante :

* Les ajouts sont simplement répertoriés
* Les suppressions sont indiquées par un texte barré.
* Les modifications sont signalées dans la note suivant le tableau .

### AccessRequest

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| action<sup>1</sup>  |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Modifications des valeurs possibles

### AccessRule<sup>1</sup> 

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| coreAction<sup>2</sup>  |   |   |   |   |   |   |
| forbiddenActions<sup>2</sup> |   |   |   |   |   |   |
| secondaryActions<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Indicateur supprimé : REPORTABLE\
<sup>2</sup> Modifications des valeurs possibles

### Approbation

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> | agileWork  | resourcePools |   |   |   |   |
| backlogOrder<sup>2</sup> | kanbanBoard  |   |   |   |   |   |
| backlogParent |   |   |   |   |   |   |
| kanbanBoardID |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>Modifications des valeurs possibles\
<sup>2</sup>Ajout d’indicateurs : DYNAMIC, LAZY_READ et NOT_GROUPABLE

### Affectation

|   |   |   |   | Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|---|---|---|---|
|   |   |   |   | assignUserToRoleOnTasks | getAssignAssignmentsForTasks  |   |   |   |   |   |
|   |   |   |   | swapUsersOnTasks | getUnassignAssignmentsForTasks |   |   |   |   |   |
|   |   |   |   | unassignUserFromTasks |   |   |   |   |   |   |

{style="table-layout:auto"}

### Client

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| bizRuleExclusions<sup>1</sup> |   |   |   | getPackagingOptionValue |   |   |
| proofPlan<sup>1</sup> |   |   |   | isPackagingOptionEnabled |   |   |

{style="table-layout:auto"}

<sup>1</sup>Modifications des valeurs possibles

### CustomerPreferences

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| name<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>Modifications des valeurs possibles

### DocumentApproval

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| ID<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>Indicateur ajouté : NOT_FILTERABLE

### DocumentVersion

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| activeProofStages |   |   |   |   |   |   |

{style="table-layout:auto"}

### Groupe

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
|   |   | propriétaires |   |   |   |   |

{style="table-layout:auto"}

### HourType

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| appGlobalID<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>Indicateur ajouté : NOT_FILTERABLE

### Itération

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
|   |   |   |   | moveStories |   |   |

{style="table-layout:auto"}

### J&#39;aime

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| `endorsementID` | `endorsement` |   |   |   |   |   |

{style="table-layout:auto"}

### Note

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| auditType<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>Modifications des valeurs possibles

### TâcheOp

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> | agileWork  |   |   |   | defaultShownTimesheetIssues  |   |
| backlogOrder | itération |   |   |   |   |   |
| backlogParent |   |   |   |   |   |   |
| estimation |   |   |   |   |   |   |
| iterationID |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>Modifications des valeurs possibles

### Portfolio

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>Modifications des valeurs possibles

### Programme

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>Modifications des valeurs possibles

### Projet

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> |   | resourcePools |   |   | defaultShownTimesheetProjects |   |

{style="table-layout:auto"}

<sup>1</sup>Modifications des valeurs possibles

### ProofApproval

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| approverID | approbateur |   |   |   |   |   |
| documentVersionID | documentVersion |   |   |   |   |   |
| ID<sup>1</sup> |   |   |   |   |   |   |
| proofCreationDate |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>Indicateur ajouté : NOT_FILTERABLE

### QueueDef

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| requestorCoreAction<sup>1</sup> |   |   |   |   |   |   |
| requestorForbiddenActions<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>Modifications des valeurs possibles

### Taux

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| endDate |   |   |   | setRatesForRole  |   |   |
| name |   |   |   |   |   |   |
| startDate |   |   |   |   |   |   |

{style="table-layout:auto"}

### RéservéTime

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| extRefID |   |   |   |   |   |   |

{style="table-layout:auto"}

### ResourceManager

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| projectPriority |   |   |   |   |   |   |

{style="table-layout:auto"}

### Tâche

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> | agileWork  |   |   |   | allTasksOnIterations  |   |
| backlogParent | kanbanBoard |   |   |   | defaultShownTimesheetTasks |   |
| kanbanBoardID |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>Modifications des valeurs possibles

### Équipe

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| agileMéthodology |   |   |   |   |   |   |
| autoAddNextStory |   |   |   |   |   |   |
| includeIssues |   |   |   |   |   |   |
| TeamStoryBoardIssueStatuses |   |   |   |   |   |   |
| wipLimit |   |   |   |   |   |   |

{style="table-layout:auto"}

### Modèle

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
|   |   | resourcePools |   |   |   |   |

{style="table-layout:auto"}

### TemplateTask

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>Modifications des valeurs possibles

Mettre à jour

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| updateType<sup>1</sup> | `updateEndorsement` |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>Modifications des valeurs possibles

### l’utilisateur ou de l’utilisatrice

|   |   | Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|---|---|
|   |   | resourcePools |   |   |   |   |   |   |
|   |   | userGroups |   |   |   |   |   |   |
|   |   | userRoles |   |   |   |   |   |   |

{style="table-layout:auto"}

### UserNote

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| `endorsementID` | `endorsement` |   |   |   |   |   |
| `endorsementShareID` | `endorsementShare` |   |   |   |   |   |
| eventType<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>Modifications des valeurs possibles

### Travail

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> | agileWork  |   |   |   |   |   |
| backlogOrder<sup>2</sup> | kanbanBoard  |   |   |   |   |   |
| backlogParent  |   |   |   |   |   |   |
| kanbanBoardID |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>Modifications des valeurs possibles\
<sup>2</sup>Ajout d’indicateurs : DYNAMIC, LAZY_READ et NOT_GROUPABLE
