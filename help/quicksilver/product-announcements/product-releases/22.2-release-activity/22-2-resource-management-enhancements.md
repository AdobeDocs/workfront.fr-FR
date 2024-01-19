---
title: 2.2 Améliorations de la gestion des ressources
description: 2.2 Améliorations de la gestion des ressources
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 5f11c43c-3aa8-4135-b6bf-07b9993e63d9
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 0%

---

# 2.2 Améliorations de la gestion des ressources

Cette page décrit toutes les améliorations apportées à la gestion des ressources avec la version 22.2 de l’environnement Aperçu. Ces améliorations seront disponibles dans l’environnement de production.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

la semaine du 4 avril 2022.

Pour obtenir la liste de toutes les modifications disponibles avec la version 22.2, voir [Présentation de la version 2.2.2](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md).

## Amélioration de la navigation de l’équilibreur de charge de travail

Pour améliorer votre expérience lors de l’utilisation de l’équilibreur de charge de travail, nous avons introduit les améliorations suivantes :

* Les boutons Annuler et Enregistrer lors de l’ajustement des allocations sont désormais collants, même si la tâche est plus longue que la période incluse à l’écran ou lorsque le panneau Résumé s’affiche.
* Le panneau de gauche qui affiche les noms des utilisateurs et des éléments de travail est maintenant collant. Il vous permet de faire défiler horizontalement les éléments pendant plus longtemps et de toujours pouvoir lire les noms des éléments répertoriés dans le panneau.
* Vous pouvez réduire et développer tous les éléments répertoriés dans le panneau de gauche d’un seul clic au lieu de l’utilisateur ou du projet.
* Le panneau de gauche peut désormais également être redimensionné.
* Il existe désormais un mode plein écran pour l’équilibreur de charge de travail.

Pour plus d’informations sur la navigation dans l’équilibreur de charge de travail, voir [Navigation dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Accès aux affectations avancées dans l’équilibreur de charge de travail

Pour faciliter l’affectation des tâches et la rendre plus précise, vous pouvez désormais effectuer des affectations avancées lorsque vous attribuez des tâches manuellement dans l’équilibreur de charge de travail. Avant cette amélioration, vous pouviez accéder aux affectations avancées lors de la modification d’éléments, à partir des en-têtes des éléments ou dans des listes.

Pour plus d’informations, voir [Affectation manuelle du travail à l’aide de l’équilibreur de charge](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-manually.md).

## Nouvelle formule de calcul de la disponibilité de l’utilisateur lorsque la préférence Planification par défaut est sélectionnée

Pour fournir des informations plus précises dans les outils de gestion des ressources, nous avons modifié la formule utilisée par Workfront pour calculer la disponibilité des utilisateurs lorsque l’administrateur de Workfront sélectionne Le planning par défaut dans les préférences de gestion des ressources. Avec la nouvelle mise à jour, Workfront utilise la formule suivante pour calculer la disponibilité de l’utilisateur :

Heures disponibles de l’utilisateur = (Heures de planification par défaut - Exceptions) &#42; ETR - Heures de désactivation

Avant cette mise à jour, Workfront utilisait la formule suivante pour calculer la disponibilité de l’utilisateur lorsque la planification par défaut était sélectionnée :

Heures disponibles de l’utilisateur = (Heures de planification par défaut - (exceptions de planification + heures de congé)) &#42; Valeur FTE de l’utilisateur

Pour plus d’informations, voir [Configuration des préférences de gestion des ressources](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

