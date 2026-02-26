---
title: Améliorations des rapports pour le deuxième trimestre 2026
description: Améliorations des rapports pour le deuxième trimestre 2026
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 8bcea5cec9f68deacc5f89ca7703303a1b00769f
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 23%

---

# Améliorations des rapports pour le deuxième trimestre 2026

Cette page décrit les améliorations apportées aux rapports avec la version du deuxième trimestre 2026 dans l’environnement Aperçu. Ces améliorations seront rendues disponibles comme indiqué, dans l’environnement de production.

Pour obtenir la liste de toutes les modifications disponibles à ce stade du cycle de publication de la version du deuxième trimestre 2026, consultez la section [Vue d’ensemble de la version du deuxième trimestre 2026](/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-release-overview.md).

## Libellés de champ personnalisés affichés lors de la création de rapports

>[!NOTE]
>
>Aperçu : 26 février 2026
>Version rapide de production : vendredi 12 mars 2026
>Production pour tous : vendredi 16 avril 2026

Le libellé du champ personnalisé s’affiche désormais avant le nom du champ et l’objet dans les outils de création de rapports, ce qui vous permet de localiser plus facilement les champs. Les libellés des champs s’affichent également lors de la définition de filtres, de vues et de regroupements dans des listes.

Le libellé du champ personnalisé est destiné à l’interface système, tandis que le nom du champ est fréquemment utilisé à des fins d’API et de stockage back-end, et peut ne pas être aussi utile lors de la localisation d’un champ.

Pour plus d’informations, voir [Créer un rapport personnalisé](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

<!--

## Shareable Report Folders

>[!NOTE]
>
>Preview: February 26, 2026
>Production fast release: March 12, 2026
>Production for everyone: April 16, 2026

You can now organize and share reports using shareable report folders. This new feature helps teams that manage large volumes of reports maintain scalable and consistent access control:

* **Create organized folder structures**: System administrators can create top-level folders, and users with manage access can create subfolders up to 4 levels deep.
* **Granular permission controls**: Share folders with two permission levels:
   * View: Users can open reports and share folders
   * Manage: Users can edit folder details, add/remove items, and automatically receive manage access to all reports within the folder
* **Inherited permissions**: Permissions cascade from parent folders to all subfolders and reports within the folder tree
* **Enhanced list experience**: When you enable sharable folders, you will have access to the enhanced list experience. For more information, see [Use enhanced lists](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).


For more information, see [Use shareable report folders](/help/quicksilver/reports-and-dashboards/reports/report-usage/use-sharable-report-folders.md).

-->

## Amélioration des libellés de date pour les regroupements de graphiques dans les tableaux de bord Zone de travail

>[!NOTE]
>
>Aperçu : 26 février 2026
>Version rapide de production : vendredi 12 mars 2026
>Production pour tous : vendredi 16 avril 2026

Les graphiques qui regroupent les données par date affichent désormais des libellés de date plus clairs et plus lisibles. Grâce à cette mise à jour, les libellés de date s’ajustent dynamiquement en fonction de l’option Regrouper par sélectionnée (par jour, semaine, mois ou année, par exemple), ce qui facilite la lecture et l’interprétation des graphiques en un coup d’œil :

<table> <tbody> <tr> <td>Jour</td> <td>Affiche la date complète. Exemple : 3/12/2026</td> </tr> <tr> <td>Semaine</td> <td>Affiche une date de début de semaine formatée. Exemple : 8 Mars 2026</td> </tr> <tr> <td>Mois</td> <td>Affiche le mois et l’année. Exemple mars 2026</td> </tr> <tr> <td>Année</td> <td>Affiche l’année uniquement. Exemple : 2026</td> </tr> </tbody> </table>

Auparavant, les regroupements de graphiques affichaient toujours la date de début de la période sélectionnée au format numérique.


