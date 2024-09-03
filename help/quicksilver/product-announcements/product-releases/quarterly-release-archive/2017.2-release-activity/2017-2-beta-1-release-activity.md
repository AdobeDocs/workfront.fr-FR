---
content-type: release-notes
navigation-topic: product-releases-archive
title: Activité Version 2017.2, version bêta 1
description: Cette page décrit toutes les modifications disponibles dans l’environnement de prévisualisation avec la version 2017.2 bêta 1. Les fonctionnalités sur cette page ont été mises à disposition dans l’environnement de prévisualisation le 10 mai 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 99812ed3-a300-478e-973f-b957382d934b
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1380'
ht-degree: 100%

---

# Activité Version 2017.2, version bêta 1

Cette page décrit toutes les modifications disponibles dans l’environnement de prévisualisation avec la version 2017.2 bêta 1. Les fonctionnalités sur cette page ont été mises à disposition dans l’environnement de prévisualisation le 10 mai 2017.

>[!IMPORTANT]
>
>Les fonctionnalités décrites sur cette page peuvent être modifiées avant leur disponibilité dans l’environnement de production.

La version 2017.2 bêta 1 contient des améliorations pour l’équipe d’administration de Workfront et l’ensemble des utilisateurs et des utilisatrices :

**Pour l’équipe d’administration :**

