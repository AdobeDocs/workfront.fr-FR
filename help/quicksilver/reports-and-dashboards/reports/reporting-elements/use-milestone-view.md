---
product-area: reporting
navigation-topic: reporting-elements
title: Utiliser la vue Jalon
description: Vous pouvez appliquer la vue Jalon à une liste de projets ou à un rapport.
author: Nolan
feature: Reports and Dashboards
exl-id: c55e53b5-5559-4b6a-a8d7-5028be6af30f
source-git-commit: 3cee374b68b26f2a423d41101300ec8b6685fadd
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Utiliser la vue Jalon

<!-- Audited: 11/2024 -->

Vous pouvez appliquer la vue Jalon à une liste de projets ou à un rapport.

Avant de pouvoir utiliser la vue de jalon, vous devez configurer les jalons, ajouter les chemins d’accès au jalon aux projets et associer les jalons aux tâches, tel que décrit dans les articles [Créer un chemin jalonné](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md) et [Associer des jalons à des tâches](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

La vue Jalon est disponible lors de l’affichage d’une liste de projets ou d’un rapport de projet. Les sections suivantes décrivent la manière d’afficher et d’utiliser la vue Jalon.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Formule Adobe Workfront</strong></td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licence Adobe Workfront</strong></td> 
   <td> 
      <p>Nouveau :</p>
         <ul>
         <li><p>Standard</p></li>
         </ul>
      <p>Actuel :</p>
         <ul>
         <li><p>Travail ou supérieur</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurations du niveau d’accès*</strong></td> 
   <td> <p>Accès en affichage ou supérieur aux rapports, au tableau de bord et aux calendriers</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet</strong></td> 
   <td> <p>Autorisations d’affichage d’un rapport de projet pour appliquer la vue Jalon à un rapport</p> </td> 
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

La vue Jalon est disponible dans les listes de projets et les rapports de projet. Cette vue vous permet d’afficher rapidement tous les jalons associés aux tâches dans les projets que vous consultez.


>[!NOTE]
>
>La vue Jalon n’est pas disponible dans les zones suivantes :
>
>* Feuilles de temps, dans la liste des projets lors de l’ajout d’un projet.


Pour plus d’informations sur la façon de basculer vers la vue Jalon, voir la section [Basculer vers la vue Jalon](#switch-to-the-milestone-view) dans cet article.

![Projet avec vue Jalon](assets/project-with-milestone-view-with-complete.png)

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
  Les dates s’affichent pour le début et l’achèvement, ainsi que pour chaque jalon dans le chemin jalonné.\
  Si vous affichez les dates prévues et que vous avez également un accès en gestion au projet, vous pouvez modifier les dates suivantes directement à partir de la vue Jalon : (Si vous affichez les dates prévisionnelles, celles-ci ne peuvent pas être modifiées, car les dates prévisionnelles sont calculées et ne peuvent pas être modifiées manuellement.)

   * **Dates de début du projet** si un projet est planifié à partir de la date de début, vous pouvez modifier manuellement la date de début du projet ; la date d’achèvement est ensuite calculée.
   * **Dates d’achèvement du projet :** si un projet est planifié à partir de la date d’achèvement, vous pouvez modifier manuellement la date d’achèvement du projet ; la date de début est ensuite calculée.
   * **Dates d’achèvement de la tâche :** vous pouvez mettre à jour manuellement la date d’achèvement des tâches directement à partir de la vue Jalon.

* **Pourcentage terminé :** affiche le pourcentage d’achèvement de chaque tâche et projet.\
  Vous pouvez désactiver l’affichage du pourcentage d’achèvement, comme décrit dans la section [Configurer les informations affichées dans la vue Jalon](#configure-what-information-displays-in-the-milestone-view) dans cet article.\
  Vous pouvez ajuster le pourcentage d’achèvement directement à partir de la vue Jalon, comme décrit dans la section [Ajuster le pourcentage terminé pour les tâches dans la vue Jalon](#adjust-percent-complete-for-tasks-in-the-milestone-view) dans cet article.

* **Icônes de statut de la tâche :** une icône de statut s’affiche à côté de chaque projet et tâche dans la vue « Jalon ».

   * À l’heure\
     ![](assets/gantt-ontime.png)

   * En retard\
     ![](assets/gantt-behind.png)

   * En danger\
     ![](assets/gantt-atrisk.png)

   * En retard\
     ![](assets/gantt-late.png)

  Vous pouvez désactiver l’affichage de ces icônes de statut, comme décrit dans cet article à la section [Configurer les informations qui s’affichent dans la vue « Jalon »](#configure-what-information-displays-in-the-milestone-view).\
  Pour plus d’informations sur chaque type de statut, consultez l’article [Vue d’ensemble du statut de progression de la tâche](../../../manage-work/tasks/task-information/task-progress-status.md).

* **Ombrage du statut de la tâche pour les tâches terminées** : une fois qu’une tâche est marquée comme terminée, l’arrière-plan de la tâche est ombré dans la vue « Jalon » pour indiquer si la tâche a été terminée à l’heure ou en retard :

   * **Ombrage rouge de la colonne de la tâche** : l’arrière-plan d’une tâche est rouge lorsque le statut de progression est **En retard**.

   * **Ombrage vert de la colonne de la tâche** : l’arrière-plan d’une tâche est vert lorsque le statut de progression est **À l’heure**.

* **Ombrage du statut du projet pour les colonnes « Début » et « Fin » du projet** :

   * **Colonne « Début » du projet** : l’arrière-plan de la colonne « Début » du projet est rouge ou vert uniquement lorsque la date de début effectif est renseignée :

      * **Ombrage rouge de la colonne « Début » du projet** : l’arrière-plan de la colonne « Début » du projet est rouge lorsque le statut de progression du projet est **En retard**.

      * **Ombrage vert pour la colonne « Début » du projet** : l’arrière-plan de la colonne « Début » du projet est vert lorsque le statut de progression du projet est **À l’heure**.

   * **Colonne d’achèvement du projet** : l’arrière-plan de la colonne d’achèvement du projet est rouge ou vert uniquement lorsque la date d’achèvement est renseignée :

      * **Ombrage rouge pour la colonne d’achèvement du projet** : l’arrière-plan de la colonne d’achèvement du projet est rouge lorsque le statut de progression du projet est **En retard**.

      * **Ombrage vert de la colonne d’achèvement du projet** : l’arrière-plan de la colonne d’achèvement du projet est vert lorsque le statut de progression du projet est **À l’heure**.

   * Aucune couleur d’ombrage n’est attribuée aux colonnes « Début » et « Achèvement » lorsque le statut de progression des tâches est « En danger » ou « En retard ».

  ![Vue jalonnée avec ombrage](assets/milestone-view-with-shading.png)

* **Nom du projet** : le nom du projet s’affiche avec un lien vers le projet.
* **Icône de condition de projet** : une icône s’affiche à côté du nom du projet, indiquant la condition du projet.

## Configurer les informations à afficher dans la vue jalonnée {#configure-what-information-displays-in-the-milestone-view}

Vous pouvez configurer l’affichage des éléments suivants dans la vue jalonnée :

* Icônes du statut de la progression
* Pourcentage d’achèvement des projets et des tâches

Par défaut, les icônes de statut du projet et le pourcentage d’achèvement des projets s’affichent.

Les modifications que vous apportez à ces options s’appliquent uniquement à vous ; elles ne s’appliquent pas aux autres utilisateurs et utilisatrices. Les modifications apportées sont conservées jusqu’à la prochaine connexion à Adobe Workfront.

Pour configurer si les icônes de statut du projet et du pourcentage d’achèvement des projets s’affichent, procédez comme suit :

{{step1-to-projects}}

1. Cliquez sur le bouton **Affichage**, puis cliquez sur **Jalon**.\
   Si vous affichez une liste de projets dans un portfolio ou un programme, sélectionnez le sous-onglet **Jalon**.

1. Cliquez sur **Options** dans le coin supérieur droit de la vue jalonnée.\
   ![milestone_view_options.png](assets/milestone-view-options-350x141.png)

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

Vous pouvez ajuster le pourcentage d’achèvement pour les tâches dans la vue jalonnée. Vous ne pouvez pas ajuster le pourcentage d’achèvement pour une tâche parent (une tâche qui contient des sous-tâches).

Pour ajuster le pourcentage d’achèvement d’une tâche dans la vue jalonnée, procédez comme suit :

{{step1-to-projects}}

1. Cliquez sur le menu déroulant **Affichage**, puis cliquez sur **Jalon**.

1. (Le cas échéant) Si les pourcentages d’achèvement ne sont pas visibles dans la vue jalonnée, cliquez sur **Options** dans le coin supérieur droit de la vue jalonnée, puis assurez-vous que **Pourcentage d’achèvement** est activé.

1. Cliquez sur le pourcentage d’achèvement sous une tâche, indiquez un nouveau pourcentage, puis appuyez sur « Entrée ».
