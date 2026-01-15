---
title: Présentation de l’accès à Adobe Workfront Planning
description: Tous les utilisateurs de l’organisation n’ont pas le même accès et les mêmes autorisations pour utiliser Adobe Workfront Planning. Cet article décrit l’accès et les autorisations que les utilisateurs peuvent avoir pour utiliser les fonctionnalités d’Adobe Workfront Planning.
author: Alina
feature: Workfront Planning
recommendations: noDisplay, noCatalog
role: User, Admin
exl-id: 99fac041-a235-4991-b826-d19944164bc9
source-git-commit: 5d326776b9c5b4d9d24e802375df4630508c8bd0
workflow-type: tm+mt
source-wordcount: '751'
ht-degree: 25%

---


# Présentation de l’accès à Adobe Workfront Planning

<!--do not use the snippet for IMPORTANT , as it links to this article-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

>[!IMPORTANT]
>
>Les informations de cet article font référence à Adobe Workfront Planning, une fonctionnalité supplémentaire d’Adobe Workfront.
>
>Votre société doit acheter un package supplémentaire pour que Workfront Planning puisse accéder à ses fonctionnalités.
>
>Pour plus d’informations, contactez votre gestionnaire de compte
>
>Pour plus d’informations sur Workfront Planning, voir [Prise en main d’Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).

Des restrictions de licence et de partage s’appliquent à l’utilisation d’Adobe Workfront Planning.

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
   <p>Tout package Workfront and Planning</p>
   <p>Tout package Workflow et Planning</p>

<p><b>NOTE</b></p>

<p>Pour accéder aux types d’enregistrements connectables :</p>
   <ul><li><p>Tout package Workfront et un package Planning</p></li>
   <li><p>N’importe quel workflow et un package Planning Prime et Ultimate</p></li></ul>

<p>Pour accéder aux types d’enregistrements globaux :</p>
   <ul><li><p>Tout package Workfront et un package Planning Plus</p></li>
   <li><p>Tout package de workflow et un package Planning Prime et Ultimate</p></li></ul> </td></tr>

<tr>
   <td role="rowheader"><p>Plateforme Adobe Workfront</p></td>
   <td>
   <p>L’instance de Workfront de votre organisation doit être intégrée à l’expérience unifiée Adobe pour pouvoir accéder à Workfront Planning.</p>
   <p><b>IMPORTANT</b></p>
   <p>Seuls les utilisateurs ajoutés au système Adobe Identity Management (IMS) peuvent se voir accorder des autorisations et être ajoutés aux champs Planning.</p>
   <p>Pour plus d’informations, voir <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience pour Workfront</a>. </p>
   </td>
  </tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Licence Adobe Workfront</p></td>
   <td>
   <ul><li><p>Tous, pour afficher les informations de planification Workfront</p></li>
   <li><p>Standard, pour créer des espaces de travail et des vues</p></li></ul>
    </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Configurations du niveau d’accès</p></td>
   <td> <p>Il n’existe aucun contrôle de niveau d’accès pour Adobe Workfront Planning.</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Autorisations d’objet</p></td>
   <td>
   <ul>
   <li><p>Autorisations d’affichage ou supérieures aux espaces de travail, aux types d’enregistrements et aux vues que vous n’avez pas créés pour y accéder et à leurs objets.</p></li>
   <li><p>Accordez des autorisations supérieures ou supérieures aux espaces de travail et aux types d’enregistrements que vous n’avez pas créés pour les modifier et créer, modifier ou supprimer des types d’enregistrements et des enregistrements.</p></li>
   <li><p>Autorisations de niveau Contribution ou supérieur aux vues que vous n’avez pas créées, pour les modifier, les supprimer et les partager</p>
   </li>
    <li><p>L’administration système peut gérer les espaces de travail qu’elle n’a pas créés. </p></li>
    <li><p>Les administrateurs système ne peuvent pas accéder aux vues qu'ils n'ont pas créées. </p></li></ul>
   <p>Pour plus d’informations sur les autorisations de partage pour les objets Workfront Planning, voir <a href="/help/quicksilver/planning/access/sharing-permissions-overview.md">Vue d’ensemble des autorisations de partage dans Adobe Workfront Planning</a>. 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Modèle de mise en page</p></td>
   <td> 
<p>Les zones Planning sont activées par défaut pour les utilisateurs standard et les administrateurs système.</p>
<p> Les utilisateurs disposant d'une licence light ou contributor doivent se voir attribuer un modèle de mise en page qui inclut l'option Planning dans les domaines suivants :</p>
   <ul><li>Menu principal</li>
   <li>Panneau de gauche de projets, portefeuilles et programmes</li>
   </ul>   
</td>
  </tr>
 </tbody>
</table>

Pour plus d’informations, voir [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


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

## Attribution de licences aux utilisateurs

Vous pouvez attribuer des licences aux utilisateurs lorsque vous configurez leur niveau d&#39;accès lors de leur modification ou de leur création.

Pour plus d’informations, voir [Modification des profils d’un utilisateur](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)

## Configurer le niveau d’accès

Il n’existe aucun contrôle de niveau d’accès Workfront pour Workfront Planning.

Les utilisateurs disposant de n&#39;importe quel type de licence Workfront peuvent accéder à Workfront Planning.

<!--For information about granting access in Workfront, see [Create and modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Octroyer des autorisations

Vous pouvez accorder des autorisations aux entités suivantes dans Workfront Planning :

* Espaces de travail
* Types d’enregistrements
* Vues
  <!--move this above Views: * <span class="preview">Records</span>-->

Pour plus d’informations, consultez la section [Vue d’ensemble des autorisations de partage dans Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).

Votre type de licence Adobe Workfront fonctionne avec vos autorisations Workfront Planning pour vous permettre d’afficher, de contribuer ou de gérer des objets Workfront Planning.

Pour plus d’informations sur la façon dont les types de licence affectent les niveaux d’autorisation des objets de Workfront Planning, consultez la section [Vue d’ensemble des types de licence lors de l’utilisation d’Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md).


