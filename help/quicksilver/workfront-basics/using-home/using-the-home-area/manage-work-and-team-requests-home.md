---
product-area: projects;agile-and-teams
navigation-topic: use-the-home-area
title: Gérer les demandes de travail et d’équipe dans la zone d’accueil
description: Lorsque des tâches et des problèmes de travail vous sont affectés, ils sont répertoriés dans les widgets Mon travail, Mes tâches et Mes problèmes .  Vous pouvez afficher, travailler ou supprimer des tâches et des requêtes.
author: Courtney
feature: Get Started with Workfront, Work Management
exl-id: 79826743-eeb9-4849-b46f-cc3f086e3194
source-git-commit: bc60d2cd3dee9be2351d751bafff0e35267ea640
workflow-type: tm+mt
source-wordcount: '834'
ht-degree: 50%

---


# Gérer les tâches et les demandes de l’équipe dans la zone [!UICONTROL Accueil]

Lorsque des tâches et des problèmes de travail vous sont affectés, ils sont répertoriés dans les widgets Mon travail, Mes tâches et Mes problèmes .  Vous pouvez afficher, travailler ou supprimer des tâches et des requêtes.

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licence*</strong></td> 
   <td> <p>[!UICONTROL Work] ou licence supérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurations du niveau d’accès*</strong></td> 
   <td> <p>[!UICONTROL Edit] l’accès aux tâches et aux problèmes</p> <p>Note : si vous n’avez toujours pas d’accès, demandez à votre administrateur ou administratrice [!DNL Workfront] si des restrictions supplémentaires ont été définies dans votre niveau d’accès. Pour plus d’informations sur la manière dont l’administration [!DNL Workfront] peut modifier votre niveau d’accès, consultez la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet</strong></td> 
   <td> <p>Autorisations de contribution ou niveau supérieur pour les tâches et les problèmes sur lesquels vous devez travailler</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir la section <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander un accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez l’administration [!DNL Workfront].

+++

## Afficher un élément de travail dans le widget Mon travail

Les éléments de travail qui vous sont affectés sont affichés dans le widget Mon travail dans [!UICONTROL Accueil]. Vous pouvez configurer les tâches qui s’affichent dans le widget Mon travail à l’aide du filtre situé en haut du widget [!UICONTROL worklist].

Vous pouvez sélectionner des filtres qui affichent les éléments prêts à être traités ou les éléments sur lesquels vous travaillez déjà.

Cet article explique comment utiliser les filtres de la zone d’[!UICONTROL accueil] pour afficher les éléments sur lesquels vous travaillez actuellement ou sur lesquels vous pourriez envisager de commencer à travailler. Pour plus d’informations sur l’utilisation des filtres dans la zone [!UICONTROL Accueil], voir [Afficher les éléments dans la [!UICONTROL liste de travail] dans la zone [!UICONTROL Accueil]](/help/quicksilver/workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md).

Pour afficher un élément de travail dans le widget Mon travail :

