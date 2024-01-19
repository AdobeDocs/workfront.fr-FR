---
content-type: release-notes
keywords: notes,trimestriel,mise à jour,version
navigation-topic: 2021-2-release-activity
title: 21.2 Améliorations de la gestion des ressources
description: Cette page décrit toutes les améliorations apportées à la gestion des ressources avec la version 21.2 de l’environnement Aperçu. Ces améliorations seront disponibles dans l’environnement de production au cours de la semaine du 10 mai 2021. Pour obtenir la liste de toutes les modifications disponibles avec la version 21.2, reportez-vous à la présentation de la version 21.2.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 00133efe-f779-4217-87af-a223dcf043ee
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 0%

---

# 21.2 Améliorations de la gestion des ressources

Cette page décrit toutes les améliorations apportées à la gestion des ressources avec la version 21.2 de l’environnement Aperçu. Ces améliorations seront disponibles dans l’environnement de production au cours de la semaine du 10 mai 2021. Pour obtenir la liste de toutes les modifications disponibles avec la version 21.2, voir [Présentation de la version 21.2](../../../product-announcements/product-releases/21.2-release-activity/21-2-release-overview.md).

## Vue au niveau du mois dans l’équilibreur de charge

Pour vous aider à gérer l’affectation des ressources pendant de plus longues périodes, nous avons maintenant mis en oeuvre une vue de niveau mois pour l’équilibreur de charge de travail. Vous pouvez afficher jusqu’à trois mois à la fois et mettre à jour les allocations de ressources mensuelles. Avant cette modification, vous ne pouviez afficher l’équilibreur de charge de travail que par jour ou par semaine.

Pour plus d’informations, voir [Navigation dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Connexion entre le planificateur de scénario, l’équilibreur de charge de travail et la liste des tâches

>[!NOTE]
>
>Disponible uniquement dans la nouvelle expérience Adobe Workfront.

Pour vous aider à planifier vos projets de manière stratégique et à vous assurer qu’ils s’alignent sur les initiatives du planificateur de scénario, nous avons créé une nouvelle zone du projet qui affiche les exigences en termes de rôle professionnel des initiatives, ainsi que les heures prévues estimées sur les éléments de travail du projet. Cette zone est disponible pour l’équilibreur de charge de travail au niveau du projet ainsi que pour la liste des tâches de la nouvelle expérience Workfront. Dans l’expérience classique, cette option est disponible uniquement pour l’équilibreur de charge de travail du projet.

Pour plus d’informations, voir les articles suivants :

* [Présentation de la réconciliation des allocations de ressources entre les projets et les initiatives](../../../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).
* [Navigation dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)

>[!IMPORTANT]
>
>Cette nouvelle fonctionnalité est visible par tous les utilisateurs, que ce soit dans l’expérience Workfront nouvelle ou classique. Cela est également visible pour les clients qui n’ont pas acheté de licence de planificateur de scénario Workfront.

## Utilisation des heures planifiées lors du calcul des valeurs nettes dans le planificateur de ressources

Un nouveau paramètre du planificateur de ressources vous permet d’utiliser les heures planifiées lors du calcul des valeurs nettes.

Avant cette amélioration, Workfront calculait les valeurs nettes uniquement à l’aide des heures budgétées. Les valeurs nettes affichent la différence entre les heures disponibles et budgétées ou planifiées, l’éditeur de texte enrichi ou le coût. La valeur Hours budgétés reste le paramètre par défaut lors du calcul des valeurs nettes.

Pour plus d’informations, voir [Vue d’ensemble des heures, de l’éditeur de texte enrichi et des coûts dans les vues Projet et Rôle du planificateur de ressources](../../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

## Vue de 12 semaines dans l’équilibreur de charge de travail

Vous pouvez désormais afficher jusqu’à 12 semaines d’informations dans l’équilibreur de charge de travail. Avant cette amélioration, vous pouviez afficher 2, 4 et 6 semaines d’informations.

Pour plus d’informations sur l’affichage de l’équilibreur de charge de travail, voir [Navigation dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)Accédez à l’équilibreur de charge de travail.

## Modification du fonctionnement du filtre Rôle de tâche dans la zone Non affecté de l’équilibreur de charge de travail

Pour améliorer le fonctionnement du filtre Rôle de tâche dans l’équilibreur de charge de travail et répondre aux attentes des utilisateurs, nous avons modifié la fonctionnalité du filtre dans la zone Non affecté. Vous pouvez désormais afficher uniquement les heures allouées aux rôles de tâche que vous spécifiez dans le filtre.

Avant cette amélioration, lorsque vous appliquez le filtre Rôle de tâche à la zone Non affecté , l’équilibreur de charge de travail affichait toutes les heures associées aux tâches affectées aux rôles de tâche .

Pour plus d’informations sur le filtrage des informations dans l’équilibreur de charge de travail, voir [Gestion des filtres dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).
