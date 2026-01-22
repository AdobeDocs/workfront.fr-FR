---
title: Partager les vues
description: Vous pouvez partager une vue avec d’autres personnes pour travailler en collaboration lors de l’utilisation d’Adobe Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 673dd888-3135-48b0-8198-c8d6d6706ddf
source-git-commit: 54a6e633e903c73a78b36e90fb27edb445dc8d47
workflow-type: tm+mt
source-wordcount: '1946'
ht-degree: 16%

---


# Partager des vues

<!--there are several mentions on how to share public links for global record types in secondary workspaces in this articel; you have to update all of these mentions when something changes-->

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de manière générale. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Après les versions mensuelles en production, les mêmes fonctionnalités sont également disponibles dans l’environnement de production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation des versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

Vous pouvez partager une vue avec d’autres personnes pour travailler en collaboration lors de l’utilisation d’enregistrements dans Adobe Workfront Planning.

>[!IMPORTANT]
>
>* L’octroi d’autorisations à un espace de travail ne donne pas à d’autres personnes les autorisations d’accès aux vues sur les pages de type enregistrement. Vous devez accorder des autorisations pour des vues individuelles dans une page de type enregistrement afin de les partager avec d’autres personnes.
>
>* Accorder des autorisations à une vue ne modifie pas les autorisations d&#39;affichage des enregistrements. Les autorisations d’enregistrement sont accordées en partageant les espaces de travail.
>
>* Lorsque vous partagez une vue, vous autorisez d’autres utilisateurs à accéder à tous les éléments de la vue. Par exemple, lorsque vous leur donnez des autorisations de niveau Gérer pour une vue, ils peuvent modifier l’aspect du regroupement, du filtre, du tri ou de la barre.


<!--
This article describes how you can share a view with others. For information about requesting, granting, or denying permissions to a view, see [Request permissions to a view or a workspace](/help/quicksilver/planning/access/request-permissions.md). -->

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article. 

<!--at GA, check that the Workfront plans article linked below has Planning info-->

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
   <td role="rowheader"><p>Package Adobe Workfront</p></td> 
   <td> 
<p>Tout package Workfront and Planning</p> 
Ou
<p>Tout package Workflow et Planning</p> 
 </tr>

<tr> 
   <td role="rowheader"><p>Licence Adobe Workfront</p></td> 
   <td><p>Tous</p> 
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
   <p><b>IMPORTANT</b></p> 
   <p>Seuls les utilisateurs disposant d’autorisations de niveau Gérer pour un espace de travail peuvent partager une vue publiquement.</p></td> 
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
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>Your organization must be onboarded to the Adobe Unified Experience for users to be able to request and grant permissions to a view from a permission request. </p>
<p>Users must be added to the Adobe Admin Console in order to gain permissions to Workfront Planning views.</p>
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard</p>
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
   <td>  <p>Manage permissions to a view</p>  
   <p>Only users with Manage permissions to a workspace can share a view publicly.</p></td> 
  </tr> 

</tbody> 
</table> -->

## Remarques concernant le partage de vues

* Vous pouvez partager une vue des manières suivantes :

   * En interne, avec les utilisateurs, les groupes, les équipes, les entreprises et les fonctions de Workfront
   * Publiquement, avec des utilisateurs en dehors de Workfront
   * En copiant puis en partageant un lien vers une vue
   * En l’exportant vers un fichier Excel ou CSV. Vous ne pouvez exporter que la vue Tableau vers un fichier. Pour plus d’informations, consultez la section [Gérer la vue en tableau](/help/quicksilver/planning/views/manage-the-table-view.md).

* Pour obtenir des informations générales sur le partage d’objets dans Workfront Planning, consultez également la section [Présentation des autorisations de partage dans Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).
* Vous pouvez accorder des autorisations d’affichage ou de gestion pour un affichage aux utilisateurs Workfront internes.

* Les utilisateurs disposant d’autorisations de niveau Gérer peuvent modifier les paramètres d’affichage, les partager, les dupliquer ou les supprimer.

* Vous pouvez partager des vues avec des personnes extérieures à votre organisation via un lien public.

* Lorsque vous partagez une vue publiquement, le lien est accessible par toute personne extérieure à votre entreprise pendant une durée limitée, indiquée par la date d’expiration. Aucune connexion n’est requise pour afficher la vue partagée.

  >[!NOTE]
  >
  >Vous ne pouvez pas partager une vue publiquement à partir d’un type d’enregistrement global dans un espace de travail secondaire. Pour plus d’informations, voir [Ajouter des types d’enregistrements existants depuis un autre espace de travail](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md).


