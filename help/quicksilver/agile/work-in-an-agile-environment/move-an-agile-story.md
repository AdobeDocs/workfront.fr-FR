---
product-area: agile-and-teams;projects
navigation-topic: work-in-an-agile-environment
title: Déplacer une histoire agile
description: Vous pouvez déplacer une histoire agile vers une itération différente (pour les équipes Scrum) ou vers le journal en souffrance (pour les équipes Kanban et Scrum).
author: Lisa
feature: Agile
exl-id: 0058792e-66b8-4e54-8ce3-50171adff875
source-git-commit: 11009f24cd482e83319ed9f1ecf3f7a2f4e79d52
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---

# Déplacer une histoire agile

Vous pouvez déplacer une histoire agile vers une itération différente (pour les équipes Scrum) ou vers le journal en souffrance (pour les équipes Kanban et Scrum).

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
   <td> <p>[!UICONTROL Work] ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Paramétrages du niveau d'accès*</strong></td> 
   <td> <p>[!UICONTROL Worker] ou version ultérieure</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre [!DNL Workfront] s’ils définissent des restrictions supplémentaires au niveau de votre accès. Pour plus d’informations sur la manière dont une [!DNL Workfront] l’administrateur peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet</strong></td> 
   <td> <p>[!UICONTROL Gérer] Accès à l’article</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

## Déplacer un article d’une itération ou d’une planche Kanban vers le journal

1. Accédez au panorama d’itération ou Kanban qui contient l’article que vous souhaitez déplacer vers le journal en souffrance.
1. Cliquez sur l’en-tête d’itération en haut de la page.
1. Sur le **[!UICONTROL Histoires]** sélectionnez les articles à déplacer.
1. Cliquez sur **[!UICONTROL Plus]** > **[!UICONTROL Déplacer vers]**.

   Le **[!UICONTROL Déplacer l’article]** s’affiche.

   ![Boîte de dialogue Déplacer l’article](assets/iteration-story-move.png)

1. Sélectionner *Team_name* est En retard.\
   Dans l’exemple ci-dessus, le nom de l’équipe est &#x200B; **Marketing.**

1. Cliquez sur **[!UICONTROL Déplacer l’article]**.

## Déplacer une histoire vers une autre itération

Vous pouvez déplacer une histoire vers une autre itération pour votre équipe Scrum.

>[!NOTE]
>
>Le **[!UICONTROL Déplacer vers]** n’est pas disponible pour les articles parents sur une itération. Vous pouvez uniquement déplacer des sous-tâches vers une autre itération.

1. Accédez à l’itération contenant l’histoire que vous souhaitez déplacer.
1. Cliquez sur l’en-tête d’itération en haut de la page.
1. Sur le **[!UICONTROL Histoires]** sélectionnez les articles à déplacer.
1. Cliquez sur **[!UICONTROL Plus]** > **[!UICONTROL Déplacer vers]**.

   Le **[!UICONTROL Déplacer l’article]** s’affiche.

   ![Boîte de dialogue Déplacer l’article](assets/iteration-story-move.png)

1. Sélectionner **[!UICONTROL Une autre itération]**, puis, dans le menu déroulant, sélectionnez l’itération dans laquelle vous souhaitez déplacer l’histoire.

   >[!NOTE]
   >
   >L’élément de travail [!UICONTROL Date de début planifiée] et [!UICONTROL Date d’achèvement prévue] sont affectés par un paramètre de la variable [!UICONTROL Modifier l’équipe] page. Pour plus d’informations, voir la section [[!UICONTROL Configurer] comment les dates sont appliquées lors de l’ajout d’éléments de travail à une itération](../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) dans l’article [Configuration de Scrum](../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

1. Cliquez sur **[!UICONTROL Déplacer l’article]**.
