---
title: Exporter la page d’enregistrement
description: Vous pouvez exporter la page d'aperçu ou de détails d'un enregistrement d'Adobe Workfront Planning vers un fichier Microsoft Word.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 8de68b70-dd87-4aad-9137-980ea9fc0d69
source-git-commit: e26a3d0e283182e08902c263252c8d067838c23a
workflow-type: tm+mt
source-wordcount: '433'
ht-degree: 5%

---

# Exporter les détails d’un enregistrement

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers, or in the Production environment for customers who enabled fast releases.</span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>-->


Pour collaborer plus efficacement avec d’autres utilisateurs qui ne disposent pas nécessairement d’un compte Workfront, vous pouvez exporter la page de détails d’un enregistrement dans un fichier Microsoft Word et la partager avec eux.

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
<p>Tout Workfront et tout package Planning</p> <p>Tout workflow et tout package Planning</p>
<p>Pour plus d’informations sur les composants inclus dans chaque package Workfront Planning, contactez votre représentant de compte Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront</p></td> 
   <td><p>Léger ou supérieur</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td>   <p>Autorisations d’affichage ou supérieures pour un espace de travail et un type d’enregistrement</a> </p>  
   <p>L’administration système a accès à tous les espaces de travail, y compris ceux qu’elle n’a pas créés.</p> </td> 
  </tr> 
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
   <td> <p>Light or higher</p>
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
   <td>   <p>View or higher permissions to a workspace and record type</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
</tbody> 
</table> 

 *For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).-->


## Considérations relatives à l’exportation des détails d’un enregistrement :

* Vous pouvez exporter les détails d’un enregistrement aux formats de fichiers suivants :

   * .docx Word
   * pdf

* Vous ne pouvez exporter que l&#39;onglet Détails de la page ou de la zone d&#39;aperçu d&#39;un enregistrement.

* Le fichier exporté conserve la disposition de la page d’enregistrement, y compris les images de la miniature et de la couverture.

## Exporter les détails d’un enregistrement

{{step1-to-planning}}

1. Cliquez sur la vignette d’un espace de travail.

   L’espace de travail s’ouvre et les types d’enregistrements s’affichent sur les cartes.

1. Cliquez sur une carte de type d’enregistrement.
La page de type d’enregistrement s’ouvre et tous les enregistrements de ce type s’affichent.

1. Dans n’importe quel affichage, cliquez sur le nom d’un enregistrement.

   La zone d&#39;aperçu de l&#39;enregistrement s&#39;ouvre.

1. (Facultatif) Cliquez sur l’icône **Ouvrir dans un nouvel onglet** ![Ouvrir les détails dans une nouvelle icône d’onglet](assets/open-details-in-a-new-tab-icon.png) pour ouvrir la page de l’enregistrement.

1. Sélectionnez l’onglet **Détails**. L’onglet Détails doit s’ouvrir par défaut.

1. Cliquez sur le menu **Exporter** ![icône Exporter dans la page des détails de l&#39;enregistrement](assets/export-icon-in-record-details-page.png) dans l&#39;aperçu ou dans la page de l&#39;enregistrement, puis cliquez sur l&#39;une des options suivantes :

   * **Microsoft Word**
   * **Adobe PDF**

   Un fichier Word (.docx) ou PDF est téléchargé et enregistré sur votre ordinateur.

   Le nom du fichier exporté est le champ de Principal de l’enregistrement.

   ![Fichier Word exporté](assets/exported-word-file.png)

   >[!NOTE]
   >
   >    Les informations supplémentaires qui ne s’affichent pas sur la page et qui ne sont visibles qu’après avoir cliqué sur Afficher plus dans la zone des détails de l’enregistrement ne s’affichent pas dans le fichier PDF exporté. Seules les informations visibles sur la page s’affichent dans le fichier exporté.


1. (Facultatif) Accédez au fichier téléchargé, ouvrez-le et modifiez-le (s’il s’agit d’un fichier Word) ou partagez-le avec d’autres personnes.

