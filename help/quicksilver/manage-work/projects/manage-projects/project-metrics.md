---
content-type: overview;how-to-procedural
product-area: projects
keywords: analytics,metrics,project,advanced,tasks,assignee,complete,status,pending,prochain
navigation-topic: manage-projects
title: Présentation des mesures de projet
description: Les mesures de projet vous donnent une visualisation de ce qui se passe dans un projet, ce qui vous permet d’évaluer rapidement les besoins et l’état d’un projet. Découvrez comment interpréter la zone Mesures dans le panneau de gauche d’un projet.
author: Alina
feature: Work Management
exl-id: 54c2a59d-9f6b-4126-9526-5169aeda8517
source-git-commit: 24cc3ece515fd778a9bc9e8afbcd534f48b24230
workflow-type: tm+mt
source-wordcount: '1275'
ht-degree: 0%

---

# Présentation des mesures de projet

Les mesures de projet vous donnent une vue d’ensemble au format graphique des performances d’un projet.

## Exigences d’accès

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Workfront*</td> 
   <td> <p>Révision ou version ultérieure </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Niveau d’accès*</td> 
   <td> <p>Affichage de l’accès aux projets</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur l’accès aux projets, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Accorder l’accès aux projets</a>. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>. </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Affichage des autorisations d’un projet</p> <p> Pour plus d’informations sur les autorisations de projet, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Partage d’un projet dans Adobe Workfront</a>.</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Conditions préalables

Pour accéder à la zone Mesures à partir du panneau de gauche d’un projet, vous devez :

* Activez l’option Mesures du panneau de gauche dans la zone Projets de votre modèle de mise en page.

   Pour savoir comment un administrateur Workfront ou un administrateur de groupe peut personnaliser le panneau de gauche avec un modèle de mise en page, voir [Personnalisation du panneau de gauche à l’aide d’un modèle de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md).

## Présentation de la zone Mesures du projet

Les mesures de projet vous donnent une visualisation de ce qui se passe dans un projet, ce qui vous permet d’évaluer rapidement les besoins et l’état d’un projet.

![](assets/project-metrics-full-screen-350x238.png)

Dans la zone Mesures , vous pouvez consulter l’intégrité globale d’un projet, ainsi que :

* Où le travail est principal ou bloqué
* Qui a des tâches ouvertes qui lui sont affectées
* Détails sur les tâches ou les problèmes en retard ou proches de la date d’achèvement planifiée

Vous pouvez également consulter chaque graphique pour examiner de plus près les tâches ou les problèmes d’une catégorie spécifique.

