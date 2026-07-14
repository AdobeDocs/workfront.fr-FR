---
title: Améliorations apportées à l’administration au troisième trimestre 2026
description: Améliorations apportées à l’administration au troisième trimestre 2026
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: f45c946e48b253018648c414915d53eca5a4de80
workflow-type: tm+mt
source-wordcount: '1334'
ht-degree: 6%

---

# Améliorations apportées à l’administration au troisième trimestre 2026

Cette page décrit les améliorations apportées par l’administrateur à l’environnement de Prévisualisation avec la version du troisième trimestre de 2026. Ces améliorations seront rendues disponibles comme indiqué, dans l’environnement de production.

Pour obtenir la liste de toutes les modifications disponibles à ce stade du cycle de publication du troisième trimestre 2026, voir [Présentation de la version du troisième trimestre 2026](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-release-overview.md).

<!--

## Change tracking for unified review and approval

>[!NOTE]
>
>Preview: July 7, 2026
>Production fast release: July 15, 2026
>Production for everyone: July 16, 2026

The Change History page in Workfront now captures activity across unified review and approval workflows, giving administrators a complete governance trail for review and document lifecycle events.

Approval, stage, and participant actions are now tracked. These actions may include:

* Making an approval decision in the Frame.io viewer
* Creating or deleting an approval
* Updating a document such as renaming, moving, or deleting it

Each entry includes the standard tracked fields: date and time, operation, user name (or "system generated"), and object name. Frame.io viewer comments are not included.

This phase of change tracking does not include MCP events. Those will be part of a future release.

For more information, see [View and manage change history](/help/quicksilver/administration-and-setup/manage-enterprise-operations/view-and-manage-change-history.md).

-->

## Champ de recherche interne remplaçant le type de champ de saisie semi-automatique

>[!NOTE]
>
>Aperçu : 7 juillet 2026Version rapide de production : 15 juillet 2026Production pour tous : 16 juillet 2026

Le nouveau type de champ **Recherche interne** dans les formulaires personnalisés offre un filtrage dynamique. Similaire au type de champ de saisie semi-automatique , il permet aux utilisateurs de rechercher et de sélectionner des objets Workfront existants en saisissant une partie du nom. Le filtre sur la recherche interne peut référencer la valeur dans un autre champ du formulaire, ce qui n’est pas possible avec les en-têtes de saisie.

La sélection multiple est prise en charge sur les recherches internes et ce type de champ offre également de meilleures performances pour les jeux de données volumineux. Les objets Workfront natifs suivants sont pris en charge dans les recherches internes : Projet, Entreprise, Groupe, Fonction, Portfolio, Programme, Équipe, Modèle, Utilisateur, Tâche, Problème, Document et Emplacement.

Le type de champ de recherche interne remplace le type de champ de saisie semi-automatique. Vous pouvez rapidement convertir des champs de saisie semi-automatique existants en recherches internes en cliquant sur le bouton dans les options de champ à droite. Lors de la conversion, les données historiques restent sur le champ et sont utilisées de la même manière dans les rapports.

>[!IMPORTANT]
>
>Les intégrations externes telles que les scénarios Workfront Fusion ou les automatisations basées sur les API peuvent référencer des structures de champ héritées et nécessiter des mises à jour après la conversion. Vous devez vérifier les intégrations avant de convertir les champs de saisie semi-automatique en champs de recherche interne.

