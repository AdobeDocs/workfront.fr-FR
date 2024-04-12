---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Balisage des autres sur les mises à jour
description: Lorsque vous fournissez des commentaires de mise à jour sur un objet Adobe Workfront, tous les utilisateurs du projet peuvent voir les informations envoyées. Cependant, il peut arriver que des utilisateurs qui ne se trouvent pas sur le projet aient intérêt à consulter ces informations. Plutôt que d’inclure ces utilisateurs dans le projet, vous pouvez les baliser sur la mise à jour pour les partager avec eux. Les utilisateurs balisés reçoivent une notification d’événement.
author: Alina
feature: Get Started with Workfront
exl-id: c4c0d74f-ac50-4fc5-89d6-28f004c25b29
source-git-commit: 886b5d9084cb1bfb63157152f05fa20128d34903
workflow-type: tm+mt
source-wordcount: '997'
ht-degree: 0%

---

# Balisage des autres sur les mises à jour

<!--Audited: April, 2024-->

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

Vous pouvez baliser les utilisateurs lors d’une mise à jour d’un objet si vous souhaitez attirer leur attention sur un objet qu’ils n’auraient pas normalement suivi.

Plutôt que d’inclure ces utilisateurs dans l’objet en les y affectant ou en les abonnant, vous pouvez les baliser sur la mise à jour pour les partager avec eux. Les utilisateurs balisés reçoivent une notification Workfront à propos de la mise à jour que vous avez saisie. En fonction de leurs paramètres de notification, ils reçoivent également un e-mail sur la mise à jour que vous avez saisie.

## Remarques concernant le balisage des utilisateurs dans les mises à jour

