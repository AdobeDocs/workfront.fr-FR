---
title: Créer des types d’enregistrements
description: Les types d’enregistrements sont les types d’objets d’Adobe Workfront Planning. Dans Workfront Planning, vous pouvez créer des types d’enregistrements personnalisés qui illustrent les éléments de travail nécessaires au cycle de vie de votre entreprise.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: ed1c4954-b338-4865-a7a9-5ba0192e7b37
source-git-commit: 8546311acf722c0f4d47d4663b02ff701416894a
workflow-type: tm+mt
source-wordcount: '1073'
ht-degree: 50%

---


<!--this is linked to the UI in an empty workspace screen-->

<!--keep the yellow for cross-workspace functionality till Jan 2026-->

# Créer des types d’enregistrements

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Les types d’enregistrements sont les types d’objets d’Adobe Workfront Planning. Dans Workfront Planning, vous pouvez créer des types d’enregistrements personnalisés qui illustrent les éléments liés au travail nécessaires tout au long du cycle de vie de votre organisation.

Pour plus d’informations sur les types d’enregistrements, voir [Présentation des types d’enregistrements](/help/quicksilver/planning/architecture/overview-of-record-types.md).

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
   <td role="rowheader"><p>Package Adobe Workfront</p></td> 
   <td> 
<p>Pour activer les types d’enregistrements connectables : </p>
<ul> 
<li><p>Tout package Workfront et tout package Planning</p></li>
<p>Ou</p>
<li><p>Packages Prime et Ultimate de workflow et de planification</p></li></ul>

<p>Pour activer les types d’enregistrements globaux :</p>

<ul> 
<li><p>Tout package Workfront et un package Planning Plus</p></li>
<p>Ou</p>
<li><p>Packages Prime et Ultimate de workflow et de planification</p></li></ul>
<p>Pour plus d’informations sur les composants inclus dans chaque package Workfront Planning, contactez votre représentant de compte Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront</p></td> 
   <td><p>Standard</p>
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

<!--Old:
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
   <td><p> Standard</p>
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
   <td>   <p>Manage permissions to a workspace</p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>  </td> 
  </tr> 
</tbody> 
</table> -->

## Remarques concernant la création de types d’enregistrements

* Vous pouvez créer des types d’enregistrements dans un espace de travail de la manière suivante :

   * Automatiquement :
      * Lorsque vous créez un espace de travail à l’aide d’un modèle.

        Pour plus d’informations, voir [Créer des espaces de travail](/help/quicksilver/planning/architecture/create-workspaces.md).

      * Lorsque vous les importez à l’aide d’un fichier CSV ou Excel.

        Pour plus d’informations, voir [Création de types d’enregistrements à partir d’un fichier CSV ou Excel](/help/quicksilver/planning/architecture/import-file-to-create-record-types.md).

     >[!TIP]
     >
     >Lorsque vous importez un type d’enregistrement à partir d’un fichier CSV ou Excel, vous pouvez également importer des enregistrements et des champs.

   * Manuellement :

      * À partir de zéro.

        Cet article décrit comment créer des types d’enregistrements à partir de zéro.

     <!--
        * <span class="preview">By adding them from another workspace</span>
            <span class="preview">For information, see [Add existing record types from another workspace](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md). </span>-->


* Vous pouvez déplacer des types d’enregistrements dans une section et d’une section d’un espace de travail vers une autre. Vous ne pouvez pas déplacer des types d’enregistrements d’un espace de travail vers un autre.

## Créer des types d’enregistrements à l’aide d’un modèle d’espace de travail

Vous pouvez créer automatiquement des types d’enregistrements lorsque vous créez un espace de travail à l’aide d’un modèle Workfront Planning. Chaque modèle contient des exemples de types d’enregistrements.

Pour plus d’informations sur la création d’espaces de travail, voir [Créer des espaces de travail](/help/quicksilver/planning/architecture/create-workspaces.md).

Pour plus d’informations sur les types d’enregistrements inclus dans chaque modèle, voir [Liste des modèles d’espace de travail](/help/quicksilver/planning/architecture/workspace-templates.md).

Lorsque vous créez un espace de travail à partir d’un modèle, les types d’enregistrements sont regroupés dans les sections suivantes :

* Types d’enregistrements opérationnels
* Taxonomies

