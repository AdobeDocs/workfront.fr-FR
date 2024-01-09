---
title: Gestion des commentaires d’enregistrement
description: Vous pouvez collaborer sur les enregistrements Adobe Maestro en ajoutant des commentaires ou des réponses dans la zone Commentaires d’un enregistrement.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 74db651f8865965f943bc89e58e7130cffe0c450
workflow-type: tm+mt
source-wordcount: '997'
ht-degree: 0%

---


# Gestion des commentaires d’enregistrement

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles dans l’ensemble. Il est disponible uniquement dans l’environnement Aperçu pour tous les clients. </span>

<span class="preview">Pour plus d’informations sur le calendrier de publication actuel, voir [Présentation de la version du premier trimestre 2024](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).</span>

Vous pouvez collaborer sur les enregistrements Adobe Maestro en ajoutant des commentaires ou des réponses dans la zone Commentaires d’un enregistrement.

## Remarques concernant les commentaires sur un enregistrement

* Vous pouvez ajouter des commentaires et des réponses aux dossiers et taxonomies opérationnels dans Maestro, dans la section Commentaires d’un enregistrement.

* Les commentaires ajoutés aux enregistrements liés ne s’affichent pas dans les enregistrements à partir desquels vous créez un lien. Par exemple, si vous commentez un enregistrement de produit Maestro lié à un enregistrement de campagne, le commentaire s’affiche uniquement sur l’enregistrement de produit dans Maestro et non sur l’enregistrement de campagne à partir duquel vous liez.

* Vous pouvez ajouter des commentaires aux enregistrements Maestro créés suite à une connexion entre un enregistrement Maestro et un objet provenant d’une autre application.

  Par exemple, vous pouvez ajouter des commentaires à l’enregistrement Project Manager après avoir connecté les projets Workfront aux enregistrements Maestro. Pour plus d’informations, voir [Connexion d’enregistrements](/help/quicksilver/maestro/records/connect-records.md).

* Les commentaires ajoutés aux objets liés dans d’autres applications ne s’affichent pas dans Maestro et les commentaires ajoutés aux objets liés dans Maestro ne s’affichent pas dans d’autres applications.

  Par exemple, les commentaires ajoutés aux projets dans Workfront ne s’affichent pas sur le même projet lié à une campagne dans Maestro, et les commentaires ajoutés à l’enregistrement du projet Maestro ne s’affichent pas dans Workfront.

* Vous pouvez marquer les utilisateurs pour attirer leur attention sur une mise à jour. Les utilisateurs balisés ne reçoivent pas de notification in-app ni d’e-mail concernant votre mise à jour. <!--this might change??-->

* Vous pouvez ajouter une mise à jour aux enregistrements des zones suivantes de Maestro :

   * Sur la page Détails .

  <!--* From the table view.-->

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto">
 <col>
 <tbody>
<td>
   <p> Adobe de produit</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Accord Adobe Workfront</p></td>
   <td>
<p>Votre entreprise doit être inscrite au programme bêta fermé Adobe Maestro. Contactez le représentant de votre compte pour en savoir plus sur cette nouvelle offre. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Formule Adobe Workfront</p></td>
   <td>
<p>Quelconque</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licence Adobe Workfront</p></td>
   <td>
   <p>Quelconque</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader">Niveau d’accès</td>
   <td> <p>Quelconque</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">Modèle de mise en page</td>
   <td> <p>L’administrateur système doit ajouter la zone Maestro à votre modèle de mise en page. Pour plus d’informations, voir <a href="../access/access-overview.md">Présentation de l’accès</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--
After permissions - replace the table with: **************CHECK ON THE VIEW PERMISSIONS TO THE WORKSPACE; RIGHT NOW, WE SAY THAT VIEW USERS CAN COMMENT BUT THE PAGE BLOWS OUT WHEN I TRY - ASKED PM TO CONFIRM*****************

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Adobe product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the Adobe Maestro closed beta program. Contact your account representative to inquire about this new offering. </p>
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
   <td role="rowheader"><p>Access level</p></td>
   <td> <p>Any</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Maestro area in your layout template. For information, see <a href="../access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>View or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
 </tbody>
</table>

-->

### Gestion des commentaires sur les enregistrements

{{step1-to-maestro}}

Le dernier espace de travail ouvert par défaut.
1. Choisissez une vue de tableau parmi les **Affichage** menu déroulant.
1. Cliquez sur le nom d’un enregistrement dans la vue de tableau.

   Le record **Détails** s’ouvre. La zone Commentaires s’ouvre par défaut dans le panneau de droite.

