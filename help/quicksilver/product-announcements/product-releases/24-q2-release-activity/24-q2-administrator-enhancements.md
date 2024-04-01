---
title: Améliorations apportées à l’administrateur au deuxième trimestre 2024
description: Améliorations apportées à l’administrateur au deuxième trimestre 2024
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: a297ee8d-d949-45ab-a219-437316fa8fa3
source-git-commit: 2faa01024a1a174bacb42e9c6e24f528252f49f4
workflow-type: tm+mt
source-wordcount: '802'
ht-degree: 0%

---

# Améliorations apportées à l’administrateur au deuxième trimestre 2024

Cette page décrit toutes les améliorations apportées à l’administrateur à la version du deuxième trimestre 2024 de l’environnement Aperçu. Ces améliorations seront rendues disponibles dans l’environnement de production, comme indiqué.

Pour obtenir la liste de toutes les modifications disponibles à ce stade du cycle de publication 2024 du deuxième trimestre, voir [Présentation de la version du deuxième trimestre 2024](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).

## La logique d’affichage et la logique de saut sont désormais disponibles en mode d’aperçu du concepteur de formulaires.

>[!NOTE]
>
>Version d’aperçu : 28 mars 2024 ; Production pour tous les clients : 24.4 (avril 2024)

Le concepteur de formulaire personnalisé bêta vous permet désormais de tester votre logique d’affichage et d’ignorer la logique en mode d’aperçu. Auparavant, tous les champs s’affichaient dans l’aperçu même lorsque la logique était appliquée.

Pour plus d’informations sur la prévisualisation d’un formulaire personnalisé dans le concepteur de formulaire, voir [Organisation et prévisualisation d’un formulaire avec le concepteur de formulaires](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md).

## Les entreprises et les utilisateurs prennent désormais en charge les champs de formulaire personnalisés avancés.

>[!NOTE]
>
>Version d’aperçu : 14 mars 2024 ; Production pour tous les clients : 24.4 (avril 2024)

Les fonctionnalités avancées de formulaire personnalisé telles que les champs de recherche externe et les champs natifs Workfront sont désormais disponibles lorsque vous joignez un formulaire personnalisé à une entreprise ou à un utilisateur. Les fonctionnalités avancées sont disponibles dans les pages Détails de la société et Détails de l’utilisateur, et non dans les boîtes de dialogue Modifier la société et Modifier l’utilisateur . Le formulaire personnalisé doit être créé dans le nouveau concepteur de formulaire pour tirer parti de ces types de champs.

Pour plus d’informations sur les champs de formulaire personnalisés, voir [Concevoir un formulaire avec le concepteur de formulaires](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## L’intégration JumpSeat est désormais disponible pour les nouveaux types de modules.

>[!NOTE]
>
>Aperçu de la version : 26 février 2024 ; Production pour une version rapide : avec la version 24.3 (14 mars 2024) ; Production pour tous les clients : 24.4 (avril 2024)

L’intégration JumpSeat existante est désormais disponible pour les comptes utilisant l’un des nouveaux types de modules (c’est-à-dire Select, Prime ou Ultimate). Vous devez toujours disposer d’un abonnement JumpSeat actif pour activer l’intégration.

Pour plus d’informations sur l’intégration JumpSeat, voir [Configuration de l’intégration JumpSeat](/help/quicksilver/administration-and-setup/configure-integrations/configure-jumpseat.md).

## Les champs natifs de Workfront sont disponibles dans la version bêta du concepteur de formulaires

>[!NOTE]
>
>Aperçu de la version : 29 février 2024 ; Production pour une version rapide : avec la version 24.3 (14 mars 2024) ; Production pour tous les clients : 24.4 (avril 2024)

Les champs natifs de Workfront sont désormais disponibles pour l’ajout de dans vos formulaires personnalisés. Ce nouveau type de champ vous permet d’organiser et de présenter les données à vos utilisateurs de manière logique, sans avoir à recréer des données existantes dans des champs personnalisés.

Après avoir sélectionné Champ natif dans la liste des champs de formulaires personnalisés pour ajouter le champ au concepteur de formulaire, vous pouvez sélectionner n’importe quel champ natif pour les objets du formulaire. Par exemple, si la liste Types d’objet située en haut du concepteur de formulaire affiche Projet, vous pouvez sélectionner des champs natifs pour les projets, mais pas des champs spécifiques aux tâches.

Lorsque le formulaire personnalisé est associé à un objet, le champ est renseigné à partir des données de l’objet. Par exemple, le champ Description d’un formulaire personnalisé joint à un projet extrait la description du projet. (Le champ peut afficher &quot;S.O.&quot; si aucune donnée n’est disponible.)

Les champs natifs utilisés dans les formulaires personnalisés sont disponibles dans la bibliothèque de champs du concepteur pour réutilisation. Ils sont également visibles dans la zone Configuration > Forms personnalisée > Champs afin que vous puissiez voir dans quels formulaires ils sont utilisés.

Cette fonctionnalité est disponible uniquement en version bêta du concepteur de formulaire, et non dans l’ancien créateur de formulaires.

Pour plus d’informations, voir [Concevoir un formulaire avec le concepteur de formulaires](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

[Affichez une démonstration vidéo de cette fonctionnalité.](https://video.tv.adobe.com/v/3427702/){target=_blank}

## Mappage d’attributs désormais disponible pour les organisations qui ont migré vers Adobe IMS

>[!NOTE]
>
>Version d’aperçu : 22 février 2024 ; Production pour tous les clients : 22 février 2024

Les administrateurs système Workfront peuvent désormais configurer le mappage des attributs utilisateur pour les organisations qui ont migré vers Adobe IMS. Cela permet aux informations utilisateur de transmettre à Workfront à partir du fournisseur d’authentification unique (SSO) de l’organisation, de sorte que les données de l’utilisateur n’aient pas à être saisies à la fois dans Workfront et dans le fournisseur d’authentification unique.

Auparavant, cette fonctionnalité n’était disponible que pour les organisations qui n’étaient pas encore intégrées à Adobe IMS.

Pour plus d’informations sur la configuration du mappage des attributs, voir [Mise en correspondance des attributs utilisateur dans l’expérience unifiée Adobe](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/map-user-attributes.md#map-user-attributes-in-the-adobe-unified-experience) dans l’article **Mappage des attributs utilisateur et configuration automatique des nouveaux utilisateurs**.

## La logique de saut et la logique d’affichage sont désormais disponibles dans la version bêta du concepteur de formulaires.

>[!NOTE]
>
>Aperçu de la version : 8 février 2024 ; Production pour une version rapide : avec la version 24.2 (15 février 2024) ; Production pour tous les clients : À déterminer

Vous pouvez désormais modifier l’affichage existant, ignorer la logique et ajouter une nouvelle logique aux formulaires personnalisés dans la version bêta du concepteur de formulaires. Un générateur de logique convivial permet de définir les champs à afficher ou à ignorer en fonction des sélections dans le formulaire.

Les icônes d’un champ dans le canevas du concepteur de formulaire indiquent que la logique est configurée sur ce champ ou que le champ est utilisé dans les règles logiques configurées sur d’autres champs.

Pour plus d’informations, voir [Ajout d’une logique d’affichage et d’exclusion à l’aide du concepteur de formulaires](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md).