* Les utilisateurs balisés dans les mises à jour doivent activer une notification personnelle dans leur profil pour qu’ils puissent recevoir la notification par e-mail. Pour plus d’informations, voir [Modifier vos propres notifications électroniques](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

  Pour plus d’informations sur l’ajout de mises à jour aux objets Workfront, voir [Mise à jour du travail](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

* Lorsqu’un problème est converti en projet ou tâche, les mises à jour sont copiées dans le nouveau projet ou la nouvelle tâche, mais pas les utilisateurs balisés. Pour continuer la conversation, vous devez marquer à nouveau les participants.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Formule Adobe Workfront</strong></td> 
   <td> <p>Quelconque</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licence Adobe Workfront*</strong></td> 
   <td> <p>Nouveau : contributeur ou version ultérieure pour les problèmes et documents ; clair ou supérieur pour tous les autres objets</p>
   <p>Actuel : demande ou version ultérieure pour les problèmes et les documents ; vérification ou version ultérieure pour tous les autres objets</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuration du niveau d’accès</strong></td> 
   <td> <p>Affichage ou accès supérieur aux objets dans lesquels vous souhaitez publier la réponse</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisation d’objet</strong></td> 
   <td> <p>Afficher ou des autorisations supérieures aux objets dans lesquels vous souhaitez publier la réponse</p> </td> 
  </tr> 
 </tbody> 
</table>

*Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront. Pour plus d’informations, voir [Exigences d’accès à la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Balisage des autres sur les mises à jour

Vous pouvez baliser d’autres utilisateurs sur les mises à jour de la manière suivante :

* **Automatiquement**: lorsqu’un utilisateur lance un thread, ajoute un commentaire ou ajoute une réponse, il est automatiquement balisé et ajouté à la zone Baliser les personnes ou les équipes de la zone de commentaire. <!--remove the tip below when the new commenting stream is the only stream and the legacy commenting is removed-->

* **Manuellement**: lorsque vous ajoutez manuellement un utilisateur à la zone Baliser les personnes de la zone de commentaire.

Vous pouvez également supprimer les utilisateurs balisés par erreur lorsque vous modifiez ou répondez à un commentaire.

1. Commencez à mettre à jour un élément de travail, comme décrit dans la section [Mise à jour du travail](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). En tant que propriétaire de commentaire, vous êtes automatiquement balisé et ajouté à la zone Baliser les personnes ou les équipes de la zone de commentaire.

   >[!TIP]
   >
   >Le propriétaire du commentaire ne peut pas voir son propre nom dans la zone Baliser les personnes ou les équipes de la zone de commentaire.

1. Dans le **Balisage de personnes ou d’équipes** , commencez à saisir le nom de l’utilisateur ou de l’équipe que vous souhaitez inclure, puis cliquez sur le nom lorsqu’il apparaît dans la liste déroulante.

   Ou

   Saisissez le symbole @ dans la zone **Rédiger un commentaire** , commencez à saisir le nom de l’utilisateur ou de l’équipe à inclure dans la mise à jour, puis cliquez sur le nom lorsqu’il apparaît dans la liste déroulante.

   >[!TIP]
   > 
   >Pour identifier le bon utilisateur lorsqu’il existe des utilisateurs portant des noms similaires ou identiques, notez l’avatar, le rôle de Principal de l’utilisateur ou son adresse électronique.
   > 
   >Les utilisateurs doivent être associés à au moins un rôle de tâche pour l’afficher au fur et à mesure que vous les marquez dans une mise à jour.
   > 
   >Pour que les utilisateurs puissent afficher les courriers électroniques de leurs utilisateurs, le paramètre Afficher les coordonnées doit être activé dans votre niveau d’accès. Pour plus d’informations, voir [Accorder l’accès aux utilisateurs](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

   ![Balisage d’un utilisateur](assets/tag-others-unified-commenting-with-all-tab.png)

1. (Facultatif) Pour rendre la mise à jour privée, activez **Privé à ma société** dans le coin inférieur droit de la zone de mise à jour. La mise à jour est ainsi visible uniquement par les utilisateurs de votre entreprise. La variable **Privé à ma société** est disponible uniquement lorsqu’une société est spécifiée dans votre profil Workfront.

   >[!NOTE]
   >
   >* Cette option s’affiche uniquement lorsque l’utilisateur est associé à une entreprise.
   >* Les utilisateurs balisés en dehors de l’entreprise peuvent toujours recevoir une notification ou un courrier électronique in-app, même s’ils ne verront pas les commentaires privés sur l’onglet Mises à jour . Nous vous recommandons de ne pas baliser les utilisateurs externes lors d’une mise à jour si vous ne souhaitez pas partager les informations avec eux.

1. (Facultatif) Pour ajouter plusieurs utilisateurs et équipes, répétez l’étape 2. <!--insure this stays accurate-->

   >[!NOTE]
   >
   >Tous les utilisateurs et membres de l’équipe répertoriés dans le champ &quot;Baliser les personnes ou les équipes&quot; reçoivent une notification in-app pour la mise à jour et peuvent recevoir un e-mail, selon la configuration de leurs paramètres de notification par e-mail. Les utilisateurs qui se marquent dans un commentaire ou une réponse reçoivent une notification pour ce commentaire ou cette réponse et peuvent voir leur nom dans la liste en tant que membre du thread pour le reste du thread, mais ils ne reçoivent pas une autre notification à moins qu’ils ne se balisent à nouveau. Pour plus d’informations, voir [Modifier vos propres notifications électroniques](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md) et [Configuration des notifications d’événement pour tous les membres du système](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

1. Cliquez sur **Envoyer**.\
   Les utilisateurs inclus dans la mise à jour se voient automatiquement accorder l’autorisation Afficher à l’objet et peuvent afficher les mises à jour apportées à l’objet et y répondre.

   Les noms des entités balisées s’affichent en regard de leurs avatars, jusqu’à deux entités. Si plus de deux entités sont balisées, le nom du premier s’affiche, en plus du nombre d’autres entités balisées.

   ![](assets/members-icons-expanded-unshimmed.png)

   Lorsque vous êtes balisé dans le texte du commentaire, votre nom est surligné dans ces commentaires.

   Pour plus d’informations sur les fonctionnalités supplémentaires disponibles lors de la mise à jour d’un élément de travail, voir [Mise à jour du travail](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

1. (Facultatif) Cliquez sur le **Plus** menu ![](assets/more-menu.png) dans le coin supérieur droit du commentaire, puis cliquez sur **Modifier**. Supprimez les utilisateurs balisés, puis cliquez sur **Envoyer**.

   >[!IMPORTANT]
   >
   >Vous ne pouvez modifier un commentaire que dans les 15 minutes qui suivent sa saisie. Vous ne pouvez modifier que les commentaires que vous avez ajoutés.


<!--
   >[!TIP]
   >
   >When using the legacy commenting experience to add comments and replies, comment owners that were not specifically tagged cannot be manually removed by people who use the new commenting experience.
-->

<!--
### Tag others on updates in the legacy Updates section

You can manually tag users in the legacy Updates section. 

1. Begin updating a work item, as described in [Update work](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. In the **Notify** field, begin typing the name of the user or team you want to include, then click the name when it appears in the drop-down list.

   Or

   Type the @ symbol in the **Start a new update** area, begin typing the name of the user or team you want to include on the update, then click the name when it appears in the drop-down list.

   >[!TIP]
   >
   >To identify the correct user when there are users with similar or identical names, notice the avatar, the user's Primary Role, or their email address. 
   >
   >Users must be associated with at least one job role to view it as you tag them in an update. 
   >
   >You must have the View Contact Info setting enabled in your access level for Users to view users' emails. For information, see [Grant access to users](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

   ![](assets/tag-users-in-update.png)

1. (Optional) To make the update private, enable **Private to my company** in the lower-right corner of the update box. This makes the update visible just to users in your company. The **Private to my company** option is available only when a Company is specified in your Workfront profile. 

   >[!NOTE]
   >
   >Tagged users outside the company could still receive an in-app notification or email, even though they will not see the private comments on the Updates tab. We recommend not to tag external users on an update if you do not want to share the information with them.  

1. (Optional) To add multiple users and teams, repeat step 2.

   >[!NOTE]
   >
   >All users and team members listed in the Notify field receive an in-app notification for the update and might receive an email, depending on the configuration of their email notification settings. Users who tag themselves in a comment or reply receive a notification for that comment or reply and can see their name in the Notify field for the remainder of the thread, but they do not receive another notification unless they tag themselves again. For more information, see [Modify your own email notifications](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md) and [Configure event notifications for everyone in the system](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

1. Click **Update**.  
   Users included in the update are automatically granted View permission to the object and can view and respond to updates made to the object.

   You can see who has been tagged in each reply at the top of the update thread. These users, along with any users subscribed to the object, receive a notification whenever an update or reply is made on the object.

   ![](assets/tagging-transparency-350x192.png)
-->

Pour plus d’informations sur les fonctionnalités supplémentaires disponibles lors de la mise à jour d’un élément de travail, voir [Mise à jour du travail](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).



