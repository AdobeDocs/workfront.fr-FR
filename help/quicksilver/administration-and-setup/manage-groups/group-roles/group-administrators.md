---
title: Administrateurs de groupe
user-type: administrator
content-type: reference;overview
product-area: system-administration;user-management
navigation-topic: group-roles
description: Les administrateurs et administratrices Adobe Workfront d’une grande entreprise comportant de nombreux services ne souhaitent peut-être pas gérer tous les services de l’entreprise et les groupes au sein de ces services. Au lieu de cela, ils peuvent créer un groupe pour chaque service et des sous-groupes au sein de ce groupe, chacun étant géré par un administrateur ou une administratrice de groupes.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 589cf9fb-f195-4b69-a240-3f73e6ca623e
source-git-commit: bd1a66950c6e16ef7eb05d385bd99fc2d3be35cc
workflow-type: tm+mt
source-wordcount: '1047'
ht-degree: 100%

---

# Administrateurs et administratrices de groupe

<!-- Audited: 12/2023 -->

Les administrateurs et administratrices Adobe Workfront d’une grande entreprise comportant de nombreux services ne souhaitent peut-être pas gérer tous les services de l’entreprise et les groupes au sein de ces services. Au lieu de cela, ils peuvent créer un groupe pour chaque service et des sous-groupes au sein de ce groupe, chacun étant géré par un administrateur ou une administratrice de groupes.

Un administrateur ou une administratrice de groupes peut gérer les besoins d’un groupe, tels que l’adhésion des personnes, les modèles de mise en page, les données personnalisées, les statuts et les préférences.

Jusqu’à 14 niveaux de sous-groupes peuvent exister sous un seul groupe.

>[!NOTE]
>
>Tous les administrateurs et administratrices de groupes dans la hiérarchie au-dessus d’un sous-groupe ont des droits administratifs pour gérer ce sous-groupe.

