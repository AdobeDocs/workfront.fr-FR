---
content-type: release-notes
navigation-topic: product-releases-archive
title: Activité Version 2018.2, version bêta 2
description: Cette page décrit tous les changements les plus récents disponibles dans l’environnement de prévisualisation avec la version bêta 2 de la version 2018.2. Cette fonctionnalité a été mise à disposition dans l’environnement de prévisualisation le 5 avril 2018. Elle a été rendue disponible dans l’environnement de production en juin 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: c8ef68f5-53db-4c3c-af0f-e1c98521ec27
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '901'
ht-degree: 100%

---

# Activité Version 2018.2, version bêta 2

Cette page décrit tous les changements les plus récents disponibles dans l’environnement de prévisualisation avec la version bêta 2 de la version 2018.2.Cette fonctionnalité a été mise à disposition dans l’environnement de prévisualisation le 5 avril 2018. Elle sera disponible dans l’environnement de production en juin 2018.

>[!IMPORTANT]
>
>Les fonctionnalités décrites sur cette page peuvent être modifiées avant d’être disponibles dans l’environnement de production.

Pour obtenir la liste de toutes les modifications apportées à la version 2018.2, voir [Vue d’ensemble de l’activité Version 2018.2](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-release-activity-overview.md).

La version 2018.2, version bêta 2 contient les améliorations suivantes :

