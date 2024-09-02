---
title: Afficher la visualisation de capacité des ressources dans Analytique améliorée
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: Vous pouvez évaluer si la charge de travail d’une équipe est trop importante, déficitaire ou égale à la capacité à l’aide de la visualisation de capacité des ressources d’Analytique améliorée dans Adobe Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: 5bb45ef6-9e49-4063-8e53-c9f3bc994870
source-git-commit: d9a8af627c8d3da4a7625cd5180bfca69da43b3d
workflow-type: ht
source-wordcount: '844'
ht-degree: 100%

---

# Afficher la visualisation de capacité des ressources dans Analytique améliorée

<!--Audited: 01/2024-->

Vous pouvez évaluer si la charge de travail d’une équipe est trop importante, déficitaire ou égale à la capacité à l’aide de la visualisation de capacité des ressources d’Analytique améliorée dans Adobe Workfront.

Les équipes illustrées dans la visualisation des ressources font référence à l’équipe interne des utilisateurs et utilisatrices affectés au travail pendant la période spécifiée.

## Conditions d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Plan Adobe Workfront</a>*</td> 
   <td> <p>Actuel : Entreprises ou supérieur</p>
   Ou
   <p>Nouveau : Tous</p>
    </td> 
  </tr> 
  <tr> 
   <td>Licence Adobe Workfront*</td> 
   <td> <p>Actuel : Révision ou supérieur</p>
   Ou
   <p>Nouveau : Standard</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuration du niveau d’accès</td> 
   <td> <p>Afficher l’accès aux projets</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisation d’affichage sur un projet</p>  </td> 
  </tr> 
 </tbody> 
</table>

* Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront. Pour plus d’informations, consultez la section [Conditions d’accès requises dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Conditions préalables

Pour connaître les conditions préalables à l’utilisation d’Analytique améliorée, consultez la section dédiée dans la [Vue d’ensemble d’Analytique améliorée](../enhanced-analytics/enhanced-analytics-overview.md).

## Présentation de la visualisation de capacité des ressources

La visualisation de capacité des ressources indique si la charge de travail d’une équipe est trop importante, déficitaire ou égale à la capacité. Ce calcul est basé sur les éléments suivants :

* **Capacité disponible** : il s’agit du nombre total d’heures pendant lesquelles une équipe interne peut travailler pendant la période spécifiée.

  >[!NOTE]
  >
  >Si vous spécifiez une période future, la capacité disponible est calculée en fonction de la capacité de l’équipe au cours des 7 derniers jours. Pour cette raison, aucun congé personnel planifié n’est pris en compte.

* **Capacité prévue** : il s’agit du nombre total d’heures de travail prévues de la part de l’équipe interne au cours de la période spécifiée.

Cette comparaison des heures prévues et des heures réellement planifiées d’une équipe interne peut vous aider à déterminer si vous n’affectez pas suffisamment de travail à l’équipe interne ou si elle subit un épuisement dû à une charge de travail importante.

![](assets/resource-capacity-350x110.png)

La visualisation de capacité des ressources affiche les informations suivantes :

* **Capacité prévue** : en regard du nom d’une équipe interne, le cercle bleu représente le nombre d’heures prévues affectées à l’équipe interne.

  ![](assets/resource-capacity-blue-circle.png)

* **Capacité réelle** : en regard du nom d’une équipe interne, la ligne verticale représente le nombre d’heures disponibles pour l’équipe interne.

  ![](assets/resource-capacity-vertical-line.png)

* **Sur-capacité** : lorsque la ligne horizontale et le cercle bleu s’affichent à droite de la ligne verticale, l’équipe interne se voit attribuer plus de travail qu’elle ne peut en accomplir durant le nombre d’heures disponibles. Cela peut indiquer que l’équipe connaît une charge de travail trop importante pendant la période spécifiée. Le nombre d’heures restantes que l’équipe doit travailler pour terminer le travail s’affiche à droite du cercle bleu.

  ![](assets/resource-capacity-over-capacity.png)

* **Inférieur à la capacité** : lorsque la ligne horizontale et le cercle bleu s’affichent à gauche de la ligne verticale, l’équipe interne dispose de plus d’heures disponibles que le nombre d’heures de travail prévues qui lui ont été affectées. Cela peut indiquer que l’équipe connaît une charge de travail déficitaire pendant la période spécifiée. Le nombre supplémentaire d’heures disponibles pour que l’équipe interne termine le travail s’affiche à gauche du cercle bleu.

  ![](assets/resource-capacity-under-capacity.png)

Pointez sur la ligne d’une équipe pour afficher le nombre exact d’heures de capacité prévue et de capacité disponible, ainsi que le nombre d’heures pendant lesquelles l’équipe interne connaît une charge de travail trop importante ou déficitaire.

Ces informations vous aident à déterminer :

* Si l’équipe connaît une charge de travail trop importante ou déficitaire.
* Principaux projets sur lesquels l’équipe interne porte ses efforts.
* Quelles sont les équipes disponibles pour travailler.

Pour savoir comment obtenir les meilleures données pour cette visualisation, consultez la section [Vue d’ensemble d’Analytique améliorée](../enhanced-analytics/enhanced-analytics-overview.md).

## Afficher la visualisation de capacité des ressources

{{step1-to-analytics}}

1. Dans le panneau de gauche, sélectionnez **Personnes**.

   ![](assets/people-area-cropped-qs-350x276.png)

1. (Facultatif) Pour utiliser une autre période, sélectionnez de nouvelles dates de début et de fin dans le filtre de période situé dans le coin supérieur droit du graphique.

   ![](assets/filters-select-date-range-350x344.png)

   Pour plus d’informations sur l’utilisation du filtre de période, consultez la section [Appliquer des filtres dans Analytique améliorée](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Le cas échéant) Si vous n’avez pas défini votre filtre d’équipe, ajoutez-le et sélectionnez chaque équipe dont vous souhaitez voir les données.

   Pour plus d’informations sur l’ajout de filtres dans Analytique améliorée, consultez la section [Appliquer des filtres dans Analytique améliorée](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Une fois les filtres ajoutés, les données de 50 projets au maximum s’affichent et les filtres restent actifs même lorsque vous quittez la page ou en cas de déconnexion de Workfront.

1. (Facultatif) Pour effectuer un zoom avant sur une période, sélectionnez un point de la visualisation pour le début de la période, puis faites-le glisser jusqu’à la fin de la période.

   Toutes les autres visualisations sont mises à jour sur la même période et un filtre de délai est créé.

   ![](assets/timeframe-filter-350x220.png)

1. Pointez sur la ligne de l’équipe interne pour afficher les éléments suivants :

   * Nombre d’heures pouvant encore être planifiées
   * Nombre d’heures prévues pour l’équipe interne
   * Nombre total d’heures travaillées. Le nombre total d’heures travaillées peut comporter les libellés suivantes :

      * Sur-capacité
      * Inférieur à la capacité
      * Égal à la capacité.

   ![](assets/resource-capacity-capacity-pop-up-350x213.png)

1. (Facultatif) Pour exporter les données de visualisation, cliquez sur l’**icône Exporter** ![](assets/export.png) dans le coin supérieur droit de la visualisation et sélectionnez le format de l’export :

   * **Graphique (PNG)**
   * **Tableau de données (XLSX)**

1. Cliquez sur le nom d’une équipe interne pour afficher plus d’informations dans la visualisation de capacité de l’équipe.

   Pour en savoir plus sur la visualisation de capacité de l’équipe, consultez la section [Visualisation de capacité de l’équipe dans Analytique améliorée](../enhanced-analytics/team-capacity-overview.md).


