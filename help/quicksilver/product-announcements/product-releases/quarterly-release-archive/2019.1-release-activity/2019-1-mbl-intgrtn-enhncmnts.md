---
content-type: release-notes
navigation-topic: 2019-1-release-activity
title: Améliorations apportées à l’application mobile et à l’intégration (version 2019.1)
description: Cette page décrit toutes les améliorations de la gestion des ressources incluses dans la version 2019.1. Cette fonctionnalité est désormais disponible dans l’environnement de production.
author: Luke
feature: Product Announcements, Workfront Integrations and Apps
recommendations: noDisplay, noCatalog
exl-id: 6b86ba0d-977a-4c89-8832-e81bf28d9dad
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '961'
ht-degree: 1%

---

# Améliorations apportées à l’application mobile et à l’intégration (version 2019.1)

Cette page décrit toutes les améliorations de la gestion des ressources incluses dans la version 2019.1. Cette fonctionnalité est désormais disponible dans l’environnement de production.

Pour obtenir la liste de toutes les modifications apportées à la version 2019.1, consultez la [présentation de l’activité de version 2019.1](../../../../product-announcements/product-releases/quarterly-release-archive/2019.1-release-activity/2019-1-release-activity-overview.md).

## Mise à jour du filtre par défaut dans le planificateur de ressources

Le filtre par défaut dans le planificateur de ressources n’est plus filtré par le groupe du projet.

Lors de l’affichage du planificateur de ressources, seuls les projets actuellement en cours et sensibles aux dates sont désormais affichés par défaut. Les informations des projets suivants sont incluses par défaut :

* avec une date d’achèvement planifiée qui survient après la première date du mois d’aujourd’hui.
* avec une date de début planifiée qui se produit avant la dernière date du quatrième mois à partir d’aujourd’hui.
* avec un état actuel ou planifié.

Auparavant, le filtre par défaut récupérait les informations des projets supplémentaires suivants :

* avec une date d’achèvement planifiée qui survient après la première date du mois d’aujourd’hui.
* avec une date de début planifiée qui se produit avant la dernière date du quatrième mois à partir d’aujourd’hui.
* avec un état actuel ou planifié.
* Avec un groupe correspondant au groupe d’accueil de l’utilisateur connecté.

Pour plus d’informations sur l’application de filtres au planificateur de ressources, voir [Filtrage des informations dans le planificateur de ressources](../../../../resource-mgmt/resource-planning/filter-resource-planner.md).

## Utilisation de caractères génériques pour les filtres du planificateur de ressources

