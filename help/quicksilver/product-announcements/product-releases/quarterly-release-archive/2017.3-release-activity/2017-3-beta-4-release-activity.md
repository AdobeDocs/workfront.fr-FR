---
content-type: release-notes
navigation-topic: product-releases-archive
title: Activité Version 2017.3, version bêta 4
description: Cette page décrit toutes les modifications les plus récentes disponibles dans l’environnement Aperçu avec la version 2017.3 de Beta 4. Les fonctionnalités de cette page ont été rendues disponibles dans l’environnement Aperçu au cours de la semaine du 25 septembre 2017. Il sera disponible dans l’environnement de production début novembre 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: d6bb889c-a057-453f-8f80-761cfb1ad4a1
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1676'
ht-degree: 1%

---

# Activité Version 2017.3, version bêta 4

Cette page décrit toutes les modifications les plus récentes disponibles dans l’environnement Aperçu avec la version 2017.3 de Beta 4. Les fonctionnalités de cette page ont été rendues disponibles dans l’environnement Aperçu au cours de la semaine du 25 septembre 2017. Il sera disponible dans l’environnement de production début novembre 2017.

>[!IMPORTANT]
>
> Les fonctionnalités décrites sur cette page peuvent être modifiées avant leur disponibilité dans l’environnement de production.

Pour obtenir la liste de toutes les modifications apportées à la version 2017.3, voir  [Présentation de l’activité de version 2017.3](../../../../product-announcements/product-releases/quarterly-release-archive/2017.3-release-activity/2017-3-release-activity-overview.md).

La version 2017.3 de Beta 4 contient des améliorations pour les administrateurs de Workfront et d’autres utilisateurs :

**Pour les administrateurs**

