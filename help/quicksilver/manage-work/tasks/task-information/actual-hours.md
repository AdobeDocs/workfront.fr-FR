---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Afficher les heures effectives
description: Les heures pendant lesquelles vous vous connectez à vos tâches dans Adobe Workfront sont considérées comme des heures réelles.
author: Alina
feature: Work Management
exl-id: c4b0e431-1765-416d-89f5-6ac663ac1d4f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '796'
ht-degree: 12%

---

# Afficher les heures effectives

Les heures pendant lesquelles vous vous connectez à vos tâches dans Adobe Workfront sont considérées comme des heures réelles.

Les heures réelles représentent le temps réel nécessaire à la réalisation d’une tâche, d’un problème ou d’un projet.

Nous recommandons que les heures soient consignées sur les tâches, qui sont des tâches et des problèmes.

En tant qu’administrateur de Workfront, vous pouvez toutefois permettre aux utilisateurs de se connecter aux projets en fonction des workflows de votre entreprise.

Pour plus d’informations sur la configuration de votre système pour permettre aux utilisateurs de se connecter aux projets, voir [ Configuration des préférences de feuille de temps et d’heure](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Travail ou supérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Affichage ou accès supérieur à Tâches, Projets ou Problèmes</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Afficher ou des autorisations supérieures pour une tâche, un projet ou un problème</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Heures réelles sur les tâches et les problèmes par rapport aux Heures réelles sur les projets

Les Heures réelles sur les tâches et les problèmes représentent le nombre d’heures enregistrées directement sur les tâches et les problèmes.

>[!NOTE]
>
>Les heures réelles des tâches enfants sont cumulées aux heures réelles sur la tâche parent. La formule suivante s’applique aux Heures réelles sur une tâche parente :

```
Parent Task Actual Hours = All Tasks Actual Hours + Parent Task Actual Hours
```

Les heures réelles pour les projets représentent un total des heures réelles de toutes les tâches du projet (y compris les heures connectées directement sur les tâches parents), tous les problèmes du projet ainsi que les heures réelles connectées sur le projet lui-même.

La formule suivante s’applique aux Heures réelles sur un projet :

```
Project Actual Hours = All Tasks Actual Hours + All Issues Actual Hours + All Project Actual Hours
```

## Rechercher les heures réelles

La recherche de la valeur Heures réelles pour un élément est identique pour les tâches, les projets et les problèmes.

Vous trouverez les informations Heures réelles sur les tâches aux emplacements suivants :

* [Heures réelles dans la section Détails](#actual-hours-in-the-details-section)
* [Heures réelles dans la section Heures](#actual-hours-in-the-hours-section)
* [Heures réelles dans les rapports](#actual-hours-in-reports)
* [Heures réelles dans les outils de gestion des ressources](#actual-hours-in-resource-management-tools)

### Heures réelles dans la section Détails {#actual-hours-in-the-details-section}

La section Détails de la recherche des heures réelles est identique pour les projets, les tâches et les problèmes.

Pour localiser Heures réelles dans Détails de la tâche :

1. Accédez à une tâche pour laquelle vous souhaitez passer en revue les Heures réelles.
1. Cliquez sur **Détails de la tâche** dans le panneau de gauche.
1. Cliquez sur **Overview** et remarquez la valeur **Real Hours** .

   Il s’agit du nombre total d’heures de connexion à cette tâche.

### Heures réelles dans la section Heures {#actual-hours-in-the-hours-section}

La section Heures réelles de la section Heures est identique pour les projets, les tâches et les problèmes.

Pour localiser les heures réelles dans la section Heures :

1. Accédez à une tâche pour laquelle vous souhaitez passer en revue les Heures réelles.
1. Cliquez sur **Hours** dans le panneau de gauche.

   Selon votre configuration, la section Heures peut être répertoriée sous **Afficher plus**.

   Cette option affiche la liste des entrées d’heure enregistrées pour la tâche.

1. Assurez-vous que la vue **Standard** et le regroupement **Project** sont appliqués à cette liste.

   Le nombre affiché dans la ligne de groupement pour la colonne **Hours** est le nombre total d’Heures réelles sur la tâche.

### Heures réelles dans les rapports {#actual-hours-in-reports}

Lors de la création de rapports de tâches, de problèmes ou de projets, vous pouvez afficher la valeur Heures réelles pour chaque tâche, problème ou projet dans le rapport.

L’ajout de la colonne Heures réelles à une vue de tâche est similaire à la création d’une vue dans un rapport.

Pour afficher les heures réelles dans un rapport de tâche :

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit de Workfront, puis sur **Rapports**.
1. Cliquez sur **Nouveau rapport**, puis choisissez **Tâche** comme objet.

1. Cliquez sur **Ajouter la colonne** et commencez à saisir **Heures réelles** lorsque le champ déroulant **Afficher dans cette colonne** s’affiche. Sélectionnez le champ lorsqu’il apparaît dans la liste.

1. Cliquez sur **Enregistrer + Fermer** pour enregistrer le rapport.

   La colonne Heures réelles indique le nombre d’heures enregistrées pour chaque tâche.

### Heures réelles dans les outils de gestion des ressources {#actual-hours-in-resource-management-tools}

Si vous souhaitez voir l’avancement du travail de vos utilisateurs sur les tâches et problèmes qui leur sont assignés, vous pouvez les afficher dans les outils de gestion des ressources suivants :

* Rapport Utilisation.\
  Pour plus d’informations sur le rapport d’utilisation, voir [Présentation du rapport d’utilisation des ressources](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

* planificateur de ressources.

  Pour plus d’informations sur l’affichage des heures réelles dans le planificateur de ressources, voir [Affichage des heures disponibles, planifiées et réelles ou de l’éditeur de texte enrichi dans le planificateur de ressources lors de l’utilisation de la vue utilisateur](../../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md).

## Enregistrer des heures

Vous pouvez consigner le temps passé sur les tâches, les problèmes et les projets de plusieurs façons.

Pour plus d’informations sur l’heure de connexion dans Workfront, voir [Durée de connexion](../../../timesheets/create-and-manage-timesheets/log-time.md).
