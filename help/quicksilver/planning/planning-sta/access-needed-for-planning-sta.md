---
title: Accès nécessaire pour Adobe Workfront Planning en tant que produit autonome
description: Cet article décrit les licences, les niveaux d'accès et les fonctionnalités utilisateur pour Adobe Workfront Planning en tant que produit autonome.
last-update: 2026-04-01T18:02:40Z
git-commit-file: 8cc175490a6aa1db68b238edbdf9da9da7fbb258
source-git-commit: 697499fadf4d5d22292ededed381cb72e53fcae3
workflow-type: tm+mt
source-wordcount: '1037'
ht-degree: 3%

---

<!--

Update metadata with this at release:
---
title: Access Required for Planning Standalone
description: This article describes how you can benefit from using the standalone version of Adobe Workfront Planning.
feature: Workfront Planning (******************ask Bob for a new feature???***********)
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
---
-->

# Accès nécessaire pour Adobe Workfront Planning en tant que produit autonome

>[!IMPORTANT]
>
>Les informations de cet article font référence à Adobe Workfront Planning, lorsqu’il est acheté en tant que produit autonome. Reportez-vous à cet article lorsque votre société a acheté un package Adobe Workfront Planning uniquement sans acheter de package Workfront Workflow.
>
>Pour plus d’informations sur Adobe Workfront Planning lorsqu’il est acheté avec un package de workflow Workfront, voir [Prise en main d’Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).

Cet article décrit les licences, les niveaux d&#39;accès et les fonctionnalités utilisateur pour Adobe Workfront Planning en tant que produit autonome.

## Packages Workfront Planning

Votre entreprise peut acheter l’un des packages Workfront Planning autonomes suivants :

* Prime
* Sélectionner
* Ultimate

Le tableau suivant décrit les composants inclus dans chaque package :

| Fonction de planification | Sélectionner | Prime | Ultimate |
|---|---|---|---|
| Planification, orchestration, gestion de campagnes | ✓ | ✓ | ✓ |
| Espaces de travail illimités | ✓ | ✓ | ✓ |
| Enregistrements par espace de travail | 25,000 | 500,000 | 1,000,000 |
| Nombre total d’enregistrements (tous les espaces de travail) | 500,000 | 2,000,000 | Illimité |
| Types d’enregistrements globaux et connexions entre espaces de travail | — | ✓ | ✓ |
| Accès aux fonctionnalités futures lors de la publication | Certains | Certains | La plupart |

## Disponibilité du package Workfront Planning

<!--
the bullets repeat in the "Planning overview" article
-->

Workfront Planning est accessible lorsque votre entreprise achète l’un des packages Workfront suivants :

* Workfront Workflow et Workfront Planning ont été achetés ensemble. Chaque utilisateur de l’organisation dispose d’une licence Workflow et Planning. Tous les utilisateurs bénéficient ainsi d’un accès complet à toutes les fonctionnalités de Workfront pour les deux modules.

* Workflow Workfront pour tous les membres de votre organisation et Planification Workfront pour certains utilisateurs uniquement. Les utilisateurs bénéficient ainsi d&#39;un accès complet à toutes les fonctionnalités de Workflow et d&#39;un accès plus limité aux fonctionnalités de Planning pour les utilisateurs disposant d&#39;une licence Planning.

* Workfront Planning en tant que produit autonome pour les utilisateurs de votre entreprise. Les utilisateurs n’ont ainsi accès ni aux fonctionnalités de Workfront Workflow, ni aux fonctionnalités de Planning.

Pour plus d’informations sur les fonctionnalités incluses dans Planning en tant que produit autonome, consultez la section « Fonctionnalités incluses dans Workfront Planning en tant que produit autonome » de l’article [Prise en main d’Adobe Workfront Planning en tant que produit autonome](/help/quicksilver/planning/planning-sta/planning-sta-overview.md).

## Licence utilisateur et niveaux d&#39;accès

<!-- should this be moved to the Manage users in Planning article??-->

Les licences Planning font partie du niveau d&#39;accès attribué aux utilisateurs.

Pour Planning en tant que produit autonome, vous ne pouvez pas attribuer de licences aux niveaux d&#39;accès. Ces licences sont déjà codées en dur pour être incluses dans les niveaux d&#39;accès attribués aux utilisateurs.

Selon le package Workfront Planning acheté par votre organisation, vous pouvez disposer de l’un des niveaux d’accès suivants pour vos utilisateurs :

