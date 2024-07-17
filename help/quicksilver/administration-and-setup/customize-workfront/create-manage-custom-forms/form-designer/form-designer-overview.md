---
title: Vue d’ensemble du créateur de formulaires
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Vous pouvez concevoir un formulaire personnalisé que les utilisateurs et utilisatrices peuvent joindre à un objet Workfront. Les utilisateurs et utilisatrices qui travaillent sur l’objet peuvent remplir le formulaire personnalisé pour fournir des informations sur l’objet.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: c2e2901b-0558-4a63-ae3c-4c3a6edf0ff0
source-git-commit: 2a2f6d93c916863177d7a9d2f46f8124d1430354
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 82%

---

# Vue d’ensemble du créateur de formulaires

Vous pouvez utiliser le nouveau créateur de formulaires pour concevoir un formulaire personnalisé que les utilisateurs et utilisatrices peuvent joindre à un objet Workfront. Les utilisateurs et utilisatrices qui travaillent sur l’objet peuvent remplir le formulaire personnalisé pour fournir des informations sur l’objet.

Le nouveau créateur de formulaire dispose d’un nouvel espace de travail de style zone de travail qui vous permet d’afficher simultanément les champs, la zone de travail et les paramètres des champs. Il vous permet également de faire glisser des champs dans les sections lors de la conception de votre formulaire.

![Exemple de créateur de formulaires](assets/form-designer-example.png)

## Accès au concepteur de formulaires

Un bouton situé en haut du nouveau concepteur de formulaires et de l’ancien créateur de formulaires vous permet de basculer entre les versions.

![Passer au nouveau créateur de formulaires](assets/switch-views.png)

## Nouvelle fonctionnalité disponible avec le créateur de formulaires

Avec le nouveau créateur de formulaires, nous avons ajouté ces possibilités :

* **Copier un champ** : vous pouvez désormais copier des champs existants en cliquant sur l’icône Copier dans les champs directement depuis la zone de travail.

* **Modifier la taille du texte descriptif** : vous pouvez désormais choisir des petites, moyennes ou grandes tailles pour les champs de texte descriptif. Vous pouvez également les utiliser sur la même ligne avec d’autres champs.

* **Utiliser une section par défaut** : si la personne à l’origine du formulaire n’a pas ajouté de section en haut du formulaire, une section Par défaut est désormais visible dans la zone de travail, de sorte que les utilisateurs et utilisatrices puissent ajuster les autorisations pour les champs auxquels aucune section personnalisée n’est affectée.

  >[!NOTE]
  >
  >La section Par défaut n’est pas visible dans les objets lorsque le formulaire est joint à l’objet.

* **Utiliser un champ de recherche externe** : ce type de champ appelle une API externe et renvoie des valeurs sous forme d’options dans un champ de liste déroulante.

## Fonctionnalité supprimée du créateur de formulaires

Nous avons supprimé les fonctionnalités suivantes du créateur de formulaires :

* Les paramètres de formulaire sont désormais disponibles en haut de la zone de travail.

* Suivre les modifications de champ dans les messages de mise à jour

  >[!NOTE]
  >
  >Cette option est disponible dans Configuration > Interface > Mettre à jour les flux.

