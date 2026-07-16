---
title: Présentation Du Type De Licence Lors De L’Utilisation D’Adobe Workfront Planning
description: Votre accès à Adobe Workfront Planning dépend de votre type de licence et de vos autorisations d'objets. Tous les utilisateurs de l’organisation n’ont pas le même accès et les mêmes autorisations pour utiliser Adobe Workfront Planning. Cet article décrit les niveaux d’accès que les utilisateurs peuvent avoir à Adobe Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 10dee6f9-06ff-435a-81a4-2125642fab59
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/2V2i9ZZOyQ6gShXK-QUKDeCZCxcrbYwb8-mn-9kQbc8
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
source-git-commit: ab0d036ea3bbcdad2daaed6b09864272fd1beb11
workflow-type: tm+mt
source-wordcount: 958
ht-degree: 3%

---

# Vue d’ensemble du type de licence lors de l’utilisation d’Adobe Workfront Planning

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

<!--{{planning-important-intro}}-->

>[!IMPORTANT]
>
>Les informations de cet article se rapportent à Adobe Workfront Planning. Workfront Planning est un produit autonome ou une fonctionnalité d’Adobe Workfront achetée en plus.
>
>
>Cet article contient des informations générales sur Workfront Planning lorsque les clients achètent également un Workfront ou un package de workflow.
>
>Pour obtenir la liste complète des articles contenant de la documentation pour Workfront Planning, consultez [Informations générales et index des articles pour Adobe Workfront Planning](/help/quicksilver/planning/planning-information.md).
>
>Pour plus d’informations sur Workfront Planning en tant que produit autonome, voir [Prise en main d’Adobe Workfront Planning en tant que produit autonome](/help/quicksilver/planning/planning-sta/planning-sta-overview.md).

Votre type de licence Adobe Workfront Workflow fonctionne conjointement avec votre type de licence Adobe Workfront Planning et avec les autorisations Planning pour accorder les accès suivants :

* Afficher, contribuer ou gérer des espaces de travail, des types d’enregistrements et des enregistrements.
* Afficher ou gérer des vues.

Pour plus d’informations sur les autorisations sur les objets Workfront Planning, consultez [Vue d’ensemble du partage d’autorisations dans Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).

Pour plus d’informations sur l’accès à Workfront Planning, consultez [Présentation de l’accès à Adobe Planning](/help/quicksilver/planning/access/access-overview.md).

## Relation entre les types de licence Workflow et Planning

Les niveaux d&#39;accès des utilisateurs peuvent être associés aux types de licence suivants :

* Type de licence de workflow
* Type de licence Planning

