---
product-area: projects
navigation-topic: manage-issues
title: Créer des problèmes
description: Lorsque vous travaillez sur un projet, des événements inattendus peuvent survenir. Vous pouvez consigner ces événements inattendus en tant que problèmes pour un projet particulier ou une tâche. Les utilisateurs et utilisatrices disposant de l’accès approprié peuvent consulter et suivre le statut des problèmes au fur et à mesure de la progression du projet ou de la tâche, ce qui élimine la nécessité de longues chaînes d’e-mails ou de réunions d’avancement. Contrairement aux tâches, qui sont des événements prévus, les problèmes représentent des éléments de travail non prévus dans Adobe Workfront.
author: Alina
feature: Work Management
topic: Collaboration
role: User
exl-id: 2a4488fb-fe2f-422a-887c-996f6367afc5
source-git-commit: b7387af018b1814c387ba3f0000fcdf7e0bf5067
workflow-type: tm+mt
source-wordcount: '1540'
ht-degree: 99%

---

# Créer des problèmes

<!--

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span> 

<span class="preview">For information about the current release, see [Fourth Quarter 2023 release overview](../../../product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md). </span> 

-->

Lorsque vous travaillez sur un projet, des événements inattendus peuvent survenir. Vous pouvez consigner ces événements inattendus en tant que problèmes pour un projet particulier ou une tâche. Les utilisateurs et utilisatrices disposant de l’accès approprié peuvent consulter et suivre le statut des problèmes au fur et à mesure de la progression du projet ou de la tâche, ce qui élimine la nécessité de longues chaînes d’e-mails ou de réunions d’avancement. Contrairement aux tâches, qui sont des événements prévus, les problèmes représentent des éléments de travail non prévus dans Adobe Workfront.

Vous pouvez également ajouter des problèmes à des projets en tant que demandes. Pour plus d’informations, voir [Créer et soumettre des demandes Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).

>[!TIP]
>
>Les problèmes et les demandes sont utilisés de manière interchangeable dans Workfront. Vous pouvez enregistrer des problèmes sur les projets et les tâches afin d’indiquer les travaux imprévus qui doivent être traités. Vous pouvez également soumettre des demandes qui sont enregistrées en tant que problèmes dans un projet désigné comme file d’attente des demandes.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

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
   <td> <p>Révision ou niveau supérieur pour ajouter des problèmes à un projet ou à une tâche</p> <p>Demande ou niveau supérieur pour ajouter des problèmes en tant que demandes, à l’aide d’une file d’attente des demandes.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux problèmes</p> <p>Affichage ou accès supérieur aux Projets et aux Tâches</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur l’accès aux problèmes liés à votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Accorder l’accès aux problèmes</a>. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations Contribuer ou supérieures comprenant la possibilité d’ajouter des problèmes à la tâche ou au projet dans lequel vous créez le problème.</p> <p> Pour plus d’informations sur l’octroi d’autorisations aux problèmes, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Partager un problème</a></p> <p>Pour plus d’informations sur la demande d’autorisations supplémentaires, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès à des objets</a></p> </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

+++

