---
title: Types d’enregistrements centralisés - Aperçu
description: Les types d’enregistrements centralisés peuvent être ajoutés à plusieurs espaces de travail à partir d’un espace de travail principal ou central dans Adobe Workfront Planning.
hidefromtoc: true
hide: true
source-git-commit: 9b95b5a52576327a3df8d6955925b96c2e45848f
workflow-type: tm+mt
source-wordcount: '1019'
ht-degree: 1%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
-->

# Types d’enregistrements centralisés - Aperçu

Les types d’enregistrements centralisés peuvent être ajoutés à plusieurs espaces de travail à partir d’un espace de travail principal ou central dans Adobe Workfront Planning.

## Présentation des types d’enregistrements centralisés

Lors de l’implémentation de Workfront Planning pour une organisation multi-équipes avec des workflows communs, vous devrez peut-être définir une structure et des métadonnées cohérentes pour les types d’enregistrements clés (tels que les campagnes ou les éléments livrables) qui peuvent être ajoutés aux espaces de travail de chaque équipe pour capturer et gérer leur travail.

En outre, vous aurez peut-être besoin du travail de chaque équipe pour atteindre un niveau central.

Dans un tel workflow, vous pouvez vous assurer que les équipes capturent leur travail de manière cohérente tout en déverrouillant la visibilité entre les équipes, sans avoir à tout ajouter à un espace de travail ou à tous les membres de l’organisation à chaque espace de travail. Pour ce faire, vous pouvez utiliser des types d’enregistrements centralisés.

Pour utiliser des types d’enregistrements centralisés, procédez comme suit :

1. Configurez un type d’enregistrement à centraliser dans un espace de travail spécifique.

   Un responsable d’espace de travail peut sélectionner des utilisateurs disposant d’une licence standard, des équipes, des groupes, des rôles ou des sociétés afin d’ajouter un type d’enregistrement sélectionné aux espaces de travail qu’il gère.

   Le type d’enregistrement d’origine existe dans son espace de travail d’origine, mais est rendu visible à partir de tous les autres espaces de travail.

   Pour plus d’informations, voir [Configuration des fonctionnalités de plusieurs espaces de travail pour les types d’enregistrements](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).
1. Ajoutez un type d’enregistrement existant à partir d’un type existant qui a été configuré en tant que type centralisé dans l’espace de travail d’une équipe.

   Le type d’enregistrement existe dans les espaces de travail suivants :

   * Son espace de travail d’origine où il a été désigné comme type d’enregistrement centralisé.
   * Espace de travail de l’équipe.

   Pour plus d’informations, voir [ Ajouter des types d’enregistrements existants ](/help/quicksilver/planning/architecture/add-cross-workspace-record-types.md).

   Les sections suivantes décrivent les points à prendre en compte concernant les types d’enregistrements centralisés dans leurs espaces de travail d’origine ou après leur ajout aux espaces de travail d’une équipe.

## Considérations sur les types d’enregistrements centralisés dans leur espace de travail d’origine

Le type d’enregistrement configuré pour être centralisé présente les propriétés suivantes :

* Toutes ses informations ne peuvent être modifiées que dans l’espace de travail d’origine.

* Vous pouvez effectuer les actions suivantes sur le type d’enregistrement centralisé à partir de l’espace de travail d’origine d’un type d’enregistrement centralisé :

   * Le modifier.

     La modification d’un type d’enregistrement centralisé comprend la modification de son apparence, des fonctionnalités de plusieurs espaces de travail et de tous les champs créés dans l’espace de travail d’origine.
   * Création de formulaires de demande
   * Gérer les formulaires de demande

* Vous ne pouvez supprimer un type d’enregistrement centralisé que s’il n’a pas été ajouté à un espace de travail d’équipe. Une fois qu’il a été ajouté à l’espace de travail d’une équipe, essayer de le supprimer de l’espace de travail d’origine génère une erreur.

  Cela permet au type d’enregistrement centralisé de rester dans les espaces de travail où il a déjà été ajouté.
* Les enregistrements que vous ajoutez à un type d&#39;enregistrement centralisé ne sont visibles que par les utilisateurs qui disposent des autorisations d&#39;affichage sur son espace de travail d&#39;origine.
* Les enregistrements que vous ajoutez à partir de l’espace de travail de l’équipe sont cumulés et affichés dans l’espace de travail d’origine. Tous les membres de l’espace de travail d’origine y obtiennent des autorisations d’affichage.

* Les types d’enregistrement connectés d’un type d’enregistrement centralisé seront disponibles pour la connexion à partir des espaces de travail où ce type d’enregistrement est ajouté.

