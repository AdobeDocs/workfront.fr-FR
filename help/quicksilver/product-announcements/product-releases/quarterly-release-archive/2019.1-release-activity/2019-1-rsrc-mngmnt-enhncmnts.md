---
content-type: release-notes
navigation-topic: 2019-1-release-activity
title: Améliorations de la gestion des ressources (version 2019.1)
description: Cette page décrit toutes les améliorations apportées à la gestion des ressources incluses dans la version 2019.1. Cette fonctionnalité est désormais disponible dans l’environnement de production.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 6eed6023-96cc-45d7-8dae-a36d45e92068
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '953'
ht-degree: 100%

---

# Améliorations de la gestion des ressources (version 2019.1)

Cette page décrit toutes les améliorations apportées à la gestion des ressources incluses dans la version 2019.1. Cette fonctionnalité est désormais disponible dans l’environnement de production.

Pour obtenir la liste de toutes les modifications apportées à la version 2019.1, consultez la section [Vue d’ensemble de l’activité de la version 2019.1](../../../../product-announcements/product-releases/quarterly-release-archive/2019.1-release-activity/2019-1-release-activity-overview.md).

## Mise à jour du filtre par défaut dans le planificateur de ressources

Le filtre par défaut dans le planificateur de ressources ne filtre plus par le groupe du projet.

Lors de l’affichage du planificateur de ressources, seuls les projets actuellement en cours et sensibles aux dates sont désormais affichés par défaut. Les informations des projets suivants sont incluses par défaut :

* Dont la date d’achèvement prévue est postérieure au premier jour du mois actuel.
* Dont la date de début prévue est antérieure à la dernière date du quatrième mois à compter d’aujourd’hui.
* Dont le statut est en cours ou planifié.

Auparavant, le filtre par défaut récupérait les informations des projets supplémentaires suivants :

* Dont la date d’achèvement prévue est postérieure au premier jour du mois actuel.
* Dont la date de début prévue est antérieure à la dernière date du quatrième mois à compter d’aujourd’hui.
* Dont le statut est en cours ou planifié.
* Dont le groupe correspond au groupe d’appartenance de l’utilisateur et de l’utilisatrice qui ont établi une connexion.

Pour plus d’informations sur l’application de filtres au planificateur de ressources, consultez la section [Filtrer les informations dans le planificateur de ressources](../../../../resource-mgmt/resource-planning/filter-resource-planner.md).

## Utilisation de caractères génériques pour les filtres du planificateur de ressources

