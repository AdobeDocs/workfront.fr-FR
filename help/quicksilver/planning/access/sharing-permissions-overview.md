---
title: Vue d’ensemble du partage d’autorisations dans Adobe Workfront Planning
description: Vous pouvez partager ou supprimer des autorisations sur un espace de travail ou une vue Adobe Workfront Planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
el-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
exl-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
source-git-commit: 402fb9d279fec258390535100e8f3d2c3c1b913b
workflow-type: tm+mt
source-wordcount: '692'
ht-degree: 65%

---

<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Workfront Planning. This article describes the levels of access that users could have to Adobe Workfront Planning. -->

<!--over time, this article should look like this one does: https://eperienceleague.adobe.com/docs/workfront/using/basics/grant-request-object-permissions/sharing-permissions-on-objects-overview.html?lang=en-->

# Vue d’ensemble du partage d’autorisations dans Adobe Workfront Planning

{{planning-important-intro}}

Vous pouvez partager ou supprimer des autorisations sur un espace de travail ou une vue dans Adobe Workfront Planning.

Cet article décrit les niveaux d’autorisation pour les objets Workfront Planning.

Pour plus d’informations sur le partage d’espaces de travail ou de vues, voir les articles suivants :

* [Partager des espaces de travail](/help/quicksilver/planning/access/share-workspaces.md)

* [Partager des vues](/help/quicksilver/planning/access/share-views.md)

## Objets que vous pouvez partager dans Adobe Workfront Planning

Vous pouvez partager les objets suivants :

* Espaces de travail

  Lorsque vous partagez un espace de travail, tous les types d’enregistrements, les enregistrements et les champs associés aux espaces de travail sont également partagés. Les vues ne sont pas partagées.

* Vues

  Vous devez accorder aux utilisateurs, y compris aux administrateurs système, des autorisations d’accès aux vues séparément de leurs autorisations d’accès aux espaces de travail. Pour plus d’informations, voir [Partage de vues](/help/quicksilver/planning/access/share-views.md).

Vous pouvez partager un espace de travail ou une vue avec les entités suivantes :

* Utilisateurs
* Groupes

<!--* You can share a view publicly, with people outside your organization when you generate a public link for a view.People accessing the record page from a public link can view all records and their fields, including connected records and fields.-->

## Considérations sur le partage d’objets dans Adobe Workfront Planning

* Votre type de licence Adobe Workfront fonctionne conjointement avec vos autorisations Workfront Planning pour vous permettre d’afficher, de contribuer ou de gérer les espaces de travail et leurs objets.

  Pour plus d’informations sur la façon dont les types de licence affectent les niveaux d’autorisation pour Workfront Planning, voir [Vue d’ensemble du type de licence lors de l’utilisation d’Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md).
* Les administrateurs système peuvent gérer tous les espaces de travail du système, y compris ceux qu’ils n’ont pas créés.
* Les autres utilisateurs et utilisatrices, y compris les administrateurs et administratrices système, ne peuvent accéder qu’aux vues qu’ils ont créées ou qui ont été partagées avec eux. Les administrateurs système ne peuvent recevoir des autorisations que pour gérer une vue.
* Vous pouvez partager un lien vers un espace de travail ou vers une vue avec d’autres personnes.

  Les personnes qui reçoivent le lien doivent être des personnes actives et se connecter à Workfront pour pouvoir accéder à l’espace de travail ou à la page du type d’enregistrement affiché dans la vue sélectionnée.

## Partager des autorisations pour les objets Adobe Workfront Planning

Les tableaux des sections suivantes illustrent le niveau d’autorisation que vous pouvez sélectionner lorsque vous partagez un espace de travail ou une vue, ainsi que les fonctionnalités autorisées par chaque niveau.

>[!IMPORTANT]
>
>Tous les utilisateurs et utilisatrices ne peuvent pas avoir les niveaux d’autorisation décrits ci-dessous. La licence individuelle de la personne détermine le niveau d’autorisation qu’elle peut recevoir pour les objets Workfront Planning.
>
>Seuls les utilisateurs de licence Standard (ou Plan) peuvent disposer de droits Contribute ou Gérer sur les espaces de travail et Gérer les autorisations pour les vues.
> 
>Les utilisateurs disposant de tous les autres types de licence peuvent disposer des autorisations d’affichage sur les espaces de travail et les vues.
>
>Pour plus d’informations, voir [Vue d’ensemble des types de licences lors de l’utilisation d’Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md).


