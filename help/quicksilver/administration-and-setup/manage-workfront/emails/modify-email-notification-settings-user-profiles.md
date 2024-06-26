---
user-type: administrator
product-area: system-administration
keywords: modifier,e-mail,notification,paramètres,bloc,modifier en bloc,configurer,multiple,utilisateurs, utilisatrices
navigation-topic: emails-administration
title: Modifier les paramètres de notification par e-mail de plusieurs personnes
description: Cet article fournit à l’équipe d’administration de Workfront ou de groupe des informations sur la façon dont elle peut mettre à jour les notifications par e-mail d’autres personnes.
author: Nolan
feature: System Setup and Administration
role: Admin
exl-id: 658f97cd-0500-421d-9c89-26041ca59655
source-git-commit: 4cab7bed6cb4c25d96e70ccce2ece7f6d156f435
workflow-type: tm+mt
source-wordcount: '458'
ht-degree: 97%

---

# Modifier les paramètres de notification par e-mail de plusieurs personnes

<!-- Audited: 12/2023 -->

Si vous faites partie de l’équipe d’administration d’Adobe Workfront ou si vous disposez d’un niveau d’accès Planificationbvous permettant de modifier les paramètres d’autres personnes, vous pouvez configurer les paramètres de notification pour plusieurs personnes à la fois. Cela inclut la spécification des notifications reçues par les personnes au fur et à mesure des événements, ou dans un e-mail de synthèse quotidienne, comme décrit dans les [notifications Adobe Workfront](../../../workfront-basics/using-notifications/wf-notifications.md). Pour plus d’informations sur le niveau d’accès requis pour modifier les personnes, voir [Accorder l’accès aux personnes](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

Vous pouvez également configurer des notifications par e-mail pour une personne à la fois, y compris votre propre profil. Pour plus d’informations, consultez [Modifier vos propres notifications par e-mail](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).


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
   <td> <p>Nouvelle formule : standard </p>
 <p>ou</p> 
<p>Formule actuelle : formule </p> 
</td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Modifier des paramètres de notification par e-mail pour plusieurs personnes

Lorsque vous configurez les paramètres de notification en bloc, vous ne pouvez modifier que les paramètres communs aux personnes sélectionnées.

Lorsque vous modifiez un paramètre de notification, le libellé **Modifié** s’affiche pour ce paramètre de notification afin de vous informer que ce paramètre de notification a été modifié.

Pour modifier les paramètres de notification par e-mail pour plusieurs personnes :

{{step-1-to-users}}

1. Sélectionnez les personnes, puis cliquez sur **Modifier**.
1. Dans la zone **Modifier la personne** qui s’affiche, cliquez sur **Notifications**.

1. Développez une catégorie pour afficher les paramètres de notification associés à cette catégorie.

   Si au moins une personne est sélectionnée alors que les notifications ne correspondent pas à celles des autres personnes sélectionnées, la case de catégorie de cette notification comporte une ligne horizontale ![](assets/straight-line-instead-of-checkmark.jpg) plutôt qu’une coche.


1. Cliquez sur les notifications que vous souhaitez que les personnes reçoivent quotidiennement ou instantanément, ou effacez celles que vous souhaitez qu’elles ne reçoivent plus.

   >[!NOTE]
   >
   >   Pour la catégorie **Communication**, vous pouvez sélectionner des notifications individuelles pour une diffusion instantanée uniquement. Vous devez sélectionner toutes les notifications à diffuser dans une synthèse quotidienne.


1. Si vous avez sélectionné des notifications à envoyer sous forme de synthèse quotidienne, sélectionnez l’heure de la journée à laquelle vous souhaitez que le résumé soit diffusé en haut de la section **Notifications** dans le menu **E-mail de synthèse quotidienne après**.

   ![](assets/daily-digest-time.png)

   La synthèse quotidienne comprend les événements qui répondent aux critères des notifications 24 heures avant l’heure sélectionnée. Les personnes reçoivent un e-mail de synthèse quotidienne pour chaque type de notification.

   La synthèse quotidienne peut arriver après l’heure sélectionnée, selon le nombre d’e-mails placés en file d’attente pour diffusion dans le système. L’heure indiquée correspond à l’heure locale spécifiée dans les paramètres du navigateur.
