---
title: Présentation du partage des autorisations dans Adobe Workfront Planning
description: Vous pouvez partager ou supprimer des autorisations sur un espace de travail ou une vue Adobe Workfront Planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
el-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
exl-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
source-git-commit: ace194b584601f9edd7862dbd74f639538891370
workflow-type: tm+mt
source-wordcount: '623'
ht-degree: 13%

---

<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Workfront Planning. This article describes the levels of access that users could have to Adobe Workfront Planning. -->

<!--over time, this article should look like this one does: https://eperienceleague.adobe.com/docs/workfront/using/basics/grant-request-object-permissions/sharing-permissions-on-objects-overview.html?lang=en-->

# Présentation du partage des autorisations dans Adobe Workfront Planning

{{maestro-important-intro}}

Vous pouvez partager ou supprimer des autorisations d’un espace de travail ou des autorisations d’affichage dans Adobe Workfront Planning.

Cet article décrit les niveaux d’autorisation des objets de planification Workfront.

Pour plus d’informations sur le partage d’espaces de travail ou de vues, consultez les articles suivants :

* [Partager des espaces de travail](/help/quicksilver/maestro/access/share-workspaces.md)

* [Partager des vues](/help/quicksilver/maestro/access/share-views.md)

## Objets que vous pouvez partager dans Adobe Workfront Planning

Vous pouvez partager les objets suivants :

* Espaces de travail

  Lorsque vous partagez un espace de travail, tous les types d’enregistrement, enregistrements et champs associés aux espaces de travail sont également partagés. Les vues ne sont pas partagées.

* Vues

## Observations relatives au partage d’objets dans la planification Adobe Workfront

* Votre type de licence Adobe Workfront fonctionne conjointement avec vos autorisations Workfront Planning pour vous permettre d’afficher, de contribuer ou de gérer des objets lors de l’utilisation de Workfront Planning.

  Pour plus d’informations sur la façon dont les types de licence affectent les niveaux d’autorisation pour Workfront Planning, voir [Présentation du type de licence lors de l’utilisation d’Adobe Workfront Planning](/help/quicksilver/maestro/access/license-type-overview.md).
* Les administrateurs système peuvent gérer et partager les espaces de travail créés par d’autres utilisateurs.
* Si vous n’êtes pas administrateur système, vous pouvez contribuer aux espaces de travail créés par d’autres utilisateurs s’ils sont partagés avec vous.
* Vous ne pouvez pas partager des espaces de travail ou des vues en bloc.
* Vous pouvez partager un espace de travail ou une vue avec les entités suivantes :
   * Utilisateurs
   * Groupes
     <!--* You can share a view publicly, with people outside your organization when you generate a public link for a view.People accessing the record page from a public link can view all records and their fields, including connected records and fields.-->
* Les autres utilisateurs, y compris les administrateurs système, ne peuvent accéder qu’aux vues qu’ils ont créées ou qui ont été partagées avec eux. Les administrateurs système peuvent uniquement disposer d’autorisations pour gérer une vue.
* Vous pouvez partager avec d’autres un lien vers un espace de travail ou vers une vue à partir d’une page de type enregistrement. Les utilisateurs qui reçoivent le lien doivent être des utilisateurs actifs et se connecter à Workfront pour pouvoir accéder à l’espace de travail ou à la page de type enregistrement affichée dans la vue sélectionnée.

## Partage des autorisations pour les objets de planification Adobe Workfront

Les tableaux des sections suivantes illustrent le niveau des autorisations que vous pouvez sélectionner lors du partage d’un espace de travail ou d’une vue et les fonctionnalités que chaque niveau autorise.

>[!IMPORTANT]
>
>Tous les utilisateurs ne peuvent pas disposer des niveaux d’autorisation décrits ci-dessous. La licence individuelle des utilisateurs détermine le niveau d’autorisation qu’ils peuvent recevoir pour les objets de planification Workfront.
>
>Pour plus d’informations, voir [Présentation du type de licence lors de l’utilisation d’Adobe Workfront Planning](/help/quicksilver/maestro/access/license-type-overview.md).


### Autorisations Workspace

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

Les autorisations de type d’enregistrement sont héritées lorsque vous accordez des autorisations à l’espace de travail.

Voici les niveaux d’autorisations pour les types d’enregistrements :


|        | Gérer | Contribuer | Afficher |
|--------|--------|------------|-------|
| Créer | ✓ |            |       |
| Supprimer | ✓ |            |       |
| Modifier | ✓ |            |       |
| Afficher | ✓ | ✓ | ✓ |

### Autorisations d’enregistrement

Les autorisations d’enregistrement sont héritées lorsque vous accordez des autorisations à l’espace de travail.

Voici les niveaux d’autorisation des enregistrements :


|        | Gérer | Contribuer | Afficher |
|--------|--------|------------|-------|
| Créer | ✓ |            |       |
| Supprimer | ✓ | ✓ |       |
| Modifier | ✓ | ✓ |       |
| Afficher | ✓ | ✓ | ✓ |

### Autorisations de champ

Les autorisations de champ sont héritées lorsque vous accordez des autorisations à l’espace de travail.
Les permissions suivantes se rapportent aux champs eux-mêmes et non aux valeurs associées à chaque champ. Pour modifier les valeurs de champ, vous devez disposer des autorisations de modification des enregistrements.

|        | Gérer | Contribuer | Afficher |
|--------|--------|------------|-------|
| Créer | ✓ |            |       |
| Supprimer | ✓ |            |       |
| Modifier | ✓ |            |       |
| Afficher | ✓ | ✓ | ✓ |


### Affichage des autorisations

Vous devez accorder des autorisations distinctes pour enregistrer les vues. L’octroi d’autorisations à l’espace de travail n’accorde pas d’autorisations aux vues d’enregistrement dans l’espace de travail.

Vous devez autoriser les utilisateurs à accéder aux vues pour leur permettre d’accéder aux éléments de vue suivants :

* Filtres
* Visibilité du champ
* Trier
* Regroupement 
* Hauteur de ligne
* Paramètres


<!--You can share views internally or publicly. -->

Voici les niveaux d’autorisation des vues et des éléments d’affichage :

|        | Gérer | Afficher |
|--------|--------|-------|
| Modifier | ✓ |       |
| Supprimer | ✓ |       |
| Partager | ✓ |       |
| Afficher | ✓ | ✓ |
| Appliquer | ✓ | ✓ |

<!--Replace the table above with the following when public sharing releases: 

|   Internal sharing     | Manage | View  |
|--------|--------|-------|
| Edit   | ✓      |       |
| Delete | ✓      |       |
| Share  | ✓       |       |
| View   | ✓      | ✓     |
| Apply  | ✓      | ✓     |

|   Public sharing      | View  |
|--------|-------|
| View   | ✓     |
| Apply  | ✓     |
-->