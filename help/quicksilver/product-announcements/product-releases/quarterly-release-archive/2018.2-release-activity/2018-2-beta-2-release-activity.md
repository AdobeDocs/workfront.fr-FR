---
content-type: release-notes
navigation-topic: product-releases-archive
title: Activité Version 2018.2, version bêta 2
description: Cette page décrit toutes les modifications les plus récentes disponibles dans l’environnement Aperçu avec la version 2018.2 de Beta 2. Cette fonctionnalité a été rendue disponible dans l’environnement Aperçu le 5 avril 2018. Il sera disponible dans l'environnement de production en juin 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: c8ef68f5-53db-4c3c-af0f-e1c98521ec27
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '901'
ht-degree: 2%

---

# Activité Version 2018.2, version bêta 2

Cette page décrit toutes les modifications les plus récentes disponibles dans l’environnement Aperçu avec la version 2018.2 de Beta 2. Cette fonctionnalité a été rendue disponible dans l’environnement Aperçu le 5 avril 2018. Il sera disponible dans l&#39;environnement de production en juin 2018.

>[!IMPORTANT]
>
> Les fonctionnalités décrites sur cette page peuvent être modifiées avant leur disponibilité dans l’environnement de production.

Pour obtenir la liste de toutes les modifications apportées à la version 2018.2, voir  [Présentation de l’activité de version 2018.2](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-release-activity-overview.md).

La version 2018.2 de Beta 2 contient les améliorations suivantes :

