---
content-type: overview;how-to-procedural
product-area: projects
keywords: analytics,metrics,project,advanced,tasks,assignee,complete,status,pending,prochain
navigation-topic: manage-projects
title: Vue d’ensemble des mesures du projet
description: Les mesures de projet vous donnent une visualisation de ce qui se passe dans un projet, ce qui vous permet d’évaluer rapidement les besoins et l’état d’un projet. Découvrez comment interpréter la zone Mesures dans le panneau de gauche d’un projet.
author: Alina
feature: Work Management
exl-id: 54c2a59d-9f6b-4126-9526-5169aeda8517
source-git-commit: 24cc3ece515fd778a9bc9e8afbcd534f48b24230
workflow-type: tm+mt
source-wordcount: '1266'
ht-degree: 8%

---

# Vue d’ensemble des mesures du projet

Les mesures de projet vous donnent une vue d’ensemble au format graphique des performances d’un projet.

## Conditions d’accès

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan Workfront*</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Workfront*</td> 
   <td> <p>Révision ou supérieur </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Niveau d’accès*</td> 
   <td> <p>Affichage de l’accès aux projets</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur l’accès aux projets, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Accorder l’accès aux projets</a>. Pour plus d’informations sur la façon dont un administrateur ou une administratrice de Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>. </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Affichage des autorisations d’un projet</p> <p> Pour plus d’informations sur les autorisations de projet, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Partager un projet dans Adobe Workfront</a>.</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

* Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Conditions préalables

Pour accéder à la zone Mesures à partir du panneau de gauche d’un projet, vous devez :

* Activez l’option Mesures du panneau de gauche dans la zone Projets de votre modèle de mise en page.

  Pour savoir comment un administrateur Workfront ou un administrateur de groupe peut personnaliser le panneau de gauche avec un modèle de mise en page, voir [ Personnalisation du panneau de gauche à l’aide d’un modèle de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md).

## Présentation de la zone Mesures du projet

Les mesures de projet vous donnent une visualisation de ce qui se passe dans un projet, ce qui vous permet d’évaluer rapidement les besoins et l’état d’un projet.

![](assets/project-metrics-full-screen-350x238.png)

Dans la zone Mesures , vous pouvez consulter l’intégrité globale d’un projet, ainsi que :

* Emplacement où le travail est actif ou bloqué
* Qui a des tâches ouvertes qui lui sont affectées
* Détails sur les tâches ou les problèmes en retard ou proches de la date d’achèvement planifiée

Vous pouvez également consulter chaque graphique pour examiner de plus près les tâches ou les problèmes d’une catégorie spécifique.

Pour en savoir plus sur l’analyse de ces tâches ou problèmes, voir [Affichage des détails des mesures](#view-metrics-details).

>[!TIP]
>
>Pour afficher les mesures à un niveau supérieur pour un groupe de projets au sein d’un programme, d’un portefeuille, etc., accédez à la zone Analyses améliorées.\
>Pour en savoir plus sur l’analyse améliorée, consultez la [présentation de l’analyse améliorée](../../../enhanced-analytics/enhanced-analytics-overview.md).

## IPC de projet

Les indicateurs de performances clés (IPC) s’affichent en haut de la zone Mesures.

![](assets/project-metrics-kpis-350x52.png)

Ces indicateurs de performance clés sont répartis dans les catégories suivantes :

| Tâches terminées | **Tâches terminées** affiche le nombre de tâches dont l’état est Terminé. Ce nombre inclut également les tâches dont l’état personnalisé est égal à Complete. |
|---|---|
| Tâches incomplètes | **Tâches incomplètes** affiche le nombre de tâches qui ne sont pas dans un état Terminé ou Fermé ou un état qui correspond à Terminé. |
| Tâches en retard | **Tâches en retard** affiche le nombre de tâches dépassant la date d’achèvement planifiée et n’ayant pas le statut Terminé ou Fermé ou dont l’état est Terminé ou Fermé. |
| Tâches totales | **Total des tâches** affiche le nombre total de tâches dans le projet. |

>[!TIP]
>
>Pour afficher une liste des tâches d’un indicateur de performance clé spécifique, cliquez sur ce dernier. Dans cette liste, vous pouvez cliquer sur une tâche spécifique pour afficher plus de détails dans un nouvel onglet.\
>![](assets/completed-tasks-dialog-350x75.png)\
>Pour plus d’informations, voir [Afficher les détails des mesures](#view-metrics-details).

## Graphique de la barre de tâches ou de problèmes

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

| Toutes les tâches | La sélection de **tâches** vous indique le nombre total de tâches dans le projet, ainsi que le rapport entre les tâches terminées et incomplètes. |
|---|---|
| Tous les problèmes | La sélection de **problèmes** vous indique le nombre total de problèmes dans le projet, ainsi que le rapport entre les problèmes terminés et incomplets. |

>[!TIP]
>
>Pour afficher la liste des tâches terminées ou incomplètes, cliquez sur cette section dans le graphique en anneau. Dans cette liste, vous pouvez cliquer sur une tâche spécifique pour afficher plus de détails dans un nouvel onglet.\
>![](assets/completed-tasks-dialog-350x75.png)\
>Pour plus d’informations, voir [Afficher les détails des mesures](#view-metrics-details).

## Graphique à barres cessionnaire

Le graphique à barres représentant les personnes désignées indique le nombre de tâches affectées à chaque personne du projet. Ce nombre varie en fonction de la catégorie sélectionnée dans le menu déroulant.

![](assets/tasks-issues-by-assignee-350x104.png)

Vous pouvez choisir de consulter les affectations de tâches pour un projet dans les catégories suivantes :

| Terminé | La sélection de **Terminé** indique le nombre de tâches affectées à chaque utilisateur ayant été terminées. |
|---|---|
| Incomplet | La sélection de **Incomplet** indique le nombre de tâches affectées à chaque utilisateur qui n’ont pas encore été terminées. |
| À venir | La sélection de **Prochaine** indique le nombre de tâches affectées à chaque utilisateur qui n’ont pas encore atteint la date de début planifiée. |
| Échu | La sélection de **Overdue** indique le nombre de tâches affectées à chaque utilisateur qui ont dépassé la date planifiée d’achèvement et n’ont pas encore été terminées. |

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

1. (Conditionnel) Si une flèche de liste déroulante s’affiche sur un graphique, cliquez sur l’icône **Flèche de liste déroulante** ![](assets/dropdown-arrow.png) du graphique et sélectionnez l’option de votre choix dans le menu.\
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

1. (Facultatif) Pour exporter le tableau de bord des mesures du projet vers un fichier .png, cliquez sur l’icône **Exporter** ![](assets/export.png), puis sélectionnez **Exporter en tant que PNG** dans le menu déroulant.

   >[!TIP]
   >
   >Lorsque vous exportez le tableau de bord, le fichier exporté n’inclut que ce qui s’affiche actuellement dans la fenêtre d’affichage. Pour inclure certains éléments dans le fichier exporté, vous devrez peut-être faire défiler la page vers le haut ou vers le bas ou ajuster les paramètres de zoom de votre navigateur.
