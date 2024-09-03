---
content-type: release-notes
navigation-topic: 2020-3-release-activity
title: 20.3 Améliorations de la gestion des ressources
description: Cette page décrit toutes les améliorations apportées à la gestion des ressources avec la version 20.3 de l’environnement de production. Ces améliorations ont été mises à disposition dans l’environnement de production au cours de la semaine du 10 août 2020.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: a2c34117-e03c-4394-9b81-7c18433531d1
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '837'
ht-degree: 100%

---

# 20.3 Améliorations de la gestion des ressources

Cette page décrit toutes les améliorations apportées à la gestion des ressources avec la version 20.3 de l’environnement de production. Ces améliorations ont été mises à disposition dans l’environnement de production au cours de la semaine du 10 août 2020.

Pour une liste de tous les changements disponibles avec la version 20.3, voir [Vue d’ensemble de la version 20.3](../../../product-announcements/product-releases/20.3-release-activity/20-3-release-overview.md).

## Inclure les heures provenant des problèmes de la zone de travail affecté de l’équilibreur de charge de travail

Pour vous permettre d’avoir une vue d’ensemble complète des charges de travail de vos employées et employés, nous avons introduit un paramètre qui vous permet d’inclure des heures à partir des problèmes de la zone de travail affecté de l’équilibreur de charge de travail.

Pour plus d’informations sur l’utilisation de l’équilibreur de charge de travail, voir la section [Naviguer dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Ajuster les affectations pour les jours non ouvrés dans l’équilibreur de charge de travail

Vous pouvez ajuster les affectations de vos ressources pour les jours non ouvrés à l’aide de l’équilibreur de charge de travail.

Pour plus d’informations sur la gestion des affectations dans l’équilibreur de charge de travail, voir la section [Gérer des affectations d’utilisateur ou d’utilisatrice dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## Filtres variables disponibles dans l’équilibreur de charge de travail

Afin d’améliorer votre expérience et de vous offrir plus de flexibilité lors du partage d’informations, nous avons maintenant mis en œuvre des filtres variables pour l’équilibreur de charge de travail. Les filtres suivants ont été ajoutés à l’équilibreur de charge de travail :

* « Moi » (lors du filtrage par les utilisateurs et utilisatrices)
* « Mon rôle principal » (lors du filtrage par rôles)
* « Mon équipe interne » ou « Toutes mes équipes » (lors du filtrage par équipes)

Ces filtres remplacent les variables de filtre génériques $$USER.ID, $$USER.roleID, $$USER.homeTeamID et $$USER.TeamID.

Lorsque vous appliquez l’un de ces filtres, puis partagez l’équilibreur de charge de travail ou que vous le placez sur un tableau de bord, tous les autres utilisateurs et utilisatrices verront leurs propres informations.

Pour plus d’informations sur l’application de filtres à l’équilibreur de charge de travail, voir la section [Filtrer des informations dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

## Nouveau tri des projets dans l’équilibreur de charge de travail

L’équilibreur de charge de travail trie désormais les projets en fonction de la première date de début prévue, puis de la dernière date d’achèvement prévue des tâches du projet qui se produisent au cours du délai que l’utilisateur ou l’utilisatrice affiche à l’écran. Cela permet d’organiser le travail dans une hiérarchie de type arborescence qui permet d’identifier plus facilement le travail pour une journée.

Pour plus d’informations sur l’affichage des projets et des éléments de travail dans l’équilibreur de charge de travail, voir la section [Naviguer dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Afficher la progression réelle du travail dans l’équilibreur de charge de travail

Pour vous donner une perspective précise de la progression de votre charge de travail, nous avons ajouté un nouveau paramètre à l’équilibreur de charge de travail qui affiche la chronologie des tâches et des problèmes en fonction de leurs dates prévisionnelles. Vous pouvez activer le paramètre Afficher les dates prévisionnelles pour afficher la chronologie prévisionnelle de l’élément de travail en plus de la chronologie prévue.

En outre, avec cette amélioration, si une tâche ou un problème se termine avant la date d’achèvement prévue, les heures affectées pour les jours restants sont barrées pour indiquer qu’elles ne sont pas prises en compte dans l’affectation globale de l’utilisateur ou l’utilisatrice.

Pour plus d’informations sur la navigation dans l’équilibreur de charge de travail et l’activation des paramètres, voir la section [Naviguer dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Fonctionnalités de l’équilibreur de charge de travail précédemment annoncées dans la version 20.2

* [Ajuster les affectations quotidiennes et hebdomadaires dans l’équilibreur de charge de travail](#adjust-daily-and-weekly-allocation-in-the-workload-balancer)
* [Mettre à jour les heures prévues de la tâche dans l’équilibreur de charge de travail](#update-task-planned-hours-in-the-workload-balancer)
* [Méthode plus pratique pour mettre à jour les affectations dans l’équilibreur de charge de travail](#a-more-convenient-way-to-update-allocations-in-the-workload-balancer)

### Ajuster les affectations quotidiennes et hebdomadaires dans l’équilibreur de charge de travail {#adjust-daily-and-weekly-allocation-in-the-workload-balancer}

Pour éviter l’épuisement de vos ressources, vous pouvez maintenant ajuster l’affectation quotidienne et hebdomadaire de vos utilisateurs et utilisatrices à l’aide de l’équilibreur de charge de travail.

Avant cette amélioration, cela n’était possible qu’à l’aide des outils de planification des ressources.

Pour plus d’informations sur la gestion des affectations dans l’équilibreur de charge de travail, voir la section [Gérer les affectations des utilisateurs et utilisatrices dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

**Disponible dans ces environnements :**

* Adobe Workfront Classic
* La nouvelle expérience Adobe Workfront

### Mettre à jour le nombre d’heures prévues dans l’équilibreur de charge de travail {#update-task-planned-hours-in-the-workload-balancer}

>[!NOTE]
>
>Cette amélioration sera disponible dans l’environnement de production peu de temps après la version 2020.2.

Une nouvelle option de la zone Gestion des ressources du niveau d’accès permet désormais aux personnes disposant de cet accès de modifier le nombre d’heures prévues à partir de l’équilibreur de charge de travail. Lorsque vous ajustez les affectations dans l’équilibreur de charge de travail, le total des affectations quotidiennes n’a pas besoin de correspondre au nombre d’heures prévues des tâches. Une fois les affectations enregistrées, le total des heures d’affectation devient le nombre d’heures prévues de la tâche. Cela n’est possible que pour les tâches ayant un type de durée simple.

Pour plus d’informations sur la gestion des affectations dans l’équilibreur de charge de travail, voir la section [Gérer les affectations des utilisateurs et utilisatrices dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

Pour plus d’informations sur l’octroi de l’accès à la gestion des ressources, voir la section [Accorder l’accès à la gestion des ressources](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md).

### Méthode plus pratique pour mettre à jour les affectations dans l’équilibreur de charge de travail {#a-more-convenient-way-to-update-allocations-in-the-workload-balancer}

Pour faciliter la gestion des affectations d’un utilisateur ou d’une utilisatrice à un élément de travail dans l’équilibreur de charge de travail, vous pouvez maintenant double-cliquer sur l’élément de travail. Vous pouvez également continuer à utiliser l’option de menu Modifier les allocations existante. En outre, vous n’avez plus besoin d’activer l’affichage des affectations pour pouvoir les mettre à jour.

Pour plus d’informations sur la gestion des affectations dans l’équilibreur de charge de travail, voir la section [Gérer les affectations des utilisateurs et utilisatrices dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).
