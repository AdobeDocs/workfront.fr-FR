---
title: Présentation des groupes d’accueil
user-type: administrator
product-area: system-administration;user-management
navigation-topic: groups-overview
description: Un groupe d’accueil est attribué dans le profil de l’utilisateur. Tous les utilisateurs doivent disposer d’un groupe d’accueil.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 89adb9ea-bfde-4c0d-9fec-b1f97e925340
source-git-commit: 01487bb9cb195d6fa89bbe0fbdb7678254642714
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 0%

---

# Vue d’ensemble des groupes résidentiels

Un groupe d’accueil est attribué dans le profil de l’utilisateur. Tous les utilisateurs doivent disposer d’un groupe d’accueil. Un utilisateur peut appartenir à plusieurs groupes, mais il ne peut avoir qu’un seul groupe d’accueil. Pour plus d’informations sur les groupes, voir [Présentation des groupes](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

Bien que tout groupe existant dans le système puisse être affecté en tant que groupe d’accueil d’un utilisateur, nous vous recommandons de créer et d’affecter de nouveaux groupes représentant des entités organisationnelles plus importantes.

Lors de la création de groupes d’accueil, considérez la manière dont votre entreprise divise vos utilisateurs Adobe Workfront. Voici quelques suggestions pour déterminer le type de groupes à utiliser comme groupe d’accueil :

* Groupes représentant des services, tels que l’informatique ou le marketing
* Groupes régis par différents budgets
* Groupes situés dans différentes zones ou régions
* Groupes composés de plusieurs équipes appartenant au même centre de coûts

>[!NOTE]
>
>Si vous devez réorganiser vos groupes d’accueil en entités organisationnelles, vous devez utiliser la commande>
>1. Créez le groupe, comme expliqué dans la section [Créer un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).
>1. Réaffectez le nouveau groupe en tant que groupe d’accueil de l’utilisateur, comme expliqué dans la section [Modification du profil d’un utilisateur](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).
>

## Gestion des modèles de mise en page

Lorsque vous attribuez un modèle de mise en page à un groupe, tous les utilisateurs auxquels le groupe est affecté en tant que groupe d’accueil peuvent voir les paramètres spécifiés dans le modèle de mise en page.

Si un modèle de mise en page est affecté à un groupe d’accueil, il n’est visible que par les utilisateurs affectés à ce groupe.

Pour plus d’informations, voir [Créer et gérer des modèles de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md) dans [Créer et gérer des modèles de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

## Gestion des licences

Chaque utilisateur ne peut être affecté qu’à un seul groupe d’accueil, ce qui facilite la gestion du nombre de licences.

Les administrateurs de Workfront ont la possibilité de définir le nombre maximal de licences pour les groupes d’accueil.

La définition d’un nombre maximal de licences permet aux administrateurs de Workfront d’empêcher une unité opérationnelle d’utiliser les licences Workfront achetées pour d’autres unités opérationnelles.

Pour plus d’informations, voir [Gestion des licences disponibles dans votre système](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).
