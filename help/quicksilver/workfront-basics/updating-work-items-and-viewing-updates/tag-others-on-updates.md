---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Balisage des autres sur les mises à jour
description: Lorsque vous fournissez des commentaires de mise à jour sur un objet Adobe Workfront, tous les utilisateurs du projet peuvent voir les informations envoyées. Cependant, il peut arriver que des utilisateurs qui ne se trouvent pas sur le projet aient intérêt à consulter ces informations. Plutôt que d’inclure ces utilisateurs dans le projet, vous pouvez les baliser sur la mise à jour pour les partager avec eux. Les utilisateurs balisés reçoivent une notification d’événement.
author: Alina
feature: Get Started with Workfront
exl-id: c4c0d74f-ac50-4fc5-89d6-28f004c25b29
source-git-commit: 56ab6fe79fe6e10be2ec61cb16ff48b30856dc0f
workflow-type: tm+mt
source-wordcount: '1621'
ht-degree: 0%

---

# Balisage des autres sur les mises à jour

{{highlighted-preview}}

<!--take new commenting and legacy commenting out when we remove the legacy commenting and the new one is the only experience-->

<!--

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>  
<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)</span>  

<span class="preview">For information about the current release schedule, see [Fourth Quarter 2023 release overview](../../product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md)</span> 
-->

>[!IMPORTANT]
>
>Nous sommes en train de reconcevoir l’expérience de commentaire dans Adobe Workfront.
>
>Selon les objets pour lesquels vous accédez à l’expérience de commentaire, les fonctionnalités suivantes peuvent s’afficher dans la section Mises à jour :
>* La nouvelle expérience
>* L’expérience héritée
>* L’expérience nouvelle et héritée
>
>Pour plus d’informations sur la nouvelle expérience de commentaire et sa disponibilité, voir [Nouvelle expérience de commentaire](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).
>
>La nouvelle expérience de commentaire n’est disponible que pour la section Mises à jour des objets Workfront et n’est pas disponible lorsque vous accédez aux objets à partir des zones suivantes :
>
> * Page d’accueil
> * Panneau Résumé dans les listes
> * Panneau Résumé dans les feuilles de temps
> * Panneau Résumé de l’équilibreur de charge de travail
>
><span class="preview">La nouvelle expérience de commentaire est disponible dans le panneau Résumé dans les listes, les feuilles de temps et l’équilibreur de charge de travail dans l’environnement Aperçu.</span>

Vous pouvez baliser les utilisateurs lors d’une mise à jour d’un objet si vous souhaitez attirer leur attention sur un objet qu’ils n’auraient pas normalement suivi.

Plutôt que d’inclure ces utilisateurs dans l’objet en les y affectant ou en les abonnant, vous pouvez les baliser sur la mise à jour pour les partager avec eux. Les utilisateurs balisés reçoivent une notification concernant la mise à jour que vous avez saisie.

## Remarques concernant le balisage des utilisateurs dans les mises à jour