* **Administrateur Planning** : disponible pour les packages Workfront Planning. Les administrateurs de Planning sont automatiquement affectés lorsque des utilisateurs sont ajoutés à Admin Console.
* **Planning Standard** : disponible pour tous les packages Workfront Planning. Vous pouvez attribuer ces niveaux d’accès aux utilisateurs lorsque vous les créez.

<!--
this is not available for Planning STA: 
* **Planning Contributor**: Available for the following customers: 

    * Customers that purchase equal amounts of Workflow and Planning packages together. In this case, Planning Contributors have limited access to Planning objects.
    * Customer that purchase unequal amounts of Workflow and Planning packages. In this case, Planning Contributors have read-only access to Planning objects.

-->

Chaque licence Planning autonome est mappée à un rôle dans le système et contrôle les zones du produit accessibles.

Le tableau suivant illustre chaque type de licence Planning et ses fonctionnalités dans Workfront Planning, lorsqu&#39;il est acheté en tant que produit autonome :

| Fonctionnalité / Type de licence | Administrateur ou administratrice de planification | Norme de planification |
|---|---|---|
| Description du niveau d&#39;accès | Accès complet au système | Peuvent gérer les espaces de travail et le contenu |
| Zone Planning du menu principal | ✔ | ✔ |
| Zone Utilisateurs du menu principal | ✔ | Afficher uniquement |
| Zone des demandes dans le menu principal | ✔ | ✔ |
| Zone Configuration du menu principal | ✔ |   |
| Gestion des espaces de travail et de leur contenu | ✔ | ✔ |
| Partage des données Planning avec les équipes | ✔ | ✔ |
| Soumettre des demandes | ✔ | ✔ |
| Créer ou modifier des utilisateurs | ✔ |   |
| Afficher la liste des utilisateurs | ✔ | Afficher uniquement |
| Configuration > Équipes | ✔ |   |
| Configuration > Connexion En Tant Que | ✔ |   |
| Configuration > Trimestres personnalisés | ✔ |   |
| Configuration > Système > Informations sur le client | ✔ |   |
| Configuration > Système > Préférences | ✔ |   |

Pour plus d’informations sur l’attribution de niveaux d’accès aux utilisateurs, voir [Gérer les utilisateurs dans Adobe Workfront Planning en tant que produit autonome](/help/quicksilver/planning/planning-sta/manage-users-in-planning-sta.md).

## Zones de navigation et dépendances de niveau d’accès

Selon la licence Planning, les utilisateurs peuvent avoir différentes zones disponibles dans leur navigation globale.

<!--
>[!NOTE]
>
>Workfront-specific toolbar actions (Search, Recents, Favorites, Notifications) are not available in the Workfront header for any Standalone user.
-->

### Présentation de la navigation de l&#39;administrateur Planning

<!--
Managing your Adobe Workfront Planning instance is similar to managing an Adobe Workfront with Planning instance, but there are some differences.
-->

Un utilisateur disposant d&#39;un niveau d&#39;accès Administrateur Planning possède les fonctionnalités suivantes :

* Dispose d’un accès en gestion complet au système.
* Peut créer et modifier des utilisateurs, gérer des équipes, configurer des trimestres personnalisés et accéder à toutes les sous-pages de configuration.

  Pour plus d’informations, voir :

   * [Gestion des utilisateurs dans Adobe Workfront Planning en tant que produit autonome](/help/quicksilver/planning/planning-sta/manage-users-in-planning-sta.md)
   * [Gestion des équipes dans Adobe Workfront Planning en tant que produit autonome](/help/quicksilver/planning/planning-sta/manage-teams-in-planning-sta.md)
* Possibilité d’envoyer et de gérer des requêtes.

  Pour plus d’informations, voir [Demandes Adobe Workfront Planning : index d’article](/help/quicksilver/planning/requests/requests-article-index.md).
* Comporte les zones suivantes dans le menu principal :

   * **Planning** : dispose de toutes les fonctionnalités nécessaires pour créer, supprimer, partager et connecter des objets Planning.
   * **Utilisateurs** : vous pouvez ajouter des utilisateurs et modifier leurs profils.
   * **Demandes**
   * **Configuration**
* Comporte les sections suivantes dans la zone Configuration :

   * **Équipes** : vous pouvez ajouter, supprimer ou modifier des équipes. La modification se limite au nom, à la description et aux membres de l&#39;équipe ; aucun filtre, affichage, regroupement ou contrôle d&#39;exportation n&#39;est disponible.
   * **Se connecter en tant que** : empruntez l’identité d’un autre utilisateur à des fins de dépannage.
   * **Trimestres personnalisés** : configurez les trimestres fiscaux personnalisés qui apparaissent dans les vues chronologiques Planning.
   * Système

