---
title: Administrateurs et administratrices de groupe
user-type: administrator
content-type: reference;overview
product-area: system-administration;user-management
navigation-topic: group-roles
description: Les administrateurs Adobe Workfront d’une grande entreprise comptant de nombreux services peuvent ne pas vouloir gérer tous les services et groupes de l’entreprise au sein de ces services. Au lieu de cela, ils peuvent créer un groupe pour chaque service et sous-groupe au sein de ce groupe, chacun géré par un administrateur de groupe.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 589cf9fb-f195-4b69-a240-3f73e6ca623e
source-git-commit: 850e0801511177efc5189258acd9b88234cf59c9
workflow-type: tm+mt
source-wordcount: '1047'
ht-degree: 5%

---

# Administrateurs et administratrices de groupe

<!-- Audited: 12/2023 -->

Les administrateurs Adobe Workfront d’une grande entreprise comptant de nombreux services peuvent ne pas vouloir gérer tous les services et groupes de l’entreprise au sein de ces services. Au lieu de cela, ils peuvent créer un groupe pour chaque service et sous-groupe au sein de ce groupe, chacun géré par un administrateur de groupe.

Un administrateur de groupe peut gérer les besoins d’un groupe, tels que l’adhésion de l’utilisateur, les modèles de mise en page, les données personnalisées, les états et les préférences.

Jusqu’à 14 niveaux de sous-groupes peuvent exister sous un seul groupe.

>[!NOTE]
>
>Tous les administrateurs de groupe dans la hiérarchie au-dessus d’un sous-groupe disposent de droits d’administration pour gérer ce sous-groupe.

