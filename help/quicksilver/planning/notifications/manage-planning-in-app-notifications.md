---
title: Gérer les notifications in-app d’Adobe Workfront Planning
description: Lorsqu’une personne vous identifie ou identifie vos équipes dans un commentaire d’enregistrement, vous recevez une notification par e-mail concernant cette balise.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: a6eb8c7c-a34d-4c84-a45c-7e7f050a4302
source-git-commit: 5404cec0cb02d363154a3696b63aaedaafc82688
workflow-type: tm+mt
source-wordcount: '359'
ht-degree: 10%

---


# Gérer les notifications in-app d’Adobe Workfront Planning

{{planning-important-intro}}

Vous pouvez recevoir des notifications in-app de Workfront Planning lorsque les scénarios suivants existent :

* Quelqu’un vous identifie ou identifie vos équipes dans un commentaire d’enregistrement.

  Pour plus d’informations sur le balisage d’autres utilisateurs dans un commentaire d’enregistrement, voir [Gérer les commentaires d’enregistrement](/help/quicksilver/planning/records/manage-record-comments.md).
* Quelqu&#39;un vous demande l&#39;autorisation d&#39;accéder à une vue ou à un espace de travail <!--<span class="preview">or record</span>-->
* Quelqu&#39;un confirme que votre accès a été accordé pour une vue ou un espace de travail <!--<span class="preview">or record</span>--> <!--Isk confirmed there is no notification for denying permissions - did not test-->

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

+++ Expand to view access requirements. 

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
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>  </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> Users with a Light or Contributor license must be assigned a layout template that includes Planning.
   <p>Standard users and System Administrators have the Planning areas enabled by default.</p></div></li></ul>
</td>
  </tr>
</tbody> 
</table> 

+++
-->

## Gérer les notifications in-app lorsqu’une personne vous identifie dans un commentaire

1. (Conditionnel) Lorsqu’un utilisateur vous a identifié ou identifié vos équipes dans un commentaire sur un enregistrement, accédez à l’icône in-app **Notifications** ![icône de notifications Experience Cloud](assets/experience-cloud-notifications-icon.png) dans Adobe Experience Cloud.

   ![ Exemple de notification in-app ](assets/in-app-notification-example.png)

1. Cliquez sur la notification.

   La page Détails de l’enregistrement s’ouvre dans Workfront Planning. Vous pouvez mettre à jour l’enregistrement ou répondre au commentaire.

1. (Facultatif) Cliquez sur **Marquer tout comme lu** pour indiquer que vous avez lu toutes les notifications.
1. (Facultatif) Cliquez sur **Afficher tout** pour accéder à la page **Notifications** dans Adobe Experience Cloud.

## Gérer les notifications in-app lors de la demande et de l’octroi d’autorisations

Vous recevez des notifications in-app lorsqu’une personne vous demande ou vous accorde des autorisations pour une vue ou un espace de travail. <!--<span class="preview">or record</span>-->

Pour plus d’informations sur la demande, l’octroi ou le refus d’autorisations, voir [Demander des autorisations pour une vue ou un espace de travail](/help/quicksilver/planning/access/request-permissions.md).

Pour plus d’informations sur la gestion des notifications Workfront Planning, voir [Gérer les préférences de notification Adobe Workfront Planning](/help/quicksilver/planning/notifications/manage-notification-preferences.md).
