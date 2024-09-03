---
content-type: release-notes
navigation-topic: product-releases-archive
title: Activité Version 2017.3, version bêta 4
description: Cette page décrit l’ensemble des changements les plus récents disponibles dans l’environnement de prévisualisation avec la version 2017.3, version bêta 4. Les fonctionnalités de cette page ont été mises à disposition dans l’environnement de prévisualisation la semaine du 25 septembre 2017. Elles ont été rendues disponibles dans l’environnement de production début novembre 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: d6bb889c-a057-453f-8f80-761cfb1ad4a1
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1676'
ht-degree: 100%

---

# Activité Version 2017.3, version bêta 4

Cette page décrit l’ensemble des changements les plus récents disponibles dans l’environnement de prévisualisation avec la version 2017.3, version bêta 4. Les fonctionnalités de cette page ont été mises à disposition dans l’environnement de prévisualisation la semaine du 25 septembre 2017. Elle ont été rendues disponibles dans l’environnement de production début novembre 2017.

>[!IMPORTANT]
>
>Les fonctionnalités décrites sur cette page peuvent être modifiées avant d’être disponibles dans l’environnement de production.

Pour obtenir la liste de toutes les modifications apportées à la version 2017.3, voir [Vue d’ensemble de l’activité Version 2017.3](../../../../product-announcements/product-releases/quarterly-release-archive/2017.3-release-activity/2017-3-release-activity-overview.md).

La version 2017.3, version bêta 4 contient des améliorations pour l’équipe d’administration de Workfront et les autres personnes :

**Pour les administrateurs et administratrices**

