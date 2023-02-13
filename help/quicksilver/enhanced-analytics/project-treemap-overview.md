---
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
title: Visualisation du graphique Treemap du projet dans les analyses améliorées
description: La visualisation du graphique Treemap du projet est une vue des heures (ou des jours) qui ont été travaillées dans une fenêtre de temps spécifique par rapport à d’autres tâches de taille. Cela vous aide à comprendre le temps que les gens ont consacré à un projet.
author: Nolan
feature: Reports and Dashboards
exl-id: 6216465e-c3bb-4f2f-b71c-766ad0c2ed40
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '858'
ht-degree: 1%

---

# Visualisation du graphique Treemap du projet dans les analyses améliorées

La visualisation du graphique Treemap du projet est une vue des heures (ou des jours) qui ont été travaillées dans une fenêtre de temps spécifique par rapport à d’autres tâches de taille. Cela vous aide à comprendre le temps que les gens ont consacré à un projet.

![](assets/project-treemap-350x126.png)

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

## Présentation de la visualisation du graphique Treemap du projet

Les zones de la visualisation du graphique Treemap du projet représentent les projets et la taille des zones montre une comparaison du temps passé sur différents projets. Plus la boîte est grande, plus le temps passé sur le projet est important.

La visualisation du graphique Treemap du projet se compose des éléments suivants :

* **Boîtes bleues plus petites**: Les projets qui comportent moins d’heures (ou de jours) s’affichent sous forme de petites zones de couleur bleu clair.

   ![](assets/project-treemap-smaller-box.png)

* **Boîtes bleues foncées plus grandes**: Les projets qui comportent plus d’heures (ou de jours) s’affichent sous forme de zones plus grandes avec une couleur bleu foncé.

   ![](assets/project-treemap-larger-box-350x205.png)

* **Boîtes de taille moyenne, bleues**: Les projets qui se situent entre les deux catégories s’affichent sous forme de zones de taille moyenne avec une nuance de bleu entre le bleu foncé et le bleu clair. Les boîtes de taille moyenne peuvent présenter 3 nuances de bleu.

La légende sur le côté droit affiche une répartition des heures terminées pour chaque nuage de bleu. Cette légende est dynamique et se met à jour en fonction des données.

![](assets/project-treemap-hours-completed.png)

>[!NOTE]
>
>Si vous observez la visualisation du graphique Treemap du projet par durée plutôt que par heures planifiées, cette légende présente une ventilation des jours travaillés pour chaque nuage de bleu.\
>![](assets/project-treemap-days-worked.png)>

L’affichage de ces informations vous permet de déterminer les éléments suivants :

* La priorité des tâches en cours de traitement au cours de la période sélectionnée.
* Sur quoi les équipes passent du temps ?
* Si les équipes se concentrent sur les bonnes choses.
* Lorsqu’un utilisateur clique sur un projet spécifique, la portée d’un projet a changé au cours de cette période.

Pour savoir comment obtenir les meilleures données pour cette visualisation, voir [Présentation des analyses améliorées](../enhanced-analytics/enhanced-analytics-overview.md).

## Visualisation du graphique Treemap du projet

1. Cliquez sur l’icône du menu principal ![](assets/main-menu-icon-16x12.png), puis sélectionnez **Analytics**.
1. (Facultatif) Pour utiliser une autre période, sélectionnez de nouvelles dates de début et de fin dans le filtre de période.

   ![](assets/filters-select-date-range-350x344.png)

   Pour plus d’informations sur l’utilisation du filtre de période, voir [Application de filtres dans les analyses améliorées](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Conditionnel) Si vous devez limiter l’ensemble de données du projet, sélectionnez les filtres à utiliser et appliquez-les.

   Pour plus d’informations sur l’ajout de filtres dans les analyses améliorées, voir [Application de filtres dans les analyses améliorées](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Une fois que vous avez ajouté des filtres, les données de 50 projets au maximum s’affichent et les filtres restent principaux même après avoir quitté la page ou vous être déconnecté de Workfront.

1. (Facultatif) Pour modifier le mode de tri des projets, cliquez sur le bouton **Tri par** dans le coin supérieur droit de la visualisation du graphique Treemap du projet, puis sélectionnez une nouvelle option de tri :

   * **A - Z**
   * **Z - A**
   * **Date d’achèvement prévue**
   * **Date de début prévue**

   Toutes les autres visualisations de la page sont mises à jour pour correspondre à votre sélection de tri.

1. (Conditionnel) S’il existe plus de 50 projets dans votre jeu de données, utilisez les flèches situées dans le coin inférieur gauche de la visualisation pour passer d’un groupe de 50 projets à un autre.

   Toutes les autres visualisations de la page sont mises à jour pour correspondre à votre sélection de page.

   ![](assets/pagination-350x118.png)

1. (Facultatif) Modifiez la vue à partir de **heures planifiées** to **durée**.

   Les heures planifiées sont sélectionnées par défaut.

1. Passez la souris sur un projet pour afficher la condition du projet, ainsi que le nombre total d’heures planifiées, le nombre total d’heures terminées et le nombre moyen d’heures passées sur le projet par jour.

   ![](assets/project-treemap-project-details-350x404.png)

   >[!NOTE]
   >
   >Si vous avez sélectionné la variable **durée** vous verrez les détails de durée suivants :
   >
   >* **Période planifiée**: Nombre de jours prévus pour terminer le projet.
   >* **Jours de travail**: La durée planifiée pour chaque tâche qui a été complétée au cours de la période sélectionnée en haut, divisée par le nombre d’heures par jour.

   >   
   >![](assets/duration-treemap-350x159.png)
   >
   >Pour plus d’informations sur la durée, voir la section &quot;Vue Durée&quot; dans [Présentation des analyses améliorées](../enhanced-analytics/enhanced-analytics-overview.md).

1. (Facultatif) Pour exporter les données de visualisation, cliquez sur le bouton **Icône Exporter** ![](assets/export.png) dans le coin supérieur droit de la visualisation, sélectionnez le format d’exportation :

   * **Graphique (PNG)**
   * **Tableau de données (XSLX)**

1. Cliquez sur un projet pour ouvrir les visualisations de Burndown et Tasks in flight afin de mieux comprendre comment les tâches et les heures (ou jours) ont contribué à la taille d’un projet.

Pour plus d’informations sur la visualisation de Burndown, voir [Affichage de la visualisation de Burndown dans les analyses améliorées](../enhanced-analytics/burndown-overview.md). Pour plus d’informations sur les tâches dans la visualisation en vol, voir [Affichage des tâches dans la visualisation en vol dans Enhanced Analytics](../enhanced-analytics/tasks-in-flight-overview.md).

