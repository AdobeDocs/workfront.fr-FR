---
content-type: release-notes
navigation-topic: product-releases-archive
title: Activité Version 2018.3, version bêta 2
description: Cette page décrit toutes les modifications les plus récentes disponibles dans l’environnement Aperçu avec la version 2018.3 de Beta 2. Cette fonctionnalité sera disponible dans l’environnement Aperçu le 1er août 2018. Les améliorations de la vérification avec Beta 2 seront disponibles dans l’environnement Aperçu le mercredi 18 juillet. Il sera disponible dans l’environnement de production en novembre 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 97945661-e97d-43c8-b564-624c4388de2f
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '908'
ht-degree: 1%

---

# Activité Version 2018.3, version bêta 2

Cette page décrit toutes les modifications les plus récentes disponibles dans l’environnement Aperçu avec la version 2018.3 de Beta 2. Cette fonctionnalité sera disponible dans l’environnement Aperçu le 1er août 2018. Les améliorations de la vérification avec Beta 2 seront disponibles dans l’environnement Aperçu le mercredi 18 juillet. Il sera disponible dans l’environnement de production en novembre 2018.

>[!NOTE]
>
> Les fonctionnalités décrites sur cette page peuvent être modifiées avant leur disponibilité dans l’environnement de production.

Pour obtenir la liste de toutes les modifications apportées à la version 2018.3, voir  [Présentation de l’activité de version 2018.3](../../../../product-announcements/product-releases/quarterly-release-archive/2018.3-release-activity/2018-3-release-activity-overview.md).

La version 2018.3 de Beta 2 contient des améliorations tant pour les administrateurs de Workfront que pour d’autres utilisateurs :

**Pour les administrateurs**

