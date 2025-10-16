---
product-area: reporting
navigation-topic: reporting-elements
title: Utiliser la vue Jalon
description: Vous pouvez appliquer la vue Jalon à une liste de projets ou à un rapport. Vous pouvez utiliser la vue Jalon pour afficher tous les jalons associés aux tâches dans les projets que vous consultez.
author: Courtney, Alina
feature: Reports and Dashboards
exl-id: c55e53b5-5559-4b6a-a8d7-5028be6af30f
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '1623'
ht-degree: 56%

---

# Utiliser la vue Jalon

<!-- Audited: 11/2024 -->

<!--remove Preview and Production mentions from the article when this comes out live-->

<div class="preview">

Les informations surlignées sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de manière générale. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Les mêmes fonctionnalités seront également disponibles dans l’environnement de production pour tous les clients et clientes à partir d’une semaine à compter de la version préliminaire.

Pour plus d’informations, voir [Modernisation des interfaces](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).

</div>

Vous pouvez appliquer la vue Jalon à une liste de projets ou à un rapport. Vous pouvez utiliser la vue Jalon pour afficher tous les jalons associés aux tâches dans les projets que vous consultez.

Pour pouvoir utiliser la vue Jalon , les éléments suivants doivent exister :

* Les chemins jalonnés sont configurés. Pour plus d’informations, voir [Créer un chemin jalonné](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md).
* Les chemins jalonnés nécessaires sont ajoutés aux projets. Pour plus d’informations, voir [Modifier les projets](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md).
* Les jalons sont associés aux tâches. Pour plus d’informations, voir [Associer des jalons à des tâches](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

La vue Jalon est disponible lors de l’affichage d’une liste de projets ou d’un rapport de projet. Les sections suivantes décrivent la manière d’afficher et d’utiliser la vue Jalon.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</strong></td> 
   <td> 
    <p>Standard</p>
    <p>Travail ou supérieur</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès en affichage ou supérieur aux rapports, au tableau de bord et aux calendriers</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
    <td> <p>Autorisations d’affichage d’un rapport de projet pour appliquer la vue Jalon à un rapport</p></td> 
   </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Basculer vers la vue Jalon {#switch-to-the-milestone-view}

{{step1-to-projects}}

1. Cliquez sur le menu déroulant **Vue**, puis cliquez sur **Jalon**.

   La liste ou le rapport s’affiche dans une vue Jalon.

   Pour plus d’informations sur la vue Jalon, voir la section [Vue d’ensemble de la vue Jalon](#milestone-view-overview) dans cet article.

## Vue d’ensemble de la vue Jalon {#milestone-view-overview}

<div class="preview">

La vue Jalon est disponible dans les listes de projets et les rapports de projet. Vous pouvez afficher rapidement tous les jalons associés aux tâches dans les projets que vous consultez.

![Projet avec vue Jalon](assets/project-with-milestone-view-with-complete.png)

</div>

>[!NOTE]
>
>La vue Jalon n’est pas disponible dans les zones suivantes :
>
>* Feuilles de temps, dans la liste des projets lors de l’ajout d’un projet.

Pour plus d’informations sur la façon de basculer vers la vue Jalon, voir la section [Basculer vers la vue Jalon](#switch-to-the-milestone-view) dans cet article.


### Sections de la vue Jalon

Lors de l’application de la vue Jalon à une liste de projets, les projets s’affichent dans les sections suivantes :

* Les projets associés à un chemin jalonné s’affichent en premier, répertoriés sous le nom de leurs chemins jalonnés respectifs.

  Workfront trie les projets de la première section selon les critères suivants, dans cet ordre :

   1. ID de chemin jalonné. Vous pouvez afficher l’ID de chemin jalonné dans un rapport Chemin jalonné.

   2. Champ sélectionné comme premier champ de tri pour la liste des projets dans la vue précédemment appliquée à la liste des projets, avant de sélectionner la vue Jalon.

* Les projets qui ne sont pas associés à un chemin jalonné s’affichent ensuite, dans la section Non attribué. Workfront trie les projets de la section Non attribué en fonction du champ sélectionné comme premier champ de tri pour la liste des projets dans la vue précédemment appliquée à la liste des projets, avant de sélectionner la vue Jalon.

### Informations sur le projet dans la vue Jalon

Lors de l’affichage d’une liste de projets ou d’un rapport de projet dans la vue Jalon, les informations suivantes sont disponibles :

* **Dates prévues ou dates prévisionnelles :** indiquez si vous souhaitez afficher les dates prévues ou les dates prévisionnelles dans la vue Jalon.\
  Les dates de début et de fin du projet, ainsi que d&#39;achèvement de chaque tâche jalonnée du chemin jalonné, s&#39;affichent.

  Si vous consultez les dates prévues, elles ne peuvent pas être modifiées. Les dates prévues sont calculées par Workfront et ne peuvent pas être modifiées manuellement.

  Si vous consultez les dates prévues et que vous disposez également d’un accès de niveau Gérer au projet, vous pouvez modifier les dates suivantes directement à partir de la vue Jalon :

   * **Dates de début du projet :** si un projet est planifié à partir de la date de début, vous pouvez modifier manuellement la date de début planifiée du projet, puis la date d’achèvement planifiée est calculée.
   * **Dates d’achèvement du projet :** si un projet est planifié à partir de la date d’achèvement prévue, vous pouvez modifier manuellement la date d’achèvement prévue du projet, puis la date de début prévue est calculée.
   * **Dates d’achèvement de la tâche :** vous pouvez mettre à jour manuellement la date d’achèvement prévue des tâches directement à partir de la vue Jalon.

* **Pourcentage terminé :** affiche le pourcentage d’achèvement de chaque tâche et projet.

  Vous pouvez désactiver l’affichage du pourcentage d’achèvement, comme décrit dans la section [Configurer les informations affichées dans la vue Jalon](#configure-what-information-displays-in-the-milestone-view) dans cet article.

  Vous pouvez ajuster le pourcentage d’achèvement directement à partir de la vue Jalon, comme décrit dans la section [Ajuster le pourcentage terminé pour les tâches dans la vue Jalon](#adjust-percent-complete-for-tasks-in-the-milestone-view) dans cet article.

* **Icônes de statut d’avancement de la tâche :** selon l’environnement utilisé pour afficher la vue jalon, les icônes suivantes indiquent le statut d’avancement de la tâche :

   * Dans l’environnement de production, les icônes de statut suivantes s’affichent en regard de chaque projet et tâche dans la vue Jalon :

      * À l’heure\
        ![Icône Heure d’activation](assets/gantt-ontime.png)

      * En retard\
        ![Icône Derrière](assets/gantt-behind.png)

      * En danger\
        ![ Icône En danger ](assets/gantt-atrisk.png)

      * En retard\
        ![Icône de retard](assets/gantt-late.png)

     <!--get new screen shots or hide them for preview or production - could not display all in devtest; idea: use color dots from Task Details tab - New status is blue; Some concerns condition is yellow etc-->

  <div class="preview">

   * Dans l’environnement de prévisualisation, les cercles colorés suivants s’affichent en regard de chaque projet et tâche dans la vue Jalon :

      * À l’heure - vert
      * Derrière - jaune
      * À risque - bleu
      * En retard - rouge

  </div>

  Vous pouvez désactiver l’affichage de ces icônes de statut, comme décrit dans cet article à la section [Configurer les informations qui s’affichent dans la vue « Jalon »](#configure-what-information-displays-in-the-milestone-view).

  Pour plus d’informations sur chaque type de statut, consultez l’article [Vue d’ensemble du statut de progression de la tâche](../../../manage-work/tasks/task-information/task-progress-status.md).

* **Ombrage du statut de la tâche pour les tâches terminées** : une fois qu’une tâche est marquée comme terminée, l’arrière-plan de la tâche est ombré dans la vue « Jalon » pour indiquer si la tâche a été terminée à l’heure ou en retard :

   * **Ombrage rouge de la colonne de la tâche** : l’arrière-plan d’une tâche est rouge lorsque le statut de progression est **En retard**.

   * **Ombrage vert de la colonne de la tâche** : l’arrière-plan d’une tâche est vert lorsque le statut de progression est **À l’heure**.

* **Ombrage du statut du projet pour les colonnes « Début » et « Fin » du projet** :

   * **Colonne « Début » du projet** : l’arrière-plan de la colonne « Début » du projet est rouge ou vert uniquement lorsque la date de début effectif est renseignée :

      * **Ombrage rouge de la colonne « Début » du projet** : l’arrière-plan de la colonne « Début » du projet est rouge lorsque le statut de progression du projet est **En retard**.

      * **Ombrage vert pour la colonne « Début » du projet** : l’arrière-plan de la colonne « Début » du projet est vert lorsque le statut de progression du projet est **À l’heure**.

     >[!TIP]
     >
     >Vous devez accéder à la page Détails du projet pour afficher la date de début effective du projet.

   * **Colonne d’achèvement du projet** : l’arrière-plan de la colonne d’achèvement du projet est rouge ou vert uniquement lorsque la date d’achèvement est renseignée :

      * **Ombrage rouge pour la colonne d’achèvement du projet** : l’arrière-plan de la colonne d’achèvement du projet est rouge lorsque le statut de progression du projet est **En retard**.

      * **Ombrage vert de la colonne d’achèvement du projet** : l’arrière-plan de la colonne d’achèvement du projet est vert lorsque le statut de progression du projet est **À l’heure**.

     >[!TIP]
     >
     >Vous devez accéder à la page Détails du projet pour afficher la date d&#39;achèvement effective du projet.

   * Aucune couleur d’ombrage n’est attribuée aux colonnes « Début » et « Achèvement » lorsque le statut de progression des tâches est « En danger » ou « En retard ».

  <!--add new screen shot for preview or production release; logged a bug as this is not happening in the new view - if at prod this is still missing, hide this screen shot-->

  ![Vue jalonnée avec ombrage](assets/milestone-view-with-shading.png)

* **Nom du projet** : le nom du projet s’affiche avec un lien vers le projet.
* **Icône Statut du projet** : selon l’environnement auquel vous accédez à la vue Jalon, les indicateurs suivants affichent le statut du projet :

   * Dans l’environnement de production , une icône s’affiche en regard du nom du projet, indiquant la condition du projet. Le statut du projet peut être l&#39;un des suivants :

      * Dans les temps
      * En danger
      * En difficulté

  <div class="preview">

   * Dans l’environnement de Prévisualisation, une icône de condition sous la forme d’un cercle coloré s’affiche en regard de chaque projet. Les conditions possibles du projet et les couleurs du cercle sont les suivantes :

      * Dans les temps - vert
      * À risque - jaune
      * En difficulté - rouge

     </div>


## Configurer les informations à afficher dans la vue jalonnée {#configure-what-information-displays-in-the-milestone-view}

Vous pouvez configurer l’affichage des éléments suivants dans la vue jalonnée :

* Icônes du statut de la progression
* Pourcentage d’achèvement des projets et des tâches

Par défaut, les icônes de statut de progression et le pourcentage d&#39;achèvement des projets et des tâches s&#39;affichent.

Les modifications que vous apportez à ces options s’appliquent uniquement à vous ; elles ne s’appliquent pas aux autres utilisateurs et utilisatrices. Les modifications que vous apportez sont conservées la prochaine fois que vous vous connectez à Workfront.

Pour configurer si les icônes de statut du projet et du pourcentage d’achèvement des projets s’affichent, procédez comme suit :

{{step1-to-projects}}

1. Cliquez sur le bouton **Affichage**, puis cliquez sur **Jalon**.

1. Dans l’environnement de production, cliquez sur **Options** dans le coin supérieur droit de la vue Jalon, puis sélectionnez l’une des options de l’étape suivante.

   ![milestone_view_options.png](assets/milestone-view-options-350x141.png)

   <div class="preview">Dans l’environnement de Prévisualisation, sélectionnez l’une des options de l’étape suivante, dans le coin supérieur droit de la vue Jalon .</div>

   <!--at Production release, replace this screen shot and adjust the Production/ Preview text above-->


1. Sélectionnez l’une des options suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Statut de progression</td> 
      <td> <p>Sélectionnez cette option pour afficher les icônes de statut de la progression à côté de chaque projet et tâche.</p> <p>Cette option est activée par défaut.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Pourcentage d’achèvement</td> 
      <td> <p>Sélectionnez cette option pour afficher le pourcentage d’achèvement à côté de chaque projet et tâche.</p> <p>Cette option est activée par défaut.</p> </td> 
     </tr> 
    </tbody> 
   </table>

## Ajuster le pourcentage d’achèvement pour les tâches dans la vue jalonnée {#adjust-percent-complete-for-tasks-in-the-milestone-view}

Vous pouvez ajuster le pourcentage d’achèvement pour les tâches dans la vue jalonnée. Vous ne pouvez pas ajuster le Pourcentage terminé pour une tâche parent (une tâche qui contient des sous-tâches) ou pour un projet.

Pour ajuster le pourcentage d’achèvement d’une tâche dans la vue jalonnée, procédez comme suit :

{{step1-to-projects}}

1. Cliquez sur le menu déroulant **Affichage**, puis cliquez sur **Jalon**.

1. (Conditionnel) Si les pourcentages d&#39;achèvement ne sont pas affichés actuellement dans la vue Jalon, activez l&#39;affichage du Pourcentage d&#39;achèvement des tâches et des projets, comme décrit dans la section [Configurer les informations affichées dans la vue Jalon](#configure-what-information-displays-in-the-milestone-view) de cet article.

1. Dans l’environnement de production, cliquez sur le pourcentage d’achèvement sous une tâche, spécifiez un nouveau pourcentage, puis appuyez sur Entrée.

   <div class="preview">Dans l’environnement de Prévisualisation, déplacez la diapositive Pourcentage terminé vers le nouveau Pourcentage terminé pour la mettre à jour. </div>
