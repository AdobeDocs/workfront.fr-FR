---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Partage d’objets sans génération de notifications
description: Découvrez comment partager des objets et empêcher l’envoi de notifications à propos de cette modification. Cela s’avère particulièrement utile lorsque vous partagez des objets en bloc.
author: Alina
feature: Get Started with Workfront
exl-id: 02106282-addb-4bdd-82d2-9da5a5f6a687
TQID: https://experienceleague.adobe.com/zhNlFwg-1UuNKXxqIj-H62rGdewhbqKHLz4NbzkEqP8
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 577
ht-degree: 21%

---

# Partage d’objets sans générer de notifications

<!--Audited: 12/2024-->

Lorsque vous partagez un objet dans Adobe Workfront, les personnes avec lesquelles vous partagez l’objet reçoivent une notification par e-mail les informant du partage.

Il est important de recevoir une notification par e-mail lorsqu’une personne partage un objet avec vous pour être au courant de cette modification. Cependant, un nombre trop élevé de notifications peut prêter à confusion pour les utilisateurs et les utilisatrices. Si vous souhaitez partager un grand nombre d’objets avec des utilisateurs et utilisatrices à la fois, la désactivation temporaire des notifications vous aidera à éviter toute confusion.

Les personnes reçoivent des notifications par e-mail lorsque les paramètres suivants sont activés en même temps :

* L’une des notifications d’événement suivantes, ou les deux, sont activées au niveau du système ou du groupe :

   * Partage d&#39;objet envoyé à l&#39;utilisateur
   * Le partage d&#39;objet vers l&#39;équipe est activé au niveau du système ou du groupe.
* L’une des notifications par e-mail suivantes, ou les deux, sont activées dans le profil de l’utilisateur :

   * Quelqu&#39;un partage un objet avec moi
   * Quelqu&#39;un partage un objet avec mon équipe

Si vous devez partager plusieurs objets avec plusieurs personnes (en bloc), mais que vous ne souhaitez pas qu’elles reçoivent des notifications par e-mail concernant cette modification, procédez comme suit :

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td> <p>Tous </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Standard</p>
   <p>Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès Affichage ou supérieur aux objets que vous souhaitez partager.</p>
   <p>Modifier l’accès aux utilisateurs</p>
   <p><b>NOTE</b></p>
   <p> Vous devez être un administrateur système ou de groupe pour vérifier le statut des notifications d’événement pour le système ou le groupe</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations d’affichage ou supérieures pour les objets que vous souhaitez partager.</p></td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Partage d’objets sans génération de notifications

1. Assurez-vous que les **notifications d’événement** suivantes sont activées au niveau du système ou du groupe :

   * **Partage d’objet pour l’utilisateur**
   * **Le partage d’objets avec l’équipe est activé au niveau du système ou du groupe**.

   Pour plus d’informations, consultez l’article [Configurer les notifications d’événements pour tous les utilisateurs et les utilisatrices du système](/help/quicksilver/administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

   Si ces notifications d’événement ne sont pas activées, les notifications de partage d’un objet ne seront pas envoyées aux utilisateurs. Si l’un des deux est activé, ou les deux, procédez comme suit.

{{step-1-to-users}}

1. Sélectionnez plusieurs utilisateurs dans la liste, puis cliquez sur **Notifications** > **Divers**.
1. Désactivez l’une ou l’autre des notifications suivantes (selon celles qui sont activées au niveau du système ou du groupe) :

   * **Quelqu’un partage un objet avec moi**
   * **Une personne partage un objet avec mon équipe**.

   Assurez-vous que ces notifications sont sélectionnées pour tous les utilisateurs sélectionnés avant de les désactiver. Ainsi, vous pouvez les réactiver en bloc pour tous les objets après les avoir partagés.

1. Cliquez sur **Enregistrer les modifications**.
1. Accédez à la liste des objets à partager et sélectionnez-les, puis cliquez sur l’icône **Partager** en haut de la liste.

   Pour plus d’informations sur le partage d’un objet en bloc, voir [Partager un objet](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

1. Revenez à la liste des utilisateurs pour lesquels vous avez désactivé les notifications et sélectionnez les mêmes utilisateurs.
1. Sélectionnez les mêmes utilisateurs dans la liste, puis cliquez sur **Notifications** > **Divers**.
1. Activez l’une ou l’autre des notifications suivantes, ou les deux (selon celles qui sont activées au niveau du système ou du groupe) :

   * **Quelqu’un partage un objet avec moi**
   * **Une personne partage un objet avec mon équipe**.

1. Cliquez sur **Enregistrer les modifications**.

   Les objets ont été partagés avec les utilisateurs sélectionnés et aucun d&#39;eux n&#39;a reçu de notification par e-mail concernant cette modification.