Pour plus d’informations, voir [Créer et modifier des niveaux d’accès personnalisés](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Le type de licences Planning disponibles pour affecter des utilisateurs diffère selon le package Workfront acheté par votre entreprise.

<!--

This list also exists here: \help\quicksilver\planning\planning-sta\planning-sta-overview.md
-->

Votre entreprise peut acheter Workfront Planning de plusieurs manières :

* Avec un package de workflow Workfront, avec un nombre égal de licences pour Workflow et Planning. Les utilisateurs ont accès à toutes les fonctionnalités d&#39;Adobe Workfront Workflow et de Planning.
* Avec un package de workflow Workfront, avec un nombre de licences différent pour Workflow et Planning. Les utilisateurs bénéficient d’un accès à toutes les fonctionnalités du workflow Adobe Workfront et d’un accès limité à Workfront Planning.
* Workfront Planning en lui-même, en tant que produit autonome. Les utilisateurs et utilisatrices ne reçoivent pas l’accès aux fonctionnalités de workflow de Workfront et disposent d’un accès complet aux fonctionnalités de Workfront Planning. Pour plus d’informations, voir [Prise en main d’Adobe Workfront Planning en tant que produit autonome](/help/quicksilver/planning/planning-sta/planning-sta-overview.md).

Le tableau ci-dessous décrit la relation entre les types de licence Workflow et Planning, ainsi que les fonctionnalités des utilisateurs en fonction de ces licences :

| Package Workfront | Types de licences Planning | Types de licence de workflow | Fonctionnalités de licence |
|---|---|---|---|
| Planning et workflow - Nombre égal de licences | Standard, Contributeur, Aucun Accès | Standard, Léger, Contributeur | - Les types de licence Planning et Workflow sont des paramètres distincts sur les niveaux d&#39;accès<br>- Le type de licence Planning autorise les options Standard, Contributeur et vide<br>- Le type de licence Planning peut être laissé vide sur n&#39;importe quel niveau d&#39;accès - Les utilisateurs avec ce niveau d&#39;accès n&#39;ont pas accès à Planning<br>- Le type de licence Workflow ne peut pas être laissé vide<br>- La combinaison de licence Planning Standard avec la licence Contributeur Workflow n&#39;est pas autorisée<br>- Planning Standard peut être sélectionné uniquement avec les licences Workflow Light et Standard |
| Planification et workflow - Nombre inégal de licences | Standard, pas d’accès | Standard, Léger, Contributeur | - Les types de licence Planning et Workflow sont des paramètres distincts sur les niveaux d&#39;accès<br>- Le type de licence Planning autorise uniquement les options Standard ou Aucun accès<br> - Planning Standard peut être sélectionné avec n&#39;importe quel type de licence Workflow<br> - Le type de licence Planning peut être Aucun - Les utilisateurs avec ce niveau d&#39;accès n&#39;auront pas accès aux données Planning du tout<br>- Le type de licence Workflow ne peut pas être laissé vide sur n&#39;importe quel niveau d&#39;accès<br>- Les utilisateurs avec une licence Planning Contributor peuvent afficher les objets Workflow connectés dans Planning, mais ne peuvent pas se connecter ni se déconnecter |

Pour plus d’informations sur les licences dans Workfront Planning, consultez [Présentation de l’accès à Adobe Workfront Planning](/help/quicksilver/planning/access/access-overview.md).

<!--
not sure if we need this anymore, this is before STA launched:

| Adobe Workfront license type                                   | Highest permissions allowed in Adobe Workfront Planning                                                                                                                                             |
|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|Standard                     | <p>Users can manage workspaces, record types, records, and views. They can create, edit, or delete workspaces, record types, records, fields, and views.</p><br><p>System administrators have Manage permissions to all workspaces, including the ones they did not create.</p>                                                                                                                     |
| Light or Contributor  | <p>Users can view the workspaces shared with them, as well as the record types, records, and fields of those workspaces.</p> <br> <p>Users can view the views shared with them, but they cannot create their own. </p><br> <p>Users cannot create, edit, or delete workspaces, record types, records, or fields.</p>|
-->

<!--
Old: 
*Workfront Planning is not available for legacy Workfront licenses. 
For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
-->


## Types de licence et autorisations des espaces de travail et des types d’enregistrement

L’octroi des autorisations d’un utilisateur à un espace de travail lui accorde également des autorisations sur les types d’enregistrements, les enregistrements et les champs.

Pour pouvoir accéder aux vues et les gérer, vous devez accorder aux utilisateurs des autorisations distinctes aux vues, en plus de celles dont ils disposent pour les espaces de travail.

Tenez compte des points suivants lorsque vous utilisez des autorisations de type enregistrement :

* Les utilisateurs héritent automatiquement des autorisations de type d’enregistrement des espaces de travail.
* Lorsque l’utilisateur dispose d’autorisations de niveau Gérer sur un espace de travail, il ne peut pas avoir un accès moindre à un type d’enregistrement.
* Les utilisateurs ne peuvent pas disposer d’autorisations plus importantes pour un type d’enregistrement que pour l’espace de travail auquel appartient le type d’enregistrement.
* La suppression des autorisations des utilisateurs sur un type d’enregistrement ne supprime pas leur accès en lecture seule à tous les types d’enregistrements dans l’espace de travail, car cela ne supprime pas leurs autorisations sur l’espace de travail.

Seuls les utilisateurs disposant d&#39;une licence Planning Standard peuvent disposer d&#39;autorisations Contribute ou Gérer sur les espaces de travail et les types d&#39;enregistrements. Les autorisations Contribuer et Gérer des espaces de travail et des types d’enregistrements sont également transférés vers les enregistrements et les champs, par défaut.

Les administrateurs peuvent afficher tous les espaces de travail du système, y compris ceux qu’ils n’ont pas créés.

<!--
Lilit asked for this to be removed as there is no Planning Admin license/ access for combos: 
>[!TIP]
>
>Planning Administrator access is automatically assigned to users that you create as Administrators in the Adobe Admin Console. 
>
>For information, see [Manage users in the Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).

Users with all other license types can have View permissions to workspaces and record types  shared with them, as well as to their records and fields. 
-->

>[!INFO]
>
>**EXEMPLE :**
>
>Les utilisateurs de Planning Contributors ou Workflow Light ne peuvent pas contribuer aux espaces de travail et à leurs objets ni les gérer.
>
>Le champ Partage indique que les utilisateurs ne peuvent pas être autorisés à contribuer à ou gérer un espace de travail s’ils disposent d’une licence de niveau inférieur, car ces niveaux d’autorisation sont grisés.
>
>![Autorisations grisées pour l’utilisateur contributeur sur l’espace de travail](assets/permissions-grayed-out-for-contributor-user-on-workspace.png)


## Types de licences et autorisations des vues

Seuls les utilisateurs disposant d&#39;une licence Planning Standard peuvent disposer d&#39;autorisations de gestion pour les vues.

Les administrateurs ne peuvent pas accéder aux vues qu’ils n’ont pas créées. Ils doivent être partagés avec eux.

Les utilisateurs disposant de tous les autres types de licence peuvent disposer d&#39;autorisations d&#39;affichage des vues partagées avec eux.

>[!INFO]
>
>**EXEMPLE**
>
>Les contributeurs Planning ou les utilisateurs de licence light Workflow ne peuvent pas gérer les vues. Ils peuvent appliquer des filtres, des tris ou des regroupements temporaires aux vues auxquelles ils ont accès.
>
>Le champ Partage indique que les utilisateurs ne peuvent pas se voir accorder d’autorisations pour gérer une vue s’ils disposent d’une licence de niveau inférieur, car ces niveaux d’autorisations sont grisés.
>
>![Autorisations grisées pour un utilisateur léger sur le partage d’affichage](assets/permissions-grayed-out-for-light-user.png)
