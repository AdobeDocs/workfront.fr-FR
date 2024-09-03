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
ht-degree: 100%

---

# Nouveautés de la version 6 de l’API

## Nouveaux objets

### Gestionnaire des ressources

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| ID | customer |   |   |   |   | Ajouter |
| customerID | projet |   |   |   |   | Nombre |
| projectID | resourceManager |   |   |   |   | Supprimer |
| resourceManagerID | modèle |   |   |   |   | Obtenir |
| templateID |   |   |   |   |   | Rapport |
|   |   |   |   |   |   | Rechercher |


### Ews

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| fileName |   |   |   |   | charger |   |
| gérer |   |   |   |   |   |   |
| objCode |   |   |   |   |   |   |


### Libellé personnalisé

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| ID |   |   |   | checkDelete | customLabels | Ajouter |
|   |   |   |   | inUseByOtherLayoutTemplate | userCustomLabels | Nombre |
|   |   |   |   | removeCustomLabel |   | Supprimer |
|   |   |   |   |   |   | Obtenir |
|   |   |   |   |   |   | Rapport |
|   |   |   |   |   |   | Recherche |


## Objets mis à jour

Modifications apportées aux objets existants : les ajouts sont simplement répertoriés, les suppressions sont barrées, les modifications apportées aux objets existants comportent une note jointe après le tableau.

### Mettre à jour

 

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| updateType<sup>1</sup> |   |   |   |   | `sinceDate` |   |
|   |   |   |   |   | objectUpdatesByCommentID<sup>2</sup> |   |

{style="table-layout:auto"}

<sup>1</sup> Modifications des valeurs possibles

<sup>2</sup> L’attribut hasFilters a été remplacé par true.

 

### Approbation

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| completedHours |   | resourceManagers | resourceManagerIDs |   |   |   |
| constraintDate<sup>1</sup> |   |   |   |   |   |   |
| isOriginalPlannedHoursSet |   |   |   |   |   |   |
| syncBurndownDate |   |   |   |   |   |   |
| workRequired<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Validation de date ajoutée

<sup>2</sup> Indicateur NOT_FILTERABLE ajouté

 

### Processus d’approbation

|   | Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|---|
|   |  | `attachedApprovalPaths` |   |   |   |   |   |

{style="table-layout:auto"}

 

### Étape d’approbation

 

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| approvalType<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Modifications apportées aux valeurs possibles

 

### Chemin d’approbation<sup>1</sup>

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| approvedStatus |   |   |   |   |   | Ajouter |
| approvedStatusLabel |   |   |   |   |   | Nombre |
| commentaire |   |   |   |   |   | Supprimer |
| enteredByID |   |   |   |   |   | Modifier |
| entryDate |   |   |   |   |   | Obtenir |
| globalPathID |   |   |   |   |   | Rapport |
| isPrivate |   |   |   |   |   | Recherche |
| lastUpdateDate |   |   |   |   |   |   |
| lastUpdateByID |   |   |   |   |   |   |
| name<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Remplacé par « pouvant faire l’objet d’un rapport »

<sup>2</sup> Ajout d’un programme de validation de longueur maximale

 

### Objet Service de travail

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| constraintDate<sup>1</sup> |   |   |   | getMyWorkCountFiltered |   |   |
| workRequired<sup>2</sup> |   |   |   | workItemStatusLabels  |   |   |

{style="table-layout:auto"}

<sup>1</sup> Validation de date ajoutée

<sup>2</sup> Indicateur Not_Filterable ajouté

 

### Affectation

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
|   |   |   |   | assignUserToRoleOnProjects |   |   |
|   |   |   |   | swapUsersOnProjects |   |   |
|   |   |   |   | unassignUserFromProjects |   |   |

{style="table-layout:auto"}

 

### Référence 

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| workRequired<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Indicateur Not_Filterable ajouté

 

### Tâche de ligne de base

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| workRequired<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Indicateur Not_Filterable ajouté

 

### Enregistrement de facturation

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| billingDate<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Indicateur de champ NO_TIME ajouté

### Événement d’avancement

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
| `checkedOutByID` | `checkedOutBy`  |   | isDir |   |   |   |
| `isDir`  |   |   |   |   |   |   |

{style="table-layout:auto"}

 

Taux de change

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| rate<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Changement du programme de validation PRECISION de 8 à 9

 

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

<sup>1</sup> Modifications apportées aux valeurs possibles

 

### Optask (problème)<sup>1</sup> 

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| workRequired<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Marqué comme RESTORABLE

<sup>2</sup> Indicateur Not_Filterable ajouté

 

### Projet<sup>1</sup> 

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| completedHours |   | `openOpTasks` |  openOpTasks |   |   |   |
| isOriginalPlannedHoursSet |   | resourceManagers | resourceManagerIDs  |   |   |   |
| originalWorkRequired |   |   | `work` |   |   |   |
| syncBurndownDate |   |   |   |   |   |   |
| work |   |   |   |   |   |   |
| workRequired |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Marqué comme RESTORABLE et RESOURCE_MANAGEABLE

<sup>2</sup> Indicateur Not_Filterable ajouté

 

### Tâche<sup>1</sup>

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| constraintDate<sup>2</sup> |   |   |   |   |   |   |
| workRequired<sup>3</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Marqué comme RESTORABLE

<sup>2</sup> Ajout du programme de validation AT_DATE_YEAR_BEFORE

<sup>3</sup> Indicateur Not_Filterable ajouté

 

### Equipe

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| `myWorkViewID` |  `myWorkView` |   |   |   |   |   |
| `requestsViewID`  | `myRequestsView`  |   |   |   |   |   |

{style="table-layout:auto"}

 

### Modèle<sup>1</sup> 

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
|   |   | resourceManagers | resourceManagerIDs |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Marqué comme RESTORABLE et RESOURCE_MANAGEABLE

### Tâche de modèle<sup>1</sup> 

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| workRequired<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Marqué comme RESTORABLE

<sup>2</sup> Indicateur Not_Filterable ajouté

 

### l’utilisateur ou de l’utilisatrice

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| myInfo<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Violateurs MAX_LENGTH

 

### Note de l’utilisateur ou utilisatrice

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| eventType<sup>1</sup> |   |   |   |   | myNotifications<sup>2</sup> |   |

{style="table-layout:auto"}

<sup>1</sup> Valeurs possibles modifiées

<sup>2</sup> contient des filtres modifiés en `[true]`

 

### Annonce

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
|   |   |   |   | `fileHandle` |   |   |
|   |   |   |   | `zipAnnouncementAttachments`  |   |   |
