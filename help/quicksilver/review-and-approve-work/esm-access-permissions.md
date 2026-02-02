---
product-area: documents
navigation-topic: approvals
title: Autorisations d’objet et présentation du niveau d’accès pour le modèle de stockage d’entreprise Adobe
description: présentation des autorisations et de l’accès au stockage d’Adobe enterprise
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
hide: true
hidefromtoc: true
source-git-commit: 89dcc972e2e29890763dba6b5f7a44489a2eee5a
workflow-type: tm+mt
source-wordcount: '537'
ht-degree: 0%

---


# Autorisations d’objet et présentation du niveau d’accès pour le modèle de stockage d’entreprise Adobe

<!--linked in UI -->

Le stockage d’entreprise Adobe est une solution de stockage cloud qui sert de référentiel de stockage central pour les ressources des produits d’entreprise Adobe. Les environnements Workfront qui utilisent le stockage d’entreprise Adobe ont des autorisations d’objet et des comportements de niveau d’accès légèrement différents de ceux qui utilisent le stockage de documents Workfront hérité.

## Niveaux d&#39;accès

Les niveaux d’accès Workfront s’appliquent uniquement dans Workfront. Les restrictions de projet et de document dans Workfront ne s’appliquent pas toujours aux autres applications Adobe.

### Environnements utilisant le stockage d’entreprise Adobe et le stockage Workfront hérité

L’accès aux documents se comporte différemment selon que le projet se trouve sur un stockage d’entreprise Adobe ou sur un stockage Workfront hérité :

* **Stockage Workfront hérité** : les projets, programmes, portfolios et modèles qui utilisent le stockage Workfront hérité suivent la logique de niveau d’accès Workfront standard pour l’accès aux documents. Lorsqu’un niveau d’accès **Aucun accès** est sélectionné pour les documents, ils ne peuvent pas voir les documents dans Workfront ou d’autres produits Adobe tels que Frame.io ou Creative Cloud.
* **Stockage d’entreprise Adobe** : les projets, programmes, portfolios et modèles qui utilisent le stockage d’entreprise Adobe suivent la logique de niveau d’accès au stockage d’entreprise Adobe pour d’autres produits Adobe.


   * **Autorisations d’objet de projets, programmes, portfolios et modèles** : lorsqu’un niveau d’accès n’a **Aucun accès** sélectionné pour les projets, programmes, portfolios et modèles, mais que l’objet est partagé avec eux, les utilisateurs ne peuvent pas voir l’objet dans Workfront, mais ils peuvent toujours afficher le nom de l’objet et tous les documents associés dans d’autres outils Adobe, tels que Frame.io et Adobe Creative Cloud.
   * **Autorisations des documents** : lorsqu’un niveau d’accès **Aucun accès** est sélectionné pour les documents, les utilisateurs ne peuvent pas voir les documents des projets dans Workfront, mais ils peuvent toujours afficher et gérer des documents pour les projets partagés avec eux dans d’autres outils Adobe, tels que Frame.io et Adobe Creative Cloud. En effet, l’accès aux documents est déterminé par les autorisations au niveau du projet dans le stockage d’entreprise Adobe, plutôt que par les seuls niveaux d’accès Workfront.

Si le stockage d’entreprise Adobe est activé dans votre environnement Workfront, vous pouvez créer des projets de stockage d’entreprise Adobe et des projets de stockage Workfront hérités. Les projets de stockage Workfront hérités affichent une icône en regard du nom du projet à l’endroit où il s’affiche dans Workfront. Les projets de stockage d’entreprise Adobe n’affichent pas d’icône.

![icône de stockage workfront héritée en regard du nom du projet](assets/legacy-project-icon.png)


### Environnements utilisant uniquement le stockage d’entreprise Adobe

Vous ne pouvez pas modifier les autorisations de document au niveau de l’accès pour les projets, programmes et portfolios qui utilisent le stockage d’entreprise d’Adobe.

Tous les niveaux d’accès ont un accès en modification aux documents. Les autorisations au niveau du projet déterminent l’accès aux documents dans d’autres outils Adobe.

Vous ne pouvez pas restreindre l’accès à l’héritage des documents.


### Environnements utilisant uniquement le stockage Workfront hérité

Aucune modification des niveaux d’accès aux documents ou du comportement.


## Projets

Les utilisateurs disposant d’autorisations au niveau du projet peuvent afficher et gérer des documents pour les projets dans d’autres produits Adobe tels que Frame.io et Adobe Creative Cloud.

Les noms de projet sont également visibles en dehors de Workfront pour les projets ESM.

Les données financières ne sont pas visibles en dehors de Workfront pour les projets ESM.

## Tâches et événements

Les documents sont stockés au niveau du projet, mais peuvent être partagés avec des tâches et des événements individuels selon les besoins. Les utilisateurs disposant d’un accès aux tâches et aux événements héritent automatiquement de l’accès aux documents du projet. Vous ne pouvez pas modifier leur niveau d’accès. Ils ont un accès en gestion ou aucun accès.