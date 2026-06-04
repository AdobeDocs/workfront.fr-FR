---
content-type: reference
product-area: user-management;agile-and-teams
navigation-topic: people-teams-and-groups
title: Gérer les demandes de travail et d'équipe
description: Une demande représente une tâche ou une affectation de problème en attente. Les demandes de travail sont faites aux personnes et les demandes d’équipe sont faites aux équipes.
author: Courtney
feature: People Teams and Groups, Work Management
exl-id: ef96e520-0d5f-4180-a27a-1fbbffff8f2b
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/h9ebMyu8AQNPQTzfYkEMbEbHtghIj-wegaml3cM3RMY
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: be65ef36-43e4-48e1-a062-caa3778e15be
  - id: c10f2e93-7a58-4212-aa24-684c265ebe76
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 488
ht-degree: 96%

---

# Gérer les demandes de travail et d’équipe

Une demande représente une tâche ou une affectation de problème en attente. Les demandes de travail sont faites aux personnes et les demandes d’équipe sont faites aux équipes.

>[!NOTE]
>
>Les équipes Agile ne disposent pas de demandes de l’équipe.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>
   <p>Pour affecter ou traiter une demande :
   <p>Léger ou supérieur</p>
  <p>Révision ou supérieur</p>
   <p>Pour réaffecter une demande :
   <p>Standard</p>
   <p>Travail ou supérieur</p></td>
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
