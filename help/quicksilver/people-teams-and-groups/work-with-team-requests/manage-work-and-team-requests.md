---
content-type: reference
product-area: user-management;agile-and-teams
navigation-topic: people-teams-and-groups
title: Gérer les requêtes de travail et d’équipe
description: Une requête représente une tâche en attente ou une affectation de problème. Les demandes de travail sont faites aux personnes et les demandes d’équipe sont faites aux équipes.
author: Lisa
feature: People Teams and Groups, Work Management
exl-id: ef96e520-0d5f-4180-a27a-1fbbffff8f2b
source-git-commit: 9693ac3792fec3eca6218a228f2067519ed433ac
workflow-type: tm+mt
source-wordcount: '504'
ht-degree: 0%

---

# Gérer les requêtes de travail et d’équipe

Une requête représente une tâche en attente ou une affectation de problème. Les demandes de travail sont faites aux personnes et les demandes d’équipe sont faites aux équipes.

>[!NOTE]
>
>Les équipes agiles n’ont pas de demandes d’équipe.

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
   <td> <p>Effectuez une révision ou une révision ultérieure pour affecter ou travailler sur une demande ; Utilisation ou ultérieure pour réaffecter une requête</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan ou le type de licence dont vous disposez, contactez votre [!DNL Workfront] administrateur.

## Affectation d’une requête à une équipe {#assign-a-request-to-a-team}

Les chefs de projet et les demandeurs de problèmes peuvent affecter du travail aux équipes lorsqu’ils ne savent pas quelle ressource est la bonne pour effectuer le travail ou quand peu importe qui termine le travail.

Les tâches affectées à l’équipe restent sur la [!UICONTROL Requêtes d’équipe] jusqu’à ce qu’un utilisateur de l’équipe se charge de travailler sur la demande.

Lorsqu’une requête est affectée à une équipe et à un utilisateur qui n’est pas membre de l’équipe, elle est visible dans la variable [!UICONTROL Requêtes d’équipe] et dans la zone des demandes de travail de l’utilisateur. Si l’utilisateur qui ne fait pas partie de l’équipe se porte volontaire pour travailler sur la tâche, la tâche reste dans la [!UICONTROL Requêtes d’équipe] jusqu’à ce qu’un utilisateur de l’équipe se charge de travailler dessus.

Les équipes peuvent être affectées à des tâches et des problèmes de l’une des manières suivantes :

* Par le biais de la [!UICONTROL Graphique Gantt]
* À partir d’une tâche ou d’une liste de problèmes (individuellement ou en bloc)
* Lorsqu’une tâche ou un problème est créé ou modifié
* Par le biais de règles de routage sur une requête (problèmes uniquement)

Vous pouvez affecter manuellement une requête à une équipe à partir de la page de l’équipe, comme décrit dans cette section.

Pour affecter manuellement une requête à une équipe à partir de la page de l’équipe :

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront], puis cliquez sur **[!UICONTROL Équipes]**.

1. Cliquez sur le bouton **[!UICONTROL Equipe de commutation]** icon ![Icône Changer l’équipe](assets/switch-team-icon.png), puis sélectionnez une nouvelle équipe dans le menu déroulant ou recherchez une équipe dans la barre de recherche.

1. Cliquez sur le bouton **[!UICONTROL Plus]** icon ![](assets/more-icon.png), puis sélectionnez **[!UICONTROL Envoyer une requête de travail]**.

   ![](assets/edit-team-settings-350x205.png)

1. Renseignez les informations dans la zone qui s’ouvre.
1. Cliquez sur **[!UICONTROL Envoyer la requête]**.\
   Une nouvelle tâche est désormais assignée à l’équipe, qui s’affiche dans l’onglet Demandes d’équipe . Cette tâche n’est actuellement pas associée à un projet, mais elle peut être déplacée, comme décrit dans la section [Déplacer les tâches](../../manage-work/tasks/manage-tasks/move-tasks.md).

## Réaffectation de requêtes {#reassign-requests}

Vous pouvez réaffecter les demandes qui ont été affectées à votre équipe :

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront], puis cliquez sur **[!UICONTROL Équipes]**.
1. Cliquez sur le bouton **[!UICONTROL Equipe de commutation]** icon ![Icône Changer l’équipe](assets/switch-team-icon.png), puis sélectionnez une nouvelle équipe dans le menu déroulant ou recherchez une équipe dans la barre de recherche.
1. Dans le panneau de navigation de gauche, sélectionnez **[!UICONTROL Requêtes d’équipe]**.
1. Cliquez sur le bouton **[!UICONTROL Réaffecter]** icône .

1. Commencez à saisir le nom de l’utilisateur, du groupe ou de l’équipe auquel vous souhaitez réaffecter la requête, puis cliquez sur **[!UICONTROL Attribuer]**.\
   La requête est réaffectée.
