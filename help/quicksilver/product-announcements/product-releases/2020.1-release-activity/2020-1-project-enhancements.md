---
content-type: release-notes
navigation-topic: 2020-1-release-activity
title: Améliorations des projets (version 2020.1)
description: Cette page décrit toutes les améliorations apportées aux projets avec la version 2020.1. Ces améliorations sont actuellement disponibles dans l’environnement de prévisualisation et seront disponibles dans l’environnement de production à la fin du mois de mars ou au début du mois d’avril 2020.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 13b6dd9e-52b9-4c5f-b727-bf32fbb94e8c
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '540'
ht-degree: 100%

---

# Améliorations des projets (version 2020.1)

Cette page décrit toutes les améliorations apportées aux projets avec la version 2020.1. Ces améliorations sont actuellement disponibles dans l’environnement de prévisualisation et seront disponibles dans l’environnement de production à la fin du mois de mars ou au début du mois d’avril 2020.

Pour obtenir la liste de toutes les modifications disponibles avec la version 2020.1, voir [Vue d’ensemble de la version 2020.1](../../../product-announcements/product-releases/2020.1-release-activity/2020-1-release-overview.md).

## Meilleure visibilité des personnes taguées dans une mise à jour

Il est désormais plus facile de voir quelles personnes sont taguées dans une mise à jour. Le nom des personnes taguées s’affiche en bleu et redirige vers leur profil.

Les personnes taguées sont également répertoriées dans la zone de commentaires.

Avant cette amélioration, les personnes précédemment taguées n’apparaissaient pas dans la zone Notifier.

Pour plus d’informations, voir [Taguer d’autres personnes sur les mises à jour](../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

## Inclure et identifier du texte cité dans une mise à jour, un commentaire ou une réponse

Lorsque vous saisissez un commentaire, vous pouvez mettre une partie de votre commentaire entre guillemets afin de le distinguer de votre propre commentaire. Utilisez le bouton Citation dans l’éditeur HTML.

Pour plus d’informations, voir [Mettre à jour le travail](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).


## Inclure un commentaire précédent dans un commentaire de mise à jour ou une réponse

Lorsque vous commentez dans un thread de mise à jour, vous pouvez rapidement inclure le texte d’un commentaire précédent. Recherchez l’option Citer la réponse dans le menu Plus en regard du commentaire que vous souhaitez citer.

Pour plus d’informations, voir [Mettre à jour le travail](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Informations supplémentaires sur les risques

Pour vous aider à mieux comprendre les risques liés à vos projets, vous pouvez désormais savoir qui et quand un risque a été saisi et quand il a été mis à jour sur un projet. Vous pouvez accéder à ces informations dans une vue des risques et par le biais de l’API Workfront publique. Ces champs seront disponibles avec la version 11 de l’API, qui sera lancée avec la version de production 2020.1.

Pour plus d’informations sur les risques dans Workfront, voir [Créer et modifier des risques sur les projets](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md).

## Champs supplémentaires ajoutés aux références et aux tâches de référence

Pour vous aider à mieux comprendre l’évolution de vos projets sur le plan financier, vous pouvez désormais inclure des informations supplémentaires sur les coûts et le revenu dans un rapport de référence ou de tâche de référence. Les informations financières supplémentaires sont ajoutées aux nouvelles références et non aux références que vous avez actuellement enregistrées.

Pour plus d’informations sur les champs financiers des projets et des tâches qui sont accessibles à partir des objets Référence et Tâche de référence, voir [Finances d’un projet incluses dans les références du projet](../../../manage-work/projects/project-finances/project-finances-included-in-project-baselines.md).

## Les problèmes avec le statut « Fermé - Approbation en attente » sont considérés comme incomplets

La manière dont Workfront gère les problèmes dont le statut est « Terminé - Approbation en attente » a été modifiée. Désormais, ces problèmes sont considérés comme ouverts et le projet ne peut pas être marqué comme terminé tant que l’approbation n’a pas été résolue.

Avant cette modification, les problèmes dont le statut était « Fermé - Approbation en attente » étaient considérés comme fermés.

Tous les problèmes dont le statut était « Fermé - Approbation en attente » avant cette modification se comporteront de la même manière qu’auparavant, considérés comme terminés et permettant au projet de s’achever également. Tous les problèmes auxquels est affecté ce statut après cette modification seront considérés comme incomplets.

Pour plus d’informations sur les statuts des projets, voir [Accéder à la liste des statuts des projets du système](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md).

