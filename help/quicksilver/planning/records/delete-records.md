---
title: Supprimer enregistrements
description: Vous pouvez supprimer des enregistrements que vous ou une autre personne avez créés.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 3f7a3667-8a9f-462a-b706-cf15850a0d1c
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/zW-UgmPeIG-6sjZZelIiYE3JDNvpqQxb-a81Ggau2nQ
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 686
ht-degree: 35%

---

# Supprimer des enregistrements


<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de manière générale. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Après les versions mensuelles en production, les mêmes fonctionnalités sont également disponibles dans l’environnement de production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation des versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Vous pouvez supprimer des enregistrements qui ne sont plus pertinents dans Adobe Workfront Planning. Vous pouvez récupérer les enregistrements supprimés pendant 30 jours après leur suppression. Pour plus d’informations sur la récupération des enregistrements supprimés, voir [ Récupérer les enregistrements supprimés ](/help/quicksilver/planning/records/restore-deleted-records.md).

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
   <td>   <p>Accorder des autorisations supérieures ou égales à un espace de travail, un type d’enregistrement et <span class="preview">gérer les autorisations d’un enregistrement</span> </p>   
   <p>L’administration système a accès à tous les espaces de travail, y compris ceux qu’elle n’a pas créés.</p> </td> 
  </tr>   
</tbody> 
</table>

Pour plus d’informations sur les exigences d’accès à Workfront, voir [Exigences d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   


<!--
Old:
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
   <td>   <p>Contribute or higher permissions to a workspace and record type </a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
</tbody> 
</table>
-->

## Considérations sur la suppression des enregistrements

* Vous pouvez supprimer des enregistrements que vous ou une autre personne avez créés.
* Vous pouvez récupérer les enregistrements supprimés que vous ou d&#39;autres personnes avez supprimés.
* Lorsque des enregistrements supprimés sont liés à d’autres enregistrements, ces enregistrements liés restent intacts, bien que les informations de l’enregistrement supprimé soient éliminées.
* Vous ne pouvez pas supprimer des enregistrements des vues Chronologie ou Calendrier.

## Supprimer des enregistrements

Vous pouvez supprimer un enregistrement à partir des zones suivantes :

* [À partir de la page de l’enregistrement](#delete-a-record-from-the-records-page)
* [À partir de la vue de tableau d’un type d’enregistrement](#delete-a-record-from-the-record-type-table-view)

### Supprimer un enregistrement à partir de la page de l’enregistrement

{{step1-to-planning}}

1. Cliquez sur l’espace de travail dont vous souhaitez supprimer les enregistrements.

   L’espace de travail s’ouvre et les types d’enregistrements s’affichent sous forme de cartes.

1. Cliquez sur la vignette d’un type d’enregistrement pour plus de détails.

   La page de type d’enregistrement s’ouvre.
1. Utilisez l’une des méthodes suivantes :

   * À partir d’une vue en tableau, cliquez sur le nom d’un enregistrement.
   * En mode Tableau, passez la souris sur le nom d’un enregistrement, puis cliquez sur le menu **Plus** ![Plus](assets/more-menu.png), puis sur **Affichage**

     ![Menu contextuel pour la ligne d’enregistrement](assets/contextual-menu-for-record-row.png)
   * Dans une vue de chronologie, cliquez sur une barre d’un enregistrement.

   La page de l’enregistrement s’ouvre.

1. Cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) à droite du nom de l’enregistrement, puis cliquez de nouveau sur **Supprimer**, **Supprimer** pour confirmer.

   ![Plus d’options de menu dans la page des détails de l’enregistrement](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed-->
L’enregistrement est supprimé.
1. (Facultatif) Accédez à la vue Tableau de la page d’enregistrement, puis cliquez sur l’icône **Annuler** ![Icône Annuler](assets/undo-icon.png) dans le coin supérieur droit de la vue, puis cliquez sur **Récemment supprimé** pour récupérer les enregistrements supprimés.

Pour plus d’informations sur la récupération des enregistrements supprimés, voir [ Récupérer les enregistrements supprimés ](/help/quicksilver/planning/records/restore-deleted-records.md).

### Supprimer un enregistrement de la vue en tableau d’un type enregistrement

{{step1-to-planning}}

1. Cliquez sur l’espace de travail dont vous souhaitez supprimer les enregistrements.

   L’espace de travail s’ouvre et les types d’enregistrements s’affichent sous forme de cartes.

1. Cliquez sur la vignette d’un type d’enregistrement pour plus de détails.

   La page de type d’enregistrement s’ouvre.
1. (Conditionnel) Dans le menu déroulant **Afficher** situé dans le coin supérieur gauche du tableau, sélectionnez une vue de tableau. Il s’agit de la vue par défaut, sauf si vous avez visualisé le type d’enregistrement dans la vue chronologique lors de votre dernier accès.

   Les enregistrements associés au type d’enregistrement sélectionné s’affichent dans la vue Tableau.
1. Utilisez l’une des méthodes suivantes :

   * Cliquez avec le bouton droit de la souris sur une ligne d’enregistrement, puis cliquez sur **Supprimer**.
   * Cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) à droite du nom de l’enregistrement, puis cliquez sur **Supprimer**.

     ![Menu contextuel pour la ligne d’enregistrement](assets/contextual-menu-for-record-row.png)

   * Cliquez sur l’icône **Ouvrir les détails** ![Icône Ouvrir les détails dans le champ nom de la table](assets/open-details-icon-in-table-name-field.png) pour ouvrir la zone contenant les informations détaillées de l’enregistrement, puis cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) à droite du nom de l’enregistrement, puis sur **Supprimer**.

   L’enregistrement est supprimé.

1. (Facultatif) Effectuez l’une des opérations suivantes pour annuler ou rétablir la suppression d’un enregistrement :

   * Cliquez sur l&#39;icône **Annuler** ![Icône Annuler](assets/undo-icon.png), puis **Récemment supprimé** pour récupérer les enregistrements supprimés. Pour plus d’informations sur la récupération des enregistrements supprimés, voir [ Récupérer les enregistrements supprimés ](/help/quicksilver/planning/records/restore-deleted-records.md).
   * Utilisez les raccourcis clavier suivants pour annuler ou rétablir la suppression d’un enregistrement :

      * Ctrl + Z (⌘ + Z pour Mac) pour annuler la suppression d’un enregistrement
      * Ctrl+Maj+Z (⌘+Maj+Z pour Mac) pour rétablir la suppression de l’enregistrement.