* [Mettre à jour l’adresse électronique dans le profil utilisateur en tant qu’administrateur de groupe](#update-the-email-address-in-the-user-profile-as-a-group-administrator)

**Pour Tous Les Utilisateurs**

* [Afficher les approbations déléguées à moi dans la zone d’accueil](#view-approvals-delegated-to-me-in-the-home-area)
* [Exporter des données pour une période donnée dans le planificateur de ressources](#export-data-for-a-given-period-in-the-resource-planner)
* [Les totaux quotidiens s’affichent maintenant en rouge lorsque l’utilisateur est suralloué](#daily-totals-now-display-in-red-when-the-user-is-overallocated)
* [Les tâches et les problèmes sont masqués dans la chronologie de planification lorsqu’ils sont minimisés](#tasks-and-issues-are-hidden-on-the-scheduling-timeline-when-minimized)
* [Filtrage des commentaires et réponses par utilisateur dans la visionneuse de vérification](#filter-comments-and-replies-by-user-in-the-proofing-viewer)
* [Commentaire sur une plage de vidéos dans un bon à tirer vidéo](#comment-on-a-range-of-footage-in-a-video-proof)
* [Nouvel outil polyligne pour le balisage des commentaires dans la visionneuse de vérification](#new-polyline-tool-for-comment-markup-in-the-proofing-viewer)
* [Suppression de Flashs pour le partage de rapports, de calendriers et de documents](#flash-removal-for-report-calendar-and-document-sharing)

## Mettre à jour l’adresse électronique dans le profil utilisateur en tant qu’administrateur de groupe {#update-the-email-address-in-the-user-profile-as-a-group-administrator}

Vous pouvez désormais mettre à jour les adresses électroniques des utilisateurs appartenant à un groupe que vous administrez. 

Auparavant, seuls les administrateurs Workfront pouvaient mettre à jour les adresses électroniques des autres utilisateurs. 

Pour plus d’informations, voir [Administrateurs de groupe](../../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

## Afficher les approbations qui m’ont été déléguées dans la zone d’accueil {#view-approvals-delegated-to-me-in-the-home-area}

Vous pouvez désormais utiliser la zone d’accueil pour afficher les approbations de projet, de tâche et d’émission qui vous ont été déléguées.

Avant cette modification, vous ne pouviez afficher les validations déléguées que dans la zone Mon travail.

Pour plus d’informations, voir [Déléguer la demande d’approbation](../../../../review-and-approve-work/manage-approvals/delegate-approval-requests.md).

## Exporter des données pour une période donnée dans le planificateur de ressources {#export-data-for-a-given-period-in-the-resource-planner}

Une nouvelle fenêtre s’affiche maintenant lors de l’export des informations dans le planificateur de ressources, qui vous permet de sélectionner une période spécifique pour votre fichier exporté.

Avant cette amélioration, vous ne pouviez exporter que les informations affichées à l’écran.

Pour plus d’informations sur l’exportation de données à partir du planificateur de ressources, consultez la [présentation de la navigation du planificateur de ressources](../../../../resource-mgmt/resource-planning/resource-planner-navigation.md) dans l’article [ ](../../../../resource-mgmt/resource-planning/resource-planner-navigation.md).

## Les totaux quotidiens s’affichent maintenant en rouge lorsque l’utilisateur est suralloué. {#daily-totals-now-display-in-red-when-the-user-is-overallocated}

>[!NOTE]
>
>Les outils de planification des ressources ont été abandonnés et supprimés de Workfront avec la version 23.1. Pour plus d’informations sur la planification des ressources à l’aide de l’équilibreur de charge de travail, voir [Présentation de l’équilibreur de charge de travail](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Lorsqu’un utilisateur est surchargé, les totaux quotidiens des jours où l’utilisateur est surchargé s’affichent désormais en rouge. Cette option s’affiche uniquement lorsque l’option Afficher les totaux pour les heures planifiées quotidiennes est activée dans les paramètres de planification de la chronologie. Avant cette amélioration, un indicateur de barre rouge était affiché pour les jours où l’utilisateur était surchargé, mais les totaux quotidiens s’affichaient sans surbrillance rouge.

Pour plus d’informations sur les affectations d’utilisateurs, voir &quot;Gestion des affectations d’utilisateurs dans les zones de planification&quot;.

## Les tâches et les problèmes sont masqués dans la chronologie de planification lorsque celle-ci est réduite {#tasks-and-issues-are-hidden-on-the-scheduling-timeline-when-minimized}

Lorsque vous réduisez les tâches et les problèmes de votre chronologie de planification, ils sont désormais masqués pour les utilisateurs et les rôles si l’option Afficher les totaux des heures planifiées quotidiennes est activée dans vos paramètres. Les tâches et les problèmes de la zone Non affecté s’affichent dans une vue compressée.

Auparavant, lors de la réduction des tâches et des problèmes, les tâches et les problèmes restaient dans la chronologie de planification des utilisateurs et des rôles, mais s’affichaient dans une vue compressée.

Pour plus d’informations sur la réduction des tâches et des problèmes dans la chronologie de planification, voir  &quot;Prise en main de la planification des ressources&quot;.

## Filtrage des commentaires et réponses par utilisateur dans la visionneuse de vérification {#filter-comments-and-replies-by-user-in-the-proofing-viewer}

Vous pouvez désormais inclure des réponses lorsque vous filtrez les commentaires effectués par les utilisateurs que vous spécifiez. Cela s’avère utile lorsque vous souhaitez vous concentrer sur tous les commentaires effectués par un réviseur important, comme un client ou un chef de projet.

Auparavant, le filtrage par utilisateur était limité aux commentaires créés (démarrés) par les opérateurs validants que vous spécifiez.

## Commentaire sur une plage de images dans un bon à tirer vidéo {#comment-on-a-range-of-footage-in-a-video-proof}

Vous pouvez créer un commentaire pour une série de séquences dans un BAT vidéo. Cela s’avère utile, par exemple, lorsque vous devez indiquer qu’un segment de séquence doit être enregistré à nouveau ou supprimé.

Auparavant, vous ne pouviez créer un commentaire que pour un seul point de la chronologie d’une vidéo.

## Nouvel outil polyligne pour le balisage des commentaires dans la visionneuse de vérification {#new-polyline-tool-for-comment-markup-in-the-proofing-viewer}

Vous pouvez désormais utiliser des annotations polylignes pour tracer des lignes et des formes segmentées lorsque vous ajoutez un commentaire à un BAT. Vous pouvez créer une ligne segmentée ouverte ou une forme fermée. Cet outil est particulièrement utile lorsque vous utilisez des images complexes, telles que des images techniques ou architecturales.

Auparavant, lors de la mise en forme d’un BAT pour ajouter un commentaire, vous pouviez tracer un rectangle, une ligne droite, une ligne à main levée ou une flèche.

## Suppression de Flashs pour le partage de rapports, de calendriers et de documents {#flash-removal-for-report-calendar-and-document-sharing}

Nous avons supprimé le Flash des boîtes de dialogue de partage suivantes dans Workfront :

* Rapports
* Calendriers
* Documents

Vous pouvez toujours partager ces objets comme vous le faisiez auparavant, mais l’expérience ne dépend plus du Flash.
