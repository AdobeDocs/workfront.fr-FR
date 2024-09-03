---
title: Partager les vues
description: Vous pouvez partager une vue avec d’autres personnes pour travailler en collaboration lors de l’utilisation d’Adobe Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 673dd888-3135-48b0-8198-c8d6d6706ddf
source-git-commit: bffa5992a530761afe57ec62b4cbba2bf03ad1e6
workflow-type: tm+mt
source-wordcount: '1378'
ht-degree: 30%

---


# Partager des vues

{{planning-important-intro}}

Vous pouvez partager une vue avec d’autres personnes pour travailler en collaboration lors de l’utilisation d’enregistrements dans Adobe Workfront Planning.

>[!IMPORTANT]
>
>* L’octroi d’autorisations à un espace de travail ne donne pas à d’autres personnes les autorisations d’accès aux vues sur les pages de type enregistrement. Vous devez accorder des autorisations pour des vues individuelles dans une page de type enregistrement afin de les partager avec d’autres personnes.
>
>* L’octroi d’autorisations à une vue ne modifie pas les autorisations d’affichage des enregistrements. Les autorisations d’enregistrement sont accordées par le partage des espaces de travail.
>
>* Lorsque vous partagez une vue, vous autorisez d’autres personnes à accéder à tous les éléments de la vue. Par exemple, lorsque vous leur accordez les autorisations Gérer pour une vue, ils peuvent modifier l’aspect du regroupement, du filtre, du tri ou de la barre.


Vous pouvez partager une vue avec les entités suivantes :

* En interne, avec les utilisateurs et les groupes Workfront
* Avec les utilisateurs en dehors de Workfront

<!--
This article describes how you can share a view with others. For information about requesting, granting, or denying permissions to a view, see [Request permissions to a view or a workspace](/help/quicksilver/planning/access/request-permissions.md). -->

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès à la planification Workfront.

<!--at GA, check that the Workfront plans article linked below has Planning info-->

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
   <td><p> Standard</p>
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
   <td>  <p>Gérer les autorisations pour une vue</p>  
   <p>Seuls les utilisateurs disposant des autorisations Manage (Gérer) pour un espace de travail peuvent partager une vue publiquement.</p></td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modèle de disposition</p></td> 
   <td> <p>Toutes les personnes, y compris les administrateurs et administratrices de Workfront, doivent se voir attribuer un modèle de mise en page incluant la zone Planning dans le menu principal. </p> </td> 
  </tr> 
</tbody> 
</table>

* Pour plus d’informations sur les exigences d’accès à Workfront, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

<!--OLD: 

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
   <td> <p>Manage permissions to a view</p>  
   <p>Only users with Manage permissions to a workspace can share a view publicly.</p>
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

+++

## Remarques concernant le partage des vues

* Vous pouvez accorder des autorisations d’affichage ou de gestion à une vue aux utilisateurs Workfront internes.

* Les utilisateurs disposant des autorisations de gestion peuvent modifier les paramètres d’affichage, les partager, les dupliquer ou les supprimer.

* Vous pouvez partager des vues avec des personnes en dehors de votre entreprise à l’aide d’un lien public.

* Lorsque vous partagez une vue publiquement, le lien est accessible à toute personne en dehors de votre société pendant une période limitée, indiquée par la date d’expiration. Aucune connexion n’est requise pour afficher la vue partagée.

* Les personnes en dehors de votre organisation qui ont accès à une vue ne peuvent pas créer d’autres vues, modifier la vue partagée, ajouter, supprimer ou modifier des informations d’enregistrement dans la vue.

## Partage des autorisations sur une vue en interne

Vous pouvez partager des vues que vous avez créées ou des vues auxquelles vous disposez des autorisations de gestion avec des utilisateurs ou des groupes dans Workfront.

>[!NOTE]
>
>Les administrateurs et administratrices système ne peuvent pas afficher ou partager des vues qu’ils n’ont pas créées eux-mêmes ou elles-mêmes. Ils ou elles peuvent uniquement accéder à des vues ou partager des vues qui ont été partagées avec eux ou elles.
>
>Les administrateurs et administratrices système peuvent uniquement disposer d’autorisations de gestion sur une vue.

