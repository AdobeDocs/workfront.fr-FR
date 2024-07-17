---
content-type: api
navigation-topic: api-navigation-topic
title: Nouveautés de la version 6 de l’API
description: Nouveautés de la version 6 de l’API
author: Becky
feature: Workfront API
role: Developer
exl-id: e671a881-b8c2-4234-a3a0-76b1fbfafd32
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '538'
ht-degree: 37%

---

# Nouveautés de la version 6 de l’API

## Nouveaux objets

### Gestionnaire des ressources

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| ID | client |   |   |   |   | Ajouter |
| customerID | projet |   |   |   |   | Nombre |
| projectID | resourceManager |   |   |   |   | Supprimer |
| resourceManagerID | modèle |   |   |   |   | Get |
| templateID |   |   |   |   |   | Rapport  |
|   |   |   |   |   |   | Rechercher  |


### Nouvelles

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| fileName |   |   |   |   | charger |   |
| handle |   |   |   |   |   |   |
| objCode |   |   |   |   |   |   |


### Libellé personnalisé

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| ID |   |   |   | checkDelete | customLabels | Ajouter |
|   |   |   |   | inUseByOtherLayoutTemplate | userCustomLabels | Nombre |
|   |   |   |   | removeCustomLabel |   | Supprimer |
|   |   |   |   |   |   | Get |
|   |   |   |   |   |   | Rapport |
|   |   |   |   |   |   | Recherche |


## Objets mis à jour

Modifications apportées aux objets existants : les ajouts sont simplement répertoriés, les suppressions ont été réalisées, les modifications apportées aux objets existants comportent une note jointe après le tableau.

### Mettre à jour

 

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| updateType<sup>1</sup> |   |   |   |   | `sinceDate` |   |
|   |   |   |   |   | objectUpdatesByCommentID<sup>2</sup> |   |

{style="table-layout:auto"}

<sup>1</sup> Modifications apportées aux valeurs possibles

L&#39;attribut <sup>2</sup> hasFilters a été remplacé par true

 

### Approbation

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| completedHours |   | resourceSuperviseurs | resourceManagerIDs |   |   |   |
| constraintDate<sup>1</sup> |   |   |   |   |   |   |
| isOriginalPlannedHoursSet |   |   |   |   |   |   |
| syncBurndownDate |   |   |   |   |   |   |
| workRequired<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Date de validation ajoutée

<sup>2</sup> L’indicateur NOT_FILTERABLE a été ajouté

 

### Processus d&#39;approbation

|   | Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|---|
|   |  | `attachedApprovalPaths` |   |   |   |   |   |

{style="table-layout:auto"}

 

### Étape de validation

 

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| approvalType<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Modifications apportées aux valeurs possibles

 

### Chemin d’approbation<sup>1</sup>

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| approvedStatus |   |   |   |   |   | Ajouter |
| approvedStatusLabel |   |   |   |   |   | Nombre |
| comment |   |   |   |   |   | Supprimer |
| entryByID |   |   |   |   |   | Modifier |
| entryDate |   |   |   |   |   | Get |
| globalPathID |   |   |   |   |   | Rapport |
| isPrivate |   |   |   |   |   | Recherche |
| lastUpdateDate |   |   |   |   |   |   |
| lastUpdateByID |   |   |   |   |   |   |
| name<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Remplacé

<sup>2</sup> Ajout de la validation de longueur maximale

 

### Objet Work Service

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| constraintDate<sup>1</sup> |   |   |   | getMyWorkCountFiltered |   |   |
| workRequired<sup>2</sup> |   |   |   | workItemStatusLabels  |   |   |

{style="table-layout:auto"}

<sup>1</sup> Date de validation ajoutée

<sup>2</sup> Ajout de l’indicateur non filtrable

 

### Affectation

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
|   |   |   |   | assignUserToRoleOnProjects |   |   |
|   |   |   |   | swapUsersOnProjects |   |   |
|   |   |   |   | unassignUserFromProjects |   |   |

{style="table-layout:auto"}

 

### Ligne de base 

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| workRequired<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Ajout de l’indicateur non filtrable

 

### Tâche de ligne de base

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| workRequired<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Ajout de l’indicateur non filtrable

 

### Enregistrement de facturation

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| billingDate<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> ajout de l’indicateur de champ NO_TIME

### Événement de Burndown 

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| eventInitiator |   |   |   |   |   | `ADD` |
|   |   |   |   |   |   | `DELETE` |

{style="table-layout:auto"}

 

### Catégorie 

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
|   |   |   |   | getCascadingRules |   |   |
|   |   |   |   | reorderCategories |   |   |

{style="table-layout:auto"}

 

Énumération personnalisée 

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
|   |   |   |   | getGroupDefaultProjectStatus | opTaskGroupStatuses |   |
|   |   |   |   | isPossibleToUnlockStatus | projectGroupStatuses |   |
|   |   |   |   |   | taskGroupStatuses |   |

{style="table-layout:auto"}

 

Document 

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| `checkedOutByID` | `checkedOutBy`  |   |  isDir |   |   |   |
| `isDir`  |   |   |   |   |   |   |

{style="table-layout:auto"}

 

Taux d’Exchange 

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| rate<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Modification du programme de validation PRECISION pour 8 à 9

 

### Intégration

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| syncBurndownDate |   |   |   |   |   |   |

{style="table-layout:auto"}

 

### Entrée au journal

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| changeType<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Modifications apportées aux valeurs possibles

 

### Optask (problème)<sup>1</sup> 

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| workRequired<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> marqué comme RESTORABLE

<sup>2</sup> Ajout de l’indicateur non filtrable

 

### Projet<sup>1</sup> 

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| completedHours |   | `openOpTasks` |  openOpTasks |   |   |   |
| isOriginalPlannedHoursSet |   | resourceSuperviseurs | resourceManagerIDs  |   |   |   |
| originalWorkRequired |   |   | `work` |   |   |   |
| syncBurndownDate |   |   |   |   |   |   |
| work |   |   |   |   |   |   |
| workRequired |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> marqué comme RESTORABLE et RESOURCE_MANAGEABLE

<sup>2</sup> Ajout de l’indicateur non filtrable

 

### Tâche<sup>1</sup>

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| constraintDate<sup>2</sup> |   |   |   |   |   |   |
| workRequired<sup>3</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> marqué comme RESTORABLE

<sup>2</sup> Ajout du programme de validation AT_DATE_YEAR_BEFORE

<sup>3</sup> Ajout de l’indicateur non filtrable

 

### Equipe

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| `myWorkViewID` |  `myWorkView` |   |   |   |   |   |
| `requestsViewID`  | `myRequestsView`  |   |   |   |   |   |

{style="table-layout:auto"}

 

### Template<sup>1</sup> 

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
|   |   | resourceSuperviseurs | resourceManagerIDs |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> marqué comme RESTORABLE et RESOURCE_MANAGEABLE

### Tâche de modèle<sup>1</sup> 

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| workRequired<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> marqué comme RESTORABLE

<sup>2</sup> Ajout de l’indicateur non filtrable

 

### l’utilisateur ou de l’utilisatrice

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| myInfo<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Violateurs MAX_LENGTH

 

### Note de l’utilisateur

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| eventType<sup>1</sup> |   |   |   |   | myNotifications<sup>2</sup> |   |

{style="table-layout:auto"}

<sup>1</sup> Valeurs possibles modifiées

<sup>2</sup> avec des filtres modifiés en `[true]`

 

### Annonce

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
|   |   |   |   | `fileHandle` |   |   |
|   |   |   |   | `zipAnnouncementAttachments`  |   |   |
