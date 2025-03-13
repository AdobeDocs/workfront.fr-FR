---
title: Partager les types d’enregistrements
description: Vous pouvez partager un type d’enregistrement avec d’autres utilisateurs pour garantir la collaboration lors de l’utilisation d’Adobe Workfront Planning.
hide: true
hidefromtoc: true
exl-id: bf49db73-09f1-417e-836b-16c6062740d4
source-git-commit: 5005493bb98b63f4c463f424be43a9d422744846
workflow-type: tm+mt
source-wordcount: '1188'
ht-degree: 13%

---

<!-- add these to metadata on release:

author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog-->

# Partage des types d’enregistrements

<span class="preview">Les informations de cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de façon générale. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Après les versions mensuelles en production, les mêmes fonctionnalités sont également disponibles dans l’environnement de production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation des versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Vous pouvez partager un type d’enregistrement avec d’autres utilisateurs pour garantir une collaboration lors de l’utilisation d’enregistrements dans Adobe Workfront Planning.

>[!IMPORTANT]
>
>* L’octroi d’autorisations à un espace de travail donne par défaut aux utilisateurs les mêmes autorisations aux types d’enregistrements dans l’espace de travail .
>* Vous pouvez ajuster les autorisations sur des types d’enregistrements individuels.
>* Vous ne pouvez pas accorder aux personnes un accès supérieur à un type d’enregistrement par rapport à l’accès qu’elles ont à l’espace de travail.
> Pour plus d’informations, consultez la section [Considérations lors du partage de types d’enregistrements](#considerations-when-sharing-record-types) de cet article.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès.

<!--at GA, check that the Workfront plans article linked below has Planning info-->

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
<p>L’instance de Workfront de votre entreprise doit être intégrée à l’expérience unifiée Adobe pour pouvoir accéder à toutes les fonctionnalités de Workfront Planning.</p> 
<p>Votre organisation doit être intégrée à l’expérience unifiée Adobe pour que les utilisateurs puissent demander et accorder des autorisations pour une vue à partir d’une demande d’autorisation. </p>
<p>Pour plus d’informations, voir <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience pour Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront*</p></td> 
   <td><p> Standard</p>
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
   <td>  <p>Gestion des autorisations relatives à un type d’enregistrement</p>  
   <p>Seuls les utilisateurs disposant d’autorisations de niveau Gérer pour un espace de travail peuvent partager ces autorisations avec un type d’enregistrement</p></td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modèle de disposition</p></td> 
   <td> <p>Toutes les personnes, y compris les administrateurs et administratrices de Workfront, doivent se voir attribuer un modèle de mise en page incluant la zone Planning dans le menu principal. </p> </td> 
  </tr> 
</tbody> 
</table>

* Pour plus d’informations sur les exigences d’accès à Workfront, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Remarques concernant le partage de types d’enregistrements

* Pour obtenir des informations générales sur le partage d’objets dans Workfront Planning, consultez également la section [Présentation des autorisations de partage dans Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).
* Vous pouvez partager un type d’enregistrement en interne avec les entités suivantes :

   * Utilisateurs, groupes, équipes, entreprises et fonctions de Workfront
* Vous ne pouvez pas partager des types d’enregistrements en externe, avec des utilisateurs en dehors de Workfront.
* Les utilisateurs héritent automatiquement des autorisations de type d’enregistrement de l’espace de travail.
* Manuellement, vous pouvez accorder aux utilisateurs des autorisations d’affichage pour un type d’enregistrement ou supprimer les autorisations héritées de l’espace de travail.

* Les utilisateurs ajoutés à la zone de partage de type d’enregistrement qui ne disposent pas d’autorisations d’espace de travail sont automatiquement ajoutés au partage de l’espace de travail avec les autorisations d’affichage.

  Pour accorder à un utilisateur qui ne dispose pas d’autorisations d’espace de travail supérieures aux autorisations d’affichage d’un type d’enregistrement, vous devez d’abord partager l’espace de travail avec lui. Si vous partagez uniquement le type d’enregistrement, ils ne peuvent recevoir que des autorisations d’affichage pour le type d’enregistrement et ils sont également ajoutés à l’espace de travail avec des autorisations d’affichage. Lorsque vous leur donnez des autorisations sur le type d’enregistrement, la zone de partage indique qu’ils sont également ajoutés à l’espace de travail.

* Vous ne pouvez pas accorder à une personne des autorisations supérieures au type d’enregistrement qu’elle ne dispose sur un espace de travail.

  Par exemple, vous ne pouvez pas accorder à quelqu&#39;un l&#39;autorisation Afficher à un espace de travail et l&#39;autorisation Gérer à un type d&#39;enregistrement.


## Partage des autorisations sur un type d’enregistrement

Vous pouvez ajuster les autorisations aux types d’enregistrements individuels d’un espace de travail si vous disposez de l’autorisation Gérer sur l’espace de travail.

{{step1-to-planning}}

1. Ouvrez l’espace de travail dont vous souhaitez partager les types d’enregistrements, puis cliquez sur une carte de type d’enregistrement.

   Cela ouvre la page du type d’enregistrement.

1. Dans l’onglet d’un affichage, cliquez sur **Partager** dans le coin supérieur droit du type d’enregistrement.

   La boîte **Partager** s’ouvre.

   ![Autorisations pour les types d’enregistrements avec des autorisations héritées sur ](assets/permissions-for-record-types-with-inherited-permissions-on.png)

1. (Facultatif) Dans la zone **Qui a accès**, sélectionnez l’une des options suivantes : <!--the Only invited people is supposed to be removed - rewrite this - according to Vahan-->

   * **Seules les personnes invitées peuvent y accéder** : vous devez spécifier les utilisateurs, groupes, équipes, sociétés ou fonctions avec lesquels vous souhaitez partager la vue.
   * **Tout le monde peut afficher dans l’espace de travail** : tous les utilisateurs disposant d’autorisations d’affichage ou d’autorisations supérieures dans l’espace de travail peuvent accéder à l’affichage. Il s’agit de l’option par défaut. <!--rewrite this based on what Lilit says in the proof: At this point, once the inherited permissions are disabled, everyone in the workspace except workspace managers will have View permission to the record type because the "Everyone in the workspace can view"  setting cannot be changed. -->

1. (Facultatif) Développez l’option **Autorisations héritées** pour afficher les utilisateurs, les équipes, les groupes, les sociétés ou les fonctions qui héritent des autorisations de l’espace de travail.

   >[!TIP]
   >
   >Vous ne pouvez pas supprimer des entités individuelles de la liste des autorisations héritées.

1. (Facultatif et conditionnel) Si vous souhaitez partager le type d’enregistrement avec des entités spécifiques et leur donner un accès au type d’enregistrement différent de celui qu’elles ont déjà pour l’espace de travail, procédez comme suit :

   1. Désactivez les autorisations héritées.
   1. Dans le champ **Accorder l’accès à ce type d’enregistrement** ajoutez les utilisateurs, équipes, groupes, sociétés ou fonctions auxquels vous souhaitez accorder un niveau d’autorisation différent.
   1. Choisissez un niveau d’autorisation.

   >[!IMPORTANT]
   >
   >* Vous ne pouvez jamais accorder aux utilisateurs des autorisations plus importantes sur un type d’enregistrement que sur un espace de travail.
   >* Vous ne pouvez pas accorder aux utilisateurs une autorisation moindre que Gérer pour un type d’enregistrement s’ils disposent des autorisations Gérer pour l’espace de travail.
   >* Vous pouvez accorder aux utilisateurs une autorisation moindre sur le type d’enregistrement s’ils disposent des autorisations de type Contributeur sur l’espace de travail.
   > Pour plus d’informations, consultez la section [Vue d’ensemble des autorisations de partage dans Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).

1. Pour permettre aux utilisateurs qui ne disposent pas des autorisations d’accès à l’espace de travail d’afficher le type d’enregistrement, dans le champ **Accorder l’accès à cette vue**, commencez à saisir le nom d’un utilisateur, d’un groupe, d’une équipe, d’une entreprise ou d’une fonction, puis cliquez dessus lorsqu’il s’affiche dans la liste.

   L&#39;entité sélectionnée est ajoutée au type d&#39;enregistrement et à l&#39;espace de travail avec les autorisations **Vue**.

   Les administrateurs système reçoivent toujours des autorisations de niveau Gérer pour les types d’enregistrements partagés avec eux. Cela indique également qu’un utilisateur est administrateur système.

1. Cliquez sur **Copier le lien** pour copier un lien vers le type d’enregistrement dans le presse-papiers.
1. Cliquer sur **Enregistrer**.

   Le type d’enregistrement est maintenant partagé avec d’autres utilisateurs.

1. Partagez le lien copié avec d’autres personnes. Les utilisateurs et utilisatrices qui reçoivent le lien doivent être des utilisateurs et utilisatrices actifs et se connecter à Workfront pour pouvoir accéder à la page du type d’enregistrement et l’afficher dans la vue sélectionnée.

<!-- This is not working yet: *************************** edit this before publishing, because this was not tested with record types - this section came from sharing views *******************: 

## Grant permissions to a record type from a permission request

Users who access a link to a record type to which they do not have permissions can request permissions to the record type. All users with Manage permissions to the view receive the permission request and can grant or deny the permissions. 

1. (Conditional) If you are are the manager of a view, you might receive a request from another user to access the view in the following areas:
   
   * An in-app notification
      ![In-app notification for access request for view](assets/in-app-notification-for-access-request-for-view.png)
   * An email notification
      ![In-app notification for access request for view](assets/in-app-notification-for-access-request-for-view.png)
1. (Conditional) From the notification area in Workfront, click the in-app notification
   Or
   From the email notification, click **View all notifications**, then click the notification in the list.

   The **Pending access requests** box displays. 

      ![Notifications list approval box](assets/notifications-list-approval-box.png)
1. (Optional) For the user whose permissions you want to approve, select one of the following options from the drop-down menu to the right of the user's name: 
   * **View**
   * **Manage**
1. Select the user for whom you want to approve or deny the permission, then click **Approve all** or **Deny all**. 
1. Click the left-pointing arrow to the left of **Pending access requests**, then click **Save**.

   If you approved the request, the users are added to the sharing box of the view. The user requesting the permission receives an email confirmation that their request was approved. <!--will they also get an in-app notification??-->

## Supprimer les autorisations d’un type d’enregistrement

<!-- take this section out - this is what Lilit said: Because of "Everyone in the workspace can view" wildcard, currently it's not possible to entirely remove access to a record type. Let's take out this section. -->

{{step1-to-planning}}

1. Ouvrez l’espace de travail dont vous souhaitez arrêter le partage des types d’enregistrements, puis cliquez sur une carte de type d’enregistrement. Cela ouvre la page du type d’enregistrement.

1. Dans l’onglet d’un affichage, cliquez sur **Partager** dans le coin supérieur droit du type d’enregistrement.

   La boîte **Partager** s’ouvre.
1. Recherchez l’utilisateur, le groupe, l’équipe, la société ou la fonction dont vous souhaitez supprimer les autorisations, développez le menu déroulant des autorisations à droite de leur nom, puis cliquez sur **Supprimer**. <!--check the screen shot below - the UI text for View might not be accurate-->

   ![Option de suppression dans le menu déroulant Partage de type d’enregistrement](assets/remove-option-on-record-type-sharing-drop-down.png)

1. Cliquer sur **Enregistrer**.

   Les personnes n’ont plus accès au type d’enregistrement. Ils peuvent toujours disposer d’autorisations sur l’espace de travail, à moins que vous ne les supprimiez également des autorisations de l’espace de travail .

   Les utilisateurs qui ont été supprimés de l’accès à l’affichage ne sont pas avertis qu’ils ne disposent plus de cet accès.
