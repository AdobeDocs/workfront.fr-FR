---
user-type: administrator
product-area: system-administration;user-management
keywords: view,group,event,notifications,configure,enable,disable
navigation-topic: create-and-manage-groups
title: Affichage et configuration des notifications d’événement pour un groupe
description: En tant qu’administrateur de groupe, vous pouvez afficher les notifications d’événement qui sont activées pour un groupe que vous gérez. En outre, si un administrateur Adobe Workfront déverrouille une notification d’événement, vous pouvez la configurer pour un groupe de niveau supérieur que vous gérez. La configuration d’une notification d’événement consiste à l’activer ou la désactiver.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: a815aeb1-3403-4491-a8ad-7e47c519905c
source-git-commit: afbf2e2fbfcc2c527223da008518bc7632872c23
workflow-type: tm+mt
source-wordcount: '558'
ht-degree: 19%

---

# Affichage et configuration des notifications d’événement pour un groupe

En tant qu’administrateur de groupe, vous pouvez afficher les notifications d’événement qui sont activées pour un groupe que vous gérez.

En outre, si un administrateur Adobe Workfront déverrouille une notification d’événement, vous pouvez la configurer pour un groupe de niveau supérieur que vous gérez. La configuration d’une notification d’événement consiste à l’activer ou la désactiver.

Un administrateur Workfront peut également le faire pour n’importe quel groupe.

La configuration d’une notification d’événement pour un groupe affecte les utilisateurs pour lesquels ce groupe, ou l’un de ses sous-groupes, est leur groupe d’accueil. Dans leurs profils utilisateur, ces utilisateurs voient les notifications d’événement activées pour leur groupe d’accueil au lieu des notifications d’événement activées à l’échelle du système.

Pour plus d’informations sur la façon dont un administrateur Workfront déverrouille une notification d’événement, voir [Déverrouiller ou verrouiller la configuration des notifications d’événement pour tous les groupes](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md).

Pour plus d’informations sur le paramètre de notification par défaut d’un événement, voir [Types de notification d’événement](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

## Conditions d’accès

Vous devez disposer des éléments suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan Workfront*</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> <p>Vous devez être un administrateur ou une administratrice de groupe pour le groupe ou un administrateur ou une administratrice de Workfront. Pour plus d’informations, consultez les sections <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administrateurs et administratrices de groupe</a> et <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Accorder l’accès administratif complet à une personne</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour savoir votre plan ou type de licence, contactez l’administration de Workfront.

## Affichage et configuration des notifications d’événement d’un groupe

1. (Conditionnel et facultatif) Si vous êtes administrateur Workfront et que vous vous trouvez déjà sur la page Notifications par e-mail (Configuration > Email > Notifications), vous pouvez effectuer les opérations suivantes, puis passer à l’étape 6 : Supprimer **Notifications d’événement système** dans la zone située au-dessus de la liste, commencer à saisir le nom du groupe dans la zone, puis cliquer dessus lorsqu’il apparaît.
1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis sur **Configuration** ![](assets/gear-icon-settings.png).

1. Dans le panneau de gauche, cliquez sur **Groupes** ![](assets/groups-icon.png).

1. Cliquez sur le nom du groupe de niveau supérieur.
1. Dans le menu de gauche, cliquez sur **Notifications d’événement**.

   Dans la liste qui s’affiche, la colonne **Actif** sur la gauche indique les notifications qui sont actives (bleu) et inactives (gris) pour le groupe.

1. Pour activer ou désactiver une notification d’événement déverrouillée : cliquez sur le bouton dans la colonne <strong>Active</strong> pour activer <img src="assets/email-notification-enabled-unlocked.png"> ou désactiver <img src="assets/email-notification-disabled-unlocked.png">.

   >[!INFO]
   >
   >**Exemple :** Vous pouvez configurer les deux premières notifications d’événement de groupe marketing affichées ci-dessous qui ont été déverrouillées pour les groupes.</p> <p> <img src="assets/configure-group-event-notifications.png">
   >* Si un bouton de la colonne <strong>Actif</strong> est gris et grisé <img src="assets/email-notification-disabled-locked.png">, la notification d’événement est désactivée pour tous les utilisateurs et les administrateurs de groupe ne peuvent pas l’activer ni modifier l’objet de l’email.
   >* Si un bouton de la colonne <strong>Actif</strong> est gris et non grisé <img src="assets/email-notification-disabled-unlocked.png">, la notification d&#39;événement est <strong> désactivée pour tous les utilisateurs et les administrateurs de groupe </strong> peuvent l&#39;activer pour leurs groupes.
   >* Si un bouton de la colonne <strong>Actif</strong> est bleu et grisé <img src="assets/email-notification-enabled-locked.png">, la notification d’événement est activée pour tous les utilisateurs et les administrateurs de groupe ne peuvent pas la désactiver ni modifier l’objet de l’email pour leurs groupes.
   >* Si un bouton de la colonne <strong>Actif</strong> est bleu et n’est pas grisé <img src="assets/email-notification-enabled-unlocked.png">, la notification d&#39;événement est <strong> activée pour tous les utilisateurs et les administrateurs de groupe </strong> peuvent la désactiver pour leurs groupes.

<!--
This step (with substeps) is for functionality from a Sprint 3 2021 story that got put on hold. Also see the PDF on the story for some text earlier in the article that needs to be added. 

1. To customize the email subject line of an event notification,
  1. Click the name of the event notification.
  1. In the <strong>Event Notification</strong> box that displays, in the <strong>Email Subject Line</strong> box, change the text and fields, including custom fields, then click <strong>Update</strong> to save the new subject lines for your emails.
  IMPORTANT: The names of the fields added must match the camel case syntax of our database structure. For more information about how our objects and their fields are named in the Workfront database, see the <a href="../../../wf-api/workfront-api.md" class="MCXref xref">Adobe Workfront API</a>.
  For more information about customizing the email subject line of an event notification, see <a href="../../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md" class="MCXref xref">Customize email subjects for event notifications</a>. 
-->

