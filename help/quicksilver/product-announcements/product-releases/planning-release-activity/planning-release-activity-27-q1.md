---
content-type: release-notes
title: Activité de la version du premier trimestre 2027 pour Adobe Workfront Planning
description: Il s’agit de l’activité de publication du produit Planification d’Adobe Workfront pour le premier trimestre 2027.
author: Becky
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: a29813d3-f0cc-4b60-9396-13b558370803
    internal-label: Product announcements
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
source-git-commit: 949503fecba92a7b8536b4af0b9c684e7f9e3300
workflow-type: tm+mt
source-wordcount: '1082'
ht-degree: 3%
---
# Activité de la version du premier trimestre 2027 pour Adobe Workfront Planning

Cet article décrit les fonctionnalités publiées pour Workfront Planning dans la version du premier trimestre 2027.

Pour obtenir la liste de toutes les fonctionnalités publiées pour Adobe Workfront Planning, voir [Activité de version d’Adobe Workfront Planning : index des articles](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).

## Meilleure visibilité des résultats de recherche rapide dans la vue Tableau

>[!NOTE]
>
>Aperçu : 29 octobre 2026
>Version rapide de production : 12 novembre 2026
>Production pour tous : 21 janvier 2027

Lorsque vous utilisez la recherche rapide dans la vue Tableau pour rechercher un élément, la vue élimine tous les enregistrements qui ne correspondent pas à la recherche et affiche uniquement les éléments qui correspondent.

Avant cette amélioration, tous les enregistrements étaient affichés avec ceux qui correspondent aux résultats de recherche mis en surbrillance.

Pour plus d’informations, consultez la section [Gérer la vue en tableau](/help/quicksilver/planning/views/manage-the-table-view.md).

<!--

## Record-level permissions - restricted access to records

PLACEHOLDER: The release note field on the Workfront task points to an anchor story that no longer exists, so there is no description yet. Add the description and help link before unhiding.

>[!NOTE]
>
>Preview: October 29, 2026
>Production fast release: November 12, 2026
>Production for everyone: January 21, 2027

-->

## Autoriser la connexion des enregistrements des types d’enregistrements globaux connectés dans les espaces de travail secondaires lorsque la connectivité entre espaces de travail est désactivée

>[!NOTE]
>
>Aperçu : 29 octobre 2026
>Version rapide de production : 12 novembre 2026
>Production pour tous : 21 janvier 2027

Lorsque deux types d’enregistrements globaux connectés sont ajoutés à un espace de travail secondaire, vous pouvez désormais désactiver la connectivité entre espaces de travail et toujours lier les enregistrements localement. Chaque espace de travail secondaire ne voit que ses propres enregistrements pour les deux types d’enregistrements et peut les connecter les uns aux autres. Les enregistrements de l’espace de travail global et d’autres espaces de travail secondaires ne s’affichent plus.

Avant cette amélioration, si la connectivité entre espaces de travail était désactivée pour les types d’enregistrements globaux connectés, les espaces de travail secondaires ne pouvaient pas lier leurs propres enregistrements les uns aux autres. Si elle était activée, les utilisateurs pouvaient afficher et lier des enregistrements de l’espace de travail global et de tous les autres espaces de travail secondaires.

Pour plus d’informations, voir [&#x200B; Présentation du type d’enregistrement de l’espace de travail croisé &#x200B;](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md).

## Afficher le nombre total d’enregistrements dans les vues Tableau

>[!NOTE]
>
>Aperçu : 29 octobre 2026
>Version rapide de production : 12 novembre 2026
>Production pour tous : 21 janvier 2027

La vue Tableau affiche désormais le nombre total d’enregistrements et le nombre est automatiquement mis à jour lorsque vous appliquez des filtres, recherchez ou modifiez la vue. Le nombre d’enregistrements reflète toujours l’intégralité des résultats filtrés et respecte vos autorisations.

Pour plus d’informations, consultez la section [Gérer la vue en tableau](/help/quicksilver/planning/views/manage-the-table-view.md).

<!--

## Field aggregators available for groupings in the table view

>[!NOTE]
>
>Preview: October 29, 2026
>Production fast release: November 12, 2026
>Production for everyone: January 21, 2027

Grouped records in the table views now show a summary row for each grouping, plus a grand total for the full table. Groupings and the grand total use the same summary functions, and nested groupings get their own summaries that include all child records. Aggregators update automatically as you filter, search, regroup, or edit records.

For information, see [Manage the table view](/help/quicksilver/planning/views/manage-the-table-view.md).

## Add sections to organize Planning views

>[!NOTE]
>
>Preview: October 29, 2026
>Production fast release: November 12, 2026
>Production for everyone: January 21, 2027

You can now create sections in the Workfront Planning View dropdown menu to organize related views as your list grows. You can name each section when you create it, then move views from My Views and Shared with Me into your custom sections. System views stay fixed in the System section.

For information, see [Manage record views](/help/quicksilver/planning/views/manage-record-views.md).

-->

<!--

## Filters for Workfront objects connected record fields

>[!NOTE]
>
>Preview: October 29, 2026
>Production fast release: November 12, 2026
>Production for everyone: January 21, 2027

You can now filter for certain Workfront object types that meet a filter criteria when you add them as a connected field in Planning.

Only those Workfront objects that meet your filtering criteria will display as options in connected fields when editing a record.

For this feature, we added a new Record filtering rules option in the New connection tab when connecting the following Workfront object types: projects, portfolios, programs, groups, companies. Prior to this enhancement, filters were available only when connecting two record types.

For information, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md).

