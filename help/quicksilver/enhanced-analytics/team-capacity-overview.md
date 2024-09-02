---
title: Afficher la visualisation de la capacité de l’équipe dans Analytique améliorée
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: La visualisation de la capacité de l’équipe montre la capacité totale dont dispose une équipe interne, si elle connaît une affectation excédentaire ou insuffisante, et le dynamisme de la capacité au fil du temps.
author: Nolan
feature: Reports and Dashboards
exl-id: cfeb1a87-01be-4088-9e33-53a97e3871ad
source-git-commit: 81118e794dca746b482b8355c24fa997a9f0edc9
workflow-type: ht
source-wordcount: '712'
ht-degree: 100%

---

# Afficher la visualisation de la capacité de l’équipe dans Analytique améliorée

<!-- Audited: 01/2024 -->

La visualisation de la capacité de l’équipe montre la capacité totale dont dispose une équipe interne, si elle connaît une affectation excédentaire ou insuffisante, et le dynamisme de la capacité au fil du temps.

![Capacité de l’équipe](assets/team-capacity.png)

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>
      <p>Nouveau : Tous</p>
      <p>ou</p>
      <p>Actuel : Entreprises ou supérieur</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td>
   <td>
      <p>Nouveau : Light ou supérieur</p>
      <p>ou</p>
      <p>Actuel : Révision ou supérieur</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td>Afficher l’accès aux projets</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td>Afficher </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur le contenu de ce tableau, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Conditions préalables

Pour connaître les conditions préalables à l’utilisation d’Analytique améliorée, reportez-vous à la section « Conditions préalables » de la section [Vue d’ensemble d’Analytique améliorée](../enhanced-analytics/enhanced-analytics-overview.md).

## Comprendre la visualisation de la capacité de l’équipe

La visualisation de la capacité de l’équipe affiche le volume de travail affecté à l’équipe interne un jour donné.

* **Surcharge de travail** : lorsque la couleur de remplissage bleu foncé est au-dessus de la ligne pointillée, cela signifie que l’équipe interne s’est vu affecter plus d’heures de travail qu’elle ne peut en effectuer au cours du nombre d’heures dont elle dispose pour travailler. Cela indique que l’équipe est surchargée et qu’elle risque l’épuisement professionnel.

  ![Sur-capacité](assets/team-capacity-over-capacity.png)

* **Incontesté** : lorsque la couleur de remplissage bleu foncé est en dessous de la ligne pointillée, cela signifie que l’équipe interne dispose de plus d’heures de travail que ce que nécessite le travail qui lui a été affecté. Cela indique que l’équipe ne reçoit pas assez de tâches et qu’elle ne rencontre pas de challenge.

  ![Inférieur à la capacité](assets/team-capacity-under-capacity.png)

* **Équilibre** : lorsque la couleur de remplissage bleue plus claire ou plus transparente se trouve juste au-dessus, juste au-dessous ou au niveau de la ligne pointillée, cela signifie que l’équipe locale s’est vu affecter une quantité de travail qu’elle devrait être en mesure d’accomplir dans le cadre des heures de travail dont elle dispose. Cela indique que la charge de travail de l’équipe est plus équilibrée.

  ![Égal à la capacité](assets/team-capacity-at-capacity.png)

Le survol d’un point quelconque de la visualisation permet d’afficher les détails suivants pour un jour donné :

* **Horaires planifiés** : il s’agit du nombre d’heures de travail prévues que l’équipe doit accomplir.
* **Heures disponibles** : il s’agit du nombre d’heures de travail dont dispose l’équipe.
* **Capacité** : en plus du pourcentage de capacité, les mentions Égal à la capacité, Inférieur à la capacité, ou Sur-capacité s’affichent également.

Ces informations vous aident à déterminer :

* Lorsque l’équipe interne a fait l’objet d’une affectation trop importante ou insuffisante.
* Si l’équipe interne fait quotidiennement l’objet d’une affectation trop importante ou insuffisante.
* La cohérence de la charge de travail d’une équipe locale au quotidien.
* Si vous créez des problèmes de capacité avec un nouveau travail.

Pour savoir comment obtenir les meilleures données pour cette visualisation, voir la section [Vue d’ensemble de l’Analytique améliorée](../enhanced-analytics/enhanced-analytics-overview.md).

## Afficher la visualisation de la capacité de l’équipe

{{step1-to-analytics}}

1. Dans le panneau de gauche, sélectionnez **Personnes**.

   ![Sélection de personnes](assets/people-area-cropped-qs-350x276.png)

1. (Facultatif) Pour utiliser une autre période, sélectionnez de nouvelles dates de début et de fin dans le filtre des périodes.

   ![Filtre de période](assets/filters-select-date-range-350x344.png)

   Pour plus d’informations sur l’utilisation du filtre de période, voir la section [Appliquer des filtres dans Analytique améliorée](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Le cas échéant) Si vous n’avez pas défini votre filtre d’équipe, ajoutez-le et sélectionnez chaque équipe dont vous souhaitez voir les données.

   Pour plus d’informations sur l’ajout de filtres dans Analytique améliorée, voir la section [Appliquer des filtres dans Analytique améliorée](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Une fois les filtres ajoutés, les données de 50 projets au maximum s’affichent et les filtres restent actifs même lorsque vous quittez la page ou en cas de déconnexion de Workfront.

1. Dans la visualisation de la capacité des ressources, cliquez sur une équipe pour obtenir davantage d’informations.

   La visualisation de la capacité de l’équipe s’affiche.

   Pour plus d’informations sur la visualisation de la capacité des ressources, voir la section [Afficher la visualisation de la capacité des ressources dans Analytique améliorée](../enhanced-analytics/resource-capacity-overview.md).

1. (Facultatif) Pour effectuer un zoom avant sur une période, sélectionnez un point de la visualisation pour le début de la période, puis faites-le glisser jusqu’à la fin de la période.

   Toutes les autres visualisations sont mises à jour sur la même période et un filtre de délai est créé.

   ![Filtre des délais](assets/timeframe-filter-350x220.png)

1. Passez la souris sur un point de la ligne graphique pour afficher les horaires planifiés et le nombre d’heures prévues pour la date donnée, ainsi que le pourcentage de capacité et si l’équipe locale était en sous-capacité, en sur-capacité ou en capacité équilibrée à ce moment-là.

   ![Pop-up sur la capacité de l’équipe](assets/team-capacity-capacity-pop-up-350x351.png)

1. (Facultatif) Pour exporter les données de visualisation, cliquez sur l’icône **Exporter** ![icône Exporter](assets/export.png) en haut à droite de la visualisation, puis sélectionnez le format d’export :

   * Graphique (PNG)
   * Table de données (XLSX)

