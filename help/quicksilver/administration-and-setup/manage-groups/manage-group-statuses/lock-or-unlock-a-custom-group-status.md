---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Statuts de groupe verrouillés et déverrouillés
description: Le verrouillage des statuts personnalisés d’un groupe permet de s’assurer que les membres du groupe et ses sous-groupes utilisent les mêmes processus dans leur flux de travail. Lorsqu’un état de groupe est verrouillé, il est disponible pour tous les utilisateurs du groupe et dans les groupes inférieurs. Bien que vous (ou un administrateur Workfront) puissiez modifier ou supprimer un état que vous verrouillez, les administrateurs des sous-groupes ci-dessous ne peuvent pas le faire pour ces groupes. À l’inverse, le déverrouillage des états personnalisés d’un groupe offre plus de flexibilité aux administrateurs des sous-groupes inférieurs pour gérer leurs workflows. Ils peuvent modifier les attributs d’un état déverrouillé ou le supprimer pour leurs groupes.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 3463e4cb-7336-49b7-b81a-c2acef72f61d
source-git-commit: d67de32fcbe4706cf8a1fc6f5bb8ec9d08b07119
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 0%

---

# Statuts de groupe verrouillés et déverrouillés

Le verrouillage des statuts personnalisés d’un groupe permet de s’assurer que les membres du groupe et ses sous-groupes utilisent les mêmes processus dans leur flux de travail. Lorsqu’un état de groupe est verrouillé, il est disponible pour tous les utilisateurs du groupe et dans les groupes inférieurs. Bien que vous (ou un administrateur Workfront) puissiez modifier ou supprimer un état que vous verrouillez, les administrateurs des sous-groupes ci-dessous ne peuvent pas le faire pour ces groupes ; ils ne peuvent modifier que l’ordre d’affichage dans la liste État .

Inversement, le déverrouillage des états personnalisés d’un groupe offre plus de flexibilité aux administrateurs des sous-groupes inférieurs pour gérer les workflows uniques utilisés dans leurs groupes. Lorsqu’un état de groupe est déverrouillé, les administrateurs de sous-groupes inférieurs peuvent modifier ses attributs ou les supprimer pour ces sous-groupes.

>[!IMPORTANT]
>
>Si vous verrouillez un état personnalisé après son déverrouillage pendant une période donnée, vos paramètres pour l’état remplacent ceux définis par les administrateurs de groupe dans les sous-groupes inférieurs. Tant que l’état est verrouillé, ces administrateurs ne peuvent pas modifier ni supprimer l’état de leurs groupes.

Pour plus d’informations sur le verrouillage ou le déverrouillage d’un état de groupe, voir [Création ou modification d’un état de groupe](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

Vous pouvez utiliser les états verrouillés et déverrouillés dans un processus d’approbation de groupe. Si vous créez un processus d’approbation de groupe avec le statut de groupe déverrouillé, les utilisateurs peuvent associer le processus d’approbation à n’importe quel projet, tâche ou problème associé au groupe.

