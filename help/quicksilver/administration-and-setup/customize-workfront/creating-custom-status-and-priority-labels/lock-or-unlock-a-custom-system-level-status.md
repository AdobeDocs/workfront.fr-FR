---
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
title: États au niveau du système verrouillés et déverrouillés
description: Le verrouillage des états personnalisés permet de s’assurer que les personnes de votre entreprise utilisent les mêmes processus dans leur flux de travail. Lorsqu’un état est verrouillé, il est disponible pour tous les utilisateurs du système. Bien que vous puissiez le modifier ou le supprimer, les administrateurs de groupe ne peuvent pas le faire pour leurs groupes. Inversement, le déverrouillage des états personnalisés offre aux administrateurs de groupe plus de flexibilité pour gérer les workflows uniques utilisés dans leurs groupes. Ils peuvent modifier les attributs d’un état déverrouillé ou le supprimer pour leurs groupes.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 0e58a1d6-5e0c-4445-a5ac-400dfd4c4948
source-git-commit: c70a10a920d32ad00a2e833b331c92a598902d21
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 0%

---

# États au niveau du système verrouillés et déverrouillés

Le verrouillage des états personnalisés permet de s’assurer que les personnes de votre entreprise utilisent les mêmes processus dans leur flux de travail. Lorsqu’un état est verrouillé, il est disponible pour tous les utilisateurs du système. Bien que vous puissiez modifier ou supprimer un état que vous verrouillez, les administrateurs de groupe ne peuvent pas le faire pour leurs groupes ; ils ne peuvent modifier que l’ordre d’affichage dans la liste État .

Inversement, le déverrouillage des états personnalisés offre aux administrateurs de groupe plus de flexibilité pour gérer les workflows uniques utilisés dans leurs groupes. Lorsqu’un état est déverrouillé, les administrateurs de groupe peuvent modifier ses attributs ou les supprimer pour leurs groupes.

>[!IMPORTANT]
>
>Si vous verrouillez un état personnalisé après son déverrouillage pendant une période donnée, vos paramètres à l’échelle du système remplacent ceux définis par les administrateurs de groupe. Bien que l’état soit verrouillé, les administrateurs de groupe ne peuvent pas modifier ni supprimer l’état de leurs groupes.

Pour plus d’informations sur le verrouillage ou le déverrouillage d’un état de niveau système, voir [Création ou modification d’un état](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

## Statuts déverrouillés dans les processus de validation

Vous pouvez utiliser les états verrouillés et déverrouillés dans un processus d’approbation du système. Si vous créez un processus d’approbation du système avec l’état déverrouillé, les utilisateurs de tout le système peuvent associer le processus d’approbation à n’importe quel projet, tâche ou problème du système.

Les messages d’avertissement s’affichent dans les scénarios suivants pour vous aider, ainsi que vos utilisateurs, à vous assurer que vous comprenez les résultats des scénarios suivants :

* Un administrateur déverrouille un état au niveau du système utilisé dans un processus d’approbation. Un message avertit que l’état de déverrouillage de leurs groupes est susceptible d’être supprimé, ce qui empêcherait les membres de ces groupes d’utiliser correctement ce processus d’approbation pour les objets qui leur sont assignés.

* Un utilisateur commence à modifier un processus d’approbation qui utilise l’état déverrouillé. Un message avertit l’utilisateur de l’état déverrouillé afin qu’il puisse déterminer s’il est préférable de le reverrouiller ou de le remplacer.

* Un processus d’approbation au niveau du système avec un état déverrouillé est associé à un objet et l’état a été supprimé pour le groupe affecté à l’objet. Lorsqu’un membre du groupe accède à la section Validations de l’objet, un message explique que le processus d’approbation ne peut pas être lancé pour l’objet.

Vous pouvez utiliser les états verrouillés et déverrouillés dans un processus d’approbation de groupe. Si vous créez un processus d’approbation de groupe avec le statut de groupe déverrouillé, les utilisateurs peuvent associer le processus d’approbation à n’importe quel projet, tâche ou problème associé au groupe.