---
title: Modifier les types d’enregistrements
description: Vous pouvez modifier les types d’enregistrement après leur enregistrement. Les types d’enregistrements sont les types d’objets d’Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7d6de742-9657-4286-968c-1fc78ebbb94e
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/PNC5GvQItDhcmQ0TSup8vbJJ3uWn2k-v-lKBZJBhakw
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 37be1f25fa54f3efd4113478496e95db3c8bce1c
workflow-type: tm+mt
source-wordcount: 611
ht-degree: 26%

---

# Modifier des types d’enregistrements

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

{{planning-important-intro}}

Les types d’enregistrements sont les types d’objets d’Adobe Workfront Planning. Vous pouvez modifier l’apparence des types d’enregistrement que vous ou toute autre personne avez créés. Pour plus d’informations sur la création de types d’enregistrement Workfront Planning, voir [Créer des types d’enregistrement](/help/quicksilver/planning/architecture/create-record-types.md).

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
<p>Tout package Workfront and Planning</p>
<p>Tout package Workfront and Planning</p>
<p><b>NOTE</b></p>
<p>Pour configurer les types d’enregistrements connectables : </p>
<ul> 
<li><p>Tout package Workfront et tout package Planning</p></li>
Ou
<li><p>Tout workflow et un package Planning Prime ou Ultimate</p></li></ul>


<p>Pour configurer les types d’enregistrements globaux :</p>

<ul> 
<li><p>Tout package Workfront et un package Planning Plus</p></li>
Ou
<li><p>Tout workflow et un package Planning Prime ou Ultimate</p></li></ul>
<p>Pour plus d’informations sur les composants inclus dans chaque package Workfront Planning, contactez votre représentant de compte Workfront. </p>

</td> </tr>
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
   <td>   <p>Manage permissions to a workspace and record type </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
   <p>Only system administrators can enable record types to connect from other workspaces</p> </td> 
  </tr> 

</tbody> 
</table>
-->

## Modifier des types d’enregistrements

{{step1-to-planning}}

1. Cliquez sur l’espace de travail dont vous souhaitez modifier les types d’enregistrements.

   La page Workspace s’ouvre et les types d’enregistrements s’affichent.
1. Utilisez l’une des méthodes suivantes :

   * Pointez sur la carte d’un type d’enregistrement et cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) dans le coin supérieur droit de la carte du type d’enregistrement, puis cliquez sur **Modifier** ou **Paramètres**
Ou
   * Cliquez sur une carte de type d’enregistrement pour ouvrir la page de type d’enregistrement, cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) à droite du nom du type d’enregistrement, puis cliquez sur **Modifier** ou **Paramètres**.

   ![Plus d’options de menu à partir d’une carte de type enregistrement avec Paramètres](assets/more-menu-options-from-record-type-card-with-settings-link.png)

1. Dans la zone **Modifier le type d’enregistrement**, l’onglet **Apparence** s’ouvre par défaut.

   ![Onglet Apparence de la zone Modifier le type d’enregistrement ](assets/edit-record-type-box-appearance-tab.png)

   Mettez à jour les informations suivantes dans l’onglet **Apparence** :

   * Modifiez le nom du type d’enregistrement, si nécessaire. <!--did they add a field label for this?-->
   * **Description** : modifiez ou ajoutez une description pour le type d’enregistrement avec plus d’informations à son sujet.
   * Modifiez la couleur et la forme de l’icône associée au type d’enregistrement. Procédez comme suit :
      * Sélectionnez une couleur pour identifier le type d’enregistrement. Il s’agit de la couleur de l’icône du type d’enregistrement.
      * Sélectionnez une icône dans la liste ou commencez à saisir le nom d’une icône pour décrire ce qu’elle représente, puis sélectionnez-la lorsqu’elle s’affiche. Il s’agit de l’icône du type d’enregistrement. Une icône de fichier est sélectionnée par défaut.

1. (Facultatif et conditionnel) Si vous êtes un administrateur système, cliquez sur l’onglet **Paramètres de l’espace de travail croisé** et mettez à jour les informations sur les fonctionnalités de l’espace de travail croisé du type d’enregistrement.

   Pour plus d’informations, voir [Configuration des fonctionnalités de plusieurs espaces de travail pour les types d’enregistrements](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).

   ![Zone Modifier le type d’enregistrement avec l’onglet Paramètres de l’espace de travail](assets/edit-record-type-box-advanced-settings-tab.png)

1. Cliquer sur **Enregistrer**.

   Si vous avez choisi de connecter cet enregistrement à partir d&#39;autres espaces de travail, l&#39;icône **Enregistrement connectable** ![Icône Se connecter à partir d&#39;autres espaces](assets/connect-from-other-workspaces-icon.png) s&#39;affiche sur la carte d&#39;enregistrement.

   Si vous avez choisi d’autoriser l’ajout de cet enregistrement à d’autres espaces de travail, l’icône **Enregistrement global** ![icône de type d’enregistrement global](assets/global-icon.png) s’affiche sur la carte d’enregistrement.

1. (Facultatif) Cliquez sur la carte de type d’enregistrement de la zone de l’espace de travail pour ouvrir la page du type d’enregistrement, puis renommez le type d’enregistrement dans l’en-tête.

1. (Facultatif) Pour modifier un autre type d’enregistrement, sur la page Type d’enregistrement , développez la flèche pointant vers le bas à droite du nom d’un type d’enregistrement, recherchez un type d’enregistrement, puis sélectionnez-le lorsqu’il s’affiche dans la liste.

   ![Liste déroulante Type d’enregistrement sur la page Type d’enregistrement avec la zone de recherche](assets/record-type-drop-down-on-record-type-page-with-search-box.png)

   >[!TIP]
   >
   >Vous pouvez utiliser la combinaison de clavier suivante pour ouvrir la zone de recherche globale à partir de n’importe quelle page Workfront Planning et rechercher des types d’enregistrements :
   >
   >* CTRL+K pour Windows
   >* ⌘+K pour Mac
   >
   >![Zone de recherche globale](assets/global-search-box.png)
