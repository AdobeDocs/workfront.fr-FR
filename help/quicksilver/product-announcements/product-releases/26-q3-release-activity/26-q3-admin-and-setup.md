---
title: Améliorations apportées à l’administration au troisième trimestre 2026
description: Améliorations apportées à l’administration au troisième trimestre 2026
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: cc0067cb2f64eae79647881ab30355b6832073d1
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 3%

---

# Améliorations apportées à l’administration au troisième trimestre 2026

Cette page décrit les améliorations apportées par l’administrateur à l’environnement de Prévisualisation avec la version du troisième trimestre de 2026. Ces améliorations seront rendues disponibles comme indiqué, dans l’environnement de production.

Pour obtenir la liste de toutes les modifications disponibles à ce stade du cycle de publication du troisième trimestre 2026, voir [Présentation de la version du troisième trimestre 2026](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-release-overview.md).

## Affichage de l’historique des modifications des objets Workfront

>[!NOTE]
>
>Aperçu : 11 juin 2026>Version rapide de production : 11 juin 2026>Production pour tous : 16 juillet 2026

Pour que vous puissiez voir plus facilement les modifications qui se sont produites dans une liste centrale, nous avons créé la liste Historique des modifications. Cette liste affiche des informations telles que l’objet, l’opération et la source de la modification (un utilisateur ou le système Workfront, par exemple).

Auparavant, les journaux d’audit étaient disponibles, mais ne couvraient pas les objets.

<!--

For more information see [View and manage change history](help/quicksilver/administration-and-setup/manage-enterprise-operations/view-and-manage-change-history.md).

-->

<!--

## New system preference to convert legacy storage portfolios to Adobe cloud storage

>[!NOTE]
>
>Preview: June 11, 2026
>Production for everyone: June 11, 2026

Workfront administrators can now convert legacy storage portfolios to Adobe cloud storage directly from System Preferences. To convert portfolios, select them in the new Select portfolios to convert to enterprise storage field and save the page.

When a portfolio is converted to Adobe cloud storage:

* You can no longer move projects that use legacy Workfront storage to this portfolio
* All new projects created in this portfolio use Adobe cloud storage
* Frame.io is the viewer for documents using Adobe cloud storage
* Child objects using legacy Workfront storage stay on legacy storage

Previously, adding an Adobe cloud storage project to a Legacy storage portfolio automatically converted the portfolio to Adobe cloud storage.

For more information, see [Configure system preferences](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

-->

## Texte enrichi remplaçant le texte par le type de champ de mise en forme

>[!NOTE]
>
>Aperçu : 28 mai 2026>Version rapide de production : 11 juin 2026>Production pour tous : 16 juillet 2026

Le nouveau type de champ **Texte enrichi** dans les formulaires personnalisés est un puissant éditeur de texte, avec des options de mise en forme telles que l’exposant et l’indice, les en-têtes et les tableaux, en plus des options traditionnelles telles que le gras, l’italique, le soulignement, les puces, la numérotation, les liens hypertexte et les guillemets. La limite de caractères reste de 15 000.

Le type de champ Texte enrichi remplace le texte par un type de champ de mise en forme. Vous pouvez rapidement convertir du texte existant avec des champs de mise en forme en texte enrichi en cliquant sur le bouton dans les options de champ à droite. Lors de la conversion, les données historiques restent sur le champ et sont utilisées de la même manière dans les rapports.

>[!IMPORTANT]
>
>Les intégrations externes telles que les scénarios Workfront Fusion ou les automatisations basées sur les API peuvent référencer des structures de champ héritées et nécessiter des mises à jour après la conversion. Vous devez vérifier les intégrations avant de convertir les champs en texte enrichi.

Pour plus d’informations, voir [Créer un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Champs financiers natifs pris en charge dans les formulaires personnalisés

>[!NOTE]
>
>Aperçu : 28 mai 2026>Version rapide de production : 11 juin 2026>Production pour tous : 16 juillet 2026

Vous pouvez désormais inclure des champs financiers natifs de Workfront dans les formulaires personnalisés. Auparavant, les champs financiers n’étaient pas pris en charge.

Les champs financiers disponibles que vous pouvez référencer dépendent du type de formulaire.

Pour plus d’informations, voir [Créer un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-workfront-native-fields).

## Les formulaires personnalisés peuvent être partagés dans tout le système et vous pouvez y joindre des formulaires

>[!NOTE]
>
>Aperçu : 28 mai 2026>Version rapide de production : 11 juin 2026>Production pour tous : 16 juillet 2026

Une nouvelle option de partage, « Tout le monde dans le système peut afficher et joindre », a été ajoutée aux formulaires personnalisés. Lorsque vous sélectionnez cette option, tous les utilisateurs à l’échelle du système peuvent joindre le formulaire à d’autres objets.

Le partage à l’échelle du système élimine la nécessité de partager manuellement les formulaires et de mettre à jour les autorisations entre les groupes ou les agences lorsque de nouveaux groupes sont ajoutés.

Pour plus d’informations, voir [Partager un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).

## Nouvelle préférence système pour appliquer les champs obligatoires dans la modification en bloc

>[!NOTE]
>
>Aperçu : 28 mai 2026>Version rapide de production : 11 juin 2026>Production pour tous : 16 juillet 2026

Actuellement, lorsque vous modifiez des objets en bloc, les champs obligatoires ne sont appliqués que lorsqu’un utilisateur modifie le champ. Si un champ n’est pas modifié, il est traité comme facultatif et non validé.

Une nouvelle préférence système vous permet désormais d’appliquer les champs obligatoires dans la modification en bloc. Pour ne pas autoriser l’enregistrement d’objets modifiés en bloc à moins que tous les champs obligatoires n’aient des valeurs, sélectionnez l’option **Toujours appliquer les champs obligatoires dans la modification en bloc** sur la page Configuration > Système > Préférences.

Pour plus d’informations, voir [Configuration des préférences système](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).
