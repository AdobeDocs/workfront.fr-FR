---
title: Créer des espaces de travail
description: Un espace de travail est une collection de types d’enregistrements utilisés par une équipe et représente le cycle de vie du travail de l’équipe. Vous pouvez entièrement personnaliser les espaces de travail dans Adobe Workfront Planning. Les types d’enregistrements sont organisés par sections dans un espace de travail.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 604b84c1-4ec6-4d4a-b9f4-4223641ff2ea
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 43%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Créer des espaces de travail

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Dans Adobe Workfront Planning, les espaces de travail sont des emplacements centralisés permettant aux équipes de planifier le travail.

Un espace de travail est une collection de types d’enregistrements utilisés par une équipe et représente le cycle de vie du travail de l’équipe. Vous pouvez entièrement personnaliser les espaces de travail dans Adobe Workfront Planning.

Pour obtenir des informations générales sur les espaces de travail, voir [Présentation des espaces de travail](/help/quicksilver/planning/architecture/workspaces-overview.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Produits</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Planification d’Adobe Workfront<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Formule Adobe Workfront*</p></td> 
   <td> 
<p>L’un des plans Workfront suivants :</p> 
<ul><li>Sélectionner</li> 
<li>Principal</li> 
<li>Final</li></ul> 
<p>Workfront Planning n’est pas disponible pour les plans Workfront hérités</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Package Adobe Workfront Planning*</p></td> 
   <td> 
<p>Tous </p> 
<p>Pour plus d’informations sur les éléments inclus dans chaque plan de planification Workfront, contactez votre gestionnaire de compte Workfront. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Plateforme Adobe Workfront</p></td> 
   <td> 
<p>L’instance de Workfront de votre organisation doit être intégrée à l’expérience unifiée Adobe pour pouvoir accéder à Workfront Planning.</p> 
<p>Pour plus d’informations, voir <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience pour Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront*</p></td> 
   <td><p> Standard </p>
   <p>Workfront Planning n’est pas disponible pour les licences Workfront héritées</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuration du niveau d’accès</p></td> 
   <td> <p>Il n’existe aucun contrôle de niveau d’accès pour Adobe Workfront Planning.</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td>   <p>Vous recevez des autorisations de gestion pour les espaces de travail que vous créez. </p> </td> 
  </tr> 
</tbody> 
</table>

* Pour plus d’informations sur les exigences d’accès à Workfront, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Créer un espace de travail

Vous pouvez créer un espace de travail et y ajouter des types d’enregistrements afin d’organiser vos objets dans Workfront Planning. Pour plus d’informations sur la modification d’un espace de travail, voir [Modifier les espaces de travail](/help/quicksilver/planning/architecture/edit-workspaces.md).

{{step1-to-planning}}

1. Cliquez sur **Créer un espace de travail**

   La zone Créer un espace de travail s’affiche. Vous pouvez créer un espace de travail à partir de zéro ou à l’aide de l’un des modèles disponibles.

1. (Facultatif et le cas échéant) Cliquez sur **Prévisualisation** dans l’un des modèles d’espace de travail prédéfinis suivants :

   * De base : Marketing Management
   * Avancé : Marketing Management
   * Entreprise : Marketing Management
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

   * Un espace de travail vide nommé **Workspace sans titre** dans lequel vous pouvez commencer à ajouter manuellement des types d’enregistrements lorsque vous créez un espace de travail à partir de zéro.
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


