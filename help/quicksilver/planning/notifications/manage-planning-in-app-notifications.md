---
title: Gestion des notifications in-app de la planification Adobe Workfront
description: Lorsqu’une personne vous balise dans un commentaire d’enregistrement, vous recevez une notification par courrier électronique pour cette balise.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: a6eb8c7c-a34d-4c84-a45c-7e7f050a4302
source-git-commit: bd202821687453288c96147933331c8a7a6b3acb
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 23%

---


# Gérer les notifications in-app d’Adobe Workfront Planning

{{planning-important-intro}}

Vous pouvez recevoir des notifications in-app de la planification Workfront lorsque les scénarios suivants se présentent :

* Quelqu&#39;un vous marquera dans un commentaire d&#39;enregistrement

  Pour plus d’informations sur le balisage des autres dans un commentaire d’enregistrement, voir [Gestion des commentaires d’enregistrement](/help/quicksilver/planning/records/manage-record-comments.md).
* Une personne demande votre autorisation d’accéder à une vue ou à un espace de travail.
* Quelqu&#39;un confirme que votre accès a été accordé pour une vue ou un espace de travail <!--Isk confirmed there is no notification for denying permissions - did not test-->

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès à la planification Workfront.

Pour pouvoir accéder à Workfront Planning, vous devez disposer des éléments suivants :

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
<p>L’instance Workfront de votre entreprise doit être intégrée à l’expérience unifiée Adobe.</p> 
<p>Les utilisateurs de votre entreprise ne reçoivent des notifications de Workfront Planning que lorsque votre entreprise est intégrée à l’expérience unifiée Adobe. </p>
<p>Pour plus d’informations, voir <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience pour Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront*</p></td> 
   <td><p> Standard, Clair ou Contributeur</p>
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
   <p>L’administration système a accès à tous les espaces de travail, y compris ceux qu’elle n’a pas créés.</p>  </td> 
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

+++ Expand to view access requirements for Workfront Planning. 

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
   <p>In order to receive notifications from Workfront Planning, your organization's instance of Workfront must be onboarded to the Adobe Unified Experience. For information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>.</p></td>
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

+++
-->

## Gestion des notifications in-app lorsqu’un utilisateur vous balise dans un commentaire

1. (Conditionnel) Après qu’un utilisateur vous ait marqué dans un commentaire sur un enregistrement, accédez à l’icône **Notifications** in-app ![](assets/experience-cloud-notifications-icon.png) dans Adobe Experience Cloud.

   ![](assets/in-app-notification-example.png)

1. Cliquez sur la notification.

   La page des détails de l’enregistrement s’ouvre dans Workfront Planning. Vous pouvez mettre à jour l’enregistrement ou répondre au commentaire.

1. (Facultatif) Cliquez sur **Tout marquer comme lu** pour indiquer que vous avez lu toutes les notifications.
1. (Facultatif) Cliquez sur **Afficher tout** pour accéder à la page **Notifications** dans Adobe Experience Cloud.

## Gérer les notifications in-app lors de la demande et de l’octroi des autorisations

Vous recevez des notifications in-app lorsqu’une personne vous demande ou vous accorde des autorisations pour une vue ou un espace de travail.

Pour plus d’informations sur la demande, l’octroi ou le refus d’accès à une vue ou à un espace de travail, voir [Demande d’accès à une vue ou à un espace de travail](/help/quicksilver/planning/access/request-permissions.md).

Pour plus d’informations sur la gestion de vos notifications Workfront Planning, voir [Gestion des préférences de notification Adobe Workfront Planning](/help/quicksilver/planning/notifications/manage-notification-preferences.md).