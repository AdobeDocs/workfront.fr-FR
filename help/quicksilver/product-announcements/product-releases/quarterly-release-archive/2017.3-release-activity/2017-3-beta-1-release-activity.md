---
content-type: release-notes
navigation-topic: product-releases-archive
title: Activité Version 2017.3, version bêta 1
description: Cette page décrit toutes les modifications les plus récentes disponibles dans l’environnement Aperçu avec la version 2017.3. Les fonctionnalités de cette page ont été rendues disponibles dans l’environnement Aperçu le 9 août 2017. Il sera disponible dans l’environnement de production début novembre 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 33a91c25-98ec-4f08-b444-4e11e05e464b
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1426'
ht-degree: 2%

---

# Activité Version 2017.3, version bêta 1

Cette page décrit toutes les modifications les plus récentes disponibles dans l’environnement Aperçu avec la version 2017.3. Les fonctionnalités de cette page ont été rendues disponibles dans l’environnement Aperçu le 9 août 2017. Il sera disponible dans l’environnement de production début novembre 2017.

>[!IMPORTANT]
>
> Les fonctionnalités décrites sur cette page peuvent être modifiées avant leur disponibilité dans l’environnement de production.

Pour obtenir la liste de toutes les modifications apportées à la version 2017.3, voir  [Présentation de l’activité de version 2017.3](../../../../product-announcements/product-releases/quarterly-release-archive/2017.3-release-activity/2017-3-release-activity-overview.md).

La version 2017.3 de Beta 1 contient des améliorations tant pour les administrateurs de Workfront que pour d’autres utilisateurs :

**Pour les administrateurs :**

