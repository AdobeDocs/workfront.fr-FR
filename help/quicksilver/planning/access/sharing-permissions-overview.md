---
title: Présentation des autorisations de partage dans Adobe Workfront Planning
description: Tous les utilisateurs de l’organisation n’ont pas le même accès et les mêmes autorisations pour utiliser Adobe Workfront Planning. Cet article fournit des informations générales sur le partage ou la suppression des autorisations sur un espace de travail ou une vue Adobe Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/eF7kBTsursbrsXr8Lo6ql6U5JBLQDvi6nw4JDpRxClw
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
source-git-commit: 37be1f25fa54f3efd4113478496e95db3c8bce1c
workflow-type: tm+mt
source-wordcount: 1372
ht-degree: 21%

---

<!--over time, this article should look like this one does: https://eperienceleague.adobe.com/docs/workfront/using/basics/grant-request-object-permissions/sharing-permissions-on-objects-overview.html?lang=en-->

<!--remove the Prod and Preview references when we release to Prod-->

# Vue d’ensemble du partage d’autorisations dans Adobe Workfront Planning

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de manière générale. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Une fois la version à prévisualiser, les mêmes fonctionnalités sont également disponibles tous les mois dans l’environnement de production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation des versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Vous pouvez partager ou supprimer des autorisations sur un espace de travail Adobe Workfront Planning, un type d’enregistrement ou une vue.

