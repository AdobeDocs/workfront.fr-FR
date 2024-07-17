---
content-type: overview
product-area: user-management
navigation-topic: configure-your-user-profile
title: Configurer les congés
description: Il est important d’indiquer dans Adobe Workfront le moment où un délai de pause approuvé se produit, car cela affecte votre planning et affecte les dates d’achèvement prévues des tâches auxquelles vous êtes affecté.
author: Lisa
feature: Get Started with Workfront
exl-id: e7710495-c418-47b1-8598-725580054fc5
source-git-commit: 16a34e4315d508e31859e962edd01026d01ee193
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 13%

---

# Configurer les congés

<!-- Audited: 12/2023 -->

[!DNL Adobe Workfront] n’est pas conçu pour répliquer ou remplacer vos systèmes existants pour gérer, accumuler et effectuer le suivi du temps libre.

Cependant, il est important d’indiquer le moment où un congé approuvé a lieu, car cela affecte à la fois votre planning et les [!UICONTROL Dates d’achèvement prévues] des tâches auxquelles vous êtes affecté.

Par exemple, si vous êtes affecté à une tâche qui doit durer deux semaines et que vous prévoyez de prendre trois jours de congé pendant cette période, [!DNL Workfront] ajoute trois jours à la chronologie de la tâche pour tenir compte du temps de congé.

Les outils de gestion des ressources utilisent également votre temps de congé personnel pour indiquer quand vous êtes disponible pour le travail planifié.

>[!NOTE]
>
>Pour garantir qu’aucune incohérence ne se produise avec les dates pour lesquelles vous planifiez votre heure de congé, nous vous recommandons de faire correspondre le fuseau horaire de votre profil utilisateur à celui de votre planification. Pour plus d’informations, consultez les articles suivants :
>
>* [Créer un planning](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)
>* [Modifier le profil d’un utilisateur](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)
>

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td> <p>Nouveau : Standard (pour configurer votre temps de congé personnel)</p>
        <p>ou</p>
        <p>Actuel : travail ou plus (pour configurer votre temps de congé personnel)</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td>[!UICONTROL Manager] avec accès à [!UICONTROL Modifier l’utilisateur] (pour apporter des modifications au calendrier des jours fériés des autres utilisateurs)<br>
   <strong>REMARQUE : </strong> Si un responsable modifie le calendrier des heures de congé personnel d’un autre utilisateur, toutes les entrées sont affichées dans le fuseau horaire de l’utilisateur et non dans celui du responsable.</td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Configurer un temps de pause personnel dans [!DNL Workfront]

{{step1-click-profile-pic}}

1. Dans le panneau de gauche, cliquez sur **[!UICONTROL Time Off]**.
1. Sélectionnez la date de votre jour de congé personnel.

   ![Calendrier des congés personnels](assets/personal-time-off-calendar.png)

1. Sélectionnez **[!UICONTROL Toute la journée]** si vous prenez un jour de congé.

   Laissez la case décochée si vous prenez moins d’une journée de congé et indiquez les heures de début et de fin de votre congé.

1. Cliquer sur **[!UICONTROL Enregistrer]**.

   Votre temps de pause est désormais visible dans l’ensemble du système [!DNL Workfront] dans les outils de gestion des ressources tels que le planificateur de ressource et l’équilibreur de charge de travail. Lorsqu’une tâche vous est affectée pendant cette période, une info-bulle informe l’utilisateur que vous avez planifié un congé.
