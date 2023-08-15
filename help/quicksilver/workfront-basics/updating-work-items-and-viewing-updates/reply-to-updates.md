---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Répondre aux mises à jour
description: Lorsqu’une personne ajoute ou répond à une mise à jour d’un objet de travail, sa réponse apparaît dans le fil de communication de la section Mises à jour de l’objet. Vous pouvez ajouter une réponse à une mise à jour ou aimer si vous disposez de l’accès Affichage à l’objet.
author: Lisa and Alina
feature: Get Started with Workfront
role: User
topic: Collaboration
exl-id: a8271f3c-7a08-4eb3-aaff-deb250f5af73
source-git-commit: d93d42322d62ff5eb927ca13febcb763cbec3f13
workflow-type: tm+mt
source-wordcount: '1052'
ht-degree: 0%

---

# Répondre aux mises à jour

<!--take "Beta" references out when we remove the beta and change "current" to "legacy" after October 26-->

<!--after August 17: 
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers, or in the Production environment for customers who enabled fast releases. </span>  
<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/enable-fast-release-process.html?lang=en ). </span>  
<span class="preview">For information about the current release, see [Fourth Quarter 2023 release overview](../../../product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md). </span>-->

<!--replace the note below with this at August 17: 
>[!NOTE]
>
>We are currently redesigning the commenting experience in Adobe Workfront.
>Depending on what environment and what objects you access the commenting experience from, you might see different functionality in the Updates section. 
>For more information about the new commenting experience and its availability, see [New commenting experience](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 
>
>The new commenting experience is available only for the Updates section, and it is not available for the following areas:
>
> * Home
> * Summary panel in lists
> * Summary panel in timesheets

-->

>[!NOTE]
>
>Nous sommes en train de reconcevoir l’expérience de commentaire dans Adobe Workfront.
>
>Pour plus d’informations sur la nouvelle expérience de commentaire, voir [Nouvelle expérience de commentaire](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).
>
>Vous pouvez accéder à la nouvelle expérience pour les objets suivants :
> * Problèmes, projets, tâches et documents.
>
>     Cette option est disponible lorsque vous activez l’expérience bêta de commentaire.
>
>     Cette fonctionnalité est disponible uniquement pour la section Mises à jour et elle ne l’est pas pour les zones suivantes :
>
>     * Page d’accueil
>     * Panneau Résumé dans les listes
>     * Panneau Résumé dans les feuilles de temps
>
> * Objectifs, cartes dans la zone Panoramas
>
>   La nouvelle expérience de commentaire est la seule expérience pour les objectifs et les cartes. Vous devez disposer d’une licence supplémentaire pour accéder aux objectifs de Workfront. Pour plus d’informations, voir [Conditions requises pour utiliser les objectifs Workfront](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
>
>     Vous pouvez ajouter et afficher des mises à jour aux cartes dans la zone Panoramas lorsque vous activez les sections Commentaires et Activité système sur une carte. Pour plus d’informations, voir [Ajouter une carte ad hoc à un panorama](../../agile/get-started-with-boards/add-card-to-board.md).


Lorsqu’une personne répond à un commentaire ou à une mise à jour système sur un objet de travail, sa réponse apparaît dans le fil de communication de la section Mises à jour de l’objet.

>[!IMPORTANT]
>
>Il n’est pas possible de répondre aux mises à jour du système dans la nouvelle expérience de commentaire. Pour plus d’informations, voir [Nouvelle expérience de commentaire](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).


## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Formule Adobe Workfront*</strong></td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licence Adobe Workfront*</strong></td> 
   <td> <p>Demande ou version ultérieure pour les problèmes et les documents ; révision ou version ultérieure pour tous les autres objets</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Paramétrages du niveau d'accès*</strong></td> 
   <td> <p>Demandeur ou supérieur pour les problèmes et les documents ; Réviseur ou supérieur pour tous les autres objets</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet</strong></td> 
   <td> <p>Afficher l’accès à l’objet</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Répondre à une mise à jour ou à une réponse dans Workfront

Vous pouvez répondre à un commentaire dans le fil d’un objet que vous pouvez afficher ou vous connecter en tant qu’administrateur Workfront ou de groupe et répondre à un commentaire au nom d’un autre utilisateur. Pour plus d’informations, voir [Connexion en tant qu’autre utilisateur](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).

La réponse à un commentaire ou à une réponse varie en fonction de l’expérience et de l’objet que vous sélectionnez.

### Répondre à une mise à jour ou répondre dans la section Mises à jour actuelles

1. Accédez à l’objet auquel vous souhaitez ajouter une réponse.
1. Sur le **Mises à jour** pour l’objet, recherchez la mise à jour ou la réponse à laquelle vous souhaitez répondre.

1. (Facultatif) Pour afficher une image dans la mise à jour existante, effectuez l’une des opérations suivantes :

   * Cliquez sur le bouton **Aperçu** icon ![](assets/previewimageicon-31x31.png) sur la miniature de l’image pour ouvrir l’image en taille réelle dans un nouvel onglet du navigateur.
   * Cliquez sur le bouton **Télécharger** icon ![](assets/downloadimageicon.png) sur la miniature de l’image pour télécharger l’image.

1. Cliquez sur **Répondre** lors de la mise à jour, saisissez une réponse dans la zone qui s’affiche.

   Vous pouvez voir les utilisateurs qui participent activement à la conversation ou qui sont balisés dans chaque réponse en haut de ce fil de mise à jour. Ces utilisateurs, ainsi que tous les utilisateurs abonnés à l’objet, reçoivent une notification chaque fois qu’une mise à jour ou une réponse est apportée à l’objet. Vous pouvez également baliser d’autres utilisateurs pour les inclure dans votre réponse.  Pour baliser davantage d’utilisateurs, voir [Balisage des autres sur les mises à jour](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

   ![](assets/tagging-transparency-350x192.png)

1. (Facultatif) Pour inclure le texte d’une mise à jour précédente dans votre réponse, cliquez sur le bouton **Plus** en regard de la mise à jour ou de la réponse que vous souhaitez citer, cliquez sur **Réponse de devis**. Le texte de la mise à jour précédente apparaît dans la zone de saisie, marquée d’une ligne grise verticale.
1. (Facultatif) Utilisez le formatage, les émoticônes, incluez des liens ou des images, comme expliqué dans la section &quot;Utiliser du texte enrichi dans une mise à jour Workfront&quot; de l’article. [Mise à jour du travail](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. Cliquez sur **Répondre** pour enregistrer la réponse.

### Répondre à un commentaire lors de l’utilisation de la nouvelle expérience de commentaire

Pour plus d’informations sur les fonctionnalités disponibles dans la nouvelle expérience de commentaire et sur les objets, voir [Nouvelle expérience de commentaire](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

1. Accédez à l’objet auquel vous souhaitez ajouter une réponse.
1. Cliquez sur **Mises à jour**, puis cliquez sur le bouton **Commentaires** pour l’objet et recherchez le commentaire ou la réponse à laquelle vous souhaitez répondre.
1. (Facultatif) Pour inclure le texte d’une mise à jour précédente dans votre réponse, cliquez sur le bouton **Plus** en regard de la mise à jour ou de la réponse que vous souhaitez citer <!--(replace placing of the More menu - August 17) <span class="preview">in the upper-right corner of the comment you want to reply to</span>-->, puis cliquez sur **Réponse entre guillemets**. Le texte de la mise à jour précédente apparaît dans la zone de saisie, marquée d’une ligne grise verticale.
1. Cliquez sur **Répondre**.

   Vous pouvez voir les utilisateurs qui participent activement à la conversation en bas de la page **Nouveau commentaire** et vous pouvez ajouter d’autres éléments ou supprimer ceux qui ne sont plus pertinents. Ces utilisateurs, ainsi que tous les utilisateurs abonnés à l’objet, reçoivent une notification chaque fois qu’une mise à jour ou une réponse est apportée à l’objet. Vous pouvez également baliser d’autres utilisateurs pour les inclure dans votre réponse.  Pour baliser davantage d’utilisateurs, voir [Balisage des autres sur les mises à jour](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

1. Commencez à saisir votre réponse et utilisez toutes les options supplémentaires de la barre d’outils Texte enrichi. Pour plus d’informations sur l’utilisation du texte enrichi ou d’autres fonctionnalités de mise à jour, voir [Mise à jour du travail](../updating-work-items-and-viewing-updates/update-work.md).

1. Cliquez sur **Envoyer** pour enregistrer la réponse.

1. (Facultatif) Cliquez sur le **Plus** menu ![](assets/more-menu.png) en regard de la mise à jour <!--(replace placing of the More menu - August 17) <span class="preview">in the upper-right corner of the comment you want to reply to</span>--> pour plus d’options de gestion de la réponse. Pour plus d’informations, voir [Mise à jour du travail](../updating-work-items-and-viewing-updates/update-work.md).


## Réponse à une mise à jour à partir d’une notification par email

Selon le mode de configuration de vos notifications électroniques, vous pouvez recevoir une notification par courrier électronique lorsqu’une mise à jour est effectuée sur certains objets auxquels vous avez accès.

Vous pouvez répondre à une mise à jour à partir d&#39;une notification par email de la manière suivante :

* Répondez à l’email que vous recevez. Votre email de réponse est ajouté en tant que réponse Workfront au commentaire d’origine.
* Utilisez le bouton Commentaire dans le courrier électronique pour revenir à Workfront et répondre à la mise à jour dans la zone Mises à jour.

Voici un exemple de notification par email déclenchée suite à une mise à jour effectuée dans l&#39;onglet Mises à jour d&#39;une tâche :

![email.png](assets/email-350x202.png)

Pour plus d’informations, voir [Répondre aux notifications par e-mail](../updating-work-items-and-viewing-updates/reply-to-email-notifications.md).






