---
content-type: reference
product-area: resource-management
navigation-topic: resource-planning
title: Limites d’affichage du planificateur de ressources
description: Pour améliorer les performances, Adobe Workfront limite la quantité d’informations que vous pouvez afficher, ainsi que la quantité d’informations que vous pouvez exporter à partir du planificateur de ressources.
author: Lisa
feature: Resource Management
exl-id: 12f56f11-59fb-4318-b43a-5ac695ca1e7e
source-git-commit: 3c3175c347431b10aed1a6034df6c756056399b3
workflow-type: tm+mt
source-wordcount: '948'
ht-degree: 99%

---

# Limites d’affichage du planificateur de ressources

Pour améliorer les performances, Adobe Workfront limite la quantité d’informations que vous pouvez afficher, ainsi que la quantité d’informations que vous pouvez exporter à partir du planificateur de ressources.

Lorsque vous approchez de cette limite, Workfront affiche un message d’avertissement vous informant que vous avez atteint cette limite.

Si les informations que vous prévoyez d’afficher dans le planificateur de ressources ne s’affichent pas, vous essayez peut-être d’afficher trop d’informations et certaines données ne s’affichent peut-être pas en raison de cette limitation.

Nous recommandons les paramètres suivants pour optimiser les performances lors de l’affichage et de l’export du planificateur de ressources :

* Utilisez des filtres pour réduire la quantité d’informations que vous affichez dans le planificateur de ressources et n’afficher que les informations qui vous concernent.
* Utilisez toutes vos options d’export pour réduire la quantité d’informations que vous exportez simultanément et pour vous assurer que vous n’exportez que des informations pertinentes.\
  Pour plus d’informations sur l’utilisation des filtres et l’export d’options dans le planificateur de ressources, voir la section [Filtrer des informations dans le planificateur de ressources](../../resource-mgmt/resource-planning/filter-resource-planner.md).

  Pour plus d’informations sur l’export d’informations à partir du planificateur de ressources, voir la section [Exporter des informations à partir du planificateur de ressources](../../resource-mgmt/resource-planning/export-resource-planner.md).

La quantité d’informations que vous pouvez afficher ou exporter dépend de la vue appliquée et de l’environnement utilisé pour accéder au planificateur de ressources.

## Limites de la vue Projet

Tenez compte des points suivants lorsque vous appliquez la vue Projet au planificateur de ressources :

* Vous ne pouvez afficher que les projets pour lesquels vous disposez d’un accès en gestion.
* Vous pouvez développer chaque projet pour afficher les rôles qui lui sont associés, ainsi que chaque rôle pour afficher les utilisateurs et utilisatrices qui lui sont associés.

  Vous pouvez afficher jusqu’à 300 projets lorsque vous faites défiler la liste jusqu’en bas, sauf s’il existe plus de 30 000 lignes de projets, de rôles et d’utilisateurs et utilisatrices. Vous recevez alors un message d’avertissement vous informant que vous avez atteint la limite de 30 000 lignes.

* Vous pouvez afficher trois ou quatre périodes à la fois, selon la taille de votre écran.

Tenez compte des points suivants lors de l’export d’informations à partir de la vue Projet du planificateur de ressources, après avoir appliqué tous les filtres et options d’export appropriés :

* Lorsque vous choisissez d’exporter tous les éléments (projets, rôles et utilisateurs et utilisatrices) du planificateur de ressources, tous les objets correspondant à vos critères s’affichent dans le fichier exporté, que vous ayez fait défiler la liste vers le bas pour les afficher ou non.
* Les lignes sans informations d’affectation sont incluses dans le fichier exporté.

* Vous pouvez exporter jusqu’à 30 000 lignes.

## Limites de la vue Rôle

Tenez compte des points suivants lorsque vous appliquez la vue Rôle au planificateur de ressources, après avoir appliqué tous les filtres appropriés :

* Vous ne pouvez afficher que les rôles associés aux projets que vous pouvez gérer.

* Vous pouvez voir jusqu’à 300 rôles lorsque vous faites défiler la liste vers le bas, sauf s’il existe plus de 30 000 lignes de rôles, de projets et d’utilisateurs et utilisatrices. Vous recevez ensuite un message d’avertissement vous informant que vous avez atteint la limite de 30 000 lignes relative à ce que vous pouvez afficher à l’écran.
* Vous pouvez développer chaque rôle pour afficher une liste de projets et chaque projet pour afficher une liste des utilisateurs et utilisatrices pouvant remplir ces rôles sur les projets.

  20 projets s’affichent par défaut et vous pouvez utiliser l’option Charger plus pour afficher d’autres projets ou faire défiler l’écran sous chaque projet pour charger davantage d’utilisateurs et d’utilisatrices.

* Vous pouvez afficher trois ou quatre périodes, selon la taille de votre écran.

Tenez compte des points suivants lors de l’export d’informations à partir de la vue Rôle du planificateur de ressources, après avoir appliqué tous les filtres et options d’export appropriés :

* Lorsque vous choisissez d’exporter tous les éléments (rôles, projets et utilisateurs et utilisatrices) du planificateur de ressources, tous les objets correspondant à vos critères apparaissent dans le fichier exporté, que vous ayez fait défiler la liste vers le bas pour les afficher ou non.
* Les lignes sans informations d’affectation sont incluses dans le fichier exporté.
* Vous pouvez exporter jusqu’à 30 000 lignes.

## Limites dans la vue utilisateur

Tenez compte des points suivants lorsque vous appliquez la vue utilisateur au planificateur de ressources :

* Vous pouvez afficher l’ensemble des utilisateurs et utilisatrices répondant aux critères suivants :

   * Vous disposez d’un accès en affichage.
   * Ils sont actifs.
   * Ils ont réalisé au moins une connexion.

* Vous pouvez développer chaque utilisateur ou utilisatrice pour afficher les projets qui lui sont associés, et chaque projet pour afficher les rôles qui lui sont associés.\
  Les 50 premiers projets et rôles s’affichent par défaut. Vous pouvez utiliser l’option Charger plus pour afficher d’autres projets ou rôles.

  >[!NOTE]
  >
  >Si vous avez filtré la liste des utilisateurs et utilisatrices par projet, seuls ceux associés aux projets filtrés peuvent être développés et peuvent afficher des informations sur l’heure.

* Vous pouvez voir jusqu’à 2 000 utilisateurs et utilisatrices dans l’interface web. Workfront affiche un message d’avertissement lorsque vous atteignez cette limite.
* Vous pouvez afficher trois ou quatre périodes, selon la taille de votre écran.

Tenez compte des points suivants lors de l’export d’informations à partir de la vue utilisateur du planificateur de ressources, une fois que vous avez appliqué tous les filtres et options d’export appropriés :

* Lorsque vous choisissez d’exporter tous les éléments (utilisateurs et utilisatrices, rôles et projets) du planificateur de ressources, ils sont inclus dans le fichier exporté, qu’ils soient développés ou non dans l’interface web.

* Vous pouvez exporter jusqu’à 30 000 lignes contenant des utilisateurs et utilisatrices, ainsi que les projets et les rôles répertoriés en dessous, que vous ayez fait défiler la liste vers le bas pour les afficher ou non. L’ensemble des utilisateurs et utilisatrices, projets et rôles sont inclus dans le fichier exporté, qu’ils soient développés ou non dans l’interface web.
* Les lignes sans informations d’affectation sont incluses dans le fichier exporté.
