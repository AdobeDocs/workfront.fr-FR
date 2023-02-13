---
product-area: projects
navigation-topic: manage-issues
title: Création de problèmes
description: Lorsque vous travaillez sur un projet, vous pouvez découvrir que des événements inattendus se produisent. Vous pouvez consigner ces événements inattendus comme des problèmes pour un projet particulier ou pour une tâche. Les utilisateurs disposant de l’accès approprié peuvent afficher et surveiller l’état des problèmes au fur et à mesure que le projet ou la tâche se termine, éliminant ainsi la nécessité de longues chaînes de messagerie ou de réunions d’état. Contrairement aux tâches, qui sont des événements planifiés, les problèmes représentent des tâches non planifiées dans Adobe Workfront.
author: Alina
feature: Work Management
exl-id: 2a4488fb-fe2f-422a-887c-996f6367afc5
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1397'
ht-degree: 0%

---

# Création de problèmes

Lorsque vous travaillez sur un projet, vous pouvez découvrir que des événements inattendus se produisent. Vous pouvez consigner ces événements inattendus comme des problèmes pour un projet particulier ou pour une tâche. Les utilisateurs disposant de l’accès approprié peuvent afficher et surveiller l’état des problèmes au fur et à mesure que le projet ou la tâche se termine, éliminant ainsi la nécessité de longues chaînes de messagerie ou de réunions d’état. Contrairement aux tâches, qui sont des événements planifiés, les problèmes représentent des tâches non planifiées dans Adobe Workfront.

Vous pouvez également ajouter des problèmes aux projets en tant que requêtes. Pour plus d’informations, voir [Création et envoi de requêtes Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).

>[!TIP]
>
>Les problèmes et les requêtes sont interchangeables dans Workfront. Vous pouvez enregistrer les problèmes sur les projets et les tâches pour indiquer les travaux imprévus qui doivent être résolus. Vous pouvez également envoyer des requêtes qui sont enregistrées en tant que problèmes sur un projet désigné comme file d’attente de requêtes.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Révision ou version ultérieure pour ajouter des problèmes à un projet ou à une tâche</p> <p>Demandez à ou à une version ultérieure d’ajouter des problèmes en tant que requêtes à l’aide d’une file d’attente de requêtes.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modifier l’accès aux problèmes</p> <p>Affichage ou accès supérieur à Projets et tâches</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur l’accès aux problèmes de votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Accorder l’accès aux problèmes</a>. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Contribuez à des autorisations ou à des autorisations supérieures avec la possibilité d’ajouter des problèmes à la tâche ou au projet dans lequel vous créez le problème.</p> <p> Pour plus d’informations sur l’octroi d’autorisations aux problèmes, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Partage d’un problème </a></p> <p>Pour plus d’informations sur la demande d’autorisations supplémentaires, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: in NWE Requestors CAN see the Issues tab on a project but in classic they cannot! However, even when they DO see it, they cannot enter the issues - logged this issue for it but they might decide not to fix it: https://hub.workfront.com/issue/60181e28000058980cce29597185b2d6/updates?email-source=comm)</p>
-->

## Limites de la création de problèmes

Lorsque vous disposez des droits d’accès et des autorisations appropriés, vous pouvez créer des problèmes sur un projet ou une tâche. Cependant, voici quelques cas où vous ne pourrez peut-être pas créer de problèmes :

