---
title: Améliorations apportées aux administrateurs au quatrième trimestre 2023
description: Améliorations apportées aux administrateurs au quatrième trimestre 2023
author: Lisa
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 7ed37978-b821-488e-9ca1-b81825255be3
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 3%

---

# Améliorations apportées aux administrateurs au quatrième trimestre 2023

Cette page décrit toutes les améliorations apportées à l’administrateur à la version du quatrième trimestre 2023 de l’environnement Aperçu. Ces améliorations ont été apportées à l’environnement de production avec la version 23.10.

Pour obtenir la liste de toutes les modifications disponibles à ce stade du cycle de publication du quatrième trimestre 2023, consultez la [présentation de la version du quatrième trimestre 2023](/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md).

## BAT et décisions de document disponibles pour les clients de modèles de licence hérités

Les clients hérités qui n’ont pas encore migré vers le nouveau modèle de licence Adobe Workfront peuvent désormais afficher dans un seul rapport les données avec le nombre de décisions de BAT/document par utilisateur et par mois. Ces données sont disponibles lorsque vous exécutez un rapport Décisions d’utilisateur .

Pour plus d’informations, voir [Comprendre les objets dans Adobe Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) et [Afficher le nombre de décisions de BAT et de document pour tous les utilisateurs](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/view-number-of-decisions-for-users.md).

## Les champs calculés sur les formulaires personnalisés peuvent désormais utiliser le caractère générique $$USER

Le caractère générique `$$USER` est désormais disponible dans les champs personnalisés calculés et les champs de recherche externes du nouveau concepteur de formulaire. Le référencement de `$$USER` dans un calcul ajoute l’identifiant de l’utilisateur actuel. Vous pouvez également utiliser le caractère générique avec un autre champ. Par exemple, `$$USER.{name}` ajouterait le nom de l’utilisateur actuel.

Pour plus d’informations sur les champs calculés, voir [Ajout de champs calculés avec le concepteur de formulaire](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

## Ajout d’options de valeur d’une API externe à un formulaire personnalisé

Un nouveau type de champ, **Recherche externe**, est désormais disponible sur le concepteur de formulaire personnalisé. Lorsque des données sont stockées sur un système externe, ce type de champ vous permet de charger des options à partir d’une API externe et de filtrer selon d’autres valeurs de champ dans le formulaire personnalisé.

Lorsque le formulaire est ajouté à un objet, les valeurs renvoyées par l’API apparaissent dans un champ déroulant et l’utilisateur peut en sélectionner une.

>[!NOTE]
>
>Le nouveau type de champ **Recherche externe** n’est pas disponible sur l’ancien créateur de formulaires.

Pour plus d’informations, voir [Concevoir un formulaire à l’aide du créateur de formulaire](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
