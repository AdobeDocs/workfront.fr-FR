---
title: Partager les espaces de travail
description: Vous pouvez partager un espace de travail avec d’autres personnes pour travailler en collaboration dans Adobe Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 475a519d-d3bd-4461-8099-0e296d556d34
source-git-commit: 58d2bf9f14b9a3adf4bacfad58f1b9862aeaf247
workflow-type: tm+mt
source-wordcount: '908'
ht-degree: 35%

---

# Partager des espaces de travail

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Vous pouvez partager un espace de travail avec d’autres personnes pour travailler en collaboration dans Adobe Workfront Planning.

<!--
This article describes how you can share a view with others. For information about requesting, granting, or denying permissions to a view, see [Request permissions to a view or a workspace](/help/quicksilver/planning/access/request-permissions.md). -->

>[!NOTE]
>
>L’octroi d’autorisations à un espace de travail ne donne pas à d’autres personnes les autorisations d’accès aux vues sur les pages de type enregistrement. Vous devez accorder des autorisations pour des vues individuelles dans une page de type enregistrement afin de les partager avec d’autres personnes. Pour plus d’informations, consultez la section [Partager une vue](/help/quicksilver/planning/access/share-views.md).


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
<p>L’instance de Workfront de votre organisation doit être intégrée à l’expérience unifiée Adobe pour pouvoir accéder à Workfront Planning.</p>
<p>Votre organisation doit être intégrée à l’expérience unifiée Adobe pour que les utilisateurs puissent demander et accorder des autorisations à un espace de travail à partir d’une demande d’autorisation. </p> 
<p>Les utilisateurs doivent être ajoutés au Adobe Admin Console pour obtenir des autorisations sur les espaces de travail Workfront Planning.</p>
<p>Pour plus d’informations, voir <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience pour Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront*</p></td> 
   <td><p> Standard </p>
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
   <td>  <p>Gérer les autorisations d’un espace de travail</p>  </td> 
  </tr>

</tbody> 
</table>

* Pour plus d’informations sur les exigences d’accès à Workfront, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considérations relatives au partage d’espaces de travail

* Pour obtenir des informations générales sur le partage d’objets dans Workfront Planning, consultez également la section [Présentation des autorisations de partage dans Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).
* Vous pouvez partager des espaces de travail avec des utilisateurs, des équipes, des rôles, des groupes ou des entreprises de votre organisation.
* Outre les équipes, les groupes, les entreprises et les fonctions, vous ne pouvez partager qu’avec des utilisateurs qui ont été ajoutés au Adobe Admin Console.
* Vous ne pouvez pas partager des espaces de travail avec des utilisateurs en dehors de votre organisation.
* Lorsque vous partagez un espace de travail, tous les types d’enregistrements, les enregistrements et les champs associés aux espaces de travail sont également partagés.
* Lorsque vous partagez un espace de travail, les vues ne sont pas partagées. Vous devez partager les vues séparément.
* Les autorisations Workspace s’affichent sous la forme d’autorisations héritées sur les types d’enregistrements.

## Autorisations de partage d’un espace de travail

Les personnes suivantes peuvent partager un espace de travail avec d’autres personnes :

* Les administrateurs et administratrices système peuvent partager tous les espaces de travail, y compris ceux qu’ils n’ont pas créés.
* Les autres personnes ne peuvent partager que les espaces de travail pour lesquels elles disposent d’autorisations de gestion.

Pour partager un espace de travail avec d’autres personnes, procédez comme suit :

{{step1-to-planning}}

1. Ouvrez l’espace de travail à partager, puis cliquez sur **Partager** dans le coin supérieur droit de l’écran.

   ![Bouton Partager dans l’espace de travail en haut à droite](assets/share-button-on-workspace-top-right.png)

