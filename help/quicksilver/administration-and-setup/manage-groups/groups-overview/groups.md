---
title: Vue d’ensemble des groupes
user-type: administrator
content-type: reference;overview
product-area: system-administration;user-management
navigation-topic: groups-overview
description: Un administrateur Workfront peut créer des groupes d’utilisateurs qui correspondent à la structure de votre service. Les groupes sont similaires aux équipes et aux entreprises, mais différents les uns des autres.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 1353ab04-7de7-4d30-a092-27807c950777
source-git-commit: b5e0a590d258df4510a0bb6a44b57099f32ae6b9
workflow-type: tm+mt
source-wordcount: '927'
ht-degree: 1%

---

# Vue d’ensemble des groupes

<!-- Audited: 01/2024 -->

Un administrateur Workfront peut créer des groupes d’utilisateurs qui correspondent à la structure de votre service. Les groupes sont similaires aux équipes et aux entreprises, mais différents les uns des autres.

L’administrateur Workfront accorde aux groupes l’accès aux zones Workfront dans lesquelles ils doivent travailler et communiquer. Chaque groupe peut ensuite conserver ses informations Workfront telles que les utilisateurs, les modèles et les formulaires personnalisés, ainsi que les projets, séparément de celles des autres services.

Au moins un administrateur de groupe est requis pour chaque groupe. Les administrateurs de groupe peuvent utiliser la page Groupes pour gérer leurs groupes au même endroit. Pour plus d’informations, voir [Administrateurs de groupe](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

Vous pouvez créer jusqu’à 14 niveaux de sous-groupes dans un seul groupe. Pour plus d’informations, voir [Présentation des sous-groupes](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md) et [Création d’un sous-groupe](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).

## Utilisation de groupes pour organiser les utilisateurs

En tant qu’administrateur Workfront ou administrateur de groupe, vous pouvez associer des utilisateurs à des groupes et des sous-groupes. Si vous rendez un groupe public, les utilisateurs disposant d’une licence Standard (nouvelle) ou Plan (en cours) peuvent y associer des utilisateurs. Pour plus d’informations sur les administrateurs de groupes et les groupes publics, voir [Création d’un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

Lorsque vous créez un utilisateur, nous vous recommandons d’ajouter cet utilisateur au groupe d’accueil approprié et aux autres groupes dans lesquels il doit travailler. Un utilisateur ne peut avoir qu’un seul groupe d’accueil, mais il peut appartenir à plusieurs autres groupes.

Faire partie d’un groupe permet à l’utilisateur d’accéder aux objets partagés avec le groupe et les sous-groupes. Par exemple, si vous partagez un projet avec un groupe, les utilisateurs du groupe et les sous-groupes du groupe y ont accès.

>[!TIP]
>
>Si les ministères de votre organisation travaillent souvent ensemble pour gérer les projets et les ressources sur ces projets, il peut ne pas être nécessaire de diviser les ministères en plusieurs groupes plus petits. Quelques groupes de haut niveau peuvent fonctionner mieux.

Un groupe peut avoir un nombre illimité d’utilisateurs.

Pour plus d’informations sur la création d’utilisateurs et d’utilisatrices, voir [Ajouter des utilisateurs et des utilisatrices](../../../administration-and-setup/add-users/add-users.md).

## Octroi à un groupe d’un accès aux objets

Lorsque vous partagez un objet avec un groupe, tous les membres de ce groupe (y compris les membres de tous les sous-groupes) ont accès à l’objet. Pour plus d’informations sur le partage dans Workfront, voir [Présentation des autorisations de partage sur les objets](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## Associer un groupe à un objet

Lorsque vous créez ou modifiez l’un des objets Workfront suivants, vous pouvez l’associer à un groupe :

* **Projet** : vous pouvez associer un seul groupe à un projet pour indiquer la propriété du projet.

  Cela n’accorde pas implicitement des droits au projet à chaque membre du groupe. Pour que les droits du projet soient respectés, les utilisateurs doivent faire partager le projet avec eux.

  Bien que les utilisateurs puissent appartenir à plusieurs groupes, un projet peut être associé à un seul groupe. Les utilisateurs d’autres groupes peuvent toujours travailler sur le même projet, si le projet a été partagé avec eux ou avec leurs groupes. Le groupe associé au projet est généralement soit le groupe responsable de la réalisation du projet, soit le groupe pour lequel le projet est diffusé.

  Pour plus d’informations sur l’association d’un projet à un groupe, voir [Gestion des informations dans la zone Aperçu du projet](../../../manage-work/projects/manage-projects/understand-project-overview-area.md).

* **Portfolio, programme ou entreprise** : lorsque vous créez ou modifiez un portefeuille, un programme ou une entreprise, vous pouvez lui affecter un seul groupe pour lui indiquer que le groupe en est propriétaire ou responsable. Grâce à cette association, les administrateurs et les utilisateurs peuvent facilement identifier les portefeuilles, programmes et entreprises sur lesquels travaillent leurs groupes.

  Par exemple, un administrateur de groupe peut répertorier tous les portefeuilles de l’organisation à l’aide d’une liste ou d’un rapport et noter, dans la colonne Groupe , les portefeuilles auxquels son groupe est affecté.

  >[!NOTE]
  >
  >L’affectation d’un groupe à un portefeuille, un programme ou une entreprise avec un groupe ne signifie pas automatiquement que les informations qu’il contient ont accès à ses données. Vous devez partager manuellement l’accès aux données avec le groupe avant qu’il ne puisse les voir.

  Pour obtenir des instructions, voir [Création d’un portefeuille](../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md), [Création d’un programme](../../../manage-work/portfolios/create-and-manage-programs/create-program.md) et [Création et modification d’entreprises](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

* **Processus d’approbation** : vous pouvez rendre un processus d’approbation disponible pour les projets, les tâches et les problèmes appartenant à un certain groupe. Pour plus d’informations, voir [Création d’un processus d’approbation pour les tâches](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).
* **Chemin d’accès au jalon** : vous pouvez autoriser les utilisateurs de certains groupes à utiliser un chemin d’accès au jalon avec leurs projets. Pour plus d’informations, voir [Création d’un chemin de jalon](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md).
* **Modèle de mise en page** : vous pouvez accorder aux administrateurs d’un groupe l’autorisation de modifier un modèle de mise en page. Pour plus d’informations, voir [Octroi d’un accès administratif pour un modèle de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/grant-admin-access-layout-template.md).

* **Profil de la feuille de temps** : vous pouvez accorder aux administrateurs d’un groupe l’autorisation de modifier un profil de feuille de temps. Pour plus d’informations, voir [Créer, modifier et affecter des profils de feuille de temps](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

* **Planifications** : vous pouvez accorder aux administrateurs d’un groupe l’autorisation de modifier une planification. Pour plus d’informations, voir [Création d’une planification](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).
* **Équipes** : vous pouvez associer un groupe à une équipe afin que les administrateurs des groupes et de leurs sous-groupes puissent afficher et travailler avec ces équipes dans la zone Groupes. Pour plus d’informations, voir [Créer une équipe](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md) ou [Modifier les paramètres de l’équipe](../../../people-teams-and-groups/create-and-manage-teams/edit-team-settings.md).
* **Modèle** : vous pouvez affecter un groupe à un modèle de projet. Cela peut vous aider à rationaliser le processus de création de projet et à identifier plus facilement les groupes qui possèdent les modèles de projet et à créer des rapports sur ces groupes. Pour plus d’informations, reportez-vous à la section [Présentation](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#overview) de l’article [Modifier les modèles de projet](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

* **Éléments récemment supprimés et restaurés** : vous pouvez afficher et gérer les groupes d’éléments récemment supprimés. Pour plus d’informations, voir [Affichage et gestion des éléments récemment supprimés d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-deleted-objects.md) et [Affichage et gestion des éléments récemment restaurés d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-restored-objects.md).
