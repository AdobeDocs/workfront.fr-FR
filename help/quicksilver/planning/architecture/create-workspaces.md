---
title: Créer des espaces de travail
description: Un espace de travail est une collection de types d’enregistrements utilisés par une équipe et représente le cycle de vie du travail de l’équipe. Vous pouvez entièrement personnaliser les espaces de travail dans Adobe Workfront Planning. Les types d’enregistrements sont organisés par sections dans un espace de travail.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 604b84c1-4ec6-4d4a-b9f4-4223641ff2ea
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: c4716157a6fdf667f7e608d0c37399f57ec1bbfe
workflow-type: tm+mt
source-wordcount: '1199'
ht-degree: 19%

---


# Créer des espaces de travail

<span class="preview">Les informations de cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de façon générale. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Après les versions mensuelles en production, les mêmes fonctionnalités sont également disponibles dans l’environnement de production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation des versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

Dans Adobe Workfront Planning, les espaces de travail sont des emplacements centralisés permettant aux équipes de planifier le travail.

Un espace de travail est une collection de types d’enregistrements utilisés par une équipe et représente le cycle de vie du travail de l’équipe. Vous pouvez entièrement personnaliser les espaces de travail dans Adobe Workfront Planning.

Pour obtenir des informations générales sur les espaces de travail, voir [Présentation des espaces de travail](/help/quicksilver/planning/architecture/workspaces-overview.md).

## Conditions d’accès

+++ Développez pour afficher les conditions d’accès requises pour la fonctionnalité de cet article. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Package Adobe Workfront</p></td> 
   <td> 
<p>Tout package de Workfront ou de workflow</p> 
<p>Tout package Workfront Planning</p>
<p>Un package Workfront Planning Prime ou version ultérieure <span class="preview">pour créer plusieurs espaces de travail à la fois</span></p>
<p>Pour plus d’informations sur les composants inclus dans chaque package Workfront Planning, contactez votre représentant de compte Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront</p></td> 
   <td><p>Standard</p>
   <p><span class="preview">L’administrateur système peut créer plusieurs espaces de travail à la fois à l’aide du lot de modèles de bonnes pratiques</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td>   <p>Gérer les autorisations d’un espace de travail</p>  
   <p>L’administration système a accès à tous les espaces de travail, y compris ceux qu’elle n’a pas créés.</p>  </td> 
  </tr>  
</tbody> 
</table>

