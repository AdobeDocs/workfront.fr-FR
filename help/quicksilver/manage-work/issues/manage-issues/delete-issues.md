---
product-area: projects
navigation-topic: manage-issues
title: Supprimer des événements
description: Vous pouvez supprimer des problèmes ou des requêtes dans Adobe Workfront si vous disposez des droits d’accès et des autorisations appropriés.
author: Alina
feature: Work Management
exl-id: 31cc802f-7fa6-420c-8494-a45313df1f10
source-git-commit: 31ee3259167532e1e1efa75d635786762f6e476e
workflow-type: tm+mt
source-wordcount: '728'
ht-degree: 7%

---

# Supprimer des événements

<!--Audited: 01/2024-->

Vous pouvez supprimer des problèmes ou des requêtes dans Adobe Workfront si vous disposez des droits d’accès et des autorisations appropriés.

>[!TIP]
>
>&quot;Problèmes&quot; et &quot;requêtes&quot; sont interchangeables dans Workfront. Vous pouvez enregistrer les problèmes sur les projets et les tâches pour indiquer les travaux imprévus qui doivent être résolus. Vous pouvez également envoyer des requêtes qui sont enregistrées en tant que problèmes sur un projet désigné comme file d’attente de requêtes.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Nouvelle : contributeur ou contributrice ou supérieure</p>
   <p>Actuelle : demande ou supérieure</p>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuration du niveau d’accès</td> 
   <td> <p>Modifier l’accès aux problèmes</p> <p>Affichage ou accès supérieur à Projets et tâches</p>  <p>Pour plus d’informations sur l’accès aux problèmes de votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Accorder l’accès aux problèmes</a>.  </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gestion des autorisations sur le problème</p> <p>Autorisations Contribute ou supérieures pour le projet ou la tâche</p> <p> Pour plus d’informations sur l’octroi d’autorisations pour les problèmes, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Partage d’un problème </a></p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront. Pour plus d’informations sur les exigences d’accès, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Observations relatives à la suppression de problèmes

* Votre administrateur Workfront ou un administrateur de groupe doit activer la suppression des problèmes dans un projet dont l’état est Terminé dans la zone Préférences du projet. Pour plus d’informations sur la configuration des préférences de projet, voir [Configuration des préférences de projet à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* Si le problème comporte des heures consignées, l’administrateur Workfront ou un administrateur de groupe doit autoriser la suppression de ces problèmes en configurant les préférences de tâche et de problème dans votre instance Workfront. Cela s’applique également lorsque vous essayez de supprimer des projets qui rencontrent des problèmes avec les heures de connexion.

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">(this is not possible in classic)</span>
  </MadCap:conditionalText>
  -->

  Pour plus d’informations sur l’activation de la suppression des problèmes lorsque des heures sont enregistrées, consultez la section &quot;Suppression&quot; dans [Configuration de la tâche à l’échelle du système et des préférences de problème](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

## Impact des problèmes de suppression

Lorsque vous supprimez un problème, vous avez un impact sur d’autres objets liés au problème.

Les objets suivants associés à un problème sont également supprimés lorsque vous supprimez un problème :

* Documents

  Vous ne pouvez pas supprimer un problème auquel est associé un document extrait. Pour plus d’informations sur l’extraction de documents, voir [Extraction de documents](../../../documents/managing-documents/check-out-documents.md).

* Notes
* Approbations

Selon la manière dont votre administrateur Workfront ou de groupe configure les préférences de projet, de tâche ou de suppression de problème dans les **préférences de la feuille de temps et de l’heure** de votre instance Workfront, les heures consignées pour les problèmes sont gérées de l’une des manières suivantes lors de la suppression d’un problème :

* Accédez au projet et ne sera pas restauré sur le problème, si le problème est restauré ultérieurement.
* être supprimé et restauré sur le problème, si le problème est restauré ultérieurement ;

  Cela s’applique également lorsque vous essayez de supprimer des projets pour lesquels des tâches sont connectées pendant des heures.

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">(this is not possible in classic)</span>
  </MadCap:conditionalText>
  -->

  Pour plus d’informations sur la configuration des préférences de suppression pour les heures de connexion aux problèmes, voir [ Configuration des préférences de feuille de temps et d’heure](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

* Les utilisateurs affectés au problème ou à l’approbation du problème restent membres de l’équipe de projet.\
  Pour plus d’informations sur les équipes de projet, consultez la [présentation de l’équipe de projet](../../../manage-work/projects/planning-a-project/project-team-overview.md).

## Supprimer des événements

* [Supprimer plusieurs problèmes simultanément dans un projet](#delete-multiple-issues-in-a-project-simultaneously)
* [Suppression d’un seul problème](#delete-a-single-issue)

### Suppression simultanée de plusieurs problèmes dans un projet  {#delete-multiple-issues-in-a-project-simultaneously}

1. Accédez au **menu principal**.
1. Cliquez sur **Projets**.
1. Cliquez sur le nom du projet qui contient les problèmes que vous souhaitez supprimer.
1. Cliquez sur **Problèmes** dans le panneau de gauche.
1. Sélectionnez un problème, puis cliquez sur l’icône **Supprimer** ![](assets/delete.png) en haut de la liste.

1. Si la suppression est autorisée, cliquez sur **Oui, supprimez-la**.\
   Votre administrateur Workfront peut ne pas autoriser la suppression des problèmes où des heures sont enregistrées.\
   Pour plus d’informations sur l’accès et les autorisations nécessaires pour supprimer un problème, voir [Problèmes de suppression](#access-and-permissions-needed).

### Suppression d’un seul problème {#delete-a-single-issue}

{{step1-to-projects}}

1. Cliquez sur le nom du projet qui contient le problème que vous souhaitez supprimer.
1. Cliquez sur **Problèmes** dans le panneau de gauche.

   ![](assets/qs-issues-icon-highlighted-on-project-350x278.png)

1. Cliquez sur le nom du problème que vous souhaitez supprimer.
1. Cliquez sur le menu **Plus** à droite du nom du problème.

   ![](assets/qs-issue-more-menu-highlighted-350x469.png)

1. Cliquez sur **Supprimer le problème**.
1. Si la suppression est autorisée, cliquez sur **Oui, supprimez-la**.

   Votre administrateur Workfront peut ne pas autoriser la suppression des problèmes où des heures sont enregistrées.\
   Pour plus d’informations sur l’accès et les autorisations nécessaires pour supprimer un problème, voir [Problèmes de suppression](#access-and-permissions-needed).

## Restauration des problèmes supprimés

Un administrateur Workfront ou de groupe peut restaurer les problèmes dans les 30 jours qui suivent leur suppression. Pour plus d’informations sur la restauration d’éléments dans Workfront, voir [Restaurer les éléments supprimés](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).
