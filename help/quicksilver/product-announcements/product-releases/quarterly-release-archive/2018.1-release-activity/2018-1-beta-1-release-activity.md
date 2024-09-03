---
content-type: release-notes
navigation-topic: product-releases-archive
title: Activité Version bêta 1 2018.1
description: Cette page décrit tous les changements les plus récents disponibles dans l’environnement de prévisualisation avec la version 2018.1 bêta 1. Les fonctionnalités présentées sur cette page ont été mises à disposition dans l’environnement de prévisualisation le 1er décembre 2017. Elles seront disponibles dans l’environnement de production en mars 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: efcc2217-ab69-4ac4-8e9a-f811eba77d49
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1065'
ht-degree: 100%

---

# Activité Version bêta 1 2018.1

Cette page décrit tous les changements les plus récents disponibles dans l’environnement de prévisualisation avec la version 2018.1 bêta 1. Les fonctionnalités présentées sur cette page ont été mises à disposition dans l’environnement de prévisualisation le 1er décembre 2017. Elles seront disponibles dans l’environnement de production en mars 2018.

>[!IMPORTANT]
>
>Les fonctionnalités décrites sur cette page peuvent être modifiées avant d’être disponibles dans l’environnement de production.

Pour obtenir la liste de toutes les modifications apportées dans la version 2018.1, consultez [Vue d’ensemble de l’activité de la version 2018.1](../../../../product-announcements/product-releases/quarterly-release-archive/2018.1-release-activity/2018-1-release-activity-overview.md).

La version 2018.1 bêta 1 contient des améliorations pour l’équipe d’administration de Workfront et les autres utilisateurs et utilisatrices :

**Pour les administrateurs et administratrices**

