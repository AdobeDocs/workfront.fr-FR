---
title: Présentation du concepteur de formulaires
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Vous pouvez concevoir un formulaire personnalisé que les utilisateurs peuvent joindre à un objet Workfront. Les utilisateurs qui travaillent sur l’objet peuvent remplir le formulaire personnalisé pour fournir des informations sur l’objet.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: c2e2901b-0558-4a63-ae3c-4c3a6edf0ff0
source-git-commit: e34a0b3bf5e2c4dc794a7d7c85245bb4d11842be
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 1%

---

# Présentation du concepteur de formulaires

Vous pouvez utiliser le nouveau concepteur de formulaire pour concevoir un formulaire personnalisé que les utilisateurs peuvent joindre à un objet Workfront. Les utilisateurs qui travaillent sur l’objet peuvent remplir le formulaire personnalisé pour fournir des informations sur l’objet.

Le nouveau concepteur de formulaire dispose d’un nouvel espace de travail de style zone de travail qui vous permet d’afficher simultanément les paramètres des champs, de la zone de travail et des champs. Il vous permet également de faire glisser des champs dans les sections lors de la conception de votre formulaire.

<!-- add screenshot when field settings empty state is ready -->

## Accès au nouveau concepteur de formulaires

Il existe un nouveau bouton en haut du nouveau concepteur de formulaire et de l’ancien créateur de formulaires. Vous pouvez utiliser ce bouton pour basculer entre le créateur hérité et le nouveau concepteur.

![Passer au nouveau concepteur de formulaires](assets/switch-views.png)

## Nouvelle fonctionnalité disponible avec le concepteur de formulaires

Avec le nouveau concepteur de formulaires, nous avons ajouté la possibilité de :

* **Copier un champ**: vous pouvez désormais copier des champs existants en cliquant sur l’icône Copier dans les champs directement depuis la zone de travail.

* **Modifier la taille du texte descriptif**: vous pouvez désormais affecter des petites, moyennes ou grandes tailles aux champs de texte descriptif. Vous pouvez également les utiliser sur la même ligne avec d’autres champs.

* **Utilisation d’une section par défaut**: si l’auteur du formulaire n’a pas ajouté de section en haut du formulaire, une section Par défaut est désormais visible dans la zone de travail, de sorte que les utilisateurs puissent ajuster les autorisations pour les champs auxquels aucune section personnalisée n’est affectée.

  >[!NOTE]
  >
  >La section par défaut n’est pas visible dans les objets lorsque le formulaire est joint à l’objet.

## Fonctionnalité bientôt disponible

Les éléments suivants ne sont actuellement pas disponibles dans le concepteur de formulaires, mais seront bientôt ajoutés :

* Filtre pour les champs de saisie anticipée

>[!IMPORTANT]
>
>Les configurations existantes pour les filtres de saisie anticipée ne seront pas affectées lorsque vous travaillerez avec le nouveau concepteur de formulaires.

## Fonctionnalité supprimée du concepteur de formulaires

Nous avons supprimé les fonctionnalités suivantes du concepteur de formulaires :

* Onglets Paramètres de formulaire, Partage de formulaires, Partage de champs

   * Les paramètres de formulaire sont désormais disponibles en haut de la zone de travail.

   * Panneau principal Partage de formulaires et sous-onglet Partage de champs

  >[!NOTE]
  >
  >Vous pouvez contrôler le partage des formulaires et des champs à partir de Configuration > Forms personnalisé > Forms ou de la zone Champs .

* Suivre les modifications de champ dans les messages de mise à jour

  >[!NOTE]
  >
  >Vous pouvez le trouver dans Configuration > Interface > Mettre à jour les flux.
