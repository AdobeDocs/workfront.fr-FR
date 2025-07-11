---
title: Gérer les notifications par e-mail de planification d’Adobe Workfront
description: Lorsqu’une personne vous identifie ou identifie vos équipes dans un commentaire d’enregistrement dans Adobe Workfront Planning, vous recevez une notification par e-mail concernant cette balise.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 3c505b3a-cda7-4e7b-b497-28b820e9bb8f
source-git-commit: d3d4a923dddb8685a981162918f34447300136cf
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 15%

---


# Gérer les notifications par e-mail d’Adobe Workfront Planning

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Vous pouvez recevoir des notifications par e-mail de Workfront Planning lorsque les scénarios suivants existent :

* Quelqu’un vous identifie ou identifie vos équipes dans un commentaire d’enregistrement.

  Pour plus d’informations sur le balisage d’autres utilisateurs dans un commentaire d’enregistrement, voir [Gérer les commentaires d’enregistrement](/help/quicksilver/planning/records/manage-record-comments.md).
* Quelqu&#39;un vous demande votre autorisation pour accéder à une vue ou à un espace de travail
* Quelqu&#39;un confirme que votre accès a été accordé pour une vue ou un espace de travail <!--Isk confirmed that there is nno email for denying access but did not test-->
* Vous devez soumettre une demande Workfront Planning. Pour plus d’informations, voir [Création et gestion d’un formulaire de demande dans Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md)
* Une personne approuve ou rejette une demande Workfront Planning que vous avez soumise. Pour plus d’informations, voir [Approuver une demande dans Adobe Workfront Planning](/help/quicksilver/planning/requests/approve-request.md)
* Le statut passe à une demande Workfront Planning que vous avez soumise.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès.

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
<p>L’un des plans Workfront suivants :</p> 
<ul><li>Sélectionner</li> 
<li>Principal</li> 
<li>Final</li></ul> 
<p>Workfront Planning n’est pas disponible pour les plans Workfront hérités</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Package Adobe Workfront Planning*</p></td> 
   <td> 
<p>Tous </p> 
<p>Pour plus d’informations sur les éléments inclus dans chaque plan de planification Workfront, contactez votre gestionnaire de compte Workfront. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Plateforme Adobe Workfront</p></td> 
   <td> 
<p>L’instance de Workfront de votre organisation doit être intégrée à l’expérience unifiée Adobe.</p> 
<p>Les utilisateurs et utilisatrices de votre organisation reçoivent des notifications de Workfront Planning uniquement lorsque votre organisation intègre l’expérience unifiée Adobe. </p>
<p>Pour plus d’informations, voir <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience pour Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront*</p></td> 
   <td><p> Standard, Léger ou Contributeur</p>
   <p>Workfront Planning n’est pas disponible pour les licences Workfront héritées</p> 
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
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> 
   <p>In order to receive notifications from Workfront Planning and manage notification preferences, your organization's instance of Workfront must be onboarded to the Adobe Unified Experience. For information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>.</p></td>
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
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configuration</p></td>
   <td> <p>There are no access level controls in Workfront Planning. </p>  
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
-->


## Gérer les notifications par e-mail lorsqu’une personne vous identifie dans un commentaire

1. (Conditionnel et facultatif) Une fois qu’une personne vous a identifié, vous ou votre équipe, dans un commentaire sur un enregistrement, accédez à l’e-mail de notification qui vous informe de la balise et du commentaire. L’expéditeur de l’e-mail est Adobe Experience Cloud.

   ![Exemple de notifications par e-mail](assets/email-notification-example.png)

1. (Facultatif) Cliquez sur le message dans la zone **Workfront** de l’e-mail.

   La page des détails de l’enregistrement s’ouvre dans Workfront. Vous pouvez mettre à jour l’enregistrement ou répondre au commentaire.

1. (Conditionnel) Si disponible, cliquez sur **Afficher toutes les notifications**. <!--check with Lilit - do non-IMS users have this button??-->
La page **Notifications** s’ouvre dans Adobe Experience Cloud. Toutes les notifications de toutes les applications Adobe Experience Cloud s’affichent.

## Gérer les notifications par e-mail lors de la demande et de l’octroi d’autorisations

1. (Conditionnel et facultatif) Lorsqu’une personne vous demande ou vous accorde des autorisations d’accès à une vue ou à un espace de travail, accédez à l’e-mail qui vous informe de la demande d’autorisation. L’expéditeur de l’e-mail est Adobe Experience Cloud.

1. (Facultatif) Cliquez sur le message dans la zone **Workfront** de l’e-mail.

   La page des détails de l’enregistrement s’ouvre dans Workfront. Vous pouvez mettre à jour l’enregistrement ou répondre au commentaire.

1. (Conditionnel) Si disponible, cliquez sur **Afficher toutes les notifications**.
La page **Notifications** s’ouvre dans Adobe Experience Cloud. Toutes les notifications de toutes les applications Adobe Experience Cloud s’affichent.


Pour plus d&#39;informations sur la demande, l&#39;octroi ou le refus d&#39;autorisations pour une vue ou un espace de travail, voir [Demander des autorisations pour une vue ou un espace de travail](/help/quicksilver/planning/access/request-permissions.md).

Pour plus d’informations sur la gestion des notifications Workfront Planning, voir [Gérer les préférences de notification Adobe Workfront Planning](/help/quicksilver/planning/notifications/manage-notification-preferences.md).

## Gérer les notifications par e-mail relatives à la soumission, l’approbation ou le rejet de demandes Workfront Planning

1. (Facultatif) Accédez à l’e-mail que Workfront vous envoie
après la soumission d&#39;une demande ou après qu&#39;une demande que vous avez soumise a été approuvée ou rejetée. L’expéditeur de l’e-mail est Adobe Workfront.

1. (Facultatif) Cliquez sur **Ouvrir la demande**. La demande s’ouvre alors dans Workfront Planning.

1. Cliquez sur l’icône **Notifications** ![Icône de la zone de notifications Unified Shell](assets/notifications-area-icon-unified-shell.png) dans le coin supérieur droit de l’écran pour accéder à la page **Notifications**.

   Pour plus d’informations sur la gestion des notifications Workfront Planning, voir [Gérer les préférences de notification Adobe Workfront Planning](/help/quicksilver/planning/notifications/manage-notification-preferences.md).
