---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Vue d’ensemble de la date d’achèvement prévue pour les projets, les tâches et les problèmes
description: La date de fin prévue est un indicateur calculé en temps réel du moment où le projet, la tâche ou le problème sera terminé. Lorsque le projet, la tâche ou le problème est marqué comme terminé, la date d’achèvement prévue est remplacée par la date d’achèvement réel.
author: Alina
feature: Work Management
exl-id: dde400e6-189f-4431-8f2f-7142ce424826
source-git-commit: 811d8076a0b344e863b25aa253a0fb1c102f0435
workflow-type: tm+mt
source-wordcount: '873'
ht-degree: 6%

---

# Vue d’ensemble de la date d’achèvement prévue pour les projets, les tâches et les problèmes

<!-- Audited: 1/2024 -->

La date de fin prévue est un indicateur calculé en temps réel du moment où le projet, la tâche ou le problème sera terminé. Lorsque le projet, la tâche ou le problème est marqué comme terminé, la date d’achèvement prévue est remplacée par la date d’achèvement réel.

Les sections suivantes décrivent comment la date d’achèvement prévue est déterminée pour les projets, les tâches et les problèmes, et comment la localiser.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> 
   <p>Nouveau : 
   <ul><li><p>Contributeur ou version ultérieure pour afficher la date d’achèvement prévue dans un rapport</p></li> <li><p>Une licence standard pour créer un rapport</p></li> </ul>

<p>Actuel : 
   <ul><li><p>Passez en revue la date d’achèvement prévue ou ultérieure pour l’afficher dans un rapport.</p></li> 
   <li><p>Une licence Plan pour créer un rapport</p> </li></ul>
      </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Niveau d’accès</td> 
   <td> <p>Accès en affichage ou supérieur pour les projets</p> <p>Pour créer un rapport, vous devez disposer des droits d’édition sur les rapports, tableaux de bord et calendriers.</p> <p>Vous devez disposer d’un accès en édition aux options Filtres, Vues et Groupements pour créer un rapport ou modifier le mode Liste.</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Affichage ou autorisations supérieures d’un projet</p> </td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations sur les informations contenues dans ce tableau, voir [Exigences d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Comment Adobe Workfront détermine la date d’achèvement prévue

La date de fin prévue est un champ calculé qui ne peut pas être modifié manuellement.

Les critères utilisés pour déterminer la date de fin prévue diffèrent selon l’objet que vous affichez :

* **Projets :** La date d’achèvement prévue des projets correspond à la date d’achèvement prévue de la dernière tâche du projet.

  Par exemple, un pourcentage plus élevé de fin déplace la date de fin prévue de la tâche plus près du jour en cours. Si l’état de la tâche est Nouveau et que la Date d’achèvement planifiée de la tâche est proche ou dépassée, la Date d’achèvement prévue se déplace plus loin dans le futur.

* **Tâches :** La date d’achèvement prévue des tâches est déterminée selon les critères suivants :

   * **Mises à jour de progression de la tâche par la personne désignée de la tâche :** Les mises à jour de progression incluent des modifications du pourcentage terminé et de l’état de la tâche.
   * **Date de validation :** Si la personne désignée pour la tâche spécifie une date de validation, la date de fin prévue change pour correspondre à la date de validation.

     Pour plus d’informations sur les dates de validation, consultez l’article [Présentation de la date de validation](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

   * **Prédécesseurs :** S’il n’y a aucun retard sur les tâches précédentes, la date d’achèvement prévue doit correspondre à la date d’achèvement prévue. En cas de retards, les tâches dépendantes affichent une date d’achèvement prévue supérieure à la date d’achèvement planifiée.

     Pour plus d’informations sur la date d’achèvement prévue des tâches, voir [Présentation de la date d’achèvement prévue de la tâche](../../../manage-work/tasks/task-information/task-planned-completion-date.md).

  >[!IMPORTANT]
  >
  >Lorsque le prédécesseur d’une tâche comporte une date de fin réelle, les tâches dépendantes reçoivent une date de fin prévue, comme décrit dans le scénario suivant :
  >
  >
  >Si le projet comporte les tâches A, B et C, et que la tâche B est le successeur de la tâche A, la tâche C succède à la tâche B et une date d’achèvement réelle est ajoutée à la tâche A, la date d’achèvement prévue est automatiquement recalculée pour la tâche B (à condition que le **Type de mise à jour** du projet soit défini sur Automatique et En changement), mais elle ne sera pas recalculée pour la tâche C actuellement. Date d’achèvement sélectionnée pour les tâches d’un niveau supérieur ou inférieur par rapport à la tâche mise à jour, pour des raisons de performances.

* **Problèmes :** Le problème La date d’achèvement prévue est initialement définie pour correspondre à la date d’achèvement prévu du problème.

  Si la personne désignée par le problème indique une date de validation, la date de fin prévue et la date de fin planifiée correspondent toutes deux à la date de validation.

  Pour plus d’informations sur les dates de validation, consultez l’article [Présentation de la date de validation](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

## Afficher la date d’achèvement prévue

Vous pouvez afficher la date d’achèvement prévue des projets, tâches et problèmes dans les rapports. Vous pouvez afficher la date d’achèvement prévue des projets et tâches dans d’autres zones de Workfront.

### Affichage de la date d’achèvement prévue d’un projet {#view-the-projected-completion-date-of-a-project}

1. Accédez au projet dans lequel vous souhaitez afficher la date de fin prévue.
1. Cliquez sur **Détails du projet** dans le panneau de gauche.
1. Recherchez le champ **Date d’achèvement prévue** dans la section **Aperçu** > **Dates du projet** .

### Afficher la date d’achèvement prévue d’une tâche {#view-the-projected-completion-date-of-a-task}

1. Accédez à la tâche où vous souhaitez afficher la date de fin prévue.
1. Cliquez sur **Détails de la tâche** dans le panneau de gauche.
1. Recherchez le champ **Date d’achèvement prévue** dans la section **Aperçu** > **Dates de la tâche et contrainte** .

### Afficher la date d’achèvement prévue d’un problème {#view-the-projected-completion-date-of-an-issue}

Vous pouvez afficher la date d’achèvement prévue pour les problèmes uniquement dans un rapport de problèmes ou en mode Liste. La création d’un mode Liste est similaire à la création d’un mode dans un rapport.

Pour créer un rapport de problème qui inclut la date de fin prévue :

1. Créez un rapport de problème, comme décrit dans l’article [Créer un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. Sélectionnez l’onglet **Colonnes (vue)** .
1. Cliquez sur **Ajouter la colonne** et commencez à saisir **Date d’achèvement prévue** dans le champ **Afficher dans cette colonne :** .

1. Sélectionnez-le lorsqu’il apparaît dans la liste, sous l’objet **Problème** .
1. Cliquez sur **Enregistrer + Fermer**.

   La colonne **Date d’achèvement prévue** du rapport est renseignée.

   ![](assets/issue-projected-completion-date-in-view-nwe-350x148.png)
