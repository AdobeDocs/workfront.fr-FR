---
title: Vue d’ensemble d’Analytique améliorée
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: Les analyses améliorées constituent un puissant outil d’Adobe Workfront avec des visualisations prédéfinies qui vous permettent d’examiner les données du projet et d’identifier les tendances en matière de planification et d’achèvement. Grâce à ces informations sur vos projets, vous pouvez gérer votre travail actuel et planifier plus précisément votre travail futur.
author: Nolan
feature: Reports and Dashboards
exl-id: a14ad57c-859b-43df-84c0-575ccda86e50
source-git-commit: 530c4451f4720a1710350f8e822e343794b63e87
workflow-type: tm+mt
source-wordcount: '1203'
ht-degree: 5%

---

# Vue d’ensemble d’Analytique améliorée

Les analyses améliorées constituent un puissant outil d’Adobe Workfront avec des visualisations prédéfinies qui vous permettent d’examiner les données du projet et d’identifier les tendances en matière de planification et d’achèvement. Grâce à ces informations sur vos projets, vous pouvez gérer votre travail actuel et planifier plus précisément votre travail futur.

Les analyses améliorées peuvent vous aider à identifier :

* La manière dont vous planifiez les projets
* Lorsque le travail est ajouté aux projets
* La durée du travail pour différents projets
* Nombre d’heures ou de jours requis pour terminer un projet par rapport aux heures ou aux jours planifiés d’une équipe d’accueil
* Fréquence à laquelle les utilisateurs effectuent des actions spécifiques au cours d’un projet
* L’avancement des projets, ainsi que les tâches individuelles au sein d’un projet

![](assets/nwe-full-screen-analytics-350x222.png)

