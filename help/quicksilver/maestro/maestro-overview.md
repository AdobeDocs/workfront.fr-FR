---
title: Présentation d’Adobe Maestro
description: Adobe Maestro est une nouvelle offre d’Adobe Workfront. Vous pouvez créer des espaces de travail entièrement personnalisables afin de définir des workflows qui répondent aux besoins de chaque entité organisationnelle de votre entreprise.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: b1d6e0b3-e6d4-46d1-a6a2-4b8b73f7d3f7
source-git-commit: d3c22c84a9b246d1a45853c5d2825241f58bebe9
workflow-type: tm+mt
source-wordcount: '1854'
ht-degree: 1%

---

# Présentation d’Adobe Maestro

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

<!--see the separate article I wrote to have the PMs vet it for this: https://adobe-my.sharepoint.com/personal/alinaw_adobe_com/_layouts/15/doc.aspx?sourcedoc={79f94807-3d73-4015-afc0-5c016fc63cfc}&action=edit-->

<!--all the links are hidden for now, so I can share this with customer zero. Activate the links before making this public. -->

<!-- remove the references to closed beta from the entire article-->

<!--update the video in the IMPORTANT below, when we have something better, especially after Open Beta - remove it-->

>[!IMPORTANT]
>
>Les informations de cet article se rapportent à Adobe Maestro, une nouvelle offre d’Adobe Workfront.
>
>Actuellement, Adobe Maestro fait partie d’un programme bêta ouvert à un nombre limité de clients. Vous devez être un client Workfront pour utiliser les fonctionnalités de Maestro.
>
>Pour plus d’informations sur l’inscription au programme bêta de Maestro, contactez le représentant de votre compte.
>[Visionner une démonstration vidéo de Adobe Maestro](https://video.tv.adobe.com/v/3424253/){target=_blank}

## Présentation d’Adobe Maestro

Adobe Maestro est une nouvelle offre d’Adobe Workfront. L’objectif de Maestro est de déverrouiller une visibilité complète sur les détails opérationnels d’une organisation et de répondre aux questions commerciales essentielles à chaque étape du cycle de vie de la gestion du travail.

Les équipes et le leadership doivent avoir des réponses claires aux questions suivantes :

* Combien de campagnes sommes-nous en cours dans la zone EMEA pour le quatrième trimestre ?
* Existe-t-il des chevauchements d’audiences entre les campagnes simultanées ?
* Dans quelle mesure les programmes de sensibilisation fonctionnent-ils en ce moment ?
* À quoi ressemblent les ressources pour une campagne spécifique ? Lequel d&#39;entre eux doit encore être approuvé ?

Pour répondre à ces questions, le leadership a besoin d&#39;une solution qui puisse fournir une vision holistique de chaque étape du travail, de la planification à l&#39;exécution, de la livraison à la mesure des résultats. Actuellement, les entreprises disposent d’outils qui peuvent couvrir certaines parties du processus, mais beaucoup n’ont pas de bonnes connexions avec toutes les phases du travail et ne peuvent pas fournir de résultats fiables.

Voici quelques-unes des principales fonctionnalités de Maestro :

* Résolvez le problème de la gestion du travail à toutes les étapes et pour toutes les parties prenantes qui participent au processus de travail.
* Personnalisez entièrement vos workflows, depuis le choix des types d’objets (ou des types d’enregistrement) utilisés par votre entreprise jusqu’à la configuration de la liaison entre ces objets.
* Liez-les aux types d’objets d’autres systèmes, créant ainsi une structure cohérente pour tous vos processus.

## Accès requis pour utiliser Maestro pendant le programme bêta fermé

>[!IMPORTANT]
>
>Actuellement, aucun niveau d’accès ou autorisation n’est associé aux utilisateurs ou aux informations dans Maestro. Tous les utilisateurs peuvent afficher, modifier et supprimer toutes les informations ajoutées à Maestro par un autre utilisateur.

Pour plus d’informations sur l’accès requis pour utiliser Maestro, voir [Présentation de l’accès à Adobe Maestro](../maestro/access/access-overview.md).

<!-- hidden the table after I moved the content to the Access overview article: 

You must have the following access to use Adobe Maestro: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Adobe product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the Adobe Maestro closed beta program. Contact your account representative to inquire about this new offering. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader">Access level</td>
   <td> <p>Any</p>  
</td>
  </tr>

<tr>
   <td role="rowheader">Layout template</td>
   <td> <p>Your system administrator must add the Maestro area in your layout template. For information, see <a href="../maestro/access/grant-access.md">Grant access to Adobe Maestro</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

************* Activate note when going to GA: 

>[!NOTE]
>
>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). 
-->

