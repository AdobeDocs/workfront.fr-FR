---
title: Afficher la visualisation de la feuille de route dans Analytique améliorée
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: La visualisation de la feuille de route montre combien de projets (selon les critères de filtre appliqués) étaient en cours, quels changements de statuts sont intervenus pendant la durée de vie de ces projets et dans quelle mesure ces projets ont respecté les délais d’achèvement prévus.
author: Nolan
feature: Reports and Dashboards
exl-id: c64ed752-151a-40f7-ab18-684e2cd032bc
source-git-commit: 2a6e767036ae702f6c19dc71cdb11dae8e9e37ea
workflow-type: tm+mt
source-wordcount: '924'
ht-degree: 93%

---

# Afficher la visualisation de la feuille de route dans Analytique améliorée

>[!IMPORTANT]
>
>Enhanced Analytics a été supprimé de Workfront le 27 mai. Workfront Data Connect est une nouvelle solution alternative qui peut être utilisée pour répliquer toutes les visualisations Enhanced Analytics que vous utilisez actuellement. <br>Pour plus d’informations, consultez le guide [Obsolescence améliorée d’Analytics](/help/quicksilver/product-announcements/announcements/enhanced-analytics-deprecation.md) .


La visualisation de la feuille de route montre combien de projets (selon les critères de filtre appliqués) étaient en cours, quels changements de statuts sont intervenus pendant la durée de vie de ces projets et dans quelle mesure ces projets ont respecté les délais d’achèvement prévus.

![Plan de vol ](assets/flight-plan-350x132.png)

## Conditions d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://business.adobe.com/products/workfront/pricing.html" target="_blank">Plan Adobe Workfront</a>*</td> 
   <td> <p>Entreprises ou niveau supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Vue d’ensemble des licences Adobe Workfront</a>*</td> 
   <td> <p>Révision ou supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Afficher l’accès aux projets</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès.<br>Pour plus d’informations sur la manière dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, consultez <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Afficher l’accès au projet</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, consultez <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès à des objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Conditions préalables

Pour connaître les conditions préalables à l’utilisation d’Analytique améliorée, reportez-vous à la section « Conditions préalables » de la section [Vue d’ensemble d’Analytique améliorée](../enhanced-analytics/enhanced-analytics-overview.md).

## Comprendre la visualisation de la feuille de route

Dans la durée réelle d’un projet, vous ne pouvez voir que les statuts suivants :

* Dans les temps
* En danger
* En difficulté

