---
product-area: documents
navigation-topic: approvals
title: Autorisations d’objet et présentation du niveau d’accès pour le modèle de stockage dans le cloud Adobe
description: présentation des autorisations et de l’accès au stockage dans le cloud d’Adobe
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 758d17e6-f31f-42b7-a9e6-6bd1821f5c15
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/ckHEVC5iDp8A8xidvA16L0csKu0ey8LZHVlA2-QlCgQ
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 944
ht-degree: 1%

---

# Autorisations d’objet et présentation du niveau d’accès pour le modèle de stockage dans le cloud Adobe

<!--linked in UI -->

le stockage dans le cloud d’Adobe est une solution de stockage dans le cloud qui sert de référentiel de stockage central pour les ressources des produits d’entreprise Adobe. Les environnements Workfront qui utilisent le stockage dans le cloud Adobe ont des autorisations d’objet et des comportements de niveau d’accès légèrement différents de ceux qui utilisent le stockage de documents Workfront hérité.

## Niveaux d&#39;accès

Les niveaux d’accès Workfront s’appliquent uniquement dans Workfront. Les restrictions de projet et de document dans Workfront ne s’appliquent pas toujours aux autres applications Adobe.

### Environnements utilisant à la fois le stockage dans le cloud Adobe et le stockage Workfront hérité

L’accès aux documents se comporte différemment selon que le projet se trouve dans l’espace de stockage cloud Adobe ou dans l’espace de stockage Workfront hérité :

* **Stockage Workfront hérité** : les projets, programmes, portfolios et modèles qui utilisent le stockage Workfront hérité suivent la logique de niveau d’accès Workfront standard pour l’accès aux documents. Lorsqu’un niveau d’accès **Aucun accès** est sélectionné pour les documents, ils ne peuvent pas voir les documents dans Workfront ou d’autres produits Adobe tels que Frame.io ou Creative Cloud.
* **Espace de stockage cloud Adobe** : les projets, programmes, portfolios et modèles qui utilisent l’espace de stockage cloud Adobe suivent la logique de niveau d’accès à l’espace de stockage cloud Adobe pour d’autres produits Adobe.


   * **Autorisations d’objet de projets, programmes, portfolios et modèles** : lorsqu’un niveau d’accès n’a **Aucun accès** sélectionné pour les projets, programmes, portfolios et modèles, mais que l’objet est partagé avec eux, les utilisateurs ne peuvent pas voir l’objet dans Workfront, mais ils peuvent toujours afficher le nom de l’objet et tous les documents associés dans d’autres outils Adobe, tels que Frame.io et Adobe Creative Cloud.
   * **Autorisations des documents** : lorsqu’un niveau d’accès **Aucun accès** est sélectionné pour les documents, les utilisateurs ne peuvent pas voir les documents des projets dans Workfront, mais ils peuvent toujours afficher et gérer des documents pour les projets partagés avec eux dans d’autres outils Adobe, tels que Frame.io et Adobe Creative Cloud. En effet, l’accès aux documents est déterminé par les autorisations au niveau du projet dans l’espace de stockage dans le cloud d’Adobe, plutôt que par les seuls niveaux d’accès de Workfront.

Si le stockage dans le cloud Adobe est activé dans votre environnement Workfront, vous pouvez créer des projets de stockage dans le cloud Adobe et des projets de stockage Workfront hérités. Les projets de stockage Workfront hérités affichent une icône en regard du nom du projet à l’endroit où il s’affiche dans Workfront. Les projets de stockage dans le cloud Adobe n’affichent pas d’icône.

![icône de stockage workfront héritée en regard du nom du projet](assets/legacy-project-icon.png)


### Environnements utilisant uniquement l’espace de stockage dans le cloud Adobe

Vous ne pouvez pas modifier les autorisations d’accès aux documents au niveau des projets, programmes et portfolios qui utilisent l’espace de stockage dans le cloud d’Adobe.

Tous les niveaux d’accès ont un accès en modification aux documents. Les autorisations au niveau du projet déterminent l’accès aux documents dans d’autres outils Adobe.

Vous ne pouvez pas restreindre l’accès à l’héritage des documents.


### Environnements utilisant uniquement le stockage Workfront hérité

Aucune modification des niveaux d’accès aux documents ou du comportement.

