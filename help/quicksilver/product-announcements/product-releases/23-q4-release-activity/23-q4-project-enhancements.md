---
title: Améliorations du projet au quatrième trimestre 2023
description: Améliorations du projet au quatrième trimestre 2023
author: Lisa
feature: Product Announcements
source-git-commit: ee84471418590401fe143741cadd1d76a8917149
workflow-type: tm+mt
source-wordcount: '442'
ht-degree: 0%

---

# Améliorations du projet au quatrième trimestre 2023

Cette page décrit toutes les améliorations de projet apportées à la version du quatrième trimestre 2023 de l’environnement Aperçu. Ces améliorations ont été apportées à l’environnement de production avec la version 23.10.

Pour obtenir la liste de toutes les modifications disponibles à ce stade du cycle de publication du quatrième trimestre 2023, voir [Présentation de la version du quatrième trimestre 2023](/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md).

## Nouvelles approbations de documents

L’approbation des documents est en cours de reconception dans un déploiement échelonné qui sera mis à la disposition d’un plus grand nombre d’utilisateurs avec chaque version.

Dans cette version, le processus d’approbation a été simplifié pour la création d’approbations et l’approbation/révision de documents, en plus de la nouvelle fonctionnalité. Voici quelques améliorations spécifiques :

* Interface améliorée pour la modification d’un utilisateur entre un réviseur et un approbateur
* Amélioration du processus d’ajout d’un approbateur ou d’un réviseur externe
* Amélioration de l’expérience d’approbation et de révision pour les approbateurs et les réviseurs externes

Pour plus d’informations sur l’utilisation des nouvelles validations de document, voir [Nouvelle présentation des approbations de documents](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md).

[Affichez une démonstration vidéo de cette fonctionnalité.](https://video.tv.adobe.com/v/3424867){target=_blank}

## Mise à jour de la conception lors de l’ajout d’un nouveau problème à un projet

Cette mise à jour a été annoncée avec la version 23.3.

Nous avons mis à jour la boîte de dialogue Nouveau problème qui s’affiche lors de l’envoi d’un nouveau problème à un projet. Désormais, l’interface correspond à la zone Nouvelle requête qui s’affiche lors de l’envoi d’une nouvelle requête à une file d’attente de requêtes.

Pour plus d’informations, voir [Création de problèmes](/help/quicksilver/manage-work/issues/manage-issues/create-issues.md).

## Recalcul dynamique des champs calculés sur les formulaires

Les champs calculés d’un formulaire joint à un objet sont désormais recalculés dynamiquement en temps réel lorsque les valeurs dépendantes d’un formulaire sur la page sont modifiées. Vous pouvez ainsi afficher les résultats mis à jour sans enregistrer le formulaire.

Le mode de calcul des champs n&#39;a pas changé.

Sur les pages qui n’ont pas été modernisées, un petit nombre de champs de formulaire ne feront pas l’objet d’un nouveau calcul dynamique.

Pour plus d’informations, voir [Modifier les informations dans les champs de formulaire personnalisés](/help/quicksilver/workfront-basics/work-with-custom-forms/edit-custom-forms.md).

[Affichez une démonstration vidéo de cette fonctionnalité.](https://video.tv.adobe.com/v/3422678/){target=_blank}

## Définition des heures planifiées sur les tâches récurrentes enfants avec le type Durée simple sans attribution

Nous avons modifié la façon dont les heures planifiées sont attribuées aux tâches récurrentes sans affectation et avec un type Durée simple . Désormais, lorsque vous définissez Heures planifiées sur une nouvelle tâche récurrente avec un type de durée simple et aucune affectation, les heures sont également allouées aux récurrences individuelles. Avant cette modification, les heures n’étaient pas enregistrées pour des récurrences individuelles lorsque les tâches parentes n’étaient pas affectées.

Pour plus d’informations sur la création de tâches récurrentes, voir [Créer des tâches récurrentes](/help/quicksilver/manage-work/tasks/create-tasks/create-recurring-tasks.md).

## Mises à jour en temps réel sur la liste des tâches

Les listes de tâches sont désormais mises à jour en temps réel. Les modifications apportées à une tâche sont mises à jour dans la liste des tâches, de sorte qu’un utilisateur qui consulte la liste des tâches puisse voir la modification sans actualiser la page.