Pour en savoir plus sur les statuts des projets, voir [Vue d’ensemble du statut des projets et du type de statut](../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

La visualisation de la feuille de route montre les détails suivants du projet :

* **Durée prévue** : la ligne bleue horizontale représente la durée prévue du projet, les triangles à chaque extrémité de la ligne indiquant la date de début et la date de fin.

  ![Durée prévue](assets/planned-duration-line-350x37.png)

* **Durée effective** : la ligne épaisse et colorée située sous la durée prévue représente la durée effective du projet. La couleur de la ligne change en fonction du statut du projet à ce moment précis de son cycle de vie.

  ![Durée réelle](assets/actual-duration-line.png)

* **Statut réel** : la ligne épaisse colorée montre également le statut d’un projet à différents moments. La couleur de la ligne change en fonction du statut du projet :

   * **Vert** : Ciblé
   * **Orange** : À risque
   * **Rouge** : À problème

  ![Condition réelle](assets/actual-condition-color.png)

En pointant sur une ligne de projet dans la visualisation de la feuille de route, vous pouvez obtenir des informations sur le délai prévu du projet, son statut actuel et, le cas échéant, son statut personnalisé. Pour vous faire une idée plus précise de ce qui a pu affecter la durée ou le statut, vous pouvez consulter les autres visualisations dans la zone Analytique améliorée.

Ces informations vous aident à déterminer :

* Événements qui prolongent un projet au-delà de la date d’achèvement prévue d’origine.
* Lorsqu’un projet commence à rencontrer des problèmes.
* Le nombre de projets ouverts au cours de la même période.
* Le nombre de projets actifs.
* Les projets qui nécessitent une attention ou un soutien supplémentaire.

Pour plus d’informations sur la manière d’obtenir les meilleures données pour cette visualisation, voir [Vue d’ensemble d’Analytique améliorée](../enhanced-analytics/enhanced-analytics-overview.md).

## Afficher la visualisation de la feuille de route

1. Cliquez sur l’icône **Menu principal** ![icône du menu principal](assets/main-menu-icon-16x12.png), puis sélectionnez **Analytics**.
1. (Facultatif) Pour utiliser une autre période, sélectionnez de nouvelles dates de début et de fin dans le filtre des périodes.

   ![Sélectionner une période](assets/filters-select-date-range-350x344.png)

   Pour plus d’informations sur l’utilisation du filtre de période, voir [Appliquer des filtres dans Analytique améliorée](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. Le cas échéant, si vous devez limiter l’ensemble de données du projet, sélectionnez les filtres à utiliser et appliquez-les.

   Pour plus d’informations sur l’ajout de filtres dans Analytique améliorée, voir [Appliquer des filtres dans Analytique améliorée](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Une fois les filtres ajoutés, les données de 50 projets au maximum s’affichent et les filtres restent actifs même lorsque vous quittez la page ou en cas de déconnexion de Workfront.

1. (Facultatif) Pour effectuer un zoom avant sur une période, sélectionnez un point de la visualisation pour le début de la période, puis faites-le glisser jusqu’à la fin de la période.

   Toutes les autres visualisations sont mises à jour sur la même période et un filtre de délai est créé.

   ![Filtre des délais](assets/timeframe-filter-350x220.png)

1. (Facultatif) Pour modifier la façon dont les projets sont triés, cliquez sur le menu **Trier par** dans le coin supérieur droit de la visualisation de la feuille de route, puis sélectionnez une nouvelle option de tri :

   * **A - Z**
   * **Z - A**
   * **Date d’achèvement prévue**
   * **Date de début prévue**

   Toutes les autres visualisations de la page sont mises à jour pour correspondre à votre sélection de classement.

1. (Le cas échéant) S’il existe plus de 50 projets dans votre jeu de données, utilisez les flèches situées dans le coin inférieur gauche de la visualisation pour passer d’un groupe de 50 projets à un autre.

   Toutes les autres visualisations de la page sont mises à jour pour correspondre à votre sélection de page.

   ![ Pagination ](assets/pagination-350x118.png)

1. Pointez sur le graphique en barres du projet pour voir la ligne bleue de la date, ainsi que les détails suivants :

   * Chronologie prévue
   * Statut actuel
   * Statut personnalisé (le cas échéant)

   ![Graphique à barres Projet](assets/project-bar-graph-350x143.png)

1. (Facultatif) Pour exporter les données de visualisation, cliquez sur l’icône **Exporter** ![icône Exporter](assets/export.png) en haut à droite de la visualisation, puis sélectionnez le format d’export :

   * **Graphique (PNG)**
   * **Table de données (XLSX)**

1. Pour obtenir davantage d’informations sur un projet, cliquez sur un projet dans la visualisation pour ouvrir les visualisations Avancement et Tâches en cours.

   Ces visualisations peuvent vous aider à mieux comprendre ce qui a retardé le projet. Elles permettent également de vérifier facilement l’état d’avancement d’un projet.\
   Pour plus d’informations sur la visualisation Avancement, voir [Afficher la visualisation Avancement dans Analytique améliorée](../enhanced-analytics/burndown-overview.md). Pour plus d’informations sur la visualisation des tâches en cours, voir [Afficher la visualisation des tâches en cours dans l’Analytique améliorée](../enhanced-analytics/tasks-in-flight-overview.md).

