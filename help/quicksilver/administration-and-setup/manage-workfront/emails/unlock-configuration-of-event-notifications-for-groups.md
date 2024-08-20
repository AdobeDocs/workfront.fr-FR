---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: Déverrouillage ou verrouillage de la configuration des notifications d’événement pour tous les groupes
description: Si vous faites partie de l’équipe d’administration Adobe Workfront, vous pouvez déverrouiller ou reverrouiller la possibilité pour l’équipe d’administration de groupe de configurer une notification d’événement pour les groupes de niveau supérieur qu’elle gère. La configuration d’une notification d’événement consiste à l’activer ou la désactiver.
author: Lisa, Nolan
feature: System Setup and Administration
role: Admin
exl-id: 056d76c1-7e9b-49b9-974a-75765e53b7fd
source-git-commit: ab774e937a15aaa04704e872579df880a9b80aaf
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 96%

---

# Déverrouiller ou verrouiller la configuration des notifications d’événement pour tous les groupes

Si vous faites partie de l’équipe d’administration Adobe Workfront, vous pouvez déverrouiller ou reverrouiller la possibilité pour l’équipe d’administration de groupe de configurer une notification d’événement pour les groupes de niveau supérieur qu’elle gère. La configuration d’une notification d’événement consiste à l’activer ou la désactiver.

S’il existe des groupes au-dessus du groupe que vous gérez, leur équipe d’administration peut également le faire pour votre groupe. Il en va de même pour l’administration de Workfront (pour n’importe quel groupe).

Lorsqu’une personne de l’équipe d’administration configure une notification d’événement pour un groupe, la configuration affecte les personnes pour lesquelles ce groupe, ou l’un de ses sous-groupes, est leur groupe principal. Dans leurs profils, ces personnes voient les notifications d’événement activées pour leur groupe principal au lieu des notifications d’événement activées à l’échelle du système. Pour plus d’informations, voir [Afficher et configurer des notifications d’événement pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

>[!NOTE]
>
>* Une personne de l’équipe d’administration Workfront peut déverrouiller et reverrouiller la configuration d’une notification d’événement dans Adobe Workfront Classic et dans la nouvelle expérience Adobe Workfront. Cependant, une personne de l’équipe d’administration de groupe peut configurer cette notification d’événement pour un groupe uniquement dans la nouvelle expérience Adobe Workfront. L’équipe d’administration de groupe qui utilise Adobe Workfront Classic peut passer à la nouvelle expérience Adobe Workfront pour configurer des notifications d’événement déverrouillées pour un groupe, puis revenir à Adobe Workfront Classic pour voir les modifications effectives.
>* Les sous-groupes héritent des configurations de notification d’événement au niveau du groupe des groupes de niveau supérieur.
>

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
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Administrateur ou administratrice système</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Déverrouiller ou reverrouiller la possibilité de configurer une notification d’événement

>[!IMPORTANT]
>
>Lorsque vous reverrouillez une notification, tous les groupes du système héritent de la notification telle que vous l’avez définie. Cela remplace toute modification que l’équipe d’administion de groupe peut avoir apportée à ses groupes. Il est donc préférable de la consulter d’abord.

{{step-1-to-setup}}

1. Cliquez sur **E-mail** > **Notifications**.

1. Assurez-vous que l’onglet **Notifications d’événement** est ouvert.
1. Cliquez sur l’icône située à droite de la notification pour la basculer entre la position verrouillée ![Lock icon](assets/lock-toggle-button.png) ou déverrouillée ![Unlock icon](assets/unlock-toggle-button.png).

   Ou

   Si vous souhaitez déverrouiller ou verrouiller plusieurs notifications à la fois, sélectionnez-les, puis cliquez sur le bouton Déverrouiller ![Unlock icon](assets/unlock-icon-toolbar.png) ou Verrouiller ![Lock icon](assets/lock-icon-locked-qs.png) qui s’affiche dans la barre d’outils située au-dessus de la liste.

1. Cliquez sur **Enregistrer**.
1. (Facultatif) Si vous souhaitez configurer la notification d’événement pour un groupe de niveau supérieur au lieu de laisser cette tâche à l’équipe d’administration du groupe, vous pouvez effectuer l’une des opérations suivantes :

   * Supprimer **Notifications d’événement système** dans la zone de recherche située au-dessus de la liste des notifications, recherchez et sélectionnez le nom du groupe de niveau supérieur pour répertorier ses notifications, puis activez ou désactivez les notifications déverrouillées dans la liste qui s’affiche.
   * Cliquez sur **Groupes** dans le menu de gauche, puis sur le nom du groupe de niveau supérieur. Cliquez sur **Notifications d’événement** dans le panneau de gauche, puis configurez la notification d’événement déverrouillée, comme expliqué à la section [Afficher et configurer des notifications d’événement pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).
