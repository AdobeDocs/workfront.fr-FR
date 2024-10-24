---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filtre : Tâches personnelles'
description: Ce filtre de tâche renvoie des requêtes de travail ad hoc envoyées à un utilisateur ou des éléments à faire ajoutés par les utilisateurs dans leur zone d’accueil. Les tâches personnelles ne sont pas connectées à un projet, mais elles peuvent être déplacées vers un projet, si nécessaire.
author: Nolan
feature: Reports and Dashboards
source-git-commit: 1e69d715f343bfef1e5aee658a1dff12abfc61a0
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 27%

---

# Filtre : tâches personnelles

<!--Audited: 10/2024-->

Ce filtre de tâche renvoie des requêtes de travail ad hoc envoyées à un utilisateur ou des éléments à faire ajoutés par les utilisateurs dans leur zone d’accueil.

Les requêtes de travail ad hoc et les tâches sont enregistrées dans Adobe Workfront en tant que tâches personnelles.

Les tâches personnelles ne sont pas connectées à un projet, mais elles peuvent être déplacées vers un projet, si nécessaire.

![](assets/personal-tasks-report.png)

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
   <ul><li><p>Contributeur à la modification d’un filtre </p></li>
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

*Pour plus d’informations, voir [Exigences d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Filtrage des tâches personnelles

Pour créer ce filtre :

1. Accédez à une liste de tâches ou à un rapport de tâches.
1. Dans le menu déroulant **Filtre**, cliquez sur **Nouveau filtre**.
1. (Conditionnel) Cliquez sur **Ajouter une règle de filtre** pour accéder au filtre à partir d’un rapport ou commencez à sélectionner vos critères de filtre dans le premier champ, si vous accédez au filtre à partir d’une liste.
1. (Conditionnel) Sélectionnez les critères de filtrage suivants :

   * À partir d’un filtre de liste : **Task** > **Personal** **Is true**
   * À partir d’un filtre de rapport : **Tâche** > **Personnelle** > **Égal À** > **True**.
1. Enregistrez le filtre.

   La liste affiche uniquement les tâches personnelles qui ne figurent sur aucun projet.
