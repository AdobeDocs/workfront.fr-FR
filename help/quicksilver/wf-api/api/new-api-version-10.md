---
content-type: api
navigation-topic: api-navigation-topic
title: Nouveautés de la version 10 de l’API
description: Ressources mises à jour
author: Becky
feature: Workfront API
role: Developer
exl-id: 8ac384ae-5d65-4c0e-98c1-cf38cfbff460
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 42%

---

# Nouveautés de la version 10 de l’API

* [Nouvelles ressources](#new-resources)
* [Ressources mises à jour](#updated-resources)
* [Ressources supprimées](#removed-resources)

## Nouvelles ressources {#new-resources}

### ActivityLog

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
|   |   |   |   |   |   | AJOUTER |
|   |   |   |   |   |   | COUNT |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

### CalendarEntry

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | AJOUTER |
|   |   |   |   |   |   | COUNT  |
|   |   |   |   |   |   | DELETE  |
|   |   |   |   |   |   | MODIFIER  |
|   |   |   |   |   |   | GET  |
|   |   |   |   |   |   | RAPPORT  |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

### CalendarEntryExternalReference

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | COUNT |
|   |   |   |   |   |   | GET  |
|   |   |   |   |   |   | RAPPORT  |
|   |   |   |   |   |   | RECHERCHE  |

{style="table-layout:auto"}

### ExternalAuthToken

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | AJOUTER |
|   |   |   |   |   |   | COUNT |
|   |   |   |   |   |   | DELETE  |
|   |   |   |   |   |   | MODIFIER  |
|   |   |   |   |   |   | GET  |
|   |   |   |   |   |   | RAPPORT  |
|   |   |   |   |   |   | RECHERCHE  |

{style="table-layout:auto"}

### LicenseTypeGroupLimit

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| customerID | client |   |   |   |   |   |
| groupID | groupe |   |   |   |   |   |
| planLimit |   |   |   |   |   |   |
| usedLicences |   |   |   |   |   |   |
| worklimit |   |   |   |   |   |   |
|   |   |   |   |   |   |   |
|   |   |   |   |   |   |   |

{style="table-layout:auto"}

### UserHomeCalendarPreference

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| customerID | client |   |   |   |   | AJOUTER |
| edTime | utilisateur |   |   |   |   | COUNT |
| firstDayOfWeek |   |   |   |   |   | SUPPRIMER |
| ID |   |   |   |   |   | MODIFIER |
| showPTO |   |   |   |   |   | GET |
| startTime |   |   |   |   |   | RAPPORT |
| userID |   |   |   |   |   | SEARCH |
| workDate |   |   |   |   |   |   |

{style="table-layout:auto"}

**Ressources mises à jour**

Les ressources existantes suivantes ont été mises à jour avec cette version de l’API Workfront. Les modifications apportées à une ressource sont indiquées comme suit :

* Les ajouts sont simplement répertoriés
* Les suppressions sont indiquées par un texte barré.
* Les modifications sont répertoriées dans la note après le tableau.

### Approbation

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| kanbanFlag |  |  | pendingApproval `<sup>1</sup>`   |   |   |   |
| `masterTaskID` |   |   |   |   |   |   |
| priorityColor  |   |   |   |   |   |   |
| projectBudgetedCost  |   |   |   |   |   |   |
| projectNetValue  |   |   |   |   |   |   |
| projectRoi  |   |   |   |   |   |   |
| resourcePlannerBudgetedLaborCost  |   |   |   |   |   |   |

{style="table-layout:auto"}

`<sup>1</sup> Type changed from null to boolean`

### Affectation

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| assignmentPercent `<sup>1</sup>` |   |   |   |   |   |   |
| viewedByAssignedToUser |   |   |   |   |   |   |

{style="table-layout:auto"}

`<sup>1</sup>` validateur ajouté LESS_THAN_EQUAL

### BudgetedHour

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   |   |

{style="table-layout:auto"}

 

### CustomerPreferences

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| name `<sup>1</sup>` |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Modifications apportées aux valeurs possibles

### DocMetadataLinkGroup

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
|   |   |   |   | getMetadataForDocument |   |   |

{style="table-layout:auto"}

### Document

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| `masterTaskID` |  |   |   |   |   |   |

{style="table-layout:auto"}

### DocumentRequest

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| `masterTaskID` |   |   |   |   |   |   |

{style="table-layout:auto"}

DocumentVersion

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| externalIntegrationType <sup>1</sup> |   |   |   |   |   |   |
|   |   |   |   |   |   |   |
|   |   |   |   |   |   |   |
|   |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Modifications apportées aux valeurs possibles

Frais

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| `masterTaskID` |   |   |   |   |   |   |

{style="table-layout:auto"}

### Groupe

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
|   | licenseTypeLimit |   |   | addRemoveLicenseTypeLimits  |   |   |
|   |   |   |   | setLicenseTypeLimit |   |   |

{style="table-layout:auto"}

### LinkedFolder

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| externalIntegrationType<sup>1</sup> |  |  |  |  |   |   |

{style="table-layout:auto"}

<sup>1</sup> Modifications apportées aux valeurs possibles

### TâcheOp

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| priorityColor |   |  | pendingApproval<sup>1</sup> |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Le type est passé de null à boolean

### PortalSection

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
|   |  |   | groupIDs |   |   |   |

{style="table-layout:auto"}

### Portfolio

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| portfolioNetValue |   |   |   |  |  |   |
| portfolioRoi |   |   |   |   |   |   |

{style="table-layout:auto"}

### Projet

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| projectBudgetedCost  |   |   |   | linkExternalObject  |   |   |
| projectNetValue |   |   |   | unlinkExternalObject |   |   |
| projectRoi |   |   |   |   |   |   |
| resourcePlannerBudgetedLaborCost |   |   |   |   |   |   |

{style="table-layout:auto"}

### ProofApproval

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| approverDecision |   |   |   |   |   |   |

{style="table-layout:auto"}

### Taux

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| rateValue <sup>1</sup> |  |  |  |  |  |   |

{style="table-layout:auto"}

<sup>1</sup>MONNAIE DU validateur ajoutée

### Tâche

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| kanbanFlag |   |   |   |   |   |   |
| `masterTaskID` |   |   |   |   |   |   |
| priorityColor  |   |   |   |   |   |   |

{style="table-layout:auto"}

 

### Equipe

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| hoursPerPoint <sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> validateur ajouté LESS_THAN

### TeamAssignment

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| `masterTaskID` |   |   |   |   |   |   |

{style="table-layout:auto"}

### TeamTask

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| `masterTaskID` |   |   |   |   |   |   |

{style="table-layout:auto"}

### Feuille de temps

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
|   |   |   |   |   |   |   |

{style="table-layout:auto"}

### Mettre à jour

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| updateType `<sup>1</sup>` |   |   |   |   |   | objectUpdatesWithNoteAndJournalEntryIndex  |

{style="table-layout:auto"}

<sup>1</sup> change les valeurs possibles

### l’utilisateur ou de l’utilisatrice

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
|   | accessLevel  |   |   |   |   |   |

{style="table-layout:auto"}

### UserNote

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| eventType <sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> change les valeurs possibles

### Travail

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| kanbanFlag |  |  | pendingApproval <sup>1</sup>  |   |   |   |
| `masterTaskID` |   |   |   |   |   |   |
| priorityColor  |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Le type est passé de null à boolean

## Ressources supprimées {#removed-resources}

### ResourceBudgetedHour

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| allocationDate |   |   |   |   |   | AJOUTER  |
| recordsHours |   |   |   |   |   | COUNT  |
| ID |   |   |   |   |   | DELETE  |
| scheduledBudgetedHours |   |   |   |   |   | MODIFIER  |
| projectID |   |   |   |   |   | GET  |
| roleID |   |   |   |   |   | RAPPORT  |
| userID |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

 

 

 
