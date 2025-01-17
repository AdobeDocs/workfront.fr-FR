---
title: Améliorations de l’équipe d’aministration au premier trimestre 2025
description: Améliorations de l’équipe d’aministration au premier trimestre 2025
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: fa24040d-0403-4799-b690-c3d172797115
source-git-commit: 9caac488522d2a12d3bdf4bf23ba7e44c6dbf7d2
workflow-type: tm+mt
source-wordcount: '834'
ht-degree: 13%

---

# Améliorations de l’équipe d’aministration au premier trimestre 2025

Cette page décrit toutes les améliorations de l’équipe d’aministration apportées à l’environnement de prévisualisation par la version du premier trimestre 2025. Ces améliorations seront rendues disponibles comme indiqué, dans l’environnement de production.

Pour obtenir la liste de toutes les modifications disponibles à ce stade du cycle de publication de la version du premier trimestre 2025, consultez l’article [Vue d’ensemble de la version du premier trimestre 2025](/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-release-overview.md).

## Les règles métier sont désormais prises en charge pour plus d’objets

>[!NOTE]
>
>Version préliminaire : 16 janvier 2025 ; Version de production pour tous les clients : avec version 25.1 (janvier 2025)
>
>_Disponible uniquement pour les organisations figurant dans le plan Ultimate._

Vous pouvez maintenant créer des règles métier et appliquer une validation à ces objets supplémentaires : Société, Itération, Catégorie de ressources hors main-d&#39;œuvre, Fonction, Utilisateur, Affectation, Pool de ressources, Congés, Document et Heure.

Les objets suivants étaient déjà pris en charge pour les règles métier : Projet, Tâche, Demande, Portfolio, Programme, Dépense, Enregistrement de facturation, Groupe, Risque et Carte tarifaire.

Pour plus d’informations, voir [Créer et modifier des règles métier](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/business-rules.md).

## Comparaison d’objets entre des environnements pour la promotion de l’environnement

>[!NOTE]
>
>Version préliminaire : 6 janvier 2025 ; Version de production pour tous les clients : avec la version 25.1 (janvier 2025)

Pour faciliter la détermination de l’objet à inclure dans un package de promotion d’environnement, nous avons ajouté la possibilité de comparer des objets entre les environnements. Vous pouvez désormais sélectionner des types d’objets et des environnements. Workfront génère une liste d’objets de ce type, indiquant s’ils sont présents dans l’environnement cible et si cet objet présente des différences entre l’environnement source et l’environnement cible. Vous pouvez ensuite ajouter des objets à un package directement à partir de cette liste.

Auparavant, si l’utilisateur souhaitait comparer des objets entre des environnements, il devait vérifier ces objets manuellement.

Pour plus d’informations, voir [Comparer des objets entre des environnements](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-compare.md).

## Plus d’objets disponibles pour la promotion de l’environnement

>[!NOTE]
>
>Version préliminaire : 6 janvier 2025 ; Version de production pour tous les clients : avec la version 25.1 (janvier 2025)

Nous avons ajouté d&#39;autres objets pour étendre les fonctionnalités de promotion d&#39;environnement. Vous pouvez maintenant ajouter les objets suivants à un package de promotion d’environnement :

* Emplacements
* Cartes tarifaires
* Affectations

Auparavant, ces objets n’étaient pas disponibles pour la promotion de l’environnement.

Pour plus d&#39;informations sur les objets disponibles pour la promotion de l&#39;environnement, consultez [Objets pris en charge pour la promotion de l&#39;environnement](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md#supported-objects-for-environment-promotion) dans l&#39;article Présentation de la promotion de l&#39;environnement.

## Empêcher le déplacement de tâches en cas d&#39;heures consignées

>[!NOTE]
>
>Version préliminaire : 19 décembre 2024 ; Version de production pour tous les clients : avec la version 25.1 (16 janvier 2025)