-->

## Limites du nombre de champs de recherche

>[!NOTE]
>
>Aperçu : 29 octobre 2026
>Version rapide de production : 12 novembre 2026
>Production pour tous : 21 janvier 2027

Nous introduisons des limites sur le nombre de champs de recherche que vous pouvez ajouter à un type d’enregistrement :

* Jusqu’à 40 champs de recherche par type d’enregistrement
* Jusqu’à 5 champs de recherche de texte long par type d’enregistrement. Les champs de recherche connectés sont comptabilisés par rapport à la limite de leur champ d’origine.
* Jusqu’à 50 000 caractères dans la valeur d’une seule cellule de recherche de texte long. Si le contenu combiné des valeurs de recherche dépasse ce seuil, les valeurs sont affichées dans l’ordre de la connexion jusqu’à ce que la limite soit atteinte. La première valeur qui la dépasse et toutes les valeurs qui la suivent sont omises. Le champ de l’objet connecté d’origine n’est jamais modifié.

Vous recevez une erreur lorsque vous essayez de créer ou de modifier un champ de recherche au-delà des deux premières limites. Les types d’enregistrements qui dépassent déjà ces limites ne sont pas affectés par cette modification. Vous pouvez les modifier, mais vous ne pouvez pas ajouter d’autres champs ou valeurs de recherche tant que vous n’êtes pas sous la limite.

Pour plus d&#39;informations, voir Présentation des limites d&#39;objet d&#39;Adobe Workfront Planning [&#128279;](/help/quicksilver/planning/general/limitations-overview.md).

## Les nouveaux champs n’apparaissent désormais que dans l’affichage où vous les créez

>[!NOTE]
>
>Aperçu : 29 octobre 2026
>Version rapide de production : 12 novembre 2026
>Production pour tous : 21 janvier 2027

Lorsque vous ajoutez un nouveau champ à un type d’enregistrement, il s’affiche désormais uniquement dans la vue dans laquelle vous travaillez et est masqué dans toutes les autres vues existantes. Les autres vues restent telles que configurées et vous pouvez y afficher le nouveau champ, si nécessaire.

Avant cette amélioration, les nouveaux champs étaient ajoutés de manière non masquée à chaque affichage, ce qui entraînait parfois de la confusion pour les utilisateurs et utilisatrices qui ne connaissaient pas les nouveaux champs.

Pour plus d’informations, consultez [Créer des champs](/help/quicksilver/planning/fields/create-fields.md).

## Exporter les détails des enregistrements depuis n’importe quelle vue

>[!NOTE]
>
>Aperçu : 29 octobre 2026
>Version rapide de production : 12 novembre 2026
>Production pour tous : 21 janvier 2027

Vous pouvez désormais exporter les détails d’un enregistrement depuis n’importe quelle vue de détail, sans avoir à passer à la vue Tous les champs .

Auparavant, l’option d’exportation n’était disponible que lorsque la vue Tous les champs était sélectionnée.

Pour plus d’informations, voir [Exporter les détails d’un enregistrement](/help/quicksilver/planning/records/export-the-record-page.md).

<!--

## Cancel and revert changes when editing records when business rules are violated

>[!NOTE]
>
>Preview: October 29, 2026
>Production fast release: November 12, 2026
>Production for everyone: January 21, 2027

To ensure data integrity, when a business rule is violated while you edit a record, the change is blocked, the value reverts, and a toast notification explains why the edit is not allowed. The warning is visible in all areas where you are editing records, including the table view or details page.