* Les personnes extérieures à votre organisation qui ont accès à une vue ne peuvent pas créer d&#39;autres vues, modifier la vue partagée ou ajouter, supprimer ou modifier des informations d&#39;enregistrement dans la vue.

## Partage des autorisations pour une vue en interne

Vous pouvez partager des vues que vous avez créées ou pour lesquelles vous disposez d&#39;autorisations de niveau Gérer avec des utilisateurs, des groupes, des équipes, des sociétés et des fonctions dans Workfront Planning.

>[!NOTE]
>
>Les administrateurs et administratrices système ne peuvent pas afficher ou partager des vues qu’ils n’ont pas créées eux-mêmes ou elles-mêmes. Ils ou elles peuvent uniquement accéder à des vues ou partager des vues qui ont été partagées avec eux ou elles.
>
>Les administrateurs et administratrices système peuvent uniquement disposer d’autorisations de gestion sur une vue.

{{step1-to-planning}}

1. Ouvrez l’espace de travail dont vous souhaitez partager la vue, puis cliquez sur une carte de type d’enregistrement.

   La page du type d’enregistrement s’affiche.

1. Dans l’onglet de la vue, effectuez l’une des opérations suivantes :

   * Cliquez sur l’onglet de la vue, survolez la vue avec la souris dans le menu déroulant, cliquez sur le menu **Plus** ![Menu Plus](assets/more-menu.png), puis cliquez sur **Partager**.

     ![Menu Plus d’une vue](assets/more-menu-for-views-expanded-with-share-option.png)

   * Cliquez sur **Partager** dans le coin supérieur droit de l&#39;écran, puis **Partager l&#39;affichage actuel**.

     ![Bouton Partager avec type d’enregistrement et options de partage d’affichage](assets/share-button-with-record-type-and-view-sharing-options.png)

   La boîte de dialogue **Partager la vue** s’ouvre et l’onglet **Partage interne** doit être sélectionné par défaut.

1. (Facultatif) Dans la zone **Qui a accès**, sélectionnez l’une des options suivantes :

   * **Seules les personnes invitées peuvent y accéder** : vous devez spécifier les utilisateurs, les groupes, l&#39;équipe, l&#39;entreprise ou la fonction avec lesquels vous souhaitez partager la vue. Il s’agit de l’option par défaut.

   >[!NOTE]
   >
   >* Outre les équipes, les groupes, les entreprises et les fonctions, vous ne pouvez partager qu’avec des utilisateurs qui ont été ajoutés au Adobe Admin Console. Vous ne pouvez pas ajouter des utilisateurs Workfront uniquement. Pour plus d’informations, voir [Gestion des utilisateurs dans Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).
   >
   >* Lorsque vous partagez une vue avec un utilisateur, sa fonction principale <span class="preview">et son adresse e-mail</span> s’affichent également dans le champ. Le paramètre Afficher les informations de contact doit être activé pour que l’objet Utilisateurs de votre niveau d’accès puisse voir l’e-mail de l’utilisateur.


   * **Tout le monde dans l’espace de travail peut afficher** : tous les utilisateurs disposant d’autorisations d’affichage ou supérieures dans les espaces de travail peuvent accéder à l’affichage.

1. Dans le champ **Accorder l’accès à cette vue**, commencez à saisir le nom d’un utilisateur, d’un groupe, d’une équipe, d’une entreprise ou d’une fonction, puis cliquez dessus lorsqu’il s’affiche dans la liste.

   ![Partage d’une vue avec des groupes](assets/sharing-a-view-ui-with-groups.png)

1. Sélectionnez l’un des niveaux d’autorisation suivants dans le menu déroulant :
   * Afficher
   * Gérer

     Pour plus d’informations sur les niveaux d’autorisation et les actions que les utilisateurs et les utilisatrices peuvent effectuer pour chaque niveau, consultez la [Vue d’ensemble des autorisations de partage dans Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).

     Les administrateurs système reçoivent toujours des autorisations de niveau Gérer pour les vues partagées avec eux.

