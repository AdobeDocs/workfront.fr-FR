---
content-type: reference
product-previous: workfront-goals
navigation-topic: goal-management
title: Conditions requises pour utiliser les objectifs Workfront
description: Votre administrateur Adobe Workfront doit s’assurer que certaines conditions sont remplies avant de pouvoir accéder aux objectifs Adobe Workfront. Dans cet article, découvrez les exigences en matière d’accès, d’autorisations et de mise en page pour accéder aux objectifs Workfront.
author: Alina
feature: Workfront Goals
exl-id: 3c7c832b-3e00-4ced-8829-8b1c23fa3871
source-git-commit: dacfd8ef7475b197ac6ce5dd598c99df97037479
workflow-type: tm+mt
source-wordcount: '644'
ht-degree: 71%

---

# Conditions d’utilisation d’Objectifs Workfront

<!--Audited P&P only: 04/2025-->

Votre administrateur ou administratrice Adobe Workfront doit s’assurer que toutes les conditions suivantes sont remplies avant que vous puissiez accéder à Objectifs Adobe Workfront :

* Votre entreprise a acheté un package Objectifs Adobe Workfront dans le passé. Adobe Workfront Goals ne peut plus être acheté.

  Pour plus d’informations, consultez la section [Accès à l’organisation Workfront Goals](#obtain-workfront-goals-organization-access) de cet article.

* Attribuez-vous le type de licence Workfront approprié. Pour plus d’informations sur l’attribution des types de licences et des niveaux d’accès, voir la section [Mettre à jour les types de licences et les paramètres de niveau d’accès](#update-license-types-and-access-level-settings) dans cet article.

  >[!NOTE]
  >
  >Les utilisateurs disposant d’un type de licence Externe ne peuvent pas accéder aux Objectifs Workfront.

* Accordez-vous un accès aux Objectifs dans votre niveau d’accès. Pour plus d’informations, voir [Accorder l’accès aux Objectifs Adobe Workfront](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).

  >[!NOTE]
  >
  >Par défaut, les utilisateurs n’ont pas accès aux objectifs dans leur niveau d’accès.


* Attribuez-vous le modèle de mise en page qui inclut la zone Objectifs dans le menu principal.

  >[!NOTE]
  >
  >Un modèle de mise en page comprenant la zone Objectifs du menu principal doit être affecté à tous les utilisateurs, y compris les administrateurs système.

  Pour plus d’informations, voir la section [Ajouter Objectifs Workfront à un modèle de mise en page](#add-workfront-goals-to-a-layout-template) dans cet article.

* Si vous devez modifier des objectifs que vous n’avez pas vous-même créés, l’auteur ou l’autrice de l’objectif doit partager les objectifs avec vous et vous accorder les autorisations de gestion.

  Pour plus d’informations, voir la section [Partager des objectifs individuels avec d’autres utilisateurs et utilisatrices](#share-individual-goals-with-other-users) dans cet article.

## Obtenir l’accès d’entreprise aux Objectifs Workfront {#obtain-workfront-goals-organization-access}

Le dernier package Adobe Workfront qui incluait les objectifs de Workfront était Adobe Workfront Ultimate.
Les objectifs Workfront ne peuvent plus être achetés pour les packages plus récents.
Contactez votre représentant de compte pour en savoir plus sur les objectifs Workfront.

<!--Old: >
Depending on which Workfront plan your company is currently on, the following scenarios exist: 

* **A new Workfront plan**: You must have an Ultimate Workfront plan. Workfront Goals are included only in this plan. 

* **A current Workfront plan**: Your organization must purchase an additional license, in addition to the Workfront license.

  After your organization purchases the additional license, Workfront enables Workfront Goals for your account. For information about purchasing a license for Workfront Goals contact your Workfront account manager.

For information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). -->

## Mettre à jour les types de licences et les paramètres de niveau d’accès  {#update-license-types-and-access-level-settings}

Si votre société a accès aux objectifs Workfront d’un achat précédent, votre administrateur Workfront doit vous accorder les autorisations suivantes pour accéder aux objectifs Workfront :

1. L&#39;une des licences suivantes :

   * Contributeur ou version ultérieure
   * Requête ou supérieure

<!--Old: 
* **The new access level model**: Your Workfront administrator must grant you one of the following Workfront license types to access Workfront Goals: 

  * Contributor
  * Light
  * Standard

* **The current access level model**: Your Workfront administrator must grant you one of the following Workfront license types to access Workfront Goals:

  * Plan
  * Work 
  * Review
  * Request
-->

1. Le niveau d&#39;accès suivant :

   * Accédez aux Objectifs ou à un niveau supérieur dans votre niveau d’accès.

   Pour plus d’informations sur l’accès à Objectifs, voir [Accorder l’accès à Objectifs Adobe Workfront](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).

En tant qu’administrateur ou administratrice Workfront, vous pouvez désormais vérifier le nombre de licences Objectifs Workfront dans votre système et savoir combien d’entre elles sont activées. Pour plus d’informations, voir [Gérer les licences disponibles dans votre système](../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

>[!NOTE]
>
>Workfront vous permet d’attribuer plus de licences Objectifs Workfront que celles que vous avez achetées. Cependant, si vous attribuez plus de licences que ce que votre contrat Objectifs Workfront autorise, une personne responsable de votre compte Workfront vous contactera pour vous informer que votre nombre contractuel est dépassé.

## Ajouter Objectifs Workfront à un modèle de mise en page {#add-workfront-goals-to-a-layout-template}

Votre administrateur ou administratrice Workfront ou de groupes doit vous attribuer un modèle de mise en page qui comprend la zone Objectifs dans le menu principal afin que vous puissiez accéder à Objectifs Workfront.

![Modèle de disposition](assets/layout-template-align-highlighted-350x220.png)

Votre administrateur ou administratrice Workfront ou votre administrateur ou administratrice de groupes peut également ajouter les éléments suivants à votre modèle de mise en page afin que vous puissiez facilement accéder à Objectifs Workfront :

* Onglet épinglé
* Faire de la zone Objectifs votre page de destination

Pour plus d’informations sur la mise à jour du modèle de mise en page, voir les articles suivants :

* [Créer et gérer des modèles de mise en page](../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)
* [Personnaliser le menu principal à l’aide d’un modèle de mise en page](../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md)
* [Personnaliser les pages épinglées à l’aide d’un modèle de mise en page](../../administration-and-setup/customize-workfront/use-layout-templates/customize-pinned-pages.md)
* [Personnaliser la page de destination à l’aide d’un modèle de mise en page](../../administration-and-setup/customize-workfront/use-layout-templates/customize-landing-page.md)
* [Affecter des utilisateurs et utilisatrices à un modèle de mise en page](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)

## Partager des objectifs individuels avec d’autres personnes {#share-individual-goals-with-other-users}

Par défaut, toutes les personnes qui disposent au moins d’un accès en affichage à Objectifs dans leur niveau d’accès peuvent afficher tous les objectifs dans Workfront.

Toute personne disposant d’un accès en modification à Objectifs peut créer des objectifs et obtenir automatiquement un accès en gestion sur les objectifs qu’elle crée. Si elle doit modifier les objectifs d’autres utilisateurs ou utilisatrices, une personne disposant des autorisations de gestion sur ces objectifs doit partager avec eux ou elles les objectifs qu’ils ou elles n’ont pas créés.

Pour plus d’informations sur le partage d’objectifs avec des utilisateurs et utilisatrices et leur attribuer des autorisations de gestion, voir [Partager un objectif dans Objectifs Workfront](../../workfront-goals/workfront-goals-settings/share-a-goal.md).