## Autorisations d’objet

Les autorisations d’objet déterminent ce que vous pouvez voir et faire avec les projets, tâches, événements et documents dans Workfront. Les autorisations sont attribuées lorsqu’une personne partage un objet avec vous.

>[!IMPORTANT]
>
>Dans l’espace de stockage cloud Adobe, les autorisations de document fonctionnent différemment de l’espace de stockage Workfront hérité. Les documents héritent des autorisations du projet, de la tâche ou du problème auxquels ils sont liés.


### Fonctionnement des autorisations de document

Les autorisations de document sont pilotées par l’objet auquel le document est lié. Vous ne pouvez pas définir d’autorisations sur des documents individuels.

Lorsque vous chargez un document vers une tâche ou un événement, un dossier généré par le système est créé à l’aide du nom de la tâche ou de l’événement. Ce dossier est lié à la tâche ou à l’événement et hérite de ses autorisations.

Vous pouvez créer des sous-dossiers dans le dossier généré par le système pour organiser davantage les documents. Tous les sous-dossiers héritent des autorisations du dossier parent. Au niveau du projet, vous pouvez charger des documents en dehors d’un dossier, mais seuls les utilisateurs disposant d’un accès au niveau du projet peuvent les voir.

Au niveau du projet, les dossiers générés par le système affichent un objet lié. Il s’agit généralement du nom de la tâche ou de l’événement, qui indique au système sur quelle tâche ou quel événement le dossier doit s’afficher.

### Autorisations de projet

Lorsque vous disposez d’autorisations au niveau du projet, vous pouvez afficher et gérer des documents pour ce projet dans Workfront et d’autres produits Adobe tels que Frame.io et Adobe Creative Cloud. Le nom du projet est également visible dans ces outils. Les autres données de projet ne sont pas visibles en dehors de Workfront.

### Autorisations des tâches et des événements

Les tâches et les événements héritent des autorisations du projet. Lorsque vous disposez d’autorisations au niveau de la tâche ou du problème, vous pouvez afficher et gérer les documents liés à cette tâche ou à ce problème dans Workfront et d’autres produits Adobe tels que Frame.io et Adobe Creative Cloud.

**Dossiers générés par le système**

* La suppression d’utilisateurs d’une tâche ou d’un événement ne supprime pas automatiquement l’accès au dossier. Ils peuvent toujours y avoir accès par le biais d’autorisations au niveau du projet.
* Les sous-tâches n’héritent pas des autorisations de dossiers générées par le système des tâches parents. Vous devez être ajouté directement à une sous-tâche pour accéder à son dossier généré par le système.
* L’ajout d’utilisateurs à une tâche ou à un problème partage avec eux le dossier généré par le système de cet objet.

**Déplacement et changement de nom des dossiers générés par le système :**

* Les dossiers générés par le système peuvent être renommés et déplacés.
* Si un dossier généré par le système est déplacé vers un autre emplacement, son objet lié est mis à jour vers le nouvel objet . Les autorisations sont alors héritées du nouvel objet parent.

Les requêtes suivent le même comportement que les tâches et les événements.

### Approbations

Lorsque vous êtes ajouté à un workflow d’approbation de document, les éléments suivants s’affichent, quelles que soient les autorisations de projet :

* Nom du projet
* Nom du document
* Miniature du document


## Mappage des autorisations sur Frame.io

Dans le cadre de l’intégration, les autorisations utilisateur sont contrôlées dans Workfront et descendent vers Frame.io. Cela signifie que vous ne pouvez pas inviter un utilisateur à un projet dans Frame.io ni modifier les autorisations utilisateur dans Frame.io. Ces actions doivent être effectuées via la fenêtre modale Partage de projet dans Workfront.

Le tableau suivant montre comment les autorisations Workfront sont mappées aux autorisations Frame.io :

<table>
<tr>
<th>Autorisation utilisateur Workfront</th>
<th>Autorisation utilisateur Frame.io</th>
</tr>
<tr>
<td>Gérer</td>
<td>Modifier et partager</td>
</tr>
<tr>
<td>Contribuer</td>
<td>Modifier et partager</td>
</tr>
<tr>
<td>Afficher</td>
<td>Commentaire uniquement</td>
</tr>
</table>






