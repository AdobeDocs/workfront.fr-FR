---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Afficher les heures effectives
description: Les heures que vous consignez pour vos éléments de travail dans Adobe Workfront sont considérées comme des heures effectives.
author: Alina
feature: Work Management
exl-id: c4b0e431-1765-416d-89f5-6ac663ac1d4f
source-git-commit: 3827e834a71084f14a99cb27aadefd97327b02d7
workflow-type: tm+mt
source-wordcount: '759'
ht-degree: 64%

---

# Afficher les heures effectives

<!-- Audited: 5/2025 -->

Les heures que vous consignez pour vos éléments de travail dans Adobe Workfront sont considérées comme des heures effectives.

Les heures effectives représentent le temps réel nécessaire à la réalisation d’une tâche, d’un problème ou d’un projet.

Nous vous recommandons de consigner les heures relatives aux éléments de travail, qui sont des tâches et des événements. Cependant, en tant qu’administrateur ou administratrice Workfront, vous pouvez autoriser les utilisateurs et utilisatrices à enregistrer également le temps passé sur les projets en fonction des workflows de votre organisation.

Pour plus d’informations sur la configuration de votre système pour permettre aux utilisateurs et utilisatrices de consigner le temps passé sur les projets, voir la section [Configurer les préférences de feuille de temps et d’heure](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

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
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> 
   <p>Nouveau : Standard<p>
   <p>Ou</p>
   <p>Actuellement : Travail ou licence supérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès en affichage ou supérieur aux tâches, projets ou problèmes</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations d’affichage ou supérieures à une tâche, un projet ou un problème</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, voir [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Heures effectives sur les tâches et les problèmes ou heures effectives sur les projets

Les heures effectives sur les tâches et les problèmes représentent le nombre d’heures consignées directement sur les tâches et les problèmes.

Les heures effectives des tâches enfant sont cumulées avec les heures effectives de la tâche parent. La formule suivante s’applique aux heures effectives sur une tâche parent :

```
Parent Task Actual Hours = All Tasks Actual Hours + Parent Task Actual Hours
```

Les heures réelles pour les projets représentent un total d&#39;heures réelles de toutes les tâches du projet (y compris les heures enregistrées directement dans les tâches parents), de tous les événements du projet et des heures réelles enregistrées dans le projet lui-même.

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

1. Accédez à une tâche pour laquelle vous souhaitez consulter les heures effectives.
1. Dans le panneau de gauche, cliquez sur **Détails de la tâche**. La section **Aperçu** s’affiche.
1. Recherchez la valeur **Heures réelles** dans la section **Temps de travail**. Il s’agit du nombre total d’heures consignées sur cette tâche.

### Heures effectives dans la section Heures {#actual-hours-in-the-hours-section}

La recherche d’heures effectives dans la section Heures est identique pour les projets, les tâches et les problèmes.

Pour localiser les heures effectives dans la section Heures :

1. Accédez à une tâche pour laquelle vous souhaitez consulter les heures effectives.

1. Dans le panneau de gauche, cliquez sur **Heures**. Une liste des entrées d’heures consignées dans la tâche s’affiche, avec la colonne **Heures** indiquant le nombre total d’heures effectives de la tâche.

1. Assurez-vous que la vue **Standard** et le regroupement **Projet** sont appliqués à cette liste.

### Heures effectives dans les rapports {#actual-hours-in-reports}

Lors de la création de rapports sur les tâches, problèmes ou projets, vous pouvez afficher la valeur Heures effectives pour chaque tâche, problème ou projet dans le rapport.

Pour afficher les heures effectives dans un rapport de tâche, procédez comme suit :

{{step1-to-reports}}

1. Sur la page **Rapports**, cliquez sur **Nouveau rapport**, puis choisissez **Tâche** comme objet.
1. Dans l’angle inférieur droit de la page, cliquez sur **Ajouter une colonne**.
1. Dans le champ déroulant **Afficher dans cette colonne** qui s’affiche, commencez à saisir **Heures réelles**, puis sélectionnez le champ lorsqu’il apparaît dans la liste.

1. Dans le coin inférieur gauche de la page, cliquez sur **Enregistrer + Fermer** pour enregistrer le rapport.

1. Dans la boîte de dialogue **Nommer ce rapport pour l’enregistrer**, saisissez un nouveau nom de rapport, puis cliquez sur **Appliquer**.

### Heures effectives dans les outils de gestion des ressources {#actual-hours-in-resource-management-tools}

Si vous souhaitez voir la progression du travail de vos utilisateurs et utilisatrices sur les tâches et problèmes qui leur sont affectés, vous pouvez les afficher dans les outils de gestion des ressources suivants :

* Rapport d’utilisation.\
  Pour plus d&#39;informations, voir [Aperçu du rapport Utilisation des ressources](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

* Planificateur de ressources.

  Pour plus d&#39;informations, voir [Afficher les heures disponibles, prévues et réelles ou l&#39;équivalent temps complet dans le planificateur de ressources lorsque vous utilisez la vue Utilisateur](../../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md).

## Enregistrer des heures

Vous pouvez consigner le temps passé sur les tâches, les problèmes et les projets de plusieurs façons.

Pour plus d’informations, voir la section [Consigner le temps](../../../timesheets/create-and-manage-timesheets/log-time.md).