* Les champs créés pour un type d’enregistrement centralisé à partir de l’espace de travail d’origine sont visibles de tous les espaces de travail où le type d’enregistrement est ajouté.

## Considérations sur les types d’enregistrements centralisés après les avoir ajoutés à l’espace de travail d’une équipe

* Les contributeurs à l’espace de travail d’équipe obtiennent l’autorisation Contribuer au type d’enregistrement centralisé dans l’espace de travail d’équipe. Il peut y ajouter et y gérer des enregistrements.

* Les observateurs de l’espace de travail d’équipe obtiennent l’autorisation d’affichage du type d’enregistrement centralisé dans l’espace de travail d’équipe. Ils ne peuvent pas ajouter ni gérer d’enregistrements dans .

* Les responsables d&#39;espace de travail d&#39;équipe peuvent effectuer les actions suivantes sur le type d&#39;enregistrement ajouté à partir d&#39;un type d&#39;enregistrement centralisé dans l&#39;espace de travail d&#39;une équipe :

   * Ajouter de nouveaux champs

     Les champs ajoutés à un enregistrement centralisé à partir de l’espace de travail d’équipe sont visibles uniquement à partir de l’espace de travail de l’équipe.
   * Partager
   * Supprimez-le.

     La suppression du type d’enregistrement de l’espace de travail d’une équipe le supprime uniquement de l’espace de travail de l’équipe. Les enregistrements qui y ont été ajoutés à partir de l’espace de travail de l’équipe sont également supprimés. Cela ne supprime pas le type d’enregistrement de son espace de travail d’origine ou de tout autre espace de travail d’équipe où il a été ajouté.

     Cette opération est effectuée de sorte qu’il soit possible de conserver le type d’enregistrement centralisé déjà ajouté dans les espaces de travail qui l’utilisent déjà.

* Vous ne pouvez pas effectuer les actions suivantes sur le type d’enregistrement ajouté à partir d’un type d’enregistrement centralisé dans l’espace de travail d’une équipe :

   * Le modifier.

     Vous ne pouvez pas modifier son apparence, les fonctionnalités de l’espace de travail croisé ou les champs importés de l’espace de travail d’origine.
   * Création de formulaires de demande
   * Gérer les formulaires de demande

* Les enregistrements ajoutés dans les espaces de travail d&#39;une équipe sont visibles à partir des espaces de travail suivants, si vous disposez d&#39;autorisations d&#39;affichage ou supérieures pour ces espaces de travail :

   * Espace de travail de l’équipe dans lequel ils sont ajoutés.
   * Espace de travail d’origine du type d’enregistrement centralisé.
   * Tous les autres espaces de travail auxquels l’espace de travail centralisé est ajouté.

* Les scénarios suivants existent pour les enregistrements créés dans les espaces de travail des équipes :

   * Si vous disposez des autorisations de niveau Gérer sur l’espace de travail d’origine et pas d’autorisations sur les espaces de travail des équipes, vous pouvez afficher les enregistrements ajoutés depuis les espaces de travail de l’équipe dans l’espace de travail d’origine, mais vous ne pouvez pas les gérer depuis l’espace de travail d’origine.
   * Si vous disposez des autorisations de niveau Gérer sur l’espace de travail de l’équipe, vous pouvez gérer les enregistrements dans l’espace de travail d’origine du type d’enregistrement centralisé ou à partir de l’espace de travail où ils ont été ajoutés.

     Vous pouvez afficher les enregistrements dans des espaces de travail d&#39;équipe supplémentaires où le type d&#39;enregistrement centralisé est ajouté uniquement si vous disposez des autorisations d&#39;affichage sur ces espaces de travail.

## Accès aux connexions

Les types d’enregistrement connectés au type d’enregistrement centralisé dans l’espace de travail d’origine deviennent visibles pour les espaces de travail d’équipe où le type d’enregistrement centralisé est ajouté.

## Comportement de l’API

Lors de l’ajout d’enregistrements à un type d’enregistrement centralisé à partir d’un espace de travail d’équipe à l’aide de l’API Workfront Planning, le système vérifie si l’utilisateur a accès à la création d’enregistrements dans l’espace de travail d’origine du type d’enregistrement centralisé.

Les cas suivants existent :

* Si l’utilisateur y a accès, l’enregistrement est créé dans l’espace de travail d’origine des types d’enregistrements centralisés.

* Si l’utilisateur n’y a pas accès, il est prévenu qu’il n’a pas accès à l’espace de travail d’origine du type d’enregistrement centralisé et qu’il doit fournir l’identifiant de l’espace de travail auquel il a accès pour créer des enregistrements.