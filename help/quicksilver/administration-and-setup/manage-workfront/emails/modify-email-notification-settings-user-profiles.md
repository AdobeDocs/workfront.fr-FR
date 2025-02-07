---
user-type: administrator
product-area: system-administration
keywords: modifier,e-mail,notification,paramètres,en masse,modifier en masse,configurer,multiple,personnes
navigation-topic: emails-administration
title: Modifier Les Paramètres De Notification Par E-Mail De Plusieurs Utilisateurs
description: Cet article fournit à l’équipe d’administration de Workfront ou de groupes des informations sur la façon dont elle peut mettre à jour les notifications par e-mail d’autres personnes.
author: Nolan
feature: System Setup and Administration
role: Admin
exl-id: 658f97cd-0500-421d-9c89-26041ca59655
source-git-commit: 612243e928c6053d9b02715d9fcfef4dae25cb7a
workflow-type: tm+mt
source-wordcount: '465'
ht-degree: 89%

---

# Modifier les paramètres de notification par e-mail de plusieurs personnes

<!-- Audited: 12/2023 -->

Si vous êtes administrateur ou administratrice Adobe Workfront ou si vous disposez d’un niveau d’accès Planificateur vous permettant de modifier les paramètres d’autres personnes, vous pouvez configurer les paramètres de notification pour plusieurs personnes à la fois. Cela inclut la spécification des notifications reçues par les personnes au fur et à mesure des événements, ou dans un e-mail de synthèse quotidienne, comme décrit dans la section [Notifications Adobe Workfront](../../../workfront-basics/using-notifications/wf-notifications.md). Pour plus d’informations sur le niveau d’accès requis pour modifier les personnes, voir [Accorder l’accès aux personnes](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

Vous pouvez également configurer des notifications par e-mail pour une personne à la fois, y compris votre propre profil. Pour plus d’informations, voir [Modifier vos propres notifications par e-mail](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).


## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Nouveau plan : standard </p>
 <p>ou</p> 
<p>Plan actuel : plan </p> 
</td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, voir [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Modifier les paramètres de notification par e-mail pour plusieurs personnes

Lorsque vous configurez les paramètres de notification en masse, vous ne pouvez modifier que les paramètres communs aux personnes sélectionnées.

Lorsque vous modifiez un paramètre de notification, le libellé **Modifié** s’affiche pour ce paramètre de notification afin de vous informer que ce paramètre de notification a été modifié.

Pour modifier les paramètres de notification par e-mail pour plusieurs personnes :

{{step-1-to-users}}

1. Sélectionnez les personnes, puis cliquez sur **Modifier**.
1. Dans la zone **Modifier la personne** qui s’affiche, cliquez sur **Notifications**.

1. Développez une catégorie pour afficher les paramètres de notification associés à cette catégorie.

   Si au moins un utilisateur est sélectionné et que les notifications ne correspondent pas aux notifications des autres utilisateurs sélectionnés, la case à cocher Catégorie de cette notification contient une ligne horizontale ![Ligne au lieu de Coche](assets/straight-line-instead-of-checkmark.jpg) au lieu d’une coche.


1. Cliquez sur les notifications que vous souhaitez que les personnes reçoivent quotidiennement ou instantanément, ou effacez celles que vous souhaitez qu’elles cessent de recevoir.

   >[!NOTE]
   >
   >   Pour la catégorie **Communication**, vous pouvez sélectionner des notifications individuelles pour une diffusion instantanée uniquement. Vous devez sélectionner toutes les notifications à diffuser dans une synthèse quotidienne.


1. Si vous avez sélectionné des notifications à envoyer sous forme de synthèse quotidienne, sélectionnez l’heure de la journée à laquelle vous souhaitez que la synthèse soit diffusée en haut de la section **Notifications** dans le menu **E-mail de synthèse quotidienne après**.

   ![Heure de synthèse quotidienne](assets/daily-digest-time.png)

   La synthèse quotidienne comprend les événements qui répondent aux critères des notifications 24 heures avant l’heure sélectionnée. Les personnes reçoivent un e-mail de synthèse quotidienne pour chaque type de notification.

   La synthèse quotidienne peut arriver après l’heure sélectionnée, selon le nombre d’e-mails placés en file d’attente pour diffusion dans le système. L’heure indiquée correspond à l’heure locale spécifiée dans les paramètres du navigateur.
