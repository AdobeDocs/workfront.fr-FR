---
title: Partage des espaces de travail
description: Vous pouvez partager un espace de travail avec d’autres personnes pour travailler en collaboration dans Adobe Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: bffa5992a530761afe57ec62b4cbba2bf03ad1e6
workflow-type: tm+mt
source-wordcount: '668'
ht-degree: 58%

---


# Partager des espaces de travail

{{planning-important-intro}}

Vous pouvez partager un espace de travail avec d’autres personnes pour travailler en collaboration dans Adobe Workfront Planning.

<!--
This article describes how you can share a view with others. For information about requesting, granting, or denying permissions to a view, see [Request permissions to a view or a workspace](/help/quicksilver/planning/access/request-permissions.md). -->

>[!NOTE]
>
>L’octroi d’autorisations à un espace de travail ne donne pas à d’autres personnes les autorisations d’accès aux vues sur les pages de type enregistrement. Vous devez accorder des autorisations pour des vues individuelles dans une page de type d’enregistrement afin de les partager avec d’autres personnes. Pour plus d’informations, consultez la section [Partager une vue](/help/quicksilver/planning/access/share-views.md).


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
   <td role="rowheader"><p>Forfait Adobe Workfront*</p></td> 
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
<p>N’importe quelle </p> 
<p>Pour plus d’informations sur les éléments inclus dans chaque plan de planification Workfront, voir <a href="https://business.adobe.com/products/workfront/pricing.html">Prix et package Adobe Workfront</a>. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Plateforme Adobe Workfront</p></td> 
   <td> 
<p>L’instance de Workfront de votre entreprise doit être intégrée à l’expérience unifiée Adobe pour pouvoir accéder à toutes les fonctionnalités de la planification Workfront.</p> 
<p>Pour plus d’informations, voir <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience pour Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront*</p></td> 
   <td><p> Standard </p>
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
   <td>  <p>Gérer les autorisations d’un espace de travail</p>  </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modèle de disposition</p></td> 
   <td> <p>Toutes les personnes, y compris les administrateurs et administratrices de Workfront, doivent se voir attribuer un modèle de mise en page incluant la zone Planning dans le menu principal. </p> </td> 
  </tr> 
</tbody> 
</table>

* Pour plus d’informations sur les exigences d’accès à Workfront, consultez les [Conditions d’accès requises dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
   <p> Adobe Workfront</p> </td>
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
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p>
   Or
   <p>Current: Plan </p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> There are no access controls for Adobe Workfront Planning</p>  
</td>
  </tr>

  <tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Planning area in the Main Menu. </p> <p>For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p> 
</td>
  </tr>
 </tbody>
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).-->



## Autorisations de partage d’un espace de travail

Les personnes suivantes peuvent partager un espace de travail avec d’autres personnes :

* L’équipe d’administration système peut partager tous les espaces de travail, y compris ceux qu’elle n’a pas créés.
* Les autres personnes ne peuvent partager que les espaces de travail pour lesquels elles disposent d’autorisations de gestion.

Pour partager un espace de travail avec d’autres personnes, procédez comme suit :

{{step1-to-planning}}

1. Ouvrez l’espace de travail à partager, puis cliquez sur **Partager** dans le coin supérieur droit de l’écran.

   ![](assets/share-button-on-workspace-top-right.png)

1. Dans le champ **Accorder un accès à l’espace de travail à**, commencez à saisir le nom d’une personne ou d’un groupe, puis cliquez dessus lorsqu’il s’affiche dans la liste.

   ![](assets/sharing-ui-with-groups.png)

1. Sélectionnez l’un des niveaux d’autorisation suivants dans le menu déroulant :
   * Afficher
   * Contribuer
   * Gérer

     Pour plus d’informations sur les niveaux d’autorisation et les actions que les utilisateurs et les utilisatrices peuvent effectuer pour chaque niveau, consultez la [Vue d’ensemble des autorisations de partage dans Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).
1. Cliquez sur **Copier le lien** pour copier un lien vers l’espace de travail dans le presse-papiers.
1. Partagez le lien copié avec d’autres personnes. Les personnes qui reçoivent le lien doivent être des personnes actives et se connecter à Workfront pour pouvoir accéder à l’espace de travail.
1. Cliquer sur **Enregistrer**.

## Octroi d’autorisations à un espace de travail à partir d’une demande d’autorisation

Les utilisateurs qui accèdent à un lien vers un espace de travail auquel ils ne sont pas autorisés peuvent demander des autorisations sur l’espace de travail. Tous les utilisateurs disposant des autorisations Manage (Gérer) pour l’espace de travail reçoivent la demande d’autorisation et peuvent accorder ou refuser des autorisations.

1. (Conditionnel) Si vous êtes le responsable d’un espace de travail, vous pouvez recevoir une demande d’un autre utilisateur pour accéder à la vue dans les zones suivantes :

   * Une notification in-app
     ![](assets/in-app-notification-for-access-request.png)
   * Une notification électronique
     ![](assets/email-notification-for-access-request.png)
1. (Conditionnel) Dans la zone de notification de Workfront, cliquez sur la notification in-app.
Ou
Dans la notification par e-mail, cliquez sur **Afficher toutes les notifications**, puis cliquez sur la notification dans la liste.

   La zone **Demandes d’accès en attente** s’affiche.

   ![](assets/notifications-list-approval-box.png)
1. Sélectionnez l’utilisateur pour lequel vous souhaitez approuver ou refuser l’autorisation, puis cliquez sur **Approuver tout** ou **Refuser tout**.
1. Cliquez sur la flèche pointant vers la gauche de **Demandes d&#39;accès en attente**, puis cliquez sur **Enregistrer**.

   Si vous avez approuvé la requête, les utilisateurs sont ajoutés à la boîte de partage de l’espace de travail. L’utilisateur qui demande l’autorisation reçoit une confirmation par email que sa demande a été approuvée. <!--will they also get an in-app notification??-->


## Supprimer des autorisations d’un espace de travail


{{step1-to-planning}}

1. Ouvrez l’espace de travail pour lequel vous souhaitez supprimer des autorisations, puis cliquez sur **Partager** dans le coin supérieur droit de l’écran.
1. Cliquez sur le menu déroulant situé à droite du nom d’une personne ou d’un groupe, puis cliquez sur **Supprimer**.
1. Cliquer sur **Enregistrer**.

   La ou les personnes appartenant au groupe supprimé n’ont plus accès à l’espace de travail ou à ses objets.