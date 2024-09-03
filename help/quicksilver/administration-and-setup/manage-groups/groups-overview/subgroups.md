---
user-type: administrator
content-type: reference;overview
product-area: system-administration;user-management
navigation-topic: groups-overview
title: Présentation des sous-groupes
description: Vous pouvez créer jusqu’à 14 niveaux de sous-groupes dans un même groupe. Dans chaque niveau, vous pouvez créer un nombre illimité de sous-groupes parallèles.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: a4280498-6719-4911-a69a-b715a5438eed
source-git-commit: 01487bb9cb195d6fa89bbe0fbdb7678254642714
workflow-type: tm+mt
source-wordcount: '639'
ht-degree: 99%

---

# Vue d’ensemble des sous-groupes

Vous pouvez créer jusqu’à 14 niveaux de sous-groupes dans un même groupe. Dans chaque niveau, vous pouvez créer un nombre illimité de sous-groupes parallèles. Pour obtenir des instructions, voir [Créer un sous-groupe](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).

Pour plus d’informations sur les groupes, voir [Vue d’ensemble des groupes](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

## De quoi héritent les sous-groupes ?

Les sous-groupes héritent de l’appartenance de leur groupe parent. Ainsi, les utilisateurs et utilisatrices et les groupes d’un sous-groupe ont la même visibilité, les mêmes autorisations et le même accès à tous les objets, car ils appartiennent au même groupe parent.

En outre, un sous-groupe hérite automatiquement des administrateurs et administratrices de son groupe de niveau supérieur, mais vous pouvez également définir des personnes membres d’un sous-groupe pour agir en tant qu’administrateurs et administratrices de groupe.

>[!TIP]
>
>Parfois, vous pouvez utiliser des sous-groupes pour ajouter plusieurs utilisateurs et utilisatrices à un groupe existant afin de leur donner accès à un objet dont ils ont besoin.
>
>Supposons, par exemple, que vous ayez un groupe de personnes techniciennes du centre d’assistance et un groupe distinct de directeurs et directrices informatiques. Le groupe du centre d’assistance dispose d’autorisations sur une certaine file d’attente des demandes. Vous souhaitez ajouter les directeurs et directrices informatiques au groupe du centre d’assistance afin qu’ils disposent également des autorisations sur la file d’attente des demandes. Sans la fonctionnalité du sous-groupe, vous devriez ajouter manuellement les directeurs et directrices informatiques au groupe du centre d’assistance, ce qui pourrait être inefficace et difficile à gérer. Si vous ajoutez le groupe des directeurs et directrices informatiques au groupe du centre d’assistance sous la forme d’un sous-groupe, vous effectuez cette tâche plus rapidement en une seule modification.

>[!NOTE]
>
>Si vous avez ajouté une personne séparément à un sous-groupe et à son groupe parent, le fait de la supprimer de l’un ne la supprime pas de l’autre. Si vous ne souhaitez pas que l’accès de la personne soit autorisé pour le groupe parent, vous devez la supprimer du sous-groupe et du groupe parent.

## Sous-groupes publics et privés

Pour un groupe public, toute personne (faisant partie ou non du groupe) disposant d’un accès d’édition peut ajouter le groupe au profil d’autres utilisateurs et utilisatrices. Cette personne ne peut pas effectuer cette action pour un groupe privé.

Vous ne pouvez modifier cette option que pour le groupe parent situé au niveau le plus haut d’une hiérarchie de groupes à plusieurs niveaux. Tous les sous-groupes du groupe parent héritent de ce paramètre.

Par défaut, si vous créez un sous-groupe dans un groupe public, le sous-groupe est également public. Pour plus d’informations sur la création d’un groupe et la manière de le rendre public, voir [Créer un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md). Pour plus d’informations sur l’accès nécessaire pour modifier les utilisateurs et utilisatrices, voir  [Accorder l’accès aux utilisateurs et utilisatrices](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

Tout groupe que vous ajoutez à un groupe existant devient automatiquement un sous-groupe et n’est plus un groupe principal. Toutefois, le sous-groupe conserve ses utilisateurs et utilisatrices existants, ainsi que toute association avec des projets, des problèmes et des tâches, en plus de tous les statuts de projet, de tâche et de problème qui appartiennent au nouveau groupe parent.

## Administrateurs et administratrices de groupes pour les sous-groupes

<!--
Group Admins of a subgroup can't manage statuses or project preferences of the subgroup YET (Sprint 22/Oct 28, 2020)</p>
-->

Vous pouvez définir des personnes membres de sous-groupe en tant qu’administrateurs et administratrices au sous-groupe lorsque vous le créez ou que vous le modifiez. Pour obtenir des instructions, voir [](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#create) dans l’article [Créer un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

Vous pouvez également laisser l’administration du sous-groupe aux administrateurs et administratrices affectés aux groupes de niveau supérieur. Lorsque vous créez un sous-groupe, les administrateurs et administratrices des groupes de niveau supérieur disposent automatiquement d’un accès pour le gérer.

>[!NOTE]
>
>Si vous ajoutez une personne à un sous-groupe et qu’elle gère l’administration d’un groupe de niveau supérieur, elle dispose des droits d’administration pour gérer le sous-groupe, même si elle n’est pas définie en tant que personne administratrice de groupe.

Pour savoir quelles actions sont disponibles pour un administrateur ou une administratrice Adobe Workfront qui gère le système Workfront, un groupe de niveau supérieur ou un sous-groupe, voir [Actions autorisées pour différents types d’administrateurs et administratrices](../../../administration-and-setup/manage-groups/group-roles/group-actions-allowed-different-types-admins.md).
