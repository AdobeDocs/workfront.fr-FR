---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Mettre à jour le travail
description: Vous pouvez ajouter une mise à jour sur un objet Adobe Workfront (projet, tâche ou problème) pour communiquer sur la progression de l’objet. Les utilisateurs et utilisatrices affectés ou les personnes abonnées à l’objet peuvent afficher votre mise à jour. Vous pouvez également baliser des utilisateurs et utilisatrices pour attirer leur attention sur la mise à jour.
author: Alina
feature: Get Started with Workfront
exl-id: 0f4d6895-6326-4a83-9bbc-bb58c876e7fc
source-git-commit: 4572ea9bb0679c599a55d5a87c1397c7b819c963
workflow-type: tm+mt
source-wordcount: '2978'
ht-degree: 82%

---

# Mettre à jour le travail

<!-- Audited: 1/2024 -->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers or in Production for customers who enabled fast releases. </span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">For information about the current release schedule, see [Second Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span>
-->

<!--info for April 11: hide the "Important" box below-->

<!--
>[!IMPORTANT]
>
>We are currently redesigning the commenting experience in Adobe Workfront.
>
>Depending on what objects you access the commenting experience for, you might see the following functionality for the Updates section:
>* The new experience
>* The legacy experience
>* The new and the legacy experience
>
>For more information about the new commenting experience and its availability, see [New commenting experience](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 
>
><Span class="preview"> The legacy commenting experience has been removed from projects, tasks, issues, and documents in the Preview environment. </span>
>
>The new commenting experience is available only for the Updates section of Workfront objects, and it is not available when you access updates from the following areas:
>
> * Home
> * Summary panel in lists
> * Summary panel in timesheets 
> * Summary panel in the Workload Balancer
>
><span class="preview">The new commenting experience is available in the Summary panel in lists, timesheets, and the Workload Balancer in the Preview environment and in the Production environment for customers who have opted for the fast release process. </span>
-->

Vous pouvez ajouter une mise à jour sur un objet Adobe Workfront pour informer d’autres personnes de la progression de l’objet. Pour plus d’informations sur les objets auxquels vous pouvez ajouter des mises à jour dans Workfront, voir [Mise à jour de la section - Aperçu](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/updates-tab-overview.md).

Les informations de cet article décrivent comment vous pouvez commenter et mettre à jour les informations pour les projets, les tâches et les problèmes. Les utilisateurs et utilisatrices affectés ou les personnes abonnées à l’objet peuvent afficher votre mise à jour. Vous pouvez également baliser des utilisateurs et utilisatrices pour attirer leur attention sur la mise à jour.

L’ajout de commentaires à d’autres objets est similaire à la mise à jour de projets, de tâches et de problèmes. Pour plus d’informations sur les commentaires sur les cartes et les objectifs, consultez également les articles suivants :

* [Gestion des commentaires d’objectif dans les objectifs Adobe Workfront](../../workfront-goals/goal-management/manage-goal-comments.md).

  Vous devez disposer d’une licence supplémentaire pour accéder aux Objectifs Workfront.

* [Ajouter une carte ad hoc à un panorama](../../agile/get-started-with-boards/add-card-to-board.md)

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Forfait Adobe Workfront</strong></td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licence Adobe Workfront</strong></td> 
   <td> 
   <p>Actuel : licence de demande ou supérieure pour les problèmes et les documents ; licence de révision ou supérieure pour tous les autres objets</p>
   <p>Nouveau : licence de contribution ou supérieure pour les problèmes et les documents ; licence légère (Light) ou supérieure pour tous les autres objets</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurations du niveau d’accès</strong></td> 
   <td> <p>Afficher ou modifier l’accès de l’objet sur lequel la mise à jour est activée</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet</strong></td> 
   <td> <p>Accès à l’affichage de l’objet</p></td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Remarques relatives à la mise à jour du travail

* Vous pouvez ajouter des commentaires à la plupart des objets dans Adobe Workfront dans la section Mises à jour. Pour plus d’informations sur les objets qui affichent la section Mises à jour, consultez [Vue d’ensemble de la section Mises à jour](../updating-work-items-and-viewing-updates/updates-tab-overview.md).

* Vous pouvez ajouter des commentaires aux objets Workfront à partir d’autres applications intégrées à Workfront ou à partir de l’application mobile Workfront.

  Toutes les applications intégrées à Workfront ne peuvent pas ajouter de commentaires aux objets Workfront.

  Toutes les fonctionnalités disponibles dans la section Mises à jour d’un objet dans Workfront ne le sont pas dans d’autres applications lors de l’accès aux objets Workfront à partir de l’application. Par exemple, les fonctionnalités de texte enrichi ou la définition d’un commentaire réservé à l’entreprise d’une personne peuvent ne pas être disponibles lors de l’ajout de commentaires à un objet Workfront à partir d’une application tierce.

* Vous pouvez communiquer sur la progression d’un objet Workfront (projet, tâche ou problème) lorsque vous commentez l’objet. Les utilisateurs et utilisatrices affectés ou les personnes abonnées à l’objet peuvent recevoir une notification concernant votre mise à jour. Toute personne disposant d’un accès Afficher à l’objet peut consulter votre mise à jour.

* Vous pouvez baliser des utilisateurs et utilisatrices pour attirer leur attention sur la mise à jour. Les utilisateurs etu utilisatrices balisés reçoivent une notification in-app et un e-mail concernant votre mise à jour.

  >[!TIP]
  >
  >Les propriétaires de commentaires sont automatiquement balisés. Pour plus d’informations, consultez [Baliser d’autres personnes sur les mises à jour](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).


* Vous pouvez ajouter un commentaire à un objet que vous pouvez afficher ou vous connecter en tant qu’administrateur ou administratrice Workfront ou de groupes et ajouter un commentaire au nom d’un autre utilisateur ou d’une autre utilisatrice. Pour plus d’informations, consultez [Se connecter en tant qu’autre utilisateur ou utilisatrice](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).

* Vous pouvez ajouter une mise à jour à des projets, tâches et problèmes à partir des zones suivantes de Workfront :

   * Dans un objet Workfront, dans la section Mises à jour (pour les projets, les tâches et les problèmes)
   * Dans la zone Accueil (pour les tâches et les problèmes)
   * Dans le panneau Résumé dans les zones suivantes (pour les tâches, les problèmes et les documents) :

      * Une liste d’objets
      * Une feuille de temps
      * Page d’accueil
      * L’équilibreur de charge de travail

<!--info for April 11: hide the section below: add an update to a work item-->

<!--
## Add an update to a work item

Adding an update to a work item differs depending on what version of the Updates section you use.

You can add updates to the following objects: 

* Projects
* Tasks
* Issues
* Programs
* Portfolios
* Templates
* Template tasks
* Users
* Timesheets
* Teams
* Goals
* Cards in the Boards area
* Iterations
-->

<!--info for April 11: hide the section below completely:-->

<!--
### Add an update to a work item in the legacy Updates section

>[!IMPORTANT]
>
>The information on this page describes how you update projects, tasks, and issues.

1. Go to the work item for which you want to provide an update (such as a project, task, or issue).
1. Click the **Updates** section.
1. (Conditional) If it is enabled, click the **New commenting** option in the upper-right corner of the Updates section to disable it and enable the legacy commenting experience.
1. Click **Start a new update,** then type your update.  
1. (Optional) Use the options in the Rich Text toolbar to format your text, add emojis, links, or images to your update, to enhance your content. For more information, see the [Use Rich Text in a Workfront update](#use-rich-text-in-a-workfront-update) section in this article.
1. (Optional) Update any of the following information about the work item:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Notify</strong></td> 
      <td>Identify users who must be notified of the update. Users assigned or subscribed to the object automatically receive notification when an update is made.<br><p>For information about how to include others on an update, see <a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Tag others on updates</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Commit Date</strong></td> 
      <td>In the date picker, select the date that you commit to complete the work item. For information about Commit Date, see <a href="../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">Commit Date overview</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Condition</strong></td> 
      <td>Select a new condition for the task or issue. For information about selecting a condition, see <a href="../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md" class="MCXref xref">Update Condition for tasks and issues</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Status</strong></td> 
      <td>Click the arrow beside the current status, then select the desired status from the drop-down menu. For information about setting a Status, see <a href="../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref">Update task status</a>.<p>Updating the status of a work item does not automatically change the status of a project. Depending on how your project is set up, you might make updates to the project status separately. For more information on the various project update types, see <a href="../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Select the project Update Type </a>.</p><p><b>NOTE</b>
      
      You cannot change the status of a work item while it is in a Pending Approval status.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Completion Bar</strong></td> 
      <td>(Only available on tasks) Indicate the percentage of work completed by sliding the progress bar to the desired percentage. You can also double-click the completion bar and enter the percent complete.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Private to my company</strong></td> 
      <td> <p>Disable this option to prevent users outside your company from having access to view this update.</p> 
      <p><b>NOTE</b></p>
      <p>This option displays only when the user is associated with a Company.</p>
      <p>This option is not available in all areas where you can add updates from. For example, this is not available in third-party applications where you can add updates from. </p>
      </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Update** to add the update to the Workfront object.

   >[!NOTE]
   >
   >A small pop-up window will appear for seven seconds after clicking **Update**, allowing you to undo the update and return to the editing pane before the update is posted. The update is posted if you dismiss the undo pop-up, wait for it to disappear, or navigate away from the page. 
   >
   >If your Workfront administrator selects the "Never allow users to delete comments" setting in your access level, you cannot undo a comment. For more information, see [Create and modify custom access levels](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

1. To reply to an update, see [Reply to updates](../../workfront-basics/updating-work-items-and-viewing-updates/reply-to-updates.md).
-->

<!--info for April 11: reword the title of this section to: "Add an update to a work item"; take out the step that says you need to enable the "New commenting" toggle (I think it is step 3??)-->

## Ajouter une mise à jour à un élément de travail

Cet article décrit comment mettre à jour un projet, des tâches ou des problèmes. La mise à jour de la plupart des autres objets est similaire.

1. Recherchez l’objet à mettre à jour, puis cliquez sur son nom pour ouvrir la page de l’objet.
1. Cliquez sur  **Mises à jour** dans le panneau de gauche.
L’onglet **Commentaires** est sélectionné par défaut.

   <!--
   1. (Conditional) If the **New commenting** option is disabled, click to enable it. 

      This enables the new commenting experience. 

         >[!TIP]
         >
         ><span class="preview">The New commenting option has been removed in the Preview environment.</span>
   -->

1. Commencez à saisir un commentaire dans la zone **Nouveau commentaire**.

   ![Zone Nouveau commentaire](assets/comment-box-all-tabs.png)

   >[!TIP]
   >
   >Lorsque vous quittez la section Mises à jour avant de terminer la saisie, un commentaire est envoyé afin de conserver le commentaire sur la page en mode brouillon, même après une déconnexion et une reconnexion. Toutes les images ajoutées au commentaire sont également enregistrées dans le brouillon. Les brouillons sont enregistrés pendant 7 jours, après quoi ils sont ignorés et ne peuvent pas être récupérés. Les brouillons de commentaires ne sont visibles que par l’utilisateur ou l’utilisatrice qui les saisit.

1. (Facultatif) Pour annuler ou rétablir une modification, utilisez les raccourcis clavier suivants :
   * Ctrl+Z (⌘+Z pour Mac) pour annuler une modification
   * Ctrl+Y (⌘+Y pour Mac) pour rétablir une modification

1. (Facultatif) Dans la zone **Taguer des personnes ou des équipes**, commencez à saisir le nom ou l’adresse e-mail d’un utilisateur ou d’une utilisatrice ou d’une équipe que vous souhaitez inclure dans ce commentaire, puis sélectionnez-le lorsqu’il apparaît dans la liste.
1. (Facultatif) Utilisez les options de la barre d’outils Texte enrichi pour mettre en forme votre texte, ajouter des émoticônes, des liens ou des images à votre mise à jour afin d’améliorer votre contenu. Pour plus d’informations, consultez la section [Utiliser du texte enrichi dans une mise à jour Workfront](#use-rich-text-in-a-workfront-update) dans cet article.

   >[!TIP]
   >
   >Si un autre utilisateur ou une autre utilisatrice soumet un commentaire sur le même élément que celui que vous mettez à jour, une ligne rouge avec un indicateur « Nouveau » s’affiche pour vous informer des commentaires plus récents.
   >
   >L’indicateur ne s’affiche qu’après la soumission du commentaire sur l’élément, et non lorsque le commentaire est en cours de rédaction.
   >
   >L’indicateur « Nouveau » ne s’affiche que lorsque la personne qui a saisi une nouvelle mise à jour, ainsi que celle qui a saisi une mise à jour, utilisent toutes les deux la nouvelle expérience de commentaire.
   >![](assets/real-time-new-red-indicator-unified-commenting.png)

1. Cliquez sur **Soumettre** pour ajouter la mise à jour à l’objet Workfront.
1. (Facultatif) Pour modifier un commentaire, cliquez sur le menu **Plus** ![](assets/more-menu.png) dans le coin supérieur droit du commentaire, puis sur **Modifier**.

   >[!IMPORTANT]
   >
   >Vous ne pouvez modifier votre commentaire que dans les 15 minutes suivant sa soumission.

1. Modifiez les informations du commentaire, ajoutez ou supprimez des images ou supprimez une des personnes balisées. Un indicateur « Modifié » est ajouté à gauche de la date et de l’heure qui indiquent quand le commentaire a été saisi.

   >[!TIP]
   >
   >Les commentaires de l’année en cours n’affichent pas l’année dans la date et l’heure. Survolez la date et l’heure pour afficher la date complète, année incluse.

   ![](assets/edited-tag-on-comment-unified-commenting.png)

   >[!TIP]
   >
   >* Un e-mail est généré pour informer les utilisateurs et utilisatrices de votre mise à jour uniquement lorsque vous envoyez la mise à jour d’origine. Aucun e-mail n’est généré après avoir modifié votre mise à jour.
   >* La date et l’heure en regard du commentaire correspondent à la date du commentaire d’origine, et non à celle de la dernière modification.
   >* Lorsque vous ajoutez un commentaire au nom d’une autre personne (lorsque vous vous connectez en tant qu’autre utilisateur ou utilisatrice, en tant qu’administrateur ou administratrice Workfront ou de groupes), vous ne pouvez pas modifier le commentaire si votre connexion est effectuée au nom de l’autre personne. Vous ne pouvez modifier le commentaire qu’après votre déconnexion au nom de l’autre personne et votre reconnexion en votre nom.

1. (Facultatif) Cliquez sur **Répondre** ou commencez à saisir un commentaire dans la variable **Ajouter une réponse ...** , pour répondre à un commentaire existant, puis suivez les étapes 3 à 7 ci-dessus. <!--(**************insure this stays accurate***********)--> Pour plus d’informations sur la réponse à une mise à jour, consultez [Répondre aux mises à jour](../../workfront-basics/updating-work-items-and-viewing-updates/reply-to-updates.md).

1. (Le cas échéant et facultatif) Si d’autres utilisateurs et utilisatrices ont ajouté des commentaires qui s’affichent en dehors de la zone visible dans la section Mises à jour pendant que vous ajoutiez vos commentaires, cliquez sur **Afficher** à l’intérieur de la **bannière de nouveaux commentaires** bleue en bas de l’écran pour afficher ces commentaires.

   ![](assets/blue-new-comments-banner-with-view-button.png)

   Les commentaires supplémentaires s’affichent en bas de l’écran.

1. (Facultatif) Cliquez sur l’icône **J’aime** ![](assets/like-icon.png). L’icône se met à jour avec le nombre de mentions « J’aime ».
1. (Le cas échéant et facultatif) Si vous avez inclus des personnes supplémentaires dans votre commentaire, cliquez sur le nombre de personnes membres incluses dans la mise à jour pour afficher une liste des entités avec lesquelles le commentaire que vous avez saisi est partagé.

   ![](assets/members-icons-expanded-unshimmed.png)

   >[!TIP]
   >
   >Les noms des deux premières entités balisées s’affichent en regard de leurs avatars. Si plus de deux entités sont balisées, seuls le nom de la première et le nombre d’entités supplémentaires s’affichent.

1. (Facultatif) Cliquez sur le nom d’un commentateur pour afficher son nom, son rôle et son adresse électronique dans une zone d’informations. Cliquez à nouveau sur le nom du commentateur dans la zone d’informations pour ouvrir son profil utilisateur.
1. (Facultatif) Cliquez sur l’onglet **Activité du système** pour afficher les mises à jour consignées par le système. Lorsque l’objet ou l’un de ses enfants est mis à jour, Workfront génère une note relative à cette mise à jour et l’affiche dans l’onglet Activité du système.

   Pour plus d’informations, consultez [Vue d’ensemble de la section Mises à jour](../updating-work-items-and-viewing-updates/updates-tab-overview.md).

   >[!TIP]
   >
   >Vous ne pouvez pas ajouter de commentaire à une mise à jour du système. Cependant, toutes les réponses apportées aux enregistrements d’activité système dans l’expérience de commentaire héritée ont été ajoutées à l’onglet Activité système en lecture seule. L’expérience de commentaire héritée a été supprimée de Workfront le 11 avril 2024.

1. (Facultatif) Cliquez sur le **Tous** pour afficher à la fois les commentaires d’utilisateur et les commentaires d’activité du système. Il s’agit d’un onglet en lecture seule.

   >[!TIP]
   >
   >Vous ne pouvez pas répondre aux commentaires ni identifier d’autres personnes dans les commentaires existants de l’onglet Tous. Pour répondre à un commentaire dans l’onglet Toutes , cliquez sur **Réponse aux commentaires** pour ouvrir le commentaire dans l’onglet Commentaires .

## Utiliser du texte enrichi dans une mise à jour Workfront{#use-rich-text-in-a-workfront-update}

Vous pouvez améliorer vos mises à jour en utilisant du texte enrichi ou en y ajoutant divers éléments, tels que des émoticônes, des liens ou des images.

1. Accédez à la zone **Mises à jour** d’un objet Workfront et commencez à saisir un commentaire.
1. (Facultatif) Pour ajouter une mise en forme de texte enrichi à votre mise à jour, utilisez un quelconque attribut de la barre d’outils **Texte enrichi** pendant la saisie.

   ![](assets/rich-text-toolbar.png)

   | **Attribut** | **Bouton de barre d’outils** | **Raccourcis clavier Mac** | **Raccourcis clavier Windows** |
   |---|---|---|---|
   | Gras | ![](assets/mceclip10.png) | ⌘+b | Ctrl+B |
   | Italique | ![mceclip9.png](assets/mceclip9.png) | ⌘+i | Ctrl+I |
   | Souligner | ![mceclip8.png](assets/mceclip8.png) | ⌘+u | Ctrl+U |
   | Lien hypertexte | ![mceclip7.png](assets/mceclip7.png) | <br>Pour ouvrir la boîte de dialogue Ajouter des liens : ⌘+K</br> <br>Pour coller un lien sur le texte sélectionné : ⌘+V</br> | <br>Pour ouvrir la boîte de dialogue Ajouter des liens : Ctrl+K</br> <br>Pour coller un lien sur le texte sélectionné : Ctrl+V</br> |
   | Liste à puces | ![mceclip6.png](assets/mceclip6.png) | ⌘+Maj+8 | Ctrl+Maj+8 |
   | Liste numérotée | ![mceclip5.png](assets/mceclip5.png) | ⌘+Maj+7 | Ctrl+Maj+7 |
   <!--| Block Quote | ![](assets/block-quote-icon-large.png)|⌘+Shift+9 |<br>Ctrl+Shift+9</br> <br>This is not available in the new commenting experience. </br> |-->

   <!--remove the last row when we remove legacy from the system-->

   Pour arrêter la mise en forme du texte, désélectionnez l’attribut sur la barre d’outils **Texte enrichi**.


   <!-- in the table above: take "Create Links" verbiage from the hyperlink when the old commenting is removed and the commenting beta is the only way to comment - with October 2023-->

   >[!NOTE]
   >
   >* La mise en forme apparaît également dans toutes les notifications par e-mail contenant votre mise à jour que les utilisateurs et utilisatrices reçoivent.
   >* La mise en forme de texte enrichi appliquée à une mise à jour dans un e-mail n’apparaît pas sur la mise à jour lorsque celle-ci est affichée dans l’onglet Mises à jour.
   >* Si votre entreprise utilise Workfront avec Internet Explorer, le texte formaté collé dans une mise à jour perd sa mise en forme de texte enrichi et s’affiche en texte brut. Vous pouvez reformater le texte à l’aide des attributs de la barre d’outils Texte enrichi.
   >* La mise en forme de texte enrichi n’est pas disponible pour les mises à jour effectuées dans la zone Feuilles de temps ou pour les objets Note et Dernière condition affichés dans un rapport.

   <!--1. (Optional and conditional) If you want to include text from previous updates or from other sources and distinguish it from your own update, you can mark it as a Block Quote. Click the **Block Quote** icon ![](assets/block-quote-small.png) and type the text you want to quote. The quoted text displays marked with a vertical gray line. Click the **Block Quote** icon again to return to normal formatting. This is not available in the new commenting experience.-->

   <!--remove this picture below and the bullet above when we remove legacy-->

   <!--![](assets/block-quote-marked-350x144.png)-->

1. (Facultatif) Cliquez sur l’icône **émoticône** ![](assets/emoji-icon.png) pour ajouter des émoticônes à votre mise à jour.

   >[!NOTE]
   >
   >* Workfront ne remplace pas les émoticônes de ponctuation telles que « :) » par des émoticônes.
   >* Les émoticônes ne sont pas disponibles pour les objets Note et Dernière condition affichés dans un rapport.
   >* La fonctionnalité d’émoticône de Workfront utilise des caractères Unicode. En tant que tels, elle ne s’affiche donc que sur les navigateurs et les systèmes d’exploitation qui prennent en charge les points du code Unicode. Les utilisateurs et utilisatrices d’une version de plateforme, de navigateur ou de système d’exploitation différente de la vôtre peuvent ne pas avoir accès aux mêmes émoticônes.
   >* Une émoticône non prise en charge est représentée par un carré noir ou blanc.
   >* Windows 7 ne prend en charge que les émoticônes en noir et blanc.
   >* Les émoticônes appliquées à une mise à jour par e-mail n’apparaissent pas sur la mise à jour lorsque celle-ci est affichée dans la zone Mises à jour.

1. (Facultatif) Pour ajouter un lien d’URL vers des sources d’informations supplémentaires :

   1. Dans votre mise à jour, cliquez sur l’endroit où vous souhaitez insérer un lien.
   1. Sur la barre d’outils **Texte enrichi**, cliquez sur l’icône **Lien hypertexte** ![](assets/link-icon.png).

   1. Dans la boîte de dialogue **Créer un lien** qui s’affiche, sous **URL**, saisissez ou collez l’URL de la source vers laquelle vous souhaitez rediriger.

   1. Sous **Texte à afficher**, saisissez ou collez le texte du lien.
   1. Cliquer sur **Enregistrer**.

1. (Facultatif) Pour joindre une image à votre mise à jour, effectuez l’une des opérations suivantes :

   * Enregistrez l’image sur votre ordinateur, puis faites-la glisser et déposez-la dans la zone Nouveau commentaire.
   * Copiez une capture d’écran de votre ordinateur, puis collez-la dans le commentaire.<!-- This is not available in the legacy commenting experience.-->
   * Cliquez sur l’icône **Ajouter une image** ![](assets/add-image-mountain-with-plus-icon.png) et accédez à l’image sur votre ordinateur.


   >[!NOTE]
   >
   >* Votre administrateur ou administratrice Workfront doit activer l’ajout d’images dans la section Préférences de mise à jour des flux de la zone d’interface de Workfront pour que vous puissiez voir les icônes Image et Ajouter une pièce jointe. Pour plus d’informations, consultez [Configuration des préférences pour les mises à jour des utilisateurs et utilisatrices](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-preferences-user-updates.md).
   >* La taille maximale du fichier image est de 7 Mo. Les types de fichiers image pris en charge sont .jpg, .gif et .png.
   >* Les images sont accessibles à partir de la section Mises à jour d’un objet et sont également disponibles dans la zone Documents sous le menu principal.
   >* Vous pouvez coller l’image en cliquant avec le bouton droit de la souris dans le nouveau commentaire, ou en appuyant sur les touches CTRL+V pour Windows (ou ⌘+V pour Mac) de votre clavier.
   >* Vous pouvez envoyer une mise à jour avec une image et sans texte.
   >* Lorsque vous supprimez un commentaire qui contient une image, celle-ci est supprimée de la section Mises à jour , ainsi que de la zone Documents . L’image est également supprimée de la zone Documents lorsque vous modifiez un commentaire et supprimez l’image.
   >* Lorsqu’une personne supprime une image jointe à un commentaire de la zone Documents, elle est également supprimée du commentaire.

   <!--remove the statement above about legacy, when we remove the legacy environment.-->

1. (Facultatif) Pour afficher une image dans la mise à jour existante, effectuez l’une des opérations suivantes :

   * Cliquez sur l’icône **Aperçu** ![](assets/previewimageicon-31x31.png) sur la miniature de l’image pour ouvrir l’image en taille réelle dans un nouvel onglet du navigateur.
   * Cliquez sur l’icône **Télécharger** ![](assets/downloadimageicon.png) sur la miniature de l’image pour télécharger l’image.

1. Cliquez sur **Soumettre** pour ajouter votre commentaire.

## Rechercher une mise à jour

Vous pouvez rechercher un commentaire ou une réponse dans la section Mises à jour d’un objet.

1. Accédez à la section **Mises à jour** d’un objet.
1. Commencez à saisir un mot-clé <!--or a user's name --> dans la zone **Rechercher** dans le coin supérieur droit de l’onglet **Commentaires**.

   <!--Add this tip or note instead of the note below - when it'll be possible: You can search for users who have been tagged or for comment owners.-->

   >[!NOTE]
   >
   >Vous ne pouvez rechercher que des mots qui sont contenus dans le texte d’un commentaire ou d’une réponse. Vous ne pouvez pas rechercher les noms d’utilisateurs et utilisatrices ou d’équipes balisés dans une mise à jour.

   ![Rechercher dans des mises à jour](assets/updates-all-tabs-with-search-field.png)

   Le mot-clé <!--or user--> que vous avez recherché est mis en surbrillance et les commentaires qui le contiennent s’affichent en haut de la section Mises à jour.

   Workfront recherche dans l’ensemble du flux de mise à jour de l’objet, en dehors des commentaires visibles à l’écran.

1. Cliquez sur l’icône **x** dans le champ de recherche pour effacer les résultats de la recherche et revenir à tous les commentaires.

<!-- when we release search to production, check above and make sure you don't have to add that the users tagged/ owners are also searchable-->

## Copie de mises à jour

Il existe plusieurs façons de copier une mise à jour.

Vous pouvez copier un lien vers la mise à jour ou copier le contenu d’une mise à jour afin de l’utiliser dans une nouvelle mise à jour.

<!--Copying an update differs depending on which commenting experience you use.-->

<!--info for April 11: take the sentence above out and reword the section title below to: Copy an update-->

### Copier une mise à jour <!--in the new commenting experience-->

<!--For information about what features are available for the new commenting experience and for what objects, see [New commenting experience](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).-->

Vous pouvez copier des informations d’un commentaire existant en effectuant l’une des opérations suivantes :

* [Copier le lien](#copy-link)
* [Copier le texte du message](#copy-body-text)
* [Citer la réponse](#quote-reply)

![](assets/copy-comment-ways-from-more-menu-on-comment.png)

#### Copier le lien

L’option Copier le lien copie le lien du commentaire ou du thread dans le presse-papiers afin que vous puissiez partager le commentaire ou l’intégralité du thread avec d’autres utilisateurs et utilisatrices.

1. Accédez à la mise à jour dont vous souhaitez copier le lien.

1. Cliquez sur le menu **Plus**, puis sur **Copier le lien**.

1. Collez le lien que vous avez copié à l’étape précédente dans un e-mail ou une autre application pour le partager avec d’autres personnes. Le lien partagé ouvre le commentaire à partir duquel vous avez partagé le lien.

   >[!TIP]
   >
   >Lorsque vous partagez le lien d’une conversation sur un objet enfant à partir d’un objet de niveau supérieur, le lien ouvre le thread dans la zone Mises à jour de l’objet de niveau supérieur.
   >
   >Par exemple, si vous copiez le lien d’un commentaire de tâche dans la zone Mises à jour du projet, le commentaire ouvre la page du projet.

#### Copier le texte du message

L’option Copier le corps de texte copie le texte d’une mise à jour spécifique dans le presse-papiers.

1. Accédez à la mise à jour ou à la réponse que vous souhaitez copier.
1. Cliquez sur le menu **Plus**, puis sur **Copier le corps de texte**.

#### Citer la réponse

L’option Citer la réponse copie le commentaire d’origine dans une nouvelle réponse sous forme de citation.

1. Accédez à la mise à jour ou à la réponse que vous souhaitez copier.
1. Cliquez sur le menu **Plus**, puis sur **Citer la réponse**.

   Une nouvelle zone de commentaire s’ouvre et la réponse citée est incluse dans le nouveau commentaire et est marquée comme une citation.

   ![](assets/block-quote-highlighted-mid-comment-before-submit.png)


1. Continuez à ajouter votre mise à jour et cliquez sur **Soumettre** pour ajouter le commentaire.

<!--info for April 11: hide the entire section below - notice that there are several sub-sub sections below this main section - hide them all, all the way up to "Delete an update"-->

<!--
### Copy an update in the legacy commenting experience

* [Copy the update](#copy-the-update) 
* [Copy the thread link](#copy-the-thread-link) 
* [Copy the update link](#copy-the-update-link)
* [Quote Reply](#quote-reply)

   >[!TIP]
   >
   >When you copy and share the link of a conversation on a child object from a higher-ranking object, the link opens the thread in the child object's Updates area. 
   >
   >For example, if you copy the link of a task comment from the project's Updates area, the comment opens the task page.

#### Copy the update {#copy-the-update}

This option copies the text from a specific update to the clipboard.

1. Go to the update or reply you want to copy.
1. Click the **More** menu, then click **Copy body text**.

   ![](assets/update-stream-comment-menu-marked-350x152.png)

#### Copy the thread link {#copy-the-thread-link}

This option copies the full thread link to the clipboard so you can share the thread with other users.

1. Go to the update thread you want to copy.

1. Click the **More** menu, then click **Copy thread link**.

   ![](assets/update-stream-comment-menu-marked-350x152.png) 

1. Paste the link you copied in the previous step in an email or another application to share it with others. The shared link opens the comment you shared the link from. 

#### Copy the update link {#copy-the-update-link}

This option copies a specific update link to the clipboard. When you share the update link, the user who follows it sees a border around the update.

1. Go to the update or reply you want to copy.
1. Click the **More** menu next to the individual update, then click **Copy update link**.

   ![](assets/copy-update-link-old-ui.png)

1. Paste the link you copied in the previous step in an email or another application to share it with others. The shared link opens the comment you shared the link from. 

#### Quote Reply  

The Quote Reply option copies the original comment to a new reply as a block quote. 

1. Go to the update or reply you want to copy.
1. Click the **More** menu, then click **Quote Reply**.

   A new comment box opens and the quoted reply is included in the new comment and marked as a block quote.

1. Continue adding your update and click **Reply** to add the comment.
-->

## Supprimer une mise à jour ou une réponse

En fonction de l’accès que l’administrateur ou l’administratrice Workfront vous accorde, vous pouvez être en mesure de supprimer des mises à jour que vous avez ajoutées dans l’onglet Mises à jour d’un objet. Pour plus d’informations, consultez [Créer ou modifier des niveaux d’accès personnalisés](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md#creating-a-new-access-from-scratch) dans l’article [Créer ou modifier des niveaux d’accès personnalisés](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Aucune personne utilisant Workfront (y compris l’administrateur ou l’administratrice Workfront) ne peut supprimer les mises à jour effectuées par une autre personne. Cependant, si le niveau d’accès d’une personne lui permet de supprimer ses propres mises à jour, l’administrateur ou l’administratrice Workfront peut se connecter au nom de cette personne et supprimer les mises à jour qu’elle a effectuées. Pour plus d’informations, consultez [Créer ou modifier des niveaux d’accès personnalisés](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md#creating-a-new-access-from-scratch) et [Se connecter en tant qu’autre utilisateur ou utilisatrice](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).

1. Accédez à la mise à jour ou à la réponse que vous souhaitez supprimer.
1. Cliquez sur le bouton **Plus** en regard de la mise à jour ou de la réponse que vous souhaitez supprimer, puis cliquez sur **Supprimer**.

   ![](assets/update-stream-comment-menu-marked-350x152.png)

1. Dans le message qui apparaît, cliquez sur **Supprimer**.

   >[!NOTE]
   >
   >La suppression d’une mise à jour à laquelle une image est jointe supprime à la fois le commentaire et l’image. Pour plus d’informations, consultez [Utiliser du texte enrichi dans une mise à jour Workfront](#use-rich-text-in-a-workfront-update) dans cet article.

   Lorsque des réponses sont associées au commentaire que vous supprimez, il est indiqué que le commentaire a été supprimé avec le nom de l’utilisateur ou de l’utilisatrice qui l’a supprimé.

   ![](assets/removed-comment-indicator-new-experience.png)

   Les commentaires supprimés le sont immédiatement de Workfront. Un utilisateur ou une utilisatrice qui utilise la section Mises à jour voit la suppression d’un commentaire par une autre personne en temps réel.


## Vérifier les mises à jour du système

La section Mises à jour d’un objet Workfront affiche deux types d’informations :

* **Mises à jour de l’utilisateur :** Les mises à jour des utilisateurs sont des commentaires que vous et d’autres utilisateurs de votre système saisissez. Les mises à jour de l’utilisateur s’affichent dans les onglets Commentaires et Tous de la section Mises à jour .

  ![](assets/user-update-cl-350x277.png)

* **Mises à jour système :** Les mises à jour système enregistrent la suppression de tâches ou de problèmes, l’ajout ou la suppression de versions de document, l’ajout ou la suppression d’une demande d’approbation, ainsi que les modifications ou modifications apportées à l’objet. Les mises à jour système s’affichent dans l’activité système et dans les onglets Toutes de la section Mises à jour .

  ![](assets/system-updates-cl-350x277.png)

  Les administrateurs et administratrices Workfront peuvent déterminer ce qui est suivi dans les mises à jour du système, comme décrit dans la section [Mises à jour suivies par le système](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md). Vous pouvez également filtrer les mises à jour ou activités système afin de n’afficher que les mises à jour des utilisateurs et utilisatrices pour tous les objets.

  Les objets suivants ne comportent pas de mises à jour générées par le système :

   * Equipe
   * Modèle
   * Tâche de modèle
   * Carte ad hoc

Pour plus d’informations sur les mises à jour du système dans la section Mises à jour, voir [Présentation de la section Mises à jour](../updating-work-items-and-viewing-updates/updates-tab-overview.md).


<!--
After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>  
<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)</span>  
-->

<!-- with October 26 release: add somewhere this, and decide where we need to keep information about the legacy commenting. Should we create an article about iterations comments like we have for goals and cards?!:

>[!NOTE]
>
>Iterations display the legacy commenting experience.-->

<!--old message, before Auhust 17: 

>[!NOTE]
>
>We are currently redesigning the commenting experience in Adobe Workfront.
>
>For more information about the new commenting experience, see [New commenting experience](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 
>
>You can access the new experience for the following objects:
> * Issues, projects, tasks, and documents.
>
>     This is available when you enable the commenting Beta experience.
>
>     This functionality is available only for the Updates section, and it is not available for the following areas:
>
>     * Home
>     * Summary panel in lists
>     * Summary panel in timesheets
>
> * Goals, cards in the Boards area
>
>   The new commenting experience is the only experience for goals and cards. You must have an additional license to access Workfront Goals. For more information, see [Requirements to use Workfront Goals](../../workfront-goals/goal-management/access-needed-for-wf-goals.md). 
>
>     You can add and view updates to cards in the Boards area when you enable the Comments and System Activity sections on a card. For more information, see [Add an ad hoc card to a board](../../agile/get-started-with-boards/add-card-to-board.md).
-->