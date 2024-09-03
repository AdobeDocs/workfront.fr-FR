---
content-type: release-notes
navigation-topic: product-releases-archive
title: Activité Version 2018.3, version bêta 2
description: Cette page décrit tous les changements les plus récents disponibles dans l’environnement de prévisualisation avec la version bêta 2 de la version 2018.3. La fonctionnalité sera disponible dans l’environnement de prévisualisation le 1er août 2018. Les améliorations apportées à la relecture par la version bêta 2 seront disponibles dans l’environnement de prévisualisation le mercredi 18 juillet. Cela sera disponible dans l’environnement de production en novembre 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 97945661-e97d-43c8-b564-624c4388de2f
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '908'
ht-degree: 100%

---

# Activité Version 2018.3, version bêta 2

Cette page décrit tous les changements les plus récents disponibles dans l’environnement de prévisualisation avec la version bêta 2 de la version 2018.3.La fonctionnalité sera disponible dans l’environnement de prévisualisation le 1er août 2018.Les améliorations apportées à la relecture par la version bêta 2 seront disponibles dans l’environnement de prévisualisation le mercredi 18 juillet. Cela sera disponible dans l’environnement de production en novembre 2018.

>[!NOTE]
>
>Les fonctionnalités décrites sur cette page peuvent être modifiées avant d’être disponibles dans l’environnement de production.

Pour une liste de tous les changements apportés à la version 2018.3, voir [Vue d’ensemble de l’activité de version 2018.3](../../../../product-announcements/product-releases/quarterly-release-archive/2018.3-release-activity/2018-3-release-activity-overview.md).

La version bêta 2 de la version 2018.3 contient des améliorations pour les administrateurs et administratrices de Workfront et les autres utilisateurs et utilisatrices :

**Pour les administrateurs et administratrices**

