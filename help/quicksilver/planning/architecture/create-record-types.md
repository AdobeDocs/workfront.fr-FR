---
title: Création de types d’enregistrement
description: Les types d’enregistrement sont les types d’objets d’Adobe Workfront Planning. Dans la planification Workfront, vous pouvez créer des types d’enregistrement personnalisés qui illustrent les tâches nécessaires au cycle de vie de votre entreprise.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: ed1c4954-b338-4865-a7a9-5ba0192e7b37
source-git-commit: 160bcc8796666c9615ebe8ead18813b96be26a71
workflow-type: tm+mt
source-wordcount: '1258'
ht-degree: 3%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->
<!--this is linked to the UI in an empty workspace screen-->

# Création de types d’enregistrement

{{planning-important-intro}}

Les types d’enregistrement sont les types d’objets d’Adobe Workfront Planning. Dans la planification Workfront, vous pouvez créer des types d’enregistrement personnalisés qui illustrent les éléments liés au travail nécessaires dans le cycle de vie de votre entreprise.

Pour plus d’informations sur les types d’enregistrement, voir [Types d’enregistrement - Aperçu](/help/quicksilver/planning/architecture/overview-of-record-types.md).

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Produit</p> </td>
   <td> Adobe Workfront
   </td>
  </tr>  
 <td role="rowheader"><p>Accord Adobe Workfront</p></td>
   <td>
<p>Votre entreprise doit être inscrite à l’étape d’accès anticipé pour la planification Workfront </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Forfait Adobe Workfront</p></td>
   <td>
<p>N’importe quelle</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licence Adobe Workfront</p></td>
   <td>
   <p>Actuel : formule</p>
   Ou
   <p>Nouveau : Standard </p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configurations du niveau d’accès</p></td>
   <td> <p>Il n’existe aucun contrôle de niveau d’accès pour la planification Workfront</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Modèle de mise en page</p></td>
   <td> <p>L’administrateur de Workfront ou de groupe doit ajouter la zone Planning dans votre modèle de mise en page. Pour plus d’informations, voir <a href="/help/quicksilver/planning/access/access-overview.md">Présentation de l’accès</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Autorisations</p></td>
   <td> <p>Gestion des autorisations d’un espace de travail</a> </p>  
   <p>Les administrateurs système disposent d’autorisations pour tous les espaces de travail, y compris ceux qu’ils n’ont pas créés.
</td>
  </tr>
 </tbody>
</table>

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Remarques concernant la création de types d’enregistrement

* Vous pouvez créer des types d’enregistrement dans un espace de travail de la manière suivante :

   * Automatiquement :
      * Lorsque vous créez un espace de travail à l’aide d’un modèle.

        Pour plus d’informations, voir [Créer des espaces de travail](/help/quicksilver/planning/architecture/create-workspaces.md).

      * Lorsque vous les importez à l’aide d’un fichier Excel ou CSV.

        >[!IMPORTANT]
        >
        >Cette fonctionnalité est temporairement désactivée depuis le 21 mars 2024. Elle sera activée ultérieurement.

     <!--this should not ne known anymore: * When you add objects from another application to a linked record field of a record. This creates a read-only record type in Workfront Planning which is connected to object types from the original application. 
        For information about connecting record types with object types from another application, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md).
        For information about connecting objects with records, see [Connect records](/help/quicksilver/planning/records/connect-records.md). -->
   * Manuellement :

      * À partir de zéro.

        Cet article décrit comment créer des types d’enregistrement à partir de zéro.

* Vous pouvez déplacer des types d’enregistrement dans une section et d’une section d’un espace de travail à une autre. Vous ne pouvez pas déplacer des types d’enregistrement d’un espace de travail vers un autre.

## Création de types d’enregistrement à l’aide d’un modèle d’espace de travail

Vous pouvez créer automatiquement des types d’enregistrement lorsque vous créez un espace de travail à l’aide d’un modèle de planification Workfront . Chaque modèle contient des exemples de types d’enregistrement.

Lorsque vous créez un espace de travail à partir d’un modèle, les types d’enregistrement sont regroupés dans les sections suivantes :

* Types d’enregistrements opérationnels
* Taxonomies

Vous pouvez ajouter manuellement des types d’enregistrements dans les sections Types d’enregistrements opérationnels et Taxonomies .

Pour plus d’informations sur la création d’espaces de travail, voir [Créer des espaces de travail](/help/quicksilver/planning/architecture/create-workspaces.md).