* Comporte les sections suivantes dans la zone Système :

   * **Informations sur le client** : affichez les détails du client et de l’organisation.
   * **Préférences** : consultez et configurez les préférences au niveau du système.

### Aperçu de la navigation dans Planning Standard

Un utilisateur disposant d&#39;un niveau d&#39;accès Planning Standard dispose des fonctionnalités suivantes :

* Peuvent gérer les espaces de travail et leur contenu.
* Possibilité d’envoyer et de gérer des requêtes.

  Pour plus d’informations, voir [Demandes Adobe Workfront Planning : index d’article](/help/quicksilver/planning/requests/requests-article-index.md).
* Les utilisateurs de Planning Standard peuvent accéder aux zones suivantes du menu principal :

   * **Planification**
   * **Utilisateurs** : ils disposent d’un accès en lecture seule aux utilisateurs. Ils ne peuvent pas créer ni modifier d’utilisateurs. <!--not sure if this is still true-->
   * **Demandes**

* N&#39;ont pas accès à la configuration ou à l&#39;une de ses sections.

## Configurer des niveaux d&#39;accès pour Planning en tant que produit autonome

Les niveaux d&#39;accès sont intégrés lorsque vous achetez Planning en tant que produit autonome et vous ne pouvez pas les configurer pour les utilisateurs Planning.

Pour attribuer des niveaux d&#39;accès aux utilisateurs, en tant qu&#39;administrateur de Planning :

* Créez des utilisateurs dans la console Adobe.

  Les scénarios suivants sont possibles :

   * Les utilisateurs ajoutés à la console Adobe en tant qu’administrateurs reçoivent un niveau d’accès d’administrateur Planning dans Workfront Planning.
   * Les utilisateurs ajoutés à la console Adobe en tant qu&#39;utilisateurs peuvent se voir attribuer un niveau d&#39;accès Planning Standard dans Workfront Planning. Il s’agit du seul accès disponible à affecter aux nouveaux utilisateurs dans Workfront Planning en tant que produit autonome.

Pour plus d’informations, voir [Gérer les utilisateurs](/help/quicksilver/planning/planning-sta/manage-users-in-planning-sta.md).

## Octroi d’autorisations dans Workfront Planning en tant que produit autonome

Vous pouvez partager les objets suivants dans Workfront Planning en tant que produit autonome :

* Espaces de travail
* Types d’enregistrements
* Enregistrements
* Vues

Le partage d&#39;objets dans Planning en tant que produit autonome est identique au partage d&#39;objets dans Planning lorsqu&#39;ils sont achetés avec un package de workflow.

Pour plus d&#39;informations, voir [Informations d&#39;accès à Adobe Workfront Planning : index des articles](/help/quicksilver/planning/access/access-information.md).

<!--

I took this out because there is NO Contributor for true STA: 

### Planning Contributor user experience

>[!IMPORTANT]
>
>Planning Contributor access level is only available for customers that purchase both Workfront Planning and a Workfront Workflow package together. 
>
>If they purchase unequal numbers of packages for the two modules, the Planning Contributor license is read-only. 

When standalone Workfront Planning users purchase a Workflow package, they receive a read-only Planning Contributor license by default. 

For more information, see [Get started with Adobe Workfront Planning as a standalone product](/help/quicksilver/planning/planning-sta/planning-sta-overview.md).

A user with a Planning Standard access level has the following capabilities: 

* View-only access to Planning data, equivalent to the Contributor license in Workfront.
* Can access the following areas in the Main menu:
    * **Planning**
    * **Requests**
* Can submit requests.
* No access to the Users list.
* No access to Setup or any of its sub-pages.

-->

<!-- 
this was moved from the STA general article - some information is already above - take out here what is not needed or add above: 

## Package overview

The following packages are available for Workfront Planning as a standalone product:

* Select
* Prime
* Ultimate

The following table describes what is included in each package:  

| Capability | Select | Prime | Ultimate |
|---|---|---|---|
| Planning, orchestration, campaign management | ✓ | ✓ | ✓ |
| Unlimited workspaces | ✓ | ✓ | ✓ |
| Records per workspace | 25,000 | 500,000 | 1,000,000 |
| Total records (all workspaces) | 500,000 | 2,000,000 | Unlimited |
| Global Record Types and cross-workspace connections | — | ✓ | ✓ |
| Access to future features at release | Some | Some | Most |

