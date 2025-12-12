---
title: Gérer les notifications par e-mail de planification d’Adobe Workfront
description: Lorsqu’une personne vous identifie ou identifie vos équipes dans un commentaire d’enregistrement dans Adobe Workfront Planning, vous recevez une notification par e-mail concernant cette balise.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 3c505b3a-cda7-4e7b-b497-28b820e9bb8f
source-git-commit: 5404cec0cb02d363154a3696b63aaedaafc82688
workflow-type: tm+mt
source-wordcount: '586'
ht-degree: 6%

---


# Gérer les notifications par e-mail d’Adobe Workfront Planning

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Vous pouvez recevoir des notifications par e-mail de Workfront Planning lorsque les scénarios suivants existent :

* Quelqu’un vous identifie ou identifie vos équipes dans un commentaire d’enregistrement.

  Pour plus d’informations sur le balisage d’autres utilisateurs dans un commentaire d’enregistrement, voir [Gérer les commentaires d’enregistrement](/help/quicksilver/planning/records/manage-record-comments.md).
* Quelqu&#39;un vous demande votre autorisation pour accéder à une vue, un espace de travail ou un type d&#39;enregistrement <!--or <span class="preview">or a record</span>-->
* Quelqu&#39;un confirme que votre accès a été accordé pour une vue, un espace de travail ou un type d&#39;enregistrement <!--<span class="preview">or record</span>--> <!--Isk confirmed that there is nno email for denying access but did not test-->
* Vous devez soumettre une demande Workfront Planning. Pour plus d’informations, voir [Création et gestion d’un formulaire de demande dans Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md)
* Une personne approuve ou rejette une demande Workfront Planning que vous avez soumise. Pour plus d’informations, voir [Approuver une demande dans Adobe Workfront Planning](/help/quicksilver/planning/requests/approve-request.md)
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

<!--
OLD: 

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
   <td><p> Standard, Light, or Contributor</p>
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
</table>
-->


## Gérer les notifications par e-mail lorsqu’une personne vous identifie dans un commentaire

1. (Conditionnel et facultatif) Une fois qu’une personne vous a identifié, vous ou votre équipe, dans un commentaire sur un enregistrement, accédez à l’e-mail de notification qui vous informe de la balise et du commentaire. L’expéditeur de l’e-mail est Adobe Experience Cloud.

   ![Exemple de notifications par e-mail](assets/email-notification-example.png)

1. (Facultatif) Cliquez sur le message dans la zone **Workfront** de l’e-mail.

   La page des détails de l’enregistrement s’ouvre dans Workfront. Vous pouvez mettre à jour l’enregistrement ou répondre au commentaire.

1. (Conditionnel) Si disponible, cliquez sur **Afficher toutes les notifications**. <!--check with Lilit - do non-IMS users have this button??-->
La page **Notifications** s’ouvre dans Adobe Experience Cloud. Toutes les notifications de toutes les applications Adobe Experience Cloud s’affichent.

## Gérer les notifications par e-mail lors de la demande et de l’octroi d’autorisations

1. (Conditionnel et facultatif) Lorsqu&#39;une personne vous demande ou vous accorde des autorisations pour accéder à un type d&#39;objet Planning, accédez à l&#39;e-mail qui vous informe de la demande d&#39;autorisation. L’expéditeur de l’e-mail est Adobe Experience Cloud.

1. (Facultatif) Cliquez sur le message dans la zone **Workfront** de l’e-mail.

   L’objet pour lequel vous avez demandé des autorisations s’ouvre dans Workfront.

1. (Conditionnel) Si disponible, cliquez sur **Afficher toutes les notifications**.
La page **Notifications** s’ouvre dans Adobe Experience Cloud. Toutes les notifications de toutes les applications Adobe Experience Cloud s’affichent.


Pour plus d’informations sur la demande, l’octroi ou le refus d’autorisations, voir [Demander des autorisations pour une vue ou un espace de travail](/help/quicksilver/planning/access/request-permissions.md).

Pour plus d’informations sur la gestion des notifications Workfront Planning, voir [Gérer les préférences de notification Adobe Workfront Planning](/help/quicksilver/planning/notifications/manage-notification-preferences.md).

## Gérer les notifications par e-mail relatives à la soumission, l’approbation ou le rejet de demandes Workfront Planning

1. (Facultatif) Accédez à l’e-mail que Workfront vous envoie
après la soumission d&#39;une demande ou après qu&#39;une demande que vous avez soumise a été approuvée ou rejetée. L’expéditeur de l’e-mail est Adobe Workfront.

1. (Facultatif) Cliquez sur **Ouvrir la demande**. La demande s’ouvre alors dans Workfront Planning.

1. Cliquez sur l’icône **Notifications** ![Icône de la zone de notifications Unified Shell](assets/notifications-area-icon-unified-shell.png) dans le coin supérieur droit de l’écran pour accéder à la page **Notifications**.

   Pour plus d’informations sur la gestion des notifications Workfront Planning, voir [Gérer les préférences de notification Adobe Workfront Planning](/help/quicksilver/planning/notifications/manage-notification-preferences.md).
