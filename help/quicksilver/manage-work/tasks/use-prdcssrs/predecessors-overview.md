---
content-type: overview
product-area: projects
navigation-topic: use-predecessors
title: Présentation des prédécesseurs de tâches
description: Un prédécesseur est la tâche dont une autre tâche (appelée successeur ou tâche dépendante) dépend. Adobe Workfront prend en charge cinq types de dépendances de prédécesseur.
author: Alina
feature: Work Management
exl-id: b2020a50-0921-4ed2-8a34-1a0411992b99
source-git-commit: 5db9a4869e1321bd268e80f786d157fbb41c0656
workflow-type: tm+mt
source-wordcount: '1107'
ht-degree: 0%

---

# Présentation des prédécesseurs de tâches

<!-- 

CONTEXT SENSITIVE HELP article. DO NOT CHANGE THE NAME OF THE ARTICLE/ DO NOT MOVE OR DELETE! -->

Un prédécesseur est la tâche dont une autre tâche (appelée successeur ou tâche dépendante) dépend. Adobe Workfront prend en charge cinq types de dépendances de prédécesseur. Pour comprendre les dépendances de prédécesseur, voir [Présentation des types de dépendances des tâches](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

## Présentation des prédécesseurs

Il est important de bien comprendre les fonctionnalités de prédécesseur pour connaître les calendriers de vos projets.

Les relations entre les tâches se présentent au sein d’un seul projet et entre plusieurs projets.

Dans le cas d’une dépendance multi-projet, vous pouvez établir des prédécesseurs multi-projets.

Que les tâches précédentes et successeurs appartiennent au même projet ou à deux projets différents, les dépendances et les chronologies sont calculées de la même manière.

En ce qui concerne les prédécesseurs, la chronologie du projet est affectée par les éléments suivants :

* Dépendance du prédécesseur
* Valeur de balise et type\
  Pour plus d’informations sur les dépendances et les décalages, voir [Exemples de valeurs de prédécesseur dans une liste de tâches](#examples-of-predecessor-values-in-a-task-list).

Par exemple, si la tâche A est un prédécesseur de la tâche B dans une relation de finalisation et de démarrage, et que la tâche B a une contrainte de tâche Dès que possible, Workfront attribue à la tâche B une date de début planifiée immédiatement après la date d’achèvement prévue de la tâche A, que le prédécesseur soit appliqué ou non.

Pour comprendre les relations de prédécesseur, vous devez comprendre :

* **Types de dépendances :** Les prédécesseurs sont liés par différents types de dépendances. Pour plus d’informations sur les types de dépendance, voir [Présentation des types de dépendances des tâches](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

* **Application d’un prédécesseur** Lors de l’application d’un prédécesseur, la tâche qui lui succède ne peut pas commencer tant que le prédécesseur n’est pas terminé. La tâche de remplacement s’affiche comme démarrant immédiatement une fois que le prédécesseur est terminé.

  Workfront ne permet pas de la marquer comme En cours ou Terminé tant que le prédécesseur n’est pas terminé. Workfront permet toutefois de générer des rapports sur les heures de la tâche.\
  Pour plus d’informations sur l’application des prédécesseurs, voir [Application des prédécesseurs](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

* **Balises :** Vous pouvez créer des décalages dans vos dépendances, ce qui crée un délai qui doit survenir après l’achèvement d’une tâche de prédécesseur et avant que la tâche qui lui succède puisse commencer. Les décalages ont un impact sur la chronologie du projet.

  Pour comprendre les types de décalages, voir [Présentation des types de balise](../../../manage-work/tasks/use-prdcssrs/lag-types.md).

## Créer des relations de prédécesseur

Pour créer des prédécesseurs, reportez-vous aux articles suivants :

* Pour établir des prédécesseurs à l’aide de l’onglet Prédécesseurs de la tâche, voir [Créer une relation de prédécesseur à l’aide de la zone Prédécesseurs](../../../manage-work/tasks/use-prdcssrs/create-predecessors-in-predecessors-area.md).
* Pour établir des prédécesseurs dans une liste de tâches, voir [Créer une relation de prédécesseur sur la liste des tâches](../../../manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).
* Pour établir des relations de prédécesseur en enchaînant des tâches, voir [Créer des relations de prédécesseur en attachant des tâches](../../../manage-work/tasks/use-prdcssrs/create-predecessors-by-chaining-tasks.md).
* Pour établir des prédécesseurs sur plusieurs projets, voir [Création de prédécesseurs sur plusieurs projets](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).

## Localisation des prédécesseurs d’une tâche {#locate-the-predecessors-of-a-task}

Pour trouver les prédécesseurs d&#39;une tâche, effectuez l&#39;une des opérations suivantes :

* Accédez au projet sur lequel vous travaillez et procédez comme suit :

   1. Recherchez la tâche pour laquelle vous souhaitez retrouver les prédécesseurs et cliquez sur la tâche.
   1. Cliquez sur **Prédécesseurs** dans le panneau de gauche. Vous devrez peut-être cliquer sur **Afficher plus**, puis **Prédécesseurs**.
   1. Le nom du projet sur lequel se trouve le prédécesseur s’affiche dans la variable **Projet** colonne .

      Le nombre indiqué dans la variable **#** affiche le numéro de la tâche du prédécesseur. Par exemple, &quot;6&quot; signifie la sixième tâche du projet.

      ![section Prédécesseurs de la tâche](assets/predecessors-area-with-task-header.png)

* Accédez au projet sur lequel vous travaillez et procédez comme suit :

   1. Cliquez sur le bouton **Tâche** .
   1. Choisissez la **Vue standard** en haut de la liste des tâches.
   1. La variable **Prédécesseurs** affiche les numéros des tâches du prédécesseur.

      Pour un prédécesseur multi-projet, la colonne Prédécesseurs indique le numéro de référence du projet auquel appartient le prédécesseur et le numéro de la tâche, séparés par deux points.

      L’icône du prédécesseur devient verte lorsque la tâche du prédécesseur est marquée comme terminée. Cela indique que la tâche dépendante est prête pour le travail.

      Passez la souris sur cette valeur pour obtenir plus d’informations sur le prédécesseur, le projet et les dates.

      ![Détails du prédécesseur](assets/predecessor-details-in-task-list.png)

## Exemples de valeurs de prédécesseur dans une liste de tâches {#examples-of-predecessor-values-in-a-task-list}

Lorsque vous affichez les prédécesseurs dans une liste de tâches, vous pouvez voir l’un des types de prédécesseurs suivants avec leurs types de dépendances et leurs quantités de charge respectifs :

* **1fs -** Le numéro de tâche du prédécesseur est 1. Le type de dépendance est Finish-Start. Dans la chronologie du projet, cette tâche doit commencer immédiatement une fois la tâche 1 terminée. Malgré cela, il peut toujours être marqué comme En cours ou Terminé.
* **1 -** Le numéro de tâche du prédécesseur est 1. Il s’agit de la même chose que **1fs**, car **fs** est la relation de prédécesseur par défaut dans Workfront.

* **1fse -** Le numéro de tâche du prédécesseur est 1. Le type de dépendance est Finish-Start-Enforced. Dans la chronologie du projet, cette tâche s’affiche comme démarrant immédiatement une fois la tâche 1 terminée. Workfront ne permet pas de la marquer comme En cours ou Terminé tant que la tâche 1 n’est pas terminée. Workfront permet toutefois de générer des rapports sur les heures de la tâche.
* **1fs+3d -** Le numéro de tâche du prédécesseur est 1. Le type de dépendance est Terminer-Démarrer avec un délai de 3 jours. Dans la chronologie du projet, cette tâche se présente comme commençant 3 jours ouvrés après la fin de la tâche 1.
* **1fs-3d -** Le numéro de tâche du prédécesseur est 1. Le type de dépendance est Terminer-Démarrer avec un délai de 3 jours. Dans la chronologie du projet, cette tâche commence 3 jours ouvrés avant que la tâche du prédécesseur ne soit terminée.
* **1fs+3de** -Le numéro de la tâche du prédécesseur est 1. Le type de dépendance est Finish-Start-Enforced avec un délai de 3 jours. Dans la chronologie du projet, cette tâche se présente comme commençant 3 jours ouvrés après la fin de la tâche 1. Workfront ne permet pas qu’elle soit marquée comme En cours ou Terminée tant que la tâche 1 n’est pas terminée. Workfront permet toutefois de générer des rapports sur les heures de la tâche.

  >[!NOTE]
  >
  >La valeur appliquée (**e**) doit être ajouté au journal, et non au prédécesseur.

* **4515:2** Le numéro de tâche du prédécesseur est 2. - Il s’agit d’une dépendance Terminer au début non appliquée avec le prédécesseur du projet avec le numéro de référence. **4515**.

## Afficher les informations du prédécesseur

Vous pouvez afficher les informations du prédécesseur dans les zones suivantes de Workfront. Cela inclut des informations sur les prédécesseurs sur plusieurs projets :

* Au niveau de la tâche, dans la section Prédécesseurs .

  Pour plus d’informations sur l’affichage des informations de prédécesseur dans la section Prédécesseurs , voir la section . [Localisation des prédécesseurs d’une tâche](#locate-the-predecessors-of-a-task) dans cet article.

* Dans le diagramme de Gantt.

  Pour plus d’informations sur l’affichage des prédécesseurs dans le diagramme de Gantt, voir [Configuration de l’affichage des informations sur le diagramme de Gantt](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

* Dans une liste de tâches.

  Pour afficher des informations sur les prédécesseurs de vos tâches dans une liste de tâches, vous pouvez effectuer l’une des opérations suivantes :

   * Appliquez la vue standard intégrée dans une liste de tâches.

     Pour plus d’informations sur l’affichage des informations de prédécesseur dans la vue Standard, voir la section [Localisation des prédécesseurs d’une tâche](#locate-the-predecessors-of-a-task) dans cet article.

   * Créez une vue de tâche ou un rapport et ajoutez la colonne Prédécesseurs à cette vue.

     Pour plus d’informations sur la création d’une vue personnalisée pour les tâches avec les informations de prédécesseur, voir [Afficher : détails du prédécesseur](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-predecessor-details.md).

* Dans l’en-tête de la tâche lors de l’accès à la tâche.

  ![](assets/qs-predecessor-info-in-task-header-350x141.png)
