---
content-type: release-notes
navigation-topic: 2019-2-release-activity
title: Améliorations de projet 2019.2
description: Cette page décrit toutes les améliorations de projet incluses dans la version 2019.2. Cette fonctionnalité devrait être disponible dans l’environnement de production au cours de la semaine du 20 mai 2019.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 76292f90-af1a-4740-9b8e-b02a6303625c
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '731'
ht-degree: 100%

---

# Améliorations de projet 2019.2

Cette page décrit toutes les améliorations de projet incluses dans la version 2019.2. Cette fonctionnalité devrait être disponible dans l’environnement de production au cours de la semaine du 20 mai 2019.

Pour consulter la liste de toutes les modifications apportées à la version 2019.2, voir [Vue d’ensemble de l’activité de version 2019.2](../../../../product-announcements/product-releases/quarterly-release-archive/2019.2-release-activity/2019-2-release-activity-overview.md).

## Rechercher des groupes plus rapidement lors de la personnalisation des statuts

Le menu déroulant de l’onglet Statuts de la zone Configuration est désormais un menu de saisie semi-automatique. Cela vous permet de rechercher rapidement n’importe quel groupe dans le système, ce qui facilite la personnalisation des statuts.

Auparavant, le menu déroulant affichait un nombre limité de groupes. Si le groupe souhaité ne s’affichait pas, vous deviez accéder à Configuration > Groupes et rechercher le groupe spécifique afin de personnaliser les statuts du groupe.

Pour plus d’informations, voir [Créer ou modifier un statut](../../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

## Joindre des formulaires perspnnalisés et des processus d’approbation personnalisés par défaut aux tâches

Vous pouvez désormais configurer des formulaires personnalisés et des processus d’approbation par défaut à joindre aux tâches lorsque vous ajoutez des tâches à un projet. Vous pouvez configurer les paramètres par défaut au niveau du projet.

Pour plus d’informations sur la configuration des formulaires personnalisés et des processus d’approbation par défaut pour les tâches au niveau du projet, reportez-vous à la section « Tâches » de l’article [Modifier des projets](../../../../manage-work/projects/manage-projects/edit-projects.md).

## Afficher la ligne entière d’une tâche parent en gras dans une liste de tâches

Dans une liste de tâches, la ligne contenant une tâche parent est affichée en gras. Cette modification est visible lorsque la liste est triée par la structure de répartition du travail ou par le numéro de la tâche dans l’ordre croissant.

## Annuler des modifications dans les listes de tâches

Un nouveau bouton d’enregistrement automatique dans la liste des tâches vous permet de choisir si vous voulez que les modifications que vous apportez soient automatiquement enregistrées ou si vous voulez voir les effets de vos modifications avant de les enregistrer. Ce paramètre s’applique à la fois à la liste des tâches et au graphique de Gantt.

Avant cette amélioration, toutes les modifications étaient toujours enregistrées automatiquement.

Pour plus d’informations sur la modification des tâches dans une liste de tâches, voir [Modifier les tâches](../../../../manage-work/tasks/manage-tasks/edit-tasks.md).

Pour plus d’informations sur la modification des tâches dans le graphique de Gantt, voir [Mettre à jour les informations de la liste des tâches dans le graphique Gantt](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md).

## Nouvelles valeurs par défaut de la largeur des colonnes dans les nouvelles listes

Désormais, Workfront ajuste automatiquement la largeur des colonnes en fonction des informations valueformat contenues dans chaque colonne. Par exemple, les colonnes qui affichent un nombre sont plus larges que celles qui affichent le champ Description.

Avant cette amélioration, la largeur des colonnes dans les nouvelles vues des projets et des tâches était fixée à 100 pixels, sauf indication contraire.

Pour plus d’informations sur la largeur des colonnes, voir [Modifier la largeur et l’ordre des colonnes](../../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

## Désactiver les objets inutilisés

>[!NOTE]
>
>Cette fonctionnalité a été publiée directement dans l’environnement de production au cours de la période de version préliminaire 2019.2.

Si vous avez des objets qui ne sont plus utilisés, vous pouvez désormais les désactiver pour les masquer dans les listes afin d’éviter que les utilisateurs ou utilisatrices ne les associent à d’autres objets.

Désormais, lorsque vous modifiez l’un des objets ci-dessous, vous pouvez indiquer s’il doit être actif. Les objets définis comme actifs apparaissent dans les menus déroulants et les champs de saisie et peuvent être attachés à d’autres objets. Les objets qui ne sont pas définis sur Actif ne sont pas visibles dans les menus déroulants et les champs de saisie permettant de les joindre à d’autres objets.

* Processus d’approbation
* Entreprises
* Formulaires personnalisés
* Chemins jalonnés
* Portefeuilles
* Programmes
* Modèles

Tout ce que vous désactivez et qui est actuellement utilisé continue de fonctionner comme avant et n’est pas supprimé ou bloqué.

>[!IMPORTANT]
>
>Lors de la création de ces objets via l’API Workfront, la valeur par défaut du paramètre « isActive » est « true ». Il s’agit d’un nouveau champ pour tous les objets et il n’est pas possible de le modifier avant la version 11 de l’API. Ce champ existait auparavant pour les portfolios, mais la valeur par défaut était « false ». Il prendra la valeur « true » par défaut à partir de la version 11 de l’API.

## Afficher le coût budgété du travail prévu (BCWS) et effectué (BCWP) dans les vues

Vous pouvez désormais afficher le coût budgété du travail prévu (BCWS) et le coût budgété du travail effectué (BCWP) dans les vues des projets et des tâches.

Bien que ces mesures de performances des projets aient été utilisées dans les calculs financiers de Workfront auparavant, elles n’étaient pas visibles dans le système avant cette amélioration.

Pour plus d’informations sur le calcul du BCWS, voir [Calculer le coût budgété du travail prévu (BCWS)](../../../../manage-work/projects/project-finances/calculate-bcws.md).

Pour plus d’informations sur le calcul du BCWP, voir [Calculer le coût budgété du travail effectué (BCWP)](../../../../manage-work/projects/project-finances/calculate-bcwp.md).

