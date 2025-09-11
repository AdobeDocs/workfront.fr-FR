---
title: Types d’enregistrements de l’espace de travail croisé - Aperçu
description: Les types d’enregistrements centralisés peuvent être ajoutés à plusieurs espaces de travail à partir d’un espace de travail principal ou central dans Adobe Workfront Planning.
hidefromtoc: true
hide: true
source-git-commit: ff5bc262a5ed2a22099c058ebdb61bc32485b201
workflow-type: tm+mt
source-wordcount: '1320'
ht-degree: 1%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
-->

# Types d’enregistrements de l’espace de travail croisé - Aperçu

Dans Adobe Workfront Planning, vous pouvez activer les fonctionnalités inter-espaces de travail pour un type d’enregistrement qui vous permet de référencer un type d’enregistrement dans plusieurs espaces de travail.

Vous trouverez ci-dessous des fonctionnalités inter-espaces de travail de types d’enregistrements :

* Vous pouvez désigner un type d’enregistrement comme centralisé. Les utilisateurs peuvent ajouter des types d’enregistrements centralisés à d’autres espaces de travail qu’ils peuvent gérer.
* Vous pouvez désigner un type d’enregistrement comme connectable. Les utilisateurs peuvent se connecter à ce type d’enregistrement à partir d’autres espaces de travail.

Cet article vous donne un aperçu des types d’enregistrements de l’ensemble des espaces de travail. Pour plus d’informations sur la définition des fonctionnalités inter-espaces de travail d’un type d’enregistrement, voir [Configuration des fonctionnalités inter-espaces de travail pour les types d’enregistrements](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).


## Présentation des types d’enregistrements centralisés

Les types d’enregistrements centralisés peuvent être ajoutés à plusieurs espaces de travail à partir d’un espace de travail principal ou central dans Adobe Workfront Planning.

Lors de l’implémentation de Workfront Planning pour une organisation multi-équipes avec des workflows communs, vous devrez peut-être définir une structure et des métadonnées cohérentes pour les types d’enregistrements clés (tels que les campagnes ou les éléments livrables) qui peuvent être ajoutés aux espaces de travail de chaque équipe pour capturer et gérer leur travail.

En outre, vous aurez peut-être besoin du travail de chaque équipe pour atteindre un niveau central.

Dans un tel workflow, vous pouvez vous assurer que les équipes capturent leur travail de manière cohérente tout en déverrouillant la visibilité entre les équipes, sans avoir à tout ajouter à un espace de travail ou à tous les membres de l’organisation à chaque espace de travail. Pour ce faire, vous pouvez utiliser des types d’enregistrements centralisés.

Pour utiliser des types d’enregistrements centralisés, procédez comme suit :

1. Configurez un type d’enregistrement à centraliser dans un espace de travail spécifique.

   Un responsable d’espace de travail peut sélectionner des utilisateurs disposant d’une licence standard, des équipes, des groupes, des rôles ou des sociétés afin d’ajouter un type d’enregistrement sélectionné aux espaces de travail qu’il gère.

   Le type d’enregistrement d’origine existe dans son espace de travail d’origine, mais est rendu visible à partir de tous les autres espaces de travail.

   Pour plus d’informations, voir [Configuration des fonctionnalités de plusieurs espaces de travail pour les types d’enregistrements](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).
1. Ajoutez un type d’enregistrement existant à partir d’un type d’enregistrement existant qui a été configuré en tant que type d’enregistrement centralisé vers un espace de travail secondaire.

   Le type d’enregistrement existe dans les espaces de travail suivants :

   * Son espace de travail d’origine où il a été désigné comme type d’enregistrement centralisé.
   * Un espace de travail secondaire.

   Pour plus d’informations, voir [Ajouter des types d’enregistrements existants depuis un autre espace de travail](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md).

   Les sections suivantes présentent des considérations sur les types d’enregistrements centralisés et leur fonctionnement dans leurs espaces de travail d’origine ou secondaires.

### Considérations sur les types d’enregistrements centralisés dans leur espace de travail d’origine

