---
title: Gestion des commentaires d’enregistrement
description: Vous pouvez collaborer sur des enregistrements Adobe Maestro en ajoutant des commentaires ou des réponses dans le panneau droit d’un enregistrement. Vous pouvez également afficher d’autres modifications apportées à l’enregistrement et enregistrées par le système dans cette zone.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 4016ba2c1b94ba84037612bdc9c1136267513fd5
workflow-type: tm+mt
source-wordcount: '1155'
ht-degree: 0%

---


# Gestion des commentaires d’enregistrement

{{maestro-important-intro}}

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--update the system updates articles when we release to open beta - check the long commenting stream article list and see articles that document where in the system we have system updates; "Maestro records" should be there-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. </span>

<span class="preview">For information about the current release schedule, see [First Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).</span> -->

Vous pouvez collaborer sur des enregistrements Adobe Maestro en ajoutant des commentaires ou des réponses dans le panneau droit d’un enregistrement. Vous pouvez également afficher d’autres modifications apportées à l’enregistrement et enregistrées par le système dans cette zone.

Le panneau de droite d’un enregistrement affiche les sections suivantes :

* **Commentaires**: affiche les commentaires et réponses que les utilisateurs ajoutent aux enregistrements.
* **Histoire**: affiche les modifications enregistrées par le système que les utilisateurs apportent aux champs d’enregistrement. Pour plus d’informations, voir [Présentation de la section Historique](/help/quicksilver/maestro/records/history-section-overview.md).

>[!TIP]
>
>Le panneau de droite s’affiche pour les enregistrements opérationnels et les enregistrements de taxonomie.


## Remarques concernant les commentaires sur un enregistrement

* Vous pouvez ajouter des commentaires et des réponses aux dossiers et taxonomies opérationnels dans Maestro, dans la section Commentaires d’un enregistrement.

* Les commentaires ajoutés aux enregistrements liés ne s’affichent pas dans les enregistrements à partir desquels vous créez un lien. Par exemple, si vous commentez un enregistrement de produit Maestro lié à un enregistrement de campagne, le commentaire s’affiche uniquement sur l’enregistrement de produit dans Maestro et non sur l’enregistrement de campagne à partir duquel vous liez.

* Vous pouvez ajouter des commentaires aux enregistrements Maestro créés suite à une connexion entre un enregistrement Maestro et un objet provenant d’une autre application.

  Par exemple, vous pouvez ajouter des commentaires à l’enregistrement Project Manager après avoir connecté les projets Workfront aux enregistrements Maestro. Pour plus d’informations, voir [Connexion d’enregistrements](/help/quicksilver/maestro/records/connect-records.md).

* Les commentaires ajoutés aux objets liés dans d’autres applications ne s’affichent pas dans Maestro et les commentaires ajoutés aux objets liés dans Maestro ne s’affichent pas dans d’autres applications.

  Par exemple, les commentaires ajoutés aux projets dans Workfront ne s’affichent pas sur le même projet lié à une campagne dans Maestro, et les commentaires ajoutés à l’enregistrement du projet Maestro ne s’affichent pas dans Workfront.

* Vous pouvez marquer les utilisateurs pour attirer leur attention sur une mise à jour. Les utilisateurs balisés ne reçoivent pas de notification in-app ni d’e-mail concernant votre mise à jour. <!--this might change??-->

* Vous pouvez ajouter une mise à jour aux enregistrements et consulter l’historique des modifications à partir des zones suivantes de Maestro :

   * Sur la page Détails d’un enregistrement ou d’une taxonomie.

  <!--* From the table view.-->

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Produit</p> </td>
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
   <td role="rowheader"><p>Configuration du niveau d’accès</p></td>
   <td> <p>Il n’existe aucun contrôle de niveau d’accès dans Maestro. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Autorisations</p></td>
   <td> <p>Affichage ou autorisations supérieures à un espace de travail</a> </p>  
   <p>Les administrateurs système disposent d’autorisations pour tous les espaces de travail, y compris ceux qu’ils n’ont pas créés.</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Modèle de mise en page</p></td>
   <td> <p>L’administrateur de Workfront ou de groupe doit ajouter la zone Maestro à votre modèle de mise en page. Pour plus d’informations, voir <a href="../access/access-overview.md">Présentation de l’accès</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

### Gestion des commentaires sur les enregistrements

{{step1-to-maestro}}

Le dernier espace de travail ouvert par défaut.
1. Choisissez une vue de tableau parmi les **Affichage** menu déroulant.
1. Cliquez sur le nom d’un enregistrement dans la vue de tableau.

   Le record **Détails** s’ouvre. La zone Commentaires s’ouvre par défaut dans le panneau de droite.

1. (Conditionnel) Si le panneau de droite ne s’ouvre pas par défaut, cliquez sur le bouton **Afficher les commentaires** ![](assets/show-comments-icon.png) dans le coin supérieur droit pour ouvrir la section Commentaires .

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
   * **Copier le texte du corps**: copie le texte du commentaire dans le presse-papiers.
   * **Réponse entre guillemets**: copie alors le contenu de votre commentaire dans une nouvelle réponse. Les images ne sont pas incluses dans la réponse copiée.

   Pour plus d’informations, voir [Mise à jour du travail](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. (Facultatif) Cliquez sur le **Plus** icon ![](assets/more-menu.png) dans le coin supérieur droit du commentaire, puis cliquez sur **Supprimer** pour supprimer le commentaire.
1. (Facultatif) Cliquez sur le **Masquer les commentaires** icon ![](assets/hide-comments-icon.png) pour fermer le panneau de droite.

## Présentation de la section Historique

Vous pouvez passer en revue les modifications apportées à l’enregistrement dans la section Historique du panneau droit d’un enregistrement opérationnel ou d’une taxonomie.

Pour plus d’informations, voir [Présentation de la section Historique](/help/quicksilver/maestro/records/history-section-overview.md).