Pour en savoir plus sur ces tâches ou problèmes, voir [Afficher les détails des mesures](#view-metrics-details).

>[!TIP]
>
>Pour afficher les mesures à un niveau supérieur pour un groupe de projets au sein d’un programme, d’un portefeuille, etc., accédez à la zone Analyses améliorées.\
>Pour en savoir plus sur les analyses améliorées, voir [Présentation des analyses améliorées](../../../enhanced-analytics/enhanced-analytics-overview.md).

## IPC de projet

Les indicateurs de performances clés (IPC) s’affichent en haut de la zone Mesures.

![](assets/project-metrics-kpis-350x52.png)

Ces indicateurs de performance clés sont répartis dans les catégories suivantes :

| Tâches terminées | **Tâches terminées** affiche le nombre de tâches dont l’état est Terminé. Ce nombre inclut également les tâches dont l’état personnalisé est égal à Complete. |
|---|---|
| Tâches incomplètes | **Tâches incomplètes** affiche le nombre de tâches qui ne sont pas à l’état Terminé ou Fermé ou dont l’état est égal à Terminé. |
| Tâches en retard | **Tâches en retard** affiche le nombre de tâches dépassant la date d’achèvement planifiée et ne présentant pas l’état Terminé ou Fermé ou un état correspondant à Terminé ou Fermé. |
| Tâches totales | **Tâches totales** affiche le nombre total de tâches dans le projet. |

>[!TIP]
>
>Pour afficher une liste des tâches d’un indicateur de performance clé spécifique, cliquez sur ce dernier. Dans cette liste, vous pouvez cliquer sur une tâche spécifique pour afficher plus de détails dans un nouvel onglet.\
>![](assets/completed-tasks-dialog-350x75.png)\
>Pour plus d’informations, voir [Afficher les détails des mesures](#view-metrics-details).

## Graphique à barres de tâches ou de problèmes

Dans le graphique à barres qui s’affiche sous les indicateurs de performance clés du projet, vous pouvez consulter l’état ou la priorité des tâches du projet. La vue Tâche est sélectionnée par défaut.

Lorsque l’état est sélectionné dans ce graphique, vous pouvez afficher tous les états des tâches ou des problèmes d’un projet. Chaque état est regroupé dans une barre du graphique. Tous les états système par défaut et les états personnalisés s’affichent dans ce graphique.

![](assets/project-metrics-task-issue-by-status-350x120.png)

Lorsque la priorité est sélectionnée dans ce graphique, vous pouvez afficher toutes les priorités des tâches ou des problèmes d’un projet.

![](assets/project-metrics-task-issue-by-priority-350x121.png)

>[!TIP]
>
>Pour afficher la liste des tâches ayant un état ou une priorité spécifique, cliquez sur une barre du graphique. Dans cette liste, vous pouvez cliquer sur une tâche spécifique pour afficher plus de détails dans un nouvel onglet.\
>![](assets/completed-tasks-dialog-350x75.png)\
>Pour plus d’informations, voir [Afficher les détails des mesures](#view-metrics-details).

## Graphique en anneau

Le graphique en anneau situé sous les indicateurs de performance clés du projet vous permet de consulter le rapport entre les tâches terminées et les tâches incomplètes dans un projet.

![](assets/tasks-issues-by-complete-status-350x250.png)

Dans le menu déroulant situé au-dessus du graphique, vous pouvez sélectionner :

| Toutes les tâches | Sélection **tâches** affiche le nombre total de tâches dans le projet, ainsi que le rapport entre les tâches terminées et incomplètes. |
|---|---|
| Tous les problèmes | Sélection **Problèmes** vous indique le nombre total de problèmes dans le projet, ainsi que le rapport entre les problèmes terminés et incomplets. |

>[!TIP]
>
>Pour afficher la liste des tâches terminées ou incomplètes, cliquez sur cette section dans le graphique en anneau. Dans cette liste, vous pouvez cliquer sur une tâche spécifique pour afficher plus de détails dans un nouvel onglet.\
>![](assets/completed-tasks-dialog-350x75.png)\
>Pour plus d’informations, voir [Afficher les détails des mesures](#view-metrics-details).

## Graphique à barres cessionnaire

Le graphique à barres représentant les personnes désignées indique le nombre de tâches affectées à chaque personne du projet. Ce nombre varie en fonction de la catégorie sélectionnée dans le menu déroulant.

![](assets/tasks-issues-by-assignee-350x104.png)

Vous pouvez choisir de consulter les affectations de tâches pour un projet dans les catégories suivantes :

| Terminé | Sélection **Terminer** indique le nombre de tâches affectées à chaque utilisateur ayant été terminées. |
|---|---|
| Incomplet | Sélection **Incomplet** indique le nombre de tâches affectées à chaque utilisateur qui n’ont pas encore été terminées. |
| À venir | Sélection **À venir** affiche le nombre de tâches affectées à chaque utilisateur qui n’ont pas encore atteint la date de début planifiée. |
| Échu | Sélection **En retard** indique le nombre de tâches affectées à chaque utilisateur qui ont dépassé la date d’achèvement planifiée et n’ont pas encore été terminées. |

>[!TIP]
>
>Pour afficher la liste des tâches de la catégorie sélectionnée qui sont affectées à un utilisateur spécifique, cliquez sur la barre en regard de son nom dans le graphique. Dans cette liste, vous pouvez cliquer sur une tâche spécifique pour afficher plus de détails dans un nouvel onglet.\
>![](assets/completed-tasks-dialog-350x75.png)\
>Pour plus d’informations, voir [Afficher les détails des mesures](#view-metrics-details).

## Afficher les détails des mesures {#view-metrics-details}

Vous pouvez interagir avec les graphiques de la zone Mesures pour examiner différents aspects d’un graphique ou examiner de plus près les tâches et les problèmes d’un graphique.

1. Accédez au projet pour lequel vous souhaitez afficher les mesures.
1. Dans le panneau de gauche, cliquez sur **Afficher plus** pour afficher d’autres sections, puis cliquez sur **Mesures**.\
   Les graphiques de la zone Mesures affichent par défaut des informations relatives aux tâches.\
   ![](assets/metrics-section-350x298.png)

1. (Conditionnel) Si une flèche de liste déroulante s’affiche sur un graphique, cliquez sur le bouton **Flèche de liste déroulante** icon ![](assets/dropdown-arrow.png) sur le graphique et sélectionnez l’option de votre choix dans le menu.\
   Pour plus d&#39;informations sur les options qui apparaissent dans les menus de chaque graphique, reportez-vous à la section correspondante ci-dessus.

1. (Facultatif) Pour examiner de plus près les tâches ou les problèmes d’une mesure de la page, procédez comme suit :

   1. Cliquez sur l’élément (tâches affectées à un utilisateur spécifique, problèmes avec une priorité élevée ou toutes tâches en retard) pour lequel vous souhaitez afficher des détails.

      Une liste de tâches ou de problèmes s’affiche.

      ![](assets/completed-tasks-dialog-350x75.png)

   1. Utilisez les flèches au bas de la liste pour localiser la tâche ou le problème à examiner.

      Ou

      Sélectionnez un nombre spécifique pour afficher les tâches ou les problèmes sur une page spécifique.

      ![](assets/pagination-300x152.png)

   1. Sélectionnez une tâche ou un problème pour afficher plus de détails.

      La tâche ou le problème s’ouvre dans un nouvel onglet.

1. (Facultatif) Pour exporter le tableau de bord des mesures du projet vers un fichier .png, cliquez sur le bouton **Exporter** icon ![](assets/export.png), puis sélectionnez **Exporter au format PNG** dans le menu déroulant.

   >[!TIP]
   >
   >Lorsque vous exportez le tableau de bord, le fichier exporté n’inclut que ce qui s’affiche actuellement dans la fenêtre d’affichage. Pour inclure certains éléments dans le fichier exporté, vous devrez peut-être faire défiler la page vers le haut ou vers le bas ou ajuster les paramètres de zoom de votre navigateur.
