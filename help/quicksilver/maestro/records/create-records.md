---
title: Créer des enregistrements
description: Dans Adobe Maestro, un enregistrement est une instance d’un type d’enregistrement. Vous devez créer des types d’enregistrement avant de pouvoir créer des enregistrements individuels.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: c7de4b1f-674b-424b-af64-a6df62fb738f
source-git-commit: 5f3d5c93c2fc721dda2dd04adac22190ef6a3f29
workflow-type: tm+mt
source-wordcount: '1091'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Créer des enregistrements

>[!IMPORTANT]
>
>Les informations de cet article se rapportent à Adobe Maestro, une nouvelle offre d’Adobe Workfront.
>
>Actuellement, Adobe Maestro fait partie d’un programme bêta ouvert à un nombre limité de clients. Vous devez être un client Workfront pour utiliser les fonctionnalités de Maestro.
>
>Pour plus d’informations sur l’inscription au programme bêta de Maestro, contactez le représentant de votre compte.
>
>Pour plus d’informations, voir [Présentation d’Adobe Maestro](../maestro-overview.md).

Dans Adobe Maestro, un enregistrement est une instance d’un type d’enregistrement.

Vous pouvez avoir les types d’enregistrements suivants :

* **Enregistrements opérationnels**: ils représentent des objets liés au travail. Par exemple, pour un enregistrement opérationnel appelé &quot;Campagne&quot;, vous pouvez avoir nommé des enregistrements tels que &quot;Newsletter mensuelle&quot; ou &quot;Solde d’été&quot;.
* **Enregistrements de taxonomie**: ils représentent des attributs qui peuvent être associés à des enregistrements opérationnels. Par exemple, pour un type d’enregistrement de taxonomie appelé &quot;Canal&quot;, vous pouvez avoir nommé des taxonomies telles que &quot;Email&quot;, &quot;Social Media&quot; ou &quot;Publicité&quot;.

La création d&#39;enregistrements opérationnels est identique à la création d&#39;enregistrements de taxonomie ou taxonomies.

Vous pouvez créer des enregistrements dans Maestro en effectuant l’une des opérations suivantes :

* Créez-les manuellement pour les types d’enregistrement Maestro
* Connectez-les aux enregistrements Maestro à partir d’applications tierces.
* Créez des enregistrements en copiant et en collant des informations à partir d’une liste externe.

Cet article décrit comment créer des enregistrements Maestro. Pour plus d’informations sur la gestion des enregistrements dans les vues de tableau ou de chronologie, consultez les articles suivants :

* [Gestion de la vue de tableau](/help/quicksilver/maestro/views/manage-the-table-view.md)
* [Gestion du mode Chronologie](/help/quicksilver/maestro/views/manage-the-timeline-view.md)

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

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
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Accord Adobe Workfront</p></td>
   <td>
<p>Votre entreprise doit être inscrite au programme bêta fermé Adobe Maestro. Contactez le représentant de votre compte pour en savoir plus sur cette nouvelle offre. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Formule Adobe Workfront</p></td>
   <td>
<p>Quelconque</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licence Adobe Workfront</p></td>
   <td>
   <p>Quelconque</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Paramétrages du niveau d'accès</p></td>
   <td> <p>Il n’existe aucun contrôle d’accès pour Maestro </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Autorisations</p></td>
   <td> <p>Attribution ou autorisations supérieures à un espace de travail</a> </p>  
   <p>Les administrateurs système disposent d’autorisations pour tous les espaces de travail, y compris ceux qu’ils n’ont pas créés.</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Modèle de mise en page</p></td>
   <td> <p>L’administrateur de Workfront ou de groupe doit ajouter la zone Maestro à votre modèle de mise en page. Pour plus d’informations, voir <a href="../access/access-overview.md">Présentation de l’accès</a>. </p>  
</td>
  </tr>

</tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Créer des enregistrements en les ajoutant manuellement à un type d’enregistrement <!--in a record type table (I don't think you can create them elsewhere right now)-->

Vous pouvez créer des enregistrements dans la vue table d’une page de type enregistrement.

{#step1-to-maestro}

L’espace de travail que vous avez consulté pour la dernière fois s’ouvre par défaut. Pour plus d’informations sur la création d’espaces de travail, voir [Créer des espaces de travail](../architecture/create-workspaces.md).
1. Cliquez sur une carte de type enregistrement. Pour plus d’informations sur la création d’un type d’enregistrement, voir [Création de types d’enregistrement](../architecture/create-record-types.md).

   La page de type enregistrement s’ouvre dans la vue à laquelle vous avez accédé la dernière fois. Par défaut, une page de type enregistrement s’ouvre dans la vue de tableau.
Tous les enregistrements du type sélectionné s&#39;affichent en mode Tableau.

1. (Conditionnel) Si la page de type enregistrement ne s’ouvre pas dans la vue de tableau, cliquez sur le bouton **Affichage** , puis sélectionnez une **Vue Tableau** ![](assets/table-view-icon.png) ou cliquez sur **Créer une vue > Tableau** pour créer une vue de tableau.

1. Pour ajouter de nouveaux enregistrements, cliquez sur **Nouveau &lt; Nom du type d’enregistrement >** dans la dernière ligne du tableau ;

   Ou

   Cliquez sur **Maj + Entrée** sur votre clavier à partir de n’importe quelle colonne ou ligne du tableau. Ceci ajoute une ligne vide.

   ![](assets/adding-a-new-campaign-in-table-row.png)

1. Commencez à saisir des informations sur le nouvel enregistrement dans la nouvelle ligne.

   >[!NOTE]
   >
   >  * Il n’existe aucun champ obligatoire pour les enregistrements. Nous vous recommandons toutefois d’ajouter un Nom pour l’enregistrement, car il est utile d’identifier les enregistrements lors de la liaison d’enregistrements.
   >
   >  * Les champs qui font référence à d’autres types d’enregistrement ou à des champs calculés sont en lecture seule.

1. Continuez à ajouter des informations sur chaque ligne, puis cliquez sur **Entrée** sur votre clavier pour enregistrer vos modifications.

1. (Facultatif) Utilisez les raccourcis clavier suivants pour annuler ou rétablir l’ajout de nouveaux enregistrements :

   * Ctrl + Z (⌘ + Z pour Mac) pour annuler une modification.
   * Ctrl + Maj + Z (⌘ + Maj + Z pour Mac) pour rétablir la modification

## Créer des enregistrements en les connectant depuis une autre application

Vous pouvez importer des enregistrements d’autres applications en les liant à des enregistrements liés à Maestro. Cela crée un type d’enregistrement Maestro pour l’objet tiers connecté à l’application. Les enregistrements que vous connectez aux enregistrements Maestro d’origine s’affichent dans la vue de tableau de type d’enregistrement Maestro d’objet connecté tiers.

1. Créez un type d’enregistrement Maestro, comme décrit dans la section [Création de types d’enregistrement](../architecture/create-record-types.md).

1. Créez des enregistrements Maestro pour le type d’enregistrement que vous avez créé à l’étape précédente. Pour plus d’informations, voir la section [Créer des enregistrements en les ajoutant manuellement à un type d’enregistrement](#create-records-by-manually-adding-them-to-a-record-type) dans cet article.

1. Créez une connexion à un type d’objet à partir d’une application tierce pour le type d’enregistrement Maestro que vous avez créé. Pour plus d’informations, voir [Connexion des types d’enregistrement](../architecture/connect-record-types.md).

1. Ajoutez des enregistrements de l’application tierce aux enregistrements Maestro que vous avez créés ci-dessus à l’aide du champ d’enregistrement lié que vous avez créé à l’étape précédente. Pour plus d’informations, voir [Connexion d’enregistrements](../records/connect-records.md).

   Les éléments suivants sont créés dans Maestro :

   * Type d’enregistrement Maestro en lecture seule qui fait référence au type d’enregistrement tiers auquel vous avez lié dans le champ d’enregistrement connecté.

     Par exemple, si vous connectez un type d’enregistrement Maestro aux projets Workfront, un type d’enregistrement en lecture seule nommé &quot;Projets Workfront&quot; est créé dans le même espace de travail.
   * Enregistrements en lecture seule sur la page de type d’enregistrement tiers. Les enregistrements importés depuis l&#39;application tierce restent en lecture seule et ne peuvent être mis à jour que dans leur application d&#39;origine.

## Créer des enregistrements en copiant et collant des informations à partir d’une liste externe

1. Dans Maestro, commencez à créer des enregistrements dans la vue Tableau, comme décrit dans la section . [Créer des enregistrements en les ajoutant manuellement à un type d’enregistrement](#create-records-by-manually-adding-them-to-a-record-type) dans cet article.

   Assurez-vous que la vue Tableau Maestro contient les colonnes (ou les champs) que vous souhaitez renseigner avec les nouvelles informations d’enregistrement.

1. Cliquez sur **Nouveau &lt; Nom du type d’enregistrement >** dans la dernière ligne du tableau pour ajouter autant de nouvelles lignes que vous souhaitez que vos nouveaux enregistrements soient.

   Par exemple, ajoutez 10 lignes à la vue de tableau si vous souhaitez coller les informations relatives à 10 nouveaux enregistrements d’une autre application.

1. Dans une autre application, créez une liste d&#39;enregistrements à importer dans Maestro.

   Vous pouvez par exemple utiliser une feuille de calcul Excel pour créer votre liste.

   La liste doit contenir des informations sous forme de tableau.

   >[!TIP]
   >
   > Les colonnes de la liste doivent contenir des informations sur les champs existants que vous avez dans Maestro.
   >
   > Assurez-vous que les champs de votre choix ont déjà été créés dans Maestro et que les informations de votre feuille s’affichent au format correct qui correspond à celui de chaque champ de Maestro.

1. Dans l’application tierce, sélectionnez plusieurs lignes et colonnes, puis collez les informations dans la vue table de type enregistrement, en commençant par le premier nouvel enregistrement.

   Les informations suivantes sont importées dans Maestro :

   * Les lignes contiennent les nouveaux enregistrements
   * Les colonnes renseignent les informations des champs des enregistrements.