Vous pouvez également partager des formulaires de demande Planning. Pour plus d’informations, voir [Création et gestion d’un formulaire de demande dans Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

Cet article décrit les niveaux d’autorisation pour les espaces de travail Workfront Planning, les types d’enregistrements, les enregistrements, les champs et les vues.

## Objets que vous pouvez partager dans Adobe Workfront Planning

Vous pouvez partager manuellement certains objets Workfront Planning, tandis que d’autres héritent de ces autorisations d’autres objets.

Vous pouvez partager manuellement les objets suivants dans Workfront Planning :

* Espaces de travail

   * Vous pouvez partager des espaces de travail avec des personnes de votre organisation.
   * Lorsque vous partagez un espace de travail, tous les types d’enregistrements, les enregistrements et les champs associés aux espaces de travail sont également partagés.
   * Lorsque vous partagez un espace de travail, les vues ne sont pas partagées. Les vues sont partagées séparément.

  Pour plus d’informations, voir [Partager des espaces de travail](/help/quicksilver/planning/access/share-workspaces.md)

* Types d’enregistrements

   * Vous pouvez partager des types d’enregistrements avec des personnes de votre organisation.
   * Le niveau des autorisations accordées pour l’espace de travail s’affiche sous la forme d’autorisations héritées pour le type d’enregistrement.
   * Vous ne pouvez pas partager un type d’enregistrement avec un niveau d’autorisation supérieur à celui de l’utilisateur sur l’espace de travail.

  Pour plus d’informations, voir [Partage de types d’enregistrements](/help/quicksilver/planning/access/share-record-types.md).

<div class="preview">

* Enregistrements

   * Vous pouvez partager des enregistrements avec des personnes au sein de votre organisation.
   * Les utilisateurs héritent par défaut des autorisations de l’espace de travail et du type d’enregistrement.
   * Vous ne pouvez pas partager un enregistrement avec un niveau d&#39;autorisation supérieur ou inférieur à celui dont dispose l&#39;utilisateur sur le type d&#39;enregistrement.

  Pour plus d’informations, voir [Partager des enregistrements](/help/quicksilver/planning/access/share-records.md).

</div>

* Vues

   * Vous devez donner aux utilisateurs, y compris aux administrateurs système, les autorisations d’accéder aux vues séparément de leurs autorisations d’accès aux espaces de travail.
   * Lorsque vous partagez une vue, tous les éléments de vue sont partagés, notamment les filtres, le regroupement, le tri ou les paramètres.
   * Lorsque vous partagez une vue, les enregistrements visibles dans la vue ne sont pas partagés. Les enregistrements doivent être partagés en partageant les espaces de travail.
   * Vous pouvez partager une vue publiquement avec des personnes extérieures à votre organisation lorsque vous générez un lien public pour une vue.Les personnes qui accèdent à la page d&#39;enregistrement à partir d&#39;un lien public peuvent afficher tous les enregistrements et leurs champs, y compris les enregistrements et champs connectés.

  Pour plus d’informations, consultez la section [Partager des vues](/help/quicksilver/planning/access/share-views.md).


## Considérations sur le partage d’objets dans Adobe Workfront Planning

* Votre type de licence Adobe Workfront fonctionne de concert avec vos autorisations Workfront Planning pour vous donner l’accès à l’affichage, à la contribution ou à la gestion des espaces de travail et de leurs objets.

  Pour plus d’informations sur la façon dont les types de licence affectent les niveaux d’autorisation pour Workfront Planning, voir [Vue d’ensemble du type de licence lors de l’utilisation d’Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md).
* Les administrateurs système peuvent gérer tous les espaces de travail du système, y compris ceux qu’ils n’ont pas créés.
* Les autres utilisateurs et utilisatrices, y compris les administrateurs et administratrices système, ne peuvent accéder qu’aux vues qu’ils ont créées ou qui ont été partagées avec eux. Les administrateurs système ne peuvent être autorisés qu&#39;à gérer une vue.

* Lorsque vous partagez des espaces de travail et des types d’enregistrements avec d’autres personnes, le niveau d’autorisation du type d’enregistrement est automatiquement hérité des enregistrements et des champs qui leur sont associés par défaut.

* Vous pouvez partager des objets Planning des manières suivantes :

   * En interne, vous pouvez partager des objets Workfront Planning avec les entités Workfront suivantes :

      * Utilisateurs et utilisatrices
      * Groupes
      * Équipes
      * Entreprises
      * Fonctions

     Vous pouvez partager un objet Planning avec un maximum de 100 entités par objet.

   * En interne, en partageant un lien vers un espace de travail ou une vue avec d&#39;autres utilisateurs de Planning. Les scénarios suivants sont possibles :

      * Les utilisateurs recevant le lien vers un espace de travail doivent être des utilisateurs actifs et se connecter à Workfront pour accéder à l’espace de travail.
      * Les utilisateurs et utilisatrices qui reçoivent un lien de partage interne pour une vue doivent être des utilisateurs et utilisatrices actifs et se connecter à Workfront pour accéder à la vue.
   * En externe, en partageant un lien de partage public vers une vue avec des utilisateurs externes qui ne disposent pas d’un compte Workfront.

## Partager des autorisations pour les objets Adobe Workfront Planning

Les tableaux des sections suivantes illustrent le niveau d’autorisation que vous pouvez sélectionner lorsque vous partagez un espace de travail ou une vue, ainsi que les fonctionnalités autorisées par chaque niveau.

>[!IMPORTANT]
>
>Tous les utilisateurs et utilisatrices ne peuvent pas avoir les niveaux d’autorisation décrits ci-dessous. La licence individuelle de la personne détermine le niveau d’autorisation qu’elle peut recevoir pour les objets Workfront Planning.
>
>Seuls les utilisateurs disposant d’une licence standard (ou de plan) peuvent disposer d’autorisations de niveau Contribuer ou Gérer sur les espaces de travail et Gérer les autorisations sur les vues.
> 
>Les utilisateurs disposant de tous les autres types de licence peuvent disposer des autorisations d’affichage des espaces de travail et des vues.
>
>Pour plus d’informations, voir [Vue d’ensemble des types de licences lors de l’utilisation d’Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md).


### Autorisations d’accès aux espaces de travail

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

### Autorisations relatives aux types d’enregistrements

<!--
 old access:
In the Production environment, Record Type permissions are always inherited when you grant permissions to the workspace.

The following are the levels of permissions for record types: 


|        | Manage | Contribute | View  |
|--------|--------|------------|-------|
| Create | ✓      |            |       |
| Delete | ✓      |            |       |
| Edit   | ✓      |            |       |
| View   | ✓      | ✓          | ✓     |

-->

Les autorisations de type d’enregistrement sont toujours héritées lorsque vous accordez des autorisations à l’espace de travail.

Vous pouvez supprimer les autorisations héritées du type d’enregistrement reçues de l’espace de travail.

Vous pouvez accorder aux utilisateurs des autorisations moindres sur le type d’enregistrement que sur l’espace de travail.

Cependant, vous ne pouvez pas effectuer les opérations suivantes :

* Accordez des autorisations plus élevées pour le type d’enregistrement que les utilisateurs n’ont sur l’espace de travail.
* Donnez aux gestionnaires d’espace de travail des autorisations inférieures sur un type d’enregistrement.
* Supprimez les autorisations d’affichage du type d’enregistrement ou de l’espace de travail en supprimant des utilisateurs des autorisations de type d’enregistrement.

Les scénarios suivants sont possibles :

| Autorisations d’espace de travail | Autorisations héritées automatiques pour un type d’enregistrement | Autorisations de type d’enregistrement possibles lorsque les autorisations héritées sont désactivées (accordées manuellement) |
|--------|--------|-------------|
| Gérer | Gérer | Gérer, supprimer des autorisations* |
| Contribuer | Contribuer | Contribuer, Afficher, Supprimer des autorisations* |
| Afficher | Afficher | Afficher, Supprimer des autorisations* |

>[!NOTE]
>
>Lorsque vous supprimez des autorisations d’un type d’enregistrement, les utilisateurs conservent toujours les autorisations d’affichage de l’espace de travail et de tous les types d’enregistrements, sauf si vous supprimez leurs autorisations de l’espace de travail.

### Autorisations aux enregistrements

Les autorisations d’enregistrement sont héritées du type d’enregistrement lorsque vous accordez des autorisations à l’espace de travail et au type d’enregistrement, par défaut.

Dans l’environnement de production, les niveaux d’autorisation des enregistrements sont les suivants :


|        | Gérer | Contribuer | Afficher |
|--------|--------|------------|-------|
| Créer | ✓ | ✓ |       |
| Supprimer | ✓ | ✓ |       |
| Modifier | ✓ | ✓ |       |
| Afficher | ✓ | ✓ | ✓ |

<div class="preview">

Dans l’environnement de Prévisualisation, les niveaux d’autorisation des enregistrements sont les suivants :

|        | Gérer | Afficher |
|--------|--------|-------|
| Créer | ✓ |       |
| Supprimer | ✓ |       |
| Modifier | ✓ |       |
| Afficher | ✓ | ✓ |

Les autorisations d’enregistrement sont toujours héritées lorsque vous accordez des autorisations à l’espace de travail et au type d’enregistrement.

Vous pouvez supprimer les autorisations héritées de l’enregistrement reçues du type d’enregistrement. Les responsables Workspace et les créateurs d’enregistrements conservent les autorisations de gestion de l’enregistrement.

Vous ne pouvez pas accorder aux utilisateurs des autorisations inférieures ou supérieures sur l’enregistrement qu’ils n’ont sur le type d’enregistrement.

Les scénarios suivants sont possibles :

| Autorisations de type Workspace et enregistrement | Autorisations héritées automatiques pour un enregistrement | Autorisations d’enregistrement possibles lorsque les autorisations héritées sont désactivées (accordées manuellement) |
|--------|--------|-------------|
| Gérer | Gérer | Gérer, supprimer des autorisations* |
| Contribuer | Gérer | Gérer, supprimer des autorisations* |
| Afficher | Afficher | Afficher, Supprimer des autorisations* |

>[!NOTE]
>
>*Lorsque vous supprimez des autorisations d’un enregistrement, les utilisateurs conservent toujours les autorisations d’affichage de l’espace de travail et du type d’enregistrement, sauf si vous supprimez leurs autorisations de l’espace de travail.

</div>

### Autorisations pour les champs d’enregistrement

Les autorisations de champ sont héritées du type d’enregistrement lorsque vous accordez des autorisations à l’espace de travail et au type d’enregistrement.

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

>[!NOTE]
>
>*Les utilisateurs doivent disposer d’autorisations d’affichage ou d’autorisations supérieures dans un espace de travail pour obtenir cet accès en affichage.


<!--
old view permissions, before sharing View permissions to a view through a workspace:
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
