---
content-type: release-notes
keywords: notes,trimestriel,mise à jour,version
navigation-topic: 2021-2-release-activity
title: 21. Améliorations de la création de rapports (version 21.2)
description: Cette page décrit toutes les améliorations apportées à la création de rapports avec la version 21.2 de l’environnement Aperçu. Ces améliorations seront disponibles dans l’environnement de production au cours de la semaine du 10 mai 2021. Pour obtenir la liste de toutes les modifications disponibles avec la version 21.2, reportez-vous à la présentation de la version 21.2.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 1d5f76ef-bea7-4630-8051-454b0d109341
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '542'
ht-degree: 3%

---

# 21. Améliorations de la création de rapports (version 21.2)

Cette page décrit toutes les améliorations apportées à la création de rapports avec la version 21.2 de l’environnement Aperçu. Ces améliorations seront disponibles dans l’environnement de production au cours de la semaine du 10 mai 2021. Pour obtenir la liste de toutes les modifications disponibles avec la version 21.2, consultez la [présentation de la version 21.2](../../../product-announcements/product-releases/21.2-release-activity/21-2-release-overview.md).

## Limitation de la modification horaire dans les projets et les rapports

Pour mieux contrôler la modification horaire sur l’onglet Heures d’un projet et les rapports Heure , nous avons ajouté un paramètre qui permet aux administrateurs de Workfront de limiter la modification horaire aux propriétaires d’heures et aux administrateurs système.

Auparavant, les utilisateurs dont les feuilles de calcul et heures étaient activées dans leur niveau d’accès pouvaient modifier les heures.

Pour plus d’informations, consultez [Configurer les préférences de feuilles de temps et d’heures](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

## Nouvelle apparence du champ Affectations dans les listes et rapports mis à jour

>[!NOTE]
>
>Cette fonctionnalité est disponible uniquement dans la nouvelle expérience Adobe Workfront.

Pour correspondre à l’aspect moderne d’autres zones de la nouvelle expérience Workfront, le style du champ Affectations a été modifié dans les listes et les rapports mis à jour. Cette reconception comprend :

* Un avatar arrondi pour les images de profil utilisateur, les rôles de tâche et les équipes
* Affichage initial pour les utilisateurs sans images de profil
* Icône Nouveau rôle de tâche
* Une nouvelle icône Personnes pour les affectations avancées
* Une nouvelle icône Accès restreint
* Autres changements de conception mineurs

Pour plus d’informations sur les affectations dans les listes, voir [Affecter des tâches](../../../manage-work/tasks/assign-tasks/assign-tasks.md) ou [Affecter des problèmes](../../../manage-work/issues/manage-issues/assign-issues.md).

![](assets/assignments-updates-350x193.png)

## Nouvelle apparence des champs de saisie anticipée dans les listes et rapports mis à jour

>[!NOTE]
>
>temporairement supprimé de l’environnement de production le 20 mai 2021.

>[!NOTE]
>
>Cette fonctionnalité est disponible uniquement dans la nouvelle expérience Adobe Workfront.

Pour correspondre à l’aspect moderne d’autres zones de la nouvelle expérience Workfront, la mise en forme des champs de saisie anticipée a été modifiée dans les listes et les rapports mis à jour. Ces modifications incluent :

* L’icône Paire de texte a été supprimée du champ.
* Lorsque vous cliquez sur un champ de saisie anticipée, le menu des suggestions s’affiche maintenant avant de saisir du texte.
* Le menu de suggestions est plus réactif à la longueur des valeurs. Ces valeurs sont désormais tronquées à la fin lorsque la limite de caractères est atteinte et non au milieu de la valeur.

Pour plus d’informations sur les listes mises à jour, voir la section [Différence entre les listes mises à jour et héritées](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md#updated) de l’article [Prise en main des listes dans Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

![](assets/typeahead-updates-350x336.png)

## Rapport sur les mises à jour système

Le nouveau rapport Entrée de journal offre une plus grande visibilité en vous permettant d’analyser les mises à jour du système, notamment :

* Changements d’état sur un projet, une tâche ou un problème
* Tâches ou problèmes supprimés
* Valeurs des champs personnalisés
* Dates d’achèvement prévues
* Modifications du propriétaire du projet

Vous pouvez, par exemple, configurer ce rapport afin d’afficher l’activité autour d’un champ personnalisé spécifique, y compris le projet du champ personnalisé, le moment où une valeur a été saisie pour la première fois, ce que était cette valeur, quand le champ a été mis à jour, quelle était la valeur précédente, quelle était la valeur nouvellement saisie, quels utilisateurs ont effectué ces actions, etc.

Auparavant, vous pouviez créer des rapports sur les mises à jour du système uniquement via l’API Workfront.

Pour en savoir plus sur ce rapport et son utilisation, consultez la section [Rapport sur la zone des mises à jour](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

