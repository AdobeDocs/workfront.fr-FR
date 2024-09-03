---
title: Présentation des groupes
user-type: administrator
content-type: reference;overview
product-area: system-administration;user-management
navigation-topic: groups-overview
description: Un administrateur ou une administratrice Workfront peut créer des groupes d’utilisateurs et d’utilisatrices qui correspondent à la structure de votre service. Les groupes, les équipes et les entreprises partagent des points communs, mais se distinguent par certains aspects.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 1353ab04-7de7-4d30-a092-27807c950777
source-git-commit: 01487bb9cb195d6fa89bbe0fbdb7678254642714
workflow-type: tm+mt
source-wordcount: '927'
ht-degree: 99%

---

# Vue d’ensemble des groupes

<!-- Audited: 01/2024 -->

Un administrateur ou une administratrice Workfront peut créer des groupes d’utilisateurs et d’utilisatrices qui correspondent à la structure de votre service. Les groupes, les équipes et les entreprises partagent des points communs, mais se distinguent par certains aspects.

L’administrateur ou l’administratrice Workfront accorde aux groupes l’accès aux zones Workfront dans lesquelles ils doivent travailler et communiquer. Chaque groupe peut ensuite conserver ses informations Workfront, telles que les utilisateurs et utilisatrices, les modèles, les formulaires personnalisés et les projets, séparément de celles des autres services.