1. Cliquez sur le **[!UICONTROL menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit, puis cliquez sur **[!UICONTROL Accueil]**.
1. (Conditionnel) Cliquez sur **Personnaliser** pour ajouter le widget **Mon travail**.

1. Cliquez sur l’icône **Filtrer** ![](assets/filter-nwepng.png) dans le coin supérieur gauche de la liste de travail du widget.

1. Cliquez sur l’une ou l’autre des options suivantes pour les tâches :

   **[!UICONTROL Prêt à démarrer] :** affiche uniquement les tâches et les problèmes qui sont prêts à démarrer. Les deux affirmations suivantes doivent être vraies :

   * Les tâches et leurs parents n’ont pas de tâches/parents antérieurs ou de contraintes de tâches qui les empêchent d’être traités.
   * La [!UICONTROL date de début prévue] des tâches ou des problèmes se situe dans le passé ou jusqu’à deux semaines dans le futur.

   **[!UICONTROL Pas prêt]** : affiche uniquement les tâches et les problèmes qui ne sont pas encore prêts à démarrer. L’une ou l’autre des affirmations suivantes doit être vraie :

   * Les tâches et leurs parents peuvent avoir des tâches/parents antérieurs ou des contraintes de tâches qui les empêchent d’être traités.
   * Les tâches ou les problèmes ont une [!UICONTROL date de début planifiée] qui se situe plus de deux semaines dans le futur.

1. Cliquez sur **[!UICONTROL En train de travailler sur]** sous [!UICONTROL Tâches] ou [!UICONTROL Problèmes] pour afficher les tâches et les problèmes sur lesquels vous travaillez actuellement.
1. Cliquez sur **[!UICONTROL Demandés]** sous [!UICONTROL Problèmes] pour afficher les problèmes qui vous ont été demandés (qui vous sont affectés), mais sur lesquels vous n’avez pas encore accepté de travailler.

## Accès à une requête de l’équipe dans le widget Demande d’équipe

Vous pouvez accéder à une requête affectée à votre équipe directement à partir du widget Demandes d’équipe dans la zone [!UICONTROL Accueil]. Pour plus d’informations sur les demandes d’équipe, voir [Vue d’ensemble des demandes d’équipe](../../../people-teams-and-groups/work-with-team-requests/team-requests-overview.md).

Pour accéder à une demande d’équipe :

1. Cliquez sur le **[!UICONTROL menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit, puis cliquez sur **[!UICONTROL Accueil]**.
1. (Conditionnel) Cliquez sur **Personnaliser** pour ajouter le widget **Requêtes d’équipe** .

   Le widget affiche les demandes de l’équipe sous des regroupements d’équipe. Le widget **[!UICONTROL Requêtes d’équipe]** s’affiche et affiche toutes les requêtes affectées à toute équipe dans laquelle vous vous trouvez. Pour plus d’informations sur l’utilisation des demandes d’équipe, voir [Gérer les demandes d’équipe et de travail](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).

   ![](assets/team-request-widget.png)

## Travail sur un élément de travail dans le widget Mon travail

Lorsque vous cliquez sur le bouton [!UICONTROL Travailler dessus], vous indiquez à l’utilisateur qui a envoyé l’élément de travail et à tout autre utilisateur qui pourrait être affecté à l’élément de travail que vous allez démarrer le travail.

Pour travailler sur un élément de travail :

1. Cliquez sur le **[!UICONTROL menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit, puis cliquez sur **[!UICONTROL Accueil]**.
1. (Conditionnel) Cliquez sur **Personnaliser** pour ajouter le widget **Mon travail**.

1. Dans la zone **[!UICONTROL worklist]** du widget, sélectionnez la requête sur laquelle vous souhaitez travailler, puis cliquez sur **[!UICONTROL Work On It]**.
1. Passez la souris sur l’élément de travail, puis cliquez sur l’icône **Résumé** pour afficher des informations sur l’élément de travail.

   ![](assets/open-summary-new-home.png)


## Suppression d’un élément de travail

Si vous décidez de ne pas travailler sur l’élément de travail, vous pouvez le supprimer de votre liste.

Pour supprimer un élément de travail :

1. Cliquez sur le **[!UICONTROL menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit, puis cliquez sur **[!UICONTROL Accueil]**.
1. (Conditionnel) Cliquez sur **Personnaliser** pour ajouter le widget **Mon travail**.

1. Dans la liste de travail du widget, passez la souris sur l’élément de travail, puis cliquez sur l’icône **Résumé** pour afficher des informations sur l’élément de travail.
   ![](assets/open-summary-new-home.png)
1. dans la section **Affectations** , supprimez votre nom.
   ![](assets/remove-assignment.png)



<!--
## Reassign a request

1. Click the **[!UICONTROL Main Menu]** ![](assets/main-menu-icon.png) in the upper-right corner, then click **[!UICONTROL Home]**.
1. In the **[!UICONTROL Work List]** area, select the request you want to reassign.

1. Click on the **[!UICONTROL Assignments]** widget and remove yourself from the request, then type the name of the user you want to reassign the request to.

   >[!TIP]
   >
   >If the work request is still in the Ready to Start or Not Ready state, you can use the **[!UICONTROL Reassign]** button in the **[!UICONTROL More]** menu in the [!UICONTROL Work List].\
   >![Reassign button](assets/reassign-in-left-panel-350x204.png)

1. If a task's status is changed to [!UICONTROL New] or [!UICONTROL In Progress] after it was completed, you must unassign the user, save the task, then reassign the user in order for the task to reappear in their Home Work List.



## Reply to a request

You can reply to a request to further clarify the request or to propose a new date.

1. Click the **[!UICONTROL Main Menu]** ![](assets/main-menu-icon.png) in the upper-right corner, then click **[!UICONTROL Home]**.
1. In the **[!UICONTROL Work List]** area, select the request you want to reply to.
1. Locate the individual who assigned the request to you.

   You can find this information on the [!UICONTROL Updates] tab of the task. Make sure the option to **[!UICONTROL Show System Updates]** is enabled.

1. Click **[!UICONTROL Start new update]** and begin typing your reply.
1. Enter the name of the recipient in the **[!UICONTROL Notify]** box, then click **[!UICONTROL Update]**.

   >[!TIP]
   >
   >If the work request is still in the Ready to Start or [!UICONTROL Not Ready] state, you can use the **[!UICONTROL Reply]** button in the **[!UICONTROL More]** menu in the [!UICONTROL Work List].\
   >![[!UICONTROL Reply button]](assets/reassign-in-left-panel-350x204.png)   

   -->