* [Empêcher la suppression des tâches et des problèmes lorsque des heures sont enregistrées](#prevent-tasks-and-issues-from-being-deleted-when-hours-are-logged)
* [Suppression du paramètre &quot;Accès anticipé&quot; de la zone de configuration](#removal-of-the-early-access-setting-from-the-setup-area)
* [Modification de l’adresse électronique par défaut de Workfront](#workfront-default-email-address-change)

**Pour Tous Les Utilisateurs :**

* [Améliorations de la planification des ressources](#resource-scheduling-improvements)
* [Affichage écran large](#widescreen-display)
* [Redimensionner et réorganiser les colonnes dans les rapports et listes](#resize-and-reorder-columns-in-reports-and-lists)
* [ Option Effacer les données personnalisées lors de la copie de tâches et de problèmes](#clear-custom-data-option-when-copying-tasks-and-issues)
* [Créer un projet directement à partir d’un modèle](#create-a-project-directly-from-a-template)
* [Notification In-App pour les objets abonnés](#in-app-notification-for-subscribed-objects)
* [@Tagging actuellement indisponible dans l’environnement de prévisualisation](#tagging-currently-not-available-in-the-preview-environment)
* [Inclure les informations d’affectation des utilisateurs dans le rapport Utilisation d’un projet](#include-user-allocation-information-in-the-utilization-report-on-a-project)

## Amélioration de la planification des ressources {#resource-scheduling-improvements}

>[!NOTE]
>
>Les outils de planification des ressources ont été abandonnés et supprimés de Workfront avec la version 23.1. Pour plus d’informations sur la planification des ressources à l’aide de l’équilibreur de charge de travail, voir [Présentation de l’équilibreur de charge de travail](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Les améliorations de planification des ressources suivantes sont disponibles lors de la planification des ressources pour une équipe, pour un projet ou pour plusieurs projets en tant que gestionnaire de ressources :

* [ Afficher la zone de planification en mode plein écran ](#view-scheduling-area-in-full-screen-mode)
* [Plus d’options de plage de dates pour afficher la zone de planification des ressources](#more-date-range-options-for-viewing-the-resource-scheduling-area)
* [Affichage des dates prévues dans la chronologie de planification](#view-projected-dates-on-the-scheduling-timeline)

### Affichage de la zone de planification en mode plein écran {#view-scheduling-area-in-full-screen-mode}

Vous pouvez afficher la chronologie de la planification en mode plein écran, ce qui vous permet d’afficher plus d’informations dans une seule vue. 

Pour plus d’informations, voir &quot;Prise en main de la planification des ressources&quot;.

### Plus d’options de période pour l’affichage de la zone de planification des ressources {#more-date-range-options-for-viewing-the-resource-scheduling-area}

Vous pouvez afficher les options de période supplémentaires suivantes lors de l’affichage de la chronologie de planification :

* Vue d’un seul jour
* Affichage 4 semaines
* Vue de 6 semaines

Avant cette modification, vous ne pouviez afficher la chronologie de la planification que dans une vue d’une semaine, de deux semaines ou de trois semaines. Ces périodes sont toujours disponibles en plus des nouvelles périodes.

Lorsque vous affichez la chronologie de la planification dans une vue d’un seul jour, les allocations utilisateur (y compris le nombre total d’heures quotidiennes) ne peuvent pas s’afficher.

Pour plus d’informations, voir &quot;Prise en main de la planification des ressources&quot;.

### Affichage des dates prévues dans la chronologie de planification {#view-projected-dates-on-the-scheduling-timeline}

Vous pouvez maintenant configurer la chronologie de la planification afin qu’elle affiche les dates prévues plutôt que les dates prévues pour les tâches et les problèmes. 

Avant cette modification, les tâches et les problèmes de la chronologie de planification n’affichaient que les dates planifiées.

Lorsque vous affichez les dates prévues dans la chronologie de planification, les affectations d’utilisateurs (y compris le nombre total d’heures quotidiennes) ne peuvent pas s’afficher.

Pour plus d’informations, voir &quot;Prise en main de la planification des ressources&quot;.

## Affichage à écran large {#widescreen-display}

Lorsque vous affichez l’un des objets suivants dans Workfront, l’intégralité de la fenêtre du navigateur est automatiquement remplie :

* Projets
* Tâches
* Problèmes
* Rapports
* Tableaux de bord
* Calendriers

Avant cette modification, deux encadrés blancs se trouvaient de chaque côté de la zone affichée. Désormais, la vue grand écran s’ajuste dynamiquement à la largeur de votre écran et de la fenêtre de votre navigateur.

## Redimensionnement et réorganisation des colonnes dans les rapports et listes {#resize-and-reorder-columns-in-reports-and-lists}

Vous pouvez désormais réorganiser et redimensionner les colonnes d’un rapport ou d’une liste, sans avoir à modifier le rapport. (Cette fonctionnalité a été supprimée avec l’abandon de l’environnement Accès anticipé au début de cette année. Elle est en train d&#39;être réintroduite.)

Cette fonctionnalité n’est pas disponible pour les listes ou les rapports de tableau de bord, car ces listes ont été repensées dans une nouvelle structure de grille de données. Cette fonctionnalité sera activée pour toutes les autres listes avec cette version.

Pour plus d’informations sur le redimensionnement et la réorganisation des colonnes, voir [Modification de la largeur et de l’ordre des colonnes](../../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

## Effacer l’option Données personnalisées lors de la copie de tâches et de problèmes {#clear-custom-data-option-when-copying-tasks-and-issues}

Lors de la copie d’une tâche ou d’un problème, vous pouvez désormais sélectionner une option pour effacer toute donnée personnalisée. Lorsque vous choisissez d’effacer les données personnalisées d’une tâche ou d’un problème, le formulaire est copié dans le nouvel élément, mais pas les données personnalisées du formulaire. L’effacement de données personnalisées affecte également les formulaires personnalisés joints aux documents joints aux éléments, ou les formulaires personnalisés joints aux dépenses de la tâche.

Avant cette modification, les données personnalisées incluses dans un formulaire personnalisé étaient également copiées dans le nouvel élément lorsque vous avez copié la tâche ou le problème. 

Pour plus d’informations sur la copie de tâches, voir [Copier et dupliquer des tâches](../../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

Pour plus d’informations sur les problèmes de copie, voir [Problèmes de copie](../../../../manage-work/issues/manage-issues/copy-issues.md).

## Création directe d’un projet à partir d’un modèle {#create-a-project-directly-from-a-template}

Vous pouvez désormais créer un projet à partir d’un modèle, au niveau du modèle.

Avant cette modification, vous ne pouviez créer un projet à partir d’un modèle que dans l’onglet Projets de la zone Projets de Workfront, à l’aide de l’option **Nouveau projet à partir du modèle** .

Pour plus d’informations sur la création d’un projet à partir d’un modèle, voir [Création d’un projet à l’aide d’un modèle](../../../../manage-work/projects/create-projects/create-project-from-template.md).

## Empêcher la suppression des tâches et des problèmes lorsque des heures sont enregistrées {#prevent-tasks-and-issues-from-being-deleted-when-hours-are-logged}

Vous pouvez maintenant configurer Workfront pour autoriser ou empêcher la suppression des tâches et problèmes ayant des heures de journalisation.

Avant cette modification, lorsque vous avez supprimé une tâche ou un problème où des heures étaient consignées, les heures étaient supprimées avec la tâche ou le problème, ou elles étaient déplacées vers le projet, selon vos préférences Frise chronologique et Heures .

Pour plus d’informations sur la suppression de tâches, voir [Suppression de tâches](../../../../manage-work/tasks/manage-tasks/delete-tasks.md).

Pour plus d’informations sur les problèmes de suppression, voir [Problèmes de suppression](../../../../manage-work/issues/manage-issues/delete-issues.md).

Pour plus d’informations sur l’activation du paramètre système pour la suppression de tâches et de problèmes, voir [ Configuration des préférences de tâches à l’échelle du système et de problèmes](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

## Suppression du paramètre &quot;Accès anticipé&quot; de la zone de configuration {#removal-of-the-early-access-setting-from-the-setup-area}

Nous supprimons le paramètre qui permettait aux administrateurs de Workfront d’inscrire des utilisateurs pour participer à l’environnement Accès anticipé. Cette fonctionnalité est obsolète depuis fin 2016. Nous n’avons publié aucune nouvelle fonctionnalité d’accès anticipé en 2017 et toutes les fonctionnalités qui restaient dans cet environnement ont été déplacées vers la production.

Avant cette modification, les administrateurs de Workfront pouvaient toujours ajouter des utilisateurs à l’environnement Accès anticipé, bien qu’il n’y ait aucune nouvelle fonctionnalité d’accès.

## Modification de l’adresse électronique par défaut de Workfront {#workfront-default-email-address-change}

L’adresse email par défaut du courrier sortant Workfront est passée de [noreply@attask.com](mailto:noreply@attask.com) à [noreply@my.workfront.com](mailto:noreply@workfront.com).

Si vous filtrez actuellement les emails envoyés depuis Workfront, vous devez modifier votre filtre pour refléter la nouvelle adresse par défaut. 

La modification de l’adresse par défaut n’a aucun effet sur les adresses électroniques Workfront configurées. 

Pour plus d’informations, poursuivez votre lecture.

## Notification In-App pour les objets abonnés {#in-app-notification-for-subscribed-objects}

Lorsqu’un utilisateur fait un commentaire sur les projets, tâches et problèmes auxquels vous êtes abonné, vous recevez désormais une notification in-app. Pour en savoir plus sur les notifications in-app d’abonnement, voir [Affichage et gestion des notifications in-app](../../../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

Selon les fonctionnalités activées par votre administrateur Workfront, vous pouvez également recevoir des notifications par e-mail pour les éléments abonnés. Vous pouvez facilement vous désabonner d’un élément par le biais d’un lien sur un email d’abonnement, comme décrit dans la section [Notifications Adobe Workfront](../../../../workfront-basics/using-notifications/wf-notifications.md).

Avant cette modification, vous avez toujours reçu une notification par e-mail pour les éléments abonnés et il n’y avait pas d’option pour recevoir une notification in-app.

Bien que vous puissiez désactiver les courriers électroniques d’abonnement, vous ne pouvez pas désactiver les notifications in-app pour les articles abonnés. Pour plus d’informations, voir [Configuration des notifications d’événement pour tous les membres du système](../../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

Pour en savoir plus sur l’abonnement aux éléments, voir [Abonnement aux éléments dans Adobe Workfront](../../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md).

## @Tagging n’est actuellement pas disponible dans l’environnement de prévisualisation {#tagging-currently-not-available-in-the-preview-environment}

Alors que nous nous efforçons d’intégrer la fonctionnalité Format de texte enrichi au flux de mise à jour, vous ne pourrez temporairement pas utiliser le symbole @ pour baliser d’autres utilisateurs dans le flux de mise à jour pour les objets suivants dans l’environnement de prévisualisation :

* Projet
* Tâche
* Problème
* Feuille de temps

Vous pouvez toujours baliser les autres en cliquant sur l&#39;icône **Inclure d&#39;autres sur cette mise à jour** .

Pour plus d’informations, consultez [Baliser d’autres personnes sur les mises à jour](../../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

## Inclure les informations d’affectation des utilisateurs dans le rapport Utilisation d’un projet {#include-user-allocation-information-in-the-utilization-report-on-a-project}

>[!NOTE]
>
>Les outils de planification des ressources ont été abandonnés et supprimés de Workfront avec la version 23.1. Pour plus d’informations sur la planification des ressources à l’aide de l’équilibreur de charge de travail, voir [Présentation de l’équilibreur de charge de travail](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Le rapport Utilisation d’un projet prend désormais en compte la réaffectation des heures planifiées sur toute la durée d’une tâche. Lorsque l’affectation des utilisateurs pour les heures a été modifiée (comme décrit dans la section &quot;Gestion des affectations des utilisateurs dans les zones de planification&quot;, les données du rapport Utilisation peuvent être affectées si les dates sélectionnées dans le rapport Utilisation ne contiennent qu’une partie d’une tâche.

Pour plus d’informations, voir [Présentation du rapport d’utilisation des ressources](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).
