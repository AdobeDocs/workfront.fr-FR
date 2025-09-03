---
title: Types d’enregistrements centralisés - Aperçu
description: Les types d’enregistrements centralisés peuvent être ajoutés à plusieurs espaces de travail à partir d’un espace de travail principal ou central dans Adobe Workfront Planning.
hidefromtoc: true
hide: true
source-git-commit: 4e295b4fdbbde7439567ef2a4f4383ad8dea738c
workflow-type: tm+mt
source-wordcount: '841'
ht-degree: 0%

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

En outre, vous aurez peut-être besoin du travail de chaque équipe pour atteindre un niveau central, plus global.

Dans ce workflow, vous pouvez vous assurer que les équipes capturent leur travail de manière cohérente tout en déverrouillant la visibilité entre les équipes, sans avoir à ajouter tous les membres de l’organisation à un seul espace de travail.

Pour utiliser des types d’enregistrements centralisés, procédez comme suit :

1. Configurez un type d’enregistrement à centraliser.

   Pour plus d’informations, consultez [Configuration des fonctionnalités de l’espace de travail croisé pour les types d’enregistrements](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).
1. Ajouter un type d’enregistrement existant à partir d’un enregistrement centralisé.

   Pour plus d’informations, voir [ Ajouter des types d’enregistrements existants ](/help/quicksilver/planning/architecture/add-cross-workspace-record-types.md).




· Un nouveau paramètre « Autoriser l’ajout du type d’enregistrement dans d’autres espaces de travail » est disponible dans les Paramètres avancés pour les types d’enregistrement.

· Si cette option est activée, le responsable d’espace de travail peut sélectionner des utilisateurs disposant d’une licence standard, des équipes, des groupes, des rôles ou des sociétés qui peuvent ajouter le type d’enregistrement dans les espaces de travail qu’ils gèrent.

· Le gestionnaire d’espace de travail qui modifie le paramètre sera automatiquement ajouté par défaut à la liste des utilisateurs sélectionnés

o Le gestionnaire d’espace de travail peut supprimer son propre nom après avoir ajouté au moins une autre entité

o Au moins 1 utilisateur/équipe/... doit être sélectionné(e) pour enregistrer le paramètre

o Une fois le type d’enregistrement ajouté dans au moins 1 autre espace de travail, tous les utilisateurs sélectionnés peuvent être supprimés

§ Cela permet d’éviter d’ajouter le type d’enregistrement global dans de nouveaux espaces de travail, mais de le conserver dans les espaces de travail qui l’utilisent déjà.

· Lors de la phase 1, tous les enregistrements des types d’enregistrements connectés sont automatiquement partagés avec tout espace de travail où le type d’enregistrement a été ajouté.

· Une fois que le type d’enregistrement est activé pour l’espace de travail, un champ « Workspace » généré par le système est ajouté au type d’enregistrement

o Affiche l’espace de travail à partir duquel chaque enregistrement a été créé.

o Ce champ est en lecture seule et ne peut pas être supprimé.

o Il peut être masqué des champs d’affichage.

o Le champ de l’espace de travail peut être utilisé à des fins de filtrage, de regroupement et de tri, ainsi que dans n’importe quel paramètre d’affichage, comme d’autres champs.


Types d’enregistrements cross-Workspace dans les espaces de travail locaux

· Lorsque vous essayez d’ajouter un nouveau type d’enregistrement à leur espace de travail, les responsables locaux de l’espace de travail voient une option permettant de sélectionner les types d’enregistrement globaux disponibles pour eux

· Lorsqu’ils sélectionnent l’un des types d’enregistrements globaux, il est immédiatement ajouté à l’espace de travail

· Il est possible de déplacer le type d’enregistrement global vers n’importe quelle section et position dans l’espace de travail local


Autorisations relatives au type d’enregistrement global dans les espaces de travail locaux

Dans les espaces de travail locaux, les membres obtiennent l’accès suivant au type d’enregistrement global :

· Au cours de la phase 1, les responsables locaux de l’espace de travail obtiennent l’autorisation Contribuer. Cela signifie :

o Les responsables de l’espace de travail local peuvent :

§ Ajouter le type d’enregistrement global

§ Ajouter/modifier/supprimer des enregistrements dans le type d’enregistrement global, quel que soit l’espace de travail à partir duquel l’enregistrement a été ajouté.

§ Supprimer le type d’enregistrement global de leur espace de travail local

o Les gestionnaires de l’espace de travail local ne peuvent pas :

§ Ajouter, modifier et supprimer des champs

§ Mettre à jour l’apparence et le libellé du type d’enregistrement

§ Voir les paramètres avancés pour le type d’enregistrement

§ Gérer les automatisations

§ Gérer les formulaires de demande

§ Ajuster le partage du type d’enregistrement pour la portée de leur espace de travail

§ Désactivez le paramètre de type d’enregistrement global dans les paramètres avancés.

· Les contributeurs de l’espace de travail local obtiennent l’autorisation de Contribuer au type d’enregistrement global et peuvent y ajouter et gérer des enregistrements

· Les observateurs de l’espace de travail local obtiennent l’autorisation d’affichage sur le type d’enregistrement global

· Dès qu’un enregistrement est ajouté au type d’enregistrement global à partir de l’un des espaces de travail locaux, le champ Workspace affiche ce nom d’espace de travail

o Pour l’instant, il n’est pas possible de modifier le champ Workspace

· Les enregistrements ajoutés aux espaces de travail locaux sont tous cumulés et affichés dans l’espace de travail principal, et tous les membres de l’espace de travail principal y ont accès en affichage.

· Les enregistrements ajoutés dans les espaces de travail locaux ne sont pas affichés dans d&#39;autres espaces de travail locaux utilisant le même type d&#39;enregistrement global et leurs membres n&#39;ont pas accès aux enregistrements.



Accès aux connexions :

· Portée du MVP

o Les types d’enregistrement connectés au type d’enregistrement global seront visibles pour les espaces de travail locaux où le type d’enregistrement global est ajouté, afin qu’ils puissent utiliser les champs de connexion pour marquer


Comportement de l’API

Si l’utilisateur tente de créer des enregistrements dans un type d’enregistrement global via l’API sans fournir l’identifiant de l’espace de travail, le système vérifie si l’utilisateur a accès à la création d’enregistrements dans l’espace de travail principal (où le type d’enregistrement global est créé)

· Si oui, l&#39;enregistrement est créé dans l&#39;espace de travail principal

· Si la réponse est non, l’utilisateur ou l’utilisatrice reçoit une erreur de validation indiquant qu’il n’a pas accès à l’espace de travail principal et qu’il doit fournir l’identifiant de l’espace de travail où il est autorisé à créer.