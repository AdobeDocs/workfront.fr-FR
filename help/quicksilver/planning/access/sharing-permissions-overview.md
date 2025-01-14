---
title: Présentation des autorisations de partage dans Adobe Workfront Planning
description: Tous les utilisateurs de l’organisation n’ont pas le même accès et les mêmes autorisations pour utiliser Adobe Workfront Planning. Cet article fournit des informations générales sur le partage ou la suppression des autorisations sur un espace de travail ou une vue Adobe Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
source-git-commit: 00e58ea9a207037b701e1be010c2c4c2995d60e0
workflow-type: tm+mt
source-wordcount: '867'
ht-degree: 43%

---


<!--over time, this article should look like this one does: https://eperienceleague.adobe.com/docs/workfront/using/basics/grant-request-object-permissions/sharing-permissions-on-objects-overview.html?lang=en-->

# Vue d’ensemble du partage d’autorisations dans Adobe Workfront Planning

{{planning-important-intro}}

Vous pouvez partager ou supprimer des autorisations sur un espace de travail ou une vue Adobe Workfront Planning.

Cet article décrit les niveaux d’autorisation pour les objets Workfront Planning.

Pour plus d’informations sur le partage d’espaces de travail ou de vues, voir les articles suivants :

* [Partager des espaces de travail](/help/quicksilver/planning/access/share-workspaces.md)

* [Partager des affichages](/help/quicksilver/planning/access/share-views.md)

## Objets que vous pouvez partager dans Adobe Workfront Planning

Vous pouvez partager les objets suivants :

* Espaces de travail

   * Vous pouvez partager des espaces de travail avec des personnes de votre organisation.
   * Lorsque vous partagez un espace de travail, tous les types d’enregistrements, les enregistrements et les champs associés aux espaces de travail sont également partagés.
   * Lorsque vous partagez un espace de travail, les vues ne sont pas partagées. Les vues sont partagées séparément.

* Vues

   * Vous devez donner aux utilisateurs, y compris aux administrateurs système, les autorisations d’accéder aux vues séparément de leurs autorisations d’accès aux espaces de travail.
   * Lorsque vous partagez une vue, tous les éléments de vue sont partagés, notamment les filtres, le regroupement, le tri ou les paramètres.
   * Lorsque vous partagez une vue, les enregistrements visibles dans la vue ne sont pas partagés. Les enregistrements doivent être partagés en partageant les espaces de travail.
   * Vous pouvez partager une vue publiquement avec des personnes extérieures à votre organisation lorsque vous générez un lien public pour une vue. Les personnes accédant à la page d&#39;enregistrement à partir d&#39;un lien public peuvent afficher tous les enregistrements et leurs champs, y compris les enregistrements et champs connectés.

  Pour plus d’informations, voir [Partager des vues](/help/quicksilver/planning/access/share-views.md).

En interne, vous pouvez partager un espace de travail ou une vue avec les entités Workfront suivantes :

* Utilisateurs
* Groupes

## Considérations sur le partage d’objets dans Adobe Workfront Planning

* Votre type de licence Adobe Workfront fonctionne de concert avec vos autorisations Workfront Planning pour vous donner l’accès à l’affichage, à la contribution ou à la gestion des espaces de travail et de leurs objets.

  Pour plus d’informations sur la façon dont les types de licence affectent les niveaux d’autorisation pour Workfront Planning, voir [Vue d’ensemble du type de licence lors de l’utilisation d’Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md).
* Les administrateurs système peuvent gérer tous les espaces de travail du système, y compris ceux qu’ils n’ont pas créés.
* Les autres utilisateurs et utilisatrices, y compris les administrateurs et administratrices système, ne peuvent accéder qu’aux vues qu’ils ont créées ou qui ont été partagées avec eux. Les administrateurs système ne peuvent être autorisés qu&#39;à gérer une vue.
* Vous pouvez partager un lien vers un espace de travail ou une vue avec d’autres personnes.

  Les scénarios suivants sont possibles :
   * Les utilisateurs recevant le lien vers un espace de travail doivent être des utilisateurs actifs et se connecter à Workfront pour pouvoir accéder à l’espace de travail.
   * Les utilisateurs et utilisatrices qui reçoivent le lien vers une vue peuvent accéder à la vue des manières suivantes :

      * Doit être un utilisateur actif et se connecter à Workfront, si le lien vers la vue a été partagé en interne.
      * Peuvent être des utilisateurs externes à Workfront et accéder à la vue à partir d’un lien partagé publiquement, sans se connecter à Workfront.

## Partager des autorisations pour les objets Adobe Workfront Planning