Le type d’enregistrement configuré pour être centralisé présente les propriétés suivantes :

* Toutes ses informations ne peuvent être modifiées que dans l’espace de travail d’origine.

* Vous pouvez effectuer les actions suivantes sur le type d’enregistrement centralisé à partir de l’espace de travail d’origine d’un type d’enregistrement centralisé :

   * Le modifier.

     La modification d’un type d’enregistrement centralisé comprend la modification de son apparence, des fonctionnalités de plusieurs espaces de travail et de tous les champs créés dans l’espace de travail d’origine.
   * Création de formulaires de demande
   * Gérer les formulaires de demande

* Vous ne pouvez supprimer un type d’enregistrement centralisé que s’il n’a pas été ajouté à un espace de travail secondaire. Une fois qu’il a été ajouté à un autre espace de travail, essayer de le supprimer de l’espace de travail d’origine génère une erreur.

  Cela permet au type d’enregistrement centralisé de rester dans les espaces de travail où il a déjà été ajouté.
* Les enregistrements que vous ajoutez à un type d&#39;enregistrement centralisé sont visibles uniquement pour les utilisateurs qui disposent des autorisations d&#39;affichage de l&#39;espace de travail dans lequel ils ont été ajoutés.
* Les enregistrements que vous ajoutez à partir d’un espace de travail secondaire sont cumulés et affichés dans l’espace de travail d’origine. Tous les membres de l’espace de travail d’origine y obtiennent des autorisations d’affichage.

* Les types d’enregistrement connectés d’un type d’enregistrement centralisé seront disponibles pour la connexion à partir des espaces de travail où ce type d’enregistrement est ajouté.

  Par exemple, si vous disposez d’un type d’enregistrement Campaign ayant une connexion avec le type d’enregistrement Régions et que vous ajoutez le type d’enregistrement Campaign à un espace de travail secondaire, les régions pourront être connectées sur plusieurs espaces de travail pour l’espace de travail secondaire. Les membres secondaires de l’espace de travail peuvent désormais créer des campagnes et les lier à des régions.

* Les champs créés pour un type d’enregistrement centralisé à partir de l’espace de travail d’origine sont visibles de tous les espaces de travail où le type d’enregistrement est ajouté. Les champs d’un espace de travail d’origine sont en lecture seule dans les espaces de travail secondaires.

### Considérations relatives aux types d’enregistrements centralisés après les avoir ajoutés à un espace de travail secondaire

* Les contributeurs à l’espace de travail Secondaire obtiennent l’autorisation de contribution pour le type d’enregistrement centralisé dans l’espace de travail de leur équipe. Il peut y ajouter et y gérer des enregistrements.

* Les visionneuses d’espace de travail Secondaire obtiennent l’autorisation d’affichage du type d’enregistrement centralisé dans l’espace de travail de leur équipe. Ils ne peuvent pas ajouter ni gérer d’enregistrements dans .

* Les gestionnaires d’espace de travail Secondaire peuvent effectuer les actions suivantes sur le type d’enregistrement ajouté à partir d’un type d’enregistrement centralisé dans un espace de travail secondaire :

   * Supprimez-le.

     La suppression du type d’enregistrement d’un espace de travail secondaire le supprime uniquement de l’espace de travail secondaire. Les enregistrements qui y ont été ajoutés à partir de l’espace de travail secondaire sont également supprimés. Le type d’enregistrement n’est pas supprimé de son espace de travail d’origine ni de tout autre espace de travail secondaire où il a été ajouté.

  <!--These two capabilities will come later:
    * Add new fields
        Fields added to a centralized record from a secondary workspace are visible only from the secondary workspace. 
    * Share it-->

* Vous ne pouvez pas effectuer les actions suivantes sur le type d’enregistrement ajouté à partir d’un type d’enregistrement centralisé dans un espace de travail secondaire :

   * Le modifier.

     Vous ne pouvez pas modifier son apparence, les fonctionnalités de l’espace de travail croisé ou les champs ajoutés à partir de l’espace de travail d’origine.
   * Créer et gérer des formulaires de demande
   * Création et gestion de formulaires de demande

