---
title: Gestion des commentaires d’enregistrement
description: Vous pouvez collaborer sur les enregistrements Adobe Maestro en ajoutant des mises à jour et en posant des questions ou des réponses dans la zone Commentaires d’un enregistrement.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 3ffb6fdebb54682abc737e55186850458a133f7c
workflow-type: tm+mt
source-wordcount: '957'
ht-degree: 0%

---


<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Gestion des commentaires d’enregistrement

Vous pouvez collaborer sur les enregistrements Adobe Maestro en ajoutant des mises à jour et en posant des questions ou des réponses dans la zone Commentaires d’un enregistrement.

## Remarques concernant les commentaires sur un enregistrement

* Vous pouvez ajouter des commentaires et des réponses aux dossiers et taxonomies opérationnels dans Maestro, dans la section Commentaires d’un enregistrement.

* Les commentaires ajoutés aux enregistrements liés ne s’affichent pas dans les enregistrements à partir desquels vous créez un lien. Par exemple, si vous commentez un projet lié à un enregistrement Campaign, le commentaire s’affiche uniquement sur l’enregistrement du projet dans Maestro et non sur l’enregistrement de campagne à partir duquel vous liez.

* Les commentaires ajoutés aux objets liés dans d’autres applications ne s’affichent pas dans Maestro.
Les commentaires ajoutés aux objets liés dans Maestro ne s’affichent pas dans d’autres applications.\
  Par exemple, les commentaires ajoutés aux projets dans Workfront ne s’affichent pas sur le même projet lié à une campagne dans Maestro.

* Vous pouvez marquer les utilisateurs pour attirer leur attention sur une mise à jour. Les utilisateurs balisés ne reçoivent pas de notification in-app ni d’e-mail concernant votre mise à jour. Vous ne pouvez pas baliser les équipes dans un commentaire Maestro.

  >[!TIP]
  >
  >* Les propriétaires de commentaires ne sont pas automatiquement balisés dans une mise à jour.
  >
  >* Vous ne pouvez pas supprimer des utilisateurs balisés d’une mise à jour lorsque vous y répondez.

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
   <td> <p>L’administrateur système doit ajouter la zone Maestro à votre modèle de mise en page. Pour plus d’informations, voir <a href="../access/grant-access.md">Accorder l’accès à Adobe Maestro</a>. </p>  
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
   <td> <p>Your Workfront or group administrator must add the Maestro area in your layout template. For information, see <a href="../access/grant-access.md">Grant access to Adobe Maestro</a>. </p>  
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


<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

### Gestion des commentaires sur les enregistrements

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![Menu Principal](assets/dots-main-menu.png) dans le coin supérieur droit d’Adobe Workfront, ou (le cas échéant), cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![Menu Principal](assets/lines-main-menu.png) dans le coin supérieur gauche, puis cliquez sur **[!UICONTROL Maestro]**.

   Le dernier espace de travail ouvert par défaut.
1. Choisissez une vue de tableau parmi les **Affichage** menu déroulant.
1. Cliquez sur le nom d’un enregistrement dans la vue de tableau.

   Le record **Détails** s’ouvre.

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

1. (Facultatif et conditionnel) Pour rechercher un commentaire existant, commencez à saisir un mot-clé dans la zone de recherche située dans le coin supérieur droit du champ **Commentaires** zone.

   ![](assets/search-box-for-comments-area.png)

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

