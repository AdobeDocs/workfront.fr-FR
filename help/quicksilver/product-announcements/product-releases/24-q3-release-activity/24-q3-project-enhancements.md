---
title: Améliorations du projet au troisième trimestre 2024
description: Améliorations du projet au troisième trimestre 2024
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 27d479d1-338a-429c-9703-8e72ed8d5c95
source-git-commit: 3326173517762a62630d6b7285cc8a22873a6712
workflow-type: tm+mt
source-wordcount: '408'
ht-degree: 45%

---

# Améliorations du projet au troisième trimestre 2024

Cette page décrit toutes les améliorations de projet apportées à la version du troisième trimestre 2024 de l’environnement Aperçu. Si indiqué, ces améliorations seront disponibles dans l’environnement de production.

Pour obtenir la liste de toutes les modifications disponibles à ce stade du cycle de publication du troisième trimestre 2024, voir [Présentation de la version du troisième trimestre 2024](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md).


## Modifiez la tâche et publiez la condition et la date de validation dans la section d’en-tête ou de détails.

>[!NOTE]
>
>Aperçu de la version : 30 mai 2024 ; Production pour une version rapide : avec la version 24.6 (13 juin 2024) ; Version de production pour tous les clients : avec la version 24.7 (18 juillet 2024).

Pour faciliter la mise à jour des tâches et des problèmes, nous avons maintenant ajouté les champs Date de validation et Condition en tant qu’options à ajouter à la section En-têtes de tâche et de problème et Détails dans un modèle de mise en page. Les utilisateurs peuvent désormais mettre à jour ces champs à partir de l’en-tête ou de la section Détails d’une page lorsqu’ils sont affectés au modèle de mise en page modifié. Avant cette amélioration, vous ne pouviez pas ajouter la condition et la date de validation des tâches et des problèmes lors de la personnalisation des en-têtes.

Pour plus d’informations sur la mise à jour de la date de validation et de la condition, voir les articles suivants :

* [Mise à jour de la condition pour les tâches et les problèmes](/help/quicksilver/manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md).
* [Mise à jour de la date de validation sur les tâches et les problèmes](/help/quicksilver/manage-work/projects/updating-work-in-a-project/update-commit-date-on-tasks-and-issues.md).

[Regardez une démonstration vidéo de cette fonctionnalité.](https://video.tv.adobe.com/v/3429471/){target=_blank}

## Affectations intelligentes plus pertinentes

>[!NOTE]
>
>Aperçu de la version : 21 décembre 2023 ; Production pour une version rapide : avec la version 24.5 (16 mai 2024) ; Version de production pour tous les clients : avec la version 24.7 (18 juillet 2024).

Nous avons modifié l’algorithme utilisé par Workfront pour calculer et suggérer des affectations intelligentes pour les tâches. Le nouvel algorithme s’applique aux zones suivantes de Workfront où vous affectez une tâche : listes de tâches, zone Affectations dans l’en-tête de la tâche, Accueil et panneau Résumé.

Désormais, l’algorithme examine les informations suivantes lorsqu’il suggère des affectations intelligentes :

* Similarités entre les noms des tâches, des projets et des portfolios.

* Fréquence d’affectation à une tâche dont le nom est similaire.

Si le nouvel algorithme ne trouve aucune correspondance, les critères existants de calcul des affectations intelligentes sont appliqués.

Tenez également compte des points suivants :

* Le nom de la liste des affectations intelligentes « Voici quelques suggestions » a été remplacé par «Affectations suggérées » dans la liste des tâches.

* Il n’y a aucune modification dans le mode de calcul des affectations intelligentes pour les problèmes. Le nom de la liste des affectations intelligentes dans une liste de problèmes est «Voici quelques recommandations ».

Pour plus d’informations, consultez [Vue d’ensemble des affectations intelligentes](/help/quicksilver/manage-work/tasks/assign-tasks/smart-assignments.md).
