---
navigation-topic: use-the-gantt-chart
title: Exporter le graphique de Gantt au format PDF
description: Vous pouvez exporter le graphique de Gantt au format PDF.
author: Alina
feature: Work Management
exl-id: 91aad9e0-25c9-4eae-aa66-8aab763d3b76
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '967'
ht-degree: 100%

---

# Exporter le [!UICONTROL graphique de Gantt] au format PDF

Vous pouvez exporter le [!UICONTROL graphique de Gantt] au format PDF.

Après l’export du [!UICONTROL graphique de Gantt] au format PDF, vous pouvez l’imprimer ou le joindre à un e-mail, afin de le partager avec d’autres utilisateurs et utilisatrices.

## Conditions d’accès

Vous devez disposer des éléments suivants pour suivre les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan [!UICONTROL Adobe Workfront]*</td> 
   <td> <p>Tous </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence [!UICONTROL Adobe Workfront]*</td> 
   <td> <p>[!UICONTROL Review] ou niveau supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Accès [!UICONTROL View] ou un accès supérieur aux projets et aux tâches.</p> <p>Note : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration [!DNL Workfront] si des restrictions supplémentaires sont définies pour votre niveau d’accès. Pour plus d’informations sur la manière dont l’administration [!DNL Workfront] peut modifier votre niveau d’accès, consultez la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Accès [!UICONTROL View] ou un accès supérieur au projet.</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, consultez la section <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice [!DNL Workfront].

## Exporter le [!UICONTROL graphique de Gantt]