* Les utilisateurs balisés dans les mises à jour doivent activer une notification personnelle dans leur profil pour qu’ils puissent recevoir la notification par e-mail. Pour plus d’informations, voir [Modifier vos propres notifications électroniques](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

  Pour plus d’informations sur l’ajout de mises à jour aux objets Workfront, voir [Mise à jour du travail](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

* Lorsqu’un problème est converti en projet ou tâche, les mises à jour sont copiées dans le nouveau projet ou la nouvelle tâche, mais pas les utilisateurs balisés. Pour continuer la conversation, vous devez marquer à nouveau les participants.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Formule Adobe Workfront*</strong></td> 
   <td> <p>Quelconque</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licence Adobe Workfront*</strong></td> 
   <td> <p>Demande ou version ultérieure pour les problèmes et les documents ; révision ou version ultérieure pour tous les autres objets</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Paramétrages du niveau d'accès*</strong></td> 
   <td> <p>Demandeur ou supérieur pour les problèmes et les documents ; Réviseur ou supérieur pour tous les autres objets</p> 
   <p><b>NOTE</b>

Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet</strong></td> 
   <td> <p>Afficher l’accès à l’objet</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Balisage des autres sur les mises à jour

Le balisage des autres dans une mise à jour varie en fonction de l’expérience et de l’objet sélectionné.

### Balisage des autres sur les mises à jour de la nouvelle expérience de commentaire

Vous pouvez baliser d’autres utilisateurs sur les mises à jour de la nouvelle expérience de commentaires en procédant comme suit :

* **Automatiquement**: lorsqu’un utilisateur lance un thread, ajoute un commentaire ou ajoute une réponse, il est automatiquement balisé et ajouté à la zone Baliser les personnes ou les équipes de la zone de commentaire. <!--remove the tip below when the new commenting stream is the only stream and the legacy commenting is removed-->

  >[!TIP]
  >
  >Lorsque le thread commence dans l’expérience de commentaire héritée, les participants au thread ne sont pas automatiquement balisés.

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

   <div class="preview">

   Exemple de balisage dans l’environnement Aperçu :
   ![Balisage d’un utilisateur](assets/tag-others-unified-commenting-with-all-tab.png)

   </div>

   Exemple de balisage dans l’environnement de production :
   ![](assets/tag-others-unified-commenting.png)

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

   Pour plus d’informations sur les fonctionnalités supplémentaires disponibles lors de la mise à jour d’un élément de travail, voir [Mise à jour du travail](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

1. (Facultatif) Cliquez sur le **Plus** menu ![](assets/more-menu.png) dans le coin supérieur droit du commentaire, puis cliquez sur **Modifier**. Supprimez les utilisateurs balisés, puis cliquez sur **Envoyer**. Vous ne pouvez modifier un commentaire que dans les 15 minutes qui suivent sa saisie. Vous ne pouvez modifier que les commentaires que vous avez ajoutés.

   >[!TIP]
   >
   >Lors de l’utilisation de l’expérience de commentaire héritée pour ajouter des commentaires et des réponses, les propriétaires de commentaires qui n’ont pas été spécifiquement balisés ne peuvent pas être supprimés manuellement par les personnes qui utilisent la nouvelle expérience de commentaire.


### Balisage des autres mises à jour dans la section Mises à jour héritées

Vous pouvez baliser manuellement les utilisateurs dans la section Mises à jour héritées .

1. Commencez à mettre à jour un élément de travail, comme décrit dans la section [Mise à jour du travail](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. Dans le **Notifier** , commencez à saisir le nom de l’utilisateur ou de l’équipe que vous souhaitez inclure, puis cliquez sur le nom lorsqu’il apparaît dans la liste déroulante.

   Ou

   Saisissez le symbole @ dans la zone **Démarrer une nouvelle mise à jour** , commencez à saisir le nom de l’utilisateur ou de l’équipe à inclure dans la mise à jour, puis cliquez sur le nom lorsqu’il apparaît dans la liste déroulante.

   >[!TIP]
   >
   >Pour identifier le bon utilisateur lorsqu’il existe des utilisateurs portant des noms similaires ou identiques, notez l’avatar, le rôle de Principal de l’utilisateur ou son adresse électronique.
   >
   >Les utilisateurs doivent être associés à au moins un rôle de tâche pour l’afficher au fur et à mesure que vous les marquez dans une mise à jour.
   >
   >Pour que les utilisateurs puissent afficher les courriers électroniques de leurs utilisateurs, le paramètre Afficher les coordonnées doit être activé dans votre niveau d’accès. Pour plus d’informations, voir [Accorder l’accès aux utilisateurs](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

   ![](assets/tag-users-in-update.png)

1. (Facultatif) Pour rendre la mise à jour privée, activez **Privé à ma société** dans le coin inférieur droit de la zone de mise à jour. La mise à jour est ainsi visible uniquement par les utilisateurs de votre entreprise. La variable **Privé à ma société** est disponible uniquement lorsqu’une société est spécifiée dans votre profil Workfront.

   >[!NOTE]
   >
   >Les utilisateurs balisés en dehors de l’entreprise peuvent toujours recevoir une notification ou un courrier électronique in-app, même s’ils ne verront pas les commentaires privés sur l’onglet Mises à jour . Nous vous recommandons de ne pas baliser les utilisateurs externes lors d’une mise à jour si vous ne souhaitez pas partager les informations avec eux.

1. (Facultatif) Pour ajouter plusieurs utilisateurs et équipes, répétez l’étape 2.

   >[!NOTE]
   >
   >Tous les utilisateurs et membres de l’équipe répertoriés dans le champ Notifier reçoivent une notification in-app pour la mise à jour et peuvent recevoir un courrier électronique, selon la configuration de leurs paramètres de notification électronique. Les utilisateurs qui se balisent dans un commentaire ou une réponse reçoivent une notification pour ce commentaire ou cette réponse et peuvent voir leur nom dans le champ Notifier pour le reste du thread, mais ils ne reçoivent aucune autre notification à moins qu’ils ne se balisent à nouveau. Pour plus d’informations, voir [Modifier vos propres notifications électroniques](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md) et [Configuration des notifications d’événement pour tous les membres du système](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

1. Cliquez sur **Mettre à jour**.\
   Les utilisateurs inclus dans la mise à jour se voient automatiquement accorder l’autorisation Afficher à l’objet et peuvent afficher les mises à jour apportées à l’objet et y répondre.

   Vous pouvez voir qui a été balisé dans chaque réponse en haut du fil de mise à jour. Ces utilisateurs, ainsi que tous les utilisateurs abonnés à l’objet, reçoivent une notification chaque fois qu’une mise à jour ou une réponse est apportée à l’objet.

   ![](assets/tagging-transparency-350x192.png)

   Pour plus d’informations sur les fonctionnalités supplémentaires disponibles lors de la mise à jour d’un élément de travail, voir [Mise à jour du travail](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).



