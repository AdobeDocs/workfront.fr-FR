---
content-type: release-notes
navigation-topic: product-releases-archive
title: Activité Version 2017.2 bêta 2
description: Cette page décrit tous les changements disponibles dans l’environnement de prévisualisation avec la version 2017.2 bêta 2. Les fonctionnalités de cette page ont été mises à disposition dans l’environnement de prévisualisation le 24 mai 2017. Elles seront disponibles dans l’environnement de production entre fin juillet et début août 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 0aa8d61e-cf8c-46a7-b093-a0dbc90d37fd
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '792'
ht-degree: 100%

---

# Activité Version 2017.2 bêta 2

Cette page décrit tous les changements disponibles dans l’environnement de prévisualisation avec la version 2017.2 bêta 2. Les fonctionnalités de cette page ont été mises à disposition dans l’environnement de prévisualisation le 24 mai 2017. Elles seront disponibles dans l’environnement de production entre fin juillet et début août 2017.

>[!IMPORTANT]
>
>Les fonctionnalités décrites sur cette page peuvent être modifiées avant leur disponibilité dans l’environnement de production.

Pour une liste de tous les changements apportés avec la version 2017.2, voir [Vue d’ensemble de l’activité de la version 2017.2](../../../../product-announcements/product-releases/quarterly-release-archive/2017.2-release-activity/2017-2-release-activity-overview.md).

La version 2017.2 bêta 2 contient des améliorations pour les équipes d’administration de Workfront et les autres utilisateurs et utilisatrices :

**Pour les administrateurs et administratrices :**