Vous pouvez ajouter manuellement des types d’enregistrements dans les sections Types d’enregistrements opérationnels et Taxonomies . Pour plus d’informations, consultez la section [Créer entièrement un enregistrement](#create-a-record-type-from-scratch) dans cet article.

## Créer un type d’enregistrement à partir de zéro

{{step1-to-planning}}

1. Cliquez sur l’espace de travail dans lequel vous souhaitez créer un type d’enregistrement,

   Ou

   Depuis un espace de travail, développez la flèche pointant vers le bas à droite d’un nom d’espace de travail existant, recherchez un espace de travail, puis sélectionnez-le lorsqu’il s’affiche dans la liste.
1. (Facultatif) Cliquez sur **Ajouter une section** pour ajouter une section à l’espace de travail.
1. Cliquez sur **Ajouter un type d’enregistrement** puis **Ajouter manuellement**.

   La zone Ajouter un type d’enregistrement s’ouvre. <!--update screen shot for preview-->

   ![Ajout d’une zone de type d’enregistrement avec des options d’apparence](assets/add-record-type-box-with-appearance-options.png)

1. Mettez à jour les informations suivantes dans l’onglet **Apparence** :

   * Remplacez « Type d’enregistrement sans titre » par le nom de votre futur type d’enregistrement. <!--did they bring back the field label here and did they rename it to "Name"-->
   * **Description** : ajoutez des informations supplémentaires sur le type d’enregistrement.
   * Sélectionnez une couleur et une forme pour l’icône associée au type d’enregistrement. Procédez comme suit :
      * Sélectionnez une couleur pour identifier votre nouveau type d’enregistrement. Il s’agit de la couleur de l’icône du type d’enregistrement. Le gris est sélectionné par défaut.
      * Sélectionnez une icône dans la liste ou commencez à saisir le nom d’une icône pour décrire ce qu’elle représente, puis sélectionnez-la lorsqu’elle s’affiche. Il s’agit de l’icône du type d’enregistrement. Une icône de fichier est sélectionnée par défaut.

1. (Facultatif et conditionnel) Si vous êtes un administrateur système, cliquez sur **Paramètres avancés** et mettez à jour les informations suivantes dans la section **Fonctionnalité interespace de travail** : <!--the info here is duplicated in the Edit record types article-->
   * Activez le paramètre **Autoriser la connexion à ce type d’enregistrement dans d’autres espaces de travail** : permet aux gestionnaires d’espace de travail de se connecter à ce type d’enregistrement à partir d’autres espaces de travail.\
     Vous pouvez désigner les espaces de travail auxquels ce type d’enregistrement peut être connecté. Vous pouvez le rendre disponible pour tous les espaces de travail ou désigner des espaces de travail spécifiques où vous pouvez l’importer.
Pour plus d’informations, voir [Configuration des fonctionnalités de plusieurs espaces de travail pour les types d’enregistrements](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).


   ![Boîte Créer un type d’enregistrement dans l’onglet Paramètres avancés](assets/create-record-type-box-advanced-settings-tab.png)

   <!--replace last point with this when we release global record types; the preview tags might need to be edited, too:
    1. <span class="preview">(Optional and conditional) If you are a system administrator, update the information in the **Cross-workspace settings** tab.</span>
    <span class="preview">For more information, see [Configure cross-workspace capabilities for record types](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).</span>
    ***********Add screenshot***********
    -->

1. Cliquer sur **Enregistrer**.

   La carte du type d’enregistrement est ajoutée à la section et à l’espace de travail que vous avez sélectionné.
La Description du type d’enregistrement s’affiche sur la carte.

   ![Carte de type enregistrement avec description](assets/record-type-card-with-description.png)

   Si vous avez choisi de connecter cet enregistrement à partir d&#39;autres espaces de travail, l&#39;icône **se connecter à partir d&#39;autres espaces** ![se connecter à partir d&#39;autres espaces](assets/connect-from-other-workspaces-icon.png) s&#39;affiche sur la carte d&#39;enregistrement.

   <!--<span class="preview">If you configured the cross-workspace capabilities for the record, the **connectable record type** icon ![Connectable record type icon](assets/connect-from-other-workspaces-icon.png) and the **global record type** icon ![Global record type icon](assets/global-icon.png) also display on the card. </span>-->

1. (Facultatif) Pointez sur la carte de type d’enregistrement, cliquez sur l’icône **Plus** ![Menu Plus](assets/more-menu.png) dans le coin supérieur droit, puis cliquez sur **Modifier** pour modifier les informations sur le type d’enregistrement.

   <!--replace the last point with this at the preview release of global record types:
    <span class="preview">(Optional) Hover over the record type card, click the **More** icon ![More menu](assets/more-menu.png) in the upper-right corner, then click **Edit** or **Settings** to modify information about the record type. </span>
    >[!TIP]
    >
    ><span class="preview">You can access the **Edit** and **Settings** options from the **More** menu of a record type in the record type page.</span>
    -->

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

<!--

<div class="preview">

## Create record types by adding existing ones from another workspace 

You can add record types to a workspace by adding existing ones from another workspace. You can only add record types that have been configured as global record types. 

For information, see [Add existing record types from another workspace](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md).

</div>

-->