<!--
(NOTE: in NWE Requestors CAN see the Issues tab on a project but in classic they cannot! However, even when they DO see it, they cannot enter the issues - logged this issue for it but they might decide not to fix it: https://hub.workfront.com/issue/60181e28000058980cce29597185b2d6/updates?email-source=comm)</p>
-->

## Limites de la création de problèmes

Lorsque vous disposez des accès et des autorisations nécessaires, vous pouvez créer des problèmes sur un projet ou une tâche. Toutefois, il se peut que vous ne puissiez pas créer de problèmes dans les cas suivants :

* Votre administration de Workfront ou de groupes doit autoriser l’ajout de problèmes à un projet dont le statut est Terminé ou Immobilisé dans la zone Préférences du projet. Pour plus d’informations sur la définition des préférences de projet, voir [Configurer les préférences de projet à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* Vous ne pouvez pas ajouter de problèmes à un projet qui est en attente d’approbation.

## Préparer le formulaire Nouveau problème

Votre organisation doit disposer d’un processus bien défini pour déterminer quand et comment enregistrer un problème. Lorsque vous configurez ce processus, la première étape consiste à créer le formulaire nécessaire à la soumission d’un problème. Que vous autorisiez l’ajout de problèmes aux tâches et aux projets directement, ou que vous ayez des files d’attente des demandes où les problèmes sont soumis, vous pouvez définir les champs Workfront ainsi que les champs personnalisés qui sont disponibles pour les utilisateurs et utilisatrices lorsqu’ils soumettent de nouveaux problèmes et qui doivent être complétés. Le formulaire Nouveau problème peut contenir des informations importantes qui permettront de résoudre rapidement le problème.

Les champs pour les nouveaux problèmes d’un projet sont définis dans la section Détails de la file d’attente du projet où les problèmes seront enregistrés. Pour plus d’informations sur la configuration de la section Détails de la file d’attente du projet, voir [Créer une file d’attente des demandes](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

Pour plus d’informations sur la création de problèmes par le biais d’une soumission à une file d’attente des demandes, voir la section [Créer des problèmes en saisissant une nouvelle demande](#create-issues-by-entering-a-new-request) de cet article.

## Créer des problèmes sur une tâche ou un projet à l’aide du bouton Nouveau problème

Après avoir défini les champs d’un nouveau formulaire de problème sur votre projet, vous pouvez commencer à créer des problèmes.

<!-- OLD UI: redesigned on Oct 26, 2023:

Creating issues differs depending on which environment you choose to create the issue. 

### Create issues on a task or project using the New Issue button in the Production environment

To create an issue on a task or a project:

1. Go to a project where you want to create the issue. 
1. (Optional) If you want to log the issue for a task, go to the **Tasks** area, then click the name of a task. 
1. Click the **Issues** section.

   
1. Click **New Issue**.

  

1. (Conditional) If the project creator created Queue Topics or Topic Groups on the project they are added to the new issue form. Specify the **Topic Group** or the **Queue Topic** of your new issue. Topic Groups and Queue Topics have names customized to your environment.  
   For more information about creating Topic Groups, see [Create Topic Groups](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md). For more information about creating Queue Topics, see [Create Queue Topics](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

   ![New issue screen](assets/new-issue-screen-when-creating-issue-from-list-project-level-nwe-350x422.png)

   * If there is only one Queue Topic set on the project, it is displayed automatically.
   * If the Topic Group does not have any Queue Topics or Topic Groups under it, nothing is available in the Topic Group drop-down.

1. (Conditional) If the project creator allowed for the **Request Type** field to display on the New Issue form, select the type of your issue from the following options:

   * Bug Report
   * Change Order
   * Issue
   * Request  
     Depending on how your Workfront administrator has configured your Project Preferences, the names of the issue types might be different for you. 

   >[!TIP]
   >
   >The Request Types must be enabled in the Queue Details and as well as when creating the Queue Topic to display as a selection in the New Issue form. For information, see the following articles: 
   >* [Create a Request Queue](../../requests/create-and-manage-request-queues/create-request-queue.md)
   >  * [Create Queue Topics](../../requests/create-and-manage-request-queues/create-queue-topics.md)


1. Add a name for the new issue in the **Issue Name** field. 
1. Continue specifying the fields available in the **New Issue** form. For more information about the fields available as you enter a new issue, see [Edit issues](../../../manage-work/issues/manage-issues/edit-issues.md).

   >[!IMPORTANT]
   >
   >Not all the issue-related fields are available in the New Issue form. The project creator enables the fields available when creating an issue when they define the Queue Details area of the project. For more information, see [Create a Requests Queue](../../requests/create-and-manage-request-queues/create-request-queue.md). 


1. (Conditional) If the Queue Topics are associated with a custom form, that custom form will display in the **New Issue** form.  
   Or  
   If the project is associated with an issue custom form through the Queue Details area, the form displays in the **New Issue** form, after the default Workfront fields.

   For information, see [Create a Request Queue](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. Click **Save New Issue.**

Issues can be assigned to multiple users, job roles or to a team. For more information about assigning and managing requests, see [Manage work and team requests](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).

<!--When this is coming to Production, remove the "Production" section above and replace it with the following content:
-->

Pour créer un problème sur une tâche ou un projet :

1. Accédez au projet dans lequel vous souhaitez créer le problème.
1. (Facultatif) Si vous souhaitez enregistrer le problème d’une tâche, accédez à la zone **Tâches**, puis cliquez sur le nom d’une tâche.
1. Cliquez sur la section **Problèmes**.

   La liste des problèmes associés au projet s’affiche.

1. Cliquez sur **Nouveau problème** en haut de la liste des problèmes.
La boîte de dialogue Nouveau problème s’affiche.

   ![Nouvelle boîte d&#39;événement](assets/new-issue-box-matches-new-request-ui.png)

1. (Le cas échéant) Si la personne à l’origine du projet a créé des rubriques de file d’attente ou des groupes de rubriques sur le projet, ils sont ajoutés au formulaire du nouveau problème. Indiquez le **groupe de rubriques** ou la **rubrique de file d’attente** de votre nouveau problème. Les groupes de rubriques et les rubriques de file d’attente ont des noms adaptés à votre environnement.\
   Pour plus d’informations sur la création de groupes de rubriques, voir [Créer des groupes de rubriques](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md). Pour plus d’informations sur la création de rubriques de file d’attente, voir [Créer des rubriques de file d’attente](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

   * S’il n’y a qu’une seule rubrique de file d’attente définie pour le projet, elle s’affiche automatiquement.
   * Si le groupe de rubriques n’a pas de rubriques de file d’attente ou de groupes de rubriques sous lui, rien n’est disponible dans le menu déroulant du groupe de rubriques.

1. Ajoutez le nom du problème dans le champ **Objet**, puis ajoutez une **description**.

1. (Le cas échéant) Si la personne qui a créé le projet a autorisé l’affichage du champ **Type de demande** dans le formulaire Nouveau problème, sélectionnez le type de votre problème parmi les options suivantes :

   * Rapport sur les bogues
   * Modifier l&#39;ordre
   * Problème
   * Demande\
     Selon la façon dont votre administrateur ou administratrice Workfront a configuré les préférences de votre projet, les noms des types de problèmes peuvent être différents pour vous.

   >[!TIP]
   >
   >Les types de demande doivent être activés dans les détails de la file d’attente et lors de la création de la rubrique de file d’attente afin d’être affichés comme sélection dans le formulaire Nouveau problème. Pour plus d’informations, voir les articles suivants :
   >* [Créer une file d’attente des demandes](../../requests/create-and-manage-request-queues/create-request-queue.md)
   >  * [Créer des rubriques de file d’attente](../../requests/create-and-manage-request-queues/create-queue-topics.md)

1. Continuez à spécifier les champs disponibles dans le formulaire **Nouveau problème**. Pour plus d’informations sur les champs disponibles lors de la saisie d’un nouveau problème, voir [Modifier les problèmes](../../../manage-work/issues/manage-issues/edit-issues.md).

   >[!IMPORTANT]
   >
   >Tous les champs relatifs au problème ne sont pas disponibles dans le formulaire Nouveau problème. La personne qui a créé le projet active les champs disponibles lors de la création d’un problème lorsqu’elle définit la zone Détails de la file d’attente du projet. Pour plus d’informations, voir [Créer une file d’attente des demandes](../../requests/create-and-manage-request-queues/create-request-queue.md).


1. (Le cas échéant) Si les rubriques de file d’attente sont associés à un formulaire personnalisé, celui-ci s’affichera dans le formulaire **Nouveau problème**.\
   Ou\
   Si le projet est associé à un formulaire personnalisé de problème par le biais de la zone Détails de la file d’attente, le formulaire s’affiche dans le formulaire **Nouveau problème**, après les champs par défaut de Workfront.

   Pour plus d’informations, voir [Créer une file d’attente des demandes](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. Cliquez sur **Soumettre**.

   Les problèmes peuvent être affectés à plusieurs utilisateurs ou utilisatrices, à des fonctions ou à une équipe. Pour plus d’informations sur l’affectation et la gestion des demandes, voir [Gérer les demandes de travail et d’équipe](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).


## Créer des problèmes en ligne sur une tâche ou un projet

>[!IMPORTANT]
>
>Le ou la propriétaire du projet doit activer **Autoriser les utilisateurs et utilisatrices à ajouter des questions en ligne** lors de la définition des paramètres des problèmes pour le projet avant que vous puissiez ajouter des problèmes en ligne au projet ou aux tâches. Pour plus d’informations sur la configuration des paramètres des problèmes sur un projet, voir [Modifier les projets](../../../manage-work/projects/manage-projects/edit-projects.md).
>

Lorsque vous souhaitez ajouter plusieurs problèmes rapidement, vous pouvez créer des problèmes pour une tâche ou un projet en ligne, en les ajoutant à une liste de problèmes.

>[!NOTE]
>
>Lorsque vous ajoutez des problèmes en ligne, Workfront n’applique pas le formulaire Nouveau problème aux nouveaux problèmes. Nous ne recommandons pas d’ajouter des problèmes en ligne si vous souhaitez que les utilisateurs et utilisatrices fournissent certaines informations lors de la saisie des problèmes. Cela peut avoir un impact négatif sur le signalement des problèmes et, par la suite, sur la capacité de la personne affectée au problème à disposer de toutes les informations nécessaires pour résoudre le problème.

Pour créer des problèmes en ligne :

1. Accédez au projet dans lequel vous souhaitez créer le problème.
1. (Facultatif) Si vous souhaitez enregistrer le problème d’une tâche, accédez à la section **Tâches**, puis cliquez sur le nom d’une tâche.
1. Cliquez sur l’onglet **Problèmes** dans le panneau de gauche.
1. Cliquez sur **Ajouter d’autres problèmes** en bas de la liste des problèmes.

   Une nouvelle ligne est créée dans la liste des problèmes de la section Problèmes.

   >[!TIP]
   >
   >Cette option est grisée si le paramètre Autoriser les utilisateurs et utilisatrices à ajouter des problèmes en ligne est désélectionné dans la boîte Modifier le projet. Pour plus d’informations, voir [Modifier les projets](../../../manage-work/projects/manage-projects/edit-projects.md).

   ![Bouton Ajouter d&#39;autres événements](assets/add-more-issues-button-highlighted-issue-list-nwe-350x272.png)

1. Commencez à saisir le nom du problème dans le champ Nom, puis continuez à ajouter des informations sur le problème en ligne.

   >[!TIP]
   >
   >Les champs qui peuvent être modifiés en ligne sont rendus disponibles par la vue que vous appliquez à votre liste de problèmes. Il se peut que vous ne puissiez pas modifier en ligne les types de champs suivants :
   >   
   >* Champs appartenant à un autre objet
   >* Champs que vous n’avez pas le droit de modifier
   >* Champs qui sont des calculs et qui sont automatiquement mis à jour par Workfront

1. Cliquez sur Entrée pour terminer la modification en ligne et ajoutez le problème au projet ou à la tâche.

## Créer des problèmes en introduisant une nouvelle demande {#create-issues-by-entering-a-new-request}

Vous pouvez désigner des projets qui serviront de réceptacles pour la réception des problèmes. Ces types de projets sont appelés files d’attente des demandes dans Workfront. Vous pouvez accéder aux files d’attente des demandes par l’intermédiaire de votre zone Demandes dans le menu principal.

>[!TIP]
>
>Les termes « problème » et « demande » sont interchangeables dans Workfront.

Pour plus d’informations sur la manière de configurer des projets en tant que files d’attente des demandes pour recevoir des problèmes, voir [Créer une file d’attente des demandes](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md). Pour plus d’informations sur la soumission des demandes, voir [Créer et soumettre des demandes Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).
