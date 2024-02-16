---
content-type: release-notes
navigation-topic: 2020-3-release-activity
title: 20.3 Améliorations de la gestion des ressources
description: Cette page décrit toutes les améliorations apportées à la gestion des ressources avec la version 20.3 de l’environnement de production. Ces améliorations ont été apportées à l’environnement de production au cours de la semaine du 10 août 2020.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: a2c34117-e03c-4394-9b81-7c18433531d1
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '837'
ht-degree: 0%

---

# 20.3 Améliorations de la gestion des ressources

Cette page décrit toutes les améliorations apportées à la gestion des ressources avec la version 20.3 de l’environnement de production. Ces améliorations ont été apportées à l’environnement de production au cours de la semaine du 10 août 2020.

Pour obtenir la liste de toutes les modifications disponibles avec la version 20.3, voir [Présentation de la version 20.3](../../../product-announcements/product-releases/20.3-release-activity/20-3-release-overview.md).

## Inclure les heures provenant des problèmes de la zone de travail affectée de l’équilibreur de charge de travail

Pour vous permettre d’avoir une vue d’ensemble complète des charges de travail de vos employés, nous avons introduit un paramètre qui vous permet d’inclure des heures à partir des problèmes de la zone de travail affectée de l’équilibreur de charge de travail.

Pour plus d’informations sur l’utilisation de l’équilibreur de charge de travail, voir [Navigation dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Ajuster les allocations pour les jours non ouvrés dans l’équilibreur de charge de travail

Vous pouvez ajuster les affectations de vos ressources pour les jours non ouvrés à l’aide de l’équilibreur de charge de travail.

Pour plus d’informations sur la gestion des affectations dans l’équilibreur de charge de travail, voir [Gestion des affectations utilisateur dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## Filtres variables disponibles dans l’équilibreur de charge de travail

Afin d’améliorer votre expérience et de vous offrir plus de flexibilité lors du partage d’informations, nous avons maintenant mis en oeuvre des filtres variables pour l’équilibreur de charge de travail. Les filtres suivants ont été ajoutés à l’équilibreur de charge de travail :

* &quot;Moi&quot; (lors du filtrage par utilisateurs)
* &quot;Mon rôle de Principal&quot; (lors du filtrage par rôles)
* &quot;Mon équipe d’accueil&quot; ou &quot;Toutes mes équipes&quot; (lors du filtrage par équipes).

Ces filtres remplacent les variables de filtre génériques $$USER.ID, $$USER.roleID, $$USER.homeTeamID et $$USER.TeamID.

Lorsque vous appliquez l’un de ces filtres, puis partagez l’équilibreur de charge de travail ou placez-le sur un tableau de bord, tous les autres utilisateurs verront leurs propres informations.

Pour plus d’informations sur l’application de filtres à l’équilibreur de charge de travail, voir [Filtrage des informations dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

## Nouveau tri des projets dans l’équilibreur de charge de travail

L’équilibreur de charge de travail trie désormais les projets en fonction de la première date de début planifiée et deuxièmement de la dernière date de fin planifiée des tâches du projet qui se produisent pendant la période que l’utilisateur affiche à l’écran. Cela vous permet d’organiser le travail dans une hiérarchie de type arborescence qui vous permet d’identifier plus facilement le travail pour une journée.

Pour plus d’informations sur l’affichage des projets et des tâches dans l’équilibreur de charge de travail, voir [Navigation dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Afficher la progression réelle du travail dans l’équilibreur de charge

Pour vous donner une perspective précise de l’avancement de votre charge de travail, nous avons ajouté un nouveau paramètre à l’équilibreur de charge de travail qui affiche la chronologie des tâches et des problèmes en fonction de leurs dates prévues. Vous pouvez activer le paramètre Afficher les dates prévues pour afficher la chronologie prévue de l’élément de travail en plus de la chronologie planifiée.

En outre, avec cette amélioration, si une tâche ou un problème est terminé avant la date d’achèvement prévue, les heures allouées des jours restants sont effectuées pour indiquer qu’elles ne sont pas prises en compte dans l’allocation globale de l’utilisateur.

Pour plus d’informations sur la navigation dans l’équilibreur de charge de travail et l’activation des paramètres, voir [Navigation dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Fonctionnalités de l’équilibreur de charge de travail précédemment communiquées comme version 20.2

* [Ajuster l’affectation quotidienne et hebdomadaire dans l’équilibreur de charge de travail](#adjust-daily-and-weekly-allocation-in-the-workload-balancer)
* [Mise à jour des heures planifiées de la tâche dans l’équilibreur de charge](#update-task-planned-hours-in-the-workload-balancer)
* [Une méthode plus pratique pour mettre à jour les allocations dans l’équilibreur de charge de travail](#a-more-convenient-way-to-update-allocations-in-the-workload-balancer)

### Ajuster l’affectation quotidienne et hebdomadaire dans l’équilibreur de charge de travail {#adjust-daily-and-weekly-allocation-in-the-workload-balancer}

Pour éviter l’épuisement de vos ressources, vous pouvez maintenant ajuster l’allocation quotidienne et hebdomadaire de vos utilisateurs afin qu’elle fonctionne à l’aide de l’équilibreur de charge de travail.

Avant cette amélioration, cela n’était possible qu’à l’aide des outils de planification des ressources.

Pour plus d’informations sur la gestion des affectations dans l’équilibreur de charge de travail, voir [Gestion des affectations utilisateur dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

**Disponible dans ces environnements :**

* Adobe Workfront Classic
* Nouvelle expérience Adobe Workfront

### Mise à jour des heures planifiées de la tâche dans l’équilibreur de charge {#update-task-planned-hours-in-the-workload-balancer}

>[!NOTE]
>
>Cette amélioration sera disponible dans Production peu de temps après la version 2020.2.

Une nouvelle option de la zone Gestion des ressources du niveau d’accès permet désormais aux utilisateurs disposant de cet accès de modifier les heures planifiées à partir de l’équilibreur de charge de travail. Lorsque vous ajustez les affectations dans l’équilibreur de charge de travail, le total des affectations quotidiennes n’a pas besoin de correspondre au nombre d’heures planifiées des tâches. Une fois les affectations enregistrées, le total des heures d’affectation devient les Heures planifiées de la tâche. Cela n’est possible que pour les tâches ayant un type de durée simple.

Pour plus d’informations sur la gestion des affectations dans l’équilibreur de charge de travail, voir [Gestion des affectations utilisateur dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

Pour plus d’informations sur l’octroi de l’accès à la gestion des ressources, voir [Accorder l’accès à la gestion des ressources](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md).

### Une méthode plus pratique pour mettre à jour les allocations dans l’équilibreur de charge de travail {#a-more-convenient-way-to-update-allocations-in-the-workload-balancer}

Pour faciliter la gestion des affectations d’un utilisateur à un élément de travail dans l’équilibreur de charge de travail, vous pouvez maintenant double-cliquer sur l’élément de travail. Vous pouvez également continuer à utiliser l’option de menu Modifier les affectations existante. En outre, vous n’avez plus besoin d’activer l’affichage des allocations pour pouvoir les mettre à jour.

Pour plus d’informations sur la gestion des affectations dans l’équilibreur de charge de travail, voir [Gestion des affectations utilisateur dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).
