---
title: Présentation du partage des autorisations dans la planification d’Adobe Workfront
description: Vous pouvez partager ou supprimer des autorisations sur un espace de travail ou une vue de planification Adobe Workfront.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
el-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
exl-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
source-git-commit: 130365bfa220337aa25f27ba03742ea3471972cb
workflow-type: tm+mt
source-wordcount: '531'
ht-degree: 7%

---

<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Workfront planning. This article describes the levels of access that users could have to Adobe Workfront planning. -->

<!--over time, this article should look like this one does: https://eperienceleague.adobe.com/docs/workfront/using/basics/grant-request-object-permissions/sharing-permissions-on-objects-overview.html?lang=en-->

# Présentation du partage des autorisations dans la planification d’Adobe Workfront

{{maestro-important-intro}}

Vous pouvez partager ou supprimer des autorisations sur un espace de travail ou les afficher dans la planification Adobe Workfront.

Cet article décrit les niveaux d’autorisation des objets de planification Workfront.

Pour plus d’informations sur le partage d’espaces de travail ou de vues, consultez les articles suivants :

* [Partage des espaces de travail](/help/quicksilver/maestro/access/share-workspaces.md)

* [Partage de vues](/help/quicksilver/maestro/access/share-views.md)

## Objets que vous pouvez partager dans la planification Adobe Workfront

Vous pouvez partager les objets suivants :

* Espaces de travail

  Lorsque vous partagez un espace de travail, tous les types d’enregistrement, enregistrements et champs associés aux espaces de travail sont également partagés. Les vues ne sont pas partagées.

* Vues

## Observations relatives au partage d’objets dans la planification d’Adobe Workfront

* Votre type de licence Adobe Workfront fonctionne conjointement avec vos autorisations de planification Workfront pour vous permettre d’afficher, de contribuer ou de gérer des objets lors de l’utilisation de la planification Workfront.

  Pour plus d’informations sur la façon dont les types de licence affectent les niveaux d’autorisation pour la planification Workfront, voir [Présentation du type de licence lors de l’utilisation de la planification Adobe Workfront](/help/quicksilver/maestro/access/license-type-overview.md).
* Les administrateurs système peuvent gérer et partager les espaces de travail créés par d’autres utilisateurs.
* Si vous n’êtes pas administrateur système, vous pouvez contribuer aux espaces de travail créés par d’autres utilisateurs s’ils sont partagés avec vous.
* Vous ne pouvez pas partager les espaces de travail en bloc.
* Vous pouvez partager un espace de travail ou une vue avec les entités suivantes :
   * Utilisateurs
   * Groupes
* Les autres utilisateurs, y compris les administrateurs système, ne peuvent accéder qu’aux vues qu’ils ont créées ou qui ont été partagées avec eux. Les administrateurs système peuvent uniquement disposer d’autorisations pour gérer une vue.
* Vous pouvez partager avec d’autres un lien vers un espace de travail ou vers une vue à partir d’une page de type enregistrement. Les utilisateurs qui reçoivent le lien doivent être des utilisateurs actifs et se connecter à Workfront pour pouvoir accéder à l’espace de travail ou à la page de type enregistrement affichée dans la vue sélectionnée.

## Autorisations de partage pour les objets de planification Adobe Workfront

Les tableaux des sections suivantes illustrent le niveau des autorisations que vous pouvez sélectionner lors du partage d’un espace de travail ou d’une vue et les fonctionnalités que chaque niveau autorise.

>[!IMPORTANT]
>
>Tous les utilisateurs ne peuvent pas disposer des niveaux d’autorisation décrits ci-dessous. La licence individuelle des utilisateurs détermine le niveau d’autorisation qu’ils peuvent recevoir pour les objets de planification Workfront.
>
>Pour plus d’informations, voir [Présentation du type de licence lors de l’utilisation de la planification Adobe Workfront](/help/quicksilver/maestro/access/license-type-overview.md).


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
