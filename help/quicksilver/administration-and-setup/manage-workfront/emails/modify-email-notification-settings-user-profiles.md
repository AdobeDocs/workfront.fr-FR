---
user-type: administrator
product-area: system-administration
keywords: modify,email,notification,settings,bulk,edit,configure,multiple,users
navigation-topic: emails-administration
title: Modification des paramètres de notification électronique dans les profils des utilisateurs
description: Si vous êtes administrateur Adobe Workfront ou si vous disposez d’un niveau d’accès Planificateur vous permettant de modifier les paramètres d’autres utilisateurs, vous pouvez configurer les paramètres de notification pour plusieurs utilisateurs à la fois. Cela inclut la spécification des notifications reçues par les utilisateurs au fur et à mesure des événements ou dans un email de résumé quotidien, comme décrit dans les notifications Adobe Workfront. Pour plus d’informations sur le niveau d’accès requis pour modifier les utilisateurs, voir Octroi de l’accès aux utilisateurs.
author: Lisa, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 658f97cd-0500-421d-9c89-26041ca59655
source-git-commit: 730932f6c8d4658273dd943e464a038828d288e9
workflow-type: tm+mt
source-wordcount: '534'
ht-degree: 0%

---

# Modification des paramètres de notification électronique dans les profils des utilisateurs

Si vous êtes administrateur Adobe Workfront ou si vous disposez d’un niveau d’accès Planificateur vous permettant de modifier les paramètres d’autres utilisateurs, vous pouvez configurer les paramètres de notification pour plusieurs utilisateurs à la fois. Cela inclut la spécification des notifications reçues par les utilisateurs au fur et à mesure des événements, ou dans un email de résumé quotidien, comme décrit dans la section [Notifications Adobe Workfront](../../../workfront-basics/using-notifications/wf-notifications.md). Pour plus d’informations sur le niveau d’accès requis pour modifier les utilisateurs, voir [Accorder l’accès aux utilisateurs](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

Lorsque vous configurez les paramètres de notification en bloc, vous ne pouvez modifier que les paramètres communs aux utilisateurs sélectionnés.

Vous pouvez également configurer des notifications électroniques pour un utilisateur à la fois. Pour plus d’informations, voir [Activation ou désactivation de vos propres notifications d’événement](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td>Plan</td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour savoir quel plan ou type de licence vous avez, contactez votre administrateur Workfront.

## Modification en masse des paramètres de notification électronique de plusieurs utilisateurs

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Utilisateurs** ![](assets/users-icon-in-main-menu.png). Sélectionnez les utilisateurs, puis cliquez sur **Modifier**.
1. Dans le **Modifier la personne** s’affiche, cliquez sur **Notifications**.

1. Développez une catégorie pour afficher les paramètres de notification associés à cette catégorie.

   Si au moins un utilisateur est sélectionné alors que les notifications ne correspondent pas à celles des autres utilisateurs sélectionnés, la case à cocher de catégorie de cette notification comporte une ligne horizontale. ![](assets/straight-line-instead-of-checkmark.jpg) plutôt qu’une coche.

1. Cliquez sur les notifications que vous souhaitez que les utilisateurs reçoivent quotidiennement ou instantanément, ou effacez celles que vous souhaitez qu’ils cessent de recevoir.

   Pour le **Communication** vous pouvez sélectionner des notifications individuelles pour une diffusion instantanée uniquement. Vous devez sélectionner toutes les notifications à diffuser dans un résumé quotidien.

   Lorsque vous modifiez un paramètre de notification, le libellé **Modifié** s’affiche pour ce paramètre de notification afin de vous informer que ce paramètre de notification a été modifié.

1. Si vous avez sélectionné des notifications à envoyer sous forme de résumé quotidien, sélectionnez l’heure de la journée à laquelle vous souhaitez que le résumé soit diffusé en haut de la page **Notifications** dans la section **Email Daily Digest après** .

   Après avoir sélectionné une heure de diffusion, la variable **Email Daily Digest après** s’affiche avec un cadre orange pour indiquer que l’heure de la diffusion a été modifiée.

   Le résumé quotidien comprend les événements qui répondent aux critères des notifications 24 heures avant l’heure sélectionnée. Les utilisateurs reçoivent un courrier électronique condensé quotidien pour chaque type de notification.

   Le résumé quotidien peut arriver après la période sélectionnée, selon le nombre d&#39;emails placés en file d&#39;attente pour diffusion dans le système. L’heure indiquée correspond à l’heure locale spécifiée dans les paramètres du navigateur.
