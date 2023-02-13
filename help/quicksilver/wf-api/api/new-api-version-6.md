---
content-type: api
navigation-topic: api-navigation-topic
title: Nouveautés de l’API version 6
description: Nouveautés de l’API version 6
author: John
feature: Workfront API
exl-id: e671a881-b8c2-4234-a3a0-76b1fbfafd32
source-git-commit: 2ec05c03a5bfa842008870ca47fb617b81fd6ebd
workflow-type: tm+mt
source-wordcount: '570'
ht-degree: 41%

---

# Nouveautés de l’API version 6

## Nouveaux objets

### Gestionnaire des ressources

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| ID | client |   |   |   |   | Ajouter |
| customerID | projet |   |   |   |   | Nombre |
| projectID | resourceManager |   |   |   |   | Supprimer |
| resourceManagerID | modèle |   |   |   |   | Get |
| templateID |   |   |   |   |   | Rapport  |
|   |   |   |   |   |   | Recherche  |


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

Modifications apportées aux objets existants : les ajouts sont simplement répertoriés, les suppressions ont été réactivées, les modifications apportées aux éléments existants comportent une note jointe après le tableau.

### Mettre à jour

 

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| updateType¹ |   |   |   |   | `sinceDate` |   |
|   |   |   |   |   | objectUpdatesByCommentID² |   |

{style=&quot;table-layout:auto&quot;}

¹ Modifications apportées aux valeurs possibles

² attribut hasFilters a été remplacé par true

 

### Approbation

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| completedHours |   | resourceGuidelines | resourceManagerIDs |   |   |   |
| constraintDate¹ |   |   |   |   |   |   |
| isOriginalScheduleHoursSet |   |   |   |   |   |   |
| syncBurndownDate |   |   |   |   |   |   |
| workRequired² |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Validation de date ajoutée

² Indicateur NOT_FILTERABLE ajouté

 

### Processus d&#39;approbation

|   | Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|---|
|  |  | `attachedApprovalPaths` |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

### Étape de validation

 

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| approvalType¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Modifications apportées aux valeurs possibles

 

### Chemin d’approbation¹

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
| name² |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Remplacé en rapport

² Ajout de la validation de longueur maximale

 

### Objet Work Service

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| constraintDate¹ |   |   |   | getMyWorkCountFiltered |   |   |
| workRequired² |   |   |   | workItemStatusLabels  |   |   |

{style=&quot;table-layout:auto&quot;}

Ajout de la validation de date ¹

² Indicateur non filtrable ajouté

 

### Affectation

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
|   |   |   |   | assignUserToRoleOnProjects |   |   |
|   |   |   |   | swapUsersOnProjects |   |   |
|   |   |   |   | unassignUserFromProjects |   |   |

{style=&quot;table-layout:auto&quot;}

 

### Niveau de référence 

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| workRequired¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Indicateur non filtrable ajouté

 

### Tâche de ligne de base

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| workRequired¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Indicateur non filtrable ajouté

 

### Enregistrement de facturation

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| billingDate¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ indicateur de champ NO_TIME ajouté

### Événement de blocage 

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| eventInitiator |   |   |   |   |   | `ADD` |
|   |   |   |   |   |   | `DELETE` |

{style=&quot;table-layout:auto&quot;}

 

### Catégorie 

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
|   |   |   |   | getCascadingRules |   |   |
|   |   |   |   | reorderCategories |   |   |

{style=&quot;table-layout:auto&quot;}

 

Énumération personnalisée 

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
|   |   |   |   | getGroupDefaultProjectStatus | opTaskGroupStatuses |   |
|   |   |   |   | isPossibleToUnlockStatus | projectGroupStatuses |   |
|   |   |   |   |   | taskGroupStatuses |   |

{style=&quot;table-layout:auto&quot;}

 

Document 

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| `checkedOutByID` | `checkedOutBy`  |   |  isDir |   |   |   |
| `isDir`  |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

Taux de change 

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| rate¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Changement de la validation PRECISION pour 8 à 9

 

### Intégration

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| syncBurndownDate |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

### Entrée au journal

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| changeType¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Modifications apportées aux valeurs possibles

 

### Optask (Problème)¹ 

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| workRequired² |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ marqués comme RESTORABLES

² Indicateur non filtrable ajouté

 

### Projet¹ 

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| completedHours |   | `openOpTasks` |  openOpTasks |   |   |   |
| isOriginalScheduleHoursSet |   | resourceGuidelines | resourceManagerIDs  |   |   |   |
| originalWorkRequired |   |   | `work` |   |   |   |
| syncBurndownDate |   |   |   |   |   |   |
| work |   |   |   |   |   |   |
| workRequired |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ marquée comme RESTORABLE et RESOURCE_MANAGEABLE

² Indicateur non filtrable ajouté

 

### Tâche¹

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| constraintDate² |   |   |   |   |   |   |
| workRequired³ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ marqués comme RESTORABLES

Ajout du programme de validation ² AT_DATE_YEAR_BEFORE

³ Indicateur non filtrable ajouté

 

### Équipe

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| `myWorkViewID` |  `myWorkView` |   |   |   |   |   |
| `requestsViewID`  | `myRequestsView`  |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

### Modèle¹ 

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
|   |   | resourceGuidelines | resourceManagerIDs |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ marquée comme RESTORABLE et RESOURCE_MANAGEABLE

### Tâche de modèle¹ 

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| workRequired² |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ marqués comme RESTORABLES

² Indicateur non filtrable ajouté

 

### Utilisateur

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| myInfo¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Violateurs MAX_LENGTH

 

### Note de l’utilisateur

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
| eventType¹ |   |   |   |   | myNotifications² |   |

{style=&quot;table-layout:auto&quot;}

¹ Valeurs possibles modifiées

² contient des filtres changés en `[true]`

 

### Annonce

| Champs | Références | Collections | Recherche | Actions | Requêtes | Opérations |
|---|---|---|---|---|---|---|
|   |   |   |   | `fileHandle` |   |   |
|   |   |   |   | `zipAnnouncementAttachments`  |   |   |