Comme le déplacement de tâches ou d’événements pour lesquels des heures ont été consignées peut parfois entraîner des problèmes de conformité ou d’audit, nous avons ajouté une préférence dans les Préférences des tâches et des événements de la Configuration qui vous permet d’empêcher les utilisateurs de déplacer des tâches et des événements si des heures y sont consignées. Avant cette amélioration, les utilisateurs et utilisatrices pouvaient déplacer des tâches et des événements vers d’autres projets, même si des heures leur étaient affectées.

Pour plus d’informations, voir [Configurer les préférences de tâche et de problème à l’échelle du système](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

## Préférence pour l&#39;utilisation des prévisions de projet ou d&#39;utilisateur pour les tâches à affectation unique

>[!NOTE]
>
>Version préliminaire : 21 novembre 2024 ; Production pour la version rapide : avec la version 24.12 (12 décembre 2024) ; Production pour la version trimestrielle : avec la version 25.1 (16 janvier 2025)

En tant qu’administrateur système ou de groupe, vous disposez désormais d’une nouvelle préférence qui permet d’indiquer si Workfront doit utiliser le planning du projet ou de l’utilisateur pour calculer la chronologie du projet lorsque vous affectez un utilisateur à une tâche et que le projet et l’utilisateur sont tous deux associés à un planning. Avant cette amélioration, ce paramètre existait pour les affectations à plusieurs utilisateurs. Le paramètre est désormais disponible pour les affectations de tâches à un seul utilisateur.

Pour plus d’informations, consultez la section [Configurer des préférences de projet à l’échelle du système](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## Les règles métier prennent désormais en charge les liens hypertexte

>[!NOTE]
>
>Version préliminaire : 21 novembre 2024 ; Production pour la version rapide : avec la version 24.12 (12 décembre 2024) ; Production pour la version trimestrielle : avec la version 25.1 (16 janvier 2025)

Vous pouvez désormais inclure des liens hypertexte dans le message d’erreur personnalisé d’une règle métier, afin de guider l’utilisateur ou l’utilisatrice sur la manière de modifier son action dans la contrainte de la règle. L’URL statique peut renvoyer vers la documentation ou d’autres pages utiles à l’utilisateur ou à l’utilisatrice.

Pour plus d’informations, voir [Créer et modifier des règles métier](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/business-rules.md).

## Le filtrage sur les champs de saisie semi-automatique natifs est désormais disponible

>[!NOTE]
>
>Version préliminaire : 21 novembre 2024 ; Production pour la version rapide : avec la version 24.12 (12 décembre 2024) ; Production pour la version trimestrielle : avec la version 25.1 (16 janvier 2025)

Lorsque vous ajoutez une référence de champ native à un formulaire personnalisé et qu’elle fait référence à un champ de saisie semi-automatique (par exemple, Portfolio, Société ou Propriétaire), une option de filtrage est désormais disponible. Le filtre vous permet de limiter les objets que les utilisateurs peuvent choisir lorsqu’ils utilisent le champ . Ce filtre personnalisé fonctionne de la même manière qu’un filtre sur un champ de saisie semi-automatique personnalisé, en utilisant le mode texte pour définir le filtre.

Pour plus d’informations, voir [Créer un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Icône « Déplacer vers » ajoutée aux champs personnalisés

>[!NOTE]
>
>Version de prévisualisation : mercredi 29 octobre 2024. Production pour version rapide : avec la version 24.11 (vendredi 14 novembre 2024). Production pour version trimestrielle : avec la version 25.1 (vendredi 16 janvier 2025).

Lorsqu’un formulaire personnalisé contient plusieurs sections avec de nombreux champs, il peut être difficile de déplacer un champ d’une section à une autre en effectuant un glisser-déposer. Une icône « Déplacer vers » a été ajoutée à chaque champ, vous permettant de sélectionner la section dans laquelle le champ est placé.

Pour plus d’informations, voir [Organisation et prévisualisation d’un formulaire](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md).