Pour plus d’informations, voir [Créer un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Logique de valeur par défaut prise en charge sur les champs de référence natifs

>[!NOTE]
>
>Aperçu : 7 juillet 2026Version rapide de production : 15 juillet 2026Production pour tous : 16 juillet 2026
>
>Cette fonctionnalité n’est disponible que pour les organisations qui utilisent les packages Workflow Prime ou Ultimate.

Dans les formulaires personnalisés, les champs de référence natifs vous permettent désormais d’ajouter une logique de valeur par défaut.

Ce type de logique sur les champs de référence natifs est disponible uniquement dans l’interface utilisateur et non dans l’API Workfront.

Pour plus d’informations, consultez la section [Ajouter une logique de valeur par défaut à un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md#add-default-value-logic-to-a-custom-form) dans l’article [Ajouter des règles de logique aux formulaires et champs personnalisés](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md).

## Mises à jour du filtrage des champs natifs dans les formulaires personnalisés

>[!NOTE]
>
>Aperçu : 7 juillet 2026Version rapide de production : 15 juillet 2026Production pour tous : 16 juillet 2026

Les filtres système qui existent sur les champs natifs sont désormais appliqués aux champs des formulaires personnalisés et visibles par l’administration.

Lorsque vous ajoutez un champ de référence natif auquel un filtre système est appliqué, vous pouvez appliquer le même filtre au champ du formulaire personnalisé et modifier le filtre si nécessaire dans la zone Mode texte .

L’ajout de votre propre filtre personnalisé au champ remplace le filtre système du champ. Si vous ne saisissez pas de filtre personnalisé, le filtre système est appliqué par défaut.

En outre, le filtrage dynamique est désormais disponible sur les champs de référence natifs. Un filtre dynamique permet de réduire la liste des éléments en fonction de la valeur d’un autre champ.

Par exemple, lorsque vous utilisez `?portfolioID={portfolio}.{ID}` dans un filtre de champ Projet et qu’un champ natif Portfolio figure dans le formulaire personnalisé, le champ Projet affiche uniquement les projets qui se trouvent dans le portfolio sélectionné. Si le champ Portfolio n’est pas renseigné, tous les projets sont disponibles dans le champ Projet .

Pour plus d’informations, voir [Créer un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Protéger les noms de champ contre les changements de nom accidentels

>[!NOTE]
>
>Aperçu : 7 juillet 2026Version rapide de production : 15 juillet 2026Production pour tous : 16 juillet 2026

Pour protéger les intégrations et l’intégrité des données, nous avons mis à jour la manière dont les noms de champ peuvent être modifiés dans le panneau des paramètres de champ d’un formulaire personnalisé.

Les noms de champ dans le panneau des paramètres de champ sont désormais en lecture seule par défaut. Vous pouvez toujours modifier le nom du champ, mais le renommage nécessite une étape de confirmation explicite. Le champ précédemment appelé **Nom** a également été mis à jour vers **Nom de l’API** pour mieux refléter sa signification technique. Le champ **Libellé** reste modifiable.

Pour plus d’informations, voir [Créer un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#notes-on-field-names-and-labels).

## Affichage de l’historique des modifications des objets Workfront

>[!NOTE]
>
>Aperçu : 11 juin 2026Version rapide de production : 11 juin 2026Production pour tous : 16 juillet 2026

Pour que vous puissiez voir plus facilement les modifications qui se sont produites dans une liste centrale, nous avons créé la liste Historique des modifications. Cette liste affiche des informations telles que l’objet, l’opération et la source de la modification (un utilisateur ou le système Workfront, par exemple).

Auparavant, les journaux d’audit étaient disponibles, mais ne couvraient pas les objets.

Pour plus d&#39;informations, voir [Afficher et gérer l&#39;historique des modifications](/help/quicksilver/administration-and-setup/manage-enterprise-operations/view-and-manage-change-history.md).

## Nouvelle préférence système pour convertir les portefeuilles de stockage hérités en stockage cloud Adobe

>[!NOTE]
>
>Aperçu : 11 juin 2026Production pour tous : 11 juin 2026Hors planning]{type=Neutral}

Les administrateurs Workfront peuvent désormais convertir les portefeuilles de stockage hérités en stockage cloud Adobe directement à partir des préférences système. Pour convertir des portfolios, sélectionnez-les dans le nouveau champ Sélectionner les portfolios à convertir en stockage d’entreprise et enregistrez la page.

Lorsqu’un portfolio est converti en espace de stockage dans le cloud Adobe :

* Vous ne pouvez plus déplacer vers ce portfolio des projets qui utilisent le stockage Workfront hérité.
* Tous les nouveaux projets créés dans ce portfolio utilisent l’espace de stockage Adobe.
* Frame.io est la visionneuse de documents utilisant l’espace de stockage cloud d’Adobe
* Les objets enfants utilisant le stockage Workfront hérité restent sur le stockage hérité

Auparavant, l’ajout d’un projet de stockage dans le cloud Adobe à un portfolio de stockage hérité convertissait automatiquement le portfolio en stockage dans le cloud Adobe.

Pour plus d’informations, voir [Configuration des préférences système](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

## Texte enrichi remplaçant le texte par le type de champ de mise en forme

>[!NOTE]
>
>Aperçu : 28 mai 2026Version rapide de production : 11 juin 2026Production pour tous : 16 juillet 2026

Le nouveau type de champ **Texte enrichi** dans les formulaires personnalisés est un puissant éditeur de texte, avec des options de mise en forme telles que l’exposant et l’indice, les en-têtes et les tableaux, en plus des options traditionnelles telles que le gras, l’italique, le soulignement, les puces, la numérotation, les liens hypertexte et les guillemets. La limite de caractères reste de 15 000.

Le type de champ Texte enrichi remplace le texte par un type de champ de mise en forme. Vous pouvez rapidement convertir du texte existant avec des champs de mise en forme en texte enrichi en cliquant sur le bouton dans les options de champ à droite. Lors de la conversion, les données historiques restent sur le champ et sont utilisées de la même manière dans les rapports.

>[!IMPORTANT]
>
>Les intégrations externes telles que les scénarios Workfront Fusion ou les automatisations basées sur les API peuvent référencer des structures de champ héritées et nécessiter des mises à jour après la conversion. Vous devez vérifier les intégrations avant de convertir les champs en texte enrichi.

Pour plus d’informations, voir [Créer un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Champs financiers natifs pris en charge dans les formulaires personnalisés

>[!NOTE]
>
>Aperçu : 28 mai 2026Version rapide de production : 11 juin 2026Production pour tous : 16 juillet 2026

Vous pouvez désormais inclure des champs financiers natifs de Workfront dans les formulaires personnalisés. Auparavant, les champs financiers n’étaient pas pris en charge.

Les champs financiers disponibles que vous pouvez référencer dépendent du type de formulaire.

Pour plus d’informations, voir [Créer un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-workfront-native-fields).

## Les formulaires personnalisés peuvent être partagés dans tout le système avec la possibilité de les joindre à d’autres éléments.

>[!NOTE]
>
>Aperçu : 28 mai 2026Version rapide de production : 11 juin 2026Production pour tous : 16 juillet 2026

Une nouvelle option de partage, « Tout le monde dans le système peut afficher et joindre », a été ajoutée aux formulaires personnalisés. Lorsque vous sélectionnez cette option, tous les utilisateurs à l’échelle du système peuvent joindre le formulaire à d’autres objets.

Le partage à l’échelle du système élimine la nécessité de partager manuellement les formulaires et de mettre à jour les autorisations entre les groupes ou les agences lorsque de nouveaux groupes sont ajoutés.

Pour plus d’informations, voir [Partager un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).

## Nouvelle préférence système pour appliquer les champs obligatoires dans la modification en bloc

>[!NOTE]
>
>Aperçu : 28 mai 2026Version rapide de production : 11 juin 2026Production pour tous : 16 juillet 2026

Actuellement, lorsque vous modifiez des objets en bloc, les champs obligatoires ne sont appliqués que lorsqu’un utilisateur modifie le champ. Si un champ n’est pas modifié, il est traité comme facultatif et non validé.

Une nouvelle préférence système vous permet désormais d’appliquer les champs obligatoires dans la modification en bloc. Pour ne pas autoriser l’enregistrement d’objets modifiés en bloc à moins que tous les champs obligatoires n’aient des valeurs, sélectionnez l’option **Toujours appliquer les champs obligatoires dans la modification en bloc** sur la page Configuration > Système > Préférences.

Pour plus d’informations, voir [Configuration des préférences système](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).
