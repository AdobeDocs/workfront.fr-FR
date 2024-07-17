---
content-type: overview
product-area: agile-and-teams
navigation-topic: scrum-board
title: Vue d’ensemble du panorama Scrum
description: Le panorama d’anecdotes agiles de Scrum s’affiche avec l’état d’achèvement et le graphique de condensation.
author: Lisa
feature: Agile
exl-id: 584288bb-2d98-4b69-8deb-d3b8e54d328c
source-git-commit: 6f817ca39c7489b85673ff601faf440fe51ab72c
workflow-type: tm+mt
source-wordcount: '878'
ht-degree: 0%

---

# Présentation du panorama [!UICONTROL Scrum]

Le panorama d’articles agiles [!UICONTROL Scrum] s’affiche avec l’état de fin et le graphique de condensation. Ces composants agiles sont disponibles dans les situations suivantes dans [!UICONTROL Adobe Workfront] :

* Lors des itérations agiles. Pour plus d’informations sur l’utilisation du tableau de bord agile, du tableau de bord et de l’état d’achèvement dans un environnement agile pur (avec des retards et une itération), voir [Travail dans un environnement agile](../../../agile/work-in-an-agile-environment/work-in-an-agile-environment.md).
* Lorsque vous affichez un projet dans une vue agile. Pour plus d’informations sur la manière d’exploiter le tableau d’articles agile, le tableau de bord et l’état d’achèvement dans un projet existant, voir [Gestion d’un projet dans la vue agile](../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md).

![itération agile](assets/agile-iteration-with-callouts.png)

## Disposition et fonctions d’un panorama d’articles

![Agile story board](assets/agile-storyboard-callouts.png)

Le tableau de bord se compose des éléments suivants :

* **[!UICONTROL Colonne Parent Story] :** Contrairement aux autres colonnes du tableau de bord, la colonne [!UICONTROL Parent Story] n’est pas un état de tâche, mais elle existe plutôt pour héberger les articles qui contiennent des sous-tâches dans l’itération ou le projet. Seules les histoires parentes qui comportent au moins une sous-tâche sur le panorama des articles peuvent résider dans cette colonne. Les histoires parentes elles-mêmes ne passent pas d’un statut à un statut dans l’ensemble du tableau.

  Dans une itération, cette colonne apparaît sur le panorama uniquement lorsqu’un ou plusieurs articles du panorama contiennent au moins une sous-tâche qui répond aux exigences suivantes :

   * Affecté à la même équipe agile que la tâche parent
   * appartient à l’itération.

     Dans un projet, cette colonne s’affiche chaque fois qu’une tâche comporte au moins une sous-tâche.

     ![Colonne d’histoire parente](assets/agile-parentstory-swimlane.png)

* **États de la tâche :** Indique la progression d’un article dans l’itération ou le projet en fonction de la colonne d’état dans laquelle se trouve l’article.

  Les états de tâche peuvent être personnalisés pour le projet en modifiant la vue agile, comme décrit dans la section [Créer ou personnaliser une vue agile](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-an-agile-view) dans la [vue d&#39;ensemble des vues dans [!UICONTROL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

* **Swim Lane :** Lorsqu’un article parent et ses sous-tâches apparaissent sur le panorama des histoires, une piste de nage est créée spécifiquement pour l’histoire et ses sous-tâches. Cela fournit une distinction visuelle pour mieux voir comment les sous-tâches d’une histoire progressent dans tout le contenu de l’histoire.

  Dans une itération, les pistes de nage apparaissent sur le panorama uniquement lorsqu’un article sur le panorama contient au moins une sous-tâche qui répond aux exigences suivantes :

   * Affecté à la même équipe agile que la tâche parent
   * appartient à l’itération.

  Dans un projet, les voies de navigation apparaissent chaque fois qu’une tâche comporte au moins une sous-tâche ou une tâche parent.

* **Histoires individuelles :** Des histoires et des problèmes individuels s’affichent sous n’importe quelle piste de nage sur le panorama des histoires. Cela permet de distinguer visuellement les histoires qui font partie d&#39;une piste de nage.

## Relation entre les sous-tâches et les articles

Si un article contient des sous-tâches, vous ne pouvez pas mettre à jour les informations sur l’article parent lui-même (comme les points/heures ou le pourcentage de fin). De plus, vous ne pouvez pas déplacer l&#39;histoire d&#39;un bout à l&#39;autre pour mettre à jour son statut. Au contraire, tout changement que vous apportez aux sous-tâches de l&#39;histoire est reflété dans l&#39;histoire. Les points ou heures d’article combinés pour toutes les sous-tâches déterminent les points ou les heures de l’article parent.

Par exemple, si une histoire ne comporte qu’une seule sous-tâche évaluée à 4 points, l’histoire elle-même comporte également 4 points. Si vous définissez la valeur du point de sous-tâche sur 3, la valeur du point de l’article parent est remplacée par 3. Si vous créez une autre sous-tâche sur le même article et que vous définissez la valeur de point de cette sous-tâche sur 4, la valeur de point de l’article est changée sur 7 afin de refléter la valeur de point combinée pour les deux sous-tâches.

Cette même logique s’applique aux sous-tâches de second niveau (sous-tâches de sous-tâches). Si une sous-tâche comporte une ou plusieurs sous-tâches de second niveau, la sous-tâche est calculée en fonction des sous-tâches de second niveau.

## Relation entre le panorama des articles et le journal

>[!NOTE]
>
>Les informations de cette section s’appliquent uniquement aux vues agiles sur une itération ; les vues agiles sur un projet n’utilisent pas de journal en souffrance. (Pour plus d’informations sur les différences entre les vues agiles d’une itération et d’un projet, voir &quot;Différences lors de l’utilisation de la vue [!UICONTROL Agile] sur un projet en itération&quot; dans [Gestion d’un projet en mode agile](../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md).)

Le journal des itérations affiche uniquement les articles ou les sous-tâches pour lesquels vous pouvez définir une estimation. Si un article parent comporte des sous-tâches qui s’affichent sur le panorama des articles (car elles sont affectées à la même équipe agile et font partie de l’itération), la tâche parent n’est pas affichée dans le journal. Dans ce cas, seules les sous-tâches sont affichées sur le journal, tandis que les sous-tâches et l’article parent sont affichés sur le panorama des articles.

Supposons, par exemple, que l’article A contienne la sous-tâche 1 et la sous-tâche 2 (et que les deux sous-tâches soient assignées à la même équipe agile). Dans ce cas, l’article A s’affiche sur le tableau de bord d’une piste de nage avec les sous-tâches 1 et 2. Toutefois, seules les sous-tâches 1 et la sous-tâche 2 sont affichées dans le journal.

Cette même logique s’applique aux sous-tâches de second niveau (sous-tâches de sous-tâches). Si une sous-tâche comporte une ou plusieurs sous-tâches de deuxième niveau affectées à la même équipe agile et qu’elles appartiennent à l’itération, seule la sous-tâche de deuxième niveau s’affiche dans le journal des tâches en souffrance.

Pour plus d’informations sur le journal des travaux, voir [Gestion du journal des travaux agiles](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).
