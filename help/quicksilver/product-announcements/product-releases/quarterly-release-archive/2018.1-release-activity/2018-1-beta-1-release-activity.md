---
content-type: release-notes
navigation-topic: product-releases-archive
title: Activité Version 2018.1, version bêta 1
description: Cette page décrit toutes les modifications les plus récentes disponibles dans l’environnement Aperçu avec la version 2018.1 de Beta 1. Les fonctionnalités de cette page ont été rendues disponibles dans l’environnement Aperçu le 1er décembre 2017. Il sera disponible dans l’environnement de production en mars 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: efcc2217-ab69-4ac4-8e9a-f811eba77d49
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1065'
ht-degree: 1%

---

# Activité Version 2018.1, version bêta 1

Cette page décrit toutes les modifications les plus récentes disponibles dans l’environnement Aperçu avec la version 2018.1 de Beta 1. Les fonctionnalités de cette page ont été rendues disponibles dans l’environnement Aperçu le 1er décembre 2017. Il sera disponible dans l’environnement de production en mars 2018.

>[!IMPORTANT]
>
> Les fonctionnalités décrites sur cette page peuvent être modifiées avant leur disponibilité dans l’environnement de production.

Pour obtenir la liste de toutes les modifications apportées à la version 2018.1, voir  [Présentation de l’activité de version 2018.1](../../../../product-announcements/product-releases/quarterly-release-archive/2018.1-release-activity/2018-1-release-activity-overview.md).

La version 2018.1 de Beta 1 contient des améliorations pour les administrateurs de Workfront et d’autres utilisateurs :

**Pour les administrateurs**

