---
title: Présentation de l’accès à Adobe Workfront Planning
description: Tous les utilisateurs de l’organisation n’ont pas le même accès et les mêmes autorisations pour utiliser Adobe Workfront Planning. Cet article décrit l’accès et les autorisations que les utilisateurs peuvent avoir pour utiliser les fonctionnalités d’Adobe Workfront Planning.
author: Alina
feature: Workfront Planning
recommendations: noDisplay, noCatalog
role: User, Admin
exl-id: 99fac041-a235-4991-b826-d19944164bc9
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/QuLxjUMlRgN0FvlDwR0JVQ-m-wV-z3C6sh30lJYRKfU
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 614b25d3255b27f09f2624afd8691e08cfb7ddf4
workflow-type: tm+mt
source-wordcount: 1002
ht-degree: 15%

---

# Vue d’ensemble de l’accès à Adobe Workfront Planning

<!--do not use the snippet for IMPORTANT , as it links to this article-->


<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

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

Cet article décrit l’accès et les paramètres dont vous avez besoin pour utiliser les fonctionnalités de Workfront Planning.

## Conditions d’accès

<!--do not collapse the access requirements below - this is the main article about Access overview-->

<!--*********ensure that the link ^^^^^^^^below^^^^^^^^ to Workfront Pricing and Packaging now also includes information about Workfront Planning. If not, talk with Lauren S.***************-->

Pour utiliser Workfront Planning, vous devez disposer des droits d&#39;accès suivants :

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
   <tr>
   <tr>
   <td role="rowheader"><p>Package Adobe Workfront</p></td>
   <td>
   <p>Tout package Workfront ou Workflow Planning
   et tout package Workfront Planning</p>
   <p><b>NOTE</b></p>
   <p>Pour accéder aux types d’enregistrements connectables :</p>
   <ul><li><p>Tout package Workfront et un package Planning</p></li>
   <li><p>N’importe quel workflow et un package Planning Prime et Ultimate</p></li></ul>

<p>Pour accéder aux types d’enregistrements globaux :</p>
   <ul><li><p>Tout package Workfront et un package Planning Plus</p></li>
   <li><p>Tout package de workflow et un package Planning Prime et Ultimate</p></li></ul> </td></tr>
   <!--
   <tr>
   <td role="rowheader"><p>Adobe Workfront platform</p></td>
   <td>
   <p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p>
   <p><b>IMPORTANT</b></p>
   <p>Only users added to the Adobe Identity Management System (IMS) can be granted permissions and added to Planning fields.</p>
   <p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p>
   </td>
   </tr>
   -->
   <tr>
   <td role="rowheader"><p>Licence Adobe Workfront</p></td>
   <td>
   <ul><li><p>Tout workflow et toute licence Planning, pour afficher les informations de Workfront Planning.</p></li>
   <li><p>Une norme de workflow et une norme de planification pour créer des espaces de travail et des vues</p></li></ul>
    </td>
   </tr>
   <tr>
   <td role="rowheader"><p>Configurations des niveaux d’accès</p></td>
   <td> <p>Tout workflow et tout type de licence Planning dans le niveau d'accès</p>  
   </td>
   </tr>
   <tr>
   <td role="rowheader"><p>Autorisations d’objet</p></td>
   <td>
   <ul>
   <li><p>Autorisations d’affichage ou supérieures aux espaces de travail, aux types d’enregistrements et aux vues que vous n’avez pas créés pour y accéder et à leurs objets.</p></li>
   <li><p>Autorisations de niveau supérieur ou de niveau supérieur relatives aux espaces de travail et aux types d’enregistrements que vous n’avez pas créés pour les modifier et créer, modifier ou supprimer des types d’enregistrements.</p></li>
   <li><p>Gérer les autorisations de modification, de partage ou de suppression des enregistrements.</p>
   <li><p>Autorisations de niveau Contribution ou supérieur aux vues que vous n’avez pas créées, pour les modifier, les supprimer et les partager</p>
   </li>
    <li><p>Les administrateurs de Planning peuvent gérer les espaces de travail qu'ils n'ont pas créés. </p></li>
    <li><p>Les administrateurs de Planning ne peuvent pas accéder aux vues qu'ils n'ont pas créées. </p></li></ul>
   <p>Pour plus d’informations sur les autorisations de partage pour les objets Workfront Planning, voir <a href="/help/quicksilver/planning/access/sharing-permissions-overview.md">Vue d’ensemble des autorisations de partage dans Adobe Workfront Planning</a>. 
   </td>
   </tr>
   <tr>
   <td role="rowheader"><p>Modèle de mise en page</p></td>
   <td> 
   <p>Les zones Planning sont activées par défaut pour les utilisateurs et les administrateurs de Planning Standard.</p>
   <p> Les utilisateurs disposant d'une licence Workflow Light ou Planning Contributor doivent se voir attribuer un modèle de mise en page qui inclut l'option Planning dans les domaines suivants :</p>
   <ul><li>Menu principal</li>
   <li>Panneau de gauche de projets, portefeuilles et programmes</li>
   </ul>   
   </td>
  </tr>
 </tbody>
</table>