* [Modifier directement les champs à partir de la zone d’accueil](#edit-fields-directly-from-the-home-area)
* [Temps de connexion en jours](#log-time-in-days)
* [ Afficher les relations entre les prédecteurs de projets sur le diagramme de Gantt dans une liste de projets](#view-cross-project-predecessor-relationships-on-the-gantt-chart-in-a-list-of-projects)
* [Utiliser le coût budgété dans Portfolio Optimizer pour calculer les finances de Portfolio](#use-budgeted-cost-in-the-portfolio-optimizer-to-calculate-portfolio-finances)
* [Rapport d’utilisation : renseigne les heures budgétées à partir de la nouvelle zone de budget des ressources](#utilization-report-populates-budgeted-hours-from-new-resource-budgeting-area) (Aperçu uniquement)

* [Rapport d’utilisation : afficher les heures budgétées par utilisateur sur un projet](#utilization-report-view-budgeted-hours-by-user-on-a-project) (aperçu uniquement)

* [Proof Progress from the Document List Available to Non-Proofing Users](#proof-progress-from-the-document-list-available-to-non-proofing-users)
* [Améliorations des périphériques mobiles](#mobile-improvements)

## Modifier directement les champs à partir de la zone d’accueil {#edit-fields-directly-from-the-home-area}

Maintenant, lorsque vous sélectionnez un objet dans la zone Accueil, vous pouvez modifier les champs qui lui sont associés directement à partir du panneau de droite de la zone Accueil. 

Avant cette modification, les informations ne pouvaient être affichées que dans la zone Accueil, et non modifiées.

Pour plus d’informations, reportez-vous à la section [Mise à jour ou modification d’un élément de travail dans la zone d’accueil](../../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md) de l’article  [Mettez à jour ou modifiez un élément de travail dans la zone Accueil](../../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md).

## Temps de connexion en jours {#log-time-in-days}

Les administrateurs de Workfront peuvent désormais configurer si les utilisateurs de leur entreprise consignent l’heure en jours ou en heures. Les utilisateurs disposant d’une licence de planificateur peuvent configurer ce paramètre pour eux-mêmes.

Avant cette modification, les utilisateurs ne pouvaient consigner le temps qu’en heures.

Vous pouvez configurer ce paramètre en modifiant le profil utilisateur. Pour plus d’informations, voir [Configurer si la durée est consignée en heures ou en jours](../../../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md).

Pour plus d’informations sur la façon dont les utilisateurs peuvent se connecter en jours après la mise à jour de ce paramètre, voir [Temps du journal](../../../../timesheets/create-and-manage-timesheets/log-time.md).

## Afficher les relations entre les prédicateurs de projets sur le diagramme de Gantt dans une liste de projets {#view-cross-project-predecessor-relationships-on-the-gantt-chart-in-a-list-of-projects}

Vous pouvez désormais afficher les relations de prédécesseur entre projets sur le graphique Gantt dans les listes de projets suivantes :

* Onglet Projets dans un portefeuille ou un programme
* Dans un rapport Projet

Avant cette modification, vous ne pouviez afficher les relations entre les prédécesseurs de plusieurs projets que pour les tâches individuelles au niveau du projet.

Pour plus d’informations, voir [Configuration de l’affichage des informations sur le diagramme de Gantt](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md). 

## Utilisation du coût budgété dans Portfolio Optimizer pour calculer les finances des Portfolios {#use-budgeted-cost-in-the-portfolio-optimizer-to-calculate-portfolio-finances}

Le nouvel Portfolio Optimizer utilise désormais le coût budgété de la nouvelle zone Budget des ressources de l’Analyse de cas ou du planificateur de ressources pour calculer les champs suivants :

* Valeur nette
* Retour sur investissement (ROI)
* Coûts

Auparavant, le nouvel Portfolio Optimizer et l’ancien utilisaient tous deux le coût budgété hérité. L’outil hérité de Portfolio Optimizer continue d’utiliser l’option Coût budgétaire hérité pour calculer la valeur nette, le retour sur investissement et le coût.

Nous avons également ajouté deux nouveaux champs aux champs financiers du Portfolio : RSI hérité et Valeur nette héritée pour capturer les nouvelles valeurs à partir des nouveaux outils de gestion des ressources.

Pour plus d’informations, reportez-vous à la section [Présentation de Portfolio Optimizer](../../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md) de l’article  [Portfolio Optimizer - Aperçu](../../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

## Rapport d’utilisation : renseigne les heures budgétisées à partir de la nouvelle zone de budget des ressources {#utilization-report-populates-budgeted-hours-from-new-resource-budgeting-area}

>[!NOTE]
>
>Cette fonctionnalité ne sera pas incluse dans la version officielle de l’environnement Aperçu avec la version 2018.2. Il sera réintroduit pendant la période bêta de la version 2018.3 et sera publié dans l’environnement de production avec la version 2018.3. 

Les heures budgétisées du rapport d’utilisation sont désormais renseignées à partir des informations disponibles dans la nouvelle zone Budget des ressources de l’Analyse de cas.

Avant cette modification, des informations de la zone des estimations de ressources héritées ont été utilisées.

Pour plus d’informations, voir [Présentation du rapport d’utilisation des ressources](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) dans l’article  [Présentation du rapport d’utilisation des ressources](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Rapport d’utilisation : affichage des heures budgétaires par utilisateur sur un projet {#utilization-report-view-budgeted-hours-by-user-on-a-project}

>[!NOTE]
>
>Cette fonctionnalité ne sera pas incluse dans la version officielle de l’environnement Aperçu avec la version 2018.2. Il sera réintroduit pendant la période bêta de la version 2018.3 et sera publié dans l’environnement de production avec la version 2018.3. 

Le rapport Utilisation d’un projet affiche désormais les heures budgétées par utilisateur.

Avant cette modification, le rapport Utilisation affichait Heures budgétées uniquement par rôle de tâche. 

Pour plus d’informations, voir [Présentation du rapport d’utilisation des ressources](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) dans l’article [Présentation du rapport d’utilisation des ressources](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Progrès du BAT depuis la liste de documents disponible pour les utilisateurs non-réviseurs {#proof-progress-from-the-document-list-available-to-non-proofing-users}

Les indicateurs de progression du BAT (Envoyé, Ouvert, Commentaires effectués et Décision) s’affichent désormais pour tous les utilisateurs qui consultent la liste du document. Cela inclut les utilisateurs qui ne sont pas en mesure de générer des bons à tirer (pour plus d’informations sur l’activation des utilisateurs à générer des bons à tirer, voir la section .

Avant cette modification, les indicateurs de progression du BAT n’étaient disponibles que pour les utilisateurs qui pouvaient générer des bons à tirer.

Pour plus d’informations, voir [Proof progress and status overview](../../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md).

## Améliorations des périphériques mobiles {#mobile-improvements}

L’application mobile contient les améliorations suivantes :

* Les liens partagés avec vous dans d’autres applications mobiles s’ouvrent désormais dans l’application mobile Workfront.

  Pour plus d’informations sur le partage de liens, voir .

  Cette mise à jour est désormais disponible sur iOS et Android.

* Nous avons mis à jour nos exigences de prise en charge de la plateforme iOS pour prendre en charge iPhone X.

  Pour plus d’informations sur les périphériques mobiles et les systèmes d’exploitation pris en charge, voir . 
