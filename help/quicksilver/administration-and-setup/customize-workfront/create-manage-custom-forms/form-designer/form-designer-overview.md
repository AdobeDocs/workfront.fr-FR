---
title: Présentation du concepteur de formulaires
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Vous pouvez concevoir un formulaire personnalisé que les utilisateurs peuvent joindre à un objet Workfront. Les utilisateurs qui travaillent sur l’objet peuvent remplir le formulaire personnalisé pour fournir des informations sur l’objet.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: c2e2901b-0558-4a63-ae3c-4c3a6edf0ff0
source-git-commit: 061d1a08a8c99b2770491ce2fcea63a9dad7a63f
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 1%

---

# Présentation du concepteur de formulaires

>[!IMPORTANT]
>
>Le concepteur de formulaire a été temporairement désactivé le 24 mai 2023. Vous pouvez utiliser l’ancien créateur de formulaires pour créer et modifier vos formulaires personnalisés. Voir [Création ou modification d’un formulaire personnalisé avec le créateur de formulaires hérité](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/use-the-custom-form-builder.md).

Vous pouvez utiliser le nouveau concepteur de formulaire pour concevoir un formulaire personnalisé que les utilisateurs peuvent joindre à un objet Workfront. Les utilisateurs qui travaillent sur l’objet peuvent remplir le formulaire personnalisé pour fournir des informations sur l’objet.

Le nouveau concepteur de formulaire dispose d’un nouvel espace de travail de style zone de travail qui vous permet d’afficher simultanément les paramètres des champs, de la zone de travail et des champs. Il vous permet également de faire glisser des champs dans les sections lors de la conception de votre formulaire.

<!-- add screenshot when field settings empty state is ready -->

## Accès au nouveau concepteur de formulaires

Il existe un nouveau bouton en haut du nouveau concepteur de formulaire et de l’ancien créateur de formulaires. Vous pouvez utiliser ce bouton pour basculer entre le créateur hérité et le nouveau concepteur.

![](assets/switch-views.png)

## Nouvelle fonctionnalité disponible avec le concepteur de formulaires

Avec le nouveau concepteur de formulaires, nous avons ajouté la possibilité d’utiliser

* **Copier un champ**: Vous pouvez désormais copier des champs existants en cliquant sur l’icône Copier dans les champs directement depuis la zone de travail.

* **Modifier la taille du texte descriptif**: Vous pouvez désormais affecter des petites, moyennes ou grandes tailles aux champs de texte descriptif. Vous pouvez également les utiliser sur la même ligne avec d’autres champs.

* **Utilisation d’une section par défaut**: Si l’auteur du formulaire n’a pas ajouté de section en haut du formulaire, une section Par défaut est désormais visible dans la zone de travail, de sorte que les utilisateurs puissent ajuster les autorisations pour les champs auxquels aucune section personnalisée n’est affectée.

   >[!NOTE]
   >
   >La section par défaut n’est pas visible dans les objets lorsque le formulaire est joint à l’objet.

## Fonctionnalité bientôt disponible

Les éléments suivants ne sont actuellement pas disponibles dans le concepteur de formulaires, mais seront bientôt ajoutés :

* Afficher/Ignorer la logique

* Filtre pour les champs de saisie anticipée

>[!IMPORTANT]
>
>Les configurations existantes pour les filtres de logique et de type anticipé ne seront pas affectées lorsque vous travaillerez avec le nouveau concepteur de formulaires.

## Fonctionnalité supprimée du concepteur de formulaires

Nous avons supprimé les fonctionnalités suivantes du concepteur de formulaires :


* Onglets Paramètres de formulaire, Partage de formulaires, Partage de champs

   * Les paramètres de formulaire sont désormais disponibles en haut de la zone de travail.

   * Panneau principal Partage de formulaires et sous-onglet Partage de champs
   >[!NOTE]
   >
   >Vous pouvez contrôler le partage de formulaire et de champ à partir de l’onglet Configuration > Forms personnalisé > Forms ou Champs .

* Suivre les modifications de champ dans les messages de mise à jour
   >[!NOTE]
   >
   >Vous pouvez le trouver dans Configuration > Interface > Mettre à jour les flux.