* [Restaurer des documents](#restore-documents)
* [Nouvelle bannière de prévisualisation avec les informations sur la version](#new-preview-banner-with-release-information)
* [Disponibilité de l’API 7](#api-7-availability)

**Pour l’ensemble des utilisateurs et des utilisatrices :**

* [S’abonner aux tâches et aux problèmes](#subscribe-to-tasks-and-issues)
* [Amélioration de la planification des ressources](#resource-scheduling-improvements)
* [Comparer les épreuves](#compare-proofs)
* [Nouveau champ pour les groupes de ressources pour les utilisateurs, les utilisatrices et les projets](#new-field-for-resource-pools-for-users-and-projects)
* [Actualisation de l’aspect et de la convivialité de la liste du tableau de bord](#updated-look-and-feel-in-the-dashboard-list)
* [Suppression de la fonctionnalité « Parrainages » dans Workfront](#removing-the-endorsements-functionality-in-workfront)
* [Réorganiser les colonnes de n’importe quelle liste par glisser-déposer (fonctionnalité en cours de suppression)](#reorder-columns-in-any-list-with-drag-and-drop-functionality-is-being-removed)

## Restaurer des documents {#restore-documents}

L’équipe d’administration de Workfront peut désormais restaurer des documents individuels qui ont été supprimés au cours des 30 derniers jours. 

Avant cette modification, l’équipe d’administration de Workfront ne pouvait restaurer que des projets, des tâches et des problèmes (y compris des documents qui avaient été supprimés en même temps que le projet, la tâche ou le problème supprimé(e)).

Pour plus d’informations, consultez la section [Restaurer des éléments supprimés](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

## Nouvelle bannière de prévisualisation avec des informations sur la version {#new-preview-banner-with-release-information}

La bannière bleue en haut de l’environnement de prévisualisation de sandbox affiche désormais le nom de la version et le numéro de version de l’environnement de prévisualisation. En cliquant sur le nom de la version, vous accédez à un article du site d’aide où vous pouvez trouver plus d’informations sur la version actuelle de la prévisualisation. Pour plus d’informations sur l’environnement de prévisualisation, voir la section [Environnement de prévisualisation d’Adobe Workfront](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md)

## Disponibilité de l’API 7 {#api-7-availability}

L’API 7 est maintenant disponible et comprend des objets nouveaux et mis à jour.

Pour plus d’informations, consutez la section [Nouveautés de la version 7 de l’API](../../../../wf-api/api/new-api-version-7.md).

## S’abonner aux tâches et aux problèmes {#subscribe-to-tasks-and-issues}

Workfront envoie des notifications sur les éléments qui vous sont affectés ou qui vous appartiennent.

À partir de la version actuelle, si vous souhaitez suivre des éléments qui ne vous sont pas affectés mais qui peuvent avoir un impact sur votre travail, vous pouvez vous y abonner.

Vous avez la possibilité de vous abonner aux problèmes et aux tâches que vous avez au moins le droit d’afficher. Lorsqu’un nouveau commentaire est ajouté à un élément (problème ou tâche) pour lequel vous avez un abonnement, un e-mail de notification vous est envoyé.

Pour plus d’informations sur l’abonnement aux problèmes et aux tâches, voir la section [S’abonner à des éléments dans Adobe Workfront](../../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md)

## Améliorations de la planification des ressources {#resource-scheduling-improvements}

>[!NOTE]
>
>Les outils de planification des ressources ont été retirés de Workfront avec la version 23.1. Pour plus d’informations sur la planification des ressources à l’aide de l’équilibreur de charge de travail, voir [Vue d’ensemble de l’équilibreur de charge de travail](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Les améliorations suivantes sont disponibles lors de la planification des ressources :

* [Afficher plus d’éléments sur la chronologie de planification des ressources dans une seule vue](#view-more-items-on-the-resource-scheduling-timeline-in-a-single-view)
* [Configurer le nom du projet à afficher sur les tâches et les problèmes de la chronologie de planification](#configure-the-project-name-to-display-on-tasks-and-issues-on-the-scheduling-timeline)
* [Configurer l’affichage des tâches parent dans la chronologie de planification](#configure-whether-parent-tasks-are-displayed-on-the-scheduling-timeline)
* [Développer ou réduire plus facilement l’ensemble des tâches et des problèmes sur la chronologie de planification](#more-easily-expand-or-collapse-all-tasks-and-issues-on-the-scheduling-timeline)
* [Les informations relatives au rôle et à l’utilisateur ou utilisatrice restent en haut de la chronologie de planification lors du défilement](#role-and-user-information-remains-at-the-top-of-the-scheduling-timeline-when-scrolling)

### Afficher plusieurs éléments de la chronologie de planification des ressources en une seule fois {#view-more-items-on-the-resource-scheduling-timeline-in-a-single-view}

Lorsque vous planifiez des ressources pour une équipe ou pour tout projet dont vous êtes la personne gestionnaire des ressources, les tâches et les problèmes occupent désormais moins d’espace vertical sur la chronologie de planification. Cela vous permet de voir plus de tâches et de problèmes dans une seule vue.

Si vous choisissez d’afficher les noms des projets sur chaque tâche et problème de la chronologie de planification, cela entraîne un élargissement de l’espace vertical de chaque tâche et problème, réduisant ainsi le nombre de tâches et de problèmes affichés dans une seule vue.

Pour plus d’informations sur la planification des ressources, voir « Commencer avec la planification des ressources ».

### Configurer le nom du projet à afficher sur les tâches et les problèmes de la chronologie de planification {#configure-the-project-name-to-display-on-tasks-and-issues-on-the-scheduling-timeline}

Lorsque vous planifiez des ressources pour une équipe ou pour tout projet dont vous êtes la personne gestionnaire de ressources, vous avez maintenant la possibilité de paramétrer le nom du projet à afficher sur chaque tâche et problème de la chronologie de planification.Cela permet aux utilisateurs et aux utilisatrices qui consultent la chronologie de planification de voir rapidement le nom du projet dans lequel se situe la tâche ou le problème.

Pour plus d’informations, voir « Commencer avec la planification des ressources ».

### Configurer l’affichage des tâches parent sur la chronologie de planification {#configure-whether-parent-tasks-are-displayed-on-the-scheduling-timeline}

Lorsque vous planifiez des ressources pour des projets que vous gérez, vous pouvez désormais configurer l’affichage des tâche parents sur la chronologie de planification lorsque l’option Mode d’achèvement du sommaire du projet est définie sur Manuel.

Avant cette modification, les tâches parents s’affichaient toujours sur la chronologie de planification lorsque le mode d’achèvement du sommaire du projet était défini sur Manuel. 

Lorsque le mode d’achèvement du sommaire du projet est défini sur Automatique, les tâches parents ne peuvent pas être affichées sur la chronologie de planification. Cette expérience n’a pas changé.

Pour plus d’informations, voir « Commencer avec la planification des ressources ».

### Développer ou réduire plus facilement toutes les tâches et tous les problèmes sur la chronologie de planification {#more-easily-expand-or-collapse-all-tasks-and-issues-on-the-scheduling-timeline}

Un nouveau lien vous permet de réduire plus facilement toutes les tâches et tous les problèmes sur la chronologie de planification.

Pour plus d’informations, voir « Commencer avec la planification des ressources ».

### Les informations relatives au rôle et à l’utilisateur ou utilisatrice restent en haut de la chronologie de planification lors du défilement {#role-and-user-information-remains-at-the-top-of-the-scheduling-timeline-when-scrolling}

Désormais, lorsque vous faites défiler la chronologie de planification vers le bas pour afficher des informations supplémentaires, le nom du rôle et le nom de la personne restent en haut de la zone Utilisateurs et utilisatrices et Rôles de la chronologie de planification. Cela permet ainsi de voir plus facilement à quelle personne et à quel rôle les tâches et les problèmes sont associés.

Avant cette modification, le nom du rôle et le nom de la personne défilaient hors de la vue actuelle.

Pour plus d’informations sur la planification des ressources, voir « Commencer avec la planification des ressources ».

## Comparer les épreuves {#compare-proofs}

Vous pouvez désormais comparer deux épreuves de documents dans n’importe quelle liste de documents, par exemple dans l’onglet Documents d’un projet, d’une tâche, d’un problème ou d’un portfolio, ou dans la zone principale Documents de la barre de navigation globale. 

Les deux épreuves sont affichées dans l’outil Révision et approbation, et vous pouvez vérifier chaque document tout en les comparant côte à côte.

Pour plus d’informations, voir [Comparer des épreuves](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/compare-proofs.md).

## Nouveau champ pour les groupes de ressources pour les utilisateurs et les utilisatrices ainsi que les projets {#new-field-for-resource-pools-for-users-and-projects}

La version R1.5 a introduit une nouvelle fonctionnalité de planification des ressources dans l’environnement de prévisualisation. Cette fonctionnalité vous permet de créer de nouveaux groupes de ressources, qui sont des collections d’utilisateurs et d’utilisatrices.

Vous pouvez maintenant associer ces groupes de ressources à des projets, ainsi qu’à des utilisateurs et utilisatrices. Vous verrez maintenant un nouveau champ appelé « Groupes de ressources » sur le projet, ainsi que sur l’objet de l’utilisateur ou utilisatrice.

Pour plus d’informations sur les nouveaux groupes de ressources et leur association à des projets et à des personnes, voir [Vue d’ensemble des groupes de ressources](../../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md).

## Aspect mis à jour dans la liste des tableaux de bord {#updated-look-and-feel-in-the-dashboard-list}

Désormais, lorsque vous affichez une liste de tableaux de bord, l’aspect est plus moderne et évolutif.

Cette fonctionnalité n’était auparavant disponible que pour les utilisateurs et utilisatrices inscrits dans l’accès anticipé. Elle est maintenant disponible pour l’ensemble des utilisateurs et utilisatrices dans l’environnement de prévisualisation. Elle sera mise à la disposition de l’ensemble des utilisateurs et utilisatrices dans l’environnement de production avec la version 2017.2. 

Pour plus d’informations sur les tableaux de bord, voir [Créer un tableau de bord](../../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## Suppression de la fonctionnalité des parrainages dans Workfront {#removing-the-endorsements-functionality-in-workfront}

Lors de l’évaluation des fonctionnalités contenues dans le flux de mises à jour, nous avons constaté que les parrainages étaient une fonctionnalité peu adoptée et peu utilisée. Dans la version 2017.2, la fonctionnalité suivante concernant les parrainages sera supprimée de Workfront à partir de la version 2017.2 (cette fonctionnalité n’est plus disponible dans la prévisualisation) :

* L’onglet Parrainages dans la zone du profil de l’utilisateur ou utilisatrice.
* L’objet Parrainages sera supprimé de l’explorateur d&#39;API ; si vous générez actuellement des rapports d’API pour les objets « Parrainage » ou « Partage de parrainage », les appels ne seront plus valides après la suppression de cet objet.

La fonctionnalité suivante continuera d’être proposée dans l’application web :

* Le parrainage d’une personne par une autre effectué avant la suppression de cette fonctionnalité restera dans le flux de mises à jour du parrain ou de la marraine. 

Les parrainages n’étant pas un objet sujet à un rapport, il n’y a pas de changement en ce qui concerne la création de rapport de cet objet.

## Réorganiser les colonnes de n’importe quelle liste par glisser-déposer (fonctionnalité en cours de suppression) {#reorder-columns-in-any-list-with-drag-and-drop-functionality-is-being-removed}

Avec la version 2017.2, la fonctionnalité permettant de modifier l’ordre des colonnes dans une liste en faisant glisser une colonne d’un emplacement à un autre est supprimée de l’accès anticipé dans l’environnement de production et ne sera plus disponible pour les utilisateurs et utilisatrices. 

Pour plus de détails sur cette fonctionnalité, voir [Modifier la largeur et l’ordre des colonnes](../../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).
