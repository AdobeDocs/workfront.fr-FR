---
content-type: reference
product-previous: workfront-goals
navigation-topic: goal-management
title: Conditions d’utilisation d’Objectifs Workfront
description: Votre administrateur Adobe Workfront doit s’assurer que certaines conditions sont remplies avant de pouvoir accéder aux objectifs Adobe Workfront.
author: Alina
feature: Workfront Goals
exl-id: 3c7c832b-3e00-4ced-8829-8b1c23fa3871
source-git-commit: 811d8076a0b344e863b25aa253a0fb1c102f0435
workflow-type: tm+mt
source-wordcount: '725'
ht-degree: 10%

---

# Conditions d’utilisation d’Objectifs Workfront

Votre administrateur Adobe Workfront doit s’assurer que toutes les conditions suivantes sont remplies avant de pouvoir accéder aux objectifs Adobe Workfront :

<!--drafted for P&P - replace the first bullet with this one when licensing changes: 
* Your company must purchase the correct Adobe Worfront plan or Adobe Workfront Goal license. For information, see the section [Obtain Workfront Goals organization access](#obtain-workfront-goals-organization-access)in this article.-->

* Votre entreprise doit acheter la licence appropriée pour les objectifs Workfront. Pour plus d’informations, reportez-vous à la section [Obtention de l’accès à l’organisation Workfront Goals](#obtain-workfront-goals-organization-access) de cet article.

* Attribuez-vous le type de licence Workfront approprié. Pour plus d’informations sur l’attribution des types de licence et des niveaux d’accès, reportez-vous à la section [Mise à jour des types de licence et des paramètres de niveau d’accès](#update-license-types-and-access-level-settings) de cet article.

>[!NOTE]
>
>Les utilisateurs disposant d’un type de licence externe ne peuvent pas accéder aux objectifs Workfront.

* Accédez aux Objectifs dans votre niveau d’accès. Pour plus d’informations, voir [Accorder l’accès aux objectifs Adobe Workfront](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)

* Attribuez-vous le modèle de mise en page qui inclut la zone Objectifs dans le menu principal.

  >[!NOTE]
  >
  >Tous les utilisateurs, y compris les administrateurs de Workfront, doivent se voir attribuer un modèle de mise en page incluant la zone Objectifs dans le menu principal.

  Pour plus d’informations, reportez-vous à la section [Ajout d’objectifs Workfront à un modèle de mise en page](#add-workfront-goals-to-a-layout-template) de cet article.

* Si vous devez modifier des objectifs que vous n’avez pas vous-même créés, l’auteur de l’objectif doit partager les objectifs avec vous et vous accorder les autorisations de Gestion .

  Pour plus d’informations, reportez-vous à la section [Partage d’objectifs individuels avec d’autres utilisateurs](#share-individual-goals-with-other-users) de cet article.

## Obtention de l’accès de l’organisation aux objectifs Workfront {#obtain-workfront-goals-organization-access}


Selon le plan Workfront actuellement utilisé par votre entreprise, les scénarios suivants existent :

* Si votre société dispose d’un nouveau plan Workfront, vous devez disposer d’un plan Workfront Ultimate. Les objectifs Workfront sont inclus uniquement dans ce plan.

* Si votre société dispose du plan Workfront actuel, votre entreprise doit acheter une licence supplémentaire, en plus de la licence Workfront, pour que vos utilisateurs puissent accéder aux objectifs Workfront.

  Une fois la licence supplémentaire achetée, Workfront active Workfront Goals pour votre compte. Pour plus d’informations sur l’achat d’une licence pour les objectifs Workfront, contactez votre gestionnaire de compte Workfront.

Pour plus d’informations sur les exigences d’accès à Workfront, voir [Exigences d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Mise à jour des types de licence et des paramètres de niveau d’accès  {#update-license-types-and-access-level-settings}

Selon le plan Workfront actuellement utilisé par votre entreprise, les scénarios suivants existent :

* Si votre société dispose du nouveau modèle de niveau d’accès, votre administrateur Workfront doit vous accorder l’un des types de licence Workfront suivants pour accéder aux objectifs Workfront :

   * Contributeur
   * Léger
   * Standard

* Si votre société dispose du modèle de niveau d’accès actuel, votre administrateur Workfront doit vous accorder l’un des types de licence Workfront suivants pour accéder aux objectifs Workfront :

   * Plan
   * Travail
   * Vérifier
   * Demande

Une fois que votre administrateur Workfront vous a accordé l’un de ces types de licences, il doit également vous donner accès aux Objectifs de votre niveau d’accès. Pour plus d’informations sur l’accès aux objectifs, voir [Accorder l’accès aux objectifs Adobe Workfront](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).

En tant qu’administrateur de Workfront, vous pouvez vérifier le nombre de licences Workfront Goals sur votre système et comprendre combien d’entre elles sont actuellement activées. Pour plus d’informations, voir [Gestion des licences disponibles dans votre système](../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

>[!NOTE]
>
>Workfront vous permet d’attribuer plus de licences Objectifs Workfront que votre contrat ne le permet. Cependant, lorsque vous attribuez plus de licences que ce que votre contrat Objectifs Workfront prévoit, une personne gestionnaire de compte Workfront vous contactera pour vous informer que vous avez dépassé le quota de votre contrat.

## Ajout d’objectifs Workfront à un modèle de mise en page {#add-workfront-goals-to-a-layout-template}

L’administrateur Workfront ou Group doit vous attribuer un modèle de mise en page qui comprend la zone Objectifs dans le menu principal afin que vous puissiez accéder aux objectifs Workfront.

![](assets/layout-template-align-highlighted-350x220.png)

Votre administrateur Workfront ou votre administrateur de groupe peut également ajouter les éléments suivants à votre modèle de mise en page afin que vous puissiez facilement accéder aux objectifs Workfront :

* Onglet épinglé
* Faire de la zone Objectifs votre page d’entrée

Pour plus d’informations sur la mise à jour du modèle de mise en page, reportez-vous aux articles suivants :

* [ Créez et gérez des modèles de mise en page](../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)
* [Personnaliser le menu principal à l’aide d’un modèle de mise en page](../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md)
* [Personnaliser les pages épinglées à l’aide d’un modèle de disposition](../../administration-and-setup/customize-workfront/use-layout-templates/customize-pinned-pages.md)
* [Personnaliser la page de destination à l’aide d’un modèle de disposition](../../administration-and-setup/customize-workfront/use-layout-templates/customize-landing-page.md)
* [Affecter des utilisateurs à un modèle de mise en page](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)

## Partage d’objectifs individuels avec d’autres utilisateurs {#share-individual-goals-with-other-users}

Par défaut, tous les utilisateurs qui ont au moins l’accès Afficher aux objectifs dans leur niveau d’accès peuvent afficher tous les objectifs dans Workfront.

Tout utilisateur disposant d’un accès Modifier aux objectifs peut créer des objectifs et obtenir automatiquement l’accès Gérer aux objectifs qu’il crée. S’ils doivent modifier les objectifs d’autres utilisateurs, une personne disposant des autorisations Gérer pour ces objectifs doit partager avec eux les objectifs qu’ils n’ont pas créés.

Pour plus d’informations sur le partage des objectifs avec les utilisateurs et sur la gestion des autorisations, voir [Partage d’un objectif dans les objectifs Workfront](../../workfront-goals/workfront-goals-settings/share-a-goal.md).
