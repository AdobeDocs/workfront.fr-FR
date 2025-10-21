---
title: Présentation des groupes principaux
user-type: administrator
product-area: system-administration;user-management
navigation-topic: groups-overview
description: Les groupe principaux sont attribués dans les profils des utilisateurs et utilisatrices. Tous les utilisateurs doivent disposer d’un groupe principal.
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 89adb9ea-bfde-4c0d-9fec-b1f97e925340
source-git-commit: cd0214917620e0b147d0da3402ea2d34e28bc9c3
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 92%

---

# Vue d’ensemble des groupes principaux

Les groupe principaux sont attribués dans les profils des utilisateurs et utilisatrices. Toute personne doit intégrer un groupe principal. Une personne peut appartenir à plusieurs groupes, mais elle ne peut intégrer qu’un seul groupe principal. Pour plus d’informations sur les groupes, consultez la section [Vue d’ensemble des groupes](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

Bien que tout groupe existant dans le système puisse être affecté à une personne en tant que groupe principal, nous vous recommandons de créer et d’affecter de nouveaux groupes représentant des entités organisationnelles plus importantes.

Lors de la création de groupes principaux, tenez compte de la manière dont votre entreprise répartit vos utilisateurs et utilisatrices Adobe Workfront. Voici quelques suggestions pour déterminer le type de groupes à utiliser comme groupe principal :

* groupes représentant des services, tels que l’informatique ou le marketing ;
* groupes régis par différents budgets ;
* groupes situés dans différentes zones ou régions ;
* groupes composés de plusieurs équipes appartenant au même centre de coûts.

>[!NOTE]
>
>Si vous devez réorganiser vos groupes principaux en entités organisationnelles, vous devez :
>
>1. créer un groupe en suivant la procédure décrite à la section [Créer un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md) ;
>1. réaffecter le nouveau groupe en tant que groupe principal de l’utilisateur ou de l’utilisatrice, comme expliqué à la section [Modifier le profil d’une personne](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Gestion des modèles de mise en page

Lorsque vous attribuez un modèle de mise en page à un groupe, toutes les personnes affectées à ce groupe en tant que groupe principal peuvent voir les paramètres spécifiés dans le modèle de mise en page.

Si un modèle de mise en page est affecté à un groupe principal, il n’est visible que par les personnes affectées à ce groupe.

Pour plus d’informations, consultez la section [Créer et gérer des modèles de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md) de l’article [Créer et gérer des modèles de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

## Gestion des licences

Les utilisateurs et utilisatrices ne peuvent être affectés qu’à un seul groupe principal, ce qui facilite la gestion du nombre de licences.

L’administration Workfront a la possibilité de définir le nombre maximal de licences pour les groupes principaux.

L’administration Workfront peut ainsi empêcher une unité opérationnelle d’utiliser les licences Workfront achetées pour d’autres unités opérationnelles.

Pour plus d’informations, consultez la section [Gérer les licences disponibles dans votre système](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).
