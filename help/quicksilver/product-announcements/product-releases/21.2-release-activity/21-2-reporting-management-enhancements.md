---
content-type: release-notes
keywords: notes,trimestriel,mise à jour,version
navigation-topic: 2021-2-release-activity
title: Améliorations apportées à la création de rapports (version 21.2)
description: Cette page décrit toutes les améliorations apportées à la création de rapports avec la version 21.2 de l’environnement de prévisualisation. Ces améliorations seront disponibles dans l’environnement de production au cours de la semaine du 10 mai 2021. Pour obtenir la liste de toutes les modifications disponibles avec la version 21.2, voir Vue d’ensemble de la version 21.2.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 1d5f76ef-bea7-4630-8051-454b0d109341
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 94%

---

# Améliorations apportées à la création de rapports (version 21.2)

Cette page décrit toutes les améliorations apportées à la création de rapports avec la version 21.2 de l’environnement de prévisualisation. Ces améliorations seront disponibles dans l’environnement de production au cours de la semaine du 10 mai 2021. Pour obtenir la liste de toutes les modifications disponibles avec la version 21.2, voir [Vue d’ensemble de la version 21.2](../../../product-announcements/product-releases/21.2-release-activity/21-2-release-overview.md).

## Limiter la modification des heures dans les projets et les rapports

Pour améliorer la gestion des modifications d’heures dans l’onglet « Heures » d’un projet et dans les rapports d’heures, nous avons introduit un paramètre permettant aux administrateurs et administratrices Workfront de restreindre les modifications d’heures aux seules personnes propriétaires d’heures et chargées de l’administration du système.

Auparavant, les utilisateurs et les utilisatrices dont le niveau d’accès permettait de modifier les feuilles de temps et les heures pouvaient modifier les heures.

Pour plus d’informations, voir [Configurer les préférences de feuille de temps et d’heure](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

## Nouvel aspect du champ Affectations dans les listes et rapports mis à jour

>[!NOTE]
>
>Cette fonctionnalité n’est disponible que dans la nouvelle version d’Adobe Workfront.

Afin qu’il corresponde mieux à l’aspect moderne des autres zones de la nouvelle expérience Workfront, le style a été modifié pour le champ Affectations dans les listes et les rapports mis à jour. Cette nouvelle conception comprend les éléments suivants :

* Avatar arrondi pour les photos de profil des utilisateurs et utilisatrices, les fonctions et les équipes
* Affichage des initiales pour les utilisateurs et utilisatrices sans photo de profil
* Nouvelle icône de fonction
* Nouvelle icône de personne pour les affectations avancées
* Nouvelle icône d’accès restreint
* Autres modifications mineures de la conception

Pour plus d’informations sur les affectations dans les listes, voir [Affecter des tâches](../../../manage-work/tasks/assign-tasks/assign-tasks.md) ou [Affecter des problèmes](../../../manage-work/issues/manage-issues/assign-issues.md).

![&#x200B; Mises à jour des affectations &#x200B;](assets/assignments-updates-350x193.png)

## Nouvel aspect des champs de saisie semi-automatique dans les listes et rapports mis à jour

>[!NOTE]
>
>Temporairement supprimé de l’environnement de production le 20 mai 2021.

>[!NOTE]
>
>Cette fonctionnalité n’est disponible que dans la nouvelle version d’Adobe Workfront.

Afin qu’il corresponde mieux à l’aspect moderne des autres zones de la nouvelle expérience Workfront, le style a été modifié pour le champ de saisie semi-automatique dans les listes et les rapports mis à jour. Ces modifications sont les suivantes :

* L’icône de saisie semi-automatique a été supprimée du champ.
* Lorsque vous cliquez sur un champ de saisie semi-automatique, le menu de suggestions s’affiche désormais avant que vous ne saisissiez le texte.
* Le menu des suggestions est plus réactif à la longueur des valeurs et celles-ci sont désormais tronquées à la fin, lorsque la limite de caractères est atteinte, au lieu d’être tronquées au milieu de la valeur.

Pour plus d’informations sur les listes mises à jour, voir la section [Différence entre les listes mises à jour et les listes héritées](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md#updated) dans l’article [Prise en main des listes dans Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

![Champ de saisie semi-automatique](assets/typeahead-updates-350x336.png)

## Créer des rapports sur les mises à jour système

Le nouveau rapport Entrée du journal offre une plus grande auditabilité en vous permettant d’analyser les mises à jour du système, notamment :

* Les changements de statut d’un projet, une tâche ou un problème
* Les tâches ou problèmes supprimés
* Les valeurs des champs personnalisés
* Les dates d’achèvement prévues
* Les changements de propriétaire du projet

Vous pouvez, par exemple, configurer ce rapport pour qu’il montre l’activité autour d’un champ personnalisé spécifique, y compris le projet du champ personnalisé, quand une valeur a été saisie pour la première fois, quelle était cette valeur, quand le champ a été mis à jour, quelle était la valeur précédente, quelle était la nouvelle valeur saisie, quels utilisateurs et quelles utilisatrices ont effectué ces actions, etc.

Auparavant, vous ne pouviez émettre des rapports sur les mises à jour du système que par l’intermédiaire de l’API Workfront.

Pour en savoir plus sur ce rapport et sur son utilisation, voir [Rapport sur la zone Mises à jour avec un rapport Entrée du journal](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

