---
title: Modifier les types d’enregistrements
description: Vous pouvez modifier les types d’enregistrement après leur enregistrement. Les types d’enregistrements sont les types d’objets d’Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7d6de742-9657-4286-968c-1fc78ebbb94e
source-git-commit: 8546311acf722c0f4d47d4663b02ff701416894a
workflow-type: tm+mt
source-wordcount: '636'
ht-degree: 25%

---


# Modifier des types d’enregistrements

<span class="preview">Les informations de cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de façon générale. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Après les versions mensuelles en production, les mêmes fonctionnalités sont également disponibles dans l’environnement de production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation des versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

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
   <td role="rowheader"><p>Package Adobe Workfront</p></td> 
   <td> 
<p>Pour activer les types d’enregistrements connectables : </p>
<ul> 
<li><p>Tout package Workfront et tout package Planning</p></li>
<p>Ou</p>
<li><p>Packages Prime et Ultimate de workflow et de planification</p></li></ul>

<p>Pour activer les types d’enregistrements globaux :</p>

<ul> 
<li><p>Tout package Workfront et un package Planning Plus</p></li>
<p>Ou</p>
<li><p>Packages Prime et Ultimate de workflow et de planification</p></li></ul>
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
   <td>   <p>Manage permissions to a workspace and record type </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
   <p>Only system administrators can enable record types to connect from other workspaces</p> </td> 
  </tr> 

</tbody> 
</table> -->

## Modifier des types d’enregistrements

{{step1-to-planning}}

1. Cliquez sur l’espace de travail dont vous souhaitez modifier les types d’enregistrements.

   La page Workspace s’ouvre et les types d’enregistrements s’affichent.
1. Utilisez l’une des méthodes suivantes :

   * Pointez sur la carte d’un type d’enregistrement et cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) dans le coin supérieur droit de la carte du type d’enregistrement, puis cliquez sur **Modifier**
     <!--<span class="preview">or **Settings**</span>-->
Ou
   * <span class="preview">Cliquez sur une carte de type d’enregistrement pour ouvrir la page de type d’enregistrement, cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) à droite du nom du type d’enregistrement, puis cliquez sur **Modifier**<!--<span class="preview">or **Settings**</span>. </span>-->

   <!--<span class="preview">![More menu options from record type card](assets/more-menu-options-from-record-type-card.png)</span>-->

1. Dans la zone **Modifier le type d’enregistrement**, l’onglet **Apparence** s’ouvre par défaut. <!--update screen shot below at preview-->

   ![Onglet Apparence de la zone Modifier le type d’enregistrement &#x200B;](assets/edit-record-type-box-appearance-tab.png)

   Mettez à jour les informations suivantes dans l’onglet **Apparence** :

   * Modifiez le nom du type d’enregistrement, si nécessaire. <!--did they add a field label for this?-->
   * **Description** : modifiez ou ajoutez une description pour le type d’enregistrement avec plus d’informations à son sujet.
   * Modifiez la couleur et la forme de l’icône associée au type d’enregistrement. Procédez comme suit :
      * Sélectionnez une couleur pour identifier le type d’enregistrement. Il s’agit de la couleur de l’icône du type d’enregistrement.
      * Sélectionnez une icône dans la liste ou commencez à saisir le nom d’une icône pour décrire ce qu’elle représente, puis sélectionnez-la lorsqu’elle s’affiche. Il s’agit de l’icône du type d’enregistrement. Une icône de fichier est sélectionnée par défaut.


1. (Facultatif et conditionnel) Si vous êtes un administrateur système, cliquez sur **Paramètres avancés** et mettez à jour les informations suivantes dans la section **Fonctionnalité interespace de travail** : <!--the info here is duplicated in the Create record types article-->
   * Activez le paramètre **Autoriser la connexion à ce type d’enregistrement dans d’autres espaces de travail** : permet aux gestionnaires d’espace de travail de se connecter à ce type d’enregistrement à partir d’autres espaces de travail.\
     Vous pouvez désigner les espaces de travail auxquels ce type d’enregistrement peut être connecté. Vous pouvez le rendre disponible pour tous les espaces de travail ou désigner des espaces de travail spécifiques où vous pouvez l’importer.
Pour plus d’informations, voir [Configuration des fonctionnalités de plusieurs espaces de travail pour les types d’enregistrements](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).


   ![Boîte Créer un type d’enregistrement dans l’onglet Paramètres avancés](assets/create-record-type-box-advanced-settings-tab.png)

   <!--replace last point with this when we release global record types; the preview tags might need to be edited, too:
    1. <span class="preview">(Optional and conditional) If you are a system administrator, update the information in the **Cross-workspace settings** tab.</span>
    <span class="preview">For more information, see [Configure cross-workspace capabilities for record types](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).</span>
    ***********Add screenshot***********
    -->

1. Cliquer sur **Enregistrer**.

   La carte de type d’enregistrement de l’espace de travail affiche une icône de connectivité ![Icône Se connecter à partir d’autres espaces de travail](assets/connect-from-other-workspaces-icon.png) dans le coin supérieur droit pour indiquer que l’enregistrement est désormais accessible à partir d’autres espaces de travail.

   <!--replace the blurb above after "Save" with this: <span class="preview">If you configured the cross-workspace capabilities for the record, the **connectable record type** icon ![Connectable record type icon](assets/connect-from-other-workspaces-icon.png) and the **global record type** icon ![Global record type icon](assets/global-icon.png) also display on the card. </span>-->

1. (Facultatif) Cliquez sur la carte de type d’enregistrement de la zone de l’espace de travail pour ouvrir la page du type d’enregistrement, puis renommez le type d’enregistrement dans l’en-tête.

1. (Facultatif) Pour modifier un autre type d’enregistrement, sur la page Type d’enregistrement , développez la flèche pointant vers le bas à droite du nom d’un type d’enregistrement, recherchez un type d’enregistrement, puis sélectionnez-le lorsqu’il s’affiche dans la liste.

   ![Liste déroulante Type d’enregistrement sur la page Type d’enregistrement avec la zone de recherche](assets/record-type-drop-down-on-record-type-page-with-search-box.png)
