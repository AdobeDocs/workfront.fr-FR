---
title: Améliorations apportées à l’administration au troisième trimestre 2026
description: Améliorations apportées à l’administration au troisième trimestre 2026
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: d83d823426b42202e83cb4db64f85d27d4dca0bb
workflow-type: tm+mt
source-wordcount: '857'
ht-degree: 9%

---

# Améliorations apportées à l’administration au troisième trimestre 2026

Cette page décrit les améliorations apportées par l’administrateur à l’environnement de Prévisualisation avec la version du troisième trimestre de 2026. Ces améliorations seront rendues disponibles comme indiqué, dans l’environnement de production.

Pour obtenir la liste de toutes les modifications disponibles à ce stade du cycle de publication du troisième trimestre 2026, voir [Présentation de la version du troisième trimestre 2026](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-release-overview.md).

## Suivi des modifications pour révision et approbation unifiées

>[!NOTE]
>
>Aperçu : 7 juillet 2026Version rapide de production : 15 juillet 2026Production pour tous : 16 juillet 2026

La page Historique des modifications dans Workfront capture désormais l’activité dans les workflows de révision et d’approbation unifiés, offrant ainsi aux administrateurs et administratrices un journal complet de gouvernance pour les événements de cycle de vie des révisions et des documents.

Les actions d’approbation, d’étape et de participant sont désormais suivies. Ces actions peuvent inclure :

* Prendre une décision d’approbation dans la visionneuse Frame.io
* Créer ou supprimer une validation
* Mettre à jour un document, par exemple le renommer, le déplacer ou le supprimer

Chaque entrée comprend les champs suivis standard : date et heure, opération, nom d’utilisateur (ou « généré par le système ») et nom d’objet. Les commentaires de la visionneuse Frame.io ne sont pas inclus.

Cette phase de suivi des modifications n’inclut pas les événements MCP. Celles-ci feront partie d’une version ultérieure.

Pour plus d&#39;informations, voir [Afficher et gérer l&#39;historique des modifications](/help/quicksilver/administration-and-setup/manage-enterprise-operations/view-and-manage-change-history.md).

<!--

## Internal lookup field replacing Typeahead field type

>[!NOTE]
>
>Preview: July 7, 2026
>Production fast release: July 15, 2026
>Production for everyone: July 16, 2026

The new **Internal lookup** field type in custom forms provides dynamic filtering. It is similar to the Typeahead field type and allows users to search and select existing Workfront objects by typing part of the name. The filter on the internal lookup can reference the value in another field on the form, which is not possible with Typeaheads.

Multi-select is supported on internal lookups, and this field type also provides improved performance for large datasets. The following native Workfront objects are supported in internal lookups: Project, Company, Group, Job Role, Portfolio, Program, Team, Template, User, Task, Issue, Document, and Location.

The Internal lookup field type is replacing the Typeahead field type. You can quickly convert existing Typeahead fields to Internal lookups by clicking the button in the field options on the right. When you convert, historical data remains on the field and it is used the same way in reports.

>[!IMPORTANT]
>
>External integrations such as Workfront Fusion scenarios or API-based automations may reference legacy field structures and require updates after the conversion. You should verify any integrations before converting Typeahead fields to Internal lookup fields.

For more information, see [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

-->

<!--

## Default value logic supported on native reference fields

>[!NOTE]
>
>Preview: July 7, 2026
>Production fast release: July 15, 2026
>Production for everyone: July 16, 2026
>
>This feature is only available for organizations on the Workflow Prime or Ultimate packages.

In custom forms, native reference fields now allow you to add default value logic.

This logic type on native reference fields is available only in the user interface and not in the Workfront API.

For information, see [Add default value logic to a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md#add-default-value-logic-to-a-custom-form) in the article [Add logic rules to custom forms and fields](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md).

-->

<!--

## Updates to native field filtering in custom forms

>[!NOTE]
>
>Preview: July 7, 2026
>Production fast release: July 15, 2026
>Production for everyone: July 16, 2026

System filters that exist on native fields are now applied to the fields in custom forms and are visible to administrators.

When you add a native reference field that has a system filter applied, you can apply the same filter to the field in the custom form and modify the filter if needed in the Text Mode box.

Adding your own custom filter to the field overrides the system filter for the field. If you do not enter a custom filter, the system filter is applied by default.

Also, dynamic filtering is now available on native reference fields. A dynamic filter allows you to narrow the list of items based on the value of another field.

For example, when you use `?portfolioID={portfolio}.{ID}` in a Project field filter and a Portfolio native field is on the custom form, the Project field shows only projects that are in the selected portfolio. If the Portfolio field is left blank, then all projects are available in the Project field.

For information, see [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

-->

<!--

## Protect field names from accidental renaming

>[!NOTE]
>
>Preview: July 7, 2026
>Production fast release: July 15, 2026
>Production for everyone: July 16, 2026

To protect integrations and data integrity, we've updated how field names can be edited in the field settings panel of a custom form.

Field names in the field settings panel are now read-only by default. You can still edit the field name, but renaming requires an explicit confirmation step. The field previously called **Name** has also been updated to **API Name** to better reflect its technical significance. The **Label** field remains editable.

For information, see [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#notes-on-field-names-and-labels).

-->

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
>Aperçu : 11 juin 2026Production pour tous : 11 juin 2026

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
