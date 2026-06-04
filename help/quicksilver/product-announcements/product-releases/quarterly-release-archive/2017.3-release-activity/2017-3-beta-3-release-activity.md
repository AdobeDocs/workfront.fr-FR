---
content-type: release-notes
navigation-topic: product-releases-archive
title: Activité de version 2017.3 Beta 3
description: La version 2017.3 sera disponible dans l’environnement de production début novembre 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: dc0cada8-4b9e-40cb-89a5-16f15268b513
TQID: https://experienceleague.adobe.com/12nUGoSnwlcVACSTf-b-Fks7QRuCCl9HBujkDNG5ubU
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 572
ht-degree: 100%

---

# Activité de version 2017.3 Beta 3

La version 2017.3 sera disponible dans l’environnement de production début novembre 2017.

>[!IMPORTANT]
>
> Les fonctionnalités décrites sur cette page peuvent être modifiées avant d’être disponibles dans l’environnement de production.

Pour obtenir la liste de toutes les modifications apportées à la version 2017.3, voir [Vue d’ensemble de l’activité Version 2017.3](../../../../product-announcements/product-releases/quarterly-release-archive/2017.3-release-activity/2017-3-release-activity-overview.md).

La version 2017.3 Beta 3 contient des améliorations pour tous les utilisateurs et utilisatrices :

* [Personnaliser les couleurs du graphique](#customize-chart-colors)
* [Options supplémentaires lors de la copie de projets](#additional-options-when-copying-projects)
* [Amélioration du planificateur de ressources : filtres](#resource-planner-improvement-filters)
* [Amélioration du planificateur de ressources : afficher les heures des problèmes dans la zone « Paramètres »](#resource-planner-improvement-show-issue-hours-in-the-settings-area)
* [Informations d’authentification unique pour les sandbox d’actualisation et de prévisualisation personnalisés Ne pas actualiser](#sso-information-for-the-custom-refresh-and-preview-sandboxes-do-not-refresh)
* [Mise à jour des exigences de prise en charge du navigateur pour Workfront Proof](#updated-browser-support-requirements-for-workfront-proof)

## Personnaliser les couleurs des graphiques {#customize-chart-colors}

Vous pouvez désormais personnaliser les couleurs des éléments des graphiques. Cela s’applique à tous les types de graphique dans les rapports. Cela ne s’applique pas au graphique de Gantt.

Avant cette modification, les couleurs des éléments de tous les graphiques étaient sélectionnées par défaut par Workfront. Pour plus d’informations sur la personnalisation des couleurs des graphiques, voir « Personnalisation des couleurs des graphiques » dans [Ajouter un graphique à un rapport](../../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

## Options supplémentaires lors de la copie de projets {#additional-options-when-copying-projects}

Désormais, lors de la copie d’un projet, les options correspondent à celles disponibles lors de la copie de tâches ou de problèmes. Vous pouvez également modifier le statut du projet copié lorsque vous le copiez.

Avant cette mise à jour, vous ne pouviez pas modifier le statut du projet copié lors de sa copie, et seules deux options étaient disponibles lors de la copie d’un projet :

* Conserver les affectations sur les tâches et le projet
* Conserver la progression des tâches et du projet

Avec la nouvelle fonctionnalité, les anciennes options ont été supprimées et les options suivantes ont été ajoutées lors de la copie d’un projet :

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

Pour plus d’informations sur les nouvelles fonctionnalités relatives à la copie de projets, voir la section « Copie d’un projet dans l’environnement de prévisualisation » dans [Copier un projet](../../../../manage-work/projects/manage-projects/copy-project.md).

## Amélioration du planificateur de ressources : filtres {#resource-planner-improvement-filters}

Vous pouvez désormais filtrer les informations affichées dans le planificateur de ressources selon les objets suivants :

* Portfolio
* Statut de projet
* Equipe
* Fonction
* Pool de ressources

Vous pouvez également ajouter un filtre personnalisé basé sur ces objets.

Pour plus d’informations sur l’utilisation du planificateur de ressources, voir [Vue d’ensemble du planificateur de ressources](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md). 

## Amélioration du planificateur de ressources : afficher les heures des problèmes dans la zone « Paramètres » {#resource-planner-improvement-show-issue-hours-in-the-settings-area}

Le planificateur de ressources comprend une nouvelle zone Paramètres qui affiche plusieurs options permettant de personnaliser le planificateur de ressources. Avec cette version, nous avons ajouté la première option, afin d’inclure le nombre d’heures prévues des problèmes dans les colonnes Nombre d’heures prévues du planificateur de ressources.

Pour plus d’informations sur l’utilisation du planificateur de ressources, consultez la section [Vue d’ensemble du planificateur de ressources](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

## Informations sur l’authentification unique pour les sandbox de prévisualisation et d’actualisation personnalisés Ne pas actualiser {#sso-information-for-the-custom-refresh-and-preview-sandboxes-do-not-refresh}

À partir de cette version, lors de l’actualisation de vos sandbox de prévisualisation et d’actualisation personnalisés, les informations d’authentification unique ne sont pas copiées depuis votre environnement de production et ne sont pas désactivées. Avant cette modification, les informations d’authentification unique dans les sandbox de prévisualisation et d’actualisation personnalisés étaient désactivées et définies sur « Aucun ».

Pour plus d’informations sur l’environnement de sandbox d’actualisation personnalisé, consultez la section [Environnement de sandbox d’actualisation personnalisé Adobe Workfront](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md).

Pour plus d’informations sur l’environnement des sandbox de prévisualisation, consultez la section [Environnement de sandbox de prévisualisation Adobe Workfront](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).

## Mise à jour des exigences de prise en charge du navigateur pour Workfront Proof {#updated-browser-support-requirements-for-workfront-proof}

Les conditions de prise en charge du navigateur pour Workfront Proof ont été mises à jour. Pour plus d’informations, consultez la section [Conditions requises du navigateur pour Adobe Workfront](../../../../workfront-basics/workfront-browser-requirements.md).