* [Mettre à jour l’adresse e-mail dans le profil d’utilisateur ou d’utilisatrice en tant qu’administrateur ou administratrice de groupes](#update-the-email-address-in-the-user-profile-as-a-group-administrator)

**Pour tous les utilisateurs et utilisatrices**

* [Voir les approbations qui me sont déléguées dans l’espace personnel](#view-approvals-delegated-to-me-in-the-home-area)
* [Exporter des données pour une période donnée dans le planificateur de ressources](#export-data-for-a-given-period-in-the-resource-planner)
* [Les totaux journaliers s’affichent désormais en rouge lorsque l’utilisateur ou l’utilisatrice a trop d’affectations.](#daily-totals-now-display-in-red-when-the-user-is-overallocated)
* [Les tâches et les problèmes sont masqués sur le journal de planification lorsqu’ils sont réduits.](#tasks-and-issues-are-hidden-on-the-scheduling-timeline-when-minimized)
* [Filtrer les commentaires et les réponses par personne dans la visionneuse de relecture](#filter-comments-and-replies-by-user-in-the-proofing-viewer)
* [Commenter une série d’enregistrements dans une épreuve vidéo](#comment-on-a-range-of-footage-in-a-video-proof)
* [Nouvel outil Polyligne pour le balisage des commentaires dans la visionneuse de relecture](#new-polyline-tool-for-comment-markup-in-the-proofing-viewer)
* [Suppression de Flash pour le partage de rapports, de calendriers et de documents](#flash-removal-for-report-calendar-and-document-sharing)

## Mettre à jour l’adresse e-mail dans le profil d’utilisateur ou d’utilisatrice en tant qu’administrateur ou administratrice de groupes {#update-the-email-address-in-the-user-profile-as-a-group-administrator}

Vous pouvez désormais mettre à jour les adresses e-mail des personnes qui appartiennent à un groupe que vous administrez. 

Auparavant, seuls les administrateurs et administratrices de Workfront pouvaient mettre à jour les adresses e-mail des autres personnes. 

Pour plus d’informations, voir [Équipe d’administration de groupes](../../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

## Voir les approbations qui me sont déléguées dans la zone Accueil {#view-approvals-delegated-to-me-in-the-home-area}

Vous pouvez désormais utiliser la zone Accueil pour afficher les approbations de projet, de tâche et de problème qui vous ont été déléguées.

Avant cette modification, vous ne pouviez consulter les approbations déléguées que dans la zone Mon travail.

Pour plus d’informations, voir [Déléguer des demandes d’approbation](../../../../review-and-approve-work/manage-approvals/delegate-approval-requests.md).

## Exporter des données pour une période donnée dans le planificateur de ressources {#export-data-for-a-given-period-in-the-resource-planner}

Une nouvelle fenêtre s’affiche désormais lors de l’export des informations dans le planificateur de ressources, qui vous permet de sélectionner une période spécifique pour votre fichier exporté.

Avant cette amélioration, vous ne pouviez exporter que les informations affichées à l’écran.

Pour plus d’informations sur l’export de données à partir du planificateur de ressources, voir [Vue d’ensemble de la navigation du planificateur de ressources](../../../../resource-mgmt/resource-planning/resource-planner-navigation.md) dans l’article [Vue d’ensemble de la navigation du planificateur de ressources](../../../../resource-mgmt/resource-planning/resource-planner-navigation.md).

## Les totaux journaliers s’affichent désormais en rouge lorsque l’utilisateur ou l’utilisatrice a trop d’affectations. {#daily-totals-now-display-in-red-when-the-user-is-overallocated}

>[!NOTE]
>
>Les outils de planification des ressources ont été retirés de Workfront avec la version 23.1. Pour plus d’informations sur la planification des ressources à l’aide de l’équilibreur de charge de travail, voir [Vue d’ensemble de l’équilibreur de charge de travail](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Lorsqu’une personne a trop d’affectations, les totaux journaliers pour les jours où la personne a trop d’affectations s’affichent désormais en rouge.Cette option ne s’affiche que lorsque l’option Afficher les totaux des heures planifiées par jour est activée dans les paramètres du journal de planification. Avant cette amélioration, il y avait un indicateur de barre rouge pour les jours où une personne avait trop d’affectations, mais les totaux quotidiens s’affichaient sans surbrillance rouge.

Pour plus d’informations sur les affectations de personnes, voir « Gérer les attributions de personnes dans les zones de planification ».

## Les tâches et les problèmes sont masqués dans le journal de planification lorsqu’ils sont réduits. {#tasks-and-issues-are-hidden-on-the-scheduling-timeline-when-minimized}

Lorsque vous réduisez les tâches et les problèmes sur votre journal de planification, ils sont désormais masqués pour les personnes et les rôles si l’option Afficher les totaux des heures planifiées par jour est activée dans vos paramètres. Les tâches et les problèmes de la zone Non attribué sont affichés dans une vue compressée.

Auparavant, lors de la réduction des tâches et des problèmes, les tâches et les problèmes restaient dans le journal de planification pour les personnes et les rôles, mais s’affichaient dans une vue compressée.

Pour plus d’informations sur la réduction des tâches et des problèmes dans le journal de planification, voir « Commencer avec la planification des ressources ».

## Filtrer les commentaires et les réponses par personne dans la visionneuse de relecture {#filter-comments-and-replies-by-user-in-the-proofing-viewer}

Vous pouvez désormais inclure les réponses lorsque vous filtrez les commentaires créés par les personnes que vous avez spécifiées. Cette option est utile lorsque vous souhaitez vous concentrer sur tous les commentaires créés par une personne approbatrice importante, comme un client ou une cliente ou une personne responsable de la gestion de projet.

Auparavant, le filtrage par utilisateur ou utilisatrice se limitait aux commentaires rédigés (commencés) par les approbateurs et approbatrices que vous aviez spécifiés.

## Faire un commentaire sur une plage d’enregistrements dans une épreuve vidéo {#comment-on-a-range-of-footage-in-a-video-proof}

Vous pouvez créer un commentaire pour une plage d’enregistrements dans une épreuve vidéo. Cette fonction est utile, par exemple, lorsque vous devez indiquer qu’une séquence d’enregistrement doit être tournée à nouveau ou supprimée.

Auparavant, vous ne pouviez créer un commentaire que pour un seul point d’une chronologie vidéo.

## Nouvel outil Polyligne pour le balisage des commentaires dans la visionneuse de relecture {#new-polyline-tool-for-comment-markup-in-the-proofing-viewer}

Vous pouvez désormais utiliser le balisage Polyligne pour dessiner des lignes et des formes segmentées lorsque vous ajoutez un commentaire à une épreuve. Vous pouvez créer une ligne segmentée ouverte ou une forme fermée. Cet outil est particulièrement utile pour travailler sur des images complexes, telles que des images techniques ou architecturales.

Auparavant, lorsque vous marquiez une épreuve pour y ajouter un commentaire, vous pouviez dessiner un rectangle, une ligne droite, une ligne ou forme à main levée ou une flèche.

## Suppression de Flash pour le partage de rapports, de calendriers et de documents {#flash-removal-for-report-calendar-and-document-sharing}

Nous avons supprimé Flash des boîtes de dialogue de partage suivantes dans Workfront :

* Rapports
* Calendriers
* Documents

Vous pouvez toujours partager ces objets comme vous le faisiez auparavant, mais l’expérience ne repose plus sur Flash.
