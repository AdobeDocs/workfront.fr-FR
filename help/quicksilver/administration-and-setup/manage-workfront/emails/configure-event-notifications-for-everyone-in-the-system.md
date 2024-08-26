---
title: Configuration des notifications d’événement pour tout le monde dans le système
description: Les notifications d’événements déclenchent l’envoi d’e-mails aux utilisateurs et utilisatrices lorsqu’un certain événement se produit. En tant qu’administrateur ou administratrice Adobe Workfront ou utilisateur ou utilisatrice ayant un niveau d’accès Planificateur ou planificatrice, vous pouvez configurer une notification d’événement pour toutes les personnes utilisant le système. La configuration d’une notification d’événement consiste à l’activer ou la désactiver.
author: Nolan
feature: System Setup and Administration
role: Admin
exl-id: 027ecebd-d9de-4cdd-b15a-88de18367591
source-git-commit: ab774e937a15aaa04704e872579df880a9b80aaf
workflow-type: tm+mt
source-wordcount: '584'
ht-degree: 98%

---

# Configurer les notifications d’événements pour toutes les personnes utilisant le système

<!-- Audited: 1/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS-->

Les notifications d’événements déclenchent l’envoi d’e-mails aux utilisateurs et utilisatrices lorsqu’un certain événement se produit. En tant qu’administrateur ou administratrice Adobe Workfront ou utilisateur ou utilisatrice ayant un niveau d’accès Planificateur ou planificatrice, vous pouvez configurer une notification d’événement pour toutes les personnes utilisant le système. La configuration d’une notification d’événement consiste à l’activer ou la désactiver.

<!--Alina annotation on the word "all" in 2nd sentence: abive, drafted and remains QS only-->

En fonction de l’événement que vous activez et que l’utilisateur ou l’utilisatrice laisse activé sur son propre profil, les utilisateurs et utilisatrices reçoivent des notifications instantanées et/ou quotidiennes par e-mail lorsqu’un événement se produit.

Vous devez d’abord spécifier les notifications que vous souhaitez que les utilisateurs et utilisatrices reçoivent dans la zone de configuration de votre instance Workfront. Une fois que vous avez activé une notification dans la zone de configuration, celle-ci s’affiche comme activée pour chaque utilisateur ou utilisatrice dans sa page de profil.

Une fois que les notifications ont été activées dans la zone de configuration et qu’elles apparaissent dans les pages de profil des utilisateurs et utilisatrices, les utilisateurs et utilisatrices individuels ou une autre personne disposant d’une licence Plan peuvent également configurer les notifications activées dans le profil d’un utilisateur ou d’une utilisatrice afin de contrôler les notifications que cette personne spécifique reçoit ainsi que leur fréquence. Pour plus d’informations, consultez [Modifier vos propres notifications par e-mail](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Pour une liste de toutes les notifications d’événements que vous pouvez activer et désactiver, voir [Types de notifications d’événements](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Pour plus d’informations sur le déverrouillage d’une notification d’événement afin que les administrateurs et administratrices de groupes puissent la configurer pour leurs groupes, voir [Déverrouiller ou verrouiller la configuration des notifications d’événements pour tous les groupes](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md) et [Visualiser et configurer les notifications d’événements pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Nouvelle : standard</p>
 <p>ou</p> 
<p>Actuelle : formule</p> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Planificateur ou version ultérieure, avec accès administratif aux notifications de rappel</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurer les notifications d’événements pour les utilisateurs et utilisatrices

Vous devez activer les notifications dans la zone de configuration de Workfront avant que les utilisateurs et utilisatrices puissent les activer ou les désactiver dans leurs profils individuels.

>[!TIP]
>
>Vous ne pouvez pas activer les notifications pour les Objectifs Workfront à partir de la zone de configuration. Les utilisateurs et utilisatrices ne peuvent activer ces notifications que dans leur profil. Les utilisateurs et utilisatrices disposant de licences Plan peuvent les activer pour d’autres personnes. Pour plus d’informations sur l’activation des notifications Objectifs Workfront pour les utilisateurs et utilisatrices, voir [Notifications : objectifs](../../../workfront-basics/using-notifications/notifications-goals.md).

{{step-1-to-setup}}

1. Cliquez sur **E-mail** > **Notifications**.

   ![](assets/notifications-area-under-setup-emails.png)


1. Assurez-vous que l’onglet **Notifications d’événements** est ouvert.
1. Appuyez sur le bouton situé à gauche du nom de l’événement pour l’activer ou le désactiver.

   Pour connaître le statut de notification par défaut d’un événement, voir [Notifications d’événements](../../../workfront-basics/using-notifications/event-notifications.md).

1. (Facultatif) Cliquez sur le nom d’une notification d’événement pour personnaliser l’objet de la notification par e-mail.

   Pour plus d’informations sur la personnalisation des objets des notifications par e-mail, voir [Personnaliser les objets des e-mails pour les notifications d’événements](../../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md).

1. (Facultatif) Si vous souhaitez déverrouiller la configuration d’une notification par e-mail afin que les administrateurs et administratrices de groupes puissent la configurer séparément pour leurs groupes, cliquez sur le bouton ![](assets/lock-toggle-button.png) à droite de la notification pour la faire passer en position déverrouillée ![](assets/unlock-toggle-button.png).

   >[!NOTE]
   >
   >Cette fonctionnalité n’est disponible dans un premier temps que pour les clientes et clients du cluster 4, dans le cadre d’un déploiement progressif. Elle sera disponible dans d’autres clusters peu de temps après. Cet article sera mis à jour au fur et à mesure.

   Pour plus d’informations, voir [Déverrouiller ou verrouiller la configuration des notifications d’événements pour tous les groupes](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md).
