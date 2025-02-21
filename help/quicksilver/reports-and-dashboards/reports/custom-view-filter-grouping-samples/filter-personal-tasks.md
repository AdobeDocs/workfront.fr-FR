---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filtrer : tâches personnelles'
description: Ce filtre de tâches renvoie les demandes de travail ad hoc envoyées à un utilisateur ou une utilisatrice, ou les tâches ajoutées par les utilisateurs et utilisatrices dans leur zone d’Accueil. Les tâches personnelles ne sont pas liées à un projet, mais elles peuvent être déplacées vers un projet, si nécessaire.
author: Nolan
feature: Reports and Dashboards
exl-id: 204cfae1-7c57-4223-9e00-ac94e1e2ba3a
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '305'
ht-degree: 26%

---

# Filtrer : tâches personnelles

<!--Audited: 10/2024-->

Ce filtre de tâches renvoie les demandes de travail ad hoc envoyées à un utilisateur ou une utilisatrice, ou les tâches ajoutées par les utilisateurs et utilisatrices dans leur widget Tâches dans la zone d’Accueil.

Les demandes de travail ad hoc et les tâches à effectuer sont enregistrées dans Adobe Workfront en tant que tâches personnelles.

Les tâches personnelles ne sont pas liées à un projet, mais elles peuvent être déplacées vers un projet, si nécessaire. Pour plus d’informations, voir [Créer des tâches personnelles](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/create-personal-tasks.md).

![Rapport des tâches personnelles](assets/personal-tasks-report.png)

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> 
    <p>Nouveau :</p>
   <ul><li><p>Contributeur pour modifier un filtre </p></li>
   <li><p>Standard pour modifier un rapport</p></li> </ul>

<p>Actuel :</p>
   <ul><li><p>Demande de modification d’un filtre </p></li>
   <li><p>Prévoir de modifier un rapport</p></li> </ul></td> 
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

*Pour plus d’informations, voir [Conditions d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
