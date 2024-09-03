---
content-type: overview
product-area: projects
navigation-topic: manage-tasks
title: Vue d’ensemble du chemin critique du projet
description: La détermination du chemin critique d’un projet est une méthode automatique permettant à Adobe Workfront de signaler une séquence de tâches dans un projet qui a le potentiel d’affecter la chronologie du projet. Les tâches pouvant avoir un impact sur la chronologie du projet sont marquées comme étant des tâches de chemin critique.
author: Alina
feature: Work Management
exl-id: 9cbc84bf-d02b-4bb7-8d5d-922554d1262e
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '764'
ht-degree: 100%

---

# Vue d’ensemble du chemin critique du projet

La détermination du chemin critique d’un projet est une méthode automatique permettant à Adobe Workfront de signaler une séquence de tâches dans un projet qui a le potentiel d’affecter la chronologie du projet. Les tâches pouvant avoir un impact sur la chronologie du projet sont marquées comme étant des tâches de chemin critique.

Les fonctionnalités suivantes peuvent avoir un impact sur le chemin critique d’un projet :

* La structure de répartition du travail du projet.

  Pour plus d’informations sur la structure de répartition du travail, voir [Déterminer la structure de répartition du travail dans un projet](../../../manage-work/projects/planning-a-project/determine-project-work-breakdown-structure.md).

* Le temps (durée) nécessaire à l’exécution de chaque tâche.
* Les dépendances entre les tâches.

  Tenez compte des points suivants :

   * Lorsqu’une tâche sur le chemin critique a une relation précédente, ses tâches antérieures et ultérieures sont également sur le chemin critique si les modifications sur les dates des tâches antérieures ou ultérieures ont un impact direct sur leurs dépendances.

     >[!TIP]
     >
     >Lorsque la date de la tâche antérieure d’une tâche n’a pas d’impact direct sur la date de leurs tâches dépendantes et qu’elle n’a aucune incidence sur les dates du projet, la tâche ultérieure n’est pas sur le chemin critique.
     >
     >
     >![](assets/successor-not-on-critical-path-350x150.png)     >
     >

   * Lorsqu’une sous-tâche est identifiée en tant que tâche sur Chemin critique, la tâche parente est également identifiée en tant que tâche sur Chemin critique, si la Date et l’heure de début prévues du parent sont identiques à celles de la sous-tâche.

En tenant compte de ces fonctions, le système calcule le chemin critique en utilisant le chemin le plus long entre la tâche la plus ancienne et la tâche qui détermine la fin du projet. Le calcul du chemin critique prend en compte la première et la dernière fois où chaque tâche peut commencer et se terminer sans rallonger le projet. Ce processus détermine quelles tâches sont « critiques » (et appartiennent au chemin le plus long) et lesquelles sont « totalement flottantes » (peuvent être retardées sans rallonger le projet).

Tout retard dans l’activité d’une tâche sur le chemin critique affecte directement la date d’achèvement projetée du projet (il n’y a pas de flottement sur le chemin critique).

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
   <td> <p>Accès d’affichage ou supérieur aux tâches</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations d’affichage ou supérieures sur une tâche </p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, consultez la section <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Afficher le chemin critique

Vous pouvez afficher les tâches qui appartiennent au chemin critique dans les zones suivantes de l’application Workfront :

* [Afficher le chemin critique dans le graphique de Gantt](#view-the-critical-path-in-the-gantt-chart)
* [Afficher le chemin critique dans une liste de tâches ou un rapport](#view-the-critical-path-in-a-task-list-or-report)

### Afficher le chemin critique dans le graphique de Gantt {#view-the-critical-path-in-the-gantt-chart}

Pour afficher les tâches sur le chemin critique dans le graphique de Gantt :

1. Accédez à un projet pour lequel vous souhaitez afficher le chemin critique.
1. Cliquez sur **Tâches** dans le panneau de gauche.
1. Cliquez sur l’icône **Graphique de Gantt** dans le coin supérieur droit de la liste des tâches.

   ![gantt_chart_icon__1_.png](assets/gantt-chart-icon--1-.png)

1. Développez le menu **Options**, puis activez l’option **Chemin critique**.

   Les tâches qui se trouvent sur le chemin critique ont une ligne rouge au-dessus de leur chronologie dans le graphique de Gantt.

   ![crtitical_path_on_gantt__1_.png](assets/crtitical-path-on-gantt--1--350x137.png)

### Afficher le chemin critique dans une liste de tâches ou un rapport {#view-the-critical-path-in-a-task-list-or-report}

Pour afficher les tâches qui se trouvent sur le chemin critique dans une liste de tâches :

1. Accédez à un projet pour lequel vous souhaitez afficher le chemin critique.
1. Cliquez sur **Tâches** dans le panneau de gauche.
1. Dans le menu déroulant **Vue**, sélectionnez **Statut**.

   Les tâches qui se trouvent sur le chemin critique ont un indicateur **Chemin critique** dans la colonne **Indicateurs** de la liste.

   Vous pouvez appliquer la même vue à un rapport de tâche.

   Pour plus d’informations sur la création de rapports, voir l’article [Créer un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

   Ou

   Cliquez sur le menu déroulant **Filtre** et sélectionnez **Nouveau filtre**.

1. Cliquez sur **Ajouter une règle de filtre** et commencez à saisir **Critique** dans le champ **Montrer uniquement les tâches dans lesquelles ...**.

1. Sélectionnez le nom qui apparaît dans la liste.
1. Cliquez sur **Enregistrer le filtre**.

   La liste ne doit afficher que les tâches qui se trouvent sur le chemin critique.