1. Dans le champ **Accorder l’accès à cet espace de travail**, commencez à saisir le nom d’un utilisateur, d’un groupe, d’une équipe, d’une entreprise ou d’une fonction, puis cliquez dessus lorsqu’il s’affiche dans la liste.

   ![Partager l’interface utilisateur avec des groupes](assets/sharing-ui-with-groups.png)

   >[!NOTE]
   >
   >   Outre les équipes, les groupes, les entreprises et les fonctions, vous ne pouvez partager qu’avec des utilisateurs qui ont été ajoutés au Adobe Admin Console. Vous ne pouvez pas ajouter des utilisateurs Workfront uniquement. Pour plus d’informations, voir [Gestion des utilisateurs dans Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).


1. Sélectionnez l’un des niveaux d’autorisation suivants dans le menu déroulant :
   * Afficher
   * Contribuer
   * Gérer

     Pour plus d’informations sur les niveaux d’autorisation et les actions que les utilisateurs et les utilisatrices peuvent effectuer pour chaque niveau, consultez la [Vue d’ensemble des autorisations de partage dans Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).
1. Cliquez sur **Copier le lien** pour copier un lien vers l’espace de travail dans le presse-papiers.
1. Partagez le lien copié avec d’autres personnes. Les personnes qui reçoivent le lien doivent être des utilisateurs et utilisatrices actifs et se connecter à Workfront pour pouvoir accéder à l’espace de travail.
1. Cliquer sur **Enregistrer**.

   Les utilisateurs avec lesquels vous avez partagé l’espace de travail reçoivent une notification in-app et par e-mail concernant leurs autorisations.

## Octroyer des autorisations à un espace de travail à partir d’une demande d’autorisation

Les utilisateurs et utilisatrices qui accèdent à un lien vers un espace de travail pour lequel ils ne disposent pas d’autorisations peuvent demander des autorisations pour l’espace de travail . Tous les utilisateurs disposant d’autorisations de niveau Gérer pour l’espace de travail reçoivent la demande d’autorisation et peuvent accorder ou refuser les autorisations.

1. (Conditionnel) Si vous êtes le responsable d&#39;un espace de travail, il se peut que vous receviez une demande d&#39;un autre utilisateur pour accéder à la vue dans les zones suivantes :

   * Une notification in-app

     ![Notification in-app pour la demande d’accès](assets/in-app-notification-for-access-request.png)
   * Notification par e-mail

     ![Notification électronique pour la demande d’accès](assets/email-notification-for-access-request.png)
1. (Conditionnel) Dans la zone de notification de Workfront, cliquez sur la notification in-app
Ou
Dans la notification par e-mail, cliquez sur **Afficher toutes les notifications**, puis cliquez sur la notification dans la liste.

   La zone **Demandes d’accès en attente** s’affiche.

   ![Zone de validation de la liste des notifications](assets/notifications-list-approval-box.png)

1. (Facultatif) Pour l’utilisateur dont vous souhaitez approuver les autorisations, sélectionnez l’une des options suivantes dans le menu déroulant situé à droite du nom de l’utilisateur :
   * **Afficher**
   * **Contribuer**
   * **Gérer**
1. Sélectionnez l’utilisateur pour lequel vous souhaitez approuver ou refuser l’autorisation, puis cliquez sur **Approuver tout** ou **Tout refuser**.
1. Cliquez sur la flèche pointant vers la gauche de **Demandes d’accès en attente**, puis cliquez sur **Enregistrer**.

   Si vous avez approuvé la demande, les utilisateurs sont ajoutés à la zone de partage de l’espace de travail. L’utilisateur demandant l’autorisation reçoit un courrier électronique de confirmation confirmant que sa demande a été approuvée. <!--will they also get an in-app notification??-->


## Supprimer des autorisations d’un espace de travail


{{step1-to-planning}}

1. Ouvrez l’espace de travail pour lequel vous souhaitez supprimer des autorisations, puis cliquez sur **Partager** dans le coin supérieur droit de l’écran.
1. Cliquez sur le menu déroulant situé à droite du nom d&#39;une entité avec laquelle vous partagez l&#39;espace de travail, puis cliquez sur **Supprimer**.
1. Cliquer sur **Enregistrer**.

   Les utilisateurs supprimés n’ont plus accès à l’espace de travail ou à ses objets.