* [Modifier directement les champs à partir de la zone d’accueil](#edit-fields-directly-from-the-home-area)
* [Consigner du temps en heures](#log-time-in-days)
* [Afficher les relations entre les prédicateurs de projets sur le graphique de Gantt dans une liste de projets](#view-cross-project-predecessor-relationships-on-the-gantt-chart-in-a-list-of-projects)
* [Utiliser le coût budgété dans l’Optimisateur de portfolio pour calculer les finances des Portfolios](#use-budgeted-cost-in-the-portfolio-optimizer-to-calculate-portfolio-finances)
* [Rapport d’utilisation : renseigne les heures budgétées dans la nouvelle zone Budget de ressources](#utilization-report-populates-budgeted-hours-from-new-resource-budgeting-area) (environnement de prévisualisation seulement)

* [Rapport d’utilisation : affichage des heures budgétées par utilisateur ou utilisatrice sur un projet](#utilization-report-view-budgeted-hours-by-user-on-a-project) (environnement de prévisualisation seulement)

* [Progression de la relecture depuis la liste de documents disponible pour les personnes non-réviseuses](#proof-progress-from-the-document-list-available-to-non-proofing-users)
* [Améliorations apportées à l’application mobile](#mobile-improvements)

## Modification des champs directement à partir de la zone d’accueil {#edit-fields-directly-from-the-home-area}

Maintenant, lorsque vous sélectionnez un objet dans la zone d’accueil, vous pouvez modifier les champs qui lui sont associés directement à partir du panneau de droite de la zone d’accueil. 

Avant cette modification, les informations ne pouvaient être affichées que dans la zone d’accueil et ne pouvaient pas être modifiées.

Pour plus d’informations, voir [Mettre à jour ou modifier un élément de travail dans la zone d’accueil](../../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md) dans l’article [Mettre à jour ou modifier un élément de travail dans la zone d’accueil](../../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md).

## Temps de connexion en jours {#log-time-in-days}

Les administrateurs et administratrices de Workfront peuvent désormais choisir si les personnes de leur entreprise doivent consigner le temps en jours ou en heures. Les personnes disposant d’une licence de planification peuvent configurer ce paramètre pour elles-mêmes.

Avant cette modification, les personnes ne pouvaient consigner le temps qu’en heures.

Vous pouvez configurer ce paramètre en modifiant le profil d’utilisation. Pour plus d’informations, voir [Configurer la consignation du temps en heures ou en jours](../../../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md).

Pour plus d’informations sur la façon dont les personnes peuvent consigner du temps après la mise à jour de ce paramètre, voir [Consigner du temps](../../../../timesheets/create-and-manage-timesheets/log-time.md).

## Afficher les relations entre les prédécesseurs de projets sur le graphique de Gantt dans une liste de projets {#view-cross-project-predecessor-relationships-on-the-gantt-chart-in-a-list-of-projects}

Vous pouvez désormais afficher les relations entre les prédécesseurs de projets sur le graphique de Gantt dans les listes de projets suivantes :

* Onglet Projets dans un portfolio ou un programme
* Dans un rapport de projet

Avant cette modification, vous ne pouviez afficher les relations entre les prédécesseurs de plusieurs projets que pour les tâches individuelles au niveau du projet.

Pour plus d’informations, voir [Configurer l’affichage des informations sur le graphique de Gantt ](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

## Utiliser le coût budgété dans l’Optimiseur de portfolio pour calculer les finances du portfolio {#use-budgeted-cost-in-the-portfolio-optimizer-to-calculate-portfolio-finances}

Le nouvel Optimisateur de portfolio utilise désormais le coût budgété de la nouvelle zone Budget de ressources de l’analyse de rentabilité ou du planificateur de ressources pour calculer les champs suivants :

* Valeur nette
* Retour sur investissement (ROI)
* Coûts

Auparavant, le nouvel Optimisateur de portfolio et l’ancien utilisaient tous deux le coût budgété hérité. L’Optimisateur de portfolio hérité continue d’utiliser l’option Coût budgété hérité pour calculer la valeur nette, le retour sur investissement et le coût.

Nous avons également ajouté deux nouveaux champs aux champs financiers du Portfolio : Ancien retour sur investissement et Ancienne valeur nette pour capturer les nouvelles valeurs à partir des nouveaux outils de gestion des ressources.

Pour plus d’informations, voir [Vue d’ensemble de l’optimisateur de portfolio](../../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md) dans l’article  [Vue d’ensemble de l’optimisateur de portfolio](../../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

## Rapport d’utilisation : renseigner les heures budgétées à partir de la zone de nouvelle ressource du budget des ressources {#utilization-report-populates-budgeted-hours-from-new-resource-budgeting-area}

>[!NOTE]
>
>Cette fonctionnalité ne sera pas incluse dans la version officielle de l’environnement de prévisualisation avec la version 2018.2. Elle sera réintroduite pendant la période bêta de la version 2018.3 et sera publiée dans l’environnement de production avec la version 2018.3. 

Les heures budgétées du rapport d’utilisation sont désormais renseignées à partir des informations disponibles dans la zone de nouvelle ressource du budget des ressources du business case.

Avant cette modification, les informations de la zone des anciennes estimations de ressources étaient utilisées.

Pour plus d’informations, consultez la section [Vue d’ensemble du rapport d’utilisation des ressources](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) dans l’article [Vue d’ensemble du rapport d’utilisation des ressources](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Rapport d’utilisation : afficher les heures budgétées par utilisateur ou par utilisatrice dans un projet {#utilization-report-view-budgeted-hours-by-user-on-a-project}

>[!NOTE]
>
>Cette fonctionnalité ne sera pas incluse dans la version officielle de l’environnement de prévisualisation avec la version 2018.2. Elle sera réintroduite pendant la période bêta de la version 2018.3 et sera publiée dans l’environnement de production avec la version 2018.3. 

Le rapport d’utilisation d’un projet affiche désormais les heures budgétées par utilisateur ou par utilisatrice.

Avant cette modification, le rapport d’utilisation affichait les heures budgétées uniquement par fonction. 

Pour plus d’informations, consultez la section [Vue d’ensemble du rapport d’utilisation des ressources](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) dans l’article [Vue d’ensemble du rapport d’utilisation des ressources](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Progression de la relecture à partir de la liste des documents disponibles pour les utilisateurs et les utilisatrices n’effectuant pas de relecture {#proof-progress-from-the-document-list-available-to-non-proofing-users}

Les indicateurs de progression de la relecture (Envoyé, Ouvert, Commentaires effectués et Décision) s’affichent désormais pour tous les utilisateurs et toutes les utilisatrices qui consultent la liste de documents. Cela inclut les utilisateurs et les utilisatrices qui ne sont pas en mesure de générer des épreuves (pour plus d’informations sur comment autoriser les utilisateurs et les utilisatrices à générer des épreuves, consultez la section .

Avant cette modification, les indicateurs de progression de la relecture n’étaient disponibles que pour les utilisateurs et les utilisatrices qui pouvaient générer des épreuves.

Pour plus d’informations, consultez la section [Vue d’ensemble du statut et de la progression de la relecture](../../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md).

## Améliorations apportées à l’application mobile {#mobile-improvements}

L’application mobile contient les améliorations suivantes :

* Les liens partagés avec vous dans d’autres applications mobiles s’ouvrent désormais dans l’application mobile Workfront.

  Pour plus d’informations sur le partage de liens, consultez la section .

  Cette mise à jour est désormais disponible sur iOS et Android.

* Nous avons mis à jour nos conditions de support de la plateforme iOS pour prendre en charge iPhone X.

  Pour plus d’informations sur les périphériques mobiles et les systèmes d’exploitation pris en charge, consultez la section . 