Au moins un administrateur ou une administratrice de groupes est nécessaire pour chaque groupe. Les administrateurs et administratrices de groupes peuvent utiliser la page Groupes pour gérer leurs groupes en un seul endroit. Pour plus d’informations, consultez la section [Administrateurs et administratrices de groupes](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

Vous pouvez créer jusqu’à 14 niveaux de sous-groupes dans un même groupe. Pour plus d’informations, consultez les sections [Vue d’ensemble des sous-groupes](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md) et [Créer un sous-groupe](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).

## Utiliser des groupes pour organiser les utilisateurs et les utilisatrices

En tant qu’équipe d’administration de Workfront ou de groupes, vous pouvez associer des utilisateurs et des utilisatrices à des groupes et des sous-groupes. Si vous rendez un groupe public, les personnes qui disposent d’une licence Standard (nouvelle) ou Plan (actuelle) peuvent y affecter des utilisateurs et des utilisatrices. Pour plus d’informations sur les administrateurs et les administratrices de groupes et les groupes publics, consultez la section [Créer un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

Lorsque vous créez un utilisateur ou une utilisatrice, il est préférable de l’intégrer au bon groupe principal et aux autres groupes pertinents pour son travail. Un utilisateur ou une utilisatrice ne peut avoir qu’un seul groupe principal, mais peut faire partie de plusieurs autres groupes.

Faire partie d’un groupe permet à l’utilisateur ou à l’utilisatrice d’accéder aux objets partagés avec ce groupe et ses sous-groupes. Par exemple, partager un projet avec un groupe permet à tous les utilisateurs et utilisatrices de ce groupe ainsi qu’aux personnes des sous-groupes d’y accéder.

>[!TIP]
>
>Si les services de votre organisation travaillent souvent ensemble pour gérer des projets et les ressources qui y sont affectées, vous n’aurez peut-être pas besoin de les diviser en plusieurs groupes plus petits. Quelques groupes de haut niveau pourraient s’avérer plus efficaces.

Un groupe peut avoir un nombre illimité d’utilisateurs et d’utilisatrices.

Pour plus d’informations sur la création de nouveaux utilisateurs et de nouvelles utilisatrices, consultez la section [Ajouter des utilisateurs et des utilisatrices](../../../administration-and-setup/add-users/add-users.md).

## Accorder à un groupe l’accès aux objets

Lorsque vous partagez un objet avec un groupe, tous les membres de ce groupe (y compris les membres de tous les sous-groupes) ont accès à cet objet. Pour plus d’informations sur le partage dans Workfront, consultez la section [Vue d’ensemble des autorisations de partage sur les objets](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## Associer un groupe à un objet

Lorsque vous créez ou modifiez l’un des objets Workfront suivants, vous pouvez l’associer à un groupe :

* **Projet** : vous pouvez associer un seul groupe à un projet pour indiquer qui est propriétaire du projet.

  Cette action n’accorde pas implicitement des droits sur le projet à chaque membre du groupe. Pour que les droits sur le projet leur soient accordés, le projet doit être partagé avec les utilisateurs et les utilisatrices.

  Bien que les utilisateurs et les utilisatrices puissent appartenir à plusieurs groupes, un projet peut être associé à un seul groupe. Les personnes faisant partie d’autres groupes peuvent toujours travailler sur le même projet, s’il a été partagé avec elles ou leurs groupes. Le groupe associé au projet est généralement soit le groupe responsable de la réalisation du projet, soit le groupe pour lequel le projet est réalisé.

  Pour obtenir des instructions sur l’association d’un projet à un groupe, consultez la section [Gérer des informations dans la zone de vue d’ensemble du projet](../../../manage-work/projects/manage-projects/understand-project-overview-area.md).

* **Portfolio, programme ou entreprise** : lorsque vous créez ou modifiez un portfolio, un programme ou une entreprise, vous pouvez lui affecter un seul groupe pour indiquer que le groupe en est propriétaire ou responsable. Grâce à cette association, l’équipe d’administration ainsi que les utilisateurs et les utilisatrices peuvent facilement identifier les portfolios, programmes et entreprises sur lesquels travaillent leurs groupes.

  Par exemple, un administrateur ou une adminstratrice de groupe peut répertorier tous les portfolios de l’entreprise à l’aide d’une liste ou d’un rapport et noter, dans la colonne de groupe, les portfolios auxquels son groupe est affecté.

  >[!NOTE]
  >
  >Affecter un groupe à un portfolio, un programme ou une entreprise ayant un groupe ne signifie pas automatiquement que les informations de ce groupe peuvent accéder à ses données. Vous devez partager manuellement l’accès aux données avec le groupe avant qu’il ne puisse y accéder.

  Pour obtenir des instructions, consultez les sections [Créer un portfolio](../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md), [Créer un programme](../../../manage-work/portfolios/create-and-manage-programs/create-program.md), et [Créer et modifier des entreprises](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

* **Processus d’approbation** : vous pouvez rendre un processus d’approbation disponible pour les projets, tâches et problèmes appartenant à un certain groupe. Pour plus d’informations, consultez la section [Créer un processus d’approbation pour les tâches](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).
* **Chemin jalonné** : vous pouvez autoriser les utilisateurs et les utilisatrices de certains groupes à utiliser un chemin jalonné avec leurs projets. Pour plus d’informations, consultez la section [Créer un chemin jalonné](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md).
* **Modèle de mise en page** : vous pouvez autoriser les administrateurs et les administratrices d’un groupe à modifier un modèle de mise en page. Pour obtenir des instructions, consultez la section [Accorder un accès administratif pour un modèle de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/grant-admin-access-layout-template.md).

* **Profil de feuille de temps** : vous pouvez autoriser les administrateurs et les administratrices d’un groupe à modifier un profil de feuille de temps. Pour plus d’informations, consultez la section [Créer, modifier et affecter des profils de feuille de temps](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

* **Plannings** : vous pouvez autoriser les administrateurs et les administratrices d’un groupe à modifier un planning. Pour plus d’informations, consultez la section [Créer un planning](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).
* **Équipes** : vous pouvez associer un groupe à une équipe afin que les administrateurs et les administratrices des groupes et de leurs sous-groupes puissent afficher et travailler avec ces équipes dans la zone des groupes. Pour plus d’informations, consultez la section [Créer une équipe](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md) ou [Modifier les paramètres de l’équipe](../../../people-teams-and-groups/create-and-manage-teams/edit-team-settings.md).
* **Modèle** : vous pouvez affecter un groupe à un modèle de projet. Cette approche peut simplifier le processus de création de projets et faciliter l’identification des groupes détenant des modèles de projet, permettant ainsi de générer des rapports sur ces groupes de manière plus efficace. Pour plus d’informations, consultez la section [Vue d’ensemble](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#overview) dans l’article [Modifier des modèles de projet](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

* **Éléments récemment supprimés et restaurés** : vous pouvez afficher et gérer les éléments récemment supprimés d’un groupe. Pour plus d’informations, consultez les sections [Afficher et gérer les éléments récemment supprimés d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-deleted-objects.md) et [Afficher et gérer les éléments récemment restaurés d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-restored-objects.md).
