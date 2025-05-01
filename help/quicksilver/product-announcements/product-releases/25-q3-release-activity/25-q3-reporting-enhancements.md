---
title: Améliorations des rapports du troisième trimestre 2025
description: Améliorations apportées aux projets au troisième trimestre 2025
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: b36cfdc4587bc440867a6a84b9460eaeaf4daf88
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 25%

---

# Améliorations des rapports du troisième trimestre 2025

Cette page décrit toutes les améliorations apportées aux rapports avec la version du troisième trimestre 2025 dans l’environnement Aperçu. Ces améliorations seront rendues disponibles comme indiqué, dans l’environnement de production.

Pour obtenir la liste de toutes les modifications disponibles à ce stade du cycle de publication de la version du troisième trimestre 2025, consultez la [Vue d’ensemble de la version du troisième trimestre 2025](/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-release-overview.md).

## Les caractères génériques utilisateur ne renvoient plus de résultats avec une valeur nulle lors du filtrage

>[!NOTE]
>
>* Aperçu : 30 avril 2025
>* Version rapide de production : 15 mai 2025
>* Production pour tous les clients : 17 juillet 2025

Nous avons mis à jour le comportement du caractère générique utilisateur pour exclure la valeur nulle lors du filtrage d’un rapport. Cette modification permet au filtre de produire des résultats plus précis, plutôt que de renvoyer des résultats qui ne sont pas correctement configurés par un utilisateur (résultat nul).

Auparavant, lorsqu’un caractère générique utilisateur générait une valeur nulle, un rapport affichait tous les enregistrements qui avaient également une valeur nulle.

Cette modification s’applique aux filtres génériques suivants :

* `$$USER.homeTeamID`
* `$$USER.otherTeamIDs`
* `$$USER.roleID`
* `$$USER.roleIDs`
* `$$USER.companyID`

