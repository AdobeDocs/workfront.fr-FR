---
content-type: release-notes
navigation-topic: product-releases-archive
title: Activité Version 2017.3, version bêta 1
description: Cette page décrit toutes les modifications les plus récentes disponibles dans l’environnement de prévisualisation avec la version 2017.3, version bêta 1. Les fonctionnalités de cette page ont été rendues disponibles dans l’environnement de prévisualisation le 9 août 2017. Elles ont été rendues disponibles dans l’environnement de production début novembre 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 33a91c25-98ec-4f08-b444-4e11e05e464b
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1426'
ht-degree: 100%

---

# Activité Version 2017.3, version bêta 1

Cette page décrit toutes les modifications les plus récentes disponibles dans l’environnement de prévisualisation avec la version 2017.3, version bêta 1. Les fonctionnalités de cette page ont été rendues disponibles dans l’environnement de prévisualisation le 9 août 2017. Elle ont été rendues disponibles dans l’environnement de production début novembre 2017.

>[!IMPORTANT]
>
>Les fonctionnalités décrites sur cette page peuvent être modifiées avant d’être disponibles dans l’environnement de production.

Pour obtenir la liste de toutes les modifications apportées à la version 2017.3, voir [Vue d’ensemble de l’activité Version 2017.3](../../../../product-announcements/product-releases/quarterly-release-archive/2017.3-release-activity/2017-3-release-activity-overview.md).

La version bêta 1 de la version 2017.3 contient des améliorations pour les administrateurs et administratrices de Workfront et les autres utilisateurs et utilisatrices :

**Pour les administrateurs et administratrices :**

