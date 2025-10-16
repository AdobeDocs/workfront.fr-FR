---
title: Exporter des enregistrements à partir de la vue Tableau
description: Vous pouvez exporter des enregistrements et leurs informations de la vue Tableau vers un fichier CSV ou Excel.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: d8ac4d94-28b5-41d6-acb8-259696897c8a
source-git-commit: 8546311acf722c0f4d47d4663b02ff701416894a
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 3%

---

# Exporter les enregistrements de la vue Tableau

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Vous pouvez exporter des enregistrements et leurs informations de la vue Tableau vers un fichier Excel ou CSV dans Adobe Workfront Planning.

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
<ul> 
<li><p>Tout Workfront et tout package Planning</p></li>
Ou
<li><p>Tout workflow et tout package Planning</p></li></ul>
<p>Pour plus d’informations sur les composants inclus dans chaque package Workfront Planning, contactez votre représentant de compte Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront</p></td> 
   <td><p>Léger ou supérieur</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td> <p>Autorisations d’affichage ou supérieures pour un espace de travail et un type d’enregistrement</p>   
   <p>Autorisations d’affichage ou supérieures</p>

</td> 
  </tr> 
  <tr>
   <td role="rowheader"><p>Modèle de mise en page</p></td>
   <td> Les utilisateurs disposant d'une licence light ou contributor doivent se voir attribuer un modèle de mise en page incluant Planning.
   <p>Les zones Planning sont activées par défaut pour les utilisateurs standard et les administrateurs système.</p></div></li></ul>
</td>
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
   <td><p> Light or higher </p>
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
   <td>   <p>View or higher permissions to a view</p>  
   </td> 
  </tr> 
</tbody> 
</table> -->


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
