---
content-type: release-notes
keywords: notes,trimestriel,mise à jour,version
navigation-topic: 2021-2-release-activity
title: Améliorations apportées à la gestion des ressources (version 21.2)
description: Cette page décrit toutes les améliorations apportées à la gestion des ressources avec la version 21.2 de l’environnement de prévisualisation. Ces améliorations seront disponibles dans l’environnement de production au cours de la semaine du 10 mai 2021. Pour obtenir la liste de toutes les modifications disponibles avec la version 21.2, voir Vue d’ensemble de la version 21.2.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 00133efe-f779-4217-87af-a223dcf043ee
TQID: https://experienceleague.adobe.com/cAM0R2azvfhRW25brnRKCUXZ5f2ZLGeBVd19okbdBpU
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2:
  - id: c33d85a1-be85-4290-854c-87408c10aa80
  - id: d1573eb8-a2e8-4a06-9526-9c3410bf4914
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 575
ht-degree: 100%

---

# Améliorations apportées à la gestion des ressources (version 21.2)

Cette page décrit toutes les améliorations apportées à la gestion des ressources avec la version 21.2 de l’environnement de prévisualisation. Ces améliorations seront disponibles dans l’environnement de production au cours de la semaine du 10 mai 2021. Pour obtenir la liste de toutes les modifications disponibles avec la version 21.2, voir [Vue d’ensemble de la version 21.2](../../../product-announcements/product-releases/21.2-release-activity/21-2-release-overview.md).

## Vue au niveau du mois dans l’équilibreur de charge de travail

Pour vous aider à gérer l’attribution des ressources sur des périodes plus longues, nous avons mis en place une vue au niveau du mois pour l’équilibreur de charge de travail. Vous pouvez afficher jusqu’à trois mois à la fois et mettre à jour les affectations de ressources mensuelles. Avant cette modification, vous ne pouviez afficher l’équilibreur de charge de travail que par jour ou par semaine.

Pour plus d’informations, voir [Naviguer dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Connexion entre le planificateur de scénarios, l’équilibreur de charge de travail et la liste des tâches

>[!NOTE]
>
>Disponible uniquement dans la nouvelle version d’Adobe Workfront.

Pour vous aider dans la planification stratégique de vos projets et vous assurer qu’ils s’alignent sur les initiatives les plus importantes du planificateur de scénarios, nous avons créé une nouvelle zone sur le projet qui affiche les exigences en matière de fonction des initiatives ainsi que le nombre d’heures prévues estimées sur les éléments de travail du projet. Cette zone est disponible pour l’équilibreur de charge de travail au niveau du projet ainsi que pour la liste des tâches de la nouvelle expérience Workfront. Dans l’expérience classique, cette option n’est disponible que pour l’équilibreur de charge de travail du projet.

Pour plus d’informations, voir les articles suivants :

* [Vue d’ensemble de la réconciliation des affectations de ressources entre les projets et les initiatives](../../../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).
* [Trouver l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)

>[!IMPORTANT]
>
>Cette nouvelle fonctionnalité est visible par tout le monde, que ce soit dans l’expérience Workfront nouvelle ou classique. Cela est également visible pour les clients et clientes qui n’ont pas acheté de licence de planificateur de scénarios Workfront.

## Utiliser des heures prévues lors du calcul des valeurs nettes dans le planificateur de ressources

Un nouveau paramètre du planificateur de ressources vous permet d’utiliser le nombre d’heures prévues lors du calcul des valeurs nettes.

Avant cette amélioration, Workfront calculait les valeurs nettes uniquement à partir des heures budgétées. Les valeurs nettes affichent la différence entre les heures prévues, budgétées et disponibles, l’équivalent temps complet et les coûts. Les heures budgétées restent le paramètre par défaut pour le calcul des valeurs nettes.

Pour plus d’informations, voir [Vue d’ensemble des informations sur les heures, les équivalents temps complet et les coûts dans les vues de Projet et Rôle du planificateur de ressources](../../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

## Vue sur 12 semaines dans l’équilibreur de charge de travail

Vous pouvez désormais afficher jusqu’à 12 semaines d’informations dans l’équilibreur de charge de travail. Avant cette amélioration, vous pouviez voir des informations sur 2, 4 et 6 semaines.

Pour plus d’informations sur l’affichage de l’équilibreur de charge de travail, voir [Naviguer dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)Naviguer dans l’équilibreur de charge de travail.

## Modifier le fonctionnement du filtre Fonction dans la zone Non affecté de l’équilibreur de charge de travail

Afin d’améliorer le fonctionnement du filtrage des fonctions dans l’équilibreur de charge de travail et de répondre aux attentes des utilisateurs et des utilisatrices, nous avons modifié la fonctionnalité du filtre dans la zone « Non affecté ». Vous pouvez désormais n’afficher que les heures affectées aux fonctions que vous avez spécifiées dans le filtre.

Avant cette amélioration, lors de l’application du filtre « Fonctions » à la zone « Non affecté », l’équilibreur de charge de travail affichait toutes les heures associées aux éléments de travail affectés aux fonctions.

Pour plus d’informations sur le filtrage des informations dans l’équilibreur de charge de travail, voir [Gérer des filtres dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).