1. Commencez à saisir un commentaire dans la variable **Nouveau commentaire** de la boîte.

   ![](assets/empty-comment-box-on-record.png)

   >[!TIP]
   >
   >Lorsque vous quittez la section Commentaires avant de terminer la saisie et d’envoyer un commentaire, le commentaire reste en mode préliminaire sur la page, même après vous être déconnecté et vous être reconnecté. Toutes les images ajoutées au commentaire sont également enregistrées dans le brouillon. Les brouillons sont enregistrés pendant 7 jours, après quoi ils sont ignorés et ne peuvent pas être récupérés. Les commentaires préliminaires ne sont visibles que par l’utilisateur qui les saisit.

1. (Facultatif) Pour annuler ou rétablir une modification, utilisez les raccourcis clavier suivants :
   * Ctrl + Z ( ⌘ + z pour Mac) pour annuler une modification.
   * Ctrl + Y ( ⌘ + y pour Mac) pour rétablir la modification
1. (Facultatif) Ajoutez **@** suivi du nom d’un utilisateur pour baliser une personne dans la mise à jour.
1. (Facultatif) Utilisez les options de la barre d’outils Texte enrichi pour mettre en forme votre texte, ajouter des émoticônes, des liens ou des images à votre mise à jour, afin d’améliorer votre contenu. Pour plus d’informations, reportez-vous à la section &quot;Utiliser du texte enrichi dans une mise à jour Workfront&quot; de l’article. [Mise à jour du travail](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

   >[!TIP]
   >
   >Si un autre utilisateur envoie un commentaire au même élément que celui que vous mettez à jour, une ligne rouge avec un indicateur &quot;Nouveau&quot; s’affiche pour vous informer des commentaires les plus récents.
   >
   >L’indicateur s’affiche uniquement après l’envoi du commentaire sur l’élément, et non lorsque le commentaire est toujours composé.
   >
   >![](assets/new-line-indicator-comments.png)

1. Cliquez sur **Envoyer** pour ajouter la mise à jour à l’enregistrement.
1. (Facultatif) Cliquez sur le bouton **Plus** menu ![](assets/more-menu.png) dans le coin supérieur droit du commentaire, puis cliquez sur **Modifier**.

   >[!IMPORTANT]
   >
   >Vous ne pouvez modifier votre commentaire que dans les 15 minutes suivant son envoi.

1. Modifiez les informations du commentaire, ajoutez ou supprimez des images ou supprimez l’un des utilisateurs balisés. Un indicateur &quot;modifié&quot; est ajouté à gauche du commentaire.

   >[!TIP]
   >
   >Les commentaires de l’année en cours n’affichent pas l’année dans l’horodatage. Le survol d’un horodatage affiche la date complète, y compris l’année.

1. <span class="preview">(Facultatif et conditionnel) Pour rechercher un commentaire existant, commencez à saisir un mot-clé dans la zone de recherche située dans le coin supérieur droit du champ **Commentaires** zone.</span>

   <span class="preview">![](assets/search-box-for-comments-area.png)</span>

1. (Facultatif) Cliquez sur **Répondre** ou commencez à saisir un commentaire dans la variable **Ajouter une réponse ...** , pour répondre à un commentaire existant, puis suivez les étapes 4 à 8 ci-dessus. <!--(**************accurate??***********)-->

1. (Conditionnel et facultatif) Si d’autres utilisateurs ont ajouté des commentaires qui s’affichent en dehors de la zone visible dans la section Commentaires pendant que vous ajoutiez vos commentaires, cliquez sur **Affichage** dans la variable **nouvelle bannière de commentaires** en bas de l’écran pour afficher ces commentaires.

   ![](assets/new-comments-banner-on-record.png)

   D’autres commentaires s’affichent en bas de l’écran.

1. (Facultatif) Cliquez sur le **Comme** pour aimer une mise à jour ou confirmer que vous l’avez lue. L’icône se met à jour avec le nombre de mentions &quot;J’aime&quot;.
1. (Conditionnel et facultatif) Si vous avez inclus des personnes supplémentaires dans votre commentaire, cliquez sur les avatars des utilisateurs inclus dans la mise à jour pour afficher la liste des utilisateurs avec lesquels le commentaire est partagé.
1. (Facultatif) Cliquez sur le **Plus** icon ![](assets/more-menu.png) dans le coin supérieur droit du commentaire, cliquez sur l’une des options suivantes pour copier une information d’un commentaire :

   * **Copier le lien**: copie un lien vers le commentaire dans le presse-papiers.
   * **Copie du texte du corps** t : le texte du commentaire est alors copié dans le presse-papiers.
   * **Réponse entre guillemets**: copie alors le contenu de votre commentaire dans une nouvelle réponse. Les images ne sont pas incluses dans la réponse copiée.

   Pour plus d’informations, voir [Mise à jour du travail](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. (Facultatif) Cliquez sur le **Plus** icon ![](assets/more-menu.png) dans le coin supérieur droit du commentaire, puis cliquez sur **Supprimer** pour supprimer le commentaire.

