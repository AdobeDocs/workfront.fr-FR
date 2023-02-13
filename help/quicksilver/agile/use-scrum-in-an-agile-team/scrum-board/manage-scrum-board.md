---
product-area: agile-and-teams;projects;user-management
navigation-topic: scrum-board
title: Gestion des articles et des problèmes sur le panorama Scrum
description: Vous pouvez déplacer un article ou un problème du panneau Scrum vers une autre itération ou vers le journal ou le supprimer du panneau Scrum. Lorsque vous supprimez un article ou un problème, il est déplacé dans la Corbeille pendant 30 jours et ne peut être récupéré que par l’administrateur système.
author: Lisa
feature: Agile
exl-id: 72990251-0264-4e68-83ef-1a9cde5b685c
source-git-commit: 6f817ca39c7489b85673ff601faf440fe51ab72c
workflow-type: tm+mt
source-wordcount: '490'
ht-degree: 0%

---

# Gérer les articles et les problèmes sur le [!UICONTROL Scrum] board

Vous pouvez déplacer un article ou un problème depuis la [!UICONTROL Scrum] panoramique sur une autre itération ou sur le journal en attente, ou supprimez-le de la [!UICONTROL Scrum] panorama. Lorsque vous supprimez un article ou un problème, il est déplacé dans la Corbeille pendant 30 jours et ne peut être récupéré que par l’administrateur système.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>[!UICONTROL Work] ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Paramétrages du niveau d'accès*</strong></td> 
   <td> <p>[!UICONTROL Worker] ou version ultérieure</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre [!DNL Workfront] s’ils définissent des restrictions supplémentaires au niveau de votre accès. Pour plus d’informations sur la manière dont une [!DNL Workfront] l’administrateur peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet</strong></td> 
   <td> <p>[!UICONTROL Gérer] Accès à la tâche ou au problème</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

## Déplacer l’histoire ou le problème à partir de [!UICONTROL Scrum] board

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront], puis cliquez sur **[!UICONTROL Équipes]**.
1. Cliquez sur le bouton **[!UICONTROL Equipe de commutation]** icon ![Icône Changer l’équipe](assets/switch-team-icon.png), puis sélectionnez une équipe Scrum dans le menu déroulant ou recherchez une équipe dans la barre de recherche.
1. Dans le panneau de gauche, sélectionnez **[!UICONTROL Itérations]** pour sélectionner une itération spécifique, ou sélectionnez **[!UICONTROL Itération actuelle]**.
1. Cliquez sur le bouton **[!UICONTROL Plus]** sur l’article ou le problème, puis sélectionnez **[!UICONTROL Déplacer vers]**.

   ![Suppression ou déplacement d’un article à partir du panneau Scrum](assets/scrum-delete-move-story.png)

1. Dans le message de confirmation, choisissez l&#39;une des options suivantes :

   <table style="table-layout:auto">
    <tr>
        <td><strong>[!UICONTROL Autre itération]</strong></td>
        <td>Sélectionnez cette option pour déplacer l’élément vers une autre itération, puis choisissez l’itération vers laquelle l’article ou le problème va se déplacer. Si aucune itération n’est définie, vous ne pouvez pas déplacer l’élément.</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Backlog]</strong></td>
        <td>Sélectionnez cette option pour déplacer l’article ou le problème dans le journal de l’équipe.</td>
    </tr>
   </table>

   >[!NOTE]
   >
   >L’élément de travail [!UICONTROL Date de début planifiée] et [!UICONTROL Date d’achèvement prévue] sont affectés par un paramètre de la variable [!UICONTROL Modifier l’équipe] page. Pour plus d’informations, voir la section [[!UICONTROL Configurer] comment les dates sont appliquées lors de l’ajout d’éléments de travail à une itération](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) dans l’article [Configuration de Scrum](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

1. Cliquez sur **[!UICONTROL Déplacer]**.

## Supprimer un article ou un problème de la [!UICONTROL Scrum] board

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront], puis cliquez sur **[!UICONTROL Équipes]**.
1. Cliquez sur le bouton **[!UICONTROL Equipe de commutation]** icon ![Icône Changer l’équipe](assets/switch-team-icon.png), puis sélectionnez une équipe Scrum dans le menu déroulant ou recherchez une équipe dans la barre de recherche.
1. Dans le panneau de gauche, sélectionnez **[!UICONTROL Itérations]** pour sélectionner une itération spécifique, ou sélectionnez **[!UICONTROL Itération actuelle]**.
1. Cliquez sur le bouton **[!UICONTROL Plus]** sur l’article ou le problème, puis sélectionnez **[!UICONTROL Supprimer l’article]** ou **[!UICONTROL Problème de suppression]**.

   ![Suppression ou déplacement d’un article à partir du panneau Scrum](assets/scrum-delete-move-story.png)

1. Dans le message de confirmation, cliquez sur **[!UICONTROL Oui, supprimez-le.]**.
