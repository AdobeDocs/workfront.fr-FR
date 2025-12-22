---
product-area: agile-and-teams;projects;user-management
navigation-topic: scrum-board
title: Gérer les histoires et les événements sur le scrum board
description: Vous pouvez déplacer une histoire ou un problème du panorama Scrum vers une autre itération ou vers la liste d’attente ou supprimer l’élément du panorama Scrum. Lorsque vous supprimez une histoire ou un problème, l’élément est placé dans la Corbeille pendant 30 jours et ne peut être récupéré que par l’administrateur ou l’administratrice système.
author: Jenny
feature: Agile
exl-id: 72990251-0264-4e68-83ef-1a9cde5b685c
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 84%

---

# Gérer les histoires et les problèmes sur le panorama [!UICONTROL Scrum]

Vous pouvez déplacer une histoire ou un problème du panorama [!UICONTROL Scrum] vers une autre itération ou vers la liste d’attente ou supprimer l’élément du panorama [!UICONTROL Scrum]. Lorsque vous supprimez une histoire ou un problème, l’élément est placé dans la Corbeille pendant 30 jours et ne peut être récupéré que par l’administrateur ou l’administratrice système.

Pour supprimer une tâche ou un événement de l&#39;itération sans la supprimer ni l&#39;envoyer à la liste d&#39;attente, accédez au projet et supprimez l&#39;équipe Agile de la colonne Affectation . Cela supprime la tâche ou l’événement du scrum board, mais il reste sur le projet.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td> <p>Nouvelle : [!UICONTROL Standard]</p> 
   ou
   <p>Actuelle : [!UICONTROL Work] ou niveau supérieur</p> </td> 
  </tr>
   <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td>Accès en [!UICONTROL Manage] à la tâche ou au problème </td> 
  </tr>
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Déplacer une histoire ou un événement du tableau [!UICONTROL Scrum]

{{step1-to-team}}

1. Cliquez sur l’icône **[!UICONTROL Changer d’équipe]** ![Icône Changer d’équipe](assets/switch-team-icon.png), puis sélectionnez une équipe Scrum dans le menu déroulant ou recherchez une équipe dans la barre de recherche.
1. Dans le panneau de gauche, sélectionnez **[!UICONTROL Itérations]** pour sélectionner une itération spécifique, ou sélectionnez **[!UICONTROL Itération actuelle]**.
1. Cliquez sur l’icône **[!UICONTROL Plus]** sur l’histoire ou le problème, puis sélectionnez **[!UICONTROL Déplacer vers]**.

   ![Suppression ou déplacement d’une histoire du panorama Scrum](assets/scrum-delete-move-story.png)

1. Dans le message de confirmation, choisissez l’une des options suivantes :

   <table style="table-layout:auto">
    <tr>
        <td><strong>[!UICONTROL Another iteration]</strong></td>
        <td>Sélectionnez cette option pour déplacer l’élément vers une autre itération, puis choisissez l’itération vers laquelle l’élément (histoire ou problème) va être déplacé. Si aucune itération n’est définie, vous ne pouvez pas déplacer l’élément.</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Backlog]</strong></td>
        <td>Sélectionnez cette option pour déplacer l’histoire ou le problème vers la liste d’attente de l’équipe.</td>
    </tr>
   </table>

   >[!NOTE]
   >
   >Les [!UICONTROL Date de début prévue] et [!UICONTROL Date d’achèvement prévue] de l’élément de travail sont affectées par un paramètre de la page [!UICONTROL Modifier l’équipe]. Pour plus d’informations, voir la section [[!UICONTROL Configurer] comment les dates sont appliquées lors de l’ajout d’éléments de travail à une itération](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) dans l’article [Configurer Scrum](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

1. Cliquez sur **[!UICONTROL Déplacer]**.

## Supprimer une histoire ou un événement du tableau [!UICONTROL Scrum]

{{step1-to-team}}

1. Cliquez sur l’icône **[!UICONTROL Changer d’équipe]** ![Icône Changer d’équipe](assets/switch-team-icon.png), puis sélectionnez une équipe Scrum dans le menu déroulant ou recherchez une équipe dans la barre de recherche.
1. Dans le panneau de gauche, sélectionnez **[!UICONTROL Itérations]** pour sélectionner une itération spécifique, ou sélectionnez **[!UICONTROL Itération actuelle]**.
1. Cliquez sur l’icône **[!UICONTROL Plus]** sur l’histoire ou le problème, puis sélectionnez **[!UICONTROL Supprimer l’histoire]** ou **[!UICONTROL Supprimer le problème]**.

   ![Suppression ou déplacement d’une histoire du panorama Scrum](assets/scrum-delete-move-story.png)

1. Dans le message de confirmation, cliquez sur **[!UICONTROL Oui, supprimer]**.
