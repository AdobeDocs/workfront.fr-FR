---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Afficher les heures effectives
description: Les heures que vous consignez pour vos éléments de travail dans Adobe Workfront sont considérées comme des heures effectives.
author: Alina
feature: Work Management
exl-id: c4b0e431-1765-416d-89f5-6ac663ac1d4f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '796'
ht-degree: 100%

---

# Afficher les heures effectives

Les heures que vous consignez pour vos éléments de travail dans Adobe Workfront sont considérées comme des heures effectives.

Les heures effectives représentent le temps réel nécessaire à la réalisation d’une tâche, d’un problème ou d’un projet.

Nous recommandons de consigner les heures sur les éléments de travail, qui sont des tâches et des problèmes.

En tant qu’administrateur ou administratrice de Workfront, vous pouvez toutefois autoriser les personnes à se connecter aux projets en fonction des workflows de votre organisation.

Pour plus d’informations sur la configuration de votre système pour permettre aux utilisateurs et utilisatrices de consigner le temps passé sur les projets, voir la section [Configurer les préférences de feuille de temps et d’heure](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Travail ou supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Accès en affichage ou supérieur aux tâches, projets ou problèmes</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations d’affichage ou supérieures à une tâche, un projet ou un problème</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Heures effectives sur les tâches et les problèmes ou heures effectives sur les projets

Les heures effectives sur les tâches et les problèmes représentent le nombre d’heures consignées directement sur les tâches et les problèmes.

>[!NOTE]
>
>Les heures effectives des tâches enfant sont cumulées avec les heures effectives de la tâche parent. La formule suivante s’applique aux heures effectives sur une tâche parent :

```
Parent Task Actual Hours = All Tasks Actual Hours + Parent Task Actual Hours
```

Les heures effectives des projets représentent le total des heures effectives de toutes les tâches du projet (y compris des heures consignées directement sur les tâches parent), de tous les problèmes du projet ainsi que des heures effectives consignées sur le projet lui-même.

La formule suivante s’applique aux heures effectives d’un projet :

```
Project Actual Hours = All Tasks Actual Hours + All Issues Actual Hours + All Project Actual Hours
```

## Trouver les heures effectives

La recherche de la valeur des heures effectives pour un élément est identique pour les tâches, les projets et les problèmes.

Vous trouverez les informations sur les heures effectives des tâches aux emplacements suivants :

* [Heures effectives dans la section Détails](#actual-hours-in-the-details-section)
* [Heures réelles dans la section Heures](#actual-hours-in-the-hours-section)
* [Heures effectives dans les rapports](#actual-hours-in-reports)
* [Heures effectives dans les outils de gestion des ressources](#actual-hours-in-resource-management-tools)

### Heures effectives dans la section Détails {#actual-hours-in-the-details-section}

La recherche d’heures effectives dans la section Détails est identique pour les projets, les tâches et les problèmes.

Pour localiser les heures effectives dans les détails de la tâche, procédez comme suit :

1. Accédez à une tâche pour laquelle vous souhaitez passer en revue les heures effectives.
1. Cliquez sur **Détails de la tâche** dans le panneau de gauche.
1. Cliquez sur **Vue d’ensemble** et notez la valeur des **Heures effectives**.

   Il s’agit du nombre total d’heures consignées sur cette tâche.

### Heures effectives dans la section Heures {#actual-hours-in-the-hours-section}

La recherche d’heures effectives dans la section Heures est identique pour les projets, les tâches et les problèmes.

Pour localiser les heures effectives dans la section Heures, procédez comme suit :

1. Accédez à une tâche pour laquelle vous souhaitez passer en revue les heures effectives.
1. Cliquez sur **Heures** dans le panneau de gauche.

   Selon votre configuration, la section Heures peut être répertoriée sous **Afficher plus**.

   Cette option affiche la liste des entrées d’heures consignées pour la tâche.

1. Assurez-vous que la vue **Standard** et le regroupement **Projet** sont appliqués à cette liste.

   Le nombre affiché dans la ligne des regroupements pour la colonne **Heures** correspond au nombre total d’heures effectives sur la tâche.

### Heures effectives dans les rapports {#actual-hours-in-reports}

Lors de la création de rapports sur les tâches, problèmes ou projets, vous pouvez afficher la valeur Heures effectives pour chaque tâche, problème ou projet dans le rapport.

L’ajout de la colonne Heures effectives à une vue de tâche est similaire à la création d’une vue dans un rapport.

Pour afficher les heures effectives dans un rapport de tâche, procédez comme suit :

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) en haut à droite de Workfront, puis cliquez sur **Rapports**.
1. Cliquez sur **Nouveau rapport**, puis choisissez l’objet **Tâche**.

1. Cliquez sur **Ajouter une colonne**, puis commencez à saisir les **Heures effectives** lorsque le champ déroulant **Afficher dans cette colonne** s’affiche. Sélectionnez le nom lorsqu’il apparaît dans la liste.

1. Cliquez sur **Enregistrer et fermer** pour enregistrer le rapport.

   La colonne Heures effectives indique le nombre d’heures consignées pour chaque tâche.

### Heures effectives dans les outils de gestion des ressources {#actual-hours-in-resource-management-tools}

Si vous souhaitez voir la progression du travail de vos utilisateurs et utilisatrices sur les tâches et problèmes qui leur sont affectés, vous pouvez les afficher dans les outils de gestion des ressources suivants :

* Rapport d’utilisation.\
  Pour plus d’informations sur le rapport d’utilisation, voir la section [Vue d’ensemble du rapport Utilisation des ressources](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

* Planificateur de ressources

  Pour plus d’informations sur l’affichage des heures effectives dans le planificateur de ressources, voir la section [Afficher les heures disponibles, prévues et effectives ou l’équivalent temps complet dans le planificateur de ressources lors de l’utilisation de la vue d’utilisation](../../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md).

## Enregistrer des heures

Vous pouvez consigner le temps passé sur les tâches, les problèmes et les projets de plusieurs façons.

Pour plus d’informations sur la consignation du temps dans Workfront, voir la section [Consigner le temps](../../../timesheets/create-and-manage-timesheets/log-time.md).
