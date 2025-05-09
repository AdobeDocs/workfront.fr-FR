---
product-area: projects;agile-and-teams
navigation-topic: plan-a-project
title: Gérer l’équipe de projet
description: L’équipe de projet est composée des utilisateurs et utilisatrices associés au projet. Les membres de l’équipe de projet s’affichent dans la section Personnes du projet.
author: Alina
feature: Work Management, Projects
role: User
exl-id: 6e8036fc-feda-4277-9502-0b973028fccb
source-git-commit: 3d96d7b7073ad194f291afe370ae813d3482bc9e
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 99%

---

# Gérer l’équipe de projet

L’équipe de projet est composée des utilisateurs et utilisatrices associés au projet. Les membres de l’équipe de projet s’affichent dans la section Personnes du projet.

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Accès en modification aux projets</p> <p>Accès en affichage de niveau supérieur aux utilisateurs et utilisatrices</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si votre niveau d’accès est soumis à des restrictions supplémentaires. Pour plus d’informations sur la façon dont l’administration Workfront peut modifier votre niveau d’accès, consultez la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations Afficher ou supérieures au projet</p> <p>Pour plus d’informations sur les demandes d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès à des objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Ajouter des utilisateurs et utilisatrices à l’équipe de projet

Lorsque vous ajoutez des utilisateurs et utilisatrices à l’équipe de projet, ils obtiennent des autorisations d’affichage sur le projet et sur les tâches, les problèmes et les documents du projet. Pour plus d’informations, voir l’article [Vue d’ensemble de l’équipe de projet](../../../manage-work/projects/planning-a-project/project-team-overview.md).

>[!TIP]
>
>Les utilisateurs et utilisatrices de l’équipe de projet ne sont pas automatiquement ajoutés aux outils de gestion des ressources du projet.

Vous pouvez ajouter des utilisateurs et utilisatrices à l’équipe de projet de la manière suivante :

* [Ajouter automatiquement des utilisateurs et utilisatrices à une équipe de projet](#automatically-add-users-to-a-project-team)
* [Ajouter manuellement des utilisateurs et utilisatrices à une équipe de projet](#manually-add-users-to-a-project-team)

### Ajouter automatiquement des utilisateurs et utilisatrices à une équipe de projet {#automatically-add-users-to-a-project-team}

Les utilisateurs et utilisatrices qui remplissent les rôles suivants dans le projet sont automatiquement ajoutés à l’équipe de projet et apparaissent dans la section Personnes lors de la création du projet :

* Le créateur ou la créatrice du projet
* Le ou la propriétaire du projet
* Le sponsor du projet

Les utilisateurs et utilisatrices sont également automatiquement ajoutés à l’équipe de projet lorsqu’ils sont affectés aux éléments suivants :

* Tâches
* Problèmes

### Ajouter manuellement des utilisateurs et utilisatrices à une équipe de projet {#manually-add-users-to-a-project-team}

Si des utilisateurs et utilisatrices n’ayant aucun rôle dans le projet souhaitent être informés de certaines mises à jour ou modifications pendant la durée du projet, vous pouvez les ajouter manuellement à l’équipe de projet.

Pour plus d’informations sur les notifications qui peuvent être activées pour les utilisateurs et utilisatrices de l’équipe de projet, voir [Types de notifications d’événement](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

<!--drafted - this used to be the case, in the note below but this limitation was removed on Jan 5, 2023 - as a patch, not a release feature:

>[!IMPORTANT]
>
>You can add to the Project Team only users that belong to the Group associated with the project. You cannot add users that belong to the Subgroups of the project's group. 

-->

1. Accédez au projet auquel vous souhaitez ajouter des utilisateurs ou utilisatrices.

1. Cliquez sur **Personnes** dans le panneau de gauche.

1. Cliquez sur **Ajouter des utilisateurs et utilisatrices**.

   La boîte de dialogue Ajouter des utilisateurs et utilisatrices à l’équipe de projet s’affiche.

   ![add_users_dialog.png](assets/add-users-dialog-350x217.png)

1. Dans la zone **Ajouter des utilisateurs et utilisatrices**, commencez à taper le nom d’un utilisateur ou d’une utilisatrice Workfront actif/active que vous souhaitez ajouter à l’équipe de projet, puis cliquez sur le nom lorsqu’il apparaît dans la liste déroulante.

   Répétez cette étape pour ajouter plusieurs utilisateurs et utilisatrices à l’équipe de projet. Les utilisateurs et utilisatrices doivent appartenir au groupe associé au projet.

   >[!TIP]
   >
   >* Vous ne pouvez pas ajouter des utilisateurs et utilisatrices en ajoutant leurs équipes, groupes, entreprises ou fonctions.
   >* Au fur et à mesure que vous ajoutez des personnes, observez l’avatar, le rôle principal de la personne et son adresse e-mail afin de distinguer les personnes au nom identique. Les utilisateurs et utilisatrices doivent être associés à au moins une fonction pour l’afficher à mesure que vous les ajoutez.
   >
   >  Pour que les utilisateurs et utilisatrices puissent afficher les e-mails de leurs utilisateurs et utilisatrices, le paramètre Afficher les coordonnées doit être activé dans votre niveau d’accès. Pour plus d’informations, consultez la section [Accorder l’accès aux utilisateurs et utilisatrices](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).


1. Cliquez sur **Ajouter**.

   Les personnes obtiennent des autorisations de visualisation du projet et reçoivent des notifications sur le projet en tant que membres de l’équipe de projet.

## Supprimer des utilisateurs et utilisatrices de l’équipe de projet

Lorsque vous supprimez le rôle d’une personne dans le projet, celle-ci continue à faire partie de l’équipe du projet.

Si vous supprimez une personne de l’équipe de projet et que cette dernière est affectée à des tâches ou à des problèmes dans le projet, la personne sera désaffectée des tâches et des problèmes qui ne sont pas terminés. Dans ce cas, les tâches et les problèmes retournent dans la zone Travail non affecté de l’équilibreur de charge de travail.

Les personnes qui sont affectées à des tâches et des problèmes terminés restent affectées même si vous les supprimez de l’équipe de projet.

Pour plus d’informations sur la suppression d’utilisateurs et d’utilisatrices de l’équipe de projet, consultez la section [Supprimer des utilisateurs et utilisatrices des projets](../../../manage-work/projects/manage-projects/remove-users-from-projects.md).