Pour plus d’informations sur les exigences d’accès à Workfront, voir [Exigences d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

<!--
Old:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard </p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>You receive Manage permissions to the workspaces you create. </p> </td> 
  </tr> 
</tbody> 
</table>
-->

## Créer un espace de travail

Vous pouvez créer un espace de travail et y ajouter des types d’enregistrements afin d’organiser vos objets dans Workfront Planning.

Pour plus d’informations sur la modification d’un espace de travail, voir [Modifier les espaces de travail](/help/quicksilver/planning/architecture/edit-workspaces.md).

Vous pouvez créer des espaces de travail comme suit :

* Créer un espace de travail à partir de zéro ou d’un modèle

  Pour plus d’informations, consultez la section [Créer entièrement un espace de travail ou à partir d’un modèle](#create-a-workspace-from-scratch-or-from-a-template) de cet article.
* Créez un espace de travail à l’aide de Planning Designer optimisé par l’IA. Actuellement, cette fonctionnalité n’est disponible que pour un nombre limité de clientes et clients dans un programme Beta.

  Pour plus d’informations, voir [Prise en main d’Adobe Workfront Planning Designer](/help/quicksilver/planning/general/planning-ai-designer.md).

<div class="preview">

* Créer plusieurs espaces de travail à l’aide d’un lot de modèle multi-espace de travail conforme aux bonnes pratiques

  Pour plus d’informations, consultez la section [Créer plusieurs espaces de travail à l’aide d’un lot de modèle multi-espace de travail conforme aux bonnes pratiques](#create-multiple-workspaces-using-a-best-practice-multi-workspace-template-bundle) dans cet article

  >[!TIP]
  >
  >Vous ne pouvez pas créer plusieurs espaces de travail à la fois à moins d’utiliser le lot de modèles de bonnes pratiques.


</div>

### Créer un espace de travail à partir de zéro ou d’un modèle

{{step1-to-planning}}

1. Cliquez sur **Créer un espace de travail**

   La zone Créer un espace de travail s’affiche. Vous pouvez créer un espace de travail à partir de zéro ou à l’aide de l’un des modèles disponibles.

1. (Facultatif et le cas échéant) Cliquez sur **Prévisualisation** dans l’un des modèles d’espace de travail prédéfinis suivants :

   * De base : Gestion marketing
   * Avancé : Gestion marketing
   * Entreprise : Gestion marketing
   * Gestion des ventes
   * Gestion des produits

   La zone d’aperçu du modèle s’ouvre.

   Les types d’enregistrements opérationnels, les taxonomies et le nombre de champs associés à chaque modèle sont indiqués.

   ![Aperçu d’un modèle d’espace de travail](assets/previewing-a-workspace-template.png)

   Pour plus d’informations sur les modèles d’espace de travail de Workfront Planning, voir [Liste des modèles d’espace de travail](/help/quicksilver/planning/architecture/workspace-templates.md).

1. Dans la zone d&#39;aperçu du modèle, cliquez sur **Utiliser le modèle** pour commencer à créer l&#39;espace de travail à partir du modèle sélectionné

   Ou

   Cliquez sur **Précédent** puis sur **Nouvel espace de travail** pour créer entièrement un espace de travail.

   Un des types d’espace de travail suivants est créé :

   * Un espace de travail vide nommé Workspace sans titre **dans lequel vous pouvez commencer à ajouter manuellement des types d’enregistrements lorsque vous créez un espace de travail à partir de zéro.**
   * Un espace de travail nommé en fonction du modèle que vous avez sélectionné et renseigné avec des exemples de types d’enregistrements. Vous pouvez personnaliser davantage les types d’enregistrements et l’espace de travail.

   Pour les administrateurs Workfront, le nouvel espace de travail s’affiche dans l’onglet **Espaces de travail auxquels je participe**.

   Pour tous les autres utilisateurs qui peuvent créer des espaces de travail, le nouvel espace de travail s’affiche dans la zone **Espaces de travail**.

1. Cliquez à l’intérieur du nom de l’espace de travail dans l’en-tête du nouvel espace de travail pour le renommer, puis appuyez sur Entrée.

1. (Facultatif et le cas échéant) Si vous avez créé l’espace de travail à partir d’un modèle, cliquez dans le nom des sections **Types d’enregistrements opérationnels** ou **Taxonomies**.

   Ou

   Pointez sur le nom d’une section, puis cliquez sur le menu **Plus** ![Plus](assets/more-menu.png), puis cliquez sur **Renommer** pour renommer la section.

   >[!TIP]
   >
   >Vous pouvez renommer n’importe quelle section de n’importe quel espace de travail, même si vous n’avez pas créé la section.

   Pour plus d’informations sur la modification des espaces de travail, y compris les sections Espace de travail, voir [Modifier les espaces de travail](/help/quicksilver/planning/architecture/edit-workspaces.md).

1. (Facultatif) Cliquez sur **Ajouter un type d’enregistrement** pour ajouter des types d’enregistrement à l’espace de travail dans n’importe quelle section.

   Pour plus d’informations, voir [Créer des types d’enregistrement](/help/quicksilver/planning/architecture/create-record-types.md).

   Pour plus d’informations sur la modification et la suppression des types d’enregistrements dans un espace de travail, voir [Modifier les espaces de travail](/help/quicksilver/planning/architecture/edit-workspaces.md).

1. (Facultatif) Cliquez sur la flèche vers l&#39;arrière à gauche du nouvel espace de travail pour ouvrir la page principale Planification. Une nouvelle carte d’espace de travail est créée pour le nouvel espace de travail dans l’onglet **Espaces de travail sur lesquels je me trouve**.

   Le nom de l’utilisateur qui a créé l’espace de travail est enregistré sur la carte de l’espace de travail en tant que Propriétaire.

   >[!NOTE]
   >
   >Pour les utilisateurs en cours de transition vers le système Adobe Identity Management (IMS), les espaces de travail créés par des utilisateurs Workfront uniquement qui ne sont pas des utilisateurs IMS s’affichent tels que créés par le **système**.
   >
   >Pour plus d’informations sur IMS, voir [Expérience unifiée Adobe pour Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

<div class="preview">

### Créer plusieurs espaces de travail à l’aide d’un lot de modèle multi-espace de travail conforme aux bonnes pratiques

>[!IMPORTANT]
>
>La création de plusieurs espaces de travail à la fois à l’aide du lot de modèle de bonnes pratiques n’est disponible que lorsque les conditions préalables suivantes sont remplies :
>
>* Votre entreprise a acheté un package Workfront Planning Prime ou Ultimate.
>* Vous êtes administrateur système

Vous pouvez utiliser un lot de modèles d’espaces de travail multiples pour créer 6 espaces de travail en un seul clic.

Les modèles inclus dans l&#39;offre groupée contiennent des espaces de travail, des types d&#39;enregistrements, des enregistrements, des vues et des champs qui vous aideront à démarrer avec l&#39;implémentation de Planning.

>[!IMPORTANT]
>
>Les noms des espaces de travail et des enregistrements inclus dans le lot sont des exemples et ne reflètent pas votre propre environnement.
>
>Les noms des types d’enregistrements et des champs peuvent être utilisés dans n’importe quelle organisation comme norme à implémenter dans n’importe quel secteur, conformément à notre recommandation.
>

{{step1-to-planning}}

1. Cliquez sur **Créer un espace de travail**

   La zone Créer un espace de travail s’affiche. Vous pouvez créer un espace de travail à partir de zéro ou à l’aide de l’un des modèles disponibles.

1. Cliquez sur **Vérifier la configuration de l’espace de travail** dans la zone **Commencer ici (recommandé)**.
1. (Facultatif) Cliquez sur **Aperçu** dans l’un des modèles d’espace de travail prédéfinis suivants pour ouvrir la zone Aperçu pour chaque modèle :

   * 1.Classifications et taxonomies globales

     Le modèle Classifications et taxonomies globales comprend tous les types d’enregistrements et champs que nous vous recommandons de créer dans votre environnement pour une implémentation réussie de Workfront Planning.

     Vous pouvez ensuite lier ou importer les types d’enregistrements de ce modèle dans d’autres espaces de travail que vous créez.
   * 2.Fréscopa Global Marketing
   * 3.Fréscopa Social Marketing
   * 4.Fréscopa Media &amp; PR
   * 5.Événements globaux Fréscopa
   * 6.Fréscopa Direction d&#39;entreprise

1. Après avoir ouvert la zone **Aperçu** pour chaque modèle d’espace de travail, cliquez sur Précédent pour revenir à la zone **Créer un espace de travail** ou cliquez sur Utiliser des modèles pour utiliser les modèles, y compris dans le lot, et créer des espaces de travail.

   Les espaces de travail sont créés et s’affichent dans les onglets **Je suis** et **Tous les espaces de travail** pour les administrateurs système. Tous les utilisateurs disposant d’une licence standard verront les espaces de travail dans leur zone Espaces de travail une fois qu’un administrateur système les aura créés et qu’il aura partagé les nouveaux espaces de travail avec eux.

1. Commencez à modifier les espaces de travail que vous avez créés et à ajouter des types d’enregistrements, des enregistrements, des vues et des champs pertinents pour votre organisation.

   Pour plus d’informations sur les bonnes pratiques relatives à l’implémentation de Workfront, consultez les articles de la section [Bonnes pratiques de planification d’Adobe Workfront : index des articles](/help/quicksilver/planning/best-practices.md/best-practices-article-index.md) .

   Pour plus d’informations sur la modification des espaces de travail, voir [&#x200B; Modifier les espaces de travail &#x200B;](/help/quicksilver/planning/architecture/edit-workspaces.md).

</div>