Pour consulter des cas d’utilisation ou en savoir plus sur la gestion des travaux actuels et la planification des travaux futurs à l’aide d’Analyses améliorées, voir [Chemins d’apprentissage Analytics améliorés](https://one.workfront.com/s/enhanced-analytics-program).

## Conditions préalables

Pour accéder à la zone Analyses améliorées, vous devez :

* Formule Entreprise ou Entreprise.

  Pour plus d’informations, voir [Plans Workfront](https://www.workfront.com/plans).

* Demandez à votre administrateur Workfront d’ajouter des analyses améliorées à votre modèle de mise en page.

  Pour plus d’informations, voir [Analytics amélioré : ajout d’analyses aux modèles de mise en page](https://one.workfront.com/s/managed-content-videos/enhanced-analytics-adding-analytics-to-layout-templates-MCH7URDSIXRREHHHF7TRTYYP2LTE).

Pour afficher les informations relatives aux projets et aux tâches, vous devez :

* Disposez de l’autorisation Afficher dans les zones Projets et tâches de votre niveau d’accès.

  Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir [Créer ou modifier les niveaux d’accès personnalisés](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* Posséder l’autorisation Afficher pour des tâches et/ou des projets spécifiques.

  Pour plus d’informations sur la demande d’accès supplémentaire, voir [Demande d’accès aux objets](../workfront-basics/grant-and-request-access-to-objects/request-access.md).

## Bonnes pratiques relatives aux analyses améliorées

Afin d’obtenir les meilleures données pour vos projets, utilisez des modèles comportant des heures et des jours planifiés précis. Vous devez également vous assurer que vos utilisateurs saisissent et mettent à jour les champs ci-dessous aussi précisément que possible.

>[!NOTE]
>
>Certains des champs suivants sont des calculs que Workfront effectue en fonction des informations que les utilisateurs saisissent. Vous ne pouvez pas mettre à jour ces champs manuellement.

* Heures prévues

  Il s’agit du champ le plus important à remplir.

  >[!NOTE]
  >
  >Si vos équipes n’utilisent pas les heures planifiées, vous pouvez toujours afficher certaines données en fonction de la durée du projet.\
  >Pour plus d’informations, voir la section [Vue Durée](#duration-view) dans cet article.

* Nom du projet

  Le nom doit être descriptif pour le projet.

* Statut du projet
* Statut de projet
* Date de début prévue du projet
* Date d&#39;achèvement prévue
* Date de début effective du projet
* Date de fin effective du projet
* Heures de durée du projet
* Heures réelles du projet
* État de la tâche (inclut les tâches de marquage terminées.)
* Nom de la tâche
* Pourcentage de la tâche terminé
* Date de début prévue de la tâche
* Date d&#39;achèvement prévue de tâche

>[!IMPORTANT]
>
>Les modifications apportées aux tâches et aux projets peuvent prendre jusqu’à 24 heures pour être répercutées dans les analyses améliorées.

## Vue Durée {#duration-view}

Par défaut, les visualisations du graphique Treemap de Burndown et Project sont basées sur les heures planifiées. Si vos équipes n’utilisent pas les heures planifiées, vous pouvez consulter ces visualisations en fonction de la durée du projet.

Dans les analyses améliorées, la durée d’un projet est calculée par les formules suivantes :

* Période planifiée :

  ```
  Planned Completion Date of the project - Start Date of the project
  ```

* Days Work:

  ```
  Planned Duration for tasks completed in the selected date range / Typical hours per work day
  ```

  >[!NOTE]
  >
  >8 heures est le nombre par défaut pour **Heures types par jour de travail**. Un administrateur Adobe Workfront peut mettre à jour la variable **Heures types par jour de travail** paramètre sous **Configuration** > **Préférences du projet** > **Projets** > **Chronologies**.\
  >Pour en savoir plus, voir [Configuration des préférences de projet à l’échelle du système](../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Pour plus d’informations sur la durée planifiée, voir [Présentation de la durée du projet](../manage-work/projects/planning-a-project/project-duration.md).

## Raccourcis clavier

Vous pouvez utiliser les touches suivantes de votre clavier pour parcourir ou exécuter des actions spécifiques dans la zone Analyses améliorées :

| Clé | Action |
|---|---|
| **Onglet** | Accédez à chaque élément de la page, ainsi qu’à un tableau contenant des informations sur chaque visualisation qui ne s’affiche pas sur la page. |
| **Entrée** | Ouvrez le widget Calendrier, supprimez un filtre existant, ouvrez les options d’ajout de filtre, sélectionnez/désélectionnez les valeurs de filtre, appliquez un filtre que vous avez créé, ouvrez les options d’exportation sur chaque visualisation, ouvrez les menus déroulants sur la liste déroulante, les tâches en cours de vol et les visualisations du graphique Treemap du projet. |
| **Touches de flèches** | Accédez aux dates dans le widget Calendrier, par le biais des options de filtre lors de l’ajout d’un filtre, et des options de tous les menus déroulants des visualisations. |
| **Barre d’espace** | Sélectionnez des dates dans le widget Calendrier, sélectionnez un type de filtre lors de l’ajout d’un filtre, sélectionnez une option d’exportation dans le menu déroulant de chaque visualisation, puis sélectionnez des options dans les menus déroulants de la visualisation de la liste déroulante, des tâches en cours de vol et des graphiques Treemap du projet. |

{style="table-layout:auto"}

Si vous utilisez un logiciel de lecture d’écran ou un plug-in, le lecteur d’écran lit les informations à l’écran à haute voix et décrit les actions que vous effectuez lorsque vous utilisez les clés répertoriées ci-dessus.

## Amélioration des vues et fonctionnalités d’analyse

Pour en savoir plus sur les détails d’une fonctionnalité spécifique dans l’analyse améliorée, les actions que vous pouvez effectuer pour obtenir des informations supplémentaires et ce que vous pouvez apprendre de ces données, consultez les articles suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Article</th> 
   <th>Explication</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><a href="../enhanced-analytics/use-enhanced-analytics-filters.md" class="MCXref xref">Application de filtres dans les analyses améliorées</a> </td> 
   <td> <p>Vous pouvez appliquer des filtres personnalisés, des filtres de champ de projet ou des filtres d’équipe pour afficher uniquement les projets qui correspondent à des critères spécifiques. Lorsque vous ajoutez des filtres, le nombre de projets est mis à jour en conséquence.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/understand-enhanced-analytics-kpis.md" class="MCXref xref">Présentation des indicateurs clés de performance d’analyse améliorés</a> </td> 
   <td> <p>Les indicateurs de performances clés (IPC) de tous les projets au cours d’une période spécifique se trouvent en haut de l’écran.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../enhanced-analytics/flight-plan-overview.md" class="MCXref xref">Visualisation du plan de vol dans Enhanced Analytics</a> </p> </td> 
   <td> <p>La variable <b>Plan de vol</b> la visualisation vous montre que la condition a changé au cours de la vie d’un projet. L’interaction avec la visualisation vous donne plus de détails sur des dates spécifiques. La sélection d’un projet ouvre les visualisations Burndown et Tasks in flight.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/burndown-overview.md" class="MCXref xref">Affichage de la visualisation de Burndown dans les analyses améliorées</a> </td> 
   <td> <p>La variable <b>Burndown</b> la visualisation vous montre la vitesse planifiée d’un projet par rapport au temps réel passé sur un projet. L’interaction avec la visualisation vous donne plus de détails sur la condition du projet à une date spécifique.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/tasks-in-flight-overview.md" class="MCXref xref">Affichage des tâches dans la visualisation en vol dans Enhanced Analytics</a> </td> 
   <td> <p>La variable <b>Tâches en cours</b> la visualisation vous montre l’état de chaque tâche au sein d’un projet. L’interaction avec la visualisation vous permet d’apporter rapidement et facilement des modifications à une tâche.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/project-activity-overview.md" class="MCXref xref">Visualisation de l’activité de projet dans les analyses améliorées</a> </td> 
   <td> <p>La variable <b>Activité du projet</b> la visualisation vous montre le moment où les utilisateurs affectés à un projet se sont connectés à Workfront, ont modifié l’état de la tâche dans ce projet et ont terminé les tâches dans ce projet. L’interaction avec la visualisation vous permet d’afficher ces détails pour chaque utilisateur. Vous pouvez également afficher des dates spécifiques pour ces actions, ainsi que le nombre de fois où chaque action a été terminée.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/project-treemap-overview.md" class="MCXref xref">Visualisation du graphique Treemap du projet dans les analyses améliorées</a> </td> 
   <td> <p>La variable <b>Treemap du projet</b> la visualisation vous montre le temps passé sur certains projets par rapport à d’autres. L’interaction avec la visualisation vous donne des détails sur la condition du projet, la fin prévue du projet et la fin réelle du projet.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/activity-by-team-overview.md" class="MCXref xref">Visualisation de l’activité par équipe dans les analyses améliorées</a> </td> 
   <td> <p>La variable <b>Activité par équipe</b> la visualisation vous montre la carte thermique des utilisateurs d’une équipe d’accueil connectés à Workfront, ayant modifié l’état d’une tâche et terminé une tâche. L’interaction avec la visualisation vous permet d’afficher ces détails pour chaque utilisateur. Vous pouvez également afficher des dates spécifiques pour ces actions, ainsi que le nombre de fois où chaque action a été terminée.</p> </td> 
  </tr> 
  <!-- Features permanently removed from Workfront
  <tr> 
   <td><a href="../enhanced-analytics/resource-capacity-overview.md" class="MCXref xref">View the Resource capacity visualization in Enhanced analytics</a> </td> 
   <td> <p>The <b>Resource capacity</b> visualization shows you which home teams have the capacity to take on more work and which home teams have more work assigned to them than they can complete. Interacting with the visualization allows you to see more details about work completed and available hours for more work.&nbsp;Selecting a team opens the Team capacity visualization.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/team-capacity-overview.md" class="MCXref xref">View the Team capacity visualization in Enhanced analytics</a> </td> 
   <td> <p>The <b>Team capacity</b> visualization shows you a percentage of the amount of work a home team has completed out of the amount of work assigned to them. Interacting with the visualization allows you to see scheduled hours and planned hours for a specific date, as well as the capacity percentage and whether the home team was over, under, or at capacity on that day.</p> </td> 
  </tr>--> 
 </tbody> 
</table>
