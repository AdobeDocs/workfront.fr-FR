---
product-area: projects;agile-and-teams
navigation-topic: plan-a-project
title: Gérer l’équipe d’un projet
description: L’équipe de projet est composée des utilisateurs associés au projet. Les membres de l’équipe de projet s’affichent dans la section Personnes du projet.
author: Alina
feature: Work Management, Projects
role: User
exl-id: 6e8036fc-feda-4277-9502-0b973028fccb
source-git-commit: afbf2e2fbfcc2c527223da008518bc7632872c23
workflow-type: tm+mt
source-wordcount: '679'
ht-degree: 22%

---

# Gérer l’équipe d’un projet

L’équipe de projet est composée des utilisateurs associés au projet. Les membres de l’équipe de projet s’affichent dans la section Personnes du projet.

## Conditions d’accès

<!--drafted for P&P:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p>
   Or
   <p>Legacy license: Plan </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p>View or higher access to Users</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux projets</p> <p>Affichage ou accès supérieur aux utilisateurs</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Affichage ou autorisations supérieures du projet</p> <p>Pour plus d’informations sur la demande d’un accès supplémentaire, consultez <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

* Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Ajout d’utilisateurs à une équipe de projet

Lorsque vous ajoutez des utilisateurs à l’équipe du projet, ils disposent des autorisations de vue sur le projet, ainsi que sur les tâches, problèmes et documents du projet. Pour plus d’informations, consultez l’article [Project Team overview](../../../manage-work/projects/planning-a-project/project-team-overview.md) (Présentation de l’équipe de projet).

>[!TIP]
>
>Les utilisateurs de l’équipe de projet ne sont pas automatiquement ajoutés aux outils de gestion des ressources du projet.

Vous pouvez ajouter des utilisateurs à l’équipe de projet de la manière suivante :

* [Ajouter automatiquement des utilisateurs à une équipe de projet](#automatically-add-users-to-a-project-team)
* [Ajout manuel d’utilisateurs à une équipe de projet](#manually-add-users-to-a-project-team)

### Ajout automatique d’utilisateurs à une équipe de projet {#automatically-add-users-to-a-project-team}

Les utilisateurs qui remplissent les rôles suivants du projet sont automatiquement ajoutés à l’équipe du projet et apparaissent dans la section Personnes lors de la création du projet :

* Créateur du projet
* Le propriétaire du projet
* Le sponsor du projet

Les utilisateurs sont également automatiquement ajoutés à l’équipe du projet lorsqu’ils sont affectés aux éléments suivants :

* Tâches
* Problèmes

### Ajout manuel d’utilisateurs à une équipe de projet {#manually-add-users-to-a-project-team}

Si les utilisateurs qui ne remplissent aucun rôle dans le projet veulent être informés de certaines mises à jour ou modifications au cours de la vie du projet, vous pouvez les ajouter manuellement à l’équipe du projet.

Pour plus d’informations sur les notifications qui peuvent être activées pour les utilisateurs de l’équipe de projet, voir [Types de notification d’événement](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

<!--drafted - this used to be the case, in the note below but this limitation was removed on Jan 5, 2023 - as a patch, not a release feature:

>[!IMPORTANT]
>
>You can add to the Project Team only users that belong to the Group associated with the project. You cannot add users that belong to the Subgroups of the project's group. 

-->

1. Accédez au projet auquel vous souhaitez ajouter des utilisateurs.

1. Cliquez sur **Personnes** dans le panneau de gauche. Vous devrez peut-être d’abord cliquer sur **Afficher plus** .

1. Cliquez sur **Ajouter des utilisateurs**.

   La boîte de dialogue Ajouter des utilisateurs à l’équipe de projet s’affiche.

   ![add_users_dialog.png](assets/add-users-dialog-350x217.png)

1. Dans la zone **Ajouter des utilisateurs**, commencez à saisir le nom d’un utilisateur Workfront actif que vous souhaitez ajouter à l’équipe de projet, puis cliquez sur le nom lorsqu’il apparaît dans la liste déroulante.

   Répétez cette étape pour ajouter plusieurs utilisateurs à l’équipe du projet. Les utilisateurs doivent appartenir au groupe associé au projet.

   >[!TIP]
   >
   >* Vous ne pouvez pas ajouter d’utilisateurs en ajoutant leurs équipes, groupes, entreprises ou rôles de tâche.
   >* À mesure que vous ajoutez des utilisateurs, notez l’avatar, le rôle de Principal de l’utilisateur et son adresse électronique pour faire la distinction entre les utilisateurs portant des noms identiques. Les personnes doivent être associées à au moins une fonction pour l’afficher à mesure que vous les ajoutez.
   >
   >  Pour pouvoir voir les adresses e-mail des utilisateurs et utilisatrices, le paramètre Afficher les coordonnées doit être activé dans votre niveau d’accès. Pour plus d’informations, consultez [Accorder l’accès aux utilisateurs et utilisatrices](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).


1. Cliquez sur **Ajouter**.

   Les utilisateurs disposent des autorisations d’affichage sur le projet et reçoivent des notifications sur le projet dans le cadre de l’équipe du projet.

## Suppression d’utilisateurs d’une équipe de projet

Lorsque vous supprimez des utilisateurs de leurs rôles sur le projet, ils restent membres de l’équipe du projet.

Si vous supprimez un utilisateur de l’équipe de projet et qu’il est affecté à des tâches ou à des problèmes dans le projet, l’utilisateur n’est plus affecté aux tâches et aux problèmes qui ne sont pas terminés. Dans ce cas, les tâches et les problèmes retournent à la zone de travail non assigné dans l’équilibreur de charge de travail.

Les utilisateurs affectés à des tâches et des problèmes terminés restent affectés même après les avoir supprimés de l’équipe de projet.

Pour plus d’informations sur la suppression des utilisateurs de l’équipe de projet, voir [Suppression des utilisateurs des projets](../../../manage-work/projects/manage-projects/remove-users-from-projects.md).
