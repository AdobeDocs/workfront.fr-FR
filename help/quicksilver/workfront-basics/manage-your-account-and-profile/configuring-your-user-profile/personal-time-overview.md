---
content-type: overview
product-area: user-management
navigation-topic: configure-your-user-profile
title: Configuration du temps de connexion personnel [!DNL Adobe Workfront]
description: Adobe Workfront n’est pas conçu pour répliquer ou remplacer vos systèmes existants pour gérer, accumuler et effectuer le suivi du temps libre. Cependant, il est important d’indiquer le moment où un congé approuvé a lieu, car cela affecte votre planning et affecte les dates d’achèvement prévues des tâches auxquelles vous êtes affecté.
author: Lisa
feature: Get Started with Workfront
exl-id: e7710495-c418-47b1-8598-725580054fc5
source-git-commit: e87f2a459314b8059a3df634e97560b5c1dffac4
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 1%

---

# Configuration du temps de connexion personnel [!DNL Adobe Workfront]

[!DNL Adobe Workfront] n’est pas conçu pour répliquer ou remplacer vos systèmes existants pour gérer, accumuler et effectuer le suivi du temps libre.

Cependant, il est important d’indiquer quand un délai de pause approuvé se produit, car cela affecte votre planning et affecte le [!UICONTROL Dates d’achèvement prévues] des tâches auxquelles vous êtes affecté.

Par exemple, si vous êtes affecté à une tâche qui doit durer deux semaines et que vous prévoyez de prendre trois jours de congé pendant cette période, [!DNL Workfront] ajoute trois jours à la chronologie de la tâche pour tenir compte du temps de congé.

Les outils de gestion des ressources utilisent également votre temps de congé personnel pour indiquer quand vous êtes disponible pour le travail planifié.

>[!NOTE]
>
>Pour garantir qu’aucune incohérence ne se produise avec les dates pour lesquelles vous planifiez votre heure de congé, nous vous recommandons de faire correspondre le fuseau horaire de votre profil utilisateur à celui de votre planification. Pour plus d’informations, voir les articles suivants :
>
>* [Création d’un planning](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)
>* [Modification du profil d’un utilisateur](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)
>




## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>[!UICONTROL Work] ou version ultérieure (pour configurer votre temps de congé personnel)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Paramétrages du niveau d'accès*</strong></td> 
   <td>[!UICONTROL Manager] avec accès à [!UICONTROL Modifier l’utilisateur] (pour apporter des modifications au calendrier des interruptions des autres utilisateurs)</td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

## Configuration du temps de connexion personnel [!DNL Workfront]

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront], puis cliquez sur votre nom d’utilisateur en regard de votre image de profil.

1. Dans le panneau de gauche, cliquez sur **[!UICONTROL Time Off]**.
1. Sélectionnez la date de votre jour de congé personnel.
1. Sélectionner **[!UICONTROL Toute la journée]**, si vous prenez une journée complète de congé.\
   Laissez cette option désélectionnée si vous prenez moins d’une journée de congé et indiquez les heures de début et de fin de votre congé.

1. Cliquer sur **[!UICONTROL Enregistrer]**.\
   Votre heure de congé est maintenant visible dans les [!DNL Workfront] système dans les outils de planification tels que la grille de ressources. Lorsqu’une tâche vous est affectée pendant cette période, une info-bulle s’affiche pour informer l’utilisateur que vous avez programmé un congé.
