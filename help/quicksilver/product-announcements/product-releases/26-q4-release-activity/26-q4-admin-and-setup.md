---
title: Améliorations apportées à l’administration pour le quatrième trimestre 2026
description: Améliorations apportées à l’administration pour le quatrième trimestre 2026
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 1dd8ab20d11b2b4471308ac5402b31e20359a04c
workflow-type: tm+mt
source-wordcount: '604'
ht-degree: 1%

---

# Améliorations apportées à l’administration pour le quatrième trimestre 2026

Cette page décrit les améliorations apportées par l’administrateur à l’environnement de Prévisualisation avec la version du quatrième trimestre 2026. Ces améliorations seront rendues disponibles comme indiqué, dans l’environnement de production.

Pour obtenir la liste de toutes les modifications disponibles à ce stade du cycle de publication du quatrième trimestre 2026, voir [présentation de la version du quatrième trimestre 2026](/help/quicksilver/product-announcements/product-releases/26-q4-release-activity/26-q4-release-overview.md).

## Les administrateurs de groupe peuvent gérer les profils professionnels

>[!NOTE]
>
>Aperçu : 30 juillet 2026>Version rapide de production : 13 août 2026>Production pour tous : 15 octobre 2026

Les administrateurs de groupe peuvent désormais créer, modifier et supprimer les profils professionnels des groupes qu’ils administrent, sans avoir besoin d’un accès d’administrateur système. Cela donne aux entreprises plus de flexibilité pour déléguer la gestion des profils métier au niveau du groupe.

Pour plus d’informations, voir [Afficher et gérer les profils métier](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/view-and-manage-business-profiles.md).

## Prise en charge des modèles de disposition pour les vues des listes améliorées

>[!NOTE]
>
>Aperçu : 30 juillet 2026>Version rapide de production : 13 août 2026>Production pour tous : 15 octobre 2026

Les vues des listes améliorées sont désormais prises en charge au niveau du système via un modèle de mise en page. Vous pouvez masquer les vues système existantes, affecter une vue spécifique en tant que vue par défaut et ajouter une vue personnalisée à la liste des vues système.

Les exemples de listes améliorées dans le modèle de mise en page sont **Toutes les demandes** et **Affectations avancées**. Une liste améliorée comporte un libellé « Nouvelle expérience » en regard des vues.

Pour plus d&#39;informations, voir [Personnaliser des filtres, des vues et des regroupements à l&#39;aide d&#39;un modèle de mise en page](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

## Modification en masse de champs de recherche externe

>[!NOTE]
>
>Aperçu : 30 juillet 2026>Version rapide de production : 13 août 2026>Production pour tous : 15 octobre 2026

Les boîtes de dialogue de modification en bloc permettent désormais de modifier les champs de recherche externes. Cela n’était pas possible auparavant.

Dans les cas où un champ de recherche dépend d’un autre champ de recherche, le champ avec la dépendance ne peut pas être modifié en bloc, sauf si le premier champ est le même pour tous les objets en cours de modification.

Par exemple, une liste de pays dépend de la sélection effectuée pour une région. Si la région d&#39;un projet est l&#39;Asie et la région d&#39;un autre projet est l&#39;Europe et que vous modifiez en bloc les deux projets, le champ Pays ne sera pas disponible car les régions ne correspondent pas. Si vous modifiez la région pour qu’elle soit la même pour les deux projets, vous pouvez également sélectionner un pays à utiliser pour les deux projets.

Pour plus d’informations sur les champs de recherche externe, voir [Création d’un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-external-lookup-fields).

## Logique avancée prise en charge dans l’aperçu du créateur de formulaire personnalisé

>[!NOTE]
>
>Aperçu : 30 juillet 2026>Version rapide de production : 13 août 2026>Production pour tous : 15 octobre 2026

Le mode d’aperçu du créateur de formulaire personnalisé prend désormais en charge les options logiques avancées, notamment la logique d’affichage avancée, la logique de valeur par défaut, la logique de validation, la logique de formatage et la logique d’modifiabilité. Vous pouvez tester les formules logiques dans l’aperçu du formulaire et les ajuster selon vos besoins dans le créateur de logiques. Vous pouvez également sélectionner un objet de test (projet, tâche, problème, etc.) pour prévisualiser le formulaire avec des données contextuelles réelles.

Auparavant, seules les options d’affichage de base et de logique d’omission étaient prises en charge en mode Aperçu.

Notez que ces types de logiques ne sont disponibles que pour les organisations sur les packages Workflow Prime ou Ultimate : affichage avancé, valeur par défaut, mise en forme conditionnelle et modifiabilité.

Pour plus d’informations, consultez les sections [Ajouter des règles de logique aux formulaires et champs personnalisés](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md) et [Organiser et prévisualiser un formulaire](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md).

## Suivi des modifications pour révision et approbation unifiées

>[!NOTE]
>
>Aperçu : 30 juillet 2026>Version rapide de production : 13 août 2026>Production pour tous : 15 octobre 2026

La page Historique des modifications dans Workfront capture désormais l’activité dans les workflows de révision et d’approbation unifiés, offrant ainsi aux administrateurs et administratrices un journal complet de gouvernance pour les événements de cycle de vie des révisions et des documents.

Les actions d’approbation, d’étape et de participant sont désormais suivies. Ces actions peuvent inclure :

* Prendre une décision d’approbation dans la visionneuse Frame.io
* Créer ou supprimer une validation
* Mettre à jour un document, par exemple le renommer, le déplacer ou le supprimer

Chaque entrée comprend les champs suivis standard : date et heure, opération, nom d’utilisateur (ou « généré par le système ») et nom d’objet. Les activités du MCP sont capturées, y compris le LLM (comme Claude) qui a effectué la mise à jour. Les commentaires de la visionneuse Frame.io ne sont pas inclus.

Pour plus d&#39;informations, voir [Afficher et gérer l&#39;historique des modifications](/help/quicksilver/administration-and-setup/manage-enterprise-operations/view-and-manage-change-history.md).