### Autorisations d’espace de travail

Vous devez autoriser les utilisateurs à accéder aux espaces de travail pour leur permettre d’accéder aux entités suivantes :

* Espaces de travail
* Types d’enregistrements
* Enregistrements
* Champs

Voici les niveaux d’autorisations des espaces de travail :

|        | Gérer | Contribuer | Afficher |
|--------|--------|------------|-------|
| Modifier | ✓ |            |       |
| Partager | ✓ |            |       |
| Supprimer | ✓ |            |       |
| Afficher | ✓ | ✓ | ✓ |

### Autorisations de type d’enregistrement

Les autorisations relatives au type d’enregistrement sont héritées lorsque vous accordez des autorisations sur l’espace de travail.

Voici les niveaux d’autorisations pour les types d’enregistrements :


|        | Gérer | Contribuer | Afficher |
|--------|--------|------------|-------|
| Créer | ✓ |            |       |
| Supprimer | ✓ |            |       |
| Modifier | ✓ |            |       |
| Afficher | ✓ | ✓ | ✓ |

### Autorisations d’enregistrement

Les autorisations d’enregistrement sont héritées lorsque vous accordez des autorisations sur l’espace de travail.

Voici les niveaux d’autorisation des enregistrements :


|        | Gérer | Contribuer | Afficher |
|--------|--------|------------|-------|
| Créer | ✓ |            |       |
| Supprimer | ✓ | ✓ |       |
| Modifier | ✓ | ✓ |       |
| Afficher | ✓ | ✓ | ✓ |

### Autorisations de champ

Les autorisations de champ sont héritées lorsque vous accordez des autorisations sur l’espace de travail.
Les autorisations suivantes se réfèrent aux champs eux-mêmes et non aux valeurs associées à chaque champ. Pour modifier les valeurs des champs, vous devez disposer des autorisations de modification des enregistrements.

|        | Gérer | Contribuer | Afficher |
|--------|--------|------------|-------|
| Créer | ✓ |            |       |
| Supprimer | ✓ |            |       |
| Modifier | ✓ |            |       |
| Afficher | ✓ | ✓ | ✓ |


### Autorisations de vue

Vous devez accorder des autorisations distinctes sur les vues d’enregistrement. Accorder des autorisations sur l’espace de travail n’accorde pas d’autorisations su les vues d’enregistrement de l’espace de travail.

Vous devez autoriser les utilisateurs à accéder aux vues pour leur permettre d’accéder aux éléments de vue suivants :

* Filtres
* Visibilité du champ
* Trier
* Regroupement 
* Hauteur de ligne
* Paramètres


<!--You can share views internally or publicly. -->

Voici les niveaux d’autorisation des vues et des éléments d’affichage :

|        | Gérer (seules les personnes invitées peuvent accéder) | Affichage (seules les personnes invitées peuvent accéder) | Tout le monde dans l’espace de travail peut afficher* |
|--------|--------|-------|------------------------------|
| Modifier | ✓ |       |                            |
| Supprimer | ✓ |       |                            |
| Partager | ✓ |       |                           |
| Afficher | ✓ | ✓ | ✓ |
| Accès à la vue | ✓ | ✓ | ✓ |
| appliquer des filtres temporaires, des groupements, un tri ; | ✓ | ✓ | ✓ |

*Les utilisateurs doivent disposer d’autorisations d’affichage ou supérieures pour accéder à un espace de travail.

<!--Replace the table above with the following when public sharing releases: 

|   Internal sharing     | Manage (Only invited people can access) | View (Only invited people can access)  |Everyone in the workspace can view*|
|--------|--------|-------|------------------------------|
| Edit   | ✓      |       |                            |
| Delete | ✓      |       |                            |
| Share  | ✓       |       |                           |
| View   | ✓      | ✓     | ✓                         |
| Apply  | ✓      | ✓     | ✓                          |

|   Public sharing      | View  |
|--------|-------|
| View   | ✓     |
| Apply  | ✓     |
-->


<!--old view permissions, before sharing View permissions to a view through a workspace:
|        | Manage | View  |
|--------|--------|-------|
| Edit   | ✓      |       |                            
| Delete | ✓      |       |                            
| Share  | ✓       |       |                           
| View   | ✓      | ✓     |                         
| Apply  | ✓      | ✓     |    
-->