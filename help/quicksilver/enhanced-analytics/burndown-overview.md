---
title: Afficher la visualisation de l’avancement dans Analytique améliorée
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: La visualisation de l’avancement présente l’avancement d’un projet spécifique au fil du temps et vous aide à comprendre la relation entre la condition du projet, la vitesse et les heures restantes (ou les jours restants).
author: Nolan
feature: Reports and Dashboards
exl-id: e67c92d5-b309-406b-b6f0-4d414d0e7dcc
source-git-commit: 2a6e767036ae702f6c19dc71cdb11dae8e9e37ea
workflow-type: tm+mt
source-wordcount: '834'
ht-degree: 95%

---

# Afficher la visualisation de l’avancement dans Analytique améliorée

>[!IMPORTANT]
>
>Enhanced Analytics a été supprimé de Workfront le 27 mai. Workfront Data Connect est une nouvelle solution alternative qui peut être utilisée pour répliquer toutes les visualisations Enhanced Analytics que vous utilisez actuellement. <br>Pour plus d’informations, consultez le guide [Obsolescence améliorée d’Analytics](/help/quicksilver/product-announcements/announcements/enhanced-analytics-deprecation.md) .


<!-- Audited: 12/2023 -->

La visualisation de l’avancement présente l’avancement d’un projet spécifique au fil du temps et vous aide à comprendre la relation entre la condition du projet, la vitesse et les heures restantes (ou les jours restants).

![Exemple d’avancement d’Analytique améliorée](assets/burndown120623.png)

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
   <td> <p>Afficher l’accès aux projets</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Afficher</p> </td>
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur le contenu de ce tableau, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Conditions préalables

Pour connaître les conditions préalables à l’utilisation d’Analytique améliorée, reportez-vous à la section « Conditions préalables » de la section [Vue d’ensemble d’Analytique améliorée](../enhanced-analytics/enhanced-analytics-overview.md).

## Comprendre la visualisation de l’avancement

La ligne bleue continue indique la vitesse prévue entre la date de début et la date d’achèvement prévue. Cette ligne s’ajuste au fur et à mesure que du travail est ajouté, supprimé ou mis à jour. Elle se transforme en ligne verticale pointillée lorsque le projet atteint la date d’achèvement prévue.

![Vitesse prévue](assets/burndown-planned-line.png)

La ligne réelle indique le nombre d’heures (ou de jours) passées sur le projet au fil du temps. La couleur de cette ligne indique l’état du projet chaque jour :

* **Vert** : le projet avance comme prévu.

  ![Dans les temps](assets/burndown-green.png)

* **Orange** : le projet est à risque.

  ![À risque](assets/burndown-orange.png)

* **Rouge** : le projet est en difficulté.

  ![En difficulté](assets/burndown-red.png)

