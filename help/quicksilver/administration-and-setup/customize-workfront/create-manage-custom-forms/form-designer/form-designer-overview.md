---
title: Vue d’ensemble du créateur de formulaires
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Vous pouvez concevoir un formulaire personnalisé que les utilisateurs peuvent joindre à un objet Workfront. Les utilisateurs qui travaillent sur l’objet peuvent remplir le formulaire personnalisé pour fournir des informations sur l’objet.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: c2e2901b-0558-4a63-ae3c-4c3a6edf0ff0
source-git-commit: 2a2f6d93c916863177d7a9d2f46f8124d1430354
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 3%

---

# Vue d’ensemble du créateur de formulaires

Vous pouvez utiliser le nouveau concepteur de formulaire pour concevoir un formulaire personnalisé que les utilisateurs peuvent joindre à un objet Workfront. Les utilisateurs qui travaillent sur l’objet peuvent remplir le formulaire personnalisé pour fournir des informations sur l’objet.

Le nouveau concepteur de formulaire dispose d’un nouvel espace de travail de style zone de travail qui vous permet d’afficher simultanément les paramètres des champs, de la zone de travail et des champs. Il vous permet également de faire glisser des champs dans les sections lors de la conception de votre formulaire.

![Concepteur d’exemple de formulaire](assets/form-designer-example.png)

## Accès au concepteur de formulaires

Un bouton situé en haut du nouveau concepteur de formulaires et de l’ancien créateur de formulaires vous permet de basculer entre les versions.

![Passer au nouveau concepteur de formulaires](assets/switch-views.png)

## Nouvelle fonctionnalité disponible avec le concepteur de formulaires

Avec le nouveau concepteur de formulaires, nous avons ajouté la possibilité de :

* **Copier un champ**: vous pouvez désormais copier des champs existants en cliquant sur l’icône Copier dans les champs directement depuis la zone de travail.

* **Modifier la taille du texte descriptif**: vous pouvez désormais affecter des petites, moyennes ou grandes tailles aux champs de texte descriptif. Vous pouvez également les utiliser sur la même ligne avec d’autres champs.

* **Utilisation d’une section par défaut**: si l’auteur du formulaire n’a pas ajouté de section en haut du formulaire, une section Par défaut est désormais visible dans la zone de travail, de sorte que les utilisateurs puissent ajuster les autorisations pour les champs auxquels aucune section personnalisée n’est affectée.

  >[!NOTE]
  >
  >La section Par défaut n’est pas visible dans les objets lorsque le formulaire est joint à l’objet.

* **Utilisation d’un champ de recherche externe**: ce type de champ appelle une API externe et renvoie les valeurs sous forme d’options dans un champ de liste déroulante.

## Fonctionnalité supprimée du concepteur de formulaires

Nous avons supprimé les fonctionnalités suivantes du concepteur de formulaires :

* Les paramètres de formulaire sont désormais disponibles en haut de la zone de travail.

* Suivre les modifications de champ dans les messages de mise à jour

  >[!NOTE]
  >
  >Cette option est disponible dans Configuration > Interface > Mettre à jour les flux.

