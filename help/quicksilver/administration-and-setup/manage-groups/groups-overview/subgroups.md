---
user-type: administrator
content-type: reference;overview
product-area: system-administration;user-management
navigation-topic: groups-overview
title: Présentation des sous-groupes
description: Vous pouvez créer jusqu’à 14 niveaux de sous-groupes dans un seul groupe. À l’un de ces niveaux, vous pouvez créer un nombre illimité de sous-groupes parallèles.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: a4280498-6719-4911-a69a-b715a5438eed
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '637'
ht-degree: 0%

---

# Présentation des sous-groupes

Vous pouvez créer jusqu’à 14 niveaux de sous-groupes dans un seul groupe. À l’un de ces niveaux, vous pouvez créer un nombre illimité de sous-groupes parallèles. Pour obtenir des instructions, voir [Création d’un sous-groupe](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).

Pour plus d’informations sur les groupes, voir [Présentation des groupes](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

## Qu’héritent les sous-groupes ?

Les sous-groupes héritent de l’appartenance de leur groupe parent. Ainsi, les utilisateurs et les groupes d’un sous-groupe ont la même visibilité, les mêmes autorisations et le même accès à tous les objets en tant qu’utilisateurs et groupes appartenant au groupe parent qu’ils partagent.

En outre, un sous-groupe hérite automatiquement des administrateurs de groupe de son groupe de niveau supérieur, mais vous pouvez également affecter des membres d’un sous-groupe pour agir en tant qu’administrateurs de groupe.

>[!TIP]
>
>Parfois, vous pouvez utiliser des sous-groupes pour ajouter plusieurs utilisateurs à un groupe existant afin de leur donner accès à un objet dont ils ont besoin.
>
>Supposons, par exemple, que vous ayez un groupe de techniciens du service d’assistance et un groupe distinct de directeurs informatiques. Le groupe du service d’assistance dispose d’autorisations sur une certaine file d’attente de requêtes. Vous souhaitez ajouter les directeurs informatiques au groupe du service d’assistance afin qu’ils disposent également des autorisations sur la file d’attente des demandes. Sans la fonctionnalité du sous-groupe, vous devrez ajouter manuellement les directeurs informatiques au groupe du service d’assistance, ce qui pourrait être inefficace et difficile à gérer. Si vous ajoutez le groupe des directeurs informatiques au groupe du service d’assistance sous forme de sous-groupe, vous effectuez cette tâche plus rapidement avec une seule modification.

>[!NOTE]
>
>Si un utilisateur a été ajouté séparément à un sous-groupe et à son groupe parent, le fait de le supprimer de l’un ne le supprime pas de l’autre. Si vous ne souhaitez pas que l’accès de l’utilisateur soit autorisé pour le groupe parent, vous devez le supprimer du sous-groupe et du groupe parent.

## Sous-groupes publics et privés

Pour un groupe public, tout utilisateur (dans ou hors du groupe) disposant d’un accès utilisateur d’édition peut ajouter le groupe au profil d’autres utilisateurs. Ils ne peuvent pas le faire pour un groupe privé.

Vous ne pouvez modifier cette option que sur le groupe parent supérieur d’une hiérarchie de groupes comportant plusieurs niveaux. Tous les sous-groupes du groupe parent héritent de son paramètre.

Si vous créez un sous-groupe sous un groupe qui est public, le sous-groupe est également public, par défaut. Pour plus d’informations sur la création d’un groupe et sa publication, voir [Création d’un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md). Pour plus d’informations sur l’accès nécessaire à la modification des utilisateurs, voir [Accorder l’accès aux utilisateurs](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

Tout groupe que vous ajoutez à un groupe existant devient automatiquement un sous-groupe et n’est plus un groupe principal. Toutefois, le sous-groupe conserve ses utilisateurs existants, ainsi que toute association avec des projets, des problèmes et des tâches, en plus de tous les états de projet, de tâche et d’émission qui appartiennent au nouveau groupe parent.

## Administrateurs de groupe pour les sous-groupes

<!--
Group Admins of a subgroup can't manage statuses or project preferences of the subgroup YET (Sprint 22/Oct 28, 2020)</p>
-->

Vous pouvez affecter des membres de sous-groupe en tant qu’administrateurs de groupe au sous-groupe lorsque vous le créez ou que vous le modifiez. Pour obtenir des instructions, voir [](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#create) dans l’article [Création d’un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

Vous pouvez également laisser l’administration du sous-groupe aux administrateurs du groupe affectés aux groupes ci-dessus. Lorsque vous créez un sous-groupe, les administrateurs de groupe au-dessus des groupes ci-dessus disposent d’un accès automatique pour le gérer.

>[!NOTE]
>
>Si vous ajoutez un utilisateur à un sous-groupe et qu’il est administrateur de groupe pour un groupe n’importe où au-dessus du sous-groupe, cet utilisateur dispose des droits d’administration pour gérer le sous-groupe, même sans être affecté en tant qu’administrateur de groupe.

Pour savoir quelles actions sont disponibles pour un administrateur Adobe Workfront qui gère le système Workfront, un administrateur de groupe qui gère un groupe de niveau supérieur et un administrateur de groupe qui gère un sous-groupe, voir [Actions autorisées pour différents types d’administrateurs](../../../administration-and-setup/manage-groups/group-roles/group-actions-allowed-different-types-admins.md).