## Licensing overview

Consider the following about Workfront Planning licenses:

* Your organization can purchase Workfront Planning licenses without requiring Workfront or Workflow licenses.
* You can add users to Workfront Planning using the Adobe Experience Platform.

    For more information, see [Manage users](/help/quicksilver/planning/planning-sta/manage-users-in-planning-sta.md). 
* Workfront Planning users are limited to Planning-only capabilities and do not receive access to any Workfront areas or capabilities.

The following access levels are hard-coded in Workfront Planning and cannot be modified: 

* Planning Administrator
* Planning Standard 

>[!IMPORTANT]
>
>In a Workfront Planning context, a user must hold a **Planning Standard** license to access the product. 

For more information, see [Access needed for Adobe Workfront Planning as a standalone product](/help/quicksilver/planning/planning-sta/access-needed-for-planning-sta.md). 

## How licensing works for customers with a Planning and Workfront combined package

Consider the following if you have both the Workfront Workflow and Planning packages:

* A Planning Contributor read-only license is available for users in Planning. 
* Any Workfront access level (including Light or Contributor) can be paired with either a Planning Standard or Planning Contributor access level, regardless of the Workfront Workflow license type.

    For example, a user with a Workfront Contributor license can still hold a Planning Standard license and have full Planning management capabilities.

### Mixed License access matrix

When a customer has both Planning and Workfront packages, access levels are determined by the combination below:

| Access Type | Planning License | Workflow License | License Origin |
|---|---|---|---|
| Default | Read Only | Workfront Light | Workfront |
| Default | Read Only | Workfront Standard | Workfront |
| Default | Read Only | Workfront Contributor | Workfront |
| Default | Read Only | Workfront External | Workfront |
| Default | Planning Standard | Workfront Contributor | Planning |
| — | Planning Standard | Workfront Light | Either Planning or Workfront |
| — | Planning Standard | Workfront Standard | Either Planning or Workfront |

Consider the following if your organization has purchased Workfront with Planning:

* Adding a new user to Planning or Workfront automatically creates default (read-only) access in the other product.
* You can upgrade the access in the opposite product. For more information, contact your account representative.

### Upgrading from standalone Planning to a Planning with a Workflow package

#### Workfront Planning with a Workfront Workflow package

When you add a Workfront Planning Standalone package to an existing Workflow license, the following changes take effect automatically:

* Planning Administrators are promoted to System Administrators.
* Non-admin Planning users (Standard and Contributor) receive Workflow Contributor licenses.
* All existing Planning data is preserved.
* All newly provisioned Workfront users are auto-assigned Planning Contributor (read-only) licenses.

#### License mapping when you upgrade to a Planning with Workflow package

| Before (Planning Standalone) | After (Workfront + Planning) |
|---|---|
| Planning Administrator | System Administrator |
| Planning Standard | Workflow Contributor |
| Planning Contributor | Workflow Contributor |

Planning and Workflow licenses remain separate after the upgrade. A Planning Standard user can hold a Workflow Contributor license, and a Planning Contributor user can hold a Workflow Standard license — these are assigned independently based on need.

All users receive an email notification when they gain access to the additional Workflow capabilities in Workfront.

-->

<!--
I took out the last column on this table and added above:

| Feature / Access | Planning Administrator | Planning Standard | Planning Contributor |
|---|---|---|---|
| Access level description | Full system access | Can manage workspaces and content | View-only access to Planning data when Planning packages are in unequal numbers to Workflow licenses. This license is not available for Planning as a standalone product.|
| Planning area in the Main Menu | ✔ | ✔ | ✔ |
| Users area in the Main Menu | ✔ | View only |   |
| Requests area in the Main Menu | ✔ | ✔ | ✔ |
| Setup area in the Main Menu | ✔ |   |   |
| Manage Workspaces and their content | ✔ | ✔ |   |
| Submit requests | ✔ | ✔ | ✔ |
| Create or edit users | ✔ |   |   |
| View users list | ✔ | View only |   |
| Setup > Teams | ✔ |   |   |
| Setup > Log In As | ✔ |   |   |
| Setup > Custom Quarters | ✔ |   |   |
| Setup > System > Customer info | ✔ |   |   |
| Setup > System > Preferences | ✔ |   |   |

-->