## Terminologie maestro

Bien que Maestro fasse partie de Workfront, il s’accompagne de concepts et de terminologie propriétaires. Assurez-vous de connaître les concepts de Maestro avant de commencer à configurer Maestro pour votre entreprise.

Le framework de Maestro est entièrement personnalisable. Vous pouvez créer tous les types d’enregistrement, leurs attributs et tous les champs qui leur sont associés en fonction des besoins exacts de votre entreprise.

Voici les principaux objets et concepts de Maestro :

* **Workspace**: collection de types d’enregistrements et de taxonomies qui définissent le cycle de vie opérationnel d’une certaine organisation. Un espace de travail est la structure de travail d’une entité organisationnelle.

  Une instance Workfront peut contenir, au maximum, 1 000 espaces de travail.

  ![](assets/marketing-workspace-with-record-type-taxonomies-opening-page.png)

  Pour plus d’informations, voir [Créer des espaces de travail](../maestro/architecture/create-workspaces.md).

* **Type d’enregistrement**: type d’objet principal Maestro.

  Contrairement à Workfront où les types d’objets sont prédéfinis, vous pouvez créer vos propres types d’objets dans Maestro.

  Par exemple, dans Workfront, les types d’objets Programme, Portfolio, Projet, Tâche ou Problème sont déjà créés.

  Dans Maestro, vous pouvez créer tous les types d’enregistrement qui correspondent aux workflows de votre entreprise. Vous pouvez ensuite définir la manière dont les types d’enregistrement sont associés les uns aux autres ou les dépendances des formulaires.

  Pour plus d’informations, voir [Présentation des types d&#39;enregistrements opérationnels et des taxonomies](../maestro/architecture/overview-of-record-types-and-taxonomies.md).

  Maestro propose les types d’enregistrement suivants :

   * **Type d’enregistrement opérationnel**: type d’enregistrement qui représente les plans stratégiques, les initiatives ou le travail exécuté.

     ![](assets/operational-record-type-blank.png)

     Par exemple, Campaign, Activity, Program peuvent être des types d’enregistrements opérationnels.

     Pour plus d’informations, voir [Création de types d’enregistrement](../maestro/architecture/create-record-types.md).

   * **Taxonomie**: type d’enregistrement qui capture les attributs d’un type d’enregistrement opérationnel.

     ![](assets/taxonomy-record-type-blank.png)

     Bien que la création de taxonomies soit identique à la création de types d&#39;enregistrements opérationnels, Maestro fait la distinction entre un type d&#39;enregistrement opérationnel et un type d&#39;enregistrement de taxonomie. L&#39;objectif des taxonomies est d&#39;améliorer les types de dossiers opérationnels. <!--this is no longer true, but might be later?!: A taxonomy is a record without dates, like a static list of attributes.-->

     Par exemple, Audience, Région ou Adresse peuvent être des types d’enregistrement de type taxonomie.

     Pour plus d’informations, voir [Création de types d’enregistrement de taxonomie](../maestro/architecture/create-a-taxonomy.md).

* **Enregistrement**: instance d’un type d’enregistrement Maestro. Un enregistrement peut faire référence à un type d’enregistrement opérationnel ou à une taxonomie.

  ![](assets/records-highlighted-in-campaign-record-type-list.png)
  ![](assets/records-highlighted-in-region-taxonomy-type-list.png)

  Après avoir ajouté un type d’enregistrement à un espace de travail, vous pouvez commencer à ajouter des enregistrements de ce type sur la page du type d’enregistrement.

  Par exemple, &quot;Campagne&quot; peut être un type d’enregistrement opérationnel et &quot;Campagne d’été pour la région EMEA&quot; un enregistrement du type d’enregistrement Campaign.

  Ou

  &quot;Région&quot; est un type d’enregistrement de type taxonomie, tandis que &quot;Amériques-Amérique latine&quot; ou &quot;EMEA - Europe centrale&quot; sont des enregistrements de taxonomie.

  Pour plus d’informations, voir [Créer des enregistrements](../maestro/records/create-records.md).

* **Modèle Workspace**: vous pouvez créer un espace de travail à l’aide de modèles prédéfinis. Vous pouvez utiliser les types d’enregistrement, taxonomies et champs prédéfinis fournis dans un modèle, ou vous pouvez ajouter les vôtres.

  ![](assets/workspaces-page-with-templates-thumbnails.png)

  Maestro est fourni avec un modèle d’espace de travail Ventes, Marketing et Gestion des produits .

  Pour plus d’informations, voir [Créer des espaces de travail](../maestro/architecture/create-workspaces.md).

* **Champs**: les champs sont des attributs que vous pouvez ajouter aux types d’enregistrements opérationnels ou de taxonomie qui contiennent des informations sur le type d’enregistrement. <!--check the shot below, "Connection" needs to be in lowercase-->

  ![](assets/drop-down-list-of-record-fields.png)

  Observations relatives aux champs Maestro :

   * Les champs que vous ajoutez pour un type d’enregistrement deviennent automatiquement associés à tous les enregistrements de ce type et peuvent être utilisés pour capturer des données sur ces enregistrements.

   * Les champs s’affichent sous forme de colonnes dans la vue Tableau appliquée à une page de type enregistrement. Elles s’affichent également dans la page Détails de l’enregistrement.

   * Les champs sont propres à un type d’enregistrement et ne sont pas transférés d’un type d’enregistrement à un autre.

   * Les champs Maestro sont entièrement personnalisables et ne sont accessibles que dans Maestro. Vous ne pouvez pas accéder aux champs Maestro à partir de Workfront.

  Pour plus d’informations, voir [Créer des champs](../maestro/fields/create-fields.md)

  Un nouveau type d&#39;enregistrement opérationnel est associé par défaut aux champs prédéfinis suivants :

   * Nom
   * Description
   * Date de début
   * Date de fin
   * Statut

  Par défaut, un nouveau type d’enregistrement de taxonomie est associé à un champ Nom .

  Vous pouvez créer des champs personnalisés des types suivants :

   * Texte à une ligne
   * Paragraphe
   * Sélection multiple
   * Sélection unique
   * Date
   * Nombre
   * Pourcentage
   * Devise
   * Case à cocher
   * Personnes
   * Créé par
   * Date de création
   * Dernière modification par
   * Date de dernière modification

* **Types d’enregistrement liés**, **Enregistrements liés**, et **Champs d’enregistrement liés**: vous pouvez créer une connexion entre les entités suivantes :

   * Deux types d’enregistrement Maestro
   * Un type d’enregistrement Maestro et un type d’objet de projet, de programme, de portefeuille, d’entreprise ou de groupe Workfront.

  ![](assets/new-connection-tab-with-workfront-option.png)

  Après avoir établi une connexion entre les types d’enregistrements, vous pouvez connecter les enregistrements individuels de ces types les uns aux autres. La connexion entre les enregistrements s&#39;affiche sous la forme d&#39;un champ d&#39;enregistrement lié.

* **Champs liés** (ou champs de recherche) : après avoir établi la connexion entre deux types d’enregistrements et lier des enregistrements individuels, vous pouvez référencer les champs des enregistrements liés sur l’enregistrement à partir duquel vous vous connectez.

  ![](assets/add-lookup-fields-modal.png)

  Pour plus d’informations sur la liaison de types d’enregistrements, d’enregistrements et la création de champs liés, consultez les articles suivants :

   * [Connexion des types d’enregistrement](../maestro/architecture/connect-record-types.md)
   * [Connexion d’enregistrements](../maestro/records/connect-records.md)

<!--not yet:* Fields are reusable across Record Types.  -->

* **Vues**: les enregistrements s’affichent sous leur page de type d’enregistrement respectif dans différents types de vues.

  ![](assets/view-types-drop-down-from-record-type-list.png)

  Les vues contiennent des paramètres personnalisés d&#39;un type de vue spécifique, tels que la liste des champs (colonnes), une liste d&#39;enregistrements (lignes), leur ordre (tri), un filtre appliqué ou applicable et un regroupement.

  Voici les types de vue que vous pouvez appliquer à la page de type enregistrement :

   * **Vue Tableau**: affiche les enregistrements et leurs champs au format d’un tableau. Les lignes du tableau sont les enregistrements individuels et les colonnes sont les champs d’enregistrement. Il s’agit de la vue par défaut.

     ![](assets/table-view-example.png)

   * **Mode Chronologie**: affiche les enregistrements comportant au moins deux champs Date dans une chronologie chronologique.

     ![](assets/grouping-applied-in-timeline-view.png)

  Pour plus d’informations, voir [Gestion des vues d’enregistrement](../maestro/views/manage-record-views.md).


## Limites des objets Maestro

Le tableau suivant indique les limites du nombre d’objets que vous pouvez créer dans Maestro. Les limites peuvent changer au fur et à mesure que nous entrons dans les phases suivantes du développement de Maestro.

| Objet Maestro | Limite |
|-------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------:|
| Nombre d’espaces de travail pour une instance Workfront | 1,000 |
| Nombre de types d’enregistrement pour un espace de travail | 1 000 (y compris les taxonomies de l’espace de travail ou les objets que vous importez à partir d’applications tierces) |
| Nombre d&#39;enregistrements pour un type d&#39;enregistrement | 10,000 |
| Nombre de champs pour un type d’enregistrement ou une taxonomie | 500 |
| Nombre de caractères d’un champ de texte | 1 000 caractères |
| Taille de fichier que vous pouvez coller dans un tableau de type enregistrement | 1MB |
| Taille de fichier que vous pouvez importer via l’API pour un tableau de type enregistrement | 1.5MB |
| Taux auquel les demandes d’API peuvent être effectuées | 200 demandes par minute |
| Taille du fichier CSV d’Excel que vous pouvez importer dans un tableau | 5MB |

## Activation de Maestro pour les utilisateurs de votre instance Workfront

Votre entreprise doit s’inscrire au programme bêta fermé Adobe Maestro avant de pouvoir accéder à Maestro. Contactez votre gestionnaire de compte pour en savoir plus sur l’inscription au programme bêta.

Pour plus d’informations sur l’octroi de l’accès à et l’autorisation d’autres utilisateurs à l’aide de Maestro, voir [Accorder l’accès à Adobe Maestro](../maestro/access/grant-access.md).

<!--hidden this after moved it to a separate article

After your organization has been enrolled in the Maestro beta program, you can add the Maestro area for other users by using a layout template. 

To share the Maestro area using a layout template: 

1. Log in to Workfront as a system administrator.  

1. Add the Maestro icon to the Main Menu using a Layout Template. For information, see [Customize the Main Menu using a layout template](../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md). 

1. Assign the  layout template to the users that you want to have access to Maestro.For information, see [Assign users to a layout template](../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

    All users who can access Maestro in their Main Menu can start creating workspaces, records types, records, and fields.  
  -->


## Localisation de Maestro

Assurez-vous que votre entreprise a reçu l’accès à Maestro et que votre administrateur système ou groupe a ajouté la zone Maestro à votre menu principal.

Pour localiser Maestro :

1. Connectez-vous à Adobe Workfront.

1. Cliquez sur le bouton **Menu Principal** ![](assets/main-menu-workfront.png) dans le coin supérieur droit, ou cliquez sur l’icône **Menu Principal** ![](assets/main-menu-shell.png) dans le coin supérieur gauche, s’il est disponible.

1. Cliquez sur **Maestro** ![](assets/maestro-icon.png).

   La zone Espaces de travail Maestro s’ouvre.

1. (Facultatif et recommandé) Passez à certaines des actions suivantes pour créer votre structure de travail dans Maestro :

   1. Créez un espace de travail entièrement ou à l’aide d’un modèle.

   1. Ajoutez des types d’enregistrement au nouvel espace de travail.

   1. Ajoutez des taxonomies aux nouveaux espaces de travail.

   1. Cliquez sur le nom d’un type d’enregistrement pour ouvrir la page de l’enregistrement. Par défaut, la page d’enregistrement s’ouvre dans la vue Tableau.

   1. Personnalisez la vue Tableau en effectuant l’une des opérations suivantes :

      * Ajoutez d’autres champs au type d’enregistrement en cliquant sur le bouton **+** dans le coin supérieur droit. Les colonnes de la vue sont des champs associés au type d&#39;enregistrement.
      * Ajoutez des enregistrements en cliquant sur le bouton **+** dans le coin inférieur gauche. Les lignes de la vue sont des enregistrements uniques du type d’enregistrement sélectionné.
      * Cliquez sur **Filtres** pour filtrer les informations affichées sur la page de type enregistrement.

   1. Cliquez sur le nom d’un enregistrement pour afficher plus d’informations dans la page Détails de l’enregistrement.

   1. Création d’une vue de chronologie à partir de **Affichage** menu déroulant dans le coin supérieur droit de la page de type enregistrement.

   1. Personnalisez la vue de la chronologie en mettant à jour les filtres, les groupes ou les paramètres.

## Fonctionnalités actuellement disponibles dans Maestro

Le tableau suivant illustre les principales fonctionnalités qui seront disponibles dans Maestro, ainsi qu’une chronologie de leur disponibilité. La liste ne contient pas toutes les fonctionnalités.

| Fonctionnalité | Disponible maintenant | Disponible bientôt | En recherche |
|----------------------------------------------------|:-----------------------------:|:--------------------------------:|:----------------:|
| Créer des espaces de travail | ✓ |                                  |                  |
| Création de types d’enregistrements opérationnels | ✓ |                                  |                  |
| Création de taxonomies | ✓ |                                  |                  |
| Créer des enregistrements et des taxonomies individuels nommés | ✓ |                                  |                  |
| Créer des champs personnalisés d’enregistrement | ✓ |                                  |                  |
| Importation de types d’enregistrement et de champs à l’aide d’un fichier Excel ou CSV | ✓ |                                  |                  |
| Enregistrement de lien | ✓ |                                  |                  |
| Affichage des enregistrements dans une table | ✓ |                                  |                  |
| Affichage des enregistrements dans une chronologie | ✓ |                                  |                  |
| Filtrage des enregistrements | ✓ |                                  |                  |
| Regroupement des enregistrements dans la vue de chronologie | ✓ |                                  |                  |
| Regroupement des enregistrements dans la vue de tableau | ✓ |                                 |                  |
| Tri des enregistrements dans la vue de tableau | ✓ |                                 |                  |
| Tri des enregistrements en mode Chronologie |                               | ✓ |                  |
| Trier les groupements dans la vue Tableau |                               | ✓ |                  |
| Tri des regroupements dans la vue de chronologie |                               | ✓ |                  |
| Connexion des espaces de travail |                               | ✓ |                  |
| Connexion des enregistrements et des taxonomies Maestro | ✓ |
| Recherche d’enregistrements dans la vue de tableau | ✓ |   |
| Connecter des enregistrements Maestro à des projets, programmes, portfolios, entreprises et groupes Workfront | ✓ |                                 |                  |
| Page Détails de l’enregistrement | ✓ |                                  |                  |
| Mettre à jour la mise en page de la page Détails de l’enregistrement |                               | ✓ |                  |
| Autorisations Workspace | | ✓ |  |
| Soumettre des demandes |                               |                                  | ✓ |
| Brève présentation créative |                               |                                  | ✓ |
| Personnalisation de la couleur et de l’icône d’un enregistrement | ✓ |                                  |                 |
<!--
Add another row for Rich text formatting:


|     Rich Text formatting for Paragraph fields                                 |      ✓                         |                                  |                 |
-->

## Activité de mise à jour Maestro

Nous publions régulièrement de nouvelles fonctionnalités sur Maestro. Pour obtenir une liste à jour des fonctionnalités publiées, voir [Activité de mise à jour Adobe Maestro](../maestro/release-activity.md).

<!--moved the contents of this whole section to its own article: release-activity.md, in the same folder

This section lists the features and patches that have been released after the launch of the Maestro closed beta program, on May 22, 2023. 

The features are released weekly and are listed in the order of their release, with the most recent first. Customers who are participating in the Maestro closed beta program can access all features in their Preview and Production environments. 

### Week of September 4, 2023

#### Connect Maestro records with Workfront companies and groups

Preview and production: September 5, 2023  

You can now connect a Maestro record with Workfront companies and groups. You must first create a connection between a Maestro record type and the Workfront companies and groups object types. Then, you can connect a single Maestro record of the selected record type to individual Workfront companies and groups.  

Consider the following:  

* You must create a connection between Maestro record types and Workfront companies and groups for each Workspace.  

* You cannot connect taxonomy record types with Workfront object types. 

* You can connect multiple Maestro records to the same Workfront company or group, and multiple companies or groups to the same Maestro record.  

* You cannot edit companies or groups in Maestro. All company or group changes performed in Workfront are visible in Maestro, when reviewing the Maestro linked records.  

#### URL support for single-line text fields 

Preview and production: September 7, 2023 

For better visibility when working with links in the Table view, we have added support for URLs in single-line text fields. Using URLs to other websites or external drives when updating a single-line text field, now identifies them as links and allows you to click them from the table.  

### Week of August 28, 2023

#### Field visibility menu for the Table View toolbar

Preview and production: August 31, 2023

To display the right information on a given set of records, especially if you intend to share the view with others who need to see some but not all fields of a record type, you can now select which fields (or columns) to display and which to hide in the Table view.  

You can hide or show individual fields, from each header of the field columns, or you can manage all fields of the record type from a setting in the table view toolbar.  

### Week of August 21, 2023

#### Connect Maestro records to programs and portfolios 

Preview and production: August 24, 2023

You can now connect a Maestro record with Workfront programs and portfolios. You must first create a connection between a Maestro record type and a program or portfolio which creates a connected field. Then, you can connect any Maestro records from all other record types within the same workspace to specific programs and portfolios which will create a read-only Workfront Program or Workfront Portfolio record type in the same workspace. Consider the following:

* Workfront connector record types are unique for each workspace. 
* You can connect multiple Maestro records to the same Workfront program or portfolio, and multiple programs and portfolios to the same Maestro record. 
* You cannot edit programs and portfolios in Maestro. All program and portfolio changes performed in Workfront are visible in Maestro, when reviewing the linked records. 

#### New sorting functionality for the table view

Preview and production: August 24, 2023

You can now sort records in the table view of a record type page. 
The following capabilities are now available: 

* Sorting at the table-level, where you can sort by multiple fields at the same time. 
* Sorting at the column or field-level, where you can sort by an individual field at a time.

#### Improvements to the timeline view: new look-and-feel for groupings and the Compact/ Standard view switch

Preview and production: August 24, 2023

We have introduced the following improvements to the timeline view: 

* You can now display the timeline view in the following modes:

    * Standard: Displays records in separate lines.
    * Compact: Display the records whose dates don't intersect on the same line. 

* We have changed the look-and-feel of the grouping lines in the timeline view to display above the timeline of the records they contain. Prior to this improvement, the grouping lines displayed across the entire length of the timeline.

### Week of August 14, 2023

#### Reorder columns in the table view

You can now reorder columns in the Maestro table view. Consider the following when reordering columns: 

* The Name field is always the first field in the table view of a record type page 

* You cannot move the Name field to another position 

* The Name field is frozen and is not part of the horizontal scroll. 

#### Horizontal scroll for timeline view

You can now scroll horizontally in the timeline view of a record type. 

### Week of August 7, 2023

#### Import record types from an Excel file 

Preview and production: August 10, 2023

You can now import an Excel file to create record types in a workspace. The sheets of the file become the record types, and the columns of the file become their respective fields.  

#### Improved experience for connecting record types and projects 

Preview and production: August 10, 2023

We have improved the way you connect record types, including connecting to Workfront projects. As part of this improvement, we made the following changes when adding a field for a record type from the table view:  

* Removed the Relationship-type field from the "New field" tab.  

* Add a "New connection" tab where you can directly select the record or object type you want to connect to, eliminating the need for a Relationship-type field. 

### Week of July 10, 2023

#### Update the appearance of a record type

Preview and production: July 13, 2023

You can now select a custom icon for a record type, as well as a custom color for the record type icon.  

#### New Checkbox field type

Preview and production: July 13, 2023 

You can now add a Checkbox field type to Maestro record types. You can use the Checkbox field type to add a single checkbox option to a record. You can use this field to indicate a specific attribute or status for that particular record. For example, you can use it as a flag for tracking completion, approval, or any other binary attribute for each record.  

### Week of June 26, 2023

#### Quick activation of the contextual menu in a table

Preview and production: June 28, 2023
 
We have enabled the ability to activate the contextual menu by right-clicking anywhere in a record row, when viewing the records in the table view or a record type. You can now quickly view, delete, or copy a link to the record's Details page when you access the contextual menu from anywhere in the table view of a record type. Prior to this enhancement, the contextual menu was accessible only from the More menu in the Name column of a record.  

### Week of June 19, 2023

#### Record field names are unique

We have introduced a requirement now that the field names of a Maestro record type should have unique names. Fields that belong to different record types do not have to have unique names.  

### Week of June 5, 2023

#### Connect Maestro records with Workfront projects

Preview and production: June 5, 2023

You can now connect a Maestro record with Workfront projects. You must first create a connector Maestro record type to establish the connection between Maestro records and Workfront projects. Then, you can connect any Maestro records from all other record types to the connector record using the Relationship field. Consider the following:

* You must have a connector record type for Workfront for each Workspace. 
* You can connect multiple Maestro records to the same Workfront project, and multiple projects to the same Maestro record. 
* You cannot edit projects in Maestro. All project changes performed in Workfront are visible in Maestro, when reviewing the linked records. 

### Week of May 29, 2023

#### Two-date requirement for creating a Timeline view

Preview and production: May 31, 2023  

You must have at least two date fields associated with a record type in order to create a Timeline view. 
-->
