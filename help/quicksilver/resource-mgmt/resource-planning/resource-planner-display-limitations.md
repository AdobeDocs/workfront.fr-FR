---
content-type: reference
product-area: resource-management
navigation-topic: resource-planning
title: Limites d’affichage du planificateur de ressources
description: Pour améliorer les performances, Adobe Workfront limite la quantité d’informations que vous pouvez afficher ainsi que la quantité d’informations que vous pouvez exporter à partir du planificateur de ressources.
author: Alina
feature: Resource Management
exl-id: 12f56f11-59fb-4318-b43a-5ac695ca1e7e
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '948'
ht-degree: 0%

---

# Limites d’affichage du planificateur de ressources

Pour améliorer les performances, Adobe Workfront limite la quantité d’informations que vous pouvez afficher ainsi que la quantité d’informations que vous pouvez exporter à partir du planificateur de ressources.

Lorsque vous approchez de cette limite, Workfront affiche un message d’avertissement vous informant que vous avez atteint cette limite.

Si les informations que vous prévoyez de voir dans le planificateur de ressources ne s’affichent pas, il est possible que vous souhaitiez afficher trop d’informations et que certaines données n’aient pas été affichées en raison de cette limitation.

Nous recommandons ce qui suit pour optimiser les performances lors de l’affichage et de l’exportation du planificateur de ressources :

* Utilisez des filtres pour réduire la quantité d’informations que vous affichez dans le planificateur de ressources et n’afficher que les informations qui vous concernent.
* Utilisez toutes vos options d’exportation pour réduire la quantité d’informations que vous exportez simultanément et pour vous assurer que vous n’exportez que des informations pertinentes.\
  Pour plus d’informations sur l’utilisation des filtres et les options d’exportation dans le planificateur de ressources, voir [Filtrer les informations dans le planificateur de ressources](../../resource-mgmt/resource-planning/filter-resource-planner.md).

  Pour plus d’informations sur l’exportation d’informations à partir du planificateur de ressources, voir [Exporter des informations à partir du planificateur de ressources](../../resource-mgmt/resource-planning/export-resource-planner.md).

La quantité d’informations que vous pouvez afficher ou exporter dépend de la vue appliquée et de l’environnement utilisé pour accéder au planificateur de ressources.

## Limites de la vue de projet

Tenez compte des points suivants lorsque vous appliquez la vue Projet au planificateur de ressources :

* Vous ne pouvez afficher que les projets que vous avez accès à la gestion.
* Vous pouvez développer chaque projet pour afficher les rôles qui lui sont associés, ainsi que chaque rôle pour afficher les utilisateurs qui lui sont associés.

  Vous pouvez afficher jusqu’à 300 projets lorsque vous faites défiler la liste jusqu’au bas de la liste, sauf s’il existe plus de 30 000 lignes de projets, de rôles et d’utilisateurs. Vous recevez ensuite un message d’avertissement vous informant que vous avez atteint la limite de 30 000 lignes.

* Vous pouvez afficher trois ou quatre périodes à la fois, selon la taille de votre écran.

Tenez compte de ce qui suit lors de l’exportation d’informations à partir de la vue Projet du planificateur de ressources, après avoir appliqué tous les filtres et options d’exportation appropriés :

* Lorsque vous choisissez d’exporter tous les éléments (projets, rôles et utilisateurs) du planificateur de ressources, tous les objets correspondant à vos critères s’affichent dans le fichier exporté, que vous ayez fait défiler la liste vers le bas pour les afficher ou non.
* Les lignes sans informations d’attribution sont incluses dans le fichier exporté.

* Vous pouvez exporter jusqu’à 30 000 lignes.

## Limites de la vue Rôle

Tenez compte des points suivants lorsque vous appliquez la vue Rôle au planificateur de ressources, après avoir appliqué tous les filtres appropriés :

* Vous ne pouvez afficher que les rôles associés aux projets que vous pouvez gérer.

* Vous pouvez voir jusqu’à 300 rôles lorsque vous faites défiler la liste vers le bas, sauf s’il existe plus de 30 000 lignes de rôles, de projets et d’utilisateurs. Vous recevez ensuite un message d’avertissement vous informant que vous avez atteint la limite de 30 000 lignes pour ce que vous pouvez afficher à l’écran.
* Vous pouvez développer chaque rôle pour afficher une liste de projets et chaque projet pour afficher une liste des utilisateurs pouvant remplir ces rôles sur les projets.

  20 projets s’affichent par défaut et vous pouvez utiliser l’option Charger plus pour afficher d’autres projets ou faire défiler l’écran sous chaque projet pour charger plus d’utilisateurs.

* Vous pouvez afficher trois ou quatre périodes, selon la taille de votre écran.

Tenez compte de ce qui suit lors de l’exportation d’informations à partir de la vue Rôle du planificateur de ressources, après avoir appliqué tous les filtres et options d’exportation appropriés :

* Lorsque vous choisissez d’exporter tous les éléments (rôles, projets et utilisateurs) du planificateur de ressources, tous les objets correspondant à vos critères apparaissent dans le fichier exporté, que vous ayez fait défiler la liste vers le bas ou non pour les afficher.
* Les lignes sans informations d’attribution sont incluses dans le fichier exporté.
* Vous pouvez exporter jusqu’à 30 000 lignes.

## Limites dans la vue utilisateur

Tenez compte des points suivants lorsque vous appliquez la vue Utilisateur au planificateur de ressources :

* Vous pouvez afficher tous les utilisateurs répondant aux critères suivants :

   * Vous avez accès à la vue
   * Sont actives
   * Vous êtes connecté au moins une fois.

* Vous pouvez développer chaque utilisateur pour afficher les projets qui lui sont associés, et chaque projet pour afficher les rôles qui lui sont associés.\
  Les 50 premiers projets et rôles s’affichent par défaut. Vous pouvez utiliser l’option Charger plus pour afficher d’autres projets ou rôles.

  >[!NOTE]
  >
  >Si vous avez filtré la liste des utilisateurs par projet, seuls les utilisateurs associés aux projets filtrés peuvent être développés, ainsi que des informations sur l’heure.

* Vous pouvez voir jusqu’à 2 000 utilisateurs dans l’interface web. Workfront affiche un message d’avertissement lorsque vous atteignez cette limite.
* Vous pouvez afficher trois ou quatre périodes, selon la taille de votre écran.

Tenez compte de ce qui suit lors de l’exportation d’informations à partir de la vue Utilisateur du planificateur de ressources, une fois que vous avez appliqué tous les filtres et options d’exportation appropriés :

* Lorsque vous choisissez d’exporter tous les rôles (utilisateurs, rôles et projets) du planificateur de ressources, tous les rôles, projets et utilisateurs sont inclus dans le fichier exporté, qu’ils soient développés ou non dans l’interface web.

* Vous pouvez exporter jusqu’à 30 000 lignes contenant des utilisateurs, ainsi que les projets et les rôles répertoriés en dessous, que vous ayez fait défiler la liste vers le bas pour les afficher ou non. Tous les utilisateurs, projets et rôles sont inclus dans le fichier exporté, qu’ils soient développés ou non dans l’interface web.
* Les lignes sans informations d’attribution sont incluses dans le fichier exporté.