Pour plus d’informations sur ces conditions de projet, voir [Vue d’ensemble de la condition et du type de condition du projet](../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

Lorsque la ligne monte verticalement, cela signifie que du travail a été ajouté au projet. Lorsque la ligne descend verticalement, cela signifie que du travail a été supprimé ou terminé dans le projet.

Sous l’axe X de la visualisation, vous trouvez d’autres informations sur la façon dont les tâches et les heures (ou jours) ont changé un jour donné (la quantité ajoutée, la quantité terminée et la différence entre les deux).

L’affichage de toutes ces informations dans la visualisation de l’avancement vous permet de déterminer :

* L’intégrité de chaque projet au fil du temps
* L’effet des problèmes (ou du travail non planifié) sur le travail planifié.
* Les événements qui ont prolongé le projet au-delà de la date d’achèvement initiale.

Pour savoir comment obtenir les meilleures données pour cette visualisation, voir [Vue d’ensemble d’Analytique améliorée](../enhanced-analytics/enhanced-analytics-overview.md).

## Afficher la visualisation de l’avancement

{{step1-to-analytics}}

1. (Facultatif) Pour utiliser une autre période, sélectionnez de nouvelles dates de début et de fin dans le filtre des périodes.

   ![Sélectionner des dates](assets/filters-select-date-range-350x344.png)

   Pour plus d’informations sur l’utilisation du filtre des périodes, voir [Appliquer des filtres dans Analytique améliorée](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. Le cas échéant, si vous devez limiter l’ensemble de données du projet, sélectionnez les filtres à utiliser et appliquez-les.

   Pour plus d’informations sur l’ajout de filtres dans Analytique améliorée, voir [Appliquer des filtres dans Analytique améliorée](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Une fois les filtres ajoutés, les données de 50 projets au maximum s’affichent et les filtres restent actifs même lorsque vous quittez la page ou en cas de déconnexion de Workfront.

1. (Facultatif) Pour effectuer un zoom avant sur une période, sélectionnez un point de la visualisation pour le début de la période, puis faites-le glisser jusqu’à la fin de la période.

   Toutes les autres visualisations sont mises à jour sur la même période et un filtre de délai est automatiquement créé.

   ![Filtre de délai](assets/timeframe-filter-350x220.png)

1. Sur la visualisation de plan de vol ou d’arborescence du projet, cliquez sur un projet pour afficher plus d’informations.

   Les visualisations d’avancement et des tâches en cours s’affichent.

   >[!NOTE]
   >
   >Pour en savoir plus sur ces autres visualisations, consultez :
   >
   >   * [Afficher la visualisation de plan de vol dans Analytique améliorée](../enhanced-analytics/flight-plan-overview.md)
   >   * [Afficher la visualisation d’arborescence du projet dans Analytique améliorée](../enhanced-analytics/project-treemap-overview.md)
   >   * [Afficher la visualisation des tâches en cours dans dans Analytique améliorée](../enhanced-analytics/tasks-in-flight-overview.md)
   >

1. (Facultatif) Remplacez l’affichage du nombre d’heures prévues par une **durée**.

   Le nombre d’heures prévues est sélectionné par défaut.

   >[!NOTE]
   >
   >Sélectionnez la **durée** pour remplacer toutes les informations en heures par des jours.\
   >![Avancement de la durée](assets/duration-burndown-350x112.png)\
   >Pour plus d’informations sur la durée dans la zone Analytique améliorée, consultez la section « Vue de la durée » dans [Vue d’ensemble d’Analytique améliorée](../enhanced-analytics/enhanced-analytics-overview.md#duration-view).

1. Cliquez sur n’importe quel point du graphique linéaire.

   La date exacte s’affiche et des informations supplémentaires sur les tâches et les heures (ou jours) du jour sélectionné s’affichent sous le graphique.

   ![Détails de l’avancement](assets/burndown-task-and-hour-changes-350x121.png)

   >[!NOTE]
   >
   >Si la vitesse réelle est une ligne plane le long de l’axe x (alignée sur 0 heure ou 0 jour) de la visualisation, cela signifie qu’aucune heure (ou jour) prévue n’a été ajoutée au projet.\
   >Si la vitesse réelle est une ligne plane au-dessus de l’axe x (alignée sur un nombre d’heures ou de jours) qui ne diminue jamais, cela signifie qu’aucune tâche n’a été effectuée pendant la période filtrée.

1. (Facultatif) Pour exporter les données de visualisation, cliquez sur l’icône **Exporter** ![icône Exporter](assets/export.png) dans le coin supérieur droit de la visualisation, puis sélectionnez le format d’export :

   * Graphique (PNG)
   * Table de données (XLSX)

1. (Facultatif) Pour afficher des détails sur la progression des tâches dans le projet sélectionné, consultez la visualisation Tâches en cours qui s’affiche sous la visualisation Avancement. Pour plus d’informations, consultez [Afficher la visualisation Tâches en cours dans Analytique améliorée](/help/quicksilver/enhanced-analytics/tasks-in-flight-overview.md).
