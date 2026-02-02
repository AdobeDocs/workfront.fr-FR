---
content-type: overview
product-area: projects
navigation-topic: use-predecessors
title: Présentation des tâches antérieures
description: Une tâche antérieure est celle dont dépend une autre tâche (appelée tâche ultérieure ou dépendante). Adobe Workfront prend en charge cinq types de dépendance de tâches antérieures.
author: Alina
feature: Work Management
exl-id: b2020a50-0921-4ed2-8a34-1a0411992b99
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '1184'
ht-degree: 98%

---

# Vue d’ensemble des tâches antérieures

<!--Audited: 12/2023-->

<!-- 

CONTEXT SENSITIVE HELP article. DO NOT CHANGE THE NAME OF THE ARTICLE/ DO NOT MOVE OR DELETE! -->

Une tâche antérieure est celle dont dépend une autre tâche (appelée tâche ultérieure ou dépendante). Adobe Workfront prend en charge cinq types de dépendance de tâches antérieures. Pour comprendre les dépendances de tâche antérieure, voir [Vue d’ensemble des types de dépendance de tâches](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

## Vue d‘ensemble des tâches antérieures

Il est important de bien comprendre les fonctionnalités des tâches antérieures pour comprendre la chronologie de vos projets.

Les relations avec les tâches antérieures existent à la fois entre les tâches d’un seul projet et entre les tâches de différents projets.

Dans le cas d’une dépendance multiprojet, vous pouvez établir des tâches antérieures inter-projets entre les tâches de deux projets différents.

Que les tâches antérieures et ultérieures appartiennent au même projet ou à deux projets différents, les dépendances et la chronologie de chaque projet sont calculées de la même manière.

En ce qui concerne les tâches antérieures, la chronologie du projet est affectée par les éléments suivants :

* Dépendance à la tâche antérieure
* Valeur et type du décalage\
  Pour plus d’informations sur les dépendances et les décalages, voir [Exemples de valeurs de tâche antérieure dans une liste de tâches](#examples-of-predecessor-values-in-a-task-list).

  Par exemple, si la tâche A est antérieure à la tâche B dans une relation de finalisation et de démarrage, et que la tâche B a une contrainte de tâche Aussi tôt que possible, Workfront attribue à la tâche B une date de début prévue immédiatement après la date d’achèvement prévue de la tâche A, que la tâche antérieure soit appliquée ou non.

Pour comprendre les relations d’antériorité, vous devez comprendre :

* **Types de dépendance :** les tâches antérieures sont liées par différents types de dépendance. Pour plus d’informations sur les types de dépendance, voir [Vue d’ensemble des types de dépendance des tâches](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

* **Application d’une tâche antérieure :** lors de l’application d’une tâche antérieure, la tâche ultérieure ne peut absolument pas démarrer tant que la tâche antérieure n’est pas terminée. La tâche ultérieure s’affiche comme démarrant immédiatement une fois que la tâche antérieure est terminée.

  Lorsque la tâche antérieure n’est pas terminée (ou démarrée) et qu’elle n’est pas appliquée, la tâche ultérieure peut démarrer, mais la chronologie du projet est toujours affectée par les dates des tâches antérieure et ultérieure.

  Avec une tâche antérieure appliquée, Workfront ne permet pas que la tâche ultérieure soit marquée comme En cours ou Terminée tant que la tâche antérieure n’est pas terminée.

  Workfront permet toutefois de générer des rapports sur les heures de la tâche.\
  Pour plus d’informations sur l’application des tâches antérieures, voir [Appliquer les tâches antérieures](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

* **Décalage :** vous pouvez créer des décalages dans vos dépendances, ce qui crée un retard qui doit survenir après l’achèvement d’une tâche antérieure et avant que la tâche ultérieure puisse commencer. Les décalages ont un impact sur la chronologie du projet.

  Pour comprendre les types de décalage, voir [Vue d’ensemble des types de décalage](../../../manage-work/tasks/use-prdcssrs/lag-types.md).

## Créer des relations d’antériorité

Pour créer des tâches antérieures, reportez-vous aux articles suivants :

* Pour établir des tâches antérieures à l’aide de l’onglet Tâches antérieures de la tâche, voir [Créer une relation d’antériorité à l’aide de la zone Tâches antérieures](../../../manage-work/tasks/use-prdcssrs/create-predecessors-in-predecessors-area.md).
* Pour établir des tâches antérieures dans une liste de tâches, voir [Créer une relation d’antériorité sur la liste des tâches](../../../manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).
* Pour établir des relations d’antériorité en chaînant des tâches, voir [Créer des relations d’antériorité en chaînant les tâches](../../../manage-work/tasks/use-prdcssrs/create-predecessors-by-chaining-tasks.md).
* Pour établir des tâches antérieures inter-projets, voir [Créer des tâches antérieures inter-projets](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).

## Localiser les tâches antérieures d’une tâche {#locate-the-predecessors-of-a-task}

Pour trouver les tâches antérieures d’une tâche, effectuez l’une des opérations suivantes :

* Accédez au projet sur lequel vous travaillez et procédez comme suit :

   1. Recherchez la tâche pour laquelle vous souhaitez retrouver les tâches antérieures et cliquez sur la tâche.
   1. Cliquez sur **Tâches antérieures** dans le panneau de gauche.
   1. Le nom du projet sur lequel se trouve la tâche antérieure s’affiche dans la colonne **Projet**.

      Le nombre indiqué dans la colonne **#** affiche le numéro de la tâche antérieure. Par exemple, « 6 » signifie la sixième tâche du projet.

      ![Section Tâches antérieures de la tâche](assets/predecessors-area-with-task-header.png)

* Accédez au projet sur lequel vous travaillez et procédez comme suit :

   1. Cliquez sur l’onglet **Tâche**.
   1. Choisissez la **Vue standard** en haut de la liste des tâches.
   1. La colonne **Tâches antérieures** affiche les numéros des tâches antérieures.

      Pour une tâche antérieure inter-projet, la colonne Tâches antérieures indique le numéro de référence du projet auquel appartient la tâche antérieure et le numéro de la tâche, séparés par deux points.

      L’icône de la tâche antérieure devient verte lorsque la tâche antérieure est marquée comme terminée. Cela indique que la tâche dépendante est prête à être exécutée.

      Pointez sur cette valeur pour obtenir plus d’informations sur la tâche antérieure, le projet et les dates.

      ![Détails de la tâche antérieure](assets/predecessor-details-in-task-list.png)

## Exemples de valeurs de tâche antérieure dans une liste de tâches {#examples-of-predecessor-values-in-a-task-list}

Lorsque vous affichez les tâches antérieures dans une liste de tâches, vous pouvez voir l’un des types de tâches antérieures suivants avec leurs types de dépendances et leurs décalages respectifs :

* **1fs -** Le numéro de la tâche antérieure est 1. Le type de dépendance est Terminer-Démarrer. Dans la chronologie du projet, cette tâche doit commencer immédiatement après l’achèvement de la tâche 1. Malgré cela, elle peut toujours être marquée comme En cours ou Terminée.
* **1 -** Le numéro de la tâche antérieure est 1. Il s’agit de la même chose que **1fs**, car **fs** est la relation de tâche antérieure par défaut dans Workfront.

* **1fse -** Le numéro de la tâche antérieure est 1. Le type de dépendance est Terminer-Démarrer-Forcé. Dans la chronologie du projet, cette tâche s’affiche comme démarrant immédiatement après l’achèvement de la tâche 1. Workfront ne permet pas de la marquer comme En cours ou Terminée tant que la tâche 1 n’est pas terminée. Workfront permet toutefois de générer des rapports sur les heures de la tâche.
* **1fs+3d -** Le numéro de la tâche antérieure est 1. Le type de dépendance est Terminer-Démarrer avec un décalage de 3 jours. Dans la chronologie du projet, cette tâche se présente comme commençant 3 jours ouvrés après l’achèvement de la tâche 1.
* **1fs-3d -** Le numéro de la tâche antérieure est 1. Le type de dépendance est Terminer-Démarrer avec un décalage de 3 jours. Dans la chronologie du projet, cette tâche commence 3 jours ouvrés avant l’achèvement de la tâche antérieure.
* **1fs+3de** - Le numéro de la tâche antérieure est 1. Le type de dépendance est Terminer-Démarrer-Forcé avec un décalage de 3 jours. Dans la chronologie du projet, cette tâche se présente comme commençant 3 jours ouvrés après l’achèvement de la tâche 1. Workfront ne permet pas de la marquer comme En cours ou Terminée tant que la tâche 1 n’est pas terminée. Workfront permet toutefois de générer des rapports sur les heures de la tâche.

  >[!NOTE]
  >
  >Vous devez ajouter la valeur appliquée (**e**) au décalage, et non à la tâche antérieure.

* **4515:2** Le numéro de la tâche antérieure est 2. - Il s’agit d’une dépendance Terminer-Démarrer non forcée avec la tâche antérieure du projet portant le numéro de référence **4515**.

## Afficher les informations sur la tâche antérieure

Vous pouvez afficher les informations sur la tâche antérieure dans les zones suivantes de Workfront. Cela inclut des informations sur les projets transversaux antérieurs :

* Au niveau de la tâche, dans la section Tâches antérieures.

  Pour plus d’informations sur l’affichage des informations sur les tâches antérieures dans la section Tâches antérieures, voir la section [Localiser les tâches antérieures d’une tâche](#locate-the-predecessors-of-a-task) dans cet article.

* Dans le graphique de Gantt.

  Pour plus d’informations sur l’affichage des tâches antérieures dans le graphique de Gantt, voir [Configurer l’affichage des informations sur le graphique de Gantt](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

* Dans une liste de tâches.

  Pour afficher des informations sur les tâches antérieures dans une liste de tâches, vous pouvez effectuer l’une des opérations suivantes :

   * Appliquez la vue Standard intégrée dans une liste de tâches.

     Pour plus d’informations sur l’affichage des informations sur les tâches antérieures dans la vue Standard, voir la section [Localiser les tâches antérieures d’une tâche](#locate-the-predecessors-of-a-task) dans cet article.

   * Créez une vue de tâche ou un rapport et ajoutez la colonne Tâches antérieures à cette vue.

     Pour plus d’informations sur la création d’une vue personnalisée pour les tâches avec les informations sur les tâches antérieures, voir [Afficher : détails de la tâche antérieure](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-predecessor-details.md).

* Dans l’en-tête de la tâche lors de l’accès à la tâche.

  ![Informations sur le prédécesseur dans l’en-tête de la tâche](assets/qs-predecessor-info-in-task-header-350x141.png)
