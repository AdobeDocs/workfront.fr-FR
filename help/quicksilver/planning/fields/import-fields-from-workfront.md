---
title: Importer des champs depuis Adobe Workfront
description: Dans Adobe Workfront Planning, vous pouvez créer des champs personnalisés pour chaque type d’enregistrement. Vous pouvez ensuite associer le champ à des enregistrements Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 994594f2-a888-423a-bf66-0d14baf57c55
source-git-commit: 53596271a838733b858c0b14a4e22b07a7cd20f6
workflow-type: tm+mt
source-wordcount: '606'
ht-degree: 20%

---

<!--add to TOC-->

# Importer des champs depuis Adobe Workfront

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>  -->


{{planning-important-intro}}

Vous pouvez importer des copies de champs Workfront existants. L’importation de champs depuis Workfront crée une copie de chaque champ pour un type d’enregistrement Workfront Planning.


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
<p>Tout Workfront et tout package Planning</p> <p>Tout workflow et tout package Planning</p>
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
   <td>   <p>Manage permissions to a workspace and record type </a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create.</p> </td> 
  </tr> 
</tbody> 
</table> -->


## Considérations relatives à l’importation de champs depuis Workfront

* Vous pouvez importer des champs Workfront natifs ou personnalisés dans un type d&#39;enregistrement dans Workfront Planning.
* L’importation de champs Workfront crée des copies des mêmes champs et conserve le nom du champ dans Workfront Planning. Une fois copiés dans Workfront Planning, les champs sont indépendants des champs Workfront d’origine et ne partagent pas d’informations.
<!--check this: * You do not need permissions or access to Workfront objects to be able to add their fields to Workfront Planning. -->
* Vous pouvez ajouter des champs natifs ou personnalisés à partir des objets Workfront suivants :
   * Portfolio
   * Programme
   * Projet
   * Tâche
   * Problème
   * Document
   * Entreprise
   * Groupe
   * l’utilisateur ou de l’utilisatrice
   * Fonction
   * Affectation
   * Heure
   * Enregistrement de facturation
     <!--Available only to Preview, but might not come to Prod:* Rate card - visible in Production but asking PM if it should be hidden-->
   * Frais
   * Itération
     <!--* Non-labor resource - - visible in Production but asking PM if it should be hidden-->
     <!--* Non-labour resource category - - visible in Production but asking PM if it should be hidden-->
* Il se peut que les champs Workfront ne conservent pas leur type de champ après leur importation dans Workfront Planning.

  Le tableau ci-dessous présente les types de champs Workfront et le type de champ Workfront Planning correspondant.

  | Type de champ Workfront | Type de champ Workfront Planning |
  |------------------------------------------|-------------------------------|
  | Texte d’une seule ligne au format texte | Texte à une ligne |
  | Texte d’une seule ligne au format numérique | Nombre |
  | Texte d’une seule ligne au format monétaire | Devise |
  | Paragraphe | Paragraphe |
  | Texte avec formatage | Paragraphe |
  | Liste déroulante à sélection unique | Sélection unique |
  | Menu déroulant multi-sélection | Sélection multiple |
  | Les filtres de saisie semi-automatique ne sont pas pris en charge | Personnes |
  | Calculé* | Formule |
  | Date | Date |
  | Groupe Case à cocher | Sélection multiple |
  | Bouton radio | Sélection multiple |

  *Les champs calculés seront disponibles ultérieurement.
Tous les autres types de champ Workfront ne sont pas pris en charge dans Workfront Planning.


## Importer les champs depuis Workfront

<!--the first 3 steps are the same as in Create fields-->

{{step1-to-planning}}

1. Cliquez sur l’espace de travail dont vous souhaitez créer les types d’enregistrements pour les champs.

   L’espace de travail et les types d’enregistrement s’affichent.

1. Cliquez sur la carte d’un type d’enregistrement.

   Tous les enregistrements existants associés au type d’enregistrement s’affichent dans les lignes de la vue Tableau.

   >[!TIP]
   >
   >    Certains champs peuvent être masqués. Cliquez sur **Champs** et activez le bouton (bascule) pour les champs que vous souhaitez afficher en tant que colonnes dans la vue Tableau.

1. Cliquez sur l’icône **+** dans le coin supérieur droit de la vue Tableau

   Ou

   Pointez sur l’en-tête d’une colonne, cliquez sur la flèche pointant vers le bas après le nom du champ, puis cliquez sur **Insérer à gauche** ou **Insérer à droite** pour ajouter le nouveau champ.
1. Cliquez sur **Ajouter un existant** dans le coin inférieur droit de l’onglet **Nouveau champ**. <!--check UI - did they change this??-->

   ![Boîte de dialogue modale Ajouter des champs existants à partir de Workfront](assets/add-existing-fields-from-workfront-modal.png)

1. Commencez à saisir le nom d’un champ Workfront existant dans la zone de recherche, puis cliquez sur **+** lorsqu’il s’affiche dans la liste.
1. (Facultatif) Saisissez un autre champ, puis cliquez sur **+** lorsqu’il s’affiche dans la liste.
1. (Facultatif) Cliquez sur l’icône **Filtres** ![Icône Filtres dans les champs d’importation](assets/filters-in-import-fields-icon.png), puis mettez à jour l’un des champs suivants, ou les deux :

   * Type d’objet : sélectionnez un type d’objet Workfront dont vous souhaitez importer les champs.
   * Formulaire personnalisé : sélectionnez un ou plusieurs formulaires personnalisés dans Workfront. Vous pouvez sélectionner un formulaire personnalisé sans sélectionner au préalable un type d’objet.
1. Cliquez sur **+**, puis sur **Ajouter des champs**.
Les champs sont ajoutés en mode Tableau et dans les pages de détails des enregistrements.

   >[!IMPORTANT]
   >
   >    Il existe une limite de 500 champs pour tout type d’enregistrement. Les champs existants ainsi que les champs importés contribuent à cette limite.

   Les champs ajoutés sont des copies des champs Workfront et ne se connectent plus aux champs d’origine dans Workfront.