* [Nouvelle zone de préférences de gestion des ressources dans la zone de configuration](#new-resource-management-preferences-area-in-the-setup-area)

**Pour Tous Les Utilisateurs**

* [ Tâches en double ](#duplicate-tasks)
* [Automatiser les affectations lors de la planification des ressources](#automate-assignments-when-scheduling-resources)
* [Modifier les affectations pour plusieurs tâches lors de la planification de ressources](#modify-assignments-for-multiple-tasks-when-scheduling-resources)
* [ Application de la distribution FTE au planificateur de ressources ](#apply-fte-distribution-to-the-resource-planner)
* [La section Rôle de tâche pour les paramètres utilisateur inclut le pourcentage de disponibilité de l’éditeur de texte enrichi](#job-role-section-for-user-settings-includes-percentage-of-fte-availability)
* [Enregistrer et gérer les filtres dans le rapport d’utilisation d’un projet](#save-and-manage-filters-in-the-utilization-report-on-a-project)
* [Options de filtrage supplémentaires dans le rapport d’utilisation](#additional-filtering-options-in-the-utilization-report)
* [Afficher le rapport d’utilisation par programme ou Portfolio](#view-the-utilization-report-by-program-or-portfolio)
* [Afficher les informations de problème d’origine dans les rapports de projet et de tâche](#show-original-issue-information-in-project-and-task-reports)
* [Les mises à jour du système de filtrage dans le flux de mise à jour sont maintenant persistantes dans tous les objets](#filter-system-updates-in-the-update-stream-is-now-persistent-across-objects)
* [Rapport sur les phases de BAT actives dans Workfront](#report-on-active-proof-stages-within-workfront)
* [Attribution de profils d’autorisation Workfront Proof personnalisés aux utilisateurs dans Workfront](#assign-custom-workfront-proof-permission-profiles-to-users-within-workfront)
* [Ressource d’heure ajoutée aux abonnements à un événement](#hour-resource-added-to-event-subscriptions)

## Dupliquer les tâches {#duplicate-tasks}

Vous pouvez désormais dupliquer rapidement une tâche ou un ensemble de tâches au sein d’un projet. Cette action crée une tâche identique à celle d’origine. Il n’existe aucune option supplémentaire pendant le processus de duplication qui vous permettrait d’apporter des modifications à la tâche nouvellement créée.  

Avant cette modification, vous pouvez copier une tâche vers un nouveau projet ou le projet existant et modifier certaines informations au fur et à mesure que vous la copiez.

Pour  Pour plus d’informations sur la duplication des tâches, voir [Copier et dupliquer des tâches](../../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

## Automatisation des affectations lors de la planification des ressources {#automate-assignments-when-scheduling-resources}

>[!NOTE]
>
>Les outils de planification des ressources ont été abandonnés et supprimés de Workfront avec la version 23.1. Pour plus d’informations sur la planification des ressources à l’aide de l’équilibreur de charge de travail, voir [Présentation de l’équilibreur de charge de travail](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Vous pouvez désormais permettre à Workfront de proposer automatiquement des affectations pour des tâches et des problèmes non attribués lors de la planification des ressources pour plusieurs projets (depuis l’onglet Planification ) ou lors de la planification des ressources pour un seul projet (depuis l’onglet Personnel ).

Workfront analyse les affectations de travail actuelles parmi vos utilisateurs disponibles et propose des affectations intelligentes et logiques pour toutes les tâches ou tous les problèmes qui ne sont pas encore affectés. Vous pouvez modifier les affectations proposées ou existantes avant de finaliser les affectations.

Pour plus d’informations, voir &quot;Affectation manuelle de tâches et de problèmes non attribués dans les zones Planification&quot;.

## Modification des affectations pour plusieurs tâches lors de la planification de ressources {#modify-assignments-for-multiple-tasks-when-scheduling-resources}

Lors de l’affectation, de la permutation ou de l’annulation de l’affectation groupée d’utilisateurs lors de la planification de ressources (que ce soit à partir de l’onglet Planification ou de l’onglet Personnel), vous pouvez désormais modifier les affectations pour des tâches spécifiques que vous désignez (y compris toutes les sous-tâches et les problèmes associés) au sein d’un ou de plusieurs projets.

Avant cette modification, vous ne pouviez modifier les affectations aux tâches et problèmes que pour des projets entiers (vous ne pouviez pas désigner de tâches spécifiques au sein d’un projet).

Pour plus d’informations, voir &quot;Affectation manuelle de tâches et de problèmes non attribués dans les zones Planification&quot;.

## Application de la distribution FTE au planificateur de ressources {#apply-fte-distribution-to-the-resource-planner}

>[!NOTE]
>
>Cette fonctionnalité n’est actuellement pas disponible dans Aperçu sur toutes les grappes.

Vous pouvez désormais afficher le nombre correct d’heures disponibles pour chaque rôle de l’utilisateur, en fonction du pourcentage de disponibilité de l’éditeur de texte enrichi pour chaque rôle, lorsque les utilisateurs disposent de plusieurs rôles.

Par exemple, si le planning d’un utilisateur indique qu’il est disponible pour travailler 100 heures par mois, et que son pourcentage de disponibilité à l’éditeur de texte enrichi pour le rôle de Principal est de 75 % et que le pourcentage de disponibilité à l’éditeur de texte enrichi de son autre rôle est de 25 %, le planificateur de ressources liste l’utilisateur avec 75 heures disponibles sous le rôle de Principal et 255 heures disponibles sous son autre rôle.

Avant cette modification, le nom de l’utilisateur s’affichait dans le planificateur de ressources uniquement pour le rôle de Principal, et la disponibilité complète de l’utilisateur selon son planning (100 heures) était associée uniquement au rôle de Principal. L’autre rôle de l’utilisateur s’affichait dans le planificateur de ressources uniquement si l’utilisateur était affecté à une tâche dans ce rôle et que les heures disponibles pour l’utilisateur dans l’autre rôle étaient nulles.

Pour plus d’informations sur la façon dont les heures disponibles et les ETR disponibles sont calculés pour les utilisateurs et les rôles dans le planificateur de ressources, voir [Présentation des heures de calcul et de l’ETR pour les utilisateurs et les rôles dans le planificateur de ressources](../../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md).

## La section Rôle de tâche des paramètres utilisateur inclut le pourcentage de disponibilité de l’éditeur de texte enrichi {#job-role-section-for-user-settings-includes-percentage-of-fte-availability}

>[!NOTE]
>
>Cette fonctionnalité n’est actuellement pas disponible dans Aperçu sur toutes les grappes.

Désormais, lors de la mise à jour d’un profil utilisateur, vous pouvez ajouter des rôles de tâche supplémentaires à un utilisateur et définir le pourcentage de l’éditeur de texte enrichi alloué à chaque rôle de tâche.

Avant cette modification, vous ne pouviez pas allouer un montant spécifique de l’éditeur de texte enrichi à l’un des rôles de tâche auxquels l’utilisateur était associé.

Pour plus d’informations sur la mise à jour du pourcentage de disponibilité de l’éditeur de texte enrichi pour les rôles de travail de l’utilisateur, voir [Modification du profil d’un utilisateur](../../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) ou [Configurer mes paramètres](../../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

## Nouvelle zone de préférences de gestion des ressources dans la zone de configuration {#new-resource-management-preferences-area-in-the-setup-area}

Vous trouverez désormais une nouvelle zone dans Configuration appelée Gestion des ressources. Dans cette zone, nous avons introduit un paramètre qui vous permet de spécifier comment calculer la disponibilité des utilisateurs dans le planificateur de ressources. Vous pouvez le calculer à l’aide des méthodes suivantes :

* Manuellement : le planning par défaut du système, en plus de l’éditeur de texte enrichi de l’utilisateur, est utilisé pour déterminer la disponibilité horaire de l’utilisateur dans le planificateur de ressources. Le planning de l’utilisateur est ignoré.
* Automatiquement : le planning de l’utilisateur est utilisé pour déterminer la disponibilité horaire de l’utilisateur dans le planificateur de ressources. La disponibilité de l’éditeur de texte enrichi est calculée en fonction de la planification de l’utilisateur et de la planification par défaut. La valeur de l’utilisateur FTE est ignorée. 

Pour plus d’informations sur la configuration des préférences de gestion des ressources pour votre système, voir [Configuration des préférences de gestion des ressources](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

## Enregistrement et gestion des filtres dans le rapport Utilisation d’un projet {#save-and-manage-filters-in-the-utilization-report-on-a-project}

Vous pouvez désormais enregistrer les filtres que vous créez dans le rapport Utilisation . En outre, vous pouvez renommer un filtre enregistré, dupliquer un filtre enregistré, supprimer un filtre enregistré ou modifier un filtre enregistré.

Auparavant, vous deviez spécifier des options de filtre individuelles chaque fois que vous filtrez le rapport Utilisation .

Pour plus d’informations sur l’enregistrement et la gestion des filtres dans le rapport Utilisation, voir [Présentation du rapport Utilisation des ressources](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) dans [Présentation du rapport Utilisation des ressources](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Options de filtrage supplémentaires dans le rapport Utilisation {#additional-filtering-options-in-the-utilization-report}

Désormais, lors de l’exécution du rapport Utilisation, de nouveaux champs de filtrage pour les Portfolios, les programmes et les projets sont disponibles lors de la création de votre filtre, en plus des champs Tâches, Problèmes et Rôles précédemment disponibles.

Avant cette modification, vous ne pouviez filtrer par portefeuille, programme et projet qu’en ajoutant une nouvelle règle de filtrage.

Pour plus d’informations, voir [Présentation du rapport d’utilisation des ressources](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) dans [Présentation du rapport d’utilisation des ressources](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Afficher le rapport d’utilisation par programme ou Portfolio {#view-the-utilization-report-by-program-or-portfolio}

Vous pouvez désormais afficher un rapport d’utilisation par programme ou portefeuille. Vous pouvez ainsi afficher les informations de plusieurs projets dans un seul rapport d’utilisation.

Pour faciliter cette modification, l’onglet Utilisation est désormais disponible dans la zone de création de rapports de Workfront, ainsi que dans un projet individuel.

Avant cette modification, les rapports d’utilisation n’étaient accessibles que dans un projet.

Pour plus d’informations, voir  [Présentation du rapport d’utilisation des ressources](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md). 

## Afficher les informations originales sur le problème dans les rapports sur les projets et les tâches {#show-original-issue-information-in-project-and-task-reports}

>[!NOTE]
>
>Cette fonctionnalité n’est actuellement pas disponible dans Aperçu sur toutes les grappes.

Vous trouverez maintenant les informations suivantes sur le problème d’origine dans un rapport de projet ou de tâche, pour les projets et les tâches qui ont été créés en convertissant un problème :

* Date d’entrée du problème d’origine
* Nom original du problème
* ID d’auteur du problème original

Ces informations peuvent être affichées dans un rapport ou une liste de tâche ou de projet en créant une vue personnalisée en mode texte.

Avant cette modification, vous ne pouviez pas générer de rapports sur ces informations.

Pour plus d’informations sur la création d’une vue de mode de texte personnalisé qui capture les informations du problème d’origine, voir [Affichage : afficher les informations du problème d’origine sur les listes de tâches et de projets](../../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-original-issue-info-task-project-list.md).

## Les mises à jour du système de filtrage dans le flux de mise à jour sont maintenant persistantes dans tous les objets {#filter-system-updates-in-the-update-stream-is-now-persistent-across-objects}

>[!NOTE]
>
>Cette fonctionnalité n’a pas été publiée dans l’environnement Aperçu avec Beta 4. Il sera disponible dans Aperçu au premier semestre d’octobre.

L’option Filtrer les mises à jour du système est désormais persistante sur tous les objets du site Workfront. Vous pouvez ainsi masquer les mises à jour du système et afficher uniquement les commentaires des utilisateurs dans le flux de mise à jour sur un objet. Ce paramètre reste conservé lorsque vous accédez à d’autres objets.

Avant cette modification, vous deviez choisir de filtrer les mises à jour du système pour chaque objet lorsque vous parcourez le site Workfront.

Pour plus d’informations, consultez la section [Mettre à jour le travail](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Rapport sur les phases de BAT actives dans Workfront {#report-on-active-proof-stages-within-workfront}

Lors de la création d’un rapport Version du document dans Workfront, une colonne intitulée &quot;Étapes de Bon à tirer actives&quot; s’affiche désormais. Cette colonne vous permet d’afficher l’étape du BAT actuellement active sur chaque version de document du rapport. Le nom de l’étape s’affiche dans la colonne &quot;Étapes de Bon à tirer actives&quot;. Si aucune étape n’est actuellement active sur la version du document, la colonne est vide.

Pour plus d’informations sur les champs disponibles dans les vues et les rapports, voir le [Glossaire de la terminologie Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

## Attribution de profils d’autorisation Workfront Proof personnalisés aux utilisateurs dans Workfront {#assign-custom-workfront-proof-permission-profiles-to-users-within-workfront}

Désormais, lorsque vous activez les fonctionnalités de vérification pour un utilisateur dans Workfront, vous pouvez attribuer un profil d’autorisation Workfront Proof personnalisé. 

Avant cette modification, seuls les profils d’autorisation suivants étaient disponibles : superviseur, responsable, administrateur.

## Ressource d’heure ajoutée aux abonnements à un événement {#hour-resource-added-to-event-subscriptions}

Grâce à la nouvelle ressource Heure , vous pouvez désormais créer un abonnement à un événement afin que votre application de facturation reste synchronisée avec Workfront.

Pour en savoir plus sur les abonnements aux événements, voir [API d’abonnement à un événement](../../../../wf-api/general/event-subs-api.md).
