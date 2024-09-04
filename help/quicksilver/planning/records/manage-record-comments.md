---
title: Gérer les commentaires d’enregistrement
description: Vous pouvez collaborer sur les enregistrements Adobe Workfront Planning en ajoutant des commentaires ou des réponses dans le panneau droit d’un enregistrement. Vous pouvez également afficher d’autres modifications apportées à l’enregistrement et enregistrées par le système dans cette zone.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 215883a4-e882-438e-9c21-954c0b1d741b
source-git-commit: bd202821687453288c96147933331c8a7a6b3acb
workflow-type: tm+mt
source-wordcount: '1267'
ht-degree: 88%

---

# Gérer les commentaires d’enregistrement

{{planning-important-intro}}

<!--update the system updates articles when we release to open beta - check the long commenting stream article list and see articles that document where in the system we have system updates; "Workfront Planning records" should be there-->

Vous pouvez collaborer sur les enregistrements Adobe Workfront Planning en ajoutant des commentaires ou des réponses dans le panneau droit d’un enregistrement. Vous pouvez également afficher d’autres modifications apportées à l’enregistrement et enregistrées par le système dans cette zone.

Le panneau de droite d’un enregistrement affiche les sections suivantes :

* **Commentaires** : affiche les commentaires et réponses que les utilisateurs et les utilisatrices ajoutent aux enregistrements.
* **Historique** : affiche les modifications enregistrées dans le système que les utilisateurs et les utilisatrices apportent aux champs des enregistrements. Pour plus d’informations, consultez la [Vue d’ensemble de la section Historique](/help/quicksilver/planning/records/history-section-overview.md).

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
<p>L’instance de Workfront de votre entreprise doit être intégrée à l’expérience unifiée Adobe pour pouvoir accéder à toutes les fonctionnalités de la planification Workfront.</p> 
<p>Pour plus d’informations, voir <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience pour Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront*</p></td> 
   <td><p> Contributeur, Clair ou Standard</p>
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

## Remarques concernant les commentaires sur un enregistrement

* Vous pouvez ajouter des commentaires et des réponses aux enregistrements dans la section Commentaires d’un enregistrement de Workfront Planning.

* Les commentaires ajoutés aux enregistrements liés ne s’affichent pas dans les enregistrements à partir desquels vous créez un lien. Par exemple, si vous commentez un enregistrement de produit Workfront Planning lié à un enregistrement Campaign, le commentaire s’affiche uniquement sur l’enregistrement de produit dans Workfront Planning et non sur l’enregistrement Campaign à partir duquel vous effectuez la liaison.

* Vous pouvez ajouter des commentaires aux enregistrements Workfront Planning créés suite à une connexion entre un enregistrement et un objet provenant d’une autre application.

  Ainsi, vous pouvez ajouter des commentaires à l’enregistrement Workfront Planning du projet après avoir connecté les projets Workfront aux enregistrements Workfront Planning. Pour plus d’informations, voir [Connecter des enregistrements](/help/quicksilver/planning/records/connect-records.md).

* Les commentaires ajoutés aux objets liés dans d’autres applications ne s’affichent pas dans Workfront Planning et les commentaires ajoutés aux objets liés dans Workfront Planning ne s’affichent pas dans d’autres applications.

  Par exemple, les commentaires ajoutés aux projets dans Workfront ne s’affichent pas sur le même projet lié à une campagne dans Workfront Planning et les commentaires ajoutés à l’enregistrement Workfront Planning du projet ne s’affichent pas dans Workfront.

* Vous pouvez taguer des utilisateurs et utilisatrices pour attirer leur attention sur la mise à jour. Les utilisateurs et utilisatrices tagués reçoivent une notification in-app et un e-mail concernant votre mise à jour. <!--this might change??-->

<!--replace the bullet above with this: * You can tag users to bring their attention to an update. Tagged users receive an in-app notification or an email notification about your update. 
   The following scenario exists:   

   * Adobe Unified Experience users receive both an in-app notification and an email notification. 
   * Users who are not in the Adobe Unified Experience receive only an email notification. 

      For information, see [Adobe Workfront Planning notifications: article index](/help/quicksilver/planning/notifications/notifications-information.md)
   
      To determine whether your company is using the Adobe Unified Experience, see [Adobe Unified Experience for Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).
      -->

* Vous pouvez ajouter une mise à jour aux enregistrements et consulter l’historique des modifications dans les sections suivantes de Workfront Planning :

   * Dans la page des détails de l’enregistrement.
   * Dans une vue, dans la zone des détails de l’enregistrement.

### Gérer les commentaires sur les enregistrements

{{step1-to-planning}}

1. Cliquez sur la carte d’un espace de travail.

   L’espace de travail s’ouvre et les types d’enregistrement s’affichent sur les cartes.

1. Cliquez sur une carte de type enregistrement.
La page de type enregistrement s’ouvre et tous les enregistrements de ce type s’affichent.

1. Choisissez une vue en tableau dans le menu déroulant **Affichage**.
1. Cliquez sur le nom d’un enregistrement dans la vue de tableau.

   La page **Détails** de l’enregistrement s’ouvre. La zone Commentaires s’ouvre par défaut dans le panneau de droite.

1. (Le cas échéant) Si le panneau de droite ne s’ouvre pas par défaut, cliquez sur l’icône **Afficher les commentaires** ![](assets/show-comments-icon.png) dans le coin supérieur droit pour ouvrir la section des commentaires.

