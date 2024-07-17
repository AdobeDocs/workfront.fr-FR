---
content-type: release-notes
navigation-topic: 2019-2-release-activity
title: Améliorations des projets (version 2019.2)
description: Cette page décrit toutes les améliorations de projet incluses dans la version 2019.2. Cette fonctionnalité devrait être disponible dans l’environnement de production au cours de la semaine du 20 mai 2019.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 76292f90-af1a-4740-9b8e-b02a6303625c
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '731'
ht-degree: 2%

---

# Améliorations des projets (version 2019.2)

Cette page décrit toutes les améliorations de projet incluses dans la version 2019.2. Cette fonctionnalité devrait être disponible dans l’environnement de production au cours de la semaine du 20 mai 2019.

Pour obtenir la liste de toutes les modifications apportées à la version 2019.2, consultez la [présentation de l’activité de version 2019.2](../../../../product-announcements/product-releases/quarterly-release-archive/2019.2-release-activity/2019-2-release-activity-overview.md).

## Recherche De Groupes Plus Rapide Lors De La Personnalisation Des Statuts

Le menu déroulant de l’onglet Statuts de la zone Configuration est désormais un menu de type . Cela vous permet de rechercher rapidement n’importe quel groupe dans le système, ce qui facilite la personnalisation des états.

Auparavant, le menu déroulant affichait un nombre limité de groupes. Si le groupe souhaité ne s’affichait pas, vous deviez accéder à Configuration > Groupes et rechercher le groupe spécifique afin de personnaliser les états du groupe.

Pour plus d’informations, voir [Création ou modification d’un état](../../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

## Joindre les processus Forms et d’approbation personnalisés par défaut aux tâches

Vous pouvez désormais configurer des formulaires personnalisés et des processus d’approbation par défaut à joindre aux tâches lorsque vous ajoutez des tâches à un projet. Vous pouvez configurer les paramètres par défaut au niveau du projet.

Pour plus d’informations sur la configuration des formulaires personnalisés par défaut et les processus d’approbation pour les tâches au niveau du projet, reportez-vous à la section &quot;Tâches&quot; de l’article [Modifier les projets](../../../../manage-work/projects/manage-projects/edit-projects.md) .

## Affichage de la ligne entière d’une tâche parente en gras dans une liste de tâches

Dans une liste de tâches, la ligne contenant une tâche parent est affichée en gras. Cette modification est visible lorsque la liste est triée par la structure Répartition du travail ou par Numéro de la tâche dans l’ordre croissant.

## Modifications inversées sur les listes de tâches

Un nouveau bouton d’enregistrement automatique dans la liste des tâches vous permet de choisir si vous souhaitez que les modifications que vous apportez soient automatiquement enregistrées ou si vous souhaitez voir les effets que vos modifications produisent avant de les enregistrer. Ce paramètre s’applique à la fois à la liste des tâches et au diagramme de Gantt.

Avant cette amélioration, toutes les modifications étaient toujours enregistrées automatiquement.

Pour plus d’informations sur l’édition de tâches dans une liste de tâches, voir [Modifier les tâches](../../../../manage-work/tasks/manage-tasks/edit-tasks.md).

Pour plus d’informations sur la modification des tâches dans le diagramme de Gantt, voir [Mise à jour d’informations dans la liste de tâches du diagramme de Gantt](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md).

## Nouvelles valeurs par défaut de la largeur des colonnes dans les nouvelles listes

Désormais, Workfront ajuste automatiquement la largeur des colonnes en fonction des informations de format de valeur de chaque colonne. Par exemple, les colonnes qui affichent un nombre sont plus larges que celles qui affichent le champ Description .

Avant cette amélioration, les largeurs de colonne dans les nouvelles vues de projet et de tâche étaient définies sur 100 pixels, sauf indication contraire.

Pour plus d’informations sur les largeurs de colonne, voir [Modification de la largeur et de l’ordre des colonnes](../../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

## Désactivation des objets inutilisés

>[!NOTE]
>
>Cette fonctionnalité a été publiée directement dans l’environnement de production au cours de la période d’aperçu 2019.2.

Si des objets ne sont plus utilisés, vous pouvez les désactiver pour les masquer des listes afin d’empêcher les utilisateurs de les associer à d’autres objets.

Désormais, lorsque vous modifiez l’un des objets ci-dessous, vous pouvez indiquer s’ils doivent être actifs. Les objets définis sur Actif s’affichent dans des menus déroulants et des champs de type avant et peuvent être associés à d’autres objets. Les objets qui ne sont pas définis sur Actif ne sont pas visibles dans les menus déroulants et les champs de type devant à joindre à d’autres objets.

* Processus d’approbation
* Entreprises
* Formulaires personnalisés
* Chemins jalonnés
* Portefeuilles
* Programmes
* Modèles

Tout ce que vous désactivez et qui est actuellement utilisé continue de fonctionner comme toujours, et n’est ni supprimé ni bloqué.

>[!IMPORTANT]
>
>Lors de la création de ces objets via l’API Workfront, la valeur par défaut du paramètre &quot;isActive&quot; est true. Il s’agit d’un nouveau champ pour tous les objets. Vous ne pouvez pas le modifier avant la version 11 de l’API. Ce champ existait auparavant pour le Portfolio, sauf que la valeur par défaut était false ; il passera à la valeur par défaut true à partir de la version 11 de l’API.

## Afficher le coût des travaux planifiés (BCWS) et exécutés (BCWP) dans les vues

Vous pouvez désormais afficher le Coût planifié des travaux (BCWS) et le Coût budgété des travaux réalisés (BCWP) dans les vues de projet et de tâche.

Bien que ces mesures de performances de projet aient été utilisées auparavant dans les calculs financiers dans Workfront, elles n’étaient pas visibles dans le système avant cette amélioration.

Pour plus d&#39;informations sur le calcul du BCWS, voir [Calculer le coût du travail planifié (BCWS)](../../../../manage-work/projects/project-finances/calculate-bcws.md).

Pour plus d&#39;informations sur le calcul du BCWP, voir [Calculer le coût du travail effectué dans la budget (BCWP)](../../../../manage-work/projects/project-finances/calculate-bcwp.md).

