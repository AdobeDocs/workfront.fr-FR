---
title: Créer des types d’enregistrements
description: Les types d’enregistrements sont les types d’objets d’Adobe Workfront Planning. Dans Workfront Planning, vous pouvez créer des types d’enregistrements personnalisés qui illustrent les éléments de travail nécessaires au cycle de vie de votre entreprise.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: ed1c4954-b338-4865-a7a9-5ba0192e7b37
source-git-commit: 6d9583f8a0e1e0c3712c8a47d68c5d5d321679f9
workflow-type: tm+mt
source-wordcount: '993'
ht-degree: 64%

---


<!--this is linked to the UI in an empty workspace screen-->

# Créer des types d’enregistrements

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Les types d’enregistrements sont les types d’objets d’Adobe Workfront Planning. Dans Workfront Planning, vous pouvez créer des types d’enregistrements personnalisés qui illustrent les éléments liés au travail nécessaires tout au long du cycle de vie de votre organisation.

Pour plus d’informations sur les types d’enregistrements, voir [Présentation des types d’enregistrements](/help/quicksilver/planning/architecture/overview-of-record-types.md).

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
<p>L’instance de Workfront de votre entreprise doit être intégrée à l’expérience unifiée Adobe pour pouvoir accéder à toutes les fonctionnalités de Workfront Planning.</p> 
<p>Pour plus d’informations, voir <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience pour Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront*</p></td> 
   <td><p> Standard</p>
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
   <td>   <p>Gérer des autorisations relatives à un espace de travail</a> </p>  
   <p>L’administration système a accès à tous les espaces de travail, y compris ceux qu’elle n’a pas créés.</p>  </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modèle de disposition</p></td> 
   <td> <p>Toutes les personnes, y compris les administrateurs et administratrices de Workfront, doivent se voir attribuer un modèle de mise en page incluant la zone Planning dans le menu principal. </p> </td> 
  </tr> 
</tbody> 
</table>

* Pour plus d’informations sur les exigences d’accès à Workfront, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Remarques concernant la création de types d’enregistrements

* Vous pouvez créer des types d’enregistrements dans un espace de travail de la manière suivante :

   * Automatiquement :
      * Lorsque vous créez un espace de travail à l’aide d’un modèle.

        Pour plus d’informations, voir [Créer des espaces de travail](/help/quicksilver/planning/architecture/create-workspaces.md).

      * Lorsque vous les importez à l’aide d’un fichier CSV ou Excel.

     >[!TIP]
     >
     >Lorsque vous importez un type d’enregistrement à partir d’un fichier CSV ou Excel, vous pouvez également importer des enregistrements et des champs.

   * Manuellement :

      * À partir de zéro.

        Cet article décrit comment créer des types d’enregistrements à partir de zéro.

* Vous pouvez déplacer des types d’enregistrements dans une section et d’une section d’un espace de travail vers une autre. Vous ne pouvez pas déplacer des types d’enregistrements d’un espace de travail vers un autre.

## Créer des types d’enregistrements à l’aide d’un modèle d’espace de travail

Vous pouvez créer automatiquement des types d’enregistrements lorsque vous créez un espace de travail à l’aide d’un modèle Workfront Planning. Chaque modèle contient des exemples de types d’enregistrements.

Lorsque vous créez un espace de travail à partir d’un modèle, les types d’enregistrements sont regroupés dans les sections suivantes :

* Types d’enregistrements opérationnels
* Taxonomies

Vous pouvez ajouter manuellement des types d’enregistrements dans les sections Types d’enregistrements opérationnels et Taxonomies.

Pour plus d’informations sur la création d’espaces de travail, voir [Créer des espaces de travail](/help/quicksilver/planning/architecture/create-workspaces.md).

Pour plus d’informations sur les types d’enregistrements inclus dans chaque modèle, voir [Liste des modèles d’espace de travail](/help/quicksilver/planning/architecture/workspace-templates.md).

## Créer un type d’enregistrement à partir de zéro

{{step1-to-planning}}

1. Cliquez sur l’espace de travail dans lequel vous souhaitez créer un type d’enregistrement,

   Ou

   Depuis un espace de travail, développez la flèche pointant vers le bas à droite d’un nom d’espace de travail existant, recherchez un espace de travail, puis sélectionnez-le lorsqu’il s’affiche dans la liste.
1. (Facultatif) Cliquez sur **Ajouter une section** pour ajouter une section à l’espace de travail.
1. Cliquez sur **Ajouter un type d’enregistrement** puis **Nouveau**.

   La boîte de dialogue Ajouter un type d’enregistrement s’ouvre.
   <!--1. (Conditional) When creating record types by importing an Excel or CSV file is enabled, click **From scratch**. Otherwise, the **Add record type** box opens. -->

   ![Ajout d’une zone de type d’enregistrement avec des options d’apparence](assets/add-record-type-box-with-appearance-options.png)