1. Accédez au [!UICONTROL graphique de Gantt] que vous souhaitez exporter au format PDF, comme décrit dans [Commencer avec le [!UICONTROL graphique de Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/get-started-with-gantt.md).
1. Vérifiez que vous avez configuré le [!UICONTROL graphique de Gantt] pour afficher les informations appropriées avant de les exporter.

   >[!NOTE]
   >
   >Si vous exportez le [!UICONTROL graphique de Gantt] à partir d’une liste de projets, le fichier PDF contiendra uniquement les projets de la liste, et non les tâches de chaque projet. Si vous souhaitez exporter une liste de tâches, vous pouvez le faire à partir du projet auquel elles sont associées, ou en créant un rapport de tâches et en affichant les résultats du rapport dans la [!UICONTROL vue Gantt].

   Vous pouvez configurer les informations suivantes :

   * Filtres, vues et regroupements selon vos besoins dans la liste des tâches. Les filtres et les regroupements sélectionnés en vue Liste sont conservés lors de l’affichage du [!UICONTROL graphique de Gantt]. Les vues sont reflétées sur le [!UICONTROL graphique de Gantt] exporté uniquement dans la liste affichée en regard du [!UICONTROL graphique de Gantt] sur la première page. Les vues ne s’affichent pas sur le [!UICONTROL graphique de Gantt] lui-même.

     >[!TIP]
     >
     >Pour accorder plus de place au [!UICONTROL graphique de Gantt] lui-même, appliquez une vue qui contient le moins de colonnes possible.

   * Options de configuration du [!UICONTROL graphique de Gantt]. Par exemple, vous pouvez activer l’affichage des jalons, des dates, des [!UICONTROL niveaux de référence] ou du [!UICONTROL pourcentage terminé] sur le [!UICONTROL graphique de Gantt].

     Pour plus d’informations, voir [Configurer l’affichage des informations sur le [!UICONTROL graphique de Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

     >[!NOTE]
     >
     > Les affectations ne s’affichent pas sur le [!UICONTROL graphique de Gantt] lorsque le [!UICONTROL graphique de Gantt] est exporté au format PDF. Lorsque le [!UICONTROL graphique de Gantt] est exportée au format PDF, les affectations s’affichent uniquement en vue Liste.

   * Période qui s’affiche sur le [!UICONTROL graphique de Gantt].

     Pour plus d’informations, voir [Afficher des informations sur le [!UICONTROL graphique de Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md).

     L’affichage de la période dans le fichier d’export dépend de la sélection de **[!UICONTROL Ce que je vois]** ou de **[!UICONTROL Plusieurs pages]** dans une étape ultérieure.

1. (Facultatif) Pour inclure uniquement certaines tâches dans le PDF exporté, sélectionnez les tâches à inclure.

   Si vous ne sélectionnez aucune tâche, toutes les tâches sont incluses dans le PDF exporté.

   Par exemple, si vous affichez le [!UICONTROL graphique de Gantt] pour un projet contenant 50 tâches, mais que vous souhaitez afficher uniquement 10 tâches sur le [!UICONTROL graphique de Gantt], sélectionnez les dix tâches à afficher.

1. Cliquez sur l’icône d’imprimante.\
   La boîte de dialogue **[!UICONTROL Exporter vers PDF]** s’affiche.\
   ![exported_gantt_UI.png](assets/exported-gantt-ui-350x225.png)

1. Indiquez si vous souhaitez exporter uniquement ce que vous voyez ou l’ensemble du [!UICONTROL graphique de Gantt] :

   * **[!UICONTROL Ce que je vois] :** exporte toutes les tâches (y compris toutes les sous-tâches) qui s’affichent à l’écran avant d’exporter jusqu’à 500 éléments. (Ce n’est pas ce qui s’affiche dans la section **[!UICONTROL Prévisualisation]** ; la section [!UICONTROL Prévisualisation] ne contient que des données d’exemple.)

     Les sous-tâches sont incluses dans le PDF exporté même si la tâche parent est réduite et que les sous-tâches ne sont pas visibles. Pour inclure uniquement les tâches parent, sélectionnez les tâches parent à inclure et ne sélectionnez pas de sous-tâches.

     Vous pouvez utiliser le menu déroulant **[!UICONTROL Zoom sur]** ou l’outil de curseur pour afficher uniquement une partie du [!UICONTROL graphique de Gantt], comme décrit dans [Afficher des informations dans le [!UICONTROL graphique de Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md).

   * **[!UICONTROL Plusieurs pages] :** exporte l’ensemble du [!UICONTROL graphique de Gantt], même ce qui n’est pas visible sur l’écran actuel, jusqu’à 500 éléments.

     Vous pouvez utiliser le menu déroulant **[!UICONTROL Zoom sur]** ou l’outil de curseur pour déterminer la quantité d’informations affichées sur chaque page, comme décrit dans [Configurer l’affichage des informations sur le [!UICONTROL graphique de Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md). Sélectionnez une option plus granulaire pour afficher davantage de pages à exporter, ou une option moins granulaire pour afficher moins de pages à exporter.

     >[!NOTE]
     >
     >Si vous devez exporter un [!UICONTROL graphique de Gantt] contenant plus de 500 éléments, appliquez un filtre à la liste avant d’afficher le [!UICONTROL graphique de Gantt], de façon à ce que moins de 500 éléments ou 250 pages s’affichent. Pour plus d’informations sur l’application d’un filtre, voir [Vue d’ensemble des filtres](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).
     >
     >
     >Vous ne pouvez pas exporter l’intégralité du graphique de Gantt dans les cas suivants :
     >
     >   
     >   
     >   * S’il s’étend sur plus de 250 pages.
     >   * S’il contient plus de 500 éléments.




1. Si le PDF est imprimé après l’export vers PDF, dans le menu déroulant **[!UICONTROL Format de page]**, sélectionnez le format du papier à imprimer.\
   Vous pouvez sélectionner **[!UICONTROL Lettre]**, **[!UICONTROL Légal]**, **[!UICONTROL Ledger]**, **[!UICONTROL A1]**, **[!UICONTROL A2]**, **[!UICONTROL A3]** (disponible uniquement pour certaines langues), ou **[!UICONTROL A4]**.
1. Dans la section **[!UICONTROL Orientation de page]**, choisissez si vous souhaitez que le PDF soit exporté en orientation paysage ou portrait.
1. Sélectionnez **[!UICONTROL Afficher la légende]** si vous souhaitez inclure la légende dans votre PDF exporté.
1. Cliquez sur **[!UICONTROL Exporter]**.

   Le PDF du [!UICONTROL graphique de Gantt] est créé et téléchargé sur votre ordinateur.

   Remarquez la légende au bas du fichier exporté. Elle explique uniquement les options que vous avez activées dans votre [!UICONTROL graphique de Gantt] et qui sont disponibles dans votre liste de tâches.

   Par exemple, les jalons ne s’affichent dans la légende que si au moins une tâche est associée à un jalon.

   ![gantt_chart_with_updated__limited__legend.png](assets/gantt-chart-with-updated--limited--legend-350x271.png)