Pour plus d’informations sur les types d’enregistrement inclus dans chaque modèle, voir [Liste des modèles d&#39;espace de travail](/help/quicksilver/planning/architecture/workspace-templates.md).

## Créer entièrement un type d’enregistrement

{{step1-to-planning}}

L’espace de travail du dernier accès doit s’ouvrir par défaut.

1. (Facultatif) Développez la flèche pointant vers le bas située à droite du nom d’un espace de travail existant, puis sélectionnez l’espace de travail pour lequel vous souhaitez créer des types d’enregistrement.
1. (Facultatif) Cliquez sur **Ajouter une section** pour ajouter une nouvelle section à l’espace de travail.
1. Cliquez sur **Ajouter un type d’enregistrement**.
1. (Conditionnel) Lorsque vous créez des types d’enregistrement en important un fichier Excel ou CSV, cliquez sur **A partir de zéro**. Sinon, la variable **Ajouter un type d’enregistrement** s’ouvre.

   ![](assets/add-record-type-box-with-appearance-options.png)

1. Mettez à jour les informations suivantes :

   * Remplacez &quot;Untitled record type&quot; par le nom de votre futur type d’enregistrement. <!--did they bring back the field label here and did they rename it to "Name"-->
   * **Description**: ajoutez des informations supplémentaires sur le type d’enregistrement.
   * Sélectionnez une couleur et une forme pour l’icône associée au type d’enregistrement. Procédez comme suit :
      * Sélectionnez une couleur pour identifier votre nouveau type d’enregistrement. Il s’agit de la couleur de l’icône de type d’enregistrement. L’option Gris est sélectionnée par défaut.
      * Sélectionnez une icône dans la liste ou commencez à saisir le nom d’une icône pour décrire ce qu’elle représente, puis sélectionnez-la lorsqu’elle s’affiche. Il s’agit de l’icône du type d’enregistrement. Une icône de fichier est sélectionnée par défaut.

1. Cliquez sur **Créer**.

   La carte de type enregistrement est ajoutée à la section et à l’espace de travail que vous avez sélectionné.
La description du type d’enregistrement s’affiche sur la carte.

   ![](assets/record-type-card-with-description.png)

1. (Facultatif) Passez la souris sur la carte de type d’enregistrement, puis cliquez sur le bouton **Plus** icon ![](assets/more-menu.png) dans le coin supérieur droit, puis cliquez sur **Modifier** pour modifier les informations sur le type d’enregistrement.
1. (Facultatif) Cliquez sur la carte de type enregistrement pour ouvrir la page de type enregistrement.

   ![](assets/operational-record-type-blank.png)

   La page de type enregistrement s’affiche par défaut dans la vue de tableau. Les colonnes du tableau sont des champs associés au nouveau type d’enregistrement. Chaque ligne est un enregistrement unique que vous devez ajouter.

   >[!TIP]
   >
   >    Si vous importez un type d’enregistrement à partir d’un fichier Excel ou CSV, les enregistrements sont également importés.

   Par défaut, les champs suivants s&#39;affichent dans les colonnes de vue de tableau d&#39;un type d&#39;enregistrement opérationnel :

   * Nom
   * Description
   * Date de début
   * Date de fin
   * Statut

1. (Facultatif) Mettez à jour le nom du type d’enregistrement dans l’en-tête de la page.

   Ou

   Cliquez sur le bouton **Plus** icon ![](assets/more-menu.png) à droite du nom du type d&#39;enregistrement et cliquez sur **Modifier** pour le renommer ou modifier les informations le concernant. Pour plus d’informations, voir [Modification des types d’enregistrement](/help/quicksilver/planning/architecture/edit-record-types.md).

1. (Facultatif) Cliquez sur **+ Nouvel enregistrement** pour ajouter des enregistrements du type d’enregistrement sélectionné. Pour plus d’informations, voir [Créer des enregistrements](/help/quicksilver/planning/records/create-records.md).
1. (Facultatif) Cliquez sur le **+** dans le coin supérieur droit du tableau pour ajouter d’autres champs au type d’enregistrement.

   Pour plus d’informations sur la création de champs, voir [Créer des champs](/help/quicksilver/planning/fields/create-fields.md).

1. (Facultatif) Cliquez sur la flèche pointant vers la gauche du nom du type d’enregistrement, dans l’en-tête, pour revenir à l’espace de travail sélectionné.

1. (Facultatif) Dans l’espace de travail, cliquez sur une carte de type enregistrement et maintenez-la enfoncée pour faire glisser et déposer le type d’enregistrement à un emplacement souhaité, ou pour le déplacer vers une autre section.

   Les modifications sont enregistrées automatiquement.

   Pour plus d’informations sur l’ajout d’enregistrements, la suppression ou la modification de types d’enregistrements, ou la mise à jour de la vue dans la page de type d’enregistrement, voir les articles suivants :

   * [Créer des enregistrements](/help/quicksilver/planning/records/create-records.md)
   * [Supprimer des types d’enregistrements](/help/quicksilver/planning/architecture/delete-record-types.md)
   * [Modifier des types d’enregistrements](/help/quicksilver/planning/architecture/edit-record-types.md)
   * [Gestion des vues d’enregistrement](/help/quicksilver/planning/views/manage-record-views.md)

## Création de types d’enregistrement à l’aide d’un import de fichier Excel ou CSV

>[!IMPORTANT]
>
>Cette fonctionnalité est temporairement désactivée depuis le 21 mars 2024. Elle sera activée ultérieurement.

Tenez compte des points suivants lors de l’importation de types d’enregistrement à l’aide d’un fichier Excel ou CSV :

* Chaque feuille du fichier Excel devient un type d’enregistrement.
* Les colonnes de chaque feuille deviennent les champs associés à chaque type d’enregistrement.
* Les champs sont uniques pour leurs types d’enregistrement respectifs.
* Chaque ligne de chaque feuille devient un enregistrement unique associé à son type d’enregistrement respectif.
* Chaque feuille du fichier Excel ne doit pas excéder les éléments suivants :
   * 50 000 lignes
   * 500 colonnes
* Le fichier Excel ne doit pas dépasser 5 Mo.
* Les feuilles vides ne sont pas prises en charge.

Pour importer des types d’enregistrement à l’aide d’un fichier Excel :

{{step1-to-planning}}

L’espace de travail du dernier accès doit s’ouvrir par défaut.

1. (Facultatif) Développez la flèche pointant vers le bas située à droite du nom d’un espace de travail existant, puis sélectionnez l’espace de travail pour lequel vous souhaitez créer des types d’enregistrement.
1. Cliquez sur **Ajouter un type d’enregistrement**.
1. Cliquez sur **Excel/CSV**.
1. Faites glisser et déposez un fichier Excel ou CSV précédemment enregistré sur votre ordinateur, ou cliquez sur **Sélection d’un fichier CSV ou Excel** pour en rechercher une.
1. Cliquez sur **Vérification des données**.

   La zone Aperçu et modification s’affiche avec les informations suivantes :

   * Les noms des feuilles ou des types d’enregistrements futurs s’affichent dans le panneau de gauche. Workfront Planning sélectionne par défaut une icône et une couleur pour chaque nouveau type d’enregistrement.
   * La première feuille ou le type d’enregistrement est sélectionné et les noms des champs qui lui sont associés s’affichent sous forme d’en-têtes de colonne. Le type de chaque champ est sélectionné par défaut.
   * Chaque ligne représente un nouvel enregistrement. Seuls les 10 premiers enregistrements s&#39;affichent dans la zone Prévisualisation et édition.

   ![](assets/preview-and-edit-box.png)

1. (Facultatif) Cliquez sur le nom de chaque feuille dans le panneau de gauche pour consulter les informations qu’elle contient.

   >[!NOTE]
   >
   >    Les feuilles vides ne sont pas prises en charge et sont grisées.


1. (Facultatif) Cliquez sur le **Sélectionner les feuilles à importer** et désélectionnez les feuilles que vous ne souhaitez pas importer.

   ![](assets/select-sheets-to-import-drop-down-with-unselected.png)

   Cette option vous permet de désélectionner l’affichage avec un arrière-plan gris.

1. Cliquez sur **Importer** lorsque vous êtes prêt à importer votre fichier.

   Les informations suivantes sont importées dans Workfront Planning :

   * Nouveaux types d’enregistrement
   * Nouveaux champs associés à chaque type d&#39;enregistrement
   * Nouveaux enregistrements associés à chaque type d&#39;enregistrement

   Vous pouvez commencer à gérer les champs et les enregistrements sur les pages de types d’enregistrement.

   Toute personne ayant accès à Workfront Planning peut désormais afficher et modifier les types d’enregistrements importés et leurs informations. <!--this will change with permissions-->

<!--## Connect record types with object types from another application

You can connect a record type and an object type from another application. This creates a read-only record type in Workfront Planning that corresponds to the object type in the other application. 

For example, you can create record types by connecting Workfront Planning record types with Workfront projects. As a result, the Workfront project object type is imported into Workfront Planning as a read-only record type. By default, the record type is named "Workfront Project." (********************)has this name changed? Lusine wanted to change it at some point***********)
    
You can import the following objects from the following applications: 

* From Workfront:

    * Projects
    * Portfolios
    * Programs
    * Company
    * Group

For more information, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md). 
-->