* [Mise à jour du modèle de mise en page pour prendre en charge la zone d’accueil](#updated-layout-template-to-support-the-home-area)
* [Désactiver les notifications par e-mail de relecture envoyées depuis Workfront](#disable-proofing-email-notifications-sent-from-workfront)
* [Nouvelles ressources ajoutées aux abonnements aux événements](#new-resources-added-to-event-subscriptions)

**Pour tous les utilisateurs et toutes les utilisatrices**

* [Zone d’accueil (mise à jour de la zone « Mon travail »)](#home-area-updated-my-work-area)
* [Afficher les données du planificateur de ressources sous le business case et le récapitulatif actualisé du business case](#display-resource-planner-data-under-the-business-case-and-updated-business-case-summary)
* [Afficher le pourcentage d’affectation des heures prévues dans le planificateur de ressources](#display-the-percentage-of-planned-hour-allocation-in-the-resource-planner)
* [Les types de mise à jour « Automatique et En cas de modification » et « Modification uniquement » déclenchent la mise à jour des objets parent en même temps que la mise à jour des tâches.](#the-automatic-and-on-change-and-change-only-update-types-trigger-updates-to-the-parent-objects-at-the-same-time-as-tasks-are-updated)
* [Instantané de la chronologie disponible dans le graphique de Gantt](#timeline-snapshot-available-in-the-gantt-chart)

## Zone Accueil (mise à jour de la zone Mon travail) {#home-area-updated-my-work-area}

La nouvelle zone Accueil offre une autre vue améliorée des mêmes données actuellement disponibles dans la zone Mon travail. La zone Accueil offre les avantages suivants par rapport à la zone Mon travail :

* Interface plus simple et intuitive
* Amélioration des performances
* Mettre à jour les tâches et les problèmes liés au formatage de texte enrichi

## Modèle de mise en page mis à jour pour prendre en charge la zone d’accueil {#updated-layout-template-to-support-the-home-area}

En tant qu’administrateur ou administratrice Workfront, vous pouvez déterminer si les utilisateurs et utilisatrices de votre entreprise ont accès à la zone d’accueil en configurant le modèle de mise en page auquel ils sont affectés. Les utilisateurs et utilisatrices auxquels aucun modèle de mise en page n’a été affecté peuvent toujours accéder à la zone d’accueil.

Pour plus d’informations, consultez la section « Créer et gérer des modèles de mise en page ».

## Désactiver les notifications par e-mail de relecture envoyées depuis Workfront {#disable-proofing-email-notifications-sent-from-workfront}

Vous avez maintenant la possibilité de paramétrer si les utilisateurs et les utilisatrices de votre instance Workfront reçoivent des notifications par e-mail de Workfront lorsqu’un commentaire est posté sur une épreuve.

Auparavant, les e-mails de relecture étaient toujours envoyés depuis Workfront lorsqu’un commentaire était posté sur une épreuve. Si les notifications étaient également activées dans Workfront Proof, les utilisateurs et les utilisatrices recevaient des notifications en double. 

Pour les clientes et les clients existants de Workfront, Workfront est configuré par défaut pour envoyer des e-mails lorsqu’un commentaire est posté sur une épreuve.

Pour savoir comment désactiver les notifications par e-mail pour les épreuves dans Workfront afin que les e-mails de relecture soient envoyés uniquement à partir de Workfront Proof, consultez la section . 

## Afficher les données du planificateur de ressources sous le business case et le récapitulatif actualisé du business case {#display-resource-planner-data-under-the-business-case-and-updated-business-case-summary}

La zone d’établissement du budget de ressources est désormais disponible dans le business case d’un projet. Dans cette zone, vous pouvez consulter les heures budgétées estimées pour vos ressources dans le planificateur de ressources et les coûts budgétés de main-d’œuvre qui leur sont associés.

La partie du business case consacrée aux estimations de ressources a été renommée « Anciennes estimations de ressources ».

Dans le cadre de ce changement, le récapitulatif du business case comprend désormais des informations financières basées à la fois sur les estimations de ressources et sur l’établissement du budget de ressources.

Avant cette modification, vous ne pouviez pas voir les informations du planificateur de ressources dans le business case du projet. Vous ne pouviez voir que les informations relatives aux estimations de ressources spécifiées dans le planificateur de capacité des anciens groupes de ressources.

Pour plus d’informations sur la création d’un business case, consultez la section [Créer un business case pour un projet](../../../../manage-work/projects/define-a-business-case/create-business-case.md).

## Afficher le pourcentage d’affectation des heures prévues dans le planificateur de ressources {#display-the-percentage-of-planned-hour-allocation-in-the-resource-planner}

La vue des utilisateurs et des utilisatrices du planificateur de ressources comprend désormais une nouvelle colonne qui vous permet d’afficher en pourcentage l’affectation des heures prévues par rapport au nombre total d’heures disponibles pour l’utilisateur ou l’utilisatrice et la fonction.

Avant cette modification, vous pouviez afficher le nombre total des heures prévues et disponibles pour les utilisateurs et les utilisatrices et les fonctions uniquement dans des colonnes séparées.

Pour plus d’informations sur la colonne Pourcentage d’attribution des heures prévues, voir la section « Visualiser la différence entre les heures disponibles et prévues ou les équivalents temps complet dans le planificateur de ressources » dans la [Vue d’ensemble du planificateur de ressources](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

## Les types de mise à jour « Automatique et En cas de modification » et « Modification uniquement » déclenchent la mise à jour des objets parent en même temps que la mise à jour des tâches. {#the-automatic-and-on-change-and-change-only-update-types-trigger-updates-to-the-parent-objects-at-the-same-time-as-tasks-are-updated}

Nous avons modifié la façon dont les tâches parent et le projet sont mis à jour lorsqu’un objet de niveau inférieur est mis à jour dans un projet. Le moment où un objet parent est mis à jour est déterminé par le champ Type de mise à jour d’un projet. Vous pouvez sélectionner l’un des types de mise à jour suivants :

* Automatique et en cas de modification
* Modification uniquement
* Automatique uniquement
* Manuel uniquement

Désormais, lorsque vous sélectionnez les types de mise à jour « Automatique et En cas de modification » ou « Modification uniquement », les modifications que vous appliquez aux tâches individuelles sont également immédiatement appliquées à la tâche parent et au projet.

Avant cette modification, vous deviez actualiser la page pour vous assurer que les objets parent et la chronologie du projet étaient également mis à jour.

Pour plus d’informations sur le type de mise à jour d’un projet, voir [Sélectionner le type de mise à jour du projet](../../../../manage-work/projects/manage-projects/select-project-update-type.md).

## Instantané de la chronologie disponible dans le graphique de Gantt {#timeline-snapshot-available-in-the-gantt-chart}

Vous pouvez désormais vous rendre rapidement à un point précis de la durée de vie d’un projet en utilisant le nouvel instantané de la chronologie dans le graphique de Gantt.

Lorsque vous sélectionnez une période plus granulaire pour le graphique e de Gantt lors de l’affichage d’une tâche ou d’une liste de projets, une barre de défilement horizontale s’affiche au bas du graphique de Gantt. En cliquant sur la barre de défilement, vous pouvez voir l’ensemble de la chronologie du projet dans un instantané. Vous pouvez cliquer n’importe où à l’intérieur de l’instantané du graphique de Gantt pour vous rendre à un point précis de la durée de vie du projet.

Avant cette modification, vous deviez faire défiler horizontalement l’ensemble du graphique de Gantt pour trouver un certain point dans le temps, ou vous deviez faire un zoom arrière sur la vue granulaire.

Pour plus d’informations sur l’affichage des informations dans le graphiquee de Gantt, voir [Configurer l’affichage des informations sur le graphique de Gantt](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

## Nouvelles ressources ajoutées aux abonnements aux événements {#new-resources-added-to-event-subscriptions}

Vous pouvez maintenant créer des abonnements à des événements pour les ressources suivantes :

* **Dépenses :** vous avertit lorsqu’une dépense est ajoutée ou modifiée.
* **Affectation :** vous avertit lorsqu’une affectation est ajoutée ou modifiée sur une tâche ou un problème pour une personne, une fonction ou une équipe.
* **Feuille de temps :** vous avertit lorsqu’une feuille de temps est soumise, refusée ou approuvée.

Pour en savoir plus sur les abonnements aux événements, voir [API d’abonnement aux événements](../../../../wf-api/general/event-subs-api.md).
