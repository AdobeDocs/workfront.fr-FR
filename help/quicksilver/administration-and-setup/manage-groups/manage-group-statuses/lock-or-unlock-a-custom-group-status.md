---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Statuts des groupes verrouillé et déverrouillé
description: Le verrouillage des statuts personnalisés d’un groupe permet de s’assurer que les membres du groupe et ses sous-groupes utilisent les mêmes processus dans leur workflow. Lorsqu’un statut de groupe est verrouillé, il est disponible pour tous les utilisateurs et utilisatrices du groupe et des groupes inférieurs.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 3463e4cb-7336-49b7-b81a-c2acef72f61d
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 91%

---

# Statuts de groupe verrouillés et déverrouillés

Le verrouillage des statuts personnalisés d’un groupe permet de s’assurer que les membres du groupe et ses sous-groupes utilisent les mêmes processus dans leur workflow. Lorsqu’un statut de groupe est verrouillé, il est disponible pour tous les utilisateurs et toutes les utilisatrices du groupe et dans les groupes inférieurs. Bien que vous (ou l’administration Workfront) puissiez modifier ou supprimer un statut que vous verrouillez, les administrateurs et les administratrices des sous-groupes ci-dessous ne peuvent pas le faire pour ces groupes ; seul l’ordre d’affichage dans la liste des statuts peut être modifié.

Inversement, le déverrouillage des statuts personnalisés d’un groupe offre plus de flexibilité aux administrateurs et aux administratrices des sous-groupes inférieurs pour gérer les workflows uniques utilisés dans leurs groupes. Lorsqu’un statut de groupe est déverrouillé, les administrateurs et les administratrices des sous-groupes inférieurs peuvent modifier ses attributs ou les supprimer pour ces sous-groupes.

>[!IMPORTANT]
>
>Si vous verrouillez un statut personnalisé après son déverrouillage pendant une période donnée, vos paramètres pour ce statut remplacent ceux définis par les administrateurs et les administratrices de groupe dans les sous-groupes inférieurs. Tant que le statut est verrouillé, ces administrateurs et ces administratrices ne peuvent pas modifier ni supprimer le statut de leurs groupes.

Pour plus d’informations sur le verrouillage ou le déverrouillage d’un statut de groupe, consultez la section [Créer ou modifier un statut de groupe](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

Vous pouvez utiliser les statuts verrouillés et déverrouillés dans un processus d’approbation de groupe. Si vous créez un processus d’approbation de groupe avec un statut de groupe déverrouillé, les utilisateurs et utilisatrices peuvent associer le processus d’approbation à n’importe quel projet, tâche ou problème associé au groupe.

