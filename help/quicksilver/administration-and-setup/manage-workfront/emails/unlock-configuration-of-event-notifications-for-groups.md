---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: Déverrouiller ou verrouiller la configuration des notifications d’événement pour tous les groupes
description: Si vous êtes administrateur ou administratrice Adobe Workfront, vous pouvez déverrouiller ou reverrouiller la possibilité pour les administrateurs et les administratrices de groupe de configurer une notification d’événement pour leurs groupes de niveau supérieur. La configuration d’une notification d’événement consiste à l’activer ou à la désactiver.
author: Courtney, Becky
feature: System Setup and Administration
role: Admin
exl-id: 056d76c1-7e9b-49b9-974a-75765e53b7fd
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '540'
ht-degree: 97%

---

# Déverrouiller ou verrouiller la configuration des notifications d’événements pour tous les groupes

Si vous êtes administrateur ou administratrice Adobe Workfront, vous pouvez déverrouiller ou reverrouiller la possibilité pour les administrateurs et les administratrices de groupe de configurer une notification d’événement pour leurs groupes de niveau supérieur. La configuration d’une notification d’événement consiste à l’activer ou à la désactiver.

S’il existe des groupes au-dessus du groupe que vous gérez, leurs administrateurs et administratrices peuvent également le faire pour votre groupe. Il en va de même pour les administrateurs et administratrices de Workfront (pour n’importe quel groupe).

Lorsqu’un administrateur ou une administratrice configure une notification d’événement pour un groupe, la configuration affecte les utilisateurs et les utilisatrices dont ce groupe, ou l’un de ses sous-groupes, est leur groupe principal. Dans leurs profils d’utilisateur ou d’utilisatrice, ces personnes voient les notifications d’événement activées pour leur groupe principal au lieu des notifications d’événement activées à l’échelle du système. Pour plus d’informations, consultez [Afficher et configurer des notifications d’événement pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

>[!NOTE]
>
>* Un administrateur ou une administratrice Workfront peut déverrouiller et reverrouiller la configuration d’une notification d’événement dans Adobe Workfront Classic et dans la nouvelle expérience Adobe Workfront. Cependant, un administrateur ou une administratrice de groupe peut configurer cette notification d’événement pour un groupe uniquement dans la nouvelle expérience Adobe Workfront. Les administrateurs et les administratrices de groupe qui utilisent Adobe Workfront Classic peuvent passer à la nouvelle expérience Adobe Workfront pour configurer des notifications d’événement déverrouillées pour un groupe, puis revenir à Adobe Workfront Classic pour voir les modifications en vigueur.
>* Les sous-groupes héritent des configurations de notification d’événement des groupes de niveau supérieur.
>

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>
   <p>Standard</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Administrateur ou administratrice système</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Déverrouiller ou reverrouiller la possibilité de configurer une notification d’événement

>[!IMPORTANT]
>
>Lorsque vous reverrouillez une notification, tous les groupes du système héritent de la notification exactement comme vous la définissez. Cela remplace toute modification que les administrateurs et administratrices de groupe peuvent avoir apportée à leurs groupes. Il est donc préférable de les consulter d’abord.

{{step-1-to-setup}}

1. Cliquez sur **E-mail** > **Notifications**.

1. Assurez-vous que l’onglet **Notifications d’événement** est ouvert.
1. Cliquez sur l’icône située à droite de la notification pour la faire basculer vers la position verrouillée ![Icône Verrouiller](assets/lock-toggle-button.png) ou déverrouillée ![Icône Déverrouiller](assets/unlock-toggle-button.png).

   Ou

   Si vous souhaitez déverrouiller ou verrouiller plusieurs notifications à la fois, sélectionnez-les, puis cliquez sur Déverrouiller ![Icône Déverrouiller](assets/unlock-icon-toolbar.png) ou Verrouiller ![Icône Verrouiller](assets/lock-icon-locked-qs.png) qui s’affiche dans la barre d’outils située au-dessus de la liste.

1. Cliquer sur **Enregistrer**.
1. (Facultatif) Si vous souhaitez configurer la notification d’événement pour un groupe de niveau supérieur au lieu de laisser cette tâche à l’administrateur ou l’administratrice du groupe, vous pouvez effectuer l’une des opérations suivantes :

   * Supprimez les **Notifications d’événement système** dans la zone de recherche située au-dessus de la liste des notifications, recherchez et sélectionnez le nom du groupe de niveau supérieur pour répertorier ses notifications, puis activez ou désactivez les notifications déverrouillées dans la liste qui s’affiche.
   * Cliquez sur **Groupes** dans le menu de gauche, cliquez sur le nom du groupe de niveau supérieur. Cliquez sur **Notifications d’événement** dans le panneau de gauche, puis configurez la notification d’événement déverrouillée, comme expliqué à la section [Afficher et configurer des notifications d’événement pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).