{{step1-to-planning}}

1. Ouvrez l’espace de travail dont vous souhaitez partager la vue, puis cliquez sur une carte de type d’enregistrement.

   La page du type d’enregistrement s’affiche.

1. Dans l’onglet Vue, pointez la souris sur la vue que vous souhaitez partager et cliquez sur le menu **Plus** ![](assets/more-menu.png) à droite du nom de la vue, puis sur **Partager**.

   ![](assets/more-menu-for-views-expanded-with-share-option.png)

   L&#39;onglet **Partage interne** doit être sélectionné par défaut.

1. (Facultatif) Dans la zone **Qui a accès à**, sélectionnez l’une des options suivantes :

   * **Seules les personnes invitées peuvent accéder à** : vous devez spécifier les utilisateurs ou les groupes avec lesquels vous souhaitez partager la vue. Il s’agit de l’option par défaut.
   * **Tous les utilisateurs de l’espace de travail peuvent afficher** : tous les utilisateurs disposant d’autorisations d’affichage ou supérieures sur les espaces de travail peuvent accéder à la vue.

1. Dans le champ **Accorder l’accès à la vue à**, commencez à saisir le nom d’un utilisateur ou d’une utilisatrice, ou d’un groupe, puis cliquez dessus lorsqu’il s’affiche dans la liste.

   ![](assets/sharing-a-view-ui-with-groups.png)

1. Sélectionnez l’un des niveaux d’autorisation suivants dans le menu déroulant :
   * Afficher
   * Gérer

     Pour plus d’informations sur les niveaux d’autorisation et les actions que les utilisateurs et les utilisatrices peuvent effectuer pour chaque niveau, consultez la [Vue d’ensemble des autorisations de partage dans Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).

     Les administrateurs système reçoivent toujours les autorisations Gérer pour les vues partagées avec eux.

1. Cliquez sur **Copier le lien** pour copier un lien vers la vue dans votre presse-papiers.
1. Cliquer sur **Enregistrer**.

   La vue se met à jour avec une icône de personnes ![](assets/view-shared-with-others-people-icon.png) pour indiquer que la vue est désormais partagée avec d’autres utilisateurs.

   >[!TIP]
   >
   >Les vues sans personne ou icône globale sont des vues que vous avez créées et que vous ne partagez pas avec d’autres personnes. Les vues non partagées ne sont visibles que par vous.

1. Partagez le lien copié avec d’autres personnes. Les utilisateurs et utilisatrices qui reçoivent le lien doivent être des utilisateurs et utilisatrices actifs et se connecter à Workfront pour pouvoir accéder à la page du type d’enregistrement et l’afficher dans la vue sélectionnée.

## Partage des autorisations sur une vue publique

Vous pouvez partager les vues que vous avez créées ou celles pour lesquelles vous disposez des autorisations de gestion avec des personnes qui ne disposent pas d’une licence Workfront et qui peuvent être externes à votre entreprise.

>[!IMPORTANT]
>
>Seuls les utilisateurs disposant des autorisations Gérer pour un espace de travail peuvent partager publiquement les vues de l’espace de travail.


Pour partager une vue publiquement dans Workfront Planning :

{{step1-to-planning}}

1. Ouvrez l’espace de travail dont vous souhaitez partager la vue, puis cliquez sur une carte de type d’enregistrement.

   La page du type d’enregistrement s’affiche.

1. Dans l’onglet Vue, pointez la souris sur la vue que vous souhaitez partager et cliquez sur le menu **Plus** ![](assets/more-menu.png) à droite du nom de la vue, puis sur **Partager**.

   ![](assets/more-menu-for-views-expanded-with-share-option.png)

1. Cliquez sur **Partage public**.

   ![](assets/public-sharing-tab-for-views.png)

