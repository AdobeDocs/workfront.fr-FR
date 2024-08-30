---
content-type: reference
product-area: user-management;agile-and-teams
navigation-topic: people-teams-and-groups
title: Gérer les requêtes de travail et d’équipe
description: Une demande représente une tâche ou une affectation de problème en attente. Les demandes de travail sont faites aux personnes et les demandes d’équipe sont faites aux équipes.
author: Lisa
feature: People Teams and Groups, Work Management
exl-id: ef96e520-0d5f-4180-a27a-1fbbffff8f2b
source-git-commit: dfd5c7423b65e6065ab9c2094578443b81189abd
workflow-type: tm+mt
source-wordcount: '505'
ht-degree: 93%

---

# Gérer les demandes de travail et d’équipe

Une demande représente une tâche ou une affectation de problème en attente. Les demandes de travail sont faites aux personnes et les demandes d’équipe sont faites aux équipes.

>[!NOTE]
>
>Les équipes Agile ne disposent pas de demandes de l’équipe.

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
   <p>Pour affecter ou travailler sur une requête :
   <p>Nouveau : clair ou supérieur</br>
    or</br>
   Actuel : révision ou version ultérieure</p>
   <p>Pour réaffecter une requête :
   <p>Nouveau : Standard</br>
    or</br>
   Actuel : travail ou plus élevé</p></td>
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Affecter une demande à une équipe {#assign-a-request-to-a-team}

Les personnes gestionnaires de projet et les personnes demandeuses pour un problème peuvent affecter du travail aux équipes lorsqu’elles ne savent pas quelle ressource est la bonne pour effectuer le travail ou quand la personne qui effectue le travail importe peu.

Les tâches affectées à l’équipe restent sur l’onglet [!UICONTROL Demandes d’équipe] jusqu’à ce qu’une personne de l’équipe se charge de travailler sur la demande.

Lorsqu’une demande est affectée à une équipe et à une personne qui n’est pas membre de l’équipe, elle est visible à la fois dans l’onglet [!UICONTROL Demandes d’équipe] et dans la zone des demandes de travail de la personne. Si la personne qui ne fait pas partie de l’équipe se porte volontaire pour travailler sur la tâche, la tâche reste dans l’onglet [!UICONTROL Demandes d’équipe] jusqu’à ce qu’une personne de l’équipe se charge de travailler dessus.

Les équipes peuvent être affectées à des tâches et à des problèmes de l’une des manières suivantes :

* Par le biais du [!UICONTROL graphique de Gantt]
* À partir d’une liste de tâches ou de problèmes (individuellement ou en masse)
* Lors de la création ou de la modification d’une tâche ou d’un problème
* Par le biais de règles de transmission sur une demande (problèmes uniquement)

Vous pouvez affecter manuellement une demande à une équipe à partir de la page de l’équipe, comme décrit dans cette section.

Pour affecter manuellement une demande à une équipe à partir de la page de l’équipe, procédez comme suit :

{{step1-to-team}}

1. Cliquez sur l’icône **[!UICONTROL Changer d’équipe]** ![Icône Changer d’équipe](assets/switch-team-icon.png), puis sélectionnez une nouvelle équipe dans le menu déroulant ou recherchez une équipe dans la barre de recherche.

1. Cliquez sur l’icône **[!UICONTROL Plus]** ![](assets/more-icon.png), puis sélectionnez **[!UICONTROL Envoyer une demande de travail]**.

   ![](assets/edit-team-settings-350x205.png)

1. Renseignez les informations dans la case qui s’ouvre.
1. Cliquez sur **[!UICONTROL Envoyer la demande]**.\
   Une nouvelle tâche est désormais assignée à l’équipe, qui s’affiche dans l’onglet Demandes d’équipe. Cette tâche n’est actuellement pas associée à un projet, mais elle peut être déplacée, comme décrit dans la section [Déplacer les tâches](../../manage-work/tasks/manage-tasks/move-tasks.md).

## Réaffecter des demandes {#reassign-requests}

Vous pouvez réaffecter les demandes qui ont été affectées à votre équipe :

{{step1-to-team}}

1. Cliquez sur l’icône **[!UICONTROL Changer d’équipe]** ![Icône Changer d’équipe](assets/switch-team-icon.png), puis sélectionnez une nouvelle équipe dans le menu déroulant ou recherchez une équipe dans la barre de recherche.
1. Dans le panneau de navigation de gauche, sélectionnez **[!UICONTROL Demandes d’équipe]**.
1. Cliquez sur l’icône **[!UICONTROL Réaffecter]**.

1. Commencez à saisir le nom de la personne, du groupe ou de l’équipe à qui vous souhaitez réaffecter la demande, puis cliquez sur **[!UICONTROL Affecter]**.\
   La demande est réaffectée.