* Les enregistrements ajoutés dans un espace de travail secondaire sont visibles à partir des espaces de travail suivants, si vous disposez d&#39;autorisations d&#39;affichage ou supérieures pour ces espaces de travail :

   * Espace de travail secondaire dans lequel ils sont ajoutés.
   * Espace de travail d’origine du type d’enregistrement centralisé.
   * Tous les autres espaces de travail auxquels l’espace de travail centralisé est ajouté.

* Les scénarios suivants existent pour les enregistrements créés dans les espaces de travail des équipes :

   * Si vous disposez d’autorisations de niveau Gérer sur l’espace de travail d’origine et d’aucune autorisation sur un espace de travail secondaire, vous pouvez afficher les enregistrements ajoutés à partir des espaces de travail secondaires dans l’espace de travail d’origine, mais vous ne pouvez pas les gérer à partir de l’espace de travail d’origine.
   * Si vous disposez des autorisations de niveau Gérer sur l’espace de travail secondaire, vous pouvez gérer les enregistrements dans l’espace de travail d’origine du type d’enregistrement centralisé ou à partir de l’espace de travail où ils ont été ajoutés.

     Vous pouvez afficher les enregistrements dans des espaces de travail secondaires supplémentaires où le type d&#39;enregistrement centralisé est ajouté uniquement si vous disposez des autorisations d&#39;affichage pour ces espaces de travail.

### Accès aux connexions d&#39;un type d&#39;enregistrement centralisé

Les types d’enregistrements connectés au type d’enregistrement centralisé dans l’espace de travail d’origine deviennent visibles à partir d’autres espaces de travail où le type d’enregistrement centralisé est ajouté.

### Accès API d’un type d’enregistrement centralisé

Lors de l’ajout d’enregistrements à un type d’enregistrement centralisé à partir d’un espace de travail secondaire à l’aide de l’API Workfront Planning, le système vérifie si l’utilisateur a accès à la création d’enregistrements dans l’espace de travail d’origine du type d’enregistrement centralisé.

Les cas suivants existent :

* Si l’utilisateur y a accès, l’enregistrement est créé dans l’espace de travail d’origine des types d’enregistrements centralisés.

* Si l’utilisateur n’y a pas accès, il est prévenu qu’il n’a pas accès à l’espace de travail d’origine du type d’enregistrement centralisé et qu’il doit fournir l’identifiant de l’espace de travail auquel il a accès pour créer des enregistrements.

## Présentation des types d’enregistrements connectables

Vous pouvez vous connecter à un type d’enregistrement défini comme pouvant être connecté à partir de n’importe quel espace de travail que vous gérez.

Vos équipes peuvent avoir besoin que leurs enregistrements soient liés à des types d&#39;enregistrements d&#39;autres espaces de travail ou afficher des informations capturées sur des enregistrements appartenant à des enregistrements d&#39;autres espaces de travail. Vous pouvez effectuer cette configuration en désignant un type d’enregistrement comme connectable.

Pour utiliser des types d’enregistrements connectables, procédez comme suit :

1. Configurez un type d’enregistrement à connecter dans un espace de travail spécifique.

   Un gestionnaire d’espace de travail peut sélectionner les espaces de travail auxquels un type d’enregistrement désigné peut se connecter.

   Le type d’enregistrement d’origine existe dans son espace de travail d’origine et est ajouté en tant que type d’enregistrement connecté à un autre espace de travail.

   Pour plus d’informations, voir [Configuration des fonctionnalités de plusieurs espaces de travail pour les types d’enregistrements](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).
1. Connectez-vous à un type d’enregistrement désigné comme connectable à partir d’un autre espace de travail que vous gérez.

   Pour plus d’informations, consultez la section [Connecter des types d’enregistrements](/help/quicksilver/planning/architecture/connect-record-types.md).

   Les sections suivantes présentent des considérations sur les types d’enregistrements centralisés et leur fonctionnement dans leurs espaces de travail d’origine ou secondaires.