---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Vue d’ensemble de la date d’achèvement prévue pour les projets, les tâches et les problèmes
description: La date d’achèvement prévisionnelle est un indicateur calculé en temps réel de la date d’achèvement du projet, de la tâche ou du problème. Lorsque le projet, la tâche ou le problème est marqué comme terminé, la date d’achèvement prévisionnelle devient la date d’achèvement effective.
author: Alina
feature: Work Management
exl-id: dde400e6-189f-4431-8f2f-7142ce424826
source-git-commit: 811d8076a0b344e863b25aa253a0fb1c102f0435
workflow-type: tm+mt
source-wordcount: '873'
ht-degree: 73%

---

# Vue d’ensemble de la date d’achèvement prévue pour les projets, les tâches et les problèmes

<!-- Audited: 1/2024 -->

La date d’achèvement prévisionnelle est un indicateur calculé en temps réel de la date d’achèvement du projet, de la tâche ou du problème. Lorsque le projet, la tâche ou le problème est marqué comme terminé, la date d’achèvement prévisionnelle devient la date d’achèvement effective.

Les sections suivantes décrivent comment la date d’achèvement prévue est déterminée pour les projets, les tâches et les problèmes, et comment la localiser.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.


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
   <p>Nouveau : 
   <ul><li><p>Contributeur ou contributrice ou supérieur pour afficher la date d’achèvement prévisionnelle dans un rapport</p></li> <li><p>Une licence standard pour créer un rapport</p></li> </ul>

<p>Actuel : 
   <ul><li><p>Révision ou supérieur pour afficher la date d’achèvement prévisionnelle dans un rapport</p></li> 
   <li><p>Une licence de plan pour créer un rapport</p> </li></ul>
      </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Niveau d’accès</td> 
   <td> <p>Accès en affichage ou supérieur aux projets</p> <p>Pour créer un rapport, vous devez disposer d’un accès en modification aux rapports, tableaux de bord et calendriers.</p> <p>Pour créer un rapport ou modifier une vue de liste, vous devez disposer d’un accès en modification aux filtres, aux vues et aux regroupements.</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations d’affichage ou de niveau supérieur sur un projet</p> </td> 
  </tr> 
 </tbody> 
</table>

* Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Comment Adobe Workfront détermine-t-il la date d’achèvement prévisionnelle ?

La date d’achèvement prévisionnelle est un champ calculé et ne peut pas être modifié manuellement.

Les critères utilisés pour déterminer la date de fin prévue diffèrent selon l’objet que vous affichez :

* **Projets :** la date d’achèvement prévisionnelle pour les projets correspond à la date d’achèvement prévisionnelle de la dernière tâche du projet.

  Par exemple, un pourcentage terminé plus élevé rapproche la date d’achèvement prévisionnelle de la tâche de la journée actuelle. Si le statut de la tâche est nouveau et que la date d’achèvement prévue de la tâche est proche ou dépassée, la date d’achèvement prévisionnelle s’éloigne dans le futur.

* **Tâches :** la date d’achèvement prévisionnelle pour les tâches est déterminée sur la base des critères suivants :

   * **Mises à jour de progression de la tâche par la personne désignée de la tâche :** Les mises à jour de progression incluent des modifications du pourcentage terminé et de l’état de la tâche.
   * **Date d’engagement :** si la personne cessionnaire de la tâche spécifie une date d’engagement, la date d’achèvement prévisionnelle est modifiée pour correspondre à la date d’engagement.

     Pour plus d’informations sur les dates de validation, consultez l’article [Présentation de la date de validation](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

   * **Prédécesseurs :** S’il n’y a aucun retard sur les tâches précédentes, la date d’achèvement prévue doit correspondre à la date d’achèvement prévue. Au fur et à mesure des retards, les tâches dépendantes affichent une date d’achèvement prévisionnelle de plus en plus ultérieure à la date d’achèvement prévue.

     Pour plus d’informations sur la date d’achèvement prévue des tâches, voir [Vue d’ensemble de date d’achèvement prévue de la tâche](../../../manage-work/tasks/task-information/task-planned-completion-date.md).

  >[!IMPORTANT]
  >
  >Lorsque le prédécesseur d’une tâche a une date d’achèvement effective, les tâches dépendantes reçoivent une date d’achèvement prévisionnelle comme décrit dans le scénario suivant :
  >
  >
  >Si le projet comporte les tâches A, B et C, et que la tâche B est le successeur de la tâche A, la tâche C succède à la tâche B et une date d’achèvement réelle est ajoutée à la tâche A, la date d’achèvement prévue est automatiquement recalculée pour la tâche B (à condition que le **Type de mise à jour** du projet soit défini sur Automatique et En changement), mais elle ne sera pas recalculée pour la tâche C actuellement. Date d’achèvement sélectionnée pour les tâches d’un niveau supérieur ou inférieur par rapport à la tâche mise à jour, pour des raisons de performances.

* **Problèmes :** la date d’achèvement prévisionnelle du problème est initialement définie pour correspondre à la date d’achèvement prévue du problème.

  Si la personne cessionnaire du problème spécifie une date d’engagement, la date d’achèvement prévisionnelle et la date d’achèvement prévue sont modifiées pour correspondre à la date d’engagement.

  Pour plus d’informations sur les dates d’engagement, voir l’article [Vue d’ensemble de la date d’engagement](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

## Afficher la date d’achèvement prévisionnelle

Vous pouvez afficher la date d’achèvement prévisionnelle des projets, des tâches et des problèmes dans les rapports. Vous pouvez consulter la date d’achèvement prévisionnelle des projets et des tâches dans d’autres zones de Workfront.

### Affichage de la date d’achèvement prévue d’un projet {#view-the-projected-completion-date-of-a-project}

1. Accédez au projet pour lequel vous souhaitez consulter la date d’achèvement prévisionnelle.
1. Cliquez sur **Détails du projet** dans le panneau de gauche.
1. Localisez le champ **Date d’achèvement prévisionnelle** dans la section **Vue d’ensemble** > **Dates du projet**.

### Afficher la date d’achèvement prévue d’une tâche {#view-the-projected-completion-date-of-a-task}

1. Accédez à la tâche pour laquelle vous souhaitez afficher la date d’achèvement prévisionnelle.
1. Cliquez sur **Détails de la tâche** dans le panneau de gauche.
1. Localisez le champ **Date d’achèvement prévisionnelle** dans la section **Vue d’ensemble** > **Dates et contrainte de tâche**.

### Afficher la date d’achèvement prévue d’un problème {#view-the-projected-completion-date-of-an-issue}

Vous pouvez afficher la date d’achèvement prévisionnelle pour les problèmes uniquement dans un rapport de problème ou une vue de liste. La création d’une vue de liste est similaire à celle d’une vue dans un rapport.

Pour créer un rapport de problème qui inclut la date d’achèvement prévisionnelle :

1. Créez un rapport de problème, comme décrit dans l’article [Créer un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. Sélectionnez l’onglet **Colonnes (Vue)**.
1. Cliquez sur **Ajouter une colonne**, et commencez à saisir la **Date d’achèvement prévisionnelle** dans le champ **Afficher dans cette colonne :**.

1. Sélectionnez-le lorsqu’il apparaît dans la liste, sous l’objet **Problème** .
1. Cliquez sur **Enregistrer + Fermer**.

   La colonne **Date d’achèvement prévue** du rapport est renseignée.

   ![](assets/issue-projected-completion-date-in-view-nwe-350x148.png)