If multiple rules are violated, each violation issues its own toast notification.

For more information, see [Configure business rules](/help/quicksilver/planning/architecture/configure-business-rules.md).

-->

## Amélioration des performances avec le chargement incrémentiel des données dans les vues Tableau et Chronologie

<!-- NOTE FROM CSV: Must check with Lilit whether this will come to the timeline view in addition to the table (Lilit said yes; this was messaged before but pulled). The second bullet will change; check with Lilit first. -->

>[!NOTE]
>
>Aperçu : 29 octobre 2026
>Version rapide de production : 12 novembre 2026
>Production pour tous : 21 janvier 2027

Pour améliorer les performances sur un grand nombre d’enregistrements, nous avons apporté les améliorations suivantes aux vues Tableau et Chronologie :

* La vue charge désormais initialement les 500 premiers enregistrements, avec des enregistrements supplémentaires chargés automatiquement lorsque vous faites défiler les lots de 500.
* La recherche et le regroupement rapides n’affectent que les enregistrements actuellement chargés dans la vue.

Pour plus d’informations, consultez la section [Gérer la vue de tableau](/help/quicksilver/planning/views/manage-the-table-view.md) et [Gérer la vue chronologique](/help/quicksilver/planning/views/manage-the-timeline-view.md).

<!--

## Additional permissions for users other than requestors to submitted requests

>[!NOTE]
>
>Preview: October 28, 2026
>Production fast release: November 12, 2026
>Production for everyone: January 21, 2027

Workspace managers can now define what access to submitted requests users other than requestors have.

By editing the Permissions area of a request form, you can define additional access for other users to requests submitted using the form.

You can grant permissions to workspace users or any other users, groups, teams, job roles or companies in the system. Once defined in the request queue, the permissions are granted automatically when the request is submitted, and any permission changes apply only to new requests.

Prior to this enhancement, you could only grant permissions to requestors.

For information, see [Create and manage a request form in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

-->

## Réorganisation manuelle du regroupement dans la vue Chronologie

>[!NOTE]
>
>Aperçu : 29 octobre 2026
>Version rapide de production : 12 novembre 2026
>Production pour tous : 21 janvier 2027

Vous pouvez désormais glisser-déposer des regroupements, des sous-regroupements et des enregistrements afin de créer un ordre personnalisé dans la vue Chronologie. Votre disposition manuelle est conservée entre les sessions et vous pouvez basculer facilement entre la commande manuelle et le tri basé sur les champs à mesure que les besoins de planification changent.

La fonctionnalité glisser-déposer est disponible pour les versions de couloir et empilées de la vue chronologique.

Pour plus d’informations, consultez [Gérer la vue chronologique](/help/quicksilver/planning/views/manage-the-timeline-view.md).

## Règles métier pour les types d’enregistrements globaux

>[!NOTE]
>
>Aperçu : 28 octobre 2026
>Version rapide de production : 12 novembre 2026
>Production pour tous : 21 janvier 2027

Les responsables Workspace peuvent désormais configurer des règles métier sur les types d’enregistrements globaux dans les espaces de travail principal et secondaire. Les règles s’appliquent à tous les enregistrements du même type dans tous les espaces de travail où elles sont ajoutées.

Les règles métier ajoutées dans les espaces de travail globaux s’affichent en lecture seule dans les espaces de travail secondaires où les types d’enregistrements ont été importés. Les règles métier ajoutées dans les espaces de travail secondaires s’affichent en lecture seule dans les espaces de travail principaux où les types d’enregistrements ont été créés à l’origine. Les règles ne sont modifiables que dans les espaces de travail où elles sont créées.

Pour plus d’informations, voir [Configurer des règles métier de type enregistrement](/help/quicksilver/planning/architecture/configure-business-rules.md).

## Configurer les paramètres d&#39;invite par défaut pour la fonctionnalité Remplir le formulaire dans les demandes Planning

>[!NOTE]
>
>Aperçu : 21 octobre 2026
>Version rapide de production : 12 novembre 2026
>Production pour tous : 21 janvier 2027

Vous pouvez désormais personnaliser l’invite que les utilisateurs voient lors de l’utilisation de la fonctionnalité de formulaire de remplissage optimisé par l’IA lors de l’envoi d’une requête Planning.

Vous pouvez créer une invite par défaut lors de la création d&#39;un formulaire de demande pour les demandes Planning.

Pour plus d’informations, voir [Création et gestion d’un formulaire de demande dans Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).
