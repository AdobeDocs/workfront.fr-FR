---
title: Présentation des autorisations de partage dans Adobe Maestro
description: Vous pouvez partager ou supprimer des autorisations sur un espace de travail ou une vue Adobe Maestro.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
el-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
source-git-commit: 86f9a88518c8a03643061b3328719d2da4016f2b
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 8%

---

<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Maestro. This article describes the levels of access that users could have to Adobe Maestro. -->

<!--over time, this article should look like this one does: https://eperienceleague.adobe.com/docs/workfront/using/basics/grant-request-object-permissions/sharing-permissions-on-objects-overview.html?lang=en-->

# Présentation des autorisations de partage dans Adobe Maestro

{{maestro-important-intro}}

Vous pouvez partager ou supprimer des autorisations sur un espace de travail ou une vue Adobe Maestro.

Cet article décrit les niveaux d’autorisation des objets Maestro.

Pour plus d’informations sur le partage d’espaces de travail ou de vues, consultez les articles suivants :

* [Partage des espaces de travail](/help/quicksilver/maestro/access/share-workspaces.md)

* [Partage de vues](/help/quicksilver/maestro/access/share-views.md)

## Objets que vous pouvez partager dans Adobe Maestro

Vous pouvez partager les objets suivants dans Maestro :

* Espaces de travail

  Lorsque vous partagez un espace de travail, tous les types d’enregistrement, enregistrements et champs associés aux espaces de travail sont également partagés. Les vues ne sont pas partagées.

* Vues

## Observations relatives au partage d’objets dans Maestro

* Vous devez disposer de la licence suivante pour créer des espaces de travail dans Maestro :

   * Nouveau modèle de tarification : licence standard
   * Modèle de tarification actuel : formule une licence.

  Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)
* Les administrateurs système peuvent gérer et partager les espaces de travail créés par d’autres utilisateurs.
* Si vous n’êtes pas administrateur système, vous pouvez contribuer aux espaces de travail créés par d’autres utilisateurs s’ils sont partagés avec vous.
* Vous ne pouvez pas partager les espaces de travail en bloc.
* Vous pouvez partager un espace de travail avec les entités suivantes :
   * Utilisateurs
   * Groupes
* Les autres utilisateurs, y compris les administrateurs système, ne peuvent accéder qu’aux vues qu’ils ont créées ou qui ont été partagées avec eux.
* Vous pouvez partager avec d’autres un lien vers un espace de travail ou vers une vue à partir d’une page de type enregistrement. Les utilisateurs qui reçoivent le lien doivent être des utilisateurs actifs et se connecter à Workfront pour pouvoir accéder à l’espace de travail ou à la page de type enregistrement affichée dans la vue sélectionnée.

## Partage des autorisations pour les objets Maestro

Les tableaux des sections suivantes illustrent le niveau des autorisations que vous pouvez sélectionner lors du partage d’un espace de travail ou d’une vue Maestro et les fonctionnalités autorisées par chaque niveau.

### Autorisations Workspace

|        | Gérer | Contribuer | Afficher |
|--------|--------|------------|-------|
| Modifier | ✓ |            |       |
| Partager | ✓ |            |       |
| Supprimer | ✓ |            |       |
| Afficher | ✓ | ✓ | ✓ |

### Autorisations de type d’enregistrement

Les autorisations de type d’enregistrement sont héritées lorsque vous accordez des autorisations à l’espace de travail.

|        | Gérer | Contribuer | Afficher |
|--------|--------|------------|-------|
| Créer | ✓ |            |       |
| Supprimer | ✓ |            |       |
| Modifier | ✓ |            |       |
| Afficher | ✓ | ✓ | ✓ |

### Autorisations d’enregistrement

Les autorisations d’enregistrement sont héritées lorsque vous accordez des autorisations à l’espace de travail.

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

|        | Gérer | Afficher |
|--------|--------|-------|
| Modifier | ✓ |       |
| Supprimer | ✓ |       |
| Afficher | ✓ | ✓ |
| Appliquer | ✓ | ✓ |