* [ Modèle de mise en page mis à jour pour prendre en charge la zone d’accueil](#updated-layout-template-to-support-the-home-area)
* [Désactiver les notifications de courrier électronique de vérification envoyées depuis Workfront](#disable-proofing-email-notifications-sent-from-workfront)
* [Nouvelles ressources ajoutées aux abonnements à un événement](#new-resources-added-to-event-subscriptions)

**Pour Tous Les Utilisateurs**

* [Zone D’Accueil (Mise À Jour De Ma Zone De Travail)](#home-area-updated-my-work-area)
* [Afficher les données du planificateur de ressources sous Analyse de cas et Résumé d’analyse de cas mis à jour](#display-resource-planner-data-under-the-business-case-and-updated-business-case-summary)
* [Afficher le pourcentage d’allocation horaire planifiée dans le planificateur de ressources](#display-the-percentage-of-planned-hour-allocation-in-the-resource-planner)
* [Les types de mise à jour &quot;Automatique et En cours de modification&quot; et &quot;Modifier uniquement&quot; déclenchent des mises à jour des objets parents en même temps que les tâches sont mises à jour](#the-automatic-and-on-change-and-change-only-update-types-trigger-updates-to-the-parent-objects-at-the-same-time-as-tasks-are-updated)
* [Instantané de la chronologie disponible dans le diagramme de Gantt](#timeline-snapshot-available-in-the-gantt-chart)

## Zone d’accueil (mise à jour de ma zone de travail) {#home-area-updated-my-work-area}

La nouvelle zone d’accueil offre une autre vue améliorée des mêmes données actuellement disponibles dans la zone Mon travail. La zone Accueil offre les avantages suivants par rapport à la zone Mon travail :

* Interface plus simple et intuitive
* Amélioration des performances
* Mettre à jour les tâches et les problèmes liés au formatage de texte enrichi

## Mise à jour du modèle de mise en page pour prendre en charge la zone d’accueil {#updated-layout-template-to-support-the-home-area}

En tant qu’administrateur Workfront, vous pouvez déterminer si les utilisateurs de votre entreprise ont accès à la zone d’accueil en configurant le modèle de mise en page auquel ils sont affectés. Les utilisateurs qui n’ont pas de modèle de mise en page peuvent toujours accéder à la zone Accueil.

Pour plus d’informations, voir &quot;Création et gestion des modèles de mise en page&quot;.

## Désactiver la vérification des notifications électroniques envoyées à partir de Workfront {#disable-proofing-email-notifications-sent-from-workfront}

Vous pouvez maintenant configurer si les utilisateurs de votre instance Workfront reçoivent des notifications par e-mail de Workfront lorsqu’un commentaire est fait sur un BAT.

Auparavant, les emails de vérification étaient toujours envoyés depuis Workfront lorsqu’un commentaire était fait sur un BAT. Si les notifications étaient également activées dans Workfront Proof, les utilisateurs recevaient des notifications en double. 

Pour les clients Workfront existants, Workfront est configuré par défaut pour envoyer des emails lorsqu’un commentaire est fait sur un BAT.

Pour plus d’informations sur la désactivation des notifications par e-mail pour les bons à tirer dans Workfront, de sorte que les emails de vérification ne soient envoyés qu’à partir de Workfront Proof, voir .  

## Afficher les données du planificateur de ressources sous Analyse de cas et Résumé des analyses de cas mises à jour {#display-resource-planner-data-under-the-business-case-and-updated-business-case-summary}

La zone Ressource/Budget est désormais disponible dans l’Analyse de cas d’un projet. Dans ce domaine, vous pouvez consulter les Heures budgétisées estimées pour vos ressources dans le planificateur de ressources et le Coût de la main-d&#39;oeuvre budgétisé qui leur sont associés.

La zone des estimations de ressources de l’analyse de cas a été renommée Estimations des ressources héritées.

Dans le cadre de cette modification, le résumé des analyses de cas opérationnels comprend désormais des informations financières basées sur les estimations des ressources et le budget des ressources.

Avant cette modification, vous ne pouviez pas voir les informations du planificateur de ressources sur l’analyse de cas du projet. Vous ne pouvez voir que les informations des estimations de ressources spécifiées dans le planificateur de capacité des pools de ressources hérités.

Pour plus d’informations sur la création d’un cas d’entreprise, voir [Création d’un cas d’entreprise pour un projet](../../../../manage-work/projects/define-a-business-case/create-business-case.md).

## Afficher le pourcentage d’allocation horaire planifiée dans le planificateur de ressources {#display-the-percentage-of-planned-hour-allocation-in-the-resource-planner}

La vue utilisateur du planificateur de ressources comprend désormais une nouvelle colonne qui vous permet d’afficher l’affectation de l’heure planifiée en tant que pourcentage du total des heures disponibles pour l’utilisateur et du rôle de tâche.

Avant cette modification, vous ne pouviez afficher le total des heures planifiées et disponibles pour les utilisateurs et les rôles de tâche que dans des colonnes distinctes.

Pour plus d’informations sur la colonne Pourcentage d’affectation des heures planifiées, consultez la section &quot;Affichage de la différence entre les heures disponibles et planifiées ou l’ETP dans le planificateur de ressources&quot; dans la [présentation du planificateur de ressources](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

## Les types de mise à jour &quot;Automatique et En cours de modification&quot; et &quot;Modifier uniquement&quot; déclenchent des mises à jour des objets parents en même temps que les tâches sont mises à jour. {#the-automatic-and-on-change-and-change-only-update-types-trigger-updates-to-the-parent-objects-at-the-same-time-as-tasks-are-updated}

Nous avons modifié la manière dont les tâches parents et le projet sont mis à jour lorsqu’un objet de niveau inférieur est mis à jour dans un projet. L’heure à laquelle un objet parent est mis à jour est déterminée par le champ Type de mise à jour sur un projet. Vous pouvez sélectionner l’un des types de mise à jour suivants :

* Automatique et en cas de modification
* Modification uniquement
* Automatique uniquement
* Manuel uniquement

Désormais, lorsque vous sélectionnez les types de mise à jour &quot;Automatique et On Change&quot; ou &quot;Change Only&quot;, les modifications que vous appliquez aux tâches individuelles sont également appliquées immédiatement à la tâche parent et au projet.

Avant cette modification, vous deviez actualiser la page pour vous assurer que les objets parents et la chronologie du projet sont également mis à jour.

Pour plus d’informations sur le type de mise à jour d’un projet, voir [Sélectionner le type de mise à jour du projet](../../../../manage-work/projects/manage-projects/select-project-update-type.md).

## Instantané de la chronologie disponible dans le diagramme de Gantt {#timeline-snapshot-available-in-the-gantt-chart}

Vous pouvez désormais faire défiler rapidement la page jusqu’à un certain point de la durée de vie d’un projet à l’aide de la nouvelle capture instantanée de la chronologie dans le diagramme de Gantt.

Lorsque vous sélectionnez une période plus granulaire pour le diagramme de Gantt lors de l’affichage d’une tâche ou d’une liste de projets, une barre de défilement horizontale s’affiche au bas du graphique de Gantt. Cliquez sur la barre de défilement pour afficher la chronologie complète du projet dans un instantané. Vous pouvez cliquer n’importe où dans l’instantané du diagramme de Gantt pour accéder à un point spécifique de la durée de vie du projet.

Avant cette modification, vous deviez faire défiler horizontalement l’ensemble du diagramme de Gantt pour trouver un certain point dans le temps, ou vous deviez effectuer un zoom arrière sur la vue granulaire.

Pour plus d’informations sur l’affichage des informations dans le diagramme de Gantt, voir [Configuration de l’affichage des informations sur le graphique de Gantt](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

## Nouvelles ressources ajoutées aux abonnements à un événement {#new-resources-added-to-event-subscriptions}

Vous pouvez maintenant créer des abonnements à des événements pour les ressources suivantes :

* **Frais :** Vous avertit lorsqu’une dépense est ajoutée ou modifiée.
* **Attribution :** vous avertit lorsqu’une affectation est ajoutée ou modifiée sur une tâche ou un problème pour un utilisateur, un rôle de tâche ou une équipe.
* **Frise chronologique :** vous avertit lorsqu’une feuille de temps est envoyée, rejetée ou approuvée.

Pour en savoir plus sur les abonnements aux événements, voir [API d’abonnement à un événement](../../../../wf-api/general/event-subs-api.md).
