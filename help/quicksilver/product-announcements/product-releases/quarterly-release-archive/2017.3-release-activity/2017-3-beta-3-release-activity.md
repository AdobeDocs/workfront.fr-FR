---
content-type: release-notes
navigation-topic: product-releases-archive
title: Activité de version 2017.3 bêta 3
description: La version 2017.3 sera disponible dans l’environnement de production début novembre 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: dc0cada8-4b9e-40cb-89a5-16f15268b513
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '572'
ht-degree: 6%

---

# Activité de version 2017.3 bêta 3

La version 2017.3 sera disponible dans l’environnement de production début novembre 2017.

>[!IMPORTANT]
>
> Les fonctionnalités décrites sur cette page peuvent être modifiées avant leur disponibilité dans l’environnement de production.

Pour obtenir la liste de toutes les modifications apportées à la version 2017.3, voir  [Présentation de l’activité de la version 2017.3](../../../../product-announcements/product-releases/quarterly-release-archive/2017.3-release-activity/2017-3-release-activity-overview.md).

La version bêta 3 2017.3 contient des améliorations pour tous les utilisateurs :

* [Personnalisation des couleurs du graphique](#customize-chart-colors)
* [Options supplémentaires lors de la copie de projets](#additional-options-when-copying-projects)
* [Amélioration du planificateur de ressources : filtres](#resource-planner-improvement-filters)
* [Amélioration du planificateur de ressources : afficher les heures de problème dans la zone &quot;Paramètres&quot;](#resource-planner-improvement-show-issue-hours-in-the-settings-area)
* [Informations d’authentification unique pour les environnements de test d’actualisation et de prévisualisation personnalisés - Ne pas actualiser](#sso-information-for-the-custom-refresh-and-preview-sandboxes-do-not-refresh)
* [Mise à jour des exigences de prise en charge du navigateur pour le BAT Workfront](#updated-browser-support-requirements-for-workfront-proof)

## Personnalisation des couleurs du graphique {#customize-chart-colors}

Vous pouvez désormais personnaliser les couleurs des éléments des graphiques. Cela s’applique à tous les types de graphique dans les rapports. Cela ne s’applique pas au diagramme de Gantt.

Avant cette modification, les couleurs des éléments de tous les graphiques étaient sélectionnées par défaut par Workfront. Pour plus d’informations sur la personnalisation des couleurs des graphiques, reportez-vous aux sections &quot;Personnalisation des couleurs des graphiques&quot; dans [Ajouter un graphique à un rapport](../../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

## Options supplémentaires lors de la copie de projets {#additional-options-when-copying-projects}

Désormais, lors de la copie d’un projet, les options correspondent à celles disponibles lors de la copie de tâches ou de problèmes. Vous pouvez également modifier l’état du projet copié lorsque vous le copiez.

Avant cette mise à jour, vous ne pouviez pas modifier l’état du projet copié lors de sa copie, et seules deux options étaient disponibles lors de la copie d’un projet :

* Pour conserver les affectations sur les tâches et le projet
* Pour conserver la progression des tâches et du projet

Avec la nouvelle fonctionnalité, les anciennes options ont été supprimées et les options suivantes ont été ajoutées lors de la copie d’un projet :

* Affectations
* Effacer informations financières
* Effacer progression
* Supprimer les approbations
* Effacer les données personnalisées
* Effacer les avis de rappel
* Effacer les documents
* Effacer les dépenses
* Effacer toutes les tâches antérieures
* Autorisations de suppression
* Sélectionner tout

Pour plus d’informations sur les nouvelles fonctionnalités relatives à la copie de projets, voir la section &quot;Copie d’un projet dans l’environnement d’aperçu&quot; dans   [Copier un projet](../../../../manage-work/projects/manage-projects/copy-project.md).

## Amélioration du planificateur de ressources : filtres {#resource-planner-improvement-filters}

Vous pouvez désormais filtrer les informations affichées dans le planificateur de ressources selon les objets suivants :

* Portfolio
* Statut de projet
* Equipe
* Fonction
* Pool de ressources

Vous pouvez également ajouter un filtre personnalisé basé sur ces objets.

Pour plus d’informations sur l’utilisation du planificateur de ressources, voir [Présentation de Resource Planner](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md). 

## Amélioration du planificateur de ressources : afficher les heures de problème dans la zone &quot;Paramètres&quot; {#resource-planner-improvement-show-issue-hours-in-the-settings-area}

Une nouvelle zone Paramètres s’affiche dans le planificateur de ressources et affiche plusieurs options permettant de personnaliser le planificateur de ressources. Avec cette version, nous avons ajouté la première option, afin d’inclure les heures planifiées des problèmes dans les colonnes Heures planifiées du planificateur de ressources.

Pour plus d’informations sur l’utilisation du planificateur de ressources, voir [Présentation de Resource Planner](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

## Informations d’authentification unique pour les environnements de test d’actualisation et de prévisualisation personnalisés - Ne pas actualiser {#sso-information-for-the-custom-refresh-and-preview-sandboxes-do-not-refresh}

À compter de cette version, lorsque vous actualisez vos environnements de test d’actualisation et de prévisualisation personnalisés, les informations d’authentification unique ne sont pas copiées à partir de votre environnement de production et ne sont pas désactivées. Avant cette modification, les informations d’authentification unique dans les sandbox d’actualisation et de prévisualisation personnalisées étaient désactivées et définies sur &quot;Aucun&quot;.

Pour plus d’informations sur l’environnement Sandbox d’actualisation personnalisée, voir [Environnement Sandbox d’actualisation personnalisée d’Adobe Workfront](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md).

Pour plus d’informations sur l’environnement de prévisualisation Sandbox, voir [Environnement Adobe Workfront Preview Sandbox](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).

## Mise à jour des exigences de prise en charge du navigateur pour le BAT Workfront {#updated-browser-support-requirements-for-workfront-proof}

Mise à jour des exigences de prise en charge du navigateur pour le BAT Workfront - Pour plus d’informations, voir [Configuration requise pour le navigateur Adobe Workfront](../../../../workfront-basics/workfront-browser-requirements.md).
