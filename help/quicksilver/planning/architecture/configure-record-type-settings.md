---
title: Configuration de la zone Paramètres d’un type d’enregistrement
description: Vous pouvez modifier les types d’enregistrements après les avoir enregistrés dans la page Paramètres.
hide: true
hidefromtoc: true
source-git-commit: 8546311acf722c0f4d47d4663b02ff701416894a
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 10%

---


<!--add better metadata at release:

title: Configure Record Type Settings
description: You can edit record types after they have been saved in the Settings page. 
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog 

-->

# Configuration de la zone Paramètres d’un type d’enregistrement

<span class="preview">Les informations de cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de façon générale. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Après les versions mensuelles en production, les mêmes fonctionnalités sont également disponibles dans l’environnement de production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation des versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Vous pouvez configurer des paramètres supplémentaires pour un type d’enregistrement après les avoir enregistrés dans Adobe Workfront Planning.

Selon les fonctionnalités que vous souhaitez définir pour un type d’enregistrement, vous pouvez configurer des paramètres supplémentaires pour celui-ci en effectuant l’une des opérations suivantes :

<!--the above will need to be reworded when we add automations and manage request forms to this area-->

* Les modifier

  Pour plus d’informations, voir [Modifier les types d’enregistrements](/help/quicksilver/planning/architecture/edit-record-types.md).

* Configuration de la page Paramètres d’un type d’enregistrement.

  Cet article décrit comment modifier un type d’enregistrement en configurant sa page Paramètres.

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
<ul><li><p>Tout package Workfront</p></li>
<p>Et</p>
<li><p>Tout package Planning permettant de créer des types d'enregistrements connectables</p></li>
<li><p>Package Planning Plus pour créer des types d'enregistrements centralisés</p></li>
</ul>
<p>Ou :</p>
<ul><li><p>Un package Workflow and Planning Prime ou Ultimate</p> </li></ul>
<p>Pour plus d’informations sur les composants inclus dans chaque package Workfront Planning, contactez votre gestionnaire de compte Workfront. </p> 
   </td>

<tr> 
   <td role="rowheader"><p>Licence Adobe Workfront</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td>   <p>Gérer des autorisations relatives à un espace de travail</a> </p>  
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
</table> 

-->

## Configurer les informations sur le type d’enregistrement dans la page Paramètres

Vous pouvez définir des fonctionnalités inter-espaces de travail pour un type d’enregistrement en configurant les informations dans sa page Paramètres.

<!--the intro above will change when we can configure more in this area -->

{{step1-to-planning}}

1. Cliquez sur l’espace de travail dont vous souhaitez modifier les types d’enregistrements,

   La page Workspace s’ouvre et les types d’enregistrements s’affichent.
1. Utilisez l’une des méthodes suivantes :

   * Pointez sur la carte d’un type d’enregistrement et cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) dans le coin supérieur droit de la carte de type d’enregistrement, puis cliquez sur **Paramètres**
Ou
   * Cliquez sur une carte de type d’enregistrement pour ouvrir la page de type d’enregistrement, cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) à droite du nom du type d’enregistrement, puis cliquez sur **Paramètres**.

   <!--update screen shot at release-->

   ![Autres options de menu de la carte de type d’enregistrement](assets/more-menu-options-from-record-type-card.png)

1. La section **Paramètres de l’espace de travail croisé** est sélectionnée par défaut.
1. Activez ou désactivez l’un des paramètres suivants :

   * **Autoriser l&#39;ajout de ce type d&#39;enregistrement à d&#39;autres espaces de travail** pour indiquer qu&#39;il s&#39;agit d&#39;un type d&#39;enregistrement global
   * **Autoriser la connexion à ce type d&#39;enregistrement dans d&#39;autres espaces de travail** pour indiquer qu&#39;il s&#39;agit d&#39;un type d&#39;enregistrement connectable.

   Les paramètres sont désactivés par défaut.

   Pour plus d’informations, voir [Configuration des fonctionnalités de plusieurs espaces de travail pour les types d’enregistrements](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md)