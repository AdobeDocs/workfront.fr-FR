---
title: Améliorations des rapports pour le quatrième trimestre 2026
description: Améliorations des rapports pour le quatrième trimestre 2026
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 63bdc885983f60c316409c3bba400ad82d475a5f
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 4%

---

# Améliorations des rapports pour le quatrième trimestre 2026

Cette page décrit les améliorations apportées aux rapports avec la version du quatrième trimestre 2026 dans l’environnement Aperçu. Ces améliorations seront rendues disponibles comme indiqué, dans l’environnement de production.

Pour obtenir la liste de toutes les modifications disponibles à ce stade du cycle de publication du quatrième trimestre 2026, voir [présentation de la version du quatrième trimestre 2026](/help/quicksilver/product-announcements/product-releases/26-q4-release-activity/26-q4-release-overview.md).

## Rapports de tableau croisé dynamique dans les tableaux de bord de la zone de travail

>[!NOTE]
>
>Aperçu : 27 août 2026
>Mise à jour rapide de la production : 17 septembre 2026
>Production pour tous : 15 octobre 2026

Le nouveau type de rapport de tableau croisé dynamique des tableaux de bord de la zone de travail agrège les données avec des déploiements complets et précis. Vous pouvez créer des mesures telles que les nombres, les sommes et les moyennes directement sur votre tableau de bord, puis accéder aux enregistrements sous-jacents derrière un total.

Pour plus d&#39;informations, voir [Créer un rapport de tableau croisé dynamique dans un tableau de bord Zone de travail](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-pivot-table-report.md).

## Application de dates de fin aux rapports planifiés

>[!NOTE]
>
>Aperçu : 13 août 2026
>Mise à jour rapide de la production : 17 septembre 2026
>Production pour tous : 15 octobre 2026

Les rapports planifiés requièrent désormais une date de fin pour empêcher une diffusion indéfinie. Les plannings dont la date de fin est dépassée sont automatiquement désactivés.

Les plannings existants ont été mis à jour avec des dates de fin pour améliorer la fiabilité et réduire l’utilisation inutile du système. Workfront offre également une visibilité accrue et des avertissements pour vous aider à gérer les cycles de vie des planifications de rapports à l’approche de leur date de fin.

Pour plus d’informations, voir [Planification de la diffusion automatique des rapports](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md).

## Les champs de référence natifs sont disponibles pour les listes et les rapports

>[!NOTE]
>
>Aperçu : 30 juillet 2026
>Version rapide de production : 13 août 2026
>Production pour tous : 15 octobre 2026

Vous pouvez désormais ajouter des champs de référence natifs aux listes et aux rapports dans Workfront.

Un champ de référence natif est un champ personnalisé. Lorsque le champ se trouve sur un formulaire personnalisé joint à un objet, le champ est renseigné à partir des données d’objet. Par exemple, si le champ fait référence au champ Description et s’il figure sur un formulaire personnalisé joint à un projet, il extrait la description du projet. (Le champ peut afficher « S.O. » si aucune donnée n’est disponible.)

Pour plus d’informations sur la création de champs de référence natifs, y compris la liste des champs natifs pris en charge, voir [Créer un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
Pour plus d’informations sur l’ajout de champs aux rapports, voir [Créer un rapport personnalisé](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Ordre cohérent des valeurs de champ à sélection multiple dans les listes et rapports hérités

>[!NOTE]
>
>Aperçu : 30 juillet 2026
>Version rapide de production : 13 août 2026
>Production pour tous : 15 octobre 2026

Les options sélectionnées pour les champs personnalisés à sélection multiple s’affichent désormais dans un ordre cohérent et prévisible sur les listes et rapports hérités. L’ordre des champs est déterminé par la manière dont les champs sont organisés dans le formulaire personnalisé.

![L’ordre des champs de formulaire personnalisé correspond à l’ordre des valeurs sélectionnées dans une liste ou un rapport](assets/new-field-order-multi-select.png)

Auparavant, les options sélectionnées s’affichaient dans l’ordre dans lequel vous les aviez choisies ou dans un ordre incohérent, ce qui rendait les lignes plus difficiles à analyser et à comparer.

Remarque : le nouveau tri ne s’applique pas si le champ utilise le mode texte.