Vous pouvez désormais utiliser des caractères génériques lors de la création de filtres dans le planificateur de ressources. Par exemple, vous pouvez utiliser $$USER.ID pour filtrer les informations sur l’utilisateur connecté ou $$USER.companyID pour filtrer les informations sur tous les utilisateurs appartenant à la même société que l’utilisateur connecté. Pour obtenir une liste complète des variables basées sur l’utilisateur, reportez-vous à la section [ Variables de filtre de caractères génériques basées sur l’utilisateur](../../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md#user-based-variables) dans [ ](../../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

Auparavant, les caractères génériques n’étaient pas disponibles pour les filtres du planificateur de ressources.

Pour plus d’informations sur le filtrage dans le planificateur de ressources, voir [Filtrage des informations dans le planificateur de ressources](../../../../resource-mgmt/resource-planning/filter-resource-planner.md)

VIDÉO

## Prise en charge des variables de filtre par caractères génériques basées sur des dates dans le planificateur de ressources

Vous pouvez désormais utiliser n’importe quelle version de la variable de filtre de caractères génériques $$TODAY lorsque vous créez un filtre dans le planificateur de ressources.

Avant cette amélioration, vous ne pouviez utiliser que des variables de filtre génériques basées sur l’utilisateur.

Pour plus d’informations sur le filtrage dans le planificateur de ressources, voir [Filtrage des informations dans le planificateur de ressources](../../../../resource-mgmt/resource-planning/filter-resource-planner.md).

Pour plus d’informations sur les variables de filtre générique, voir [Variables de filtre générique](../../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

VIDÉO

## Options d’exportation pour la vue Rôle dans le planificateur de ressources

Vous pouvez maintenant sélectionner les niveaux d’informations à exporter à partir du planificateur de ressources dans la vue Rôle.

Vous pouvez exporter les éléments suivants :

* Rôles uniquement
* Rôles et projets
* Rôles, projets et utilisateurs

Avant cette amélioration, tous les niveaux d’informations étaient exportés dans la vue Rôle. Ces options ont été introduites dans les vues Projet et Utilisateur dans une version précédente.

Pour plus d’informations sur l’exportation d’informations à partir du planificateur de ressources, voir [Exporter des informations à partir du planificateur de ressources](../../../../resource-mgmt/resource-planning/export-resource-planner.md).

VIDÉO

## Options de formatage des données pour l’exportation du planificateur de ressource

Vous pouvez maintenant sélectionner le mode d’affichage des informations dans le fichier Excel lors de l’exportation à partir du planificateur de ressources.

Vous pouvez afficher la disponibilité et l’affectation des informations exportées à partir du planificateur de ressources de la manière suivante :

* Dégroupé par le nom des objets auxquels il appartient. Dans ce cas, les noms des objets auxquels il appartient s’affichent sur chaque ligne de données. (cette option est par défaut)
* Regroupé par le nom des objets auxquels il appartient. Dans ce cas, les informations contenues dans le fichier exporté apparaissent telles qu’elles sont affichées dans Workfront.

Avant cette amélioration, les informations du fichier exporté s’affichaient telles qu’elles s’affichaient dans Workfront.

Pour plus d’informations sur l’exportation d’informations à partir du planificateur de ressources, voir [Exporter des informations à partir du planificateur de ressources](../../../../resource-mgmt/resource-planning/export-resource-planner.md).

VIDÉO

## Chronologie de planification persistante

>[!NOTE]
>
>Les outils de planification des ressources ont été abandonnés et supprimés de Workfront avec la version 23.1. Pour plus d’informations sur la planification des ressources à l’aide de l’équilibreur de charge de travail, voir [Présentation de l’équilibreur de charge de travail](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

La planification des chronologies conserve désormais la période sélectionnée lorsque vous actualisez la chronologie ou quittez la page.

Avant cette amélioration, les chronologies de planification renvoyaient à la période par défaut lorsque vous actualisiez ou quittiez la page.

Cette amélioration est disponible dans les domaines suivants :

* Onglet Planification dans la zone Personnes
* Onglet Travail d’équipe
* Sous-onglet Planification de l’onglet Personnel d’un projet

Pour plus d’informations sur l’utilisation de la chronologie dans les zones Planification des ressources, voir &quot;Prise en main de la planification des ressources&quot;.

VIDÉO

## Nouvelles options d’exportation dans le planificateur de ressources

Vous pouvez maintenant sélectionner les niveaux d’informations à exporter à partir du planificateur de ressources.

Dans la vue Projet, vous pouvez exporter les éléments suivants :

* Projets uniquement
* Projets et rôles
* Projets, rôles et utilisateurs

Dans la vue Utilisateur, vous pouvez exporter les éléments suivants :

* Utilisateurs uniquement
* Utilisateurs et projets
* Utilisateurs, projets, rôles, tâches et problèmes

Avant cette amélioration, tous les niveaux d’informations étaient exportés par défaut dans toutes les vues du planificateur de ressources.

Pour plus d’informations sur l’exportation d’informations à partir du planificateur de ressources, voir [Exporter des informations à partir du planificateur de ressources](../../../../resource-mgmt/resource-planning/export-resource-planner.md).

VIDÉO

## Mise à jour de la vue utilisateur dans le planificateur de ressources

Tous les utilisateurs du système s’affichent désormais dans la vue Utilisateur du planificateur de ressources, mais seuls les utilisateurs associés aux projets filtrés affichent également les informations sur l’heure.

Avant cette mise à jour, seuls les utilisateurs affectés aux tâches sur les projets pour lesquels vous filtrez les ressources s’affichaient dans la vue Utilisateur du planificateur de ressources.

Vous pouvez utiliser des filtres basés sur les utilisateurs pour réduire le nombre d’utilisateurs affichés dans la vue Utilisateur à ceux qui sont affectés aux projets que vous souhaitez afficher.

Pour plus d’informations sur les filtres dans le planificateur de ressources, voir [Filtrage des informations dans le planificateur de ressources](../../../../resource-mgmt/resource-planning/filter-resource-planner.md).
