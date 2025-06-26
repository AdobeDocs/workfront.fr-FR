---
title: Améliorations apportées aux projets au troisième trimestre 2025
description: Améliorations apportées aux projets au troisième trimestre 2025
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
hide: true
hidefromtoc: true
exl-id: 33fa5a61-5300-402c-9f80-f2701f7999a8
source-git-commit: e3fa5f6fd86f0fe9ba221fb7c20f46f966437a42
workflow-type: tm+mt
source-wordcount: '745'
ht-degree: 7%

---

# Améliorations apportées aux projets au troisième trimestre 2025

Cette page décrit les améliorations apportées par Project à l’environnement de Prévisualisation avec la version du troisième trimestre de 2025. Ces améliorations seront rendues disponibles comme indiqué, dans l’environnement de production.

Pour obtenir la liste de toutes les modifications disponibles à ce stade du cycle de publication de la version du troisième trimestre 2025, consultez la [Vue d’ensemble de la version du troisième trimestre 2025](/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-release-overview.md).

## Le champ Heures réelles existant a été remplacé par les anciens et un nouveau champ Heures réelles a été créé

>[!NOTE]
>
> Prévisualisation et production : 24 juin 2025 

Le champ existant des heures effectives a été renommé en heures effectives héritées. Ce champ stocke le temps enregistré pour les projets, les tâches et les événements en minutes. Le champ est stocké dans la base de données Workfront en tant que realWorkRequired.

Nous avons ajouté un nouveau champ Heures réelles qui stocke les heures enregistrées pour les projets, tâches et événements dans des heures, avec une précision décimale. Le champ est stocké dans la base de données Workfront sous le nom actuelWorkRequiredDouble.

Les champs Heures réelles et Héritage d&#39;heures réelles sont visibles dans les vues et les rapports Projet, Tâche et Événements.

Le champ Heures réelles visible dans la section Détails du projet, des tâches et des événements représente les nouvelles heures réelles.



>[!IMPORTANT]
>
>Selon le moment où les heures ont été consignées, il peut y avoir une incohérence entre les heures réelles et les heures réelles héritées pour un projet, une tâche ou un événement.<br>
>&#x200B;>Les scénarios suivants sont possibles :
>
>* Les heures réelles qui représentent les heures enregistrées pour les projets, les tâches et les événements depuis mai 2021 ont été déplacées du champ Heures réelles héritées vers le nouveau champ Heures réelles.
>* Les heures réelles qui représentent les heures consignées pour les projets, les tâches et les événements avant mai 2021 ne sont prises en compte que dans le champ Heures réelles héritées.
>  &#x200B;><br>Vous devrez peut-être mettre à jour vos rapports pour refléter le nouveau champ et ses valeurs.


Pour plus d&#39;informations, voir [Afficher les heures réelles](/help/quicksilver/manage-work/tasks/task-information/actual-hours.md).


## Modification de la manière dont les heures réelles sont stockées dans la base de données pour les appels API

>[!NOTE]
>
>* Aperçu : avec la prochaine version de l’API, prévue pour plus tard en 2025
>* Mise à jour rapide de la production : avec la prochaine version de l’API, prévue pour plus tard en 2025
>* Production pour tous les clients : avec la prochaine version de l’API, prévue pour plus tard en 2025

Cette mise à jour apporte une modification à la façon dont les heures réelles des projets, tâches et événements sont stockées dans la base de données. À compter de cette mise à jour, les heures effectives utiliseront un champ de valeur de `actualWorkRequiredDouble` (avec une valeur en heures).

Avant cette mise à jour, les heures réelles étaient stockées avec un champ de valeur de `actualWorkRequired` (avec une valeur en minutes). Cette mise à jour garantit un comptage plus précis des heures réelles lors de leur calcul à l’aide d’un appel API.

En raison de cette modification, vous devrez peut-être mettre à jour tous les appels API qui font référence au champ de valeur d’origine. N’apportez aucune modification si vous utilisez un champ de valeur de `actualWorkRequiredExpression` dans les appels API.

Cette mise à jour ne modifie pas les calculs des heures effectives pour les projets, tâches et événements, dans les colonnes de champs calculés personnalisés.

## Mettre à jour dans à l’aide du curseur Pourcentage terminé dans l’en-tête d’une tâche ou d’un événement

>[!NOTE]
>
>* Prévisualisation : mercredi 27 mai 2025
>* Version rapide de production : 27 mai 2025
>* Production pour tous les clients : 27 mai 2025

Nous avons mis à jour la façon dont le curseur Pourcentage terminé fonctionne pour les tâches et les événements.

La fonctionnalité suivante est désormais disponible :

* Lorsque vous faites glisser la bulle bleue Pourcentage terminé dans l’en-tête d’une tâche ou d’un événement, le Pourcentage terminé de la tâche ou de l’événement est désormais mis à jour par incréments de cinq points. Avant cette mise à jour, le fait de faire glisser la bulle bleue Pourcentage terminé mettait à jour les tâches ou les problèmes par incréments d’un point.

* Vous pouvez double-cliquer sur la bulle bleue et la mettre à jour manuellement avec le nombre souhaité, sans utiliser le curseur. Cette fonctionnalité n’a pas été modifiée.

Aucune autre modification n’a été apportée à la mise à jour du pourcentage d’achèvement des tâches et des événements dans d’autres zones de Workfront.

Pour plus d&#39;informations, voir [Afficher et mettre à jour le pourcentage d&#39;achèvement des tâches](/help/quicksilver/manage-work/projects/updating-work-in-a-project/view-update-percent-complete-for-tasks.md).

## Plus de transparence lors de l’utilisation de l’assistant AI sur des projets, tâches et événements

>[!NOTE]
>
>* Prévisualisation : mardi 19 mai 2025
>* Version rapide de production : 19 mai 2025
>* Production pour tous les clients : 19 mai 2025

Pour clarifier la manière dont l’assistant AI localise les réponses aux questions sur les projets, tâches et problèmes Workfront, nous avons ajouté ces informations à la réponse à la question. Désormais, l’assistant AI inclut ses informations de recherche dans la sortie. Vous pouvez utiliser ces informations pour vérifier que l’assistant AI a correctement identifié la question que vous posiez et pour comprendre le contexte de la réponse.

Auparavant, ces informations n’étaient pas disponibles dans la réponse de l’assistant d’IA.

Pour plus d’informations sur l’utilisation de l’assistant AI afin d’obtenir des informations sur les éléments de Workfront, voir [ Utiliser l’assistant AI pour travailler sur des projets, des tâches et des événements](/help/quicksilver/workfront-basics/ai-assistant/work-with-pti-through-ai-assisant.md).
