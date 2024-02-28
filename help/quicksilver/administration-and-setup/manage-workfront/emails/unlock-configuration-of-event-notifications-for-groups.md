---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: Déverrouiller ou verrouiller la configuration des notifications d’événement pour tous les groupes
description: Si vous êtes administrateur Adobe Workfront, vous pouvez déverrouiller ou reverrouiller la possibilité pour les administrateurs de groupe de configurer une notification d’événement pour les groupes de niveau supérieur qu’ils gèrent. La configuration d'une notification d'événement consiste à l'activer ou la désactiver.
author: Lisa, Nolan
feature: System Setup and Administration
role: Admin
exl-id: 056d76c1-7e9b-49b9-974a-75765e53b7fd
source-git-commit: 1c0a656f2603c5decabd2bb4e88da1b9530f9e1c
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 0%

---

# Déverrouiller ou verrouiller la configuration des notifications d’événement pour tous les groupes

Si vous êtes administrateur Adobe Workfront, vous pouvez déverrouiller ou reverrouiller la possibilité pour les administrateurs de groupe de configurer une notification d’événement pour les groupes de niveau supérieur qu’ils gèrent. La configuration d&#39;une notification d&#39;événement consiste à l&#39;activer ou la désactiver.

S’il existe des groupes au-dessus du groupe que vous gérez, leurs administrateurs peuvent également le faire pour votre groupe. Il en va de même pour les administrateurs de Workfront (pour n’importe quel groupe).

Lorsqu’un administrateur configure une notification d’événement pour un groupe, la configuration affecte les utilisateurs pour lesquels ce groupe, ou l’un de ses sous-groupes, est leur groupe d’accueil. Dans leurs profils utilisateur, ces utilisateurs voient les notifications d’événement activées pour leur groupe d’accueil au lieu des notifications d’événement activées à l’échelle du système. Pour plus d’informations, voir [Affichage et configuration des notifications d’événement pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

>[!NOTE]
>
>* Un administrateur Workfront peut déverrouiller et reverrouiller la configuration d’une notification d’événement dans Adobe Workfront Classic et dans la nouvelle expérience Adobe Workfront. Cependant, un administrateur de groupe peut configurer cette notification d’événement pour un groupe uniquement dans la nouvelle expérience Adobe Workfront. Les administrateurs de groupe qui utilisent Adobe Workfront Classic peuvent passer à la nouvelle expérience Adobe Workfront pour configurer des notifications d’événement déverrouillées pour un groupe, puis revenir à Adobe Workfront Classic pour voir les modifications en vigueur.
>* Les sous-groupes héritent des configurations de notification d’événement au niveau du groupe des groupes de niveau supérieur.
>

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Quelconque</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès</td> 
   <td> <p>Administrateur système</p> </td> 
  </tr> 
 </tbody> 
</table>

## Déverrouiller ou reverrouiller la possibilité de configurer une notification d’événement ;

>[!IMPORTANT]
>
>Lorsque vous reverrouillez une notification, tous les groupes du système héritent de la notification exactement comme vous la définissez. Cela remplace toute modification que les administrateurs de groupe peuvent avoir apportée à leurs groupes. Il est donc préférable de les consulter d’abord.

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Cliquez sur **Email** > **Notifications**.

1. Assurez-vous que la variable **Notifications d’événement** est ouvert.
1. Cliquez sur l’icône située à droite de la notification pour la basculer vers le fichier verrouillé. ![Icône Verrouiller](assets/lock-toggle-button.png) ou déverrouillé ![Icône Déverrouiller](assets/unlock-toggle-button.png) position.

   Ou

   Si vous souhaitez déverrouiller ou verrouiller plusieurs notifications à la fois, sélectionnez-les, puis cliquez sur Déverrouiller . ![Icône Déverrouiller](assets/unlock-icon-toolbar.png) ou Verrouiller ![Icône Verrouiller](assets/lock-icon-locked-qs.png) qui s’affiche dans la barre d’outils située au-dessus de la liste.

1. Cliquer sur **Enregistrer**.
1. (Facultatif) Si vous souhaitez configurer la notification d’événement pour un groupe de niveau supérieur au lieu de laisser cette tâche à l’administrateur du groupe, vous pouvez effectuer l’une des opérations suivantes :

   * Supprimer **Notifications d’événement système** dans la zone de recherche située au-dessus de la liste des notifications, recherchez et sélectionnez le nom du groupe de niveau supérieur pour répertorier ses notifications, puis activez ou désactivez les notifications déverrouillées dans la liste qui s’affiche.
   * Cliquez sur **Groupes** dans le menu de gauche, cliquez sur le nom du groupe de niveau supérieur. Cliquez sur **Notifications d’événement** dans le panneau de gauche, puis configurez la notification d’événement déverrouillée, comme expliqué à la section [Affichage et configuration des notifications d’événement pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).
