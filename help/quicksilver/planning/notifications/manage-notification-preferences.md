---
title: Gérer les préférences de notification d’Adobe Workfront Planning
description: Vous pouvez peut-être gérer vos préférences de notification pour Adobe Workfront Planning. Cet article décrit comment configurer vos préférences de notifications.
author: Alina
feature: Workfront Planning
role: User
recommendations: noDisplay, noCatalog
exl-id: ec549a61-095c-433f-80e2-1be5c0a05180
source-git-commit: 5404cec0cb02d363154a3696b63aaedaafc82688
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 11%

---


# Gérer les préférences de notification d’Adobe Workfront Planning

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Vous pouvez recevoir une notification in-app ou par e-mail lorsque les actions suivantes se produisent dans Workfront Planning :

* Quelqu’un vous ajoute, vous ou vos équipes, à un commentaire sur la page d’enregistrement
* Quelqu&#39;un demande l&#39;autorisation d&#39;accéder à une vue ou à un espace de travail <!--or <span class="preview">or a record</span>-->
* Quelqu&#39;un vous accorde l&#39;autorisation d&#39;accéder à une vue ou à un espace de travail <!--or <span class="preview">or a record</span>--> <!--I could not test this but Isk confirmed-->
* Vous devez soumettre une demande Workfront Planning.
* Une personne approuve ou rejette une demande Workfront Planning que vous avez soumise.
* Le statut passe à une demande Workfront Planning que vous avez soumise.

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
   <td><p>Léger ou supérieur</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td>   <p>Autorisations d’affichage ou supérieures à un espace de travail</a> </p>  
   <p>L’administration système a accès à tous les espaces de travail, y compris ceux qu’elle n’a pas créés.</p> </td> 
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
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience.</p> 
<p>The users in your organization receive notifications from Workfront Planning only when your organization is onboarded to the Adobe Unified Experience. </p>
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p><p>Standard, Light, or Contributor
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
   <td>   <p>View or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> Users with a Light or Contributor license must be assigned a layout template that includes Planning.
   <p>Standard users and System Administrators have the Planning areas enabled by default.</p></div></li></ul>
  
</td>
  </tr>

</tbody> 
</table> -->

Pour plus d’informations sur les notifications de Workfront Planning, consultez également les articles suivants :

* Pour plus d’informations sur les commentaires des enregistrements, voir [Gérer les commentaires des enregistrements](/help/quicksilver/planning/records/manage-record-comments.md).
* Pour plus d’informations sur les notifications in-app depuis Workfront Planning, voir [Gérer les notifications in-app pour Adobe Workfront Planning](/help/quicksilver/planning/notifications/manage-planning-in-app-notifications.md).
* Pour plus d’informations sur les notifications par e-mail provenant de Workfront Planning, voir [Gérer les notifications par e-mail pour Adobe Workfront Planning](/help/quicksilver/planning/notifications/manage-planning-email-notifications.md).


## Gestion des préférences de notification

1. Connectez-vous à Workfront à l’aide de vos informations d’identification Adobe Experience Cloud.
1. Cliquez sur l’icône **menu du compte** ![icône du menu du compte dans Experience Cloud](assets/account-menu-icon-on-experience-cloud.png) dans le coin supérieur droit de l’écran, puis cliquez sur **Préférences**.
1. Dans la section **Notifications**, cliquez sur **Workfront**.
1. Sélectionnez les notifications que vous souhaitez recevoir.
Ou
Désélectionnez les notifications que vous souhaitez arrêter de recevoir.

   Panneau de notifications ![Adobe Experience Cloud pour Workfront Planning](assets/adobe-experience-cloud-notifications-panel-for-workfront-planning.png)
1. Les notifications suivantes sont disponibles pour Workfront :

   * **Mentions** : vous recevez une notification lorsqu’une personne vous identifie ou identifie votre équipe dans un commentaire dans Workfront Planning
   * **Demandes** : vous recevez une notification lorsqu’une personne effectue l’une des opérations suivantes :

      * Demande ou vous accorde l&#39;autorisation d&#39;accéder à un objet Workfront Planning
      * Vous avez soumis une demande Workfront Planning
      * Statut d’une demande Workfront Planning que vous avez soumise modifications
      * Demande, accorde ou rejette une approbation à une demande Workfront Planning

   Pour plus d’informations sur la gestion des notifications, voir [ Préférences du compte et notifications ](https://experienceleague.adobe.com/fr/docs/core-services/interface/features/account-preferences).

<!--OLD: notifications are not available to non-IMS customers: 

When someone adds you to a comment in the record page, you may receive an in-app as well as an email notification about the comment. 

The following scenarios exist:   

* Adobe Unified Experience customers receive both an in-app notification and an email notification. They can manage their in-app and email notification preferences in the Preferences area of their Adobe Experience Cloud profile for the Workfront product. 

    For more information, see [Account preferences and notifications](https://experienceleague.adobe.com/en/docs/core-services/interface/features/account-preferences).

* Customers who are not on the Adobe Unified Experience receive only an email notification. They cannot manage their email notifications preferences and will always receive an email when someone adds them to a comment on a record in Workfront Planning.   

-->
