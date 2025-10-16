---
title: Créer des enregistrements en important des informations depuis un fichier CSV ou Excel
description: Les enregistrements sont des instances individuelles de types d'enregistrements, qui sont les types d'objet d'Adobe Workfront Planning. Dans Workfront Planning, vous pouvez créer des enregistrements en important des informations à partir d'un fichier CSV ou Excel.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 940945df-391c-4672-9d9d-180d5028509b
source-git-commit: 8546311acf722c0f4d47d4663b02ff701416894a
workflow-type: tm+mt
source-wordcount: '886'
ht-degree: 11%

---


# Créer des enregistrements en important des informations depuis un fichier CSV ou Excel

<span class="preview">Les informations de cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de façon générale. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Après les versions mensuelles en production, les mêmes fonctionnalités sont également disponibles dans l’environnement de production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation des versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Les enregistrements sont des instances individuelles de types d&#39;enregistrements, qui sont les types d&#39;objet d&#39;Adobe Workfront Planning. Dans Workfront Planning, vous pouvez créer des enregistrements en important des informations à partir d&#39;un fichier CSV ou Excel.

Pour plus d&#39;informations sur la création d&#39;enregistrements, voir [Créer des enregistrements](/help/quicksilver/planning/records/create-records.md).

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
   <td><p>Standard</p>
   </td> 
  </tr>

<tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td> <p>Des autorisations de niveau Contribution ou supérieur pour l’espace de travail et le type d’enregistrement où vous importez des enregistrements. </p>
   <p>L’administration système a accès à tous les espaces de travail, y compris ceux qu’elle n’a pas créés.</p>
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
   <td> Standard
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p> 
   <p>Edit access in Workfront for the object types that you want to create (projects, programs, and portfolios) as you connect them from new records  </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td> <p>Contribute or higher permissions to the workspace and record type where you want to add records. </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
   <p>Manage permissions to Workfront objects (portfolios) to add children objects (projects).</p>
   </td> 
  </tr> 
</tbody> 
</table> -->


## Remarques concernant l’importation d’enregistrements à l’aide d’un fichier Excel ou CSV

* Les en-têtes des colonnes de chaque feuille deviennent les champs associés aux enregistrements.
* Chaque ligne de chaque feuille devient un enregistrement unique associé.
* Si le fichier Excel contient plusieurs feuilles, seules les informations d&#39;une feuille que vous sélectionnez lors du processus d&#39;importation sont importées.
* Le fichier ne doit pas dépasser les valeurs suivantes :
   * 25 000 lignes
   * 500 colonnes
* La taille du fichier ne doit pas dépasser 5 Mo.
* Les feuilles vides ne sont pas prises en charge.
* Les champs des types suivants ne sont pas pris en charge et ne peuvent pas être mappés aux champs de la feuille d’importation :

   * Champs de connexion aux types d’objet Workfront et AEM Assets. Vous ne pouvez mapper que les champs de connexion aux types d&#39;enregistrements Planning.
   * Champs de recherche des enregistrements Planning connectés ou des objets Workfront et AEM Assets
   * Champs de formule
   * Date de création, Créé par
   * Date de dernière modification, Dernière modification par
   * <span class="preview">Date d’approbation, Approuvé par</span>
   * Personnes
   * Si un champ à sélection multiple ou unique est importé et qu&#39;il offre plus de choix qu&#39;un champ similaire dans Planning, les options supplémentaires sont créées lors de l&#39;importation. Seuls les utilisateurs disposant d’autorisations de niveau Gérer pour l’espace de travail peuvent importer de nouveaux choix.

## Créer des enregistrements en important un fichier CSV ou Excel

{{step1-to-planning}}

1. Cliquez sur l’espace de travail dans lequel vous souhaitez créer des enregistrements,

   Ou

   Depuis un espace de travail, développez la flèche pointant vers le bas à droite d’un nom d’espace de travail existant, recherchez un espace de travail, puis sélectionnez-le lorsqu’il s’affiche dans la liste.