Pour plus d’informations, voir [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


## Niveaux d’accès et licences Workfront Planning

Vous pouvez attribuer une licence d&#39;administrateur Planning à un utilisateur lorsque vous l&#39;ajoutez au Adobe Admin Console en tant qu&#39;administrateur.

Pour plus d’informations, voir [Gestion des utilisateurs dans Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).

Vous ne pouvez pas modifier le niveau d&#39;accès Administrateur Planning dans Workfront Planning.

Vous pouvez attribuer les types de licence suivants lorsque vous configurez des niveaux d’accès dans Workfront :

* Types de licence des workflows
* Types de licence Planning

Pour accéder à Workfront Planning, les utilisateurs doivent disposer des deux types de licence attribués à leur niveau d&#39;accès.

Vous pouvez attribuer les licences Planning suivantes à un niveau d&#39;accès :

* **Planning Standard** : accordez cet accès aux utilisateurs s&#39;ils doivent créer et gérer tous les objets Planning sans être administrateurs.
* **Contributeur Planning** : accordez cet accès aux utilisateurs s&#39;ils doivent contribuer à des enregistrements, mais qu&#39;ils n&#39;ont pas besoin de créer des objets Planning.

  >[!TIP]
  >
  >Le type de licence Contributeur Planning n&#39;est pas disponible si votre organisation a acheté un nombre inégal de licences Workflow et Planning.


* **Aucun** : lorsque vous attribuez ce type de licence Planning, vous supprimez spécifiquement tout accès Planning aux utilisateurs affectés à ce niveau d&#39;accès.

  >[!IMPORTANT]
  >
  >Les licences Planning et les licences Workflow fonctionnent ensemble pour permettre aux utilisateurs d&#39;accéder à Workfront.
  >
  >Vous pouvez accorder à un utilisateur différents niveaux d&#39;accès entre Workflow et Planning, mais la licence Workflow ne peut pas être inférieure à la licence Planning.
  >
  >Par exemple, vous pouvez accorder à un utilisateur une licence Workflow Standard et une licence Planning Contributor, mais vous ne pouvez pas lui accorder de licence Workflow Contributor et de licence Planning Standard.
  >
  >Le type de licence Workflow ne peut pas être vide si l&#39;utilisateur doit accéder à Workflow ou Planning.

Pour plus d’informations, voir [Présentation du type de licence avec Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md).

## Configurer le niveau d’accès

Pour plus d’informations sur la configuration de l’accès dans Workfront, voir [ Création et modification de niveaux d’accès personnalisés ](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

## Attribution de licences aux utilisateurs

Vous pouvez attribuer des licences aux utilisateurs lorsque vous leur attribuez un niveau d&#39;accès lors de leur modification ou de leur création.

Pour plus d’informations, voir [Modifier le profil d’une personne](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Octroyer des autorisations

Vous pouvez accorder des autorisations aux entités suivantes dans Workfront Planning :

* Espaces de travail
* Types d’enregistrements
* Vues
* Enregistrements

Pour plus d’informations, consultez la section [Vue d’ensemble des autorisations de partage dans Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).

Votre type de licence Adobe Workfront fonctionne avec votre type de licence Workfront Planning et vos autorisations Planning pour vous permettre d’afficher, de contribuer ou de gérer des objets Workfront Planning.

Pour plus d’informations sur la façon dont les types de licence affectent les niveaux d’autorisation des objets de Workfront Planning, consultez la section [Vue d’ensemble des types de licence lors de l’utilisation d’Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md).

## Partage de la zone Planning à l&#39;aide d&#39;un modèle de mise en page

<!--First, contact your account manager to obtain access to the current Workfront Planning program.-->

Les zones Planning sont activées par défaut pour les utilisateurs standard et les administrateurs système dans les domaines suivants :

* Menu principal
* Panneau de gauche de projets, portfolios ou programmes

Votre administrateur système doit vous ajouter les zones Planning si vous disposez d’une autre licence Workfront et que vous devez contribuer aux travaux de planification Workfront.

L&#39;administrateur peut ajouter l&#39;option Planification aux zones suivantes en modifiant et en vous affectant à un modèle de mise en page :

* Menu principal
* Page de destination
* Panneau de gauche pour les projets, portfolios et programmes
* Épingles

Pour ajouter ou supprimer des zones Workfront Planning des utilisateurs de votre instance Workfront :

1. Connectez-vous à **Workfront** en tant qu’administrateur ou administratrice système.

1. Accédez à **Menu principal** > **Configuration** > **Interface** > **Modèles de disposition** et ouvrez ou créez un modèle de disposition.

   Pour plus d’informations sur la personnalisation d’un modèle de mise en page, voir [Créer et gérer des modèles de mise en page](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

1. Affectez le modèle de mise en page aux personnes auxquelles vous souhaitez accorder l’accès à Workfront Planning.

   Pour plus d’informations, consultez la section [Affecter des personnes à un modèle de mise en page](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

   Toutes les personnes affectées au modèle peuvent désormais accéder à Workfront Planning dans leur menu principal.

   Les personnes peuvent commencer à créer des espaces de travail, des types d’enregistrements, des enregistrements et des champs.


