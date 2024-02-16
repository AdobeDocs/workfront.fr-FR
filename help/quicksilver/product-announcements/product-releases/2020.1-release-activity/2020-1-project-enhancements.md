---
content-type: release-notes
navigation-topic: 2020-1-release-activity
title: Améliorations du projet 2020.1
description: Cette page décrit toutes les améliorations apportées aux projets avec la version 2020.1. Ces améliorations sont actuellement disponibles dans l’environnement Aperçu et seront disponibles dans l’environnement Production à la fin du mois de mars ou au début du mois d’avril 2020.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 13b6dd9e-52b9-4c5f-b727-bf32fbb94e8c
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '540'
ht-degree: 0%

---

# Améliorations du projet 2020.1

Cette page décrit toutes les améliorations apportées aux projets avec la version 2020.1. Ces améliorations sont actuellement disponibles dans l’environnement Aperçu et seront disponibles dans l’environnement Production à la fin du mois de mars ou au début du mois d’avril 2020.

Pour obtenir la liste de toutes les modifications disponibles avec la version 2020.1, voir [Présentation de la version 2020.1](../../../product-announcements/product-releases/2020.1-release-activity/2020-1-release-overview.md).

## Identifier plus facilement les balises d’une mise à jour

Il est désormais plus facile de voir quels utilisateurs sont balisés dans une mise à jour. L’affichage en bleu du nom d’utilisateur balisé et le lien vers le profil utilisateur.

Les utilisateurs balisés sont également répertoriés sous la zone de commentaire.

Avant cette amélioration, les utilisateurs précédemment balisés ne s’affichaient pas dans la zone Notifier .

Pour plus d’informations, voir [Balisage des autres sur les mises à jour](../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

## Inclure et identifier le texte entre guillemets dans un commentaire ou une réponse de mise à jour

Lorsque vous saisissez un commentaire, vous pouvez le marquer comme une partie de votre commentaire entre guillemets afin de le distinguer de votre propre commentaire. Utilisez le bouton Blocs de citations dans l’éditeur de HTMLS.

Pour plus d’informations, voir [Mise à jour du travail](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).


## Citer un commentaire précédent dans un commentaire ou une réponse de mise à jour

Lorsque vous commentez dans un thread de mise à jour, vous pouvez rapidement inclure le texte d’un commentaire précédent dans le thread. Recherchez l’option Réponse aux guillemets dans le menu Plus en regard du commentaire que vous souhaitez citer.

Pour plus d’informations, voir [Mise à jour du travail](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Informations supplémentaires sur les risques

Pour vous aider à mieux comprendre les risques de vos projets, vous pouvez désormais savoir qui et quand un risque a été saisi et quand il a été mis à jour sur un projet. Vous pouvez accéder à ces informations dans une vue des risques et via l’API Workfront publique. Ces champs seront disponibles avec l’API version 11, qui est disponible avec la version de production 2020.1.

Pour plus d’informations sur les risques dans Workfront, voir [Créer et modifier des risques sur les projets](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md).

## Champs supplémentaires ajoutés aux lignes de base et aux tâches de base

Pour vous aider à mieux comprendre l’avancement financier de vos projets, vous pouvez désormais inclure des informations supplémentaires sur les coûts et les recettes dans un rapport de ligne de base ou de tâche de ligne de base. Les informations financières supplémentaires ne sont pas ajoutées aux lignes de base que vous avez actuellement enregistrées, mais elles sont ajoutées pour les nouvelles lignes de base.

Pour plus d’informations sur les champs financiers de projet et de tâche accessibles à partir des objets Tâche de ligne de base et Tâche de ligne de base, voir [Finances du projet incluses dans les lignes de base du projet](../../../manage-work/projects/project-finances/project-finances-included-in-project-baselines.md).

## Les problèmes à l’état &quot;Approbation fermée en attente&quot; sont considérés comme incomplets.

La manière dont Workfront gère les problèmes dans un état &quot;Approbation complète en attente&quot; a été modifiée. Désormais, ces problèmes sont perçus comme ouverts et le projet ne peut pas être marqué comme terminé tant que l’approbation n’a pas été résolue.

Avant cette modification, les problèmes dont le statut était &quot;Fermé en attente d’approbation&quot; étaient considérés comme fermés.

Tous les problèmes qui ont été placés dans un état Fermé - En attente d’approbation avant cette modification se comporteront de la même manière qu’auparavant, étant considérés comme terminés et permettant au projet de se terminer également. Toutes les questions placées dans cet état après cette modification seront considérées comme incomplètes.

Pour plus d’informations sur les états d’un projet, voir [Accéder à la liste des états des projets système](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md).