Les tableaux des sections suivantes illustrent le niveau d’autorisation que vous pouvez sélectionner lorsque vous partagez un espace de travail ou une vue, ainsi que les fonctionnalités autorisées par chaque niveau.

>[!IMPORTANT]
>
>Tous les utilisateurs et utilisatrices ne peuvent pas avoir les niveaux d’autorisation décrits ci-dessous. La licence individuelle de la personne détermine le niveau d’autorisation qu’elle peut recevoir pour les objets Workfront Planning.
>
>Seuls les utilisateurs disposant d’une licence standard (ou de plan) peuvent disposer d’autorisations Contribute ou Gérer sur les espaces de travail et Gérer les autorisations sur les vues.
> 
>Les utilisateurs disposant de tous les autres types de licence peuvent disposer des autorisations d’affichage des espaces de travail et des vues.
>
>Pour plus d’informations, voir [Vue d’ensemble des types de licences lors de l’utilisation d’Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md).


### Autorisations d’espace de travail

Vous devez autoriser les utilisateurs à accéder aux espaces de travail afin de leur permettre d&#39;accéder aux entités suivantes :

* Espaces de travail
* Types d’enregistrements
* Enregistrements
* Champs

Voici les niveaux d’autorisation des espaces de travail :

|        | Gérer | Contribuer | Afficher |
|--------|--------|------------|-------|
| Modifier | ✓ |            |       |
| Partager | ✓ |            |       |
| Supprimer | ✓ |            |       |
| Afficher | ✓ | ✓ | ✓ |

### Autorisations de type d’enregistrement

Les autorisations relatives au type d’enregistrement sont héritées lorsque vous accordez des autorisations à l’espace de travail.

Voici les niveaux d’autorisation pour les types d’enregistrements :


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
| Créer | ✓ | ✓ |       |
| Supprimer | ✓ | ✓ |       |
| Modifier | ✓ | ✓ |       |
| Afficher | ✓ | ✓ | ✓ |

### Autorisations de champ

Les autorisations de champ sont héritées lorsque vous accordez des autorisations à l’espace de travail.
Les autorisations suivantes se réfèrent aux champs eux-mêmes et non aux valeurs associées à chaque champ. Pour modifier les valeurs des champs, vous devez avoir les autorisations de modifier les enregistrements.

|        | Gérer | Contribuer | Afficher |
|--------|--------|------------|-------|
| Créer | ✓ |            |       |
| Supprimer | ✓ |            |       |
| Modifier | ✓ |            |       |
| Afficher | ✓ | ✓ | ✓ |


### Autorisations d’affichage

Vous devez accorder des autorisations distinctes aux vues d’enregistrement. Accorder des autorisations à l’espace de travail n’accorde pas d’autorisations aux vues d’enregistrement de l’espace de travail.

Vous devez autoriser les utilisateurs à accéder aux vues pour leur permettre d&#39;accéder aux éléments d&#39;affichage suivants :

* Filtres
* Visibilité du champ
* Trier
* Regroupement 
* Hauteur de ligne
* Paramètres

Vous pouvez partager des vues en interne ou publiquement.

Vous trouverez ci-dessous les niveaux d’autorisations pour les vues et les éléments de vue :

| Partage interne | Gérer (seules les personnes invitées peuvent accéder) | Afficher (seules les personnes invitées peuvent accéder) | Tout le monde dans l’espace de travail peut afficher* |
|--------|--------|-------|------------------------------|
| Modifier | ✓ |       |                            |
| Supprimer | ✓ |       |                            |
| Partager | ✓ |       |                           |
| Afficher | ✓ | ✓ | ✓ |
| Appliquer | ✓ | ✓ | ✓ |

| Partage public | Afficher |
|--------|-------|
| Afficher | ✓ |
| Appliquer | ✓ |

*Les utilisateurs doivent disposer d’autorisations d’affichage ou d’autorisations supérieures dans un espace de travail pour obtenir cet accès en affichage.

<!--old view permissions, before sharing View permissions to a view through a workspace:
|        | Manage | View  |
|--------|--------|-------|
| Edit   | ✓      |       |                            
| Delete | ✓      |       |                            
| Share  | ✓       |       |                           
| View   | ✓      | ✓     |                         
| Apply  | ✓      | ✓     |  


|        | Manage (Only invited people can access) | View (Only invited people can access)  |Everyone in the workspace can view*|
|--------|--------|-------|------------------------------|
| Edit   | ✓      |       |                            |
| Delete | ✓      |       |                            |
| Share  | ✓       |       |                           |
| View   | ✓      | ✓     | ✓                         |
| Access the view  | ✓      | ✓     | ✓                          |
| Apply temporary filters, groupings, sort  | ✓      | ✓     | ✓                          |
-->