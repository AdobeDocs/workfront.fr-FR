---
content-type: reference
product-area: user-management
navigation-topic: people-teams-and-groups
title: Envoi de messages directs à d’autres utilisateurs
description: Adobe Workfront vous permet d’envoyer rapidement et facilement des messages qui ne sont pas liés à un élément de travail directement à d’autres personnes de Workfront.
author: Lisa
feature: People Teams and Groups
exl-id: 82a1c304-176a-48c5-809d-40663ee768b7
source-git-commit: 82dc1cef02c6724dd0bc5b98d2a8f60a420b72bd
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 50%

---

# Envoyer des messages directs à d’autres utilisateurs et utilisatrices

{{preview-fast-release-general}}

[!DNL Adobe Workfront] vous permet d’envoyer rapidement et facilement des messages qui ne sont pas liés à un élément de travail, directement à d’autres personnes de [!DNL Workfront]. Les messages envoyés comme décrit dans cette section apparaissent dans l’onglet [!UICONTROL Mises à jour] de la page de profil de l’utilisateur et sont visibles par tous les utilisateurs. Pour plus d’informations sur les mises à jour, voir [Mettre à jour les éléments de travail et afficher les mises à jour : index des articles](../../workfront-basics/updating-work-items-and-viewing-updates/update-work-items-and-view-updates.md).

La personne à laquelle vous envoyez le message reçoit les types de notifications suivants lorsque vous envoyez un message comme décrit dans cette section :

* Notification in-app, comme décrit dans [Afficher et gérer les notifications in-app](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md)
* Notification par e-mail

  Cela dépend de la configration de réception des types de notifications par e-mail de la personne. Pour plus d’informations, voir [Configurer des notifications d’événement pour toutes les personnes du système](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md), [Afficher et configurer des notifications d’événement pour un groupe](../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md) et [Modifier vos propres notifications par e-mail](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>
   <p>Pour envoyer un message à partir de la page de profil de l’utilisateur, vous devez disposer de :<br>
   Nouveau : clair ou supérieur<br>
   or<br>
   Actuel : révision ou version ultérieure</p>
   <p>Pour envoyer un message à partir de la liste des utilisateurs, vous devez disposer de :<br>
   Nouveau : Standard<br>
   or<br>
   Actuel : travail ou plus élevé</p></td>
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Envoyer un message sans rapport avec un élément de travail à un autre utilisateur à partir de sa page de profil

1. Accédez à la page de profil de l’utilisateur auquel vous souhaitez envoyer un message.

   Pour accéder à la page de profil d’un utilisateur, cliquez sur le nom lié de l’utilisateur tel qu’il apparaît n’importe où dans l’interface [!DNL Workfront]. Les noms d’utilisateur s’affichent dans de nombreuses zones, comme dans un commentaire de l’utilisateur.

1. Dans l’onglet **[!UICONTROL Mises à jour]**, cliquez sur le champ de la zone de texte.

   ![Envoyer un message à la personne sur l’onglet [!UICONTROL Mises à jour]](assets/send-message-to-user-on-updates-tab.png)

1. Saisissez votre message.
1. (Facultatif) Cliquez dans le champ **[!UICONTROL Notifier]**, puis commencez à saisir le nom d’une autre personne que vous souhaitez inclure dans ce message.

1. (Facultatif) Sélectionnez **[!UICONTROL Réservé à mon entreprise]** pour que ce message ne soit visible que par les autres personnes de votre entreprise.

1. Cliquez sur **[!UICONTROL Mettre à jour].**
Le message est publié en haut de la liste des messages dans l’onglet **[!UICONTROL Mises à jour]** de la page de profil de l’utilisateur.

## Envoyer un message à un ou plusieurs utilisateurs à partir de la liste des utilisateurs

Cette option n’est disponible que si vous disposez d’une licence Standard, Plan ou Work.

{{step-1-to-users}}

1. Sélectionnez le ou les utilisateurs auxquels vous souhaitez envoyer un message, puis cliquez sur [!UICONTROL **Envoyer la mise à jour à l’utilisateur**].
1. Saisissez votre message dans la fenêtre [!UICONTROL Envoyer la mise à jour à l’utilisateur] .

   <span class="preview">Exemple d’image dans l’environnement de prévisualisation :</span>

   <span class="preview">![Message user sur la fenêtre Envoyer la mise à jour à l’utilisateur](assets/send-message-to-user-dialog-from-user-list.png)</span>

1. (Facultatif) Recherchez d’autres utilisateurs que vous souhaitez marquer dans le message. Il n’est pas nécessaire de baliser les utilisateurs que vous avez déjà sélectionnés dans la liste des utilisateurs.
1. (Facultatif) Sélectionnez **[!UICONTROL Réservé à mon entreprise]** pour que ce message ne soit visible que par les autres personnes de votre entreprise.
1. Cliquez sur [!UICONTROL **Send**].
Le message est publié en haut de la liste des messages dans l’onglet **[!UICONTROL Mises à jour]** de la page de profil de chaque utilisateur.