Pour plus d’informations sur la création et la gestion des groupes, voir [Création d’un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md) et [Gestion d’un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md). Voir aussi [Présentation des sous-groupes](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

## Désignation des administrateurs de groupe

Chaque groupe de niveau supérieur doit avoir au moins un administrateur de groupe. Un administrateur ou administrateur Workfront d’un groupe peut affecter des administrateurs de groupe aux sous-groupes du groupe, mais cela n’est pas obligatoire. Pour plus d’informations, voir [Création d’un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

Si vous êtes administrateur Workfront, nous vous recommandons d’effectuer les opérations suivantes avant de désigner des utilisateurs en tant qu’administrateurs de groupe :

* Notez le nombre actuel d’administrateurs Workfront dans votre système.
* Notez le nombre de groupes présents dans votre système.
* Déterminez si vous pouvez modifier le niveau d’accès de certains administrateurs Workfront et désigner ces derniers comme administrateurs de groupe à la place.

  Pour plus d’informations sur les fonctionnalités des administrateurs de groupe, voir [Tâches effectuées par les administrateurs de groupe](#tasks-done-by-group-administrators) dans cet article.

* Déterminez si vous souhaitez que les administrateurs de groupe puissent se connecter en tant qu’autres utilisateurs ou réinitialiser les mots de passe des utilisateurs dans les groupes que vous administrez. Un accès supplémentaire est nécessaire pour effectuer ces tâches, comme expliqué ci-dessous dans la section [Accès requis pour les administrateurs de groupe](#access-needed-for-group-administrators).
* Pour une meilleure gestion des utilisateurs, envisagez d’affecter des groupes ou des sous-groupes plutôt que des utilisateurs aux objets suivants :

   * Modèles de mise en page
   * Planifications
   * Profils de feuilles de temps

## Accès requis pour les administrateurs de groupe {#access-needed-for-group-administrators}

Chaque administrateur de groupe doit disposer des

* Une licence Plan dans le modèle de tarification et de package actuel
* Une licence standard dans le nouveau modèle de tarification et de package

Nous recommandons aux administrateurs de groupe de disposer de l’accès Modifier aux utilisateurs afin qu’ils puissent effectuer les tâches suivantes :

* Connectez-vous en tant qu’autres utilisateurs dans les groupes et sous-groupes qu’ils gèrent.
* Réinitialisez le mot de passe d’un autre utilisateur dans les groupes qu’il gère.

>[!IMPORTANT]
>
>Les administrateurs de groupe doivent disposer d’un accès supérieur à celui qu’ils gèrent ; dans le cas contraire, ils ne pourront pas afficher ni modifier les niveaux d’accès inférieurs.
>Pour obtenir des instructions sur l’octroi de cet accès, voir [Création ou modification de niveaux d’accès personnalisés](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Pour un administrateur de groupe qui doit affecter des profils de feuille de temps aux utilisateurs de leurs groupes et sous-groupes, nous vous recommandons également d’accéder aux feuilles de temps et heures de manière administrative. Pour obtenir des instructions sur l&#39;octroi de cet accès, voir [Octroi aux utilisateurs d&#39;un accès administratif à certaines zones](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

## Tâches effectuées par les administrateurs de groupe {#tasks-done-by-group-administrators}

En tant qu’administrateur de groupe, vous pouvez effectuer les tâches décrites ci-dessous pour gérer les groupes que vous supervoyez. Certaines d’entre elles sont identiques à celles offertes à un administrateur Workfront.

>[!NOTE]
>
>Dans le nouveau modèle de tarification et de conditionnement, vous devez avoir un plan Prime ou supérieur pour effectuer les opérations suivantes :
>
> * Créer des notifications d’événement de groupe
> * Configurer les préférences des projets de groupe
> * Configurer les préférences des groupes en matière de tâches et de problèmes
> * Déverrouiller la configuration des préférences des sous-groupes
> * Préférences des groupes en matière de feuilles de temps et d’heures
> * Déverrouiller les préférences en matière de feuilles de temps et d’heures

### Gestion des membres de groupe {#manage-group-members}

* Créez, modifiez et supprimez des sous-groupes dans les groupes et sous-groupes que vous gérez. Pour obtenir des instructions, voir [Création d’un sous-groupe](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).
* Ajoutez tous les utilisateurs pour lesquels vous avez l’accès Modifier à vos groupes et sous-groupes. Vous pouvez également ajouter des utilisateurs à des groupes et des sous-groupes en modifiant leurs profils.

  Vous pouvez également mettre à jour les champs du profil d’un membre du groupe si l’autorisation Admin utilisateur (Utilisateurs de groupe) est activée dans votre niveau d’accès.

  Pour plus d’informations, voir [Modification du profil d’un utilisateur](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

  >[!NOTE]
  >
  >Les administrateurs Workfront peuvent remplacer les modifications apportées aux appartenances à un groupe par un administrateur de groupe.

* Réinitialisez les mots de passe des utilisateurs membres des groupes que vous gérez. Pour plus d’informations, voir [Modification du profil d’un utilisateur](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).
* Connectez-vous en tant qu’utilisateurs membres des groupes que vous gérez. Pour plus d’informations, consultez [Se connecter en tant qu’autre utilisateur ou utilisatrice](../../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).
* Affichez le nombre de licences disponibles pour votre groupe et les sous-groupes situés en dessous. Pour plus d’informations, voir [Gestion des licences disponibles dans votre système](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

### Gérer les objets des groupes {#manage-group-objects}

* Créez des modèles de mise en page au niveau du groupe et associez-les aux groupes et aux sous-groupes que vous gérez. Pour plus d’informations, voir [Créer et gérer des modèles de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
* Créez des profils de feuille de temps au niveau du groupe, associez-les aux utilisateurs et aux groupes que vous gérez, puis générez manuellement des feuilles de temps. Pour plus d’informations, voir [Créer, modifier et affecter des profils de feuille de temps](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).
* Sans accès administratif aux processus de validation, créez et éditez des processus de validation pour les groupes et sous-groupes que vous gérez. Pour plus d’informations, voir [Création d’un processus d’approbation pour les tâches](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

  Pour plus d&#39;informations sur l&#39;accès administratif aux processus de validation, voir [Octroi aux utilisateurs d&#39;un accès administratif à certaines zones](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Créez des planifications et associez-les à un groupe que vous gérez. Pour plus d’informations, voir [Création d’une planification](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).
* Gérez une équipe affectée à un groupe que vous gérez, sans être membre de l’équipe. Créez également un rapport d’équipe basé sur le champ Groupe afin d’identifier le groupe auquel une certaine équipe est affectée. Pour plus d’informations, voir [Création d’une équipe](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md).
* Restaurez un projet associé à un groupe que vous gérez, ainsi que les tâches, problèmes ou documents associés au projet. Pour plus d’informations, voir [Restaurer les éléments supprimés](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

### Gestion des préférences et des outils de groupe {#manage-group-preferences-and-tools}

* Lorsqu’une préférence de projet, de tâche ou d’émission, ou une préférence de temps et d’heure est déverrouillée pour les groupes dans l’ensemble du système, modifiez cette préférence pour les groupes que vous gérez. Ces préférences ont un impact sur le projet, la tâche et le comportement du problème. Pour plus d’informations, voir :

   * [Configuration des préférences de projet pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md)
   * [Configuration des préférences de tâche et de problème pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)

* Créez et modifiez des états de groupe pour les groupes que vous gérez. Pour plus d’informations, voir [Création ou modification de l’état d’un groupe](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
* Configurez une notification d’événement pour les groupes que vous gérez. Vous ne pouvez le faire qu’après qu’un administrateur Workfront a déverrouillé la possibilité de configurer des notifications d’événement pour des groupes dans le système. Pour plus d’informations, voir [Afficher et configurer des notifications d’événement pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).
