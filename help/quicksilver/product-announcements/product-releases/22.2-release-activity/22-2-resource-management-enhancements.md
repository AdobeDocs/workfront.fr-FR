---
title: 22.2 Améliorations de la gestion des ressources
description: 22.2 Améliorations de la gestion des ressources
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 5f11c43c-3aa8-4135-b6bf-07b9993e63d9
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 100%

---

# 22.2 Améliorations de la gestion des ressources

Cette page décrit toutes les améliorations apportées à la gestion des ressources avec la version 22.2 de l’environnement de prévisualisation. Ces améliorations seront disponibles dans l’environnement de production.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

La semaine du 4 avril 2022.

Pour obtenir la liste de toutes les modifications disponibles avec la version 22.2, voir [Présentation de la version 22.2](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md).

## Améliorations apportées à la navigation dans l’équilibreur de charge de travail

Afin d’améliorer votre expérience lors de l’utilisation de l’équilibreur de charge de travail, nous avons introduit les améliorations suivantes :

* Les boutons Annuler et Enregistrer lors de l’ajustement des affectations sont désormais flottants, même lorsque la tâche est plus longue que le délai indiqué à l’écran ou lorsque le panneau Résumé s’affiche.
* Le panneau de gauche qui affiche les noms des utilisateurs et utilisatrices et des éléments de travail est désormais flottant, ce qui vous permet de faire défiler les pages horizontalement sur des périodes plus longues tout en conservant la possibilité de lire les noms des éléments énumérés dans le panneau.
* Vous pouvez réduire et développer tous les éléments répertoriés dans le panneau de gauche en un seul clic au lieu de le faire à l’échelle de l’utilisateur et de l’utilisatrice ou du projet.
* En outre, le panneau de gauche est désormais redimensionnable.
* Il existe désormais un mode plein écran pour l’équilibreur de charge de travail.

Pour plus d’informations sur la navigation dans l’équilibreur de charge de travail, voir [Naviguer dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Accéder aux affectations avancées dans l’équilibreur de charge de travail

Pour faciliter l’affectation des éléments de travail et la rendre plus précise, vous pouvez désormais procéder à des affectations avancées lorsque vous attribuez manuellement des éléments de travail dans l’équilibreur de charge de travail. Avant cette amélioration, vous pouviez accéder aux affectations avancées lors de la modification des éléments, à partir de l’en-tête des éléments ou dans les listes.

Pour plus d’informations, voir [Affecter manuellement du travail à l’aide de l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-manually.md).

## Nouvelle formule de calcul de la disponibilité de l’utilisateur ou de l’utilisatrice lorsque la préférence Planning par défaut est sélectionnée.

Afin de fournir des informations plus précises dans les outils de gestion des ressources, nous avons modifié la formule utilisée par Workfront pour calculer la disponibilité des utilisateurs et utilisatrices lorsque l’administrateur ou l’administratrice Workfront sélectionne le Planning par défaut dans les préférences de gestion des ressources. Avec la nouvelle mise à jour, Workfront utilise la formule suivante pour calculer la disponibilité des utilisateurs et utilisatrices :

Heures disponibles de l’utilisateur ou de l’utilisatrice = (Heures de planning par défaut - Exceptions) &#42; Équivalent temps complet - Heures de congés

Avant cette mise à jour, Workfront utilisait la formule suivante pour calculer la disponibilité des utilisateurs et utilisatrices lorsque le planning par défaut était sélectionné :

Heures disponibles de l’utilisateur ou l’utilisatrice = (Heures de planning par défaut - (Exceptions d’horaire + Heures de congés)) &#42; Valeur de l’équivalent temps complet de l’utilisateur ou l’utilisatrice

Pour plus d’informations, voir [Configurer les préférences de gestion des ressources](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

