---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Afficher les heures effectives
description: Les heures que vous enregistrez pour vos tâches dans Adobe Workfront sont considérées comme des heures réelles. Les heures effectives représentent le temps réel nécessaire à la réalisation d’une tâche, d’un problème ou d’un projet.
author: Alina
feature: Work Management
exl-id: c4b0e431-1765-416d-89f5-6ac663ac1d4f
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '1276'
ht-degree: 27%

---

# Afficher les heures effectives

<!-- Audited: 5/2025 -->

Les heures que vous consignez pour vos éléments de travail dans Adobe Workfront sont considérées comme des heures effectives.

Les heures effectives représentent le temps réel nécessaire à la réalisation d’une tâche, d’un problème ou d’un projet.

Nous vous recommandons de consigner les heures relatives aux éléments de travail, qui sont des tâches et des événements. Cependant, en tant qu’administrateur ou administratrice Workfront, vous pouvez autoriser les utilisateurs et utilisatrices à enregistrer également le temps passé sur les projets en fonction des workflows de votre organisation.

Pour plus d’informations sur la configuration de votre système pour permettre aux utilisateurs et utilisatrices de consigner le temps passé sur les projets, voir la section [Configurer les préférences de feuille de temps et d’heure](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

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
   <p>Standard<p>
   <p>Travail ou supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Afficher ou un accès supérieur aux tâches, projets ou événements</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations d’affichage ou supérieures à une tâche, un projet ou un problème</p></td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
 
 <table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> 
   <p>New: Standard<p>
   <p>Or</p>
   <p>Current: Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>View or higher access to Tasks, Projects, or Issues</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a task, a project, or an issue</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Heures réelles par rapport aux heures réelles héritées

En fonction de la zone du Workfront à partir de laquelle vous accédez aux heures réelles, elles peuvent se référer à l’une des heures consignées suivantes :

* Dans les rapports et listes de projets, de tâches et d’événements :

   * **Heures réelles** : heures enregistrées pour un projet, des tâches ou des événements entre mai 2021 et aujourd’hui. Ils sont stockés dans la base de données Workfront en heures et leur champ de valeur est `actualWorkRequiredDouble`.
   * **Heures réelles héritées** : heures enregistrées pour des projets, des tâches ou des événements, à tout moment, entre une date antérieure à mai 2021 et aujourd’hui. Elles sont stockées dans la base de données Workfront en minutes et leur champ de valeur est `actualWorkRequired`.

     Les heures consignées actuellement mettront à jour les heures réelles et les anciennes heures réelles.

     >[!IMPORTANT]
     >
     >Le coût réel du projet utilise les heures réelles héritées pour calculer.

* Dans la zone Détails du projet, de la tâche ou de l’événement , les heures réelles peuvent s’afficher dans les champs suivants :

   * **Heures réelles** : dans l’onglet Détails , il s’agit des heures enregistrées pour des projets, des tâches ou des événements entre mai 2021 et aujourd’hui. Ils sont stockés dans la base de données Workfront en heures et leur champ de valeur est `actualWorkRequiredDouble`.
   * **Heures réelles** : dans un formulaire personnalisé de projet, de tâche ou d’événement, lorsqu’ils sont accessibles à l’aide d’un champ personnalisé de référence de champ natif qui fait référence au champ natif des heures réelles. Il s’agit d’heures enregistrées pour des projets, des tâches ou des événements entre une date antérieure à mai 2021 et aujourd’hui. Ils sont stockés dans la base de données Workfront en heures et leur champ de valeur est `actualWorkRequiredDouble`.

     Les heures consignées actuellement mettront à jour les heures réelles et les anciennes heures réelles.

>[!NOTE]
>
>Il est recommandé d’utiliser le champ Heures réelles autant que possible, car le champ Anciennes heures réelles peut afficher des heures inexactes en raison de la manière dont les incréments sont arrondis lorsque les heures sont stockées en minutes.

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

### Heures effectives dans la section Détails {#actual-hours-in-the-details-section}

La recherche d’heures effectives dans la section Détails est identique pour les projets, les tâches et les problèmes.

Pour localiser les heures effectives dans les détails de la tâche, procédez comme suit :

1. Accédez à une tâche pour laquelle vous souhaitez consulter les heures effectives.
1. Dans le panneau de gauche, cliquez sur **Détails de la tâche**. La section **Aperçu** s’affiche.
1. Recherchez la valeur **Heures réelles** dans la section **Temps de travail**. Il s’agit du nombre total d’heures consignées sur cette tâche.
1. (Facultatif et conditionnel) Si la référence native du champ Heures réelles a été ajoutée à un formulaire personnalisé de projet, de tâche ou de problème, accédez au formulaire personnalisé et recherchez les Heures réelles dans le champ personnalisé. Il s’agit du nombre total d’heures enregistrées pour l’objet.

### Heures effectives dans la section Heures {#actual-hours-in-the-hours-section}

La recherche d’heures effectives dans la section Heures est identique pour les projets, les tâches et les problèmes.

Pour localiser les heures effectives dans la section Heures d&#39;une tâche :

1. Accédez à une tâche pour laquelle vous souhaitez consulter les heures effectives.

1. Dans le panneau de gauche, cliquez sur **Heures**. Une liste des entrées d’heures consignées dans la tâche s’affiche, avec la colonne **Heures** indiquant le nombre total d’heures effectives de la tâche.

1. Assurez-vous que la vue **Standard** et le regroupement **Projet** sont appliqués à cette liste.
1. Les heures réelles de la tâche s&#39;affichent dans la ligne de regroupement de la colonne **Heures réelles**.

### Heures réelles et heures réelles héritées dans les rapports

Lors de la création de rapports sur des tâches, des événements ou des projets, vous pouvez afficher les valeurs des heures effectives et des heures effectives héritées pour chaque tâche, événement ou projet du rapport.

Pour plus d&#39;informations sur la différence entre les heures effectives et les heures effectives héritées, voir la section [Heures effectives par rapport aux heures effectives héritées](#actual-hours-vs-legacy-actual-hours) dans cet article.

Pour afficher les heures effectives et les heures effectives héritées dans un rapport de tâche :

{{step1-to-reports}}

1. Sur la page **Rapports**, cliquez sur **Nouveau rapport**, puis choisissez **Tâche** comme objet.
1. Dans l’angle inférieur droit de la page, cliquez sur **Ajouter une colonne**.
1. Dans le champ déroulant **Afficher dans cette colonne**, commencez à saisir **Heures réelles**, puis sélectionnez le champ lorsqu’il apparaît dans la liste.
1. Répétez l’étape ci-dessus pour ajouter le champ **Anciennes heures effectives** au rapport.

1. Dans le coin inférieur gauche de la page, cliquez sur **Enregistrer + Fermer** pour enregistrer le rapport.

1. Dans la boîte de dialogue **Nommer ce rapport pour l’enregistrer**, saisissez un nouveau nom de rapport, puis cliquez sur **Appliquer**.
1. Répétez les mêmes étapes pour un rapport de projet ou de problème.

### Heures effectives dans les outils de gestion des ressources {#actual-hours-in-resource-management-tools}

Si vous souhaitez voir la progression du travail de vos utilisateurs et utilisatrices sur les tâches et problèmes qui leur sont affectés, vous pouvez les afficher dans les outils de gestion des ressources suivants :

* Rapport d’utilisation.\
  Pour plus d&#39;informations, voir [Aperçu du rapport Utilisation des ressources](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

* Planificateur de ressources.

  Pour plus d&#39;informations, voir [Afficher les heures disponibles, prévues et réelles ou l&#39;équivalent temps complet dans le planificateur de ressources lorsque vous utilisez la vue Utilisateur](../../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md).


### Heures réelles dans l’API Workfront

<!--this section was added as a result to this issue: https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/task/6810910e0001b932e0948336208e76f2/overview-->

La plupart des champs Workfront qui stockent des heures sont enregistrés dans la base de données Workfront en quelques minutes. Par exemple, le nom du champ Heures prévues d’une tâche est `workRequired` dans la base de données Workfront et stocké en minutes.

Vous devez tenir compte de la conversion de minutes en heures lors de l’accès à ces champs dans les appels API ou dans les champs ou colonnes calculés personnalisés.

Les heures réelles consignées pour les projets, tâches ou événements sont actuellement stockées dans la base de données Workfront sous la forme de minutes et leur champ de valeur est `actualWorkRequired`.

La publication de la version suivante de l’API Workfront est prévue pour fin 2025. Les heures réelles sont stockées dans les champs et unités suivants de la base de données :

* **Heures réelles** : heures enregistrées pour un projet, des tâches ou des événements postérieurs à mai 2021. Ils sont stockés dans la base de données Workfront en heures et leur champ de valeur est `actualWorkRequiredDouble`.
* **Heures réelles héritées** : heures enregistrées pour des projets, des tâches ou des événements, à tout moment, y compris avant mai 2021. Elles sont stockées dans la base de données Workfront en minutes et leur champ de valeur est `actualWorkRequired`.

Pour plus d’informations sur les versions des API, voir [Contrôle de version des API et planning de prise en charge](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

>[!IMPORTANT]
>
>Le coût réel du projet utilise les heures réelles héritées pour calculer.

Pour plus d&#39;informations sur l&#39;utilisation des heures réelles dans les colonnes ou champs calculés, voir [FAQ sur les rapports](/help/quicksilver/reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md).

## Enregistrer des heures

Vous pouvez consigner le temps passé sur les tâches, les problèmes et les projets de plusieurs façons.

Pour plus d’informations, voir la section [Consigner le temps](../../../timesheets/create-and-manage-timesheets/log-time.md).
