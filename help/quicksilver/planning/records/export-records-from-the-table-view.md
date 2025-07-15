---
title: Exporter des enregistrements à partir de la vue Tableau
description: Vous pouvez exporter des enregistrements et leurs informations de la vue Tableau vers un fichier CSV ou Excel.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 8f4c1be156094d18df4bc3628d4f1fca90372119
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 12%

---


# Exporter les enregistrements de la vue Tableau

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Vous pouvez exporter des enregistrements et leurs informations de la vue Tableau vers un fichier Excel ou CSV dans Adobe Workfront Planning.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès.

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
   <td>   <p>Gérer les autorisations pour une vue</p>  
   <p>Autorisations d'affichage sur une vue pour modifier temporairement les paramètres d'affichage, la dupliquer ou l'exporter.</p> </td> 
  </tr> 
</tbody> 
</table>

* Pour plus d’informations sur les exigences d’accès à Workfront, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Exporter les enregistrements de la vue Tableau

Tenez compte des points suivants lors de l’exportation de la vue Tableau :

* Les informations exportées vers un fichier Excel conservent les filtres, les regroupements et les tris appliqués à la vue Tableau dans Workfront Planning. Les regroupements ne sont pas visibles dans le fichier CSV.

* Les miniatures et les couleurs de ligne personnalisées ne sont pas prises en charge dans les fichiers exportés.

* Seuls les champs rendus visibles dans l’interface de Workfront sont exportés. Les champs masqués ne sont pas exportés.

Pour exporter des informations à partir de la vue Table ou d&#39;un type d&#39;enregistrement :

1. Accédez à une page de type enregistrement et cliquez sur un onglet de vue Tableau.
1. Utilisez l’une des méthodes suivantes :

   * Pointez sur le nom de l’onglet d’affichage du tableau, puis cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) à droite du nom de l’affichage, puis cliquez sur **Exporter**.

   ![Menu Plus sur une vue](assets/view-more-menu-with-duplicate-option.png)

   * Cliquez sur **Partager** > **Exporter la vue actuelle**. Cette option n’est disponible que lorsque vous affichez la vue Tableau.

   ![Bouton Partager avec type d’enregistrement et options de partage d’affichage](assets/share-button-with-record-type-and-view-sharing-options.png)

1. Sélectionnez l’un des formats suivants :

   * **Excel**
   * **CSV**

   >[!IMPORTANT]
   >
   >Vous ne pouvez pas exporter des informations de la vue Tableau lorsque vous affichez une vue différente à l’écran. Vous devez afficher la vue du tableau que vous souhaitez exporter afin d’accéder à l’option Exporter du menu Plus .

   Le fichier est téléchargé sur votre ordinateur.

1. (Facultatif) Accédez au dossier des téléchargements sur votre ordinateur et recherchez le fichier téléchargé.

   Le nom du fichier exporté suit le format suivant :

   `Name of the view - name of the record type`

   Par exemple, une vue Tableau pour le type d’enregistrement Campagnes génère un fichier nommé `Table view - Campaigns`.

   Le fichier affiche les informations suivantes :

   * Les en-têtes des colonnes sont surlignés en noir dans le fichier Excel
   * Tous les champs visibles dans l’interface de Workfront, triés et filtrés selon les mêmes critères
   * Les regroupements sont conservés dans le fichier Excel

   Vous pouvez désormais partager les fichiers exportés avec d’autres personnes ou les joindre à une communication.

</div>