1. Mettez à jour les informations suivantes :

   * Remplacez « Type d’enregistrement sans titre » par le nom de votre futur type d’enregistrement. <!--did they bring back the field label here and did they rename it to "Name"-->
   * **Description** : ajoutez des informations supplémentaires sur le type d’enregistrement.
   * Sélectionnez une couleur et une forme pour l’icône associée au type d’enregistrement. Procédez comme suit :
      * Sélectionnez une couleur pour identifier votre nouveau type d’enregistrement. Il s’agit de la couleur de l’icône du type d’enregistrement. Le gris est sélectionné par défaut.
      * Sélectionnez une icône dans la liste ou commencez à saisir le nom d’une icône pour décrire ce qu’elle représente, puis sélectionnez-la lorsqu’elle s’affiche. Il s’agit de l’icône du type d’enregistrement. Une icône de fichier est sélectionnée par défaut.

1. Cliquez sur **Créer**.

   La carte du type d’enregistrement est ajoutée à la section et à l’espace de travail que vous avez sélectionné.
La Description du type d’enregistrement s’affiche sur la carte.

   ![Carte de type enregistrement avec description](assets/record-type-card-with-description.png)

1. (Facultatif) Pointez sur la carte de type d’enregistrement, cliquez sur l’icône **Plus** ![Menu Plus](assets/more-menu.png) dans le coin supérieur droit, puis cliquez sur **Modifier** pour modifier les informations sur le type d’enregistrement.
1. (Facultatif) Cliquez sur la carte du type d’enregistrement pour ouvrir la page du type d’enregistrement.

   ![Type d’enregistrement opérationnel vide](assets/operational-record-type-blank.png)

   La page du type d’enregistrement s’affiche par défaut dans la vue de tableau. Les colonnes du tableau sont des champs associés au nouveau type d’enregistrement. Chaque ligne est un enregistrement unique que vous devez ajouter.

   Par défaut, les champs suivants s’affichent dans les colonnes de la vue Tableau d’un type d’enregistrement opérationnel :

   * Nom
   * Description
   * Date de début
   * Date de fin
   * Statut

1. (Facultatif) Mettez à jour le nom du type d’enregistrement dans l’en-tête de la page

   Ou

   Cliquez sur l’icône **Plus** ![Menu Plus](assets/more-menu.png) à droite du nom du type d’enregistrement et cliquez sur **Modifier** pour le renommer ou modifier les informations le concernant. Pour plus d’informations, voir [Modifier les types d’enregistrements](/help/quicksilver/planning/architecture/edit-record-types.md).

1. (Facultatif) Cliquez sur **+ Nouvel enregistrement** pour ajouter des enregistrements du type sélectionné. Pour plus d’informations, voir [Créer des enregistrements](/help/quicksilver/planning/records/create-records.md).
1. (Facultatif) Cliquez sur l’icône **+** dans le coin supérieur droit du tableau pour ajouter des champs supplémentaires au type d’enregistrement.

   Pour plus d’informations sur la création de champs, voir [Créer des champs](/help/quicksilver/planning/fields/create-fields.md).

1. (Facultatif) Cliquez sur la flèche pointant vers la gauche du nom du type d’enregistrement, dans l’en-tête, pour revenir à l’espace de travail sélectionné.

1. (Facultatif) Dans l’espace de travail, cliquez sur une carte de type d’enregistrement et maintenez-la enfoncée pour faire glisser et déposer le type d’enregistrement à un emplacement souhaité, ou pour le déplacer vers une autre section.

   Les modifications sont enregistrées automatiquement.

   Pour plus d’informations sur l’ajout d’enregistrements, la suppression ou la modification de types d’enregistrements, ou la mise à jour de la vue dans la page du type d’enregistrement, voir les articles suivants :

   * [Créer des enregistrements](/help/quicksilver/planning/records/create-records.md)
   * [Supprimer des types d’enregistrements](/help/quicksilver/planning/architecture/delete-record-types.md)
   * [Modifier des types d’enregistrements](/help/quicksilver/planning/architecture/edit-record-types.md)
   * [Gérer les vues d’enregistrement](/help/quicksilver/planning/views/manage-record-views.md)

## Créer des types d’enregistrements en important des informations depuis un fichier CSV ou Excel

Vous pouvez importer les éléments suivants lors de l’importation d’informations à partir d’un fichier CSV ou Excel :

* Types d’enregistrements
* Enregistrements
* Champs d’enregistrement

Pour plus d’informations, voir [Création de types d’enregistrements à partir d’un fichier CSV ou Excel](/help/quicksilver/planning/architecture/import-file-to-create-record-types.md).