1. Activez le paramètre **Créer un lien public** .

   Un lien devient disponible. C&#39;est un lien public. Une fois partagé, toute personne disposant du lien, y compris les personnes extérieures à votre entreprise, peut accéder à la page de type d’enregistrement et afficher les enregistrements et les champs sur la page.

1. Cliquez sur l’icône **Copier le lien** ![](assets/copy-link-view.png) pour copier le lien dans le presse-papiers.

1. Saisissez manuellement une date ou utilisez le calendrier dans le champ **Date d’expiration du lien** pour sélectionner une date d’expiration pour le lien public. La page vue de l’enregistrement ne sera pas accessible après la date sélectionnée.

1. Cliquer sur **Enregistrer**.

   La vue se met à jour avec une icône globale ![](assets/public-shared-view-icon-highlighted.png) pour indiquer que la vue est partagée publiquement.

   >[!TIP]
   >
   >Les vues sans personne ou icône globale sont des vues que vous avez créées et que vous ne partagez pas avec d’autres personnes. Les vues non partagées ne sont visibles que par vous.


1. (Facultatif) Collez le lien que vous avez copié dans un email, un message de conversation, un document ou dans un commentaire Workfront pour le partager avec d’autres personnes.

## Octroi d’autorisations à une vue à partir d’une demande d’autorisation

Les utilisateurs qui accèdent à un lien vers une vue pour laquelle ils ne disposent pas d’autorisations peuvent demander des autorisations sur la vue. Tous les utilisateurs disposant des autorisations Gérer pour l’affichage reçoivent la demande d’autorisation et peuvent accorder ou refuser des autorisations.

1. (Conditionnel) Si vous êtes le responsable d’une vue, vous pouvez recevoir une demande d’un autre utilisateur pour accéder à la vue dans les zones suivantes :

   * Une notification in-app
     ![](assets/in-app-notification-for-access-request-for-view.png)
   * Notification par e-mail
     ![](assets/in-app-notification-for-access-request-for-view.png)
1. (Conditionnel) Dans la zone de notification de Workfront, cliquez sur la notification in-app.
Ou
Dans la notification par e-mail, cliquez sur **Afficher toutes les notifications**, puis cliquez sur la notification dans la liste.

   La zone **Demandes d’accès en attente** s’affiche.

   ![](assets/notifications-list-approval-box.png)
1. Sélectionnez l’utilisateur pour lequel vous souhaitez approuver ou refuser l’autorisation, puis cliquez sur **Approuver tout** ou **Refuser tout**.
1. Cliquez sur la flèche pointant vers la gauche de **Demandes d&#39;accès en attente**, puis cliquez sur **Enregistrer**.

   Si vous avez approuvé la requête, les utilisateurs sont ajoutés à la boîte de partage de la vue. L’utilisateur qui demande l’autorisation reçoit une confirmation par email que sa demande a été approuvée. <!--will they also get an in-app notification??-->

## Supprimer les autorisations pour une vue

{{step1-to-planning}}

1. Ouvrez l’espace de travail dont vous souhaitez arrêter le partage, puis cliquez sur une carte de type enregistrement. Cela ouvre la page du type d’enregistrement.
1. Passez la souris sur le nom de l’onglet de la vue à partir de laquelle vous souhaitez supprimer le partage et cliquez sur le menu **Plus** ![](assets/more-menu.png), puis cliquez sur **Partager**.
1. Pour supprimer le partage interne d’une vue, procédez comme suit :

   1. Assurez-vous que l’onglet **Partage interne** est sélectionné.
   1. Recherchez l’utilisateur ou le groupe à supprimer, développez le menu déroulant des autorisations situé à droite du nom de l’utilisateur ou du groupe, puis cliquez sur **Supprimer**.

1. Pour supprimer le partage public d’une vue, procédez comme suit :

   1. Cliquez sur l&#39;onglet **Partage public** .
   1. Désélectionnez l’option **Créer un lien public** .

1. Cliquer sur **Enregistrer**.

   Les personnes n’ont plus accès à la vue. Les utilisateurs qui ont été supprimés de la vue ne reçoivent aucune notification leur indiquant qu’ils ne disposent plus de cet accès.