1. Commencez à saisir un commentaire dans la boîte **Nouveau commentaire**.

   ![](assets/empty-comment-box-on-record.png)

   >[!TIP]
   >
   >Lorsque vous quittez la section Commentaires avant de terminer la saisie et d’envoyer un commentaire, le commentaire reste en mode brouillon sur la page, même après votre déconnexion et reconnexion. Toutes les images ajoutées au commentaire sont également enregistrées dans le brouillon. Les brouillons sont enregistrés pendant 7 jours, après quoi ils sont éliminés et ne peuvent pas être récupérés. Les commentaires en mode brouillon ne sont visibles que par l’utilisateur ou l’utilisatrice qui les saisit.

1. (Facultatif) Pour annuler ou rétablir une modification, utilisez les raccourcis clavier suivants :
   * Ctrl+Z (⌘+z pour Mac) pour annuler une modification
   * Ctrl+Y (⌘+y pour Mac) pour rétablir la modification
1. (Facultatif) Ajoutez **@** suivi du nom d’un utilisateur ou d’une utilisatrice pour identifier une personne dans la mise à jour.

   <!--Adobe Unified Experience users can receive an in-app and an email notification when they are tagged. All other users receive an email when they are tagged. For more information, see the section [Considerations about commenting on a record](#considerations-about-commenting-on-a-record) in this article. -->

1. (Facultatif) Utilisez les options de la barre d’outils de texte enrichi pour mettre en forme votre texte, ajouter des émoticônes, des liens ou des images à votre mise à jour, afin d’améliorer votre contenu. Pour plus d’informations, reportez-vous à la section « Utiliser du texte enrichi dans une mise à jour Workfront » de l’article [Mettre à jour le travail](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

   >[!TIP]
   >
   >Si une autre personne envoie un commentaire au même élément que celui que vous mettez à jour, une ligne rouge s’affiche avec un indicateur « Nouveau » pour vous informer des commentaires les plus récents.
   >
   >L’indicateur s’affiche uniquement après l’envoi du commentaire sur l’élément, et non tant que le commentaire est toujours en train d’être composé.
   >
   >![](assets/new-line-indicator-comments.png)

1. Cliquez sur **Envoyer** pour ajouter la mise à jour à l’enregistrement.
1. (Facultatif) Pour modifier un commentaire, cliquez sur le menu **Plus** ![](assets/more-menu.png) dans le coin supérieur droit du commentaire, puis cliquez sur **Modifier**.

   >[!IMPORTANT]
   >
   >Vous ne pouvez modifier votre commentaire qu’au cours des 15 minutes suivant son envoi.

1. Modifiez les informations du commentaire, ajoutez ou supprimez des images ou supprimez l’une des personnes mentionnées. Un indicateur « modifié » est ajouté à gauche du commentaire.

   >[!TIP]
   >
   >Les commentaires de l’année en cours n’affichent pas l’année dans l’horodatage. Le survol d’un horodatage affiche la date complète, année incluse.

1. (Facultatif et le cas échéant) Pour rechercher un commentaire existant, commencez à saisir un mot-clé dans la zone de recherche située dans le coin supérieur droit de la zone **Commentaires**.

   ![](assets/search-box-for-comments-area.png)

1. (Facultatif) Cliquez sur **Répondre** ou commencez à saisir un commentaire dans la zone **Ajouter une réponse ...**, pour répondre à un commentaire existant, puis suivez les étapes 4 à 8 ci-dessus. <!--(**************accurate??***********)-->

1. (Le cas échéant et facultatif) Si d’autres personnes ont ajouté des commentaires qui s’affichent en dehors de la zone visible dans la section Commentaires pendant que vous ajoutiez vos commentaires, cliquez sur **Afficher** dans la **nouvelle bannière de commentaires** en bas de l’écran pour afficher ces commentaires.

   ![](assets/new-comments-banner-on-record.png)

   D’autres commentaires s’affichent en bas de l’écran.

1. (Facultatif) Cliquez sur l’icône **J’aime** pour aimer une mise à jour ou confirmer que vous l’avez lue. L’icône se met à jour avec le nombre de mentions « J’aime ».
1. (Le cas échéant et facultatif) Si vous avez inclus des personnes supplémentaires dans votre commentaire, cliquez sur les avatars des personnes incluses dans la mise à jour pour afficher la liste des utilisateurs et utilisatrices avec qui le commentaire est partagé.
1. (Facultatif) Cliquez sur l’icône **Plus** ![](assets/more-menu.png) dans le coin supérieur droit du commentaire, cliquez sur l’une des options suivantes pour copier une information d’un commentaire :

   * **Copier le lien** : copie un lien vers le commentaire dans le presse-papiers.
   * **Copier le corps de texte** : copie le texte du commentaire dans le presse-papiers.
   * **Citer la réponse** : copie le contenu de votre commentaire dans une nouvelle réponse. Les images ne sont pas incluses dans la réponse copiée.

   Pour plus d’informations, consultez la section [Mettre à jour le travail](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. (Facultatif) Cliquez sur l’icône **Plus** ![](assets/more-menu.png) dans le coin supérieur droit du commentaire, puis cliquez sur **Supprimer** pour supprimer le commentaire.
1. (Facultatif) Cliquez sur l’icône **Masquer les commentaires** ![](assets/hide-comments-icon.png) pour fermer le panneau de droite.

## Vue d’ensemble de la section Historique

Vous pouvez consulter les modifications apportées à l’enregistrement dans la section Historique du panneau droit d’un enregistrement.

Pour plus d’informations, consultez la [Vue d’ensemble de la section Historique](/help/quicksilver/planning/records/history-section-overview.md).