* Votre administrateur Workfront ou un administrateur de groupe doit activer l’ajout de problèmes à un projet dont l’état est Terminé ou Mort dans la zone Préférences du projet. Pour plus d’informations sur la définition des préférences de projet, voir [Configuration des préférences de projet à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* Vous ne pouvez pas ajouter de problèmes à un projet qui est en attente d’approbation.

## Préparation du formulaire New Issue

Votre entreprise doit avoir un processus bien défini pour savoir quand et comment enregistrer un problème. Lorsque vous configurez ce processus, la première étape consiste à créer le formulaire nécessaire à l’envoi d’un problème. Que vous autorisiez l’ajout direct de problèmes aux tâches et aux projets, ou que vous ayez des files d’attente de requêtes lorsque des problèmes sont envoyés, vous pouvez définir les champs Workfront ainsi que les champs personnalisés disponibles pour les utilisateurs lorsqu’ils envoient de nouveaux problèmes et qu’ils doivent être remplis. Le formulaire Nouveau problème peut contenir des informations importantes qui aideront à résoudre rapidement le problème.

Les champs correspondant aux nouveaux problèmes d’un projet sont définis dans la section Détails de la file d’attente du projet où les problèmes seront consignés. Pour plus d’informations sur la configuration de la section Détails de la file d’attente du projet, voir [Création d’une file d’attente de requête](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

Pour plus d’informations sur la création de problèmes en les envoyant à une file d’attente de requêtes, voir [Créer des problèmes en saisissant une nouvelle requête](#create-issues-by-entering-a-new-request) dans cet article.

## Création de problèmes sur une tâche ou un projet à l’aide du bouton Nouveau problème

Après avoir défini les champs d’un nouveau formulaire de problème sur votre projet, vous pouvez commencer à créer des problèmes.

Pour créer un problème sur une tâche ou un projet :

1. Accédez à un projet dans lequel vous souhaitez créer le problème.
1. (Facultatif) Si vous souhaitez consigner le problème pour une tâche, accédez au **Tâches** , puis cliquez sur le nom d’une tâche.
1. Cliquez sur le bouton **Problèmes** .

   ![](assets/qs-issues-icon-highlighted-on-project-350x216.png)

1. Cliquez sur **Nouveau problème**.

   ![](assets/qs-issue-list-on-project-with-new-issue-button-highlighted-350x270.png)

1. (Conditionnel) Si le créateur du projet a créé des rubriques de file d’attente ou des groupes de rubriques sur le projet, ils sont ajoutés au nouveau formulaire de problème. Spécifiez la variable **Groupe de rubriques** ou le **Rubrique de la file d’attente** de votre nouveau problème. Des noms doivent être personnalisés en fonction de votre environnement.\
   Pour plus d’informations sur la création de groupes de rubriques, voir [Création de groupes de rubriques](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md). Pour plus d’informations sur la création de rubriques de file d’attente, voir [Création de rubriques de file d’attente](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

   ![](assets/new-issue-screen-when-creating-issue-from-list-project-level-nwe-350x422.png)

   * Si une seule rubrique de file d’attente est définie sur le projet, elle s’affiche automatiquement.
   * Si le groupe de rubriques ne contient aucune rubrique de file d’attente ou aucun groupe de rubriques, rien n’est disponible dans la liste déroulante Groupe de rubriques .

1. (Conditionnel) Si le créateur du projet a autorisé la variable **Type de problème** pour afficher le champ Nouveau problème dans le formulaire, sélectionnez le type de problème parmi les options suivantes :

   * Rapport sur les bogues
   * Modifier l&#39;ordre
   * Problème
   * Demande\
      Selon la manière dont votre administrateur Workfront a configuré vos préférences de projet, les noms des types de problèmes peuvent être différents pour vous.

1. Indiquez les champs disponibles dans la variable **Nouveau problème** formulaire. Pour plus d’informations sur la définition des champs lorsque vous saisissez un nouveau problème, voir [Modification des problèmes](../../../manage-work/issues/manage-issues/edit-issues.md).
1. (Conditionnel) Si les rubriques de la file d’attente sont associées à un formulaire personnalisé, ce formulaire personnalisé s’affiche dans la variable **Nouveau problème** formulaire.\
   Ou\
   Si le projet est associé à un formulaire personnalisé de problème via la zone Détails de la file d’attente, le formulaire s’affiche dans la variable **Nouveau problème** formulaire, sous les champs Workfront par défaut.

   Pour plus d’informations, voir [Création d’une file d’attente de requête](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. Cliquez sur **Enregistrer un nouveau problème.**

Les problèmes peuvent être affectés à plusieurs utilisateurs, rôles de tâche ou à une équipe. Pour plus d’informations sur l’affectation et la gestion des requêtes, voir [Gérer les requêtes de travail et d’équipe](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).

## Création de problèmes sur une tâche ou un projet intégré

>[!IMPORTANT]
>
>Le propriétaire du projet doit activer **Autoriser les utilisateurs à ajouter des problèmes en ligne** lorsque vous définissez les paramètres de problème du projet avant de pouvoir ajouter des problèmes en ligne au projet ou aux tâches. Pour plus d’informations sur la configuration des paramètres de problème sur un projet, voir [Modification de projets](../../../manage-work/projects/manage-projects/edit-projects.md).

Lorsque vous souhaitez ajouter rapidement plusieurs problèmes, vous pouvez créer des problèmes pour une tâche ou un projet intégré, en les ajoutant à une liste de problèmes.

>[!NOTE]
>
>Lorsque vous ajoutez des problèmes en ligne, Workfront n’applique pas le formulaire Nouveau problème aux nouveaux problèmes. Il est déconseillé d’ajouter des problèmes en ligne si vous souhaitez que les utilisateurs fournissent certaines informations lors de la saisie des problèmes. Cela peut avoir un impact négatif sur la création de rapports sur les problèmes, puis sur la capacité de l’utilisateur affecté au problème à disposer de toutes les informations nécessaires pour résoudre le problème.

Pour créer des problèmes en ligne :

1. Accédez à un projet dans lequel vous souhaitez créer le problème.
1. (Facultatif) Si vous souhaitez consigner le problème pour une tâche, accédez au **Tâches** , puis cliquez sur le nom d’une tâche.
1. Cliquez sur le bouton **Problèmes** .
1. Cliquez sur **Ajout de problèmes**.

   Une nouvelle ligne est créée dans la liste des problèmes de la section Problèmes .

   >[!TIP]
   >
   >Cette option est grisée si le paramètre Autoriser les utilisateurs à ajouter des problèmes en ligne est désélectionné dans la zone Modifier le projet . Pour plus d’informations, voir [Modification de projets](../../../manage-work/projects/manage-projects/edit-projects.md).

   ![](assets/add-more-issues-button-highlighted-issue-list-nwe-350x272.png)

1. Commencez à saisir le nom du problème dans le champ Nom , puis continuez à ajouter des informations supplémentaires sur le problème en ligne.

   >[!TIP]
   >
   >Les champs pouvant être modifiés en ligne sont disponibles dans la vue que vous appliquez à votre liste de problèmes. Vous ne pourrez peut-être pas modifier en ligne les types de champs suivants :
   >   
   >* Champs appartenant à un autre objet
   >* Champs que vous n’avez pas accès à la modification
   >* Champs qui sont des calculs et qui sont automatiquement mis à jour par Workfront


1. Cliquez sur Entrée pour terminer la modification en ligne et ajoutez le problème au projet ou à la tâche.

## Créer des problèmes en saisissant une nouvelle requête {#create-issues-by-entering-a-new-request}

Vous pouvez désigner les projets comme des réceptacles pour les problèmes de réception. Ces types de projets sont appelés files d’attente de demande dans Workfront. Vous pouvez accéder aux files d’attente de demandes par le biais de la zone Demandes du menu principal.

>[!TIP]
>
>Les termes &quot;problème&quot; et &quot;demande&quot; sont interchangeables dans Workfront.

Pour plus d’informations sur la configuration de projets en tant que files d’attente de demandes pour recevoir des problèmes, voir [Création d’une file d’attente de requête](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md). Pour plus d’informations sur l’envoi de requêtes, voir [Création et envoi de requêtes Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).
