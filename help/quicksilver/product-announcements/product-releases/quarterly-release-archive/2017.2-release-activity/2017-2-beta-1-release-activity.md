---
content-type: release-notes
navigation-topic: product-releases-archive
title: Activité Version 2017.2, version bêta 1
description: Cette page décrit toutes les modifications disponibles dans l’environnement Aperçu avec la version 2017.2 de Beta 1. Les fonctionnalités de cette page ont été rendues disponibles dans l’environnement Aperçu le 10 mai 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 99812ed3-a300-478e-973f-b957382d934b
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1380'
ht-degree: 0%

---

# Activité Version 2017.2, version bêta 1

Cette page décrit toutes les modifications disponibles dans l’environnement Aperçu avec la version 2017.2 de Beta 1. Les fonctionnalités de cette page ont été rendues disponibles dans l’environnement Aperçu le 10 mai 2017.

>[!IMPORTANT]
>
>Les fonctionnalités décrites sur cette page peuvent être modifiées avant leur disponibilité dans l’environnement de production.

La version 2017.2 de Beta 1 contient des améliorations tant pour les administrateurs de Workfront que pour d’autres utilisateurs :

**Pour les administrateurs :**

* [Restaurer des documents](#restore-documents)
* [Nouvelle bannière d’aperçu avec informations de mise à jour](#new-preview-banner-with-release-information) 
* [Disponibilité de l’API 7](#api-7-availability)

**Pour Tous Les Utilisateurs :**

* [S’abonner aux tâches et aux problèmes](#subscribe-to-tasks-and-issues)
* [Améliorations de la planification des ressources](#resource-scheduling-improvements)
* [Comparer les bons à tirer](#compare-proofs)
* [Nouveau champ pour les groupes de ressources pour les utilisateurs et les projets](#new-field-for-resource-pools-for-users-and-projects)
* [ Représentation mise à jour dans la liste des tableaux de bord ](#updated-look-and-feel-in-the-dashboard-list)
* [Suppression de la fonctionnalité de validations dans Workfront](#removing-the-endorsements-functionality-in-workfront)
* [Réorganiser les colonnes dans n’importe quelle liste par glisser-déplacer (fonctionnalité supprimée)](#reorder-columns-in-any-list-with-drag-and-drop-functionality-is-being-removed)

## Restaurer des documents {#restore-documents}

Les administrateurs de Workfront peuvent désormais restaurer des documents qui ont été supprimés au cours des 30 derniers jours. 

Avant cette modification, les administrateurs de Workfront pouvaient restaurer uniquement les projets, les tâches et les problèmes (y compris les documents qui avaient été supprimés conjointement avec le projet, la tâche ou le problème supprimé).

Pour plus d’informations, voir [Restaurer les éléments supprimés](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

## Nouvelle bannière d’aperçu avec informations de mise à jour {#new-preview-banner-with-release-information}

La bannière bleue située en haut de l’environnement de prévisualisation Sandbox affiche désormais le nom et le numéro de version de l’environnement de prévisualisation. Cliquez sur le nom de la version pour accéder à un article du site d’aide dans lequel vous trouverez plus d’informations sur la version actuelle de l’aperçu. Pour plus d’informations sur l’environnement de test d’aperçu, voir [L’environnement de test d’aperçu Adobe Workfront](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md) 

## Disponibilité de l’API 7 {#api-7-availability}

L’API 7 est désormais disponible et inclut de nouveaux objets et des objets mis à jour.

Pour plus d’informations, voir [Nouveautés de l’API version 7](../../../../wf-api/api/new-api-version-7.md).

## Abonnement aux tâches et aux problèmes {#subscribe-to-tasks-and-issues}

Workfront envoie des notifications sur les éléments auxquels vous êtes affecté ou dont vous êtes propriétaire.

À compter de la version actuelle, si vous souhaitez suivre les éléments qui ne vous sont pas attribués mais qui peuvent avoir un impact sur votre travail, vous pouvez vous y abonner.

Vous pouvez vous abonner à des problèmes et à des tâches pour lesquels vous êtes autorisé à au moins afficher. Lorsqu’un nouveau commentaire est ajouté au problème ou à la tâche auquel vous êtes abonné, vous êtes averti par e-mail de ce commentaire.

Pour plus d’informations sur l’abonnement aux problèmes et aux tâches, voir [Abonnement aux éléments dans Adobe Workfront](../../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md)

## Amélioration de la planification des ressources {#resource-scheduling-improvements}

>[!NOTE]
>
>Les outils de planification des ressources ont été abandonnés et supprimés de Workfront avec la version 23.1. Pour plus d’informations sur la planification des ressources à l’aide de l’équilibreur de charge de travail, voir [Présentation de l’équilibreur de charge de travail](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Les améliorations suivantes sont disponibles lors de la planification des ressources :

* [Afficher plus d’éléments sur la chronologie de planification des ressources dans une vue unique](#view-more-items-on-the-resource-scheduling-timeline-in-a-single-view)
* [Configurez le nom du projet à afficher sur les tâches et les problèmes de la chronologie de planification](#configure-the-project-name-to-display-on-tasks-and-issues-on-the-scheduling-timeline)
* [Configuration de l’affichage des tâches parentes dans la chronologie de planification](#configure-whether-parent-tasks-are-displayed-on-the-scheduling-timeline)
* [ Développer ou réduire plus facilement toutes les tâches et tous les problèmes sur la chronologie de planification ](#more-easily-expand-or-collapse-all-tasks-and-issues-on-the-scheduling-timeline)
* [Les informations sur le rôle et l’utilisateur figurent toujours en haut de la chronologie de planification lors du défilement](#role-and-user-information-remains-at-the-top-of-the-scheduling-timeline-when-scrolling)

### Afficher d’autres éléments sur la chronologie de planification des ressources en une seule vue {#view-more-items-on-the-resource-scheduling-timeline-in-a-single-view}

Lors de la planification de ressources pour une équipe ou pour tout projet pour lequel vous êtes le Gestionnaire de ressources, les tâches et les problèmes consomment désormais moins d’espace vertical dans la chronologie de planification. Vous pouvez ainsi afficher davantage de tâches et de problèmes dans une seule vue.

Si vous décidez d’afficher les noms des projets pour chaque tâche et chaque problème dans la chronologie de planification, l’espace vertical de chaque tâche et problème est développé, ce qui entraîne une diminution du nombre de tâches et de problèmes qui s’affichent dans une seule vue.

Pour plus d’informations sur la planification des ressources, voir  &quot;Prise en main de la planification des ressources&quot;.

### Configuration du nom du projet à afficher sur les tâches et les problèmes de la chronologie de planification {#configure-the-project-name-to-display-on-tasks-and-issues-on-the-scheduling-timeline}

Lors de la planification de ressources pour une équipe ou pour tout projet pour lequel vous êtes le Gestionnaire de ressources, vous pouvez maintenant configurer le nom du projet pour qu’il s’affiche sur chaque tâche et chaque problème dans la chronologie de la planification. Cela permet aux utilisateurs qui visualisent la chronologie de la planification de voir rapidement le nom du projet dans lequel réside la tâche ou le problème.

Pour plus d’informations, voir &quot;Prise en main de la planification des ressources&quot;.

### Configuration de l’affichage des tâches parentes dans la chronologie de planification {#configure-whether-parent-tasks-are-displayed-on-the-scheduling-timeline}

Lors de la planification de ressources pour les projets pour lesquels vous êtes le gestionnaire de ressources, vous pouvez maintenant configurer si les tâches parents s’affichent dans la chronologie de planification lorsque l’option Mode d’achèvement du résumé du projet est définie sur Manuel.

Avant cette modification, les tâches parents s’affichaient toujours dans la chronologie de planification lorsque le mode d’achèvement récapitulatif du projet était défini sur Manuel. 

Lorsque le mode d’achèvement du résumé du projet est défini sur Automatique, les tâches parentes ne peuvent pas être affichées dans la chronologie de la planification. Cette expérience n’a pas changé.

Pour plus d’informations, voir &quot;Prise en main de la planification des ressources&quot;.

### Développer ou réduire plus facilement toutes les tâches et tous les problèmes de la chronologie de planification {#more-easily-expand-or-collapse-all-tasks-and-issues-on-the-scheduling-timeline}

Un nouveau lien permet de réduire plus facilement toutes les tâches et tous les problèmes de la chronologie de planification.

Pour plus d’informations, voir &quot;Prise en main de la planification des ressources&quot;.

### Les informations sur le rôle et l’utilisateur figurent toujours en haut de la chronologie de planification lors du défilement {#role-and-user-information-remains-at-the-top-of-the-scheduling-timeline-when-scrolling}

Désormais, lorsque vous faites défiler la chronologie de la planification pour afficher des informations supplémentaires, le nom du rôle et le nom d’utilisateur restent en haut de la zone Utilisateurs et rôles de la chronologie de la planification, ce qui facilite l’affichage de l’utilisateur et du rôle associés aux tâches et problèmes.

Avant cette modification, le nom du rôle et le nom d’utilisateur défilaient hors de la vue actuelle.

Pour plus d’informations sur la planification des ressources, voir  &quot;Prise en main de la planification des ressources&quot;.

## Comparaison des bons à tirer {#compare-proofs}

Vous pouvez désormais comparer deux bons à tirer de documents dans n’importe quelle liste de documents, par exemple dans l’onglet Documents d’un projet, d’une tâche, d’un problème, d’un portfolio ou dans la zone Documents principale de la barre de navigation globale. 

Les deux bons à tirer s’affichent dans l’outil de vérification et d’approbation. Vous pouvez tester chaque document en le comparant côte à côte.

Pour plus d’informations, voir [Comparaison des bons à tirer](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/compare-proofs.md).

## Nouveau champ pour les groupes de ressources pour les utilisateurs et les projets {#new-field-for-resource-pools-for-users-and-projects}

La version R1.5 introduit de nouvelles fonctionnalités concernant la planification des ressources dans l’environnement Aperçu. Cette fonctionnalité vous permet de créer des groupes de ressources, qui sont des groupes d’utilisateurs.

Vous pouvez désormais associer ces groupes de ressources aux projets, ainsi qu’aux utilisateurs. Un nouveau champ appelé &quot;Pools de ressources&quot; s’affiche désormais sur le projet, ainsi que sur l’objet utilisateur.

Pour plus d’informations sur les nouveaux pools de ressources et la manière dont ils peuvent être associés aux projets et aux utilisateurs, consultez la [présentation des pools de ressources](../../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md)

## Représentation mise à jour de la liste des tableaux de bord {#updated-look-and-feel-in-the-dashboard-list}

Désormais, lorsque vous affichez une liste de tableaux de bord, l’apparence est plus moderne et évolutive.

Cette fonctionnalité était auparavant disponible uniquement pour les utilisateurs inscrits en accès anticipé. Cette option est désormais disponible pour tous les utilisateurs de l’environnement Aperçu . Elle sera mise à la disposition de tous les utilisateurs de l’environnement Production avec la version 2017.2. 

Pour plus d’informations sur les tableaux de bord, voir [Création d’un tableau de bord](../../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## Suppression de la fonctionnalité Validations dans Workfront {#removing-the-endorsements-functionality-in-workfront}

Lors de l’évaluation de la fonctionnalité contenue dans le flux de mise à jour, nous avons identifié les Endorsures comme une fonctionnalité à faible adoption et à faible utilisation. Dans la version 2017.2, les fonctionnalités suivantes relatives aux Endorsements seront supprimées de Workfront à compter de la version 2017.2 (cette fonctionnalité n’est plus disponible dans l’aperçu) :

* l’onglet Validations de la zone de profil utilisateur ;
* L’objet Endorsements sera supprimé de l’explorateur d’API. Si vous extrayez actuellement des rapports d’API pour les objets &quot;Endorsement&quot; ou &quot;Endorsement Share&quot;, les appels seront invalides après la suppression de cet objet.

Les fonctionnalités suivantes continueront à rester dans l’application web :

* L’approbation d’un utilisateur par un autre utilisateur qui a été effectuée avant la suppression de cette fonctionnalité restera dans le flux de mise à jour de l’approbation. 

Les validations n’ont pas été un objet à signaler. Il n’y a donc aucune modification concernant la création de rapports pour cet objet.

## Réorganiser les colonnes dans n’importe quelle liste par glisser-déplacer (fonctionnalité supprimée) {#reorder-columns-in-any-list-with-drag-and-drop-functionality-is-being-removed}

La fonctionnalité de modification de l’ordre des colonnes d’une liste en faisant glisser une colonne d’un emplacement et en la déposant dans un autre emplacement est supprimée des accès anticipés dans l’environnement de production avec la version 2017.2 et ne sera plus disponible pour aucun utilisateur. 

Pour plus d’informations sur cette fonctionnalité, voir [Modification de la largeur et de l’ordre des colonnes](../../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).
