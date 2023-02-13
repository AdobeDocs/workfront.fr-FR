---
title: Visualisation de la capacité des ressources dans les analyses améliorées
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: La visualisation Capacité des ressources indique si une équipe est terminée, sous ou à capacité. Ce calcul est basé sur - EDIT ME.
author: Nolan
feature: Reports and Dashboards
exl-id: 5bb45ef6-9e49-4063-8e53-c9f3bc994870
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '833'
ht-degree: 0%

---

# Visualisation de la capacité des ressources dans les analyses améliorées

La visualisation Capacité des ressources indique si une équipe est terminée, sous ou à capacité.

## Exigences d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Formule Adobe Workfront</a>*</td> 
   <td> <p>Professionnel ou supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Présentation des licences Adobe Workfront</a>*</td> 
   <td> <p>Révision ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Affichage de l’accès aux projets</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès.<br>Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Afficher</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Conditions préalables

Pour connaître les conditions préalables à l’utilisation d’Analytics amélioré, reportez-vous à la section &quot;Conditions préalables&quot; de la section [Présentation des analyses améliorées](../enhanced-analytics/enhanced-analytics-overview.md).

## Présentation de la visualisation de la capacité de ressource

La visualisation Capacité des ressources indique si une équipe est terminée, sous ou à capacité. Ce calcul est basé sur :

* **Capacité disponible**: Nombre total d’heures pendant lesquelles une équipe d’accueil peut travailler pendant la période filtrée.

   >[!NOTE]
   >
   >Si vous envisagez une période future, la capacité disponible est calculée en fonction de la capacité de l’équipe au cours des 7 derniers jours. Pour cette raison, aucun PTO planifié n’est pris en compte.

* **Capacité planifiée**: Le nombre total d’heures de travail planifiées attendues de la part de l’équipe d’accueil au cours de la période filtrée.

Cette comparaison des heures prévues et des heures planifiées réelles d’une équipe peut vous aider à déterminer si vous n’affectez pas suffisamment de travail à l’équipe locale ou si elle subit un épuisement dû à une charge de travail importante.

![](assets/resource-capacity-350x110.png)

Dans la visualisation de la capacité de ressource, vous pouvez voir les détails suivants :

* **Capacité planifiée**: En ligne avec le nom d’une équipe d’accueil, le cercle bleu représente le nombre d’heures planifiées attribuées à l’équipe d’accueil.

   ![](assets/resource-capacity-blue-circle.png)

* **Capacité réelle**: Avec le nom d’une équipe d’accueil, la ligne verticale représente le nombre d’heures disponibles pour l’équipe d’accueil.

   ![](assets/resource-capacity-vertical-line.png)

* **Capacité excédentaire**: Lorsque la ligne horizontale et le cercle bleu s’affichent à droite de la ligne verticale, l’équipe d’accueil se voit attribuer plus de travail qu’elle ne peut en faire en nombre d’heures disponibles. Cela signifie que l’équipe peut être surchargée pendant la période filtrée. Le nombre d’heures restantes que l’équipe doit terminer s’affiche à droite du cercle bleu.

   ![](assets/resource-capacity-over-capacity.png)

* **Sous capacité**: Lorsque la ligne horizontale et le cercle bleu s’affichent à gauche de la ligne verticale, l’équipe d’accueil dispose de plus d’heures disponibles que le nombre d’heures de travail planifiées qui leur ont été affectées. Cela signifie que l’équipe peut être en capacité pendant la période filtrée. Le nombre supplémentaire d’heures disponibles pour que l’équipe d’accueil termine le travail s’affiche à gauche du cercle bleu.

   ![](assets/resource-capacity-under-capacity.png)

Le survol d’une ligne indique le nombre exact d’heures de capacité planifiée et de capacité disponible, ainsi que le nombre d’heures pendant lesquelles l’équipe d’accueil est supérieure ou inférieure à sa capacité.

L’affichage de ces informations vous permet de déterminer les éléments suivants :

* Si l&#39;équipe d&#39;accueil a été surchargée ou sous-affectée.
* Ce sur quoi l&#39;équipe d&#39;accueil s&#39;est concentrée, ce sont les plus grands projets.
* Quelles équipes domestiques sont disponibles pour le travail ?

Pour savoir comment obtenir les meilleures données pour cette visualisation, voir [Présentation des analyses améliorées](../enhanced-analytics/enhanced-analytics-overview.md).

## Visualisation de la capacité de ressource

1. Cliquez sur l’icône du menu principal ![](assets/main-menu-icon-16x12.png), puis sélectionnez **Analytics**.
1. Dans le panneau de gauche, sélectionnez **Personnes**.

   ![](assets/people-area-cropped-qs-350x276.png)

1. (Facultatif) Pour utiliser une autre période, sélectionnez de nouvelles dates de début et de fin dans le filtre de période.

   ![](assets/filters-select-date-range-350x344.png)

   Pour plus d’informations sur l’utilisation du filtre de période, voir [Application de filtres dans les analyses améliorées](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Conditionnel) Si vous n’avez pas défini le filtre Équipe, ajoutez le filtre Équipe et sélectionnez chaque équipe pour laquelle vous souhaitez afficher des données.

   Pour plus d’informations sur l’ajout de filtres dans les analyses améliorées, voir [Application de filtres dans les analyses améliorées](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Une fois que vous avez ajouté des filtres, les données de 50 projets au maximum s’affichent et les filtres restent principaux même après avoir quitté la page ou vous être déconnecté de Workfront.

1. (Facultatif) Pour effectuer un zoom avant sur une période, sélectionnez un point de la visualisation pour le début de la période et faites glisser le curseur jusqu’à la fin de la période.

   Toutes les autres visualisations se mettent à jour sur la même période et un filtre de période est créé.

   ![](assets/timeframe-filter-350x220.png)

1. Passez la souris sur la ligne de l’équipe d’accueil pour voir combien d’heures sont encore disponibles pour la planification, le nombre d’heures planifiées pour l’équipe d’accueil et le nombre total d’heures travaillées, qui est indiqué comme étant terminé, inférieur ou à capacité.

   ![](assets/resource-capacity-capacity-pop-up-350x213.png)

1. (Facultatif) Pour exporter les données de visualisation, cliquez sur le bouton **Icône Exporter** ![](assets/export.png) dans le coin supérieur droit de la visualisation, sélectionnez le format d’exportation :

   * **Graphique (PNG)**
   * **Tableau de données (XSLX)**

1. Cliquez sur le nom d’une équipe d’accueil pour afficher plus d’informations dans la visualisation de capacité de l’équipe.

   Pour en savoir plus sur la visualisation de la capacité de l’équipe, voir [Visualisation de la capacité de l’équipe dans Enhanced Analytics](../enhanced-analytics/team-capacity-overview.md).