* [Empêcher la suppression des tâches et des problèmes avec des heures consignées](#prevent-tasks-and-issues-from-being-deleted-when-hours-are-logged)
* [Suppression du paramètre « Accès anticipé » de la zone de configuration](#removal-of-the-early-access-setting-from-the-setup-area)
* [Changement de l’adresse e-mail par défaut de Workfront](#workfront-default-email-address-change)

**Pour tous les utilisateurs et utilisatrices :**

* [Amélioration de la planification des ressources](#resource-scheduling-improvements)
* [Affichage au format écran large](#widescreen-display)
* [Redimensionner et réorganiser les colonnes dans les rapports et les listes](#resize-and-reorder-columns-in-reports-and-lists)
* [Effacer l’option Données personnalisées lors de la copie de tâches et de problèmes](#clear-custom-data-option-when-copying-tasks-and-issues)
* [Créer un projet directement à partir d’un modèle](#create-a-project-directly-from-a-template)
* [Notification in-app pour les objets abonnés](#in-app-notification-for-subscribed-objects)
* [Le tag @ n’est actuellement pas disponible dans l’environnement de prévisualisation.](#tagging-currently-not-available-in-the-preview-environment)
* [Inclure les informations d’affectation des utilisateurs et utilisatrices dans le rapport d’utilisation d’un projet](#include-user-allocation-information-in-the-utilization-report-on-a-project)

## Améliorations de la planification des ressources {#resource-scheduling-improvements}

>[!NOTE]
>
>Les outils de planification des ressources ont été retirés de Workfront avec la version 23.1. Pour plus d’informations sur la planification des ressources à l’aide de l’équilibreur de charge de travail, voir [Vue d’ensemble de l’équilibreur de charge de travail](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Les améliorations de planification des ressources suivantes sont disponibles lors de la planification des ressources pour une équipe, pour un projet ou pour plusieurs projets en tant que personne gestionnaire de ressources :

* [Afficher la zone de planification en mode plein écran](#view-scheduling-area-in-full-screen-mode)
* [Plus d’options de période pour l’affichage de la zone de planification des ressources](#more-date-range-options-for-viewing-the-resource-scheduling-area)
* [Afficher les dates prévisionnelles dans la chronologie de planification](#view-projected-dates-on-the-scheduling-timeline)

### Afficher la zone de planification en mode plein écran {#view-scheduling-area-in-full-screen-mode}

Vous pouvez afficher la chronologie de la planification en mode plein écran, ce qui vous permet d’afficher plus d’informations dans une seule vue. 

Pour plus d’informations, voir « Commencer avec la planification des ressources ».

### Plus d’options de période pour l’affichage de la zone de planification des ressources {#more-date-range-options-for-viewing-the-resource-scheduling-area}

Vous pouvez afficher les options de période supplémentaires suivantes lors de l’affichage de la chronologie de la planification :

* Vue d’un seul jour
* Vue de 4 semaines
* Vue de 6 semaines

Avant cette modification, vous ne pouviez afficher la chronologie de la planification que dans une vue d’une semaine, de 2 semaines ou de 3 semaines. Ces périodes sont toujours disponibles en plus des nouvelles.

Lorsque vous affichez la chronologie de la planification dans une vue d’un seul jour, les affectations d’utilisateurs et d’utilisatrices (y compris le nombre total d’heures quotidiennes) ne peuvent pas s’afficher.

Pour plus d’informations, voir « Commencer avec la planification des ressources ».

### Afficher les dates prévisionnelles dans la chronologie de planification {#view-projected-dates-on-the-scheduling-timeline}

Vous pouvez maintenant configurer la chronologie de la planification afin qu’elle affiche les dates prévisionnelles plutôt que les dates prévues pour les tâches et les problèmes. 

Avant cette modification, les tâches et les problèmes dans la chronologie de la planification n’affichaient que les dates prévues.

Lorsque vous affichez les dates prévisionnelles dans la chronologie de la planification, les affectations d’utilisateurs et d’utilisatrices (y compris le nombre total d’heures quotidiennes) ne peuvent pas s’afficher.

Pour plus d’informations, voir « Commencer avec la planification des ressources ».

## Affichage au format écran large {#widescreen-display}

Lorsque vous affichez l’un des objets suivants dans Workfront, l’intégralité de la fenêtre du navigateur est automatiquement remplie :

* Projets
* Tâches
* Problèmes
* Rapports
* Tableaux de bord
* Calendriers

Avant cette modification, deux encadrés blancs se trouvaient de chaque côté de la zone affichée. Désormais, la vue au format écran large s’ajuste dynamiquement à la largeur de votre écran et de la fenêtre de votre navigateur.

## Redimensionner et réorganiser les colonnes dans les rapports et listes {#resize-and-reorder-columns-in-reports-and-lists}

Vous pouvez désormais réorganiser et redimensionner les colonnes d’un rapport ou d’une liste, sans avoir à modifier le rapport. (Cette fonctionnalité a été supprimée avec l’abandon de l’environnement Accès anticipé au début de cette année. Elle est en train d’être réintroduite.)

Cette fonctionnalité n’est pas disponible pour les listes ou les rapports de tableau de bord, car ces listes ont été repensées dans une nouvelle structure de grille de données. Cette fonctionnalité sera activée pour toutes les autres listes avec cette version.

Pour plus d’informations sur le redimensionnement et la réorganisation des colonnes, voir [Modifier la largeur et l’ordre des colonnes](../../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

## Effacer l’option Données personnalisées lors de la copie de tâches et de problèmes {#clear-custom-data-option-when-copying-tasks-and-issues}

Lors de la copie d’une tâche ou d’un problème, vous pouvez désormais sélectionner une option pour effacer toute donnée personnalisée.Lorsque vous choisissez d’effacer les données personnalisées d’une tâche ou d’un problème, le formulaire est copié dans le nouvel élément, mais pas les données personnalisées du formulaire. L’effacement de données personnalisées affecte également les formulaires personnalisés joints aux documents joints aux éléments, ou les formulaires personnalisés joints aux dépenses de la tâche.

Avant cette modification, les données personnalisées incluses dans un formulaire personnalisé étaient également copiées dans le nouvel élément lors de la copie de la tâche ou du problème. 

Pour plus d’informations sur la copie de tâches, voir [Copier et dupliquer des tâches](../../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

Pour plus d’informations sur la copie de problèmes, voir [Copier des problèmes](../../../../manage-work/issues/manage-issues/copy-issues.md).

## Créer un projet directement à partir d’un modèle {#create-a-project-directly-from-a-template}

Vous pouvez désormais créer un projet à partir d’un modèle, au niveau du modèle.

Avant cette modification, vous ne pouviez créer un projet à partir d’un modèle que dans l’onglet Projets de la zone Projets de Workfront, en utilisant l’option **Nouveau projet à partir d’un modèle**.

Pour plus d’informations sur la création d’un projet à partir d’un modèle, voir [Créer un projet à l’aide d’un modèle](../../../../manage-work/projects/create-projects/create-project-from-template.md).

## Empêcher la suppression des tâches et des problèmes avec des heures consignées {#prevent-tasks-and-issues-from-being-deleted-when-hours-are-logged}

Vous pouvez maintenant configurer Workfront pour autoriser ou empêcher la suppression des tâches et problèmes ayant des heures consignées.

Avant cette modification, lorsque vous supprimiez une tâche ou un problème où des heures étaient consignées, les heures étaient supprimées avec la tâche ou le problème, ou elles étaient déplacées vers le projet, selon vos préférences de feuille de temps et d’heures.

Pour plus d’informations sur la suppression de tâches, voir [Supprimer des tâches](../../../../manage-work/tasks/manage-tasks/delete-tasks.md).

Pour plus d’informations sur la suppression de problèmes, voir [Supprimer des problèmes](../../../../manage-work/issues/manage-issues/delete-issues.md).

Pour plus d’informations sur l’activation du paramètre système pour la suppression de tâches et de problèmes, voir [Configurer les préférences des tâches et des problèmes à l’échelle du système](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

## Suppression du paramètre « Accès anticipé » de la zone de configuration {#removal-of-the-early-access-setting-from-the-setup-area}

Nous supprimons le paramètre qui permettait aux administrateurs et administratrices Workfront d’inscrire des personnes pour participer à l’environnement Accès anticipé. Cette fonctionnalité est obsolète depuis la fin de l’année 2016. Nous n’avons pas publié de nouvelles fonctionnalités pour l’accès anticipé en 2017, et toutes les fonctionnalités qui restaient dans cet environnement ont été déplacées vers la production.

Avant ce changement, les administrateurs et administratrices Workfront pouvaient encore ajouter des personnes à l’environnement Accès anticipé, bien qu’il n’y ait pas de nouvelles fonctionnalités accessibles.

## Changement de l’adresse e-mail par défaut de Workfront {#workfront-default-email-address-change}

L’adresse e-mail par défaut pour le courrier sortant de Workfront est passée de [noreply@attask.com](mailto:noreply@attask.com) à [noreply@my.workfront.com](mailto:noreply@workfront.com).

Si vous filtrez actuellement les e-mails envoyés par Workfront, vous devez modifier votre filtre pour refléter la nouvelle adresse par défaut. 

La modification de l’adresse par défaut n’a aucun effet sur les adresses e-mail Workfront configurées. 

Pour plus d’informations, voir :

## Notification in-app pour les objets abonnés {#in-app-notification-for-subscribed-objects}

Lorsqu’une personne fait un commentaire sur les projets, les tâches et les problèmes pour lesquels vous avez un abonnement, vous recevez désormais une notification dans l’application. Pour en savoir plus sur les notifications d’abonnement in-app, voir [Afficher et gérer les notifications in-app](../../../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

Selon les fonctionnalités activées par votre administrateur ou administratrice Workfront, vous pouvez également recevoir des notifications par e-mail pour les éléments abonnés. Vous pouvez facilement vous désabonner d’un élément grâce à un lien sur un e-mail d’abonnement, comme décrit dans [Notifications Adobe Workfront](../../../../workfront-basics/using-notifications/wf-notifications.md).

Avant cette modification, vous receviez toujours une notification par e-mail pour les éléments abonnés et il n’y avait pas d’option pour recevoir une notification in-app.

Vous pouvez désactiver l’envoi d’e-mails d’abonnement, mais vous ne pouvez pas désactiver les notifications in-app pour les éléments abonnés. Pour plus d’informations, voir [Configurer les notifications d’événements pour tous les utilisateurs et utilisatrices du système](../../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

Pour en savoir plus sur l’abonnement aux éléments, voir [S’abonner aux éléments dans Adobe Workfront](../../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md).

## Le tag @ n’est actuellement pas disponible dans l’environnement de prévisualisation. {#tagging-currently-not-available-in-the-preview-environment}

Comme nous travaillons à l’introduction de la fonctionnalité de format de texte enrichi dans le flux de mise à jour, vous ne pourrez temporairement pas utiliser le symbole @ pour taguer d’autres utilisateurs et utilisatrices dans le flux de mise à jour pour les objets suivants dans l’environnement de prévisualisation :

* Projet
* Tâche
* Problème
* Feuille de temps

Vous pouvez encore taguer d’autres personnes en cliquant sur l’icône **Inclure d’autres personnes dans cette mise à jour**.

Pour plus d’informations, voir [Taguer d’autres personnes sur les mises à jour](../../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

## Inclure les informations d’affectation des utilisateurs et utilisatrices dans le rapport d’utilisation d’un projet {#include-user-allocation-information-in-the-utilization-report-on-a-project}

>[!NOTE]
>
>Les outils de planification des ressources ont été retirés de Workfront avec la version 23.1. Pour plus d’informations sur la planification des ressources à l’aide de l’équilibreur de charge de travail, voir [Vue d’ensemble de l’équilibreur de charge de travail](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Le rapport d’utilisation d’un projet tient désormais en compte de la réaffectation éventuelle des heures prévues tout au long de la durée d’une tâche. Lorsque l’affectation des heures aux utilisateurs et utilisatrices a été modifiée (comme décrit dans « Gérer les affectations de personnes dans les zones de planification »), les données du rapport d’utilisation peuvent être affectées si les dates sélectionnées dans le rapport d’utilisation ne contiennent qu’une partie d’une tâche.

Pour plus d’informations, voir [Vue d’ensemble du rapport d’utilisation des ressources](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).
