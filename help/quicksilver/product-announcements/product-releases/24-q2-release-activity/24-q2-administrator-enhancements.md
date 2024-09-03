---
title: Améliorations apportées à l’équipe d’administration au deuxième trimestre 2024
description: Améliorations apportées à l’équipe d’administration au deuxième trimestre 2024
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: a297ee8d-d949-45ab-a219-437316fa8fa3
source-git-commit: a1386652f5181d4aa94ddab8e4f9714ef1c08b73
workflow-type: tm+mt
source-wordcount: '797'
ht-degree: 100%

---

# Améliorations apportées à l’équipe d’administration au deuxième trimestre 2024

Cette page décrit toutes les améliorations apportées à l’équipe d’administration avec la version du deuxième trimestre 2024 de l’environnement de prévisualisation. Ces améliorations seront rendues disponibles comme indiqué, dans l’environnement de production.

Pour obtenir la liste de toutes les modifications disponibles à ce stade du cycle de publication de la version du deuxième trimestre 2024, consultez la section [Vue d’ensemble de la version du deuxième trimestre 2024](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).

## Disponibilité de la logique d’affichage et de la logique de saut en mode prévisualisation du créateur de formulaire

>[!NOTE]
>
>Version de prévisualisation : 28 mars 2024. Production pour l’ensemble des clientes et clients : 24.4 (11 avril 2024)

La version bêta du créateur de formulaire personnalisé vous permet désormais de tester votre logique d’affichage et logique de saut en mode d’aperçu. Auparavant, tous les champs s’affichaient dans l’aperçu même lorsque la logique était appliquée.

Pour plus d’informations sur la prévisualisation d’un formulaire personnalisé dans le créateur de formulaire, voir [Organiser et prévisualiser un formulaire avec le créateur de formulaire](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md).

## Prise en charge des champs de formulaire personnalisés avancés pour les entreprises et les utilisateurs et utilisatrices

>[!NOTE]
>
>Version de prévisualisation : 14 mars 2024. Production pour l’ensemble des clientes et clients : 24.4 (11 avril 2024)

Les fonctionnalités avancées de formulaire personnalisé telles que les champs de recherche externe et les champs natifs Workfront sont désormais disponibles lorsque vous joignez un formulaire personnalisé à une entreprise ou à un utilisateur ou une utilisatrice. Les fonctionnalités avancées sont disponibles dans les pages Détails de l’entreprise et Détails de l’utilisateur ou de l’utilisatrice, et non dans les boîtes de dialogue Modifier entreprise et Modifier utilisateur ou utilisatrice. Le formulaire personnalisé doit être créé dans le nouveau créateur de formulaire pour tirer parti de ces types de champs.

Pour plus d’informations sur les champs de formulaire personnalisés, voir [Concevoir un formulaire avec le créateur de formulaire](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Disponibilité de l’intégration JumpSeat pour les nouveaux types de packages

>[!NOTE]
>
>Version de prévisualisation : 26 février 2024. Production pour un déploiement rapide : avec la version 24.3 (14 mars 2024). Production pour l’ensemble des clientes et clients : 24.4 (11 avril 2024).

L’intégration JumpSeat existante est désormais disponible pour les comptes utilisant l’un des nouveaux types de packages (c’est-à-dire Select, Prime ou Ultimate). Vous devez toujours disposer d’un abonnement JumpSeat actif pour activer l’intégration.

Pour plus d’informations sur l’intégration JumpSeat, voir [Configurer l’intégration JumpSeat](/help/quicksilver/administration-and-setup/configure-integrations/configure-jumpseat.md).

## Disponibilité des champs natifs Workfront dans la version bêta du créateur de formulaire

>[!NOTE]
>
>Version de prévisualisation : 29 février 2024. Production pour un déploiement rapide : avec la version 24.3 (14 mars 2024). Production pour l’ensemble des clientes et clients : 24.4 (11 avril 2024)

Les champs natifs de Workfront sont désormais disponibles pour l’ajout dans vos formulaires personnalisés. Ce nouveau type de champ vous permet d’organiser et de présenter les données à vos utilisateurs et utilisatrices de manière logique, sans avoir à recréer des données existantes dans des champs personnalisés.

Après avoir sélectionné Champ natif dans la liste des champs de formulaires personnalisés à ajouter au créateur de formulaire, vous pouvez sélectionner n’importe quel champ natif pour les objets du formulaire. Par exemple, si la liste des types d’objets en haut du créateur de formulaire affiche Projet, vous pourrez sélectionner des champs natifs pour les projets, mais pas des champs spécifiques aux tâches.

Lorsque le formulaire personnalisé est joint à un objet, le champ est renseigné à partir des données de l’objet. Par exemple, le champ Description d’un formulaire personnalisé joint à un projet extrait la description du projet. (Le champ peut afficher « S.O. » si aucune donnée n’est disponible.)

Les champs natifs utilisés dans les formulaires personnalisés sont disponibles dans la bibliothèque de champs du créateur, pour une réutilisation en toute facilité. Ils sont également visibles dans la zone Configuration > Formulaires personnalisés > Champs afin que vous puissiez voir dans quels formulaires ils sont utilisés.

Cette fonctionnalité est disponible uniquement en version bêta du créateur de formulaire, et non dans l’ancien créateur de formulaire.

Pour plus d’informations, voir [Concevoir un formulaire à l’aide du créateur de formulaire](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

[Regardez une démonstration vidéo de cette fonctionnalité.](https://video.tv.adobe.com/v/3427702/){target=_blank}

## Disponibilité du mappage d’attributs pour les organisations ayant migré vers Adobe IMS

>[!NOTE]
>
>Version de prévisualisation : 22 février 2024 ; production pour tous les clients : 22 février 2024

Les équipes d’administration système Workfront peuvent désormais configurer le mappage des attributs utilisateur pour les organisations qui ont migré vers Adobe IMS. Cela permet de transmettre les informations des utilisateurs et utilisatrices à Workfront à partir du fournisseur d’authentification unique (SSO) de l’organisation, de sorte qu’il ne soit pas nécessaire de saisir ces données à la fois dans Workfront et dans le fournisseur d’authentification unique.

Auparavant, cette fonctionnalité n’était disponible que pour les organisations qui n’étaient pas encore intégrées à Adobe IMS.

Pour plus d’informations sur la configuration du mappage des attributs, voir [Mapper des attributs utilisateur dans l’expérience unifiée Adobe](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/map-user-attributes.md#map-user-attributes-in-the-adobe-unified-experience) dans l’article **Mapper des attributs utilisateur et configurer automatiquement des nouveaux utilisateurs et nouvelles utilisatrices**.

## La logique de saut et la logique d’affichage sont désormais disponibles dans la version bêta du concepteur de formulaires.

>[!NOTE]
>
>Version de prévisualisation : vendredi 8 février 2024. Production pour un déploiement rapide : avec la version 24.2 (vendredi 15 février 2024). Production pour l’ensemble des clientes et clients : 24.4 (11 avril 2024)

Vous pouvez désormais modifier les logiques d’affichage et de saut existantes et ajouter des nouvelles logiques aux formulaires personnalisés dans la version bêta du concepteur de formulaires. Un générateur de logique convivial permet de définir les champs à afficher ou à ignorer en fonction des sélections dans le formulaire.

Les icônes sur un champ dans la zone de travail du créateur de formulaire indiquent si la logique est configurée sur ce champ ou si le champ est utilisé dans les règles de logique configurées sur d’autres champs.

Pour plus d’informations, voir [Ajouter une logique d’affichage et d’exclusion à l’aide du concepteur de formulaires](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md).
