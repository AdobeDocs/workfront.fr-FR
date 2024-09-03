---
title: Améliorations apportées à l’administration du quatrième trimestre 2023
description: Améliorations apportées à l’administration du quatrième trimestre 2023
author: Lisa
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 7ed37978-b821-488e-9ca1-b81825255be3
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 100%

---

# Améliorations apportées à l’administration du quatrième trimestre 2023

Cette page décrit toutes les améliorations apportées à l’administration dans l’environnement de prévisualisation par la version du quatrième trimestre 2023. Ces améliorations ont été apportées à l’environnement de production avec la version 23.10.

Pour une liste de tous les changements disponibles à ce stade du cycle de publication de la version du quatrième trimestre 2023, voir [Vue d’ensemble de la version du quatrième trimestre 2023](/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md).

## Décisions relatives aux épreuves et documents disponibles pour la clientèle utilisant les modèles de licence hérités

La clientèle héritée qui n’a pas encore migré vers le nouveau modèle de licence Adobe Workfront peut désormais afficher les données relatives au nombre de décisions en matière d’épreuves/documents par personne et par mois, dans un rapport unique. Ces données sont disponibles lorsque vous exécutez un rapport Décisions des utilisateurs et utilisatrices.

Pour plus d’informations, voir [Comprendre les objets dans Adobe Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) et [Afficher le nombre de décisions relatives aux épreuves et aux documents pour tous les utilisateurs et utilisatrices](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/view-number-of-decisions-for-users.md).

## Les champs calculés sur les formulaires personnalisés peuvent désormais utiliser le caractère générique $$USER.

Le caractère générique `$$USER` est désormais disponible dans les champs personnalisés calculés et les champs de recherche externes du nouveau créateur de formulaire. Le fait de référencer `$$USER` dans un calcul ajoute l’identifiant de la personne actuelle. Vous pouvez également utiliser le caractère générique avec un autre champ. Par exemple, `$$USER.{name}` ajoute le nom de la personne actuelle.

Pour plus d’informations sur les champs calculés, voir [Ajouter des champs calculés avec le créateur de formulaires](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

## Ajouter des options de valeur d’une API externe à un formulaire personnalisé

Un nouveau type de champ, **Recherche externe**, est désormais disponible sur le créateur de formulaire personnalisé. Lorsque des données sont stockées sur un système externe, ce type de champ vous permet de charger des options à partir d’une API externe et de filtrer selon d’autres valeurs de champ dans le formulaire personnalisé.

Lorsque le formulaire est ajouté à un objet, les valeurs renvoyées par l’API apparaissent dans un champ déroulant et la personne peut en sélectionner une.

>[!NOTE]
>
>Le nouveau type de champ **Recherche externe** n’est pas disponible sur le créateur de formulaires hérité.

Pour plus d’informations, voir [Concevoir un formulaire avec le créateur de formulaire](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
