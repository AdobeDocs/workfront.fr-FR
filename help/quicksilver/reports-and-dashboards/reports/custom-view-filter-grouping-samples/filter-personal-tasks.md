---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filtrer : tâches personnelles'
description: Ce filtre de tâches renvoie les demandes de travail ad hoc envoyées à un utilisateur ou une utilisatrice, ou les tâches ajoutées par les utilisateurs et utilisatrices dans leur zone d’Accueil. Les tâches personnelles ne sont pas liées à un projet, mais elles peuvent être déplacées vers un projet, si nécessaire.
author: Courtney
feature: Reports and Dashboards
exl-id: 204cfae1-7c57-4223-9e00-ac94e1e2ba3a
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/qh9Tp3JY32C-GL2U5ucjapeVoR4dKq0F8K6lysGiOag
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 296
ht-degree: 22%

---

# Filtre : tâches personnelles

<!--Audited: 10/2024-->

Ce filtre de tâches renvoie les demandes de travail ad hoc envoyées à un utilisateur ou une utilisatrice, ou les tâches ajoutées par les utilisateurs et utilisatrices dans leur widget Tâches dans la zone d’Accueil.

Les demandes de travail ad hoc et les tâches à effectuer sont enregistrées dans Adobe Workfront en tant que tâches personnelles.

Les tâches personnelles ne sont pas liées à un projet, mais elles peuvent être déplacées vers un projet, si nécessaire. Pour plus d’informations, voir [Créer des tâches personnelles](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/create-personal-tasks.md).

![Rapport des tâches personnelles](assets/personal-tasks-report.png)

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> 
   <p>Contributeur ou demande de modification d’un filtre </p>
   <p>Standard ou Plan pour modifier un rapport</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès aux rapports, tableaux de bord et calendriers pour modifier un rapport</p> <p>Modifier l’accès aux filtres, aux vues et aux regroupements pour modifier un filtre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p>  </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez l’article [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Filtrer les tâches personnelles

Pour créer ce filtre :

1. Accédez à une liste de tâches ou à un rapport de tâche.
1. Dans le menu déroulant **Filtre**, cliquez sur **Nouveau filtre**.
1. (Conditionnel) Cliquez sur **Ajouter une règle de filtrage** si vous accédez au filtre à partir d’un rapport ou commencez à sélectionner vos critères de filtre dans le premier champ, si vous accédez au filtre à partir d’une liste.
1. (Conditionnel) Sélectionnez les critères de filtrage suivants :

   * À partir d’un filtre de liste : **Tâche** > **Personnel** **Est vrai**
   * À partir d’un filtre de rapport : **Tâche** > **Personnel** > **Égal à (sensible à la casse)** > **Vrai**.
1. Enregistrez le filtre.

   La liste affiche uniquement les tâches personnelles qui ne font partie d’aucun projet.