Pour plus d’informations sur la création et la gestion des groupes, voir [Créer un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md) et [Gérer un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md). Voir également [Vue d’ensemble des sous-groupes](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

## Désigner les administrateurs et administratrices de groupes

Le groupe doit avoir au moins une personne chargée de l’administration de groupes. Une personne chargée de l’administration Workfront ou de groupes peut affecter des administrateurs et administratrices de groupes aux sous-groupes du groupe, mais ce n’est pas obligatoire. Pour plus d’informations, voir [Créer un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

Si vous êtes un administrateur ou une administratrice Workfront, nous vous recommandons de procéder comme suit avant de désigner des personnes comme administrateurs et administratrices de groupes :

* Notez le nombre actuel d’administrateurs et administratrices Workfront dans votre système.
* Notez le nombre de groupes que vous avez dans votre système.
* Déterminez si vous pouvez modifier le niveau d’accès de certains administrateurs et administratrices Workfront et les désigner comme administrateurs et administratrices de groupes.

  Pour plus d’informations sur les capacités des administrateurs et administratrices de groupe, voir [Tâches effectuées par les administrateurs et administratrices de groupes](#tasks-done-by-group-administrators) dans cet article.

* Déterminez si vous souhaitez que les administrateurs et administratrices de groupes puissent se connecter en tant qu’autres personnes ou réinitialiser les mots de passe des utilisateurs et utilisatrices des groupes que vous administrez. Un accès supplémentaire est nécessaire pour effectuer ces tâches, comme expliqué ci-dessous dans [Accès nécessaire pour les administrateurs et administratrices de groupes](#access-needed-for-group-administrators).
* Pour une meilleure gestion des utilisateurs et utilisatrices, il est possible d’affecter des groupes ou des sous-groupes au lieu d’utilisateurs et d’utilisatrices pour les objets suivants :

   * Modèle de mise en page
   * Planifications
   * Profils de feuilles de temps

## Accès nécessaire pour les administrateurs et administratrices de groupes {#access-needed-for-group-administrators}

Chaque personne chargée de l’administration de groupes doit disposer des éléments suivants :

* Licence Plan dans le modèle actuel de tarification et de packaging
* Licence Standard dans le nouveau modèle de tarification et de packaging

Nous recommandons que les administrateurs et administratrices de groupes aient un accès Modifier aux utilisateurs et utilisatrices afin qu’ils puissent effectuer les tâches suivantes :

* Se connecter en tant qu’autres personnes dans les groupes et sous-groupes qu’ils gèrent.
* Réinitialiser le mot de passe d’une autre personne dans les groupes qu’ils gèrent.

>[!IMPORTANT]
>
>Les administrateurs et administratrices de groupes doivent disposer d’un accès supérieur par rapport aux personnes qu’ils gèrent ; dans le cas contraire, ils ne pourront pas consulter ou modifier les niveaux d’accès inférieurs.
>Pour savoir comment accorder cet accès, voir [Créer ou modifier des niveaux d’accès personnalisés](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Pour un administrateur ou une administratrice de groupes qui doit attribuer des profils de feuilles de temps aux personnes de ses groupes et sous-groupes, nous recommandons également l’accès administratif aux feuilles de temps et aux heures. Pour savoir comment accorder cet accès, voir [Accorder aux utilisateurs et utilisatrices un accès administratif à certaines zones](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

## Tâches effectuées par les administrateurs et administratrices de groupes {#tasks-done-by-group-administrators}

En tant qu’administrateur ou administratrice de groupes, vous pouvez effectuer les tâches décrites ci-dessous pour gérer les groupes que vous supervisez. Certaines de ces capacités sont les mêmes que celles accordées à un administrateur ou à une administratrice Workfront.

>[!NOTE]
>
>Dans le nouveau modèle de tarification et de packaging, vous devez disposer d’une formule Prime ou supérieure pour effectuer les opérations suivantes :
>
> * Créer des notifications d’événement de groupe
> * Configurer les préférences des projets de groupe
> * Configurer les préférences des groupes en matière de tâches et de problèmes
> * Déverrouiller la configuration des préférences des sous-groupes
> * Préférences de feuilles de temps et d’heures pour les groupes
> * Déverrouiller les préférences en matière de feuilles de temps et d’heures

### Gérer les personnes membres du groupe {#manage-group-members}

* Créez, modifiez et supprimez des sous-groupes au sein des groupes et sous-groupes que vous gérez. Pour plus d’informations, voir [Créer un sous-groupe](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).
* Ajoutez à vos groupes et sous-groupes tous les utilisateurs et utilisatrices pour lesquels vous disposez d’un accès en modification. Vous pouvez également ajouter des utilisateurs et utilisatrices à des groupes et sous-groupes en modifiant leur profil.

  Vous pouvez également mettre à jour les champs du profil d’une personne membre d’un groupe si vous disposez de l’autorisation Administration des utilisateurs et utilisatrices (utilisateurs et utilisatrices du groupe) dans votre niveau d’accès.

  Pour plus d’informations, consultez [Modifier le profil d’un utilisateur ou d’une utilisatrice](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

  >[!NOTE]
  >
  >Les administrateurs et administratrices Workfront peuvent annuler les modifications apportées par un administrateur ou une administratrice de groupes à l’appartenance à un groupe.

* Réinitialiser les mots de passe des personnes membres des groupes que vous gérez. Pour plus d’informations, consultez la section [Modifier le profil d’un utilisateur ou d’une utilisatrice](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).
* Se connecter en tant qu’utilisateur ou utilisatrice membre des groupes que vous gérez. Pour plus d’informations, consultez [Se connecter en tant qu’un autre utilisateur ou qu’une autre utilisatrice](../../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).
* Afficher le nombre de licences disponibles pour votre groupe et les sous-groupes situés en dessous. Pour plus d’informations, consultez [Gérer les licences disponibles dans votre système](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

### Gérer les objets des groupes {#manage-group-objects}

* Créez des modèles de mise en page au niveau du groupe et associez-les aux groupes et sous-groupes que vous gérez. Pour plus d’informations, consultez [Créer et gérer des modèles de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
* Créez des profils de feuille de temps au niveau du groupe, associez-les aux utilisateurs et utilisatrices et aux groupes que vous gérez et générez manuellement des feuilles de temps. Pour plus d’informations, consultez [Créer, modifier et attribuer des profils de feuille de temps](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).
* Sans accès administratif aux processus d’approbation, créez et modifiez les processus d’approbation pour les groupes et sous-groupes que vous gérez. Pour plus d’informations, consultez [Créer un processus d’approbation pour les éléments de travail](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

  Pour plus d’informations sur l’accès administratif aux processus d’approbation, consultez [Accorder un accès administratif à certaines zones aux utilisateurs et utilisatrices](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Créez des plannings et associez-les à un groupe que vous gérez. Pour plus d’informations, consultez [Créer un planning](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).
* Gérez une équipe affectée à un groupe que vous gérez, sans être membre de l’équipe. Créez également un rapport d’équipe basé sur le champ Groupe afin d’identifier le groupe auquel une équipe donnée est affectée. Pour plus d’informations, consultez [Créer une équipe](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md).
* Restaurez un projet associé au groupe que vous gérez, ainsi que les tâches, problèmes ou documents associés au projet. Pour plus d’informations, consultez [Restaurer les éléments supprimés](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

### Gérer les préférences et les outils des groupes {#manage-group-preferences-and-tools}

* Lorsqu’une préférence de projet, une préférence de tâche ou de problème, ou une préférence de feuilles de temps et d’heures est déverrouillée pour les groupes dans l’ensemble du système, modifiez cette préférence pour les groupes que vous gérez. Ces préférences ont un impact sur le comportement des projets, des tâches et des problèmes. Pour plus d’informations, consultez les sections suivantes :

   * [Configurer les préférences de projet pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md)
   * [Configurer les préférences de tâches et de problèmes pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)

* Créez et modifiez les statuts des groupes que vous gérez. Pour plus d’informations, consultez [Créer ou modifier un statut de groupe](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
* Configurez une notification d’événement pour les groupes que vous gérez. Vous ne pouvez le faire qu’après qu’un administrateur ou une administratrice Workfront a déverrouillé la possibilité de configurer les notifications d’événements pour les groupes dans l’ensemble du système. Pour plus d’informations, consultez [Afficher et configurer les notifications d’événements pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).