* [Amélioration de l’API : abonnements aux événements](#api-enhancement-event-subscriptions)

**Pour tous les utilisateurs et utilisatrices :**

* [S’abonner aux projets](#subscribe-to-projects)
* [Se désabonner d’éléments à partir d’un e-mail](#unsubscribe-from-items-from-email)
* [Configurer l’affichage des jalons sur le graphique de Gantt](#configure-how-milestones-are-displayed-on-the-gantt-chart)
* [Modèles de groupes de ressources](#resource-pools-templates)
* [Afficher les versions des documents relus dans Workfront](#view-versions-of-proofed-documents-within-workfront)
* [Nouvel objet Demande dans le rapport d’approbation des épreuves](#new-requester-object-in-proof-approval-report)

## Amélioration de l’API : abonnements aux événements {#api-enhancement-event-subscriptions}

Désormais, lorsqu’une action se produit sur un objet Workfront qui est pris en charge par les abonnements aux événements, vous pouvez configurer Workfront pour qu’il envoie une réponse au point d’entrée de votre choix. Cela signifie que vos intégrations peuvent interagir avec l’API Workfront en temps réel.

Pour plus d’informations, voir [API d’abonnement aux événements](../../../../wf-api/general/event-subs-api.md).

## S’abonner aux projets {#subscribe-to-projects}

Vous pouvez désormais vous abonner aux nouveaux commentaires sur les projets pour lesquels vous ne faites pas partie de l’équipe. Avant cette version, vous ne pouviez vous abonner qu’aux commentaires sur les problèmes et les tâches.

Pour plus d’informations sur l’abonnement aux éléments, voir [S’abonner à des éléments dans Adobe Workfront](../../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md)

## Se désabonner d’éléments à partir d’un e-mail {#unsubscribe-from-items-from-email}

Vous pouvez vous désabonner d’éléments en utilisant le lien « Se désabonner » dans l’e-mail d’abonnement. Auparavant, vous ne pouviez vous désabonner d’un élément qu’à partir de l’interface Workfront.

Pour plus d’informations sur la désinscription à partir des e-mails d’abonnement, voir la section « Désactiver les notifications par e-mail » dans [Notifications Adobe Workfront](../../../../workfront-basics/using-notifications/wf-notifications.md)

## Configurer l’affichage des jalons sur le graphique de Gantt {#configure-how-milestones-are-displayed-on-the-gantt-chart}

***CORRECTION ** : cette fonctionnalité n’est pas encore disponible dans l’environnement sandbox de prévisualisation. Sa sortie est prévue à une date ultérieure, au cours du mois de juin 2017.*

Il existe désormais deux options pour afficher les informations sur les jalons dans un graphique de Gantt. Vous pouvez configurer l’un des indicateurs de jalon suivants, ou les deux :

* Losanges de jalons (icône)

  Cette icône s’affiche dans le graphique de Gantt après toute tâche associée à un jalon.

* Lignes de jalons

  Une ligne s’affiche après chaque tâche associée au jalon, sur l’ensemble des tâches du graphique de Gantt.

Avant cette modification, il n’existait qu’une seule option pour permettre l’affichage des jalons dans un graphique de Gantt, appelée « Jalons ». Cette option permet d’activer à la fois l’icône de losange de jalon et la ligne de jalon. Ces indicateurs ne pouvaient pas être séparés. Les deux options sont désormais disponibles sur tous les graphiques de Gantt, y compris les listes de projets et les rapports. 

Pour plus d’informations sur la configuration de l’affichage des informations dans le graphique de Gantt, voir [Configurer l’affichage des informations sur le graphique de Gantt](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

## Modèles de groupes de ressources {#resource-pools-templates}

Vous pouvez désormais spécifier des groupes de ressources comme modèles. Avant cette version, vous ne pouviez associer les groupes de ressources qu’aux utilisateurs et utilisatrices et aux projets.

Pour plus d’informations sur les groupes de ressources, voir [Vue d’ensemble des groupes de ressources](../../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md).

## Afficher les versions des documents relus dans Workfront {#view-versions-of-proofed-documents-within-workfront}

Vous pouvez désormais afficher les épreuves de toutes les versions d’un document relu dans l’interface Workfront. 

Avant cette modification, vous ne pouviez afficher que la dernière version du document relu.

Les utilisateurs et utilisatrices ne disposant pas d’une licence de relecture peuvent effectuer les opérations suivantes :

* Ouvrir une épreuve sur une version précédente d’un document relu.

Les utilisateurs et utilisatrices disposant d’une licence de relecture peuvent effectuer les opérations suivantes :

* Ouvrir une épreuve sur une version précédente d’un document relu.
* Afficher les détails de l’épreuve d’une version précédente d’un document relu.

Pour plus d’informations, voir [Gérer les versions des documents](../../../../documents/managing-documents/manage-document-versions.md) dans [Gérer les versions des documents](../../../../documents/managing-documents/manage-document-versions.md).

## Nouvel objet Demande dans le rapport d’approbation des épreuves {#new-requester-object-in-proof-approval-report}

Désormais, lors de la création d’un rapport d’approbation d’épreuve, un nouvel objet Demande est créé. Cet objet vous permet d’établir un rapport sur les informations relatives à l’utilisateur ou à l’utilisatrice qui a demandé l’approbation de l’épreuve. 

Le nouvel objet Demande du rapport d’approbation d’épreuve contient tous les champs disponibles avec l’objet Utilisateur ou utilisatrice existant dans d’autres types de rapports d’objets.

>[!NOTE]
>
>Ces informations ne sont disponibles dans le rapport qu’à partir du moment où cette fonctionnalité a été introduite pour la première fois dans les environnements de prévisualisation ou de production respectifs ; les informations contenues dans les rapports concernant l’objet Demande avant l’introduction de cette fonctionnalité ne sont pas disponibles.

Vous accédez à l’objet Demande lors de la création d’un rapport d’approbation d’épreuve, comme décrit dans [Créer un rapport personnalisé](../../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Pour plus d’informations sur le rapport d’objets d’approbation d’épreuve, voir la section [Comprendre les objets dans Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) dans [Comprendre les objets dans Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).