Vous pouvez désormais utiliser des caractères génériques lors de la création de filtres dans le planificateur de ressources. Par exemple, vous pouvez utiliser $$USER.ID pour filtrer les informations sur la personne connectée ou $$USER.companyID pour filtrer les informations sur l’ensemble des utilisateurs et des utilisatrices appartenant à la même société que la personne connectée. Pour obtenir la liste complète des variables basées sur l’utilisateur ou l’utilisatrice, reportez-vous à la section [Variables de filtre de caractères génériques basées sur l’utilisateur ou l’utilisatrice](../../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md#user-based-variables) dans [Variables de filtre de caractères génériques](../../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

Auparavant, les caractères génériques n’étaient pas disponibles pour les filtres du planificateur de ressources.

Pour plus d’informations sur le filtrage dans le planificateur de ressources, voir [Filtrer des informations dans le planificateur de ressources](../../../../resource-mgmt/resource-planning/filter-resource-planner.md).

<!--
<iframe class="mt-media" src="assets/290697527?title=0&byline=0&portrait=0" width="640px" height="360px" frameborder="0" allowfullscreen></iframe>
-->

## Prise en charge des variables de filtrage des caractères génériques basées sur des dates dans le planificateur de ressources

Vous pouvez désormais utiliser n’importe quelle version de la variable de filtre de caractères génériques $$TODAY lorsque vous créez un filtre dans le planificateur de ressources.

Avant cette amélioration, vous ne pouviez utiliser que des variables de filtrage de caractères génériques basées sur l’utilisateur ou l’utilisatrice.

Pour plus d’informations sur le filtrage dans le planificateur de ressources, consultez la section [Filtrer les informations dans le planificateur de ressources](../../../../resource-mgmt/resource-planning/filter-resource-planner.md).

Pour plus d’informations sur les variables de filtrage des caractères génériques, consultez la section [Variables de filtrage des caractères génériques](../../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

## Options d’export pour afficher les rôles dans le planificateur de ressources

Vous pouvez maintenant sélectionner les niveaux d’informations à exporter à partir du planificateur de ressources lorsque vous affichez des rôles. Vous pouvez exporter l’une des options suivantes :

* Rôles uniquement
* Rôles et projets
* Rôles, projets et utilisateur ou utilisatrice

Avant cette amélioration, tous les niveaux d’informations étaient exportés dans l’affichage du rôle. Ces options ont été introduites dans les vues « Projet » et « Utilisateur ou Utilisatrice » dans une version précédente.

Pour plus d’informations sur l’export d’informations à partir du planificateur de ressources, consultez la section [Exporter des informations à partir du planificateur de ressources](../../../../resource-mgmt/resource-planning/export-resource-planner.md).

## Options de formatage des données pour l’export à partir du planificateur de ressources

Vous pouvez maintenant sélectionner le mode d’affichage des informations dans le fichier Excel lors de l’export à partir du planificateur de ressources.

Vous pouvez afficher la disponibilité et l’affectation des informations exportées à partir du planificateur de ressources de la manière suivante :

* non groupées par le nom des objets auxquels elles appartiennent. Dans ce cas, les noms des objets auxquels elles appartiennent s’affichent sur chaque ligne de données. (Il s’agit de l’option par défaut.)
* regroupées par le nom des objets auxquelles elles appartiennent. Dans ce cas, les informations contenues dans le fichier exporté apparaissent telles qu’elles sont affichées dans Workfront.

Avant cette amélioration, les informations du fichier exporté s’affichaient telles qu’elles apparaissaient dans Workfront.

Pour plus d’informations sur l’export d’informations à partir du planificateur de ressources, voir [Exporter des informations à partir du planificateur de ressources](../../../../resource-mgmt/resource-planning/export-resource-planner.md).

## Chronologie de planification persistante

>[!NOTE]
>
>Les outils de planification des ressources ont été retirés de Workfront avec la version 23.1. Pour plus d’informations sur la planification des ressources à l’aide de l’équilibreur de charge de travail, voir [Vue d’ensemble de l’équilibreur de charge de travail](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

La planification des chronologies conserve désormais la période sélectionnée lorsque vous actualisez la chronologie ou lorsque vous quittez la page.

Avant cette amélioration, la planification des chronologies renvoyait à la période par défaut lorsque vous actualisiez ou quittiez la page.

Les zones suivantes sont concernées par cette amélioration :

* Onglet Planification dans la zone Personnes
* Onglet Équipe en train de travailler sur
* Sous-onglet Planification de l’onglet Personnel d’un projet

Pour plus d’informations sur l’utilisation de la chronologie dans les zones Planification des ressources, voir « Commencer avec la planification des ressources ».

## Nouvelles options d’export dans le planificateur de ressources

Vous pouvez maintenant sélectionner les niveaux d’informations à exporter à partir du planificateur de ressources. Dans la vue Projet, vous pouvez exporter les éléments suivants :

* Projets uniquement
* Projets et rôles
* Projets, rôles et utilisateurs et utilisatrices

Dans la vue utilisateur, vous pouvez exporter les éléments suivants :

* Utilisateurs et utilisatrices uniquement
* Utilisateurs et projets
* Utilisateurs et utilisatrices, projets, rôles, tâches et problèmes

Avant cette amélioration, tous les niveaux d’informations étaient exportés par défaut dans toutes les vues du planificateur de ressources.

Pour plus d’informations sur l’export d’informations à partir du planificateur de ressources, voir [Exporter des informations à partir du planificateur de ressources](../../../../resource-mgmt/resource-planning/export-resource-planner.md).

## Mise à jour de la vue utilisateur dans le planificateur de ressources

Tous les utilisateurs et utilisatrices du système s’affichent désormais dans la vue utilisateur du planificateur de ressources, mais seules les personnes associées aux projets filtrés affichent également les informations sur l’heure.

Avant cette mise à jour, seules les personnes affectées aux éléments de travail sur les projets pour lesquels vous filtrez les ressources s’affichaient dans la vue utilisateur du planificateur de ressources.

Vous pouvez utiliser des filtres basés sur les utilisateurs et utilisatrices pour réduire le nombre d’utilisateurs et d’utilisatrices affichés dans la vue utilisateur à ceux qui sont affectés aux projets que vous souhaitez afficher.

Pour plus d’informations sur les filtres dans le planificateur de ressources, voir [Filtrer des informations dans le planificateur de ressources](../../../../resource-mgmt/resource-planning/filter-resource-planner.md).
