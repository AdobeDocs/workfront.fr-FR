---
title: Gérer les préférences de notification d’Adobe Workfront Planning
description: Vous pouvez peut-être gérer vos préférences de notification pour Adobe Workfront Planning. Cet article décrit comment configurer vos préférences de notifications.
author: Alina
feature: Workfront Planning
role: User
recommendations: noDisplay, noCatalog
exl-id: ec549a61-095c-433f-80e2-1be5c0a05180
source-git-commit: d3d4a923dddb8685a981162918f34447300136cf
workflow-type: tm+mt
source-wordcount: '519'
ht-degree: 23%

---


# Gérer les préférences de notification d’Adobe Workfront Planning

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Vous pouvez recevoir une notification in-app ou par e-mail lorsque les actions suivantes se produisent dans Workfront Planning :

* Quelqu’un vous ajoute, vous ou vos équipes, à un commentaire sur la page d’enregistrement
* Quelqu&#39;un demande l&#39;autorisation d&#39;accéder à une vue ou à un espace de travail
* Quelqu&#39;un vous accorde l&#39;autorisation d&#39;accéder à une vue ou à un espace de travail <!--I could not test this but Isk confirmed-->
* Vous devez soumettre une demande Workfront Planning.
* Une personne approuve ou rejette une demande Workfront Planning que vous avez soumise.
* Le statut passe à une demande Workfront Planning que vous avez soumise.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès.

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
   <td><p><p>Standard, Léger ou Contributeur
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

Pour plus d’informations sur les notifications de Workfront Planning, consultez également les articles suivants :

* Pour plus d’informations sur les commentaires des enregistrements, voir [Gérer les commentaires des enregistrements](/help/quicksilver/planning/records/manage-record-comments.md).
* Pour plus d’informations sur les notifications in-app depuis Workfront Planning, voir [Gérer les notifications in-app pour Adobe Workfront Planning](/help/quicksilver/planning/notifications/manage-planning-in-app-notifications.md).
* Pour plus d’informations sur les notifications par e-mail provenant de Workfront Planning, voir [Gérer les notifications par e-mail pour Adobe Workfront Planning](/help/quicksilver/planning/notifications/manage-planning-email-notifications.md).


## Gérer les préférences de notification

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

   Pour plus d’informations sur la gestion des notifications, voir [ Préférences du compte et notifications ](https://experienceleague.adobe.com/en/docs/core-services/interface/features/account-preferences).

<!--OLD: notifications are not available to non-IMS customers: 

When someone adds you to a comment in the record page, you may receive an in-app as well as an email notification about the comment. 

The following scenarios exist:   

* Adobe Unified Experience customers receive both an in-app notification and an email notification. They can manage their in-app and email notification preferences in the Preferences area of their Adobe Experience Cloud profile for the Workfront product. 

    For more information, see [Account preferences and notifications](https://experienceleague.adobe.com/en/docs/core-services/interface/features/account-preferences).

* Customers who are not on the Adobe Unified Experience receive only an email notification. They cannot manage their email notifications preferences and will always receive an email when someone adds them to a comment on a record in Workfront Planning.   

-->
