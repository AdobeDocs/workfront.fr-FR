---
product-area: projects
navigation-topic: manage-tasks
title: Supprimer des tâches
description: Vous pouvez supprimer les tâches qui pourraient être des doublons ou qui ont été créées par erreur.
author: Alina
feature: Work Management
exl-id: aee5c293-e5fa-413e-9d9b-c62528941be7
source-git-commit: 463fc65db6adb5cae6ecffb2e165155c89a63d6d
workflow-type: tm+mt
source-wordcount: '851'
ht-degree: 98%

---

# Supprimer des tâches

Vous pouvez supprimer les tâches qui pourraient être des doublons ou qui ont été créées par erreur.

Pour les tâches qui contiennent des informations historiques (mises à jour, changements de planning, statuts ou d’autres champs), nous vous recommandons de les fermer ou de les marquer comme Immobilisées, au lieu de les supprimer.Cette fonction vous permet de conserver les informations historiques de vos projets.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Travail ou supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Accès en modification aux tâches et projets avec accès à la suppression</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur l’accès aux tâches, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md" class="MCXref xref">Accorder l’accès aux tâches</a>. Pour plus d’informations sur la façon dont l’administration Workfront peut modifier votre niveau d’accès, consultez la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations Contribuer pour le projet avec la capacité d’ajouter des tâches ou autorisations supérieures</p> <p>Lorsque vous créez une tâche, vous recevez automatiquement des autorisations de gestion de la tâche.</p> <p> Pour plus d’informations sur les autorisations de tâches, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">Partager une tâche</a>. </p> <p>Pour plus d’informations sur la demande d’autorisations supplémentaires, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès à des objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre équipe d’administration Workfront.

## Comprendre le processus de suppression des tâches

* [Limites de suppression des tâches](#limitations-for-deleting-tasks)
* [Impact de la suppression des tâches](#the-impact-of-deleting-tasks)

### Limites de la suppression des tâches  {#limitations-for-deleting-tasks}

* Lorsque le statut d’un projet est défini sur Terminé, vous ne pouvez supprimer des tâches que si votre administrateur ou administratrice Workfront ou de groupes l’a autorisé dans la zone Préférences du projet. Pour plus d’informations sur la définition des préférences de projet, voir [Configurer les préférences de projet à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* Si la tâche a des heures consignées, l’administrateur ou l’administratrice Workfront ou du groupe doit autoriser la suppression de ces tâches en configurant les préférences de tâches et de problèmes dans votre instance Workfront. Cela s’applique également lorsque vous essayez de supprimer des projets dans lesquels se trouvent des tâches avec des heures consignées.

  <!--
  (NOTE: the last statement is NWE&nbsp;only; not possible in classic)
  -->

  Pour plus d’informations sur l’activation de la suppression des tâches dans lesquelles des heures sont consignées, voir la section « Suppression » dans [Configurer les préférences de tâches et de problèmes à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

### Impact de la suppression des tâches {#the-impact-of-deleting-tasks}

La suppression d’une tâche a un impact sur les autres objets liés à cette tâche.

Les objets suivants attachés à une tâche sont également supprimés lorsque vous supprimez une tâche :

* Documents

  Vous ne pouvez pas supprimer une tâche à laquelle est joint un document qui a été extrait. Pour plus d’informations sur l’extraction de documents, voir [Extraire des documents](../../../documents/managing-documents/check-out-documents.md).

* Problèmes
* Sous-tâches
* Notes
* Approbations

Selon la façon dont votre administrateur ou administratrice Workfront configure les préférences de suppression de projet, de tâche ou de problème dans les préférences de feuille de temps et d’heures de votre instance Workfront, les heures consignées pour les tâches sont traitées de l’une des façons suivantes lors de la suppression d’une tâche :

* Les heures consignées sont déplacées vers le projet et ne seront pas restaurées sur la tâche si celle-ci est restaurée ultérieurement.
* Les heures consignées sont supprimées et seront restaurées sur la tâche, si celle-ci est restaurée ultérieurement.

  Cela s’applique également lorsque vous essayez de supprimer des projets dans lesquels se trouvent des tâches avec des heures consignées.

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: this stays NWE; not possible in classic;)
  </MadCap:conditionalText>
  -->

  Pour plus d’informations sur la configuration des préférences de suppression des heures consignées sur les problèmes, voir [Configurer les préférences de feuilles de temps et d’heures](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

* Les dépenses relatives à la tâche seront transférées au projet.

* Les utilisateurs et utilisatrices affectés à la tâche ou à l’approbation de la tâche restent dans l’équipe de projet.

  Pour plus d’informations sur les équipes de projet, voir [Vue d’ensemble de l’équipe de projet](../../../manage-work/projects/planning-a-project/project-team-overview.md).

## Supprimer des tâches

* [Supprimer simultanément plusieurs tâches d’un projet](#delete-multiple-tasks-in-a-project-simultaneously)
* [Supprimer une seule tâche](#delete-a-single-task)

### Supprimer simultanément plusieurs tâches d’un projet  {#delete-multiple-tasks-in-a-project-simultaneously}

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront.

1. Cliquez sur **Projets**.
1. Cliquez sur le nom du projet qui contient les tâches à supprimer.
1. Cliquez sur **Tâches** dans le panneau de gauche.
1. Utilisez l’une des méthodes suivantes :

   1. (Le cas échéant) Lorsque le bouton (bascule) **Enregistrement automatique** est activé :

      1. Sélectionnez les tâches que vous souhaitez supprimer, puis cliquez sur **Plus**.
      1. Cliquez sur **Supprimer**, puis sur **Supprimer** pour confirmer la suppression.

         Les tâches sont supprimées.

   1. (Le cas échéant) Cliquez sur l’icône **Mode Plan** et sélectionnez **Enregistrement manuel** si vous souhaitez annuler les modifications apportées à la liste des tâches.

      ![Sélection de l’enregistrement manuel](assets/manual-save-option.png)

      Procédez comme suit :

      1. Sélectionnez les tâches à supprimer.
      1. Cliquez sur **Supprimer**.
      1. (Facultatif) Cliquez sur **Annuler** pour annuler votre modification et ne pas supprimer les tâches.
      1. Cliquez sur **Rétablir** si vous souhaitez conserver les modifications et supprimer la tâche.
      1. Cliquez sur **Enregistrer** pour supprimer les tâches.

         Les tâches ne sont supprimées qu’après l’enregistrement des modifications.

### Supprimer une seule tâche {#delete-a-single-task}

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront.

1. Cliquez sur **Projets**.
1. Cliquez sur le nom du projet qui contient la tâche à supprimer.
1. Cliquez sur **Tâches** dans le panneau de gauche.
1. Cliquez sur le nom de la tâche à supprimer.
1. Cliquez sur l’icône **Plus** ![](assets/qs-more-menu.png) en haut à droite.

   ![](assets/delete-tasks-task-level-nwe-350x225.png)

1. Cliquez sur **Supprimer la tâche**.
1. Si la suppression est autorisée, cliquez sur **Supprimer**.

   Il se peut que votre administrateur ou administratrice Workfront ou de groupes n’autorise pas la suppression des tâches dans lesquelles des heures sont consignées.

   Pour plus d’informations sur l’accès et les autorisations nécessaires pour supprimer une tâche, voir la section [Limites de la suppression des tâches](#limitations-for-deleting-tasks) dans cet article.

## Restaurer les tâches supprimées

Un administrateur ou une administratrice Workfront ou de groupes peut restaurer des tâches dans les 30 jours suivant leur suppression, comme décrit dans [Restaurer les éléments supprimés](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).