* [Nouvelle zone de préférences pour la gestion des ressources dans la zone de configuration](#new-resource-management-preferences-area-in-the-setup-area)

**Pour tous les utilisateurs et utilisatrices**

* [Dupliquer les tâches](#duplicate-tasks)
* [Automatiser les affectations lors de la planification des ressources](#automate-assignments-when-scheduling-resources)
* [Modifier les affectations pour des tâches multiples lors de la planification des ressources](#modify-assignments-for-multiple-tasks-when-scheduling-resources)
* [Appliquer la répartition des équivalents temps complet au planificateur de ressources](#apply-fte-distribution-to-the-resource-planner)
* [La section Fonction des paramètres utilisateur inclut le pourcentage de disponibilité équivalent temps complet.](#job-role-section-for-user-settings-includes-percentage-of-fte-availability)
* [Enregistrer et gérer les filtres dans le rapport d’utilisation d’un projet](#save-and-manage-filters-in-the-utilization-report-on-a-project)
* [Options de filtrage supplémentaires dans le rapport d’utilisation](#additional-filtering-options-in-the-utilization-report)
* [Consulter le rapport d’utilisation par programme ou par portfolio](#view-the-utilization-report-by-program-or-portfolio)
* [Afficher les informations sur le problème d’origine dans les rapports de tâches et de projets](#show-original-issue-information-in-project-and-task-reports)
* [Les mises à jour du système de filtrage dans le flux de mise à jour sont désormais persistantes d’un objet à l’autre.](#filter-system-updates-in-the-update-stream-is-now-persistent-across-objects)
* [Rapport sur les étapes de vérification actives au sein de Workfront](#report-on-active-proof-stages-within-workfront)
* [Attribuer des profils d’autorisation Workfront Proof personnalisés à des personnes dans Workfront](#assign-custom-workfront-proof-permission-profiles-to-users-within-workfront)
* [Ajout d’une ressource Heure aux abonnements aux événements](#hour-resource-added-to-event-subscriptions)

## Dupliquer les tâches {#duplicate-tasks}

Vous pouvez désormais dupliquer rapidement une tâche ou un ensemble de tâches au sein d’un projet. Cette action crée une tâche identique à la tâche originale. Il n’y a pas d’options supplémentaires pendant le processus de duplication qui vous permettraient d’apporter des modifications à la tâche nouvellement créée.  

Avant ce changement, vous pouviez copier une tâche dans un nouveau projet ou dans un projet existant et modifier certaines informations au moment de la copie.

Pour plus d’informations sur la duplication des tâches, voir [Copier et dupliquer des tâches](../../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

## Automatiser les affectations lors de la planification des ressources {#automate-assignments-when-scheduling-resources}

>[!NOTE]
>
>Les outils de planification des ressources ont été retirés de Workfront avec la version 23.1. Pour plus d’informations sur la planification des ressources à l’aide de l’équilibreur de charge de travail, voir [Vue d’ensemble de l’équilibreur de charge de travail](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Vous pouvez désormais autoriser Workfront à proposer automatiquement des affectations pour les tâches et les problèmes non affectés lors de la planification des ressources pour plusieurs projets (à partir de l’onglet Planification) ou lors de la planification des ressources pour un seul projet (à partir de l’onglet Personnel).

Workfront analyse les affectations de travail actuelles parmi vos utilisateurs et utilisatrices disponibles et propose des affectations intelligentes et logiques pour l’ensemble des tâches et problèmes qui ne sont pas encore affectés. Vous pouvez modifier les affectations proposées ou existantes avant de les finaliser.

Pour plus d’informations, voir « Attribuer manuellement des tâches et des problèmes non assignés dans les zones de planification ».

## Modifier les affectations pour des tâches multiples lors de la planification des ressources {#modify-assignments-for-multiple-tasks-when-scheduling-resources}

Lors de l’affectation, de la permutation ou de la désaffectation en masse de personnes durant la planification de ressources (à partir de l’onglet Planification ou de l’onglet Personnel), vous pouvez désormais modifier les affectations pour des tâches spécifiques que vous désignez (y compris toutes les sous-tâches et les problèmes associés) au sein d’un ou de plusieurs projets.

Avant cette modification, vous ne pouviez modifier les affectations aux tâches et aux problèmes que pour des projets entiers. Il était en effet impossible de désigner des tâches spécifiques au sein d’un projet.

Pour plus d’informations, voir « Attribuer manuellement des tâches et des problèmes non assignés dans les zones de planification ».

## Appliquer la répartition équivalent temps complet au planificateur de ressources {#apply-fte-distribution-to-the-resource-planner}

>[!NOTE]
>
>Cette fonctionnalité n’est pas encore disponible en version préliminaire sur tous les clusters.

Vous pouvez désormais afficher le nombre correct d’heures disponibles pour chaque rôle de la personne en fonction du pourcentage de disponibilité équivalent temps complet de chaque rôle si la personne en a plus d’un.

Par exemple, si l’emploi du temps d’une personne indique qu’elle est disponible pour travailler 100 heures au cours d’un mois, que son pourcentage de disponibilité équivalent temps complet pour le rôle principal est de 75 % et que le pourcentage de disponibilité équivalent temps complet de son autre rôle est de 25 %, le planificateur de ressources affichera 75 heures disponibles sous le rôle principal et 25 heures disponibles sous l’autre rôle.

Avant cette modification, le nom de la personne ne s’affichait dans le planificateur de ressources que pour le rôle principal, et la disponibilité totale de la personne sur la base de son planning (100 heures) n’était associée qu’au rôle principal. Son autre rôle ne s’affichait dans le planificateur de ressources que si la personne était affectée à une tâche dans ce rôle et si ses heures disponibles dans l’autre rôle étaient nulles.

Pour plus d’informations sur la manière dont les heures et les équivalents temps complet disponibles sont calculés pour les personnes et les rôles dans le planificateur de ressources, voir [Vue d’ensemble du calcul des heures et des équivalents temps complet pour les personnes et les rôles dans le planificateur de ressources](../../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md).

## La section Fonction des paramètres de la personne inclut le pourcentage de disponibilité équivalent temps complet. {#job-role-section-for-user-settings-includes-percentage-of-fte-availability}

>[!NOTE]
>
>Cette fonctionnalité n’est pas encore disponible en version préliminaire sur tous les clusters.

Désormais, lors de la mise à jour d’un profil de l’utilisateur ou de l’utilisatrice, vous pouvez ajouter des fonctions supplémentaires à une personne et définir le pourcentage équivalent temps complet alloué à chaque fonction.

Avant cette modification, il n’était pas possible d’attribuer un nombre spécifique d’équivalent temps complet à l’une des fonctions auxquelles la personne était associée.

Pour plus d’informations sur la mise à jour du pourcentage de disponibilité équivalent temps complet pour les fonctions de la personne, consultez [Modifier le profil d’un utilisateur ou d’une utilisatrice](../../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) ou [Configurer mes paramètres](../../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

## Nouvelle zone de préférences pour la gestion des ressources dans la zone de configuration {#new-resource-management-preferences-area-in-the-setup-area}

Vous trouverez désormais une nouvelle zone dans Configuration appelée Gestion des ressources. Dans cette zone, nous avons ajouté un paramètre qui vous permet de spécifier comment calculer la disponibilité des utilisateurs et utilisatrices dans le planificateur de ressources. Vous pouvez la calculer à l’aide des méthodes suivantes :

* Manuellement : le planning par défaut du système ainsi que l’équivalent temps complet individuel de l’utilisateur ou de l’utilisatrice sont utilisés pour déterminer la disponibilité horaire de l’utilisateur ou de l’utilisatrice dans le planificateur de ressources. Le planning de la personne est ignoré.

* Automatiquement : le planning de l’utilisateur ou de l’utilisatrice est utilisé pour déterminer la disponibilité horaire de l’utilisateur ou de l’utilisatrice dans le planificateur de ressources. La disponibilité équivalent temps complet est calculée sur la base du planning de l’utilisateur ou de l’utilisatrice et du planning par défaut. La valeur de l’ETP de la personne est ignorée. 

Pour plus d’informations sur la configuration des préférences de gestion des ressources pour votre système, consultez [Configurer les préférences de gestion des ressources](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

## Enregistrer et gérer les filtres dans le rapport d’utilisation d’un projet {#save-and-manage-filters-in-the-utilization-report-on-a-project}

Vous pouvez désormais enregistrer les filtres que vous créez dans le rapport d’utilisation. En outre, vous pouvez renommer un filtre enregistré, dupliquer un filtre enregistré, supprimer un filtre enregistré ou modifier un filtre enregistré.

Auparavant, vous deviez spécifier des options de filtrage individuelles à chaque fois que vous filtriez le rapport d’utilisation.

Pour plus d’informations sur l’enregistrement et la gestion des filtres dans le rapport d’utilisation, consultez [Vue d’ensemble du rapport d’utilisation des ressources](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) dans [Vue d’ensemble du rapport d’utilisation des ressources](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Options de filtrage supplémentaires dans le rapport d’utilisation {#additional-filtering-options-in-the-utilization-report}

Désormais, lors de l’exécution du rapport d’utilisation, de nouveaux champs de filtrage pour Portfolios, Programmes et Projets sont disponibles lors de la création de votre filtre, en plus des champs Tâches, Problèmes et Rôles qui étaient auparavant disponibles.

Avant cette modification, vous pouviez filtrer par portfolio, programme et projet uniquement en ajoutant une nouvelle règle de filtrage.

Pour plus d’informations, consultez [Vue d’ensemble du rapport d’utilisation des ressources](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) dans [Vue d’ensemble du rapport d’utilisation des ressources](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Consulter le rapport d’utilisation par programme ou par portfolio {#view-the-utilization-report-by-program-or-portfolio}

Vous pouvez désormais consulter un rapport d’utilisation par programme ou par portfolio. Cela vous permet de voir les informations de plusieurs projets dans un seul rapport d’utilisation.

Pour faciliter ce changement, l’onglet Utilisation est désormais disponible à la fois dans la zone Rapports de Workfront et dans un projet individuel.

Avant cette modification, les rapports d’utilisation n’étaient accessibles que dans un projet.

Pour plus d’informations, consultez [Vue d’ensemble du rapport d’utilisation des ressources](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Afficher les informations du problème initial dans les rapports de projet et de tâche {#show-original-issue-information-in-project-and-task-reports}

>[!NOTE]
>
>Cette fonctionnalité n’est pas encore disponible en version préliminaire sur tous les clusters.

Vous pouvez désormais trouver les informations suivantes sur le problème initial dans un rapport de projet ou de tâche, pour les projets et les tâches qui ont été créés en convertissant un problème :

* Date d’entrée du problème initial
* Nom du problème initial
* ID de créateur ou créatrice du problème initial

Ces informations peuvent être affichées dans un rapport ou une liste de tâches ou de projets en créant une vue personnalisée en mode texte.

Avant ce changement, vous ne pouviez pas générer de rapports sur ces informations.

Pour plus d’informations sur la création d’une vue personnalisée en mode texte qui capture les informations du problème initial, consultez [Vue : afficher les informations du problème initial sur les listes de tâches et de projets](../../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-original-issue-info-task-project-list.md).

## L’option Filtrer les mises à jour du système dans le flux de mise à jour est désormais persistante d’un objet à l’autre. {#filter-system-updates-in-the-update-stream-is-now-persistent-across-objects}

>[!NOTE]
>
>Cette fonctionnalité n’a pas été introduite dans l’environnement de prévisualisation avec la version bêta 4. Elle sera disponible dans l’environnement de prévisualisation dans la première quinzaine d’octobre.

L’option Filtrer les mises à jour du système est désormais persistante pour tous les objets du site Workfront. Cela vous permet de masquer les mises à jour du système et de n’afficher que les commentaires des utilisateurs et utilisatrices dans le flux de mises à jour d’un objet, et de conserver ce paramètre lorsque vous naviguez vers d’autres objets.

Avant cette modification, vous deviez choisir de filtrer les mises à jour du système pour chaque objet lorsque vous naviguiez sur le site Workfront.

Pour plus d’informations, consultez la section [Mettre à jour le travail](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Rapport sur les étapes de vérification actives au sein de Workfront {#report-on-active-proof-stages-within-workfront}

Lors de la création d’un rapport de version du document dans Workfront, une nouvelle colonne est disponible, « Étapes de vérification actives ». Cette colonne vous permet de visualiser l’étape de relecture actuellement active pour chaque version du document dans le rapport. Le nom de l’étape est affiché dans la colonne « Étapes de vérification actives ». Si aucune étape n’est actuellement active dans la version du document, la colonne est vide.

Pour plus d’informations sur les champs disponibles dans les vues et les rapports, voir [Glossaire de la terminologie Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

## Affecter des profils d’autorisation Workfront Proof personnalisés à des personnes dans Workfront {#assign-custom-workfront-proof-permission-profiles-to-users-within-workfront}

Désormais, lorsque vous accorder des autorisations en relecture pour une personne dans Workfront, vous pouvez affecter un profil d’autorisation Workfront Proof personnalisé. 

Avant cette modification, seuls les profils d’autorisation suivants étaient disponibles : Superviseur et superviseuse, Gestionnaire, Administrateur et administratrice.

## Ajout d’une ressource Heure aux abonnements aux événements {#hour-resource-added-to-event-subscriptions}

En utilisant la nouvelle ressource Heure, vous pouvez désormais créer un abonnement à un événement pour que votre application de facturation reste synchronisée avec Workfront.

Pour en savoir plus sur les abonnements aux événements, voir [API d’abonnement aux événements](../../../../wf-api/general/event-subs-api.md).
