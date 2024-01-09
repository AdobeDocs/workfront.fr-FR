---
title: Présentation des autorisations de partage dans Adobe Maestro
description: Vous pouvez partager ou supprimer des autorisations sur un espace de travail ou une vue Adobe Maestro.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
el-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
source-git-commit: 3c49657c929c414888e6678022ef61b1bba1a420
workflow-type: tm+mt
source-wordcount: '474'
ht-degree: 8%

---

<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Maestro. This article describes the levels of access that users could have to Adobe Maestro. -->

<!--over time, this article should look like this one does: https://eperienceleague.adobe.com/docs/workfront/using/basics/grant-request-object-permissions/sharing-permissions-on-objects-overview.html?lang=en-->

<!-- *********add to TOC****************-->

# Présentation des autorisations de partage dans Adobe Maestro

>[!IMPORTANT]
>
>Les informations de cet article se rapportent à Adobe Maestro, une nouvelle offre d’Adobe Workfront.
>
>Actuellement, Adobe Maestro fait partie d’un programme bêta ouvert à un nombre limité de clients. Ypu doit être un client Workfront pour avoir accès à Maestro.
>
>Pour plus d’informations sur l’inscription au programme bêta de Maestro, contactez le représentant de votre compte.
>
>Pour plus d’informations, voir [Présentation d’Adobe Maestro](../maestro-overview.md).

Vous pouvez partager ou supprimer des autorisations sur un espace de travail ou une vue Adobe Maestro.

Cet article décrit les niveaux d’autorisation des objets Maestro.

Pour plus d’informations sur le partage d’espaces de travail ou de vues, consultez les articles suivants :

* [Partager un espace de travail](/help/quicksilver/maestro/access/share-workspaces.md)

* [Partage d’une vue](/help/quicksilver/maestro/access/share-views.md)

## Objets que vous pouvez partager dans Adobe Maestro

Vous pouvez partager les objets suivants dans Maestro :

* Espaces de travail

  Lorsque vous partagez un espace de travail, tous les types d’enregistrement, enregistrements et champs associés aux espaces de travail sont également partagés. Les vues ne sont pas partagées.

* Vues

## Observations relatives au partage d’objets dans Maestro

* Vous devez disposer de la licence suivante pour créer des espaces de travail dans Maestro :

   * Nouveau modèle de tarification : licence standard
   * Modèle de tarification actuel : licence professionnelle ou supérieure

  Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)
* Les administrateurs système peuvent gérer et partager les espaces de travail créés par d’autres utilisateurs.
* Si vous n’êtes pas administrateur système, vous pouvez contribuer aux espaces de travail créés par d’autres utilisateurs s’ils sont partagés avec vous.
* Vous ne pouvez pas partager les espaces de travail en bloc.
* Vous pouvez partager un espace de travail avec les entités suivantes :
   * Utilisateurs
   * Groupes
* Les autres utilisateurs, y compris les administrateurs système, ne peuvent accéder qu’aux vues qu’ils ont créées ou qui ont été partagées avec eux.

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




<!--
<table>
  <tr>
   

   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td><p><b>New: Standard license</b></p> <p><b>Current: Worker or higher license</b></p></strong>
   </td>
   <td><strong>Manage permissions</strong>
   </td>
   <td><strong>Contribute permissions</strong>
   </td>
   <td><strong>View permissions</strong>
   </td>
  </tr>
  <tr>
   <td><strong>Create</strong>
   </td>
   <td rowspan="5" ><strong>Workspace</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><strong>Delete</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><strong>Share</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><strong>Edit</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><strong>View</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
  </tr>
  <tr>
   <td><strong>Create/delete</strong>
   </td>
   <td rowspan="3" ><strong>Record Type*</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><strong>Edit</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><strong>View</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
  </tr>
  <tr>
   <td><strong>Create/delete</strong>
   </td>
   <td rowspan="3" ><strong>Record*</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><strong>Edit</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><strong>View</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
  </tr>
  <tr>
   <tr>
   <td><strong>Create</strong>
   </td>
   <td rowspan="5" ><strong>View</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><strong>Delete</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><strong>Share</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><strong>Edit</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><strong>View</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>
   </td>
   <td>✓
   </td>
  </tr>

<tr>
   <td><strong>Create/delete</strong>
   </td>
   <td rowspan="3" ><strong>Fields*</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><strong>Edit</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><strong>View</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
  </tr>



</table>

*Record types, records, and fields inherit permissions from the Workspace. -->