1. Cliquer sur **Enregistrer**.

   L’affichage est mis à jour avec une icône de personnes ![Affichage partagé avec d’autres](assets/view-shared-with-others-people-icon.png) pour indiquer que l’affichage est désormais partagé avec d’autres utilisateurs.

   Les utilisateurs avec lesquels vous avez partagé la vue reçoivent à la fois une notification in-app et une notification par e-mail concernant leurs autorisations pour cette vue.

   >[!TIP]
   >
   >Les vues sans peuple ou sans icône globale sont des vues que vous avez créées et ne sont pas partagées avec d&#39;autres personnes. Les vues non partagées ne sont visibles que par vous.

1. Partagez le lien copié avec d’autres personnes. Les utilisateurs et utilisatrices qui reçoivent le lien doivent être des utilisateurs et utilisatrices actifs et se connecter à Workfront pour pouvoir accéder à la page du type d’enregistrement et l’afficher dans la vue sélectionnée.

## Partager les autorisations d’accès à une vue publiquement

Vous pouvez partager des vues que vous avez créées ou pour lesquelles vous disposez d’autorisations de niveau Gérer avec des personnes qui ne disposent pas d’une licence Workfront et qui sont susceptibles d’être externes à votre organisation.

Vous ne pouvez pas partager une vue publiquement à partir d’un type d’enregistrement global dans son espace de travail secondaire.

>[!IMPORTANT]
>
>Seuls les utilisateurs disposant d’autorisations de niveau Gérer pour un espace de travail peuvent partager publiquement les vues de l’espace de travail.


Pour partager une vue publiquement dans Workfront Planning :

{{step1-to-planning}}

1. Ouvrez l’espace de travail dont vous souhaitez partager la vue, puis cliquez sur une carte de type d’enregistrement.

   La page du type d’enregistrement s’affiche.

1. Dans l’onglet Affichage , effectuez l’une des opérations suivantes :

   * Pointez sur le nom de l’onglet de la vue à partager et cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) à droite du nom de la vue, puis cliquez sur **Partager**.

   ![Menu Plus pour les vues développées avec l’option de partage](assets/more-menu-for-views-expanded-with-share-option.png)
   * Cliquez sur **Partager** > **Partager la vue actuelle**

   La boîte de dialogue **Partager la vue** s’ouvre.

1. Cliquez sur **Partage public**.

   ![Onglet Partage public pour les vues](assets/public-sharing-tab-for-views.png)

1. Activez le paramètre **Créer un lien public**.

   Un lien devient disponible. Il s’agit d’un lien public. Lors du partage, toute personne disposant du lien, y compris des personnes extérieures à votre organisation, peut accéder à la page de type d’enregistrement et afficher les enregistrements et les champs de la page.

   >[!TIP]
   >
   >L’onglet **Partage public** est supprimé pour un type d’enregistrement global dans son espace de travail secondaire.


1. Cliquez sur l’icône **Copier le lien** ![Copier la vue du lien](assets/copy-link-view.png) pour copier le lien dans le presse-papiers.

1. Saisissez manuellement une date ou utilisez le calendrier dans le champ **Date d’expiration du lien** pour sélectionner une date d’expiration pour le lien public. La page d’enregistrement vue ne sera pas accessible après la date sélectionnée.

1. Cliquer sur **Enregistrer**.

   L’affichage est mis à jour avec une icône globale ![icône d’affichage partagé public mise en surbrillance](assets/public-shared-view-icon-highlighted.png) pour indiquer que l’affichage est partagé publiquement.

   >[!TIP]
   >
   >Les vues sans peuple ou sans icône globale sont des vues que vous avez créées et ne sont pas partagées avec d&#39;autres personnes. Les vues non partagées ne sont visibles que par vous.


1. (Facultatif) Collez le lien que vous avez copié dans un e-mail, un message de conversation, un document ou un commentaire Workfront pour le partager avec d’autres personnes.

## Copier un lien vers une vue

Vous pouvez copier un lien vers une vue dans le presse-papiers et l’inclure dans une autre application ou le partager avec d’autres utilisateurs.

