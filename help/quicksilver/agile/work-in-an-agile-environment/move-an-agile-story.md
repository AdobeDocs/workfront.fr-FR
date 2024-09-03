---
product-area: agile-and-teams;projects
navigation-topic: work-in-an-agile-environment
title: Déplacer une histoire agile
description: Vous pouvez déplacer une histoire agile vers une itération différente (pour les équipes Scrum) ou vers la liste d’attente (pour les équipes Kanban et Scrum).
author: Lisa
feature: Agile
exl-id: 0058792e-66b8-4e54-8ce3-50171adff875
source-git-commit: 452f8ddc5268a0d67e32090d166199f2fad7dbc7
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 95%

---

# Déplacer une story agile

Vous pouvez déplacer une histoire agile vers une itération différente (pour les équipes Scrum) ou vers la liste d’attente (pour les équipes Kanban et Scrum).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
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
   <td>Accès [!UICONTROL Manage] à l’histoire</td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Déplacer une histoire d’une itération ou d’un panorama Kanban vers la liste d’attente

1. Accédez à l’itération ou au panorama Kanban qui contient l’histoire que vous souhaitez déplacer vers la liste d’attente.
1. Cliquez sur l’en-tête d’itération en haut de la page.
1. Sur l’onglet **[!UICONTROL Histoires]**, sélectionnez les histoires à déplacer.
1. Cliquez sur **[!UICONTROL Plus]** > **[!UICONTROL Déplacer vers]**.

   La boîte de dialogue **[!UICONTROL Déplacer l’histoire]** s’affiche.

   ![Boîte de dialogue Déplacer l’histoire](assets/iteration-story-move.png)

1. Sélectionnez **Équipe_name&#39;s Backlog**.
Dans l’exemple ci-dessus, le nom de l’équipe est **Marketing**.

1. Cliquez sur **[!UICONTROL Déplacer l’histoire]**.

## Déplacer une histoire vers une autre itération

Vous pouvez déplacer une histoire vers une autre itération pour votre équipe Scrum.

>[!NOTE]
>
>L’option **[!UICONTROL Déplacer vers]** n’est pas disponible pour les histoires parents sur une itération. Vous pouvez déplacer des sous-tâches uniquement vers une autre itération.

1. Accédez à l’itération contenant l’histoire que vous souhaitez déplacer.
1. Cliquez sur l’en-tête d’itération en haut de la page.
1. Sur l’onglet **[!UICONTROL Histoires]**, sélectionnez les histoires à déplacer.
1. Cliquez sur **[!UICONTROL Plus]** > **[!UICONTROL Déplacer vers]**.

   La boîte de dialogue **[!UICONTROL Déplacer l’histoire]** s’affiche.

   ![Boîte de dialogue Déplacer l’histoire](assets/iteration-story-move.png)

1. Sélectionnez **[!UICONTROL Autre itération]**, puis, dans le menu déroulant, sélectionnez l’itération dans laquelle vous souhaitez déplacer l’histoire.

   >[!NOTE]
   >
   >La [!UICONTROL Date de début prévue] et la [!UICONTROL Date d’achèvement prévue] de l’élément de travail sont affectées par un paramètre sur la page [!UICONTROL Modifier l’équipe]. Pour plus d’informations, voir dans la section [[!UICONTROL Configurer] comment les dates sont appliquées lors de l’ajout d’éléments de travail à une itération ](../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configure-how-dates-are-applied-when-adding-work-items-to-an-iteration) dans l’article [Configure Scrum](../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

1. Cliquez sur **[!UICONTROL Déplacer l’histoire]**.
