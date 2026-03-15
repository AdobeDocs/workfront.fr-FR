---
content-type: overview
product-area: agile-and-teams
navigation-topic: scrum-board
title: Présentation du tableau de mêlée
description: Le scénarimage Scrum Agile s’affiche avec l’état d’achèvement et le graphique de gravure.
author: Courtney
feature: Agile
exl-id: 584288bb-2d98-4b69-8deb-d3b8e54d328c
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '803'
ht-degree: 51%

---

# Vue d’ensemble du panorama [!UICONTROL Scrum]

<!-- Audited: 5/2025 -->

Le scénarimage Agile [!UICONTROL Scrum] s&#39;affiche avec l&#39;état d&#39;achèvement et le graphique d&#39;obscurcissement. Ces composants Agile sont disponibles dans les situations suivantes dans [!UICONTROL Adobe Workfront] :

* Sur les itérations Agile. Pour plus de détails sur l&#39;utilisation du scénarimage Agile, du graphique d&#39;analyse et de l&#39;état d&#39;achèvement dans un environnement Agile pur (avec des retards et une itération), consultez [Travailler dans un environnement Agile](../../../agile/work-in-an-agile-environment/work-in-an-agile-environment.md).
* Lors de l’affichage d’un projet dans une vue Agile. Pour plus d&#39;informations sur la façon dont vous pouvez tirer parti du scénarimage Agile, du graphique d&#39;analyse et de l&#39;état d&#39;achèvement dans un projet existant, voir [Gérer un projet dans la vue Agile](../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md).

![Itération Agile](assets/agile-iteration-with-callouts.png)

## Disposition et fonctions d’un storyboard

![Storyboard Agile](assets/agile-storyboard-callouts.png)

Le storyboard se compose des éléments suivants :

* **Colonne parent** : contrairement aux autres colonnes du scénarimage, la colonne [!UICONTROL Parent] n’est pas un état de tâche, mais elle existe pour héberger tous les articles contenant des tâches subordonnées dans l’itération ou le projet. Cette colonne est uniquement réservée aux histoires parent comportant au moins une sous-tâche représentée sur le storyboard. Les histoires parent elles-mêmes ne passent pas d’un statut à l’autre dans le storyboard.

  Cette colonne est visible sur le storyboard durant une itération uniquement si une ou plusieurs histoires intègrent au moins une sous-tâche qui répond aux exigences suivantes :

   * Affecté à la même équipe Agile que la tâche parent.
   * Appartient à l&#39;itération.

     Cette colonne est affichée dans un projet chaque fois qu’une tâche contient une ou plusieurs sous-tâches.

     ![Colonne d’histoire parent](assets/agile-parentstory-swimlane.png)

* **États des tâches** : indiquent la progression d’un article dans l’itération ou le projet en fonction de la colonne d’état dans laquelle se trouve l’article.

  Les statuts de tâche peuvent être personnalisés pour le projet en modifiant la vue Agile.

* **Voie de baignade** : lorsqu’un article parent et ses tâches subordonnées apparaissent sur le scénarimage, une voie de baignade est créée spécifiquement pour l’article et ses tâches subordonnées. Cette méthode permet de distinguer visuellement et de suivre plus aisément la progression des sous-tâches à travers le contenu global du storyboard.

  Au cours d’une itération, les couloirs (swim lanes) sur le storyboard apparaissent seulement si une histoire contient au moins une sous-tâche qui satisfait aux exigences suivantes :

   * Affecté à la même équipe Agile que la tâche parent.
   * Appartient à l&#39;itération.

  Dans un projet, les couloirs apparaissent chaque fois qu’une tâche comporte au moins une sous-tâche ou une tâche parent.

* **Histoires individuelles** : les histoires et les problèmes individuels sont affichés sous les couloirs de natation du scénarimage. Il est ainsi facile de distinguer visuellement les histoires qui font partie d’un couloir.

## Relation entre les sous-tâches et les histoires

Si un article contient des tâches subordonnées, vous ne pouvez pas mettre à jour les informations sur l’article parent lui-même (telles que les points/heures ou le pourcentage achevé). En outre, vous ne pouvez pas déplacer l’article dans l’ensemble du scénarimage pour mettre à jour son statut. Au contraire, tout changement que vous apportez aux sous-tâches de l’histoire est reflété dans l’histoire. Les points ou les heures de l’histoire combinés pour toutes les sous-tâches déterminent les points ou les heures de l’histoire parent.

Par exemple, si une histoire ne comporte qu’une seule sous-tâche évaluée à 4 points, l’histoire elle-même comporte également 4 points. Si vous remplacez la valeur du point de sous-tâche sur 3, la valeur du point de l’histoire parent est aussi remplacée par 3. Si vous créez une autre sous-tâche sur la même histoire et que vous définissez la valeur du point de cette sous-tâche sur 4, la valeur du point de l’histoire est remplacée par 7 afin de refléter la valeur de point combinée pour les deux sous-tâches.

Cette même logique s’applique aux sous-tâches de deuxième niveau (sous-tâches de sous-tâches). Si une sous-tâche comporte une ou plusieurs sous-tâches de deuxième niveau, elle est calculée en fonction des sous-tâches de deuxième niveau.

## Relation entre le storyboard et la liste d’attente

La liste d’attente des itérations affiche uniquement les histoires ou les sous-tâches pour lesquelles vous pouvez définir une estimation. Si un article parent comporte des sous-tâches qui s&#39;affichent sur le scénarimage (car elles sont affectées à la même équipe agile et appartiennent à l&#39;itération), la tâche parent ne s&#39;affiche pas dans le journal des travaux en souffrance. Dans ce cas, seules les sous-tâches sont affichées dans la liste d’attente, tandis que les sous-tâches et l’histoire parent sont affichées sur le storyboard.

Par exemple, supposons que l’article A contienne la tâche secondaire 1 et la tâche secondaire 2 (et que les deux tâches secondaires soient affectées à la même équipe agile). Dans ce cas, l’histoire A s’affiche dans un couloir sur le storyboard avec les sous-tâches 1 et 2. Toutefois, seules les sous-tâches 1 et 2 sont affichées dans la liste d’attente.

Cette même logique s’applique aux sous-tâches de deuxième niveau (sous-tâches de sous-tâches). Si une tâche secondaire comporte une ou plusieurs tâches secondaires affectées à la même équipe mobile et appartenant à l&#39;itération, seule la tâche secondaire de deuxième niveau est affichée dans le journal des travaux en souffrance.

Pour plus d&#39;informations sur le portefeuille de commandes, voir [Gérer le portefeuille de commandes Agile](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).
