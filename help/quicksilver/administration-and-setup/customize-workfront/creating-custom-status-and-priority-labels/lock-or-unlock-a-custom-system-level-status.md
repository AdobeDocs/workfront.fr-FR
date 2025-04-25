---
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
title: Statuts système verrouillés et déverrouillés
description: Le verrouillage des statuts personnalisés permet de s’assurer que les personnes de votre entreprise utilisent les mêmes processus dans leur flux de travail. Lorsqu’un statut est verrouillé, il est disponible pour l’ensemble des utilisateurs et utilisatrices du système. Bien que vous puissiez le modifier ou le supprimer, les administrateurs et administratrices de groupes ne peuvent pas le faire pour leurs groupes. À l’inverse, le déverrouillage des statuts personnalisés permet aux administrateurs et administratrices de groupes de gérer avec plus de souplesse les workflows uniques utilisés dans leurs groupes. Les attributs d’un statut déverrouillé peuvent être modifiés ou supprimés pour leurs groupes.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 0e58a1d6-5e0c-4445-a5ac-400dfd4c4948
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 98%

---

# Statuts verrouillés et déverrouillés au niveau du système

Le verrouillage des statuts personnalisés permet de s’assurer que les personnes de votre entreprise utilisent les mêmes processus dans leur flux de travail. Lorsqu’un statut est verrouillé, il est disponible pour l’ensemble des utilisateurs et utilisatrices du système. Bien que vous puissiez modifier ou supprimer un statut que vous verrouillez, les administrateurs et administratrices de groupes ne peuvent pas le faire pour leurs groupes et ne peuvent modifier que son ordre d’affichage dans la liste Statut.

À l’inverse, le déverrouillage des statuts personnalisés permet aux administrateurs et administratrices de groupes de gérer avec plus de souplesse les workflows uniques utilisés dans leurs groupes. Lorsqu’un statut est déverrouillé, les administrateurs et administratrices de groupes peuvent modifier ses attributs ou les supprimer pour leurs groupes.

>[!IMPORTANT]
>
>Si vous verrouillez un statut personnalisé après qu’il a été déverrouillé pendant une certaine période, vos paramètres à l’échelle du système remplacent ceux définis par les administrateurs et administratrices de groupes. Pendant que le statut est verrouillé, les administrateurs et administratrices de groupes ne peuvent pas modifier ni supprimer le statut de leurs groupes.

Pour plus d’informations sur le verrouillage ou le déverrouillage d’un statut au niveau du système, consultez [Créer ou modifier un statut](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

## Statuts déverrouillés dans les processus d’approbation

Vous pouvez utiliser les statuts verrouillés et déverrouillés dans le cadre d’un processus d’approbation de système. Si vous créez un processus d’approbation de système avec un statut déverrouillé, les utilisateurs et utilisatrices dans tout le système peuvent associer le processus d’approbation à n’importe quel objet (projet, tâche ou problème) du système.

Les messages d’avertissement s’affichent dans les scénarios suivants pour vous aider, ainsi que vos utilisateurs et utilisatrices, à vous assurer que vous comprenez les résultats de ces scénarios :

* Un administrateur ou une administratrice déverrouille un statut au niveau du système utilisé dans un processus d’approbation. Un message l’avertit que le statut de déverrouillage de ses groupes est susceptible d’être supprimé, ce qui empêcherait les personnes membres de ces groupes d’utiliser correctement ce processus d’approbation pour les objets qui leur sont affectés.

* Une personne commence à modifier un processus d’approbation qui utilise le statut déverrouillé. Un message l’avertit du statut déverrouillé afin qu’elle puisse déterminer s’il est préférable de le reverrouiller ou de le remplacer.

* Un processus d’approbation au niveau du système avec un statut déverrouillé est associé à un objet et le statut a été supprimé pour le groupe affecté à l’objet. Lorsqu’une personne membre du groupe accède à la section Approbations de l’objet, un message explique que le processus d’approbation ne peut pas être lancé pour l’objet.

Vous pouvez utiliser les statuts verrouillés et déverrouillés dans un processus d’approbation de groupe. Si vous créez un processus d’approbation de groupe avec un statut de groupe déverrouillé, les utilisateurs et utilisatrices peuvent associer le processus d’approbation à n’importe quel projet, tâche ou problème associé au groupe.
