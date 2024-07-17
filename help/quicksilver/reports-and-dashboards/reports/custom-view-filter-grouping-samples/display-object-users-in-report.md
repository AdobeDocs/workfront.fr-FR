---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Rapports ou listes : afficher les utilisateurs associés à un objet"
description: Vous pouvez afficher les utilisateurs, les rôles de tâche et les équipes associés aux objets dans les rapports ou les listes, et les référencer dans les filtres. Vous ne pouvez pas les regrouper par utilisateurs, rôles de tâche ou équipes associés à des objets.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 9abdaafb-da2c-4b5d-9117-59afa4a1e71f
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '659'
ht-degree: 3%

---

# Rapports ou listes : afficher les utilisateurs et utilisatrices associés à un objet

Vous pouvez afficher les utilisateurs, les rôles de tâche et les équipes associés aux objets dans les rapports ou les listes, et les référencer dans les filtres. Vous ne pouvez pas les regrouper par utilisateurs, rôles de tâche ou équipes associés à des objets.

Vous pouvez afficher ou filtrer par utilisateurs, rôles de tâche ou équipes associés aux objets suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Objet</td> 
   <td>Utilisateurs associés ou rôles de tâche</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Projet</td> 
   <td> <p>Vous pouvez afficher tous les utilisateurs et les rôles de tâche qu’ils remplissent sur le projet dans un rapport de projet. Vous ne pouvez pas filtrer par les utilisateurs ni par leurs rôles de tâche associés dans un rapport de projet. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Tâches</td> 
   <td>Vous pouvez afficher et filtrer par tous les utilisateurs, rôles de tâche et équipes affectés à une tâche dans un rapport de tâche.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Problèmes</td> 
   <td>Vous pouvez afficher et filtrer par tous les utilisateurs, rôles de tâche et équipes affectés à un problème dans un rapport de problème.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Portefeuilles</td> 
   <td>Vous pouvez afficher tous les utilisateurs et les rôles de tâche qu’ils remplissent sur le projet dans un rapport de projet et les regrouper par Portfolio. Vous ne pouvez pas filtrer par les utilisateurs ni par leurs rôles de tâche associés dans un rapport de projet.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Programmes</td> 
   <td>Vous pouvez afficher tous les utilisateurs et les rôles de tâche qu’ils remplissent sur le projet dans un rapport de projet et regrouper le rapport par programme. Vous ne pouvez pas filtrer par les utilisateurs ni par leurs rôles de tâche associés dans un rapport de projet.</td> 
  </tr> 
 </tbody> 
</table>

## Affichage de tous les utilisateurs et rôles de tâche associés à un projet

Vous pouvez afficher tous les utilisateurs associés à dans le projet dans la vue d’une liste de projets ou d’un rapport. Cela inclut tous les utilisateurs répertoriés dans la section Personnes du projet. Vous pouvez également afficher les rôles auxquels ils sont associés lorsqu’ils sont affectés à des tâches ou à des problèmes sur le projet dans un rapport de projet.

![](assets/project-with-user-and-role-information-report-350x100.png)

Pour plus d’informations sur la création d’un rapport de projet pour afficher tous les utilisateurs et leurs rôles sur le projet, voir [Affichage : liste des utilisateurs de projet avec des rôles de tâche](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-project-user-list.md).

Vous ne pouvez pas filtrer les utilisateurs ou les rôles de tâche associés aux projets dans un filtre de projet.

## Affichage de tous les utilisateurs, rôles de tâche ou équipes affectés à une tâche

Vous pouvez afficher tous les utilisateurs, rôles ou équipes affectés à une tâche dans la vue d’une liste de tâches ou d’un rapport en ajoutant le champ Affectations à la vue.

![](assets/assignments-field-task-view-350x124.png)

Vous pouvez filtrer par utilisateurs, rôles de tâche ou équipes affectés à des tâches en référençant les champs suivants dans un filtre de tâche :

* Utilisateurs de l’affectation
* Rôles pour l’affectation
* Equipe

![](assets/assignment-users-roles-task-filter-350x334.png)

## Affichage de tous les utilisateurs, rôles de tâche ou équipes affectés à un problème

Vous pouvez afficher tous les utilisateurs, rôles ou équipes affectés à un problème dans l’affichage d’une liste de problèmes ou d’un rapport en ajoutant le champ Affectations à la vue.

Vous pouvez filtrer par utilisateurs, rôles de tâche ou équipes affectés à des problèmes en référençant les champs suivants dans un filtre de problèmes :

* Utilisateurs de l’affectation
* Rôles pour l’affectation
* Equipe

## Affichage de tous les utilisateurs et rôles de tâche associés à un portfolio

Vous pouvez afficher tous les utilisateurs et rôles associés à un portfolio en les affichant dans un rapport de projet, puis en regroupant le rapport par Portfolio.

Pour plus d’informations sur la création d’un rapport de projet pour afficher tous les utilisateurs et leurs rôles sur le projet, voir [Affichage : liste des utilisateurs de projet avec des rôles de tâche](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-project-user-list.md).

Vous ne pouvez pas filtrer les utilisateurs ou les rôles de tâche associés aux projets d’un portfolio ou d’un filtre de projet.

## Afficher tous les utilisateurs et les rôles de tâche associés à un programme

Vous pouvez afficher tous les utilisateurs et rôles associés à un programme en les affichant dans un rapport de projet, puis en regroupant le rapport par programme.

Pour plus d’informations sur la création d’un rapport de projet pour afficher tous les utilisateurs et leurs rôles sur le projet, voir [Affichage : liste des utilisateurs de projet avec des rôles de tâche](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-project-user-list.md).

Vous ne pouvez pas filtrer les utilisateurs ou les rôles de tâche associés aux projets dans un programme ou un filtre de projet.
