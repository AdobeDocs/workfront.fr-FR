---
product-area: projects
navigation-topic: manage-issues
title: Supprimer des événements
description: Vous pouvez supprimer des problèmes ou des requêtes dans Adobe Workfront si vous disposez des droits d’accès et des autorisations appropriés.
author: Alina
feature: Work Management
exl-id: 31cc802f-7fa6-420c-8494-a45313df1f10
source-git-commit: b7387af018b1814c387ba3f0000fcdf7e0bf5067
workflow-type: tm+mt
source-wordcount: '735'
ht-degree: 97%

---

# Supprimer des événements

<!--Audited: 01/2024-->

Vous pouvez supprimer des problèmes ou des requêtes dans Adobe Workfront si vous disposez des droits d’accès et des autorisations appropriés.

>[!TIP]
>
>« Problèmes » et « demandes » sont interchangeables dans Workfront. Vous pouvez enregistrer des problèmes sur les projets et les tâches afin d’indiquer les travaux imprévus qui doivent être traités. Vous pouvez également soumettre des demandes qui sont enregistrées en tant que problèmes dans un projet désigné comme file d’attente des demandes.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Nouvelle : contributeur ou supérieure</p>
   <p>Actuelle : demande ou niveau supérieur</p>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuration du niveau d’accès</td> 
   <td> <p>Modifier l’accès aux problèmes</p> <p>Affichage ou accès supérieur aux Projets et aux Tâches</p>  <p>Pour plus d’informations sur l’accès aux problèmes liés à votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Accorder l’accès aux problèmes</a>.  </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations sur le problème</p> <p>Autorisations Contribuer ou supérieures pour la tâche ou le projet</p> <p> Pour plus d’informations sur l’octroi d’autorisations aux problèmes, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Partager un problème</a></p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront. Pour plus d’informations sur les conditions d’accès, voir [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Observations relatives à la suppression de problèmes

* Votre équipe d’administration Workfront ou de groupes doit activer la suppression des problèmes dans un projet dont le statut est Terminé dans la zone Préférences du projet. Pour plus d’informations sur la configuration des préférences de projet, voir [Configurer les préférences de projet à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* Si le problème comporte des heures consignées, l’équipe d’administration Workfront ou de groupes doit autoriser la suppression de ces problèmes en configurant les préférences de tâche et de problème dans votre instance Workfront. Cela s’applique également lorsque vous essayez de supprimer des projets qui rencontrent des problèmes avec les heures consignées.

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">(this is not possible in classic)</span>
  </MadCap:conditionalText>
  -->

  Pour plus d’informations sur l’activation de la suppression des problèmes lorsque des heures sont consignées, voir la section « Suppression » dans [Configurer les préférences de tâches et de problèmes à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

## Impact de la suppression de problèmes

Lorsque vous supprimez un problème, cela impacte d’autres objets liés au problème.

Les objets suivants associés à un problème sont également supprimés lorsque vous supprimez le problème :

* Documents

  Vous ne pouvez pas supprimer un problème auquel est associé un document extrait. Pour plus d’informations sur l’extraction de documents, voir [Extraire des documents](../../../documents/managing-documents/check-out-documents.md).

* Notes
* Approbations

Selon la manière dont votre équipe d’administration Workfront ou de groupes configure les préférences de suppression de projet, de tâche ou de problème dans **Préférences de la feuille de temps et des heures** dans votre instance Workfront, les heures consignées pour les problèmes sont gérées de l’une des manières suivantes lors de la suppression d’un problème :

* Elles sont déplacées vers le projet et ne seront pas restaurées sur le problème, si le problème est restauré ultérieurement.
* Elles sont supprimées et restaurées sur le problème, si le problème est restauré ultérieurement.

  Cela s’applique également lorsque vous essayez de supprimer des projets dans lesquels se trouvent des tâches avec des heures consignées.

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">(this is not possible in classic)</span>
  </MadCap:conditionalText>
  -->

  Pour plus d’informations sur la configuration des préférences de suppression pour les heures consignées sur les problèmes, voir [Configurer les préférences de feuille de temps et d’heures](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

* Les personnes affectées au problème ou à l’approbation du problème restent membres de l’équipe de projet.\
  Pour plus d’informations sur les équipes de projet, voir [Vue d’ensemble de l’équipe de projet](../../../manage-work/projects/planning-a-project/project-team-overview.md).

## Supprimer des événements

* [Supprimer simultanément plusieurs problèmes dans un projet](#delete-multiple-issues-in-a-project-simultaneously)
* [Supprimer un seul problème](#delete-a-single-issue)

### Supprimer simultanément plusieurs problèmes dans un projet  {#delete-multiple-issues-in-a-project-simultaneously}

1. Accédez au **Menu principal**.
1. Cliquez sur **Projets**.
1. Cliquez sur le nom du projet qui contient les problèmes que vous souhaitez supprimer.
1. Cliquez sur **Problèmes** dans le panneau de gauche.
1. Sélectionnez un événement, puis cliquez sur l’icône **Supprimer** ![Icône Supprimer](assets/delete.png) en haut de la liste.

1. Si la suppression est autorisée, cliquez sur **Oui, supprimer**.\
   Il se peut que votre administrateur ou administratrice Workfront n’autorise pas la suppression des problèmes dans lesquels des heures sont consignées.\
   Pour plus d’informations sur l’accès et les autorisations nécessaires pour supprimer un problème, voir [Supprimer des problèmes](#access-and-permissions-needed).

### Supprimer un seul problème {#delete-a-single-issue}

{{step1-to-projects}}

1. Cliquez sur le nom du projet qui contient le problème que vous souhaitez supprimer.
1. Cliquez sur **Problèmes** dans le panneau de gauche.

   ![Icône Événements](assets/qs-issues-icon-highlighted-on-project-350x278.png)

1. Cliquez sur le nom du problème que vous souhaitez supprimer.
1. Cliquez sur le menu **Plus** à droite du nom du problème.

   ![Menu Autres événements](assets/qs-issue-more-menu-highlighted-350x469.png)

1. Cliquez sur **Supprimer le problème**.
1. Si la suppression est autorisée, cliquez sur **Oui, supprimer**.

   Il se peut que votre administrateur ou administratrice Workfront n’autorise pas la suppression des problèmes dans lesquels des heures sont consignées.\
   Pour plus d’informations sur l’accès et les autorisations nécessaires pour supprimer un problème, voir [Supprimer des problèmes](#access-and-permissions-needed).

## Restaurer des problèmes supprimés

Un administrateur ou une administratrice Workfront ou de groupes peut restaurer des problèmes dans les 30 jours suivant leur suppression. Pour plus d’informations sur la restauration d’éléments dans Workfront, voir [Restaurer des éléments supprimés](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).
