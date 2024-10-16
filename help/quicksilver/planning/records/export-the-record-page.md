---
title: Exportation de la page d’enregistrement
description: Vous pouvez exporter la page d’aperçu ou de détails de l’enregistrement vers Word.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 8de68b70-dd87-4aad-9137-980ea9fc0d69
source-git-commit: f7ad56375c20e26b0d45ae0966e2e156b5a200f1
workflow-type: tm+mt
source-wordcount: '480'
ht-degree: 22%

---

# Exporter les détails d’un enregistrement

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers, or in the Production environment for customers who enabled fast releases.</span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">For information about the current release, see [Fourth Quarter 2023 release overview](/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md).</span>-->


Pour collaborer plus efficacement avec d’autres utilisateurs qui ne disposent pas d’un compte Workfront, vous pouvez exporter les détails d’un enregistrement vers un fichier et le partager avec eux.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès à la planification Workfront.

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
<p>L’un des projets Workfront suivants est prévu :</p> 
<ul><li>Sélectionner</li> 
<li>Principal</li> 
<li>Final</li></ul> 
<p>La planification Workfront n’est pas disponible pour les plans Workfront hérités</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Formule de planification Adobe Workfront*</p></td> 
   <td> 
<p>Tous </p> 
<p>Pour plus d’informations sur les éléments inclus dans chaque plan de planification Workfront, contactez votre gestionnaire de compte Workfront. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Plateforme Adobe Workfront</p></td> 
   <td> 
<p>L’instance de Workfront de votre entreprise doit être intégrée à l’expérience unifiée Adobe pour pouvoir accéder à toutes les fonctionnalités de la planification Workfront.</p> 
<p>Pour plus d’informations, voir <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience pour Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront*</p></td> 
   <td> <p>Standard</p>
   <p>La planification Workfront n’est pas disponible pour les licences Workfront héritées</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuration du niveau d’accès</p></td> 
   <td> <p>Il n’existe aucun contrôle de niveau d’accès pour Adobe Workfront Planning.</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td>   <p>Autorisations d’affichage ou supérieures à un espace de travail</a> </p>  
   <p>L’administration système a accès à tous les espaces de travail, y compris ceux qu’elle n’a pas créés.</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modèle de disposition</p></td> 
   <td> <p>Toutes les personnes, y compris les administrateurs et administratrices de Workfront, doivent se voir attribuer un modèle de mise en page incluant la zone Planning dans le menu principal. </p> </td> 
  </tr> 
</tbody> 
</table>

* Pour plus d’informations sur les exigences d’accès à Workfront, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--OLD:

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p>
   Or
   <p>Current: Plan</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> <p>There are no access controls for Adobe Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>View or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>

 </tbody>
</table>

*For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). -->

## Remarques concernant l’export des détails d’un enregistrement :

* Vous pouvez exporter les détails d’un enregistrement vers les formats de fichier suivants :

   * .docx Word
   * pdf

* Vous pouvez exporter l’onglet Détails de la page d’un enregistrement. Vous ne pouvez pas exporter l’onglet Connexions .

* Le fichier exporté conserve la mise en page de la page d’enregistrement, y compris la miniature et les images de couverture.

## Exporter les détails d’un enregistrement

{{step1-to-planning}}

1. Cliquez sur la carte d’un espace de travail.

   L’espace de travail s’ouvre et les types d’enregistrement s’affichent sur les cartes.

1. Cliquez sur une carte de type enregistrement.
La page de type enregistrement s’ouvre et tous les enregistrements de ce type s’affichent.

1. Dans n’importe quelle vue, cliquez sur le nom d’un enregistrement.

   La boîte d’aperçu de l’enregistrement s’ouvre.

1. (Facultatif) Cliquez sur l’icône **Ouvrir dans un nouvel onglet** ![](assets/open-details-in-a-new-tab-icon.png) pour ouvrir la page de l’enregistrement.

1. Sélectionnez l’onglet **Détails** . L’onglet Détails doit s’ouvrir par défaut.

1. Cliquez sur l&#39;icône **Exporter** ![](assets/export-icon-in-record-details-page.png) dans la page d&#39;aperçu ou d&#39;enregistrement, puis cliquez sur l&#39;une des options suivantes :

   * **Microsoft Word**
   * **Adobe PDF**

   Un fichier Word (.docx) ou PDF est téléchargé et enregistré sur votre ordinateur.

   Le nom du fichier exporté est le champ de Principal de l’enregistrement.

   ![](assets/exported-word-file.png)

   >[!NOTE]
   >
   >    Les informations supplémentaires qui ne s’affichent pas sur la page et ne sont visibles qu’après avoir cliqué sur Afficher plus dans la zone des détails de l’enregistrement ne s’affichent pas dans le fichier de PDF exporté. Seules les informations visibles sur la page s’affichent dans le fichier exporté.


1. (Facultatif) Accédez au fichier téléchargé, ouvrez-le et modifiez-le (s’il s’agit d’un fichier Word) ou partagez-le avec d’autres personnes.