Pour copier un lien vers une vue partagée publiquement, reportez-vous à la section [Partager les autorisations d&#39;une vue partagée publiquement](#share-permissions-to-a-view-publicly) dans cet article.

Cette section décrit comment partager une vue en interne.

>[!IMPORTANT]
>
>Tout d’abord, vous devez partager la vue avec les utilisateurs et utilisatrices avant de partager le lien vers la vue pour qu’ils ou elles puissent l’afficher.


{{step1-to-planning}}

1. Ouvrez l’espace de travail dont vous souhaitez copier la vue et partager le lien vers, puis cliquez sur une carte de type d’enregistrement.

   Cela ouvre la page du type d’enregistrement.

1. Dans l’onglet d’une vue, effectuez l’une des opérations suivantes :

   * Pointez sur l’onglet de la vue à partager et cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) à droite du nom de la vue, puis cliquez sur **Partager** > **Copier le lien** dans la zone **Partager la vue**.
   * Cliquez sur **Partager** > **Copier le lien d’affichage** à partir de la page du type d’enregistrement.

   Un lien vers la vue est copié dans le presse-papiers et vous recevez une confirmation en bas de l’écran.

   Vous pouvez maintenant coller le lien vers une autre application ou l&#39;envoyer à d&#39;autres.

## Octroi d’autorisations pour une vue à partir d’une demande d’autorisation

Les utilisateurs et utilisatrices qui accèdent à un lien vers une vue pour laquelle ils ne disposent pas d’autorisations peuvent demander des autorisations pour la vue. Tous les utilisateurs disposant d’autorisations de niveau Gérer pour l’affichage reçoivent la demande d’autorisation et peuvent accorder ou refuser les autorisations.

1. (Conditionnel) Si vous êtes le responsable d&#39;une vue, il se peut que vous receviez une demande d&#39;un autre utilisateur pour accéder à la vue dans les domaines suivants :

   * Une notification in-app
     ![&#x200B; Notification in-app pour la demande d’accès à la vue &#x200B;](assets/in-app-notification-for-access-request-for-view.png)
   * Notification par e-mail
     ![&#x200B; Notification in-app pour la demande d’accès à la vue &#x200B;](assets/in-app-notification-for-access-request-for-view.png)
1. (Conditionnel) Dans la zone de notification de Workfront, cliquez sur la notification in-app
Ou
Dans la notification par e-mail, cliquez sur **Afficher toutes les notifications**, puis cliquez sur la notification dans la liste.

   La zone **Demandes d’accès en attente** s’affiche.

   ![Zone de validation de la liste des notifications](assets/notifications-list-approval-box.png)
1. (Facultatif) Pour l’utilisateur dont vous souhaitez approuver les autorisations, sélectionnez l’une des options suivantes dans le menu déroulant situé à droite du nom de l’utilisateur :
   * **Afficher**
   * **Gérer**
1. Sélectionnez l’utilisateur pour lequel vous souhaitez approuver ou refuser l’autorisation, puis cliquez sur **Approuver tout** ou **Tout refuser**.
1. Cliquez sur la flèche pointant vers la gauche de **Demandes d’accès en attente**, puis cliquez sur **Enregistrer**.

   Si vous avez approuvé la demande, les utilisateurs sont ajoutés à la zone de partage de la vue. L’utilisateur demandant l’autorisation reçoit un courrier électronique de confirmation confirmant que sa demande a été approuvée. <!--will they also get an in-app notification??-->

## Supprimer les autorisations pour une vue

{{step1-to-planning}}

1. Ouvrez l’espace de travail dont vous souhaitez arrêter le partage de la vue, puis cliquez sur une carte de type d’enregistrement. Cela ouvre la page du type d’enregistrement.
1. Dans l’onglet Affichage , effectuez l’une des opérations suivantes :

   * Pointez sur le nom de l’onglet de la vue à partager et cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) à droite du nom de la vue, puis cliquez sur **Partager**.

   * Cliquez sur **Partager** > **Partager la vue actuelle**

   La boîte de dialogue **Partager la vue** s’ouvre.
1. Pour supprimer le partage interne d’une vue, procédez comme suit :

   1. Assurez-vous que l’onglet **Partage interne** est sélectionné.
   1. Recherchez l’utilisateur, le groupe, l’équipe, l’entreprise ou la fonction à supprimer, développez le menu déroulant des autorisations à droite du nom de l’entité avec laquelle vous partagez la vue, puis cliquez sur **Supprimer**.

1. Pour supprimer le partage public d’une vue, procédez comme suit :

   1. Cliquez sur l’onglet **Partage public**.
   1. Désélectionnez l’option **Créer un lien public**.

1. Cliquer sur **Enregistrer**.

   Les gens n&#39;ont plus accès à la vue. Les utilisateurs qui ont été supprimés de l’accès à l’affichage ne sont pas avertis qu’ils ne disposent plus de cet accès.
