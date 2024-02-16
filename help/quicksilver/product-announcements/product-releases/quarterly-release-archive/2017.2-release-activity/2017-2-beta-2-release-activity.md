---
content-type: release-notes
navigation-topic: product-releases-archive
title: Activité de version 2017.2 bêta 2
description: Cette page décrit toutes les modifications disponibles dans l’environnement Aperçu avec la version 2017.2 bêta 2. Les fonctionnalités de cette page ont été rendues disponibles dans l’environnement Aperçu le 24 mai 2017. Il sera disponible dans l’environnement de production entre fin juillet et début août 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 0aa8d61e-cf8c-46a7-b093-a0dbc90d37fd
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '792'
ht-degree: 0%

---

# Activité de version 2017.2 bêta 2

Cette page décrit toutes les modifications disponibles dans l’environnement Aperçu avec la version 2017.2 bêta 2. Les fonctionnalités de cette page ont été rendues disponibles dans l’environnement Aperçu le 24 mai 2017. Il sera disponible dans l’environnement de production entre fin juillet et début août 2017.

>[!IMPORTANT]
>
>Les fonctionnalités décrites sur cette page peuvent être modifiées avant leur disponibilité dans l’environnement de production.

Pour obtenir la liste de toutes les modifications apportées à la version 2017.2, voir [Présentation de l’activité de la version 2017.2](../../../../product-announcements/product-releases/quarterly-release-archive/2017.2-release-activity/2017-2-release-activity-overview.md).

La version 2017.2 bêta 2 contient des améliorations à la fois pour les administrateurs de Workfront et pour les autres utilisateurs :

**Pour les administrateurs :**

* [Amélioration de l’API : abonnements aux événements](#api-enhancement-event-subscriptions)

**Pour tous les utilisateurs :**

* [Abonnement à des projets](#subscribe-to-projects)
* [Se désabonner des éléments du courrier électronique](#unsubscribe-from-items-from-email)
* [Configuration de l’affichage des jalons sur le diagramme de Gantt](#configure-how-milestones-are-displayed-on-the-gantt-chart)
* [Modèles de groupes de ressources](#resource-pools-templates)
* [Affichage des versions des documents protégés dans Workfront](#view-versions-of-proofed-documents-within-workfront)
* [Nouvel objet Requester dans le rapport d’approbation de BAT](#new-requester-object-in-proof-approval-report)

## Amélioration de l’API : abonnements aux événements {#api-enhancement-event-subscriptions}

Lorsqu’une action se produit sur un objet Workfront pris en charge par les abonnements aux événements, vous pouvez maintenant configurer Workfront pour envoyer une réponse au point de terminaison souhaité. Cela signifie que vos intégrations peuvent interagir avec l’API Workfront en temps réel.

Pour plus d’informations, voir [API d’abonnement à un événement](../../../../wf-api/general/event-subs-api.md). 

## Abonnement à des projets {#subscribe-to-projects}

Vous pouvez désormais vous abonner à de nouveaux commentaires sur les projets pour lesquels vous ne faites pas partie de l’équipe de projet. Avant cette version, vous ne pouviez vous abonner qu’aux commentaires sur les problèmes et les tâches.

Pour plus d’informations sur l’abonnement aux éléments, voir [Abonnement aux éléments dans Adobe Workfront](../../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md)

## Se désabonner des éléments du courrier électronique {#unsubscribe-from-items-from-email}

Vous pouvez vous désabonner des éléments à l’aide du lien &quot;Se désabonner&quot; dans l’email d’abonnement. Auparavant, vous ne pouviez vous désabonner que d’un élément de l’interface de Workfront.

Pour plus d’informations sur la désinscription aux e-mails d’abonnement, voir la section &quot;Désinscription de la notification par e-mail&quot; dans [Notifications Adobe Workfront](../../../../workfront-basics/using-notifications/wf-notifications.md) 

## Configuration de l’affichage des jalons sur le diagramme de Gantt {#configure-how-milestones-are-displayed-on-the-gantt-chart}

***CORRECTION **: cette fonctionnalité n’est actuellement pas dans l’environnement de prévisualisation Sandbox. Il devrait être publié à une date ultérieure, au cours du mois de juin 2017.*

Deux options sont désormais disponibles pour afficher les informations de jalon dans un graphique Gantt. Vous pouvez configurer l’un des indicateurs de jalon suivants, ou les deux :

* Diamants de jalon (icône)

  Cette icône s’affiche dans le diagramme de Gantt après toute tâche associée à un jalon.

* Lignes de jalons

  Une ligne s’affiche après toute tâche associée au jalon, dans toutes les tâches du graphique Gantt.

Avant cette modification, il n’existait qu’une seule option permettant aux jalons de s’afficher sur un graphique de Gantt, appelé &quot;Jalons&quot;. Cette option a activé l’icône représentant un jalon et la ligne de jalon. Ces indicateurs n’ont pas pu être séparés. Les deux options sont désormais disponibles sur tous les graphiques Gantt, y compris toutes les listes de projets et tous les rapports. 

Pour plus d’informations sur la configuration de l’affichage des informations dans le diagramme de Gantt, voir [Configuration de l’affichage des informations sur le diagramme de Gantt](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

## Modèles de groupes de ressources {#resource-pools-templates}

Vous pouvez désormais spécifier des groupes de ressources pour les modèles. Avant cette version, vous ne pouviez associer les groupes de ressources qu’aux utilisateurs et aux projets.

Pour plus d’informations sur les pools de ressources, voir [Présentation des pools de ressources](../../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md)

## Affichage des versions des documents protégés dans Workfront {#view-versions-of-proofed-documents-within-workfront}

Vous pouvez désormais afficher les bons à tirer de toutes les versions d’un document à tirer dans l’interface de Workfront. 

Avant cette modification, vous ne pouviez afficher que la dernière version du document testé.

Les utilisateurs sans licence de vérification peuvent :

* Ouvrir un BAT sur une version précédente d’un document révisé

Les utilisateurs disposant d’une licence de vérification peuvent effectuer l’une des opérations suivantes :

* Ouvrir un BAT sur une version précédente d’un document révisé
* Afficher les détails du BAT sur une version précédente d’un document révisé

Pour plus d’informations, voir [Gestion des versions de document](../../../../documents/managing-documents/manage-document-versions.md) in [Gestion des versions de document](../../../../documents/managing-documents/manage-document-versions.md).

## Nouvel objet Requester dans le rapport d’approbation de BAT {#new-requester-object-in-proof-approval-report}

Désormais, lors de la création d’un rapport d’approbation de BAT, un nouvel objet Requester (Demander l’approbation) est disponible. Cet objet vous permet de générer des rapports sur les informations concernant l’utilisateur qui a demandé l’approbation du BAT. 

Le nouvel objet Requester du rapport Approbation de BAT contient tous les champs disponibles avec l’objet User existant dans d’autres types de rapports d’objet.

>[!NOTE]
>
> Ces informations ne sont disponibles dans le rapport qu’à partir du moment où cette fonctionnalité a été introduite pour la première fois dans les environnements de prévisualisation ou de production respectifs ; les informations contenues dans les rapports concernant l’objet Requester avant l’introduction de cette fonctionnalité ne sont pas disponibles.

Vous accédez à l’objet Requester lors de la création d’un rapport d’approbation de BAT, comme décrit dans la section [Création d’un rapport personnalisé](../../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Pour plus d’informations sur le rapport d’objet Approbations de BAT, voir [Présentation des objets dans Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) dans [Présentation des objets dans Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).
