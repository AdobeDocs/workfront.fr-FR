---
title: Affichage des tâches dans la visualisation en vol dans Enhanced Analytics
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: La visualisation Tâches en vol indique le nombre de tâches (dans les critères de filtrage appliqués) en cours pour un projet, le pourcentage de tâches terminées pour chaque tâche et la planification des tâches.
author: Nolan
feature: Reports and Dashboards
exl-id: cc738450-362a-49e8-836f-611fa82057b5
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '717'
ht-degree: 0%

---

# Affichage des tâches dans la visualisation en vol dans Enhanced Analytics

La visualisation Tâches en vol indique le nombre de tâches (dans les critères de filtrage appliqués) en cours pour un projet, le pourcentage de tâches terminées pour chaque tâche et la planification des tâches.

![](assets/tasks-in-flight-possible-replacement-350x104.png)

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
   <td> <p>Affichage de l’accès aux projets</p> <p>Afficher l’accès aux tâches (pour mettre à jour les tâches, vous devez disposer de l’accès Modifier aux tâches.)</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès.<br>Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Affichage des autorisations pour les objets de projet et de tâche</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Conditions préalables

Pour connaître les conditions préalables à l’utilisation d’Analytics amélioré, reportez-vous à la section &quot;Conditions préalables&quot; de la section [Présentation des analyses améliorées](../enhanced-analytics/enhanced-analytics-overview.md).

## Présentation des tâches dans la visualisation en vol

La visualisation Tâches dans le plan de vol affiche les détails de la tâche suivants :

* **Durée planifiée de la tâche**: La longueur d’une barre de tâches indique la durée planifiée, basée sur la date de début et la date d’achèvement de la tâche.

   ![](assets/tasks-in-flight-duration-350x80.png)

* **Travail terminé**: La couleur bleue foncée d’une barre de tâches indique la quantité de travail terminée pour une tâche. Ce pourcentage d’achèvement s’affiche à droite de la barre des tâches.

   ![](assets/tasks-in-flight-dark-blue-350x35.png)

* **Reste de l&#39;effort**: La couleur bleue claire d’une barre de tâches indique la quantité de travail à effectuer pour une tâche.

   ![](assets/tasks-in-flight-light-blue-350x35.png)

Ces informations peuvent vous aider à déterminer :

* Là où les efforts ont été concentrés.
* Les tâches qui pourraient mettre un projet en danger.
* À quel point une tâche est près d’être terminée.
* À qui vous devez parler d’une tâche spécifique.

Pour savoir comment obtenir les meilleures données pour cette visualisation, voir [Présentation des analyses améliorées](../enhanced-analytics/enhanced-analytics-overview.md).

## Affichage des tâches dans la visualisation en vol

1. Cliquez sur l’icône du menu principal ![](assets/main-menu-icon-16x12.png), puis sélectionnez **Analytics**.
1. (Facultatif) Pour utiliser une autre période, sélectionnez de nouvelles dates de début et de fin dans le filtre de période.

   ![](assets/filters-select-date-range-350x344.png)

   Pour plus d’informations sur l’utilisation du filtre de période, voir [Application de filtres dans les analyses améliorées](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Conditionnel) Si vous devez limiter l’ensemble de données du projet, sélectionnez les filtres à utiliser et appliquez-les.

   Pour plus d’informations sur l’ajout de filtres dans les analyses améliorées, voir [Application de filtres dans les analyses améliorées](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Une fois que vous avez ajouté des filtres, les données de 50 projets au maximum s’affichent et les filtres restent principaux même après avoir quitté la page ou vous être déconnecté de Workfront.

1. Sur la visualisation Plan de vol ou Plan Treemap du projet , cliquez sur un projet pour afficher plus d’informations.

   Les visualisations Burndown et Tasks in flight s’affichent.

   >[!NOTE]
   >
   >Pour en savoir plus sur ces autres visualisations, voir :
   >
   >   
   >   
   >   * [Visualisation du plan de vol dans Enhanced Analytics](../enhanced-analytics/flight-plan-overview.md)
   >   * [Visualisation du graphique Treemap du projet dans les analyses améliorées](../enhanced-analytics/project-treemap-overview.md)
   >   * [Affichage de la visualisation de Burndown dans les analyses améliorées](../enhanced-analytics/burndown-overview.md)


1. (Facultatif) Pour effectuer un zoom avant sur une période, sélectionnez un point de la visualisation pour le début de la période et faites glisser le curseur jusqu’à la fin de la période.

   Toutes les autres visualisations se mettent à jour sur la même période et un filtre de période est créé.

   ![](assets/timeframe-filter-350x220.png)

1. (Facultatif) Pour modifier le mode de tri des tâches, cliquez sur le bouton **Tri par** , puis sélectionnez une nouvelle option de tri :

   * **Date d&#39;achèvement**
   * **Ordre alphabétique A-Z**
   * **Structure de la répartition des tâches** (Cette option correspond à l’ordre dans lequel les tâches apparaissent dans le projet.)

   Toutes les autres visualisations de la page sont mises à jour pour correspondre à votre sélection de tri.

1. Passez en revue l’état d’avancement des tâches dans le projet sélectionné, puis passez le curseur de la souris sur une tâche spécifique pour afficher le nombre d’heures planifiées, la date d’échéance prévue et le pourcentage d’achèvement.

   ![](assets/tasks-in-flight-task-details-350x242.png)

1. Cliquez sur une tâche pour ouvrir les Détails de la tâche dans la partie droite de l’écran, où vous pouvez voir plus d’informations sur la tâche, afficher ou saisir des mises à jour, ou apporter des modifications à la tâche.

   ![](assets/task-details-qs-350x675.png)

1. (Facultatif) Pour exporter les données de visualisation, cliquez sur le bouton **Icône Exporter** ![](assets/export.png) dans le coin supérieur droit de la visualisation, sélectionnez le format d’exportation :

   * **Graphique (PNG)**
   * **Tableau de données (XSLX)**

