---
user-type: administrator
product-area: system-administration;user-management
keywords: vue,groupe,événement,notifications,configurer,activer,désactiver
navigation-topic: create-and-manage-groups
title: Affichage et configuration des notifications d’événement pour un groupe
description: En tant qu’administrateur ou administratrice de groupes, vous pouvez afficher les notifications d’événement qui sont activées pour un groupe que vous gérez. En outre, si un administrateur ou une administratrice Adobe Workfront déverrouille une notification d’événement, vous pouvez la configurer pour un groupe de niveau supérieur que vous gérez. La configuration d’une notification d’événement consiste à l’activer ou à la désactiver.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: a815aeb1-3403-4491-a8ad-7e47c519905c
source-git-commit: a42a167447d2f11b5502e4a0953b5e7eec2e67b1
workflow-type: tm+mt
source-wordcount: '523'
ht-degree: 83%

---

# Afficher et configurer des notifications d’événement pour un groupe

En tant qu’administrateur ou administratrice de groupes, vous pouvez afficher les notifications d’événement qui sont activées pour un groupe que vous gérez.

En outre, si un administrateur ou une administratrice Adobe Workfront déverrouille une notification d’événement, vous pouvez la configurer pour un groupe de niveau supérieur que vous gérez. La configuration d’une notification d’événement consiste à l’activer ou à la désactiver.

Un administrateur ou une administratrice Workfront peut également le faire pour n’importe quel groupe.

La configuration d’une notification d’événement pour un groupe affecte les personnes dont ce groupe, ou l’un de ses sous-groupes, est le groupe principal. Dans leurs profils d’utilisateur ou d’utilisatrice, ces personnes voient les notifications d’événement activées pour leur groupe principal au lieu des notifications d’événement activées à l’échelle du système.

Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront déverrouille une notification d’événement, voir [Déverrouiller ou verrouiller la configuration des notifications d’événement pour tous les groupes](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md).

Pour plus d’informations sur le paramètre de notification par défaut d’un événement, voir [Types de notification d’événement](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Package Adobe Workfront</td> 
   <td><p>Tous</p></td> 
  </tr> 
  <tr> 
   <td>Licence Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr>
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td>Vous devez être un administrateur de groupe du groupe ou un administrateur système.</td>
  </tr>
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Afficher et configurer les notifications d’événement d’un groupe

>[!TIP]
>
>Si vous êtes un administrateur Workfront et que vous êtes déjà sur la page Notifications par e-mail (Configuration > E-mail > Notifications), vous pouvez effectuer les opérations suivantes, puis passer à l’étape 6 : Supprimer **Notifications d’événement système** dans la zone située au-dessus de la liste, commencez à saisir le nom du groupe dans la zone, puis cliquez dessus lorsqu’il apparaît.

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Groupes** ![Groupes](assets/groups-icon.png).

1. Cliquez sur le nom du groupe de niveau supérieur.
1. Dans le menu de gauche, cliquez sur **Notifications d’événement**.

   Dans la liste qui s’affiche, la colonne **Actif** de gauche indique les notifications actives (bleu) et inactives (gris) pour le groupe.

1. Pour activer ou désactiver une notification d’événement déverrouillée, cliquez sur le bouton dans la colonne <strong>Actif</strong> pour l’activer <img src="assets/email-notification-enabled-unlocked.png"> ou la désactiver <img src="assets/email-notification-disabled-unlocked.png">.

   >[!INFO]
   >
   >**Exemple :** vous pouvez configurer les deux premières notifications d’événement de groupe marketing affichées ci-dessous qui ont été déverrouillées pour les groupes.</p> <p> <img src="assets/configure-group-event-notifications.png">
   >* Si un bouton dans la colonne <strong>Actif</strong> est gris et grisé <img src="assets/email-notification-disabled-locked.png">, la notification d’événement est désactivée pour toutes les personnes et les administrateurs et administratrices de groupe ne peuvent pas l’activer ni modifier l’objet de l’e-mail.
   >* Si un bouton dans la colonne <strong>Actif</strong> est gris et non grisé <img src="assets/email-notification-disabled-unlocked.png">, la notification d’événement est <strong>désactivée pour toutes les personnes et</strong> les administrateurs et administratrices de groupes peuvent l’activer pour leurs groupes.
   >* Si un bouton dans la colonne <strong>Actif</strong> est bleu et grisé <img src="assets/email-notification-enabled-locked.png">, la notification d’événement est activée pour toutes les personnes et les administrateurs et administratrices de groupes ne peuvent pas la désactiver ni modifier l’objet de l’e-mail pour leurs groupes.
   >* Si un bouton dans la colonne <strong>Actif</strong> est bleu et non grisé <img src="assets/email-notification-enabled-unlocked.png">, la notification d’événement est <strong>activée pour toutes les personnes et</strong> les administrateurs et administratrices de groupes peuvent la désactiver pour leurs groupes.

<!--
This step (with substeps) is for functionality from a Sprint 3 2021 story that got put on hold. Also see the PDF on the story for some text earlier in the article that needs to be added. 

1. To customize the email subject line of an event notification,
  1. Click the name of the event notification.
  1. In the <strong>Event Notification</strong> box that displays, in the <strong>Email Subject Line</strong> box, change the text and fields, including custom fields, then click <strong>Update</strong> to save the new subject lines for your emails.
  IMPORTANT: The names of the fields added must match the camel case syntax of our database structure. For more information about how our objects and their fields are named in the Workfront database, see the <a href="../../../wf-api/workfront-api.md" class="MCXref xref">Adobe Workfront API</a>.
  For more information about customizing the email subject line of an event notification, see <a href="../../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md" class="MCXref xref">Customize email subjects for event notifications</a>. 
-->