1. Cliquez sur la carte du type d’enregistrement sur lequel vous souhaitez importer les enregistrements.
1. Cliquez sur **Nouvel enregistrement** dans le coin supérieur droit de l’écran.

   ![Choisir la méthode d&#39;ajout des enregistrements à trois boutons](assets/choose-way-to-add-records-three-button-box.png)
1. Cliquez sur **Télécharger à partir du fichier**, puis sur **Continuer**. <!--add screen shot when all three buttons are added - with the Submit a request button-->
1. Faites glisser un fichier Excel ou CSV préalablement enregistré sur votre ordinateur ou cliquez sur **Sélectionner un fichier CSV ou Excel** pour en rechercher un.
1. Cliquez sur **Prévisualiser et modifier**.
1. (Conditionnel) Si le fichier importé comporte plusieurs feuilles, sélectionnez le bouton radio de la feuille à importer dans la zone **Sélectionner une feuille à importer**, puis cliquez sur **Suivant**. Sinon, passez à l’étape suivante.

   ![Sélectionner une feuille pour importer des enregistrements](assets/select-a-sheet-to-import-box.png)
1. Dans la **Mapper les champs Planning à vos en-têtes de colonne** sélectionnez le **champ Planning** qui correspond le mieux aux informations de chacune des colonnes de la feuille.

   ![Mapper les champs Planning aux colonnes lors de l&#39;import d&#39;enregistrements](assets/map-planning-fields-to-columns-when-importing-records.png)

   Chaque ligne représente un nouvel enregistrement. Seuls les 10 premiers enregistrements s’affichent dans la zone Prévisualiser et modifier.

   >[!TIP]
   >
   >Tous les types de champ ne sont pas pris en charge. Pour plus d’informations, consultez la section [Considérations relatives à l’importation d’enregistrements à l’aide d’un fichier Excel ou CSV](#considerations-about-importing-records-using-an-excel-or-csv-file) dans cet article.


1. (Facultatif et conditionnel) Si vous disposez d’autorisations de niveau Gérer pour l’espace de travail, sélectionnez l’option **Créer les options manquantes** dans le coin inférieur gauche de l’écran. Lorsqu’ils sont activés, les choix manquants de champs à sélection unique et à sélection multiple sont ajoutés.

   >[!NOTE]
   >
   >Par exemple, si le type d’enregistrement sélectionné comporte un champ Statut à sélection unique avec les choix Nouveau, En cours et Fermé et qu’un champ Statut importé d’un fichier comporte également un choix Statut En attente , le choix Statut En attente est également ajouté.
   >
   >Si vous ne disposez pas des autorisations de niveau Gérer pour l&#39;espace de travail, vous pouvez importer des enregistrements, mais les choix supplémentaires ne seront pas créés. Au lieu de cela, vous recevez le message suivant dans le coin supérieur droit de la zone Mapper les champs Planning à vos en-têtes de colonne : **Les choix qui n’existent pas dans le cadre d’une connexion, les champs à sélection unique ou multiple ne seront pas ajoutés**.

1. Cliquez sur **Importer**.

   Les informations suivantes sont importées dans Workfront Planning :

   * Nouveaux enregistrements qui s’affichent au bas de la vue Tableau du type d’enregistrement sélectionné.
   * Nouvelles valeurs de champs pour les champs existants associés à chaque enregistrement.
   * Nouveaux choix d&#39;un champ à sélection multiple ou unique qui n&#39;existait pas dans Planning.  <!--when we add connected records - add those here too-->

   Vous pouvez commencer à gérer les champs et les enregistrements dans la page des types d’enregistrements.

   Toute personne ayant accès à Workfront Planning et à l’espace de travail peut désormais afficher et modifier les enregistrements importés et leurs informations.

   <!--when we add connected records and the info icon in the tool changes, also add those items to the Import step and to the NOTE above it-->
