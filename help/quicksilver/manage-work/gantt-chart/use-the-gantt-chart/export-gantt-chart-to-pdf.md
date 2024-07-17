---
navigation-topic: use-the-gantt-chart
title: Exporter le graphique de Gantt au format PDF
description: Vous pouvez exporter le diagramme de Gantt vers un PDF.
author: Alina
feature: Work Management
exl-id: 91aad9e0-25c9-4eae-aa66-8aab763d3b76
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '967'
ht-degree: 6%

---

# Exportez le [!UICONTROL diagramme de Gantt] vers PDF

Vous pouvez exporter le [!UICONTROL diagramme de Gantt] vers un PDF.

Après avoir exporté le [!UICONTROL diagramme de Gantt] vers PDF, vous pouvez l’imprimer ou le joindre à un email, pour le partager avec d’autres utilisateurs.

## Conditions d’accès

Pour suivre les étapes de cet article, vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule [!UICONTROL Adobe Workfront]*</td> 
   <td> <p>N’importe quelle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence [!UICONTROL Adobe Workfront]*</td> 
   <td> <p>[!UICONTROL Review] ou niveau supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Accès à [!UICONTROL View] ou supérieur à Projects and Tasks</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur [!DNL Workfront] s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la manière dont un administrateur ou une administratrice [!DNL Workfront] peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>[!UICONTROL Affichage] ou accès supérieur au projet</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice [!DNL Workfront].

## Exporter le [!UICONTROL diagramme de Gantt]

1. Accédez au [!UICONTROL diagramme de Gantt] que vous souhaitez exporter vers PDF, comme décrit dans la section [Prise en main du [!UICONTROL diagramme de Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/get-started-with-gantt.md).
1. Assurez-vous d’avoir configuré le [!UICONTROL diagramme de Gantt] pour afficher les informations appropriées avant de l’exporter.

   >[!NOTE]
   >
   >Si vous exportez le [!UICONTROL diagramme de Gantt] à partir d’une liste de projets, le fichier du PDF contient uniquement les projets de la liste, et non les tâches de chaque projet. Si vous souhaitez exporter une liste de tâches, vous pouvez le faire à partir du projet auquel elles sont associées, ou en créant un rapport de tâches et en affichant les résultats du rapport dans la [!UICONTROL vue Gantt].

   Vous pouvez configurer les informations suivantes :

   * Filtres, vues et regroupements selon vos besoins dans la liste des tâches. Tous les filtres et groupes sélectionnés en mode Liste sont conservés lors de l’affichage du [!UICONTROL diagramme de Gantt]. Les vues ne sont reflétées sur le [!UICONTROL diagramme de Gantt] exporté que dans la liste affichée en regard du [!UICONTROL  diagramme de Gantt] sur la première page. Les vues ne sont pas affichées sur le [!UICONTROL diagramme de Gantt] lui-même.

     >[!TIP]
     >
     >Pour accorder plus d’espace au [!UICONTROL diagramme de Gantt] lui-même, appliquez une vue qui contient le moins de colonnes possible.

   * Options de configuration sur le [!UICONTROL diagramme de Gantt]. Par exemple, vous pouvez activer les jalons, dates, [!UICONTROL lignes de base] ou [!UICONTROL pourcentage terminé] pour apparaître sur le [!UICONTROL diagramme de Gantt].

     Pour plus d’informations, voir   [Configurez le mode d’affichage des informations sur le [!UICONTROL diagramme de Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

     >[!NOTE]
     >
     > Les affectations ne s’affichent pas sur le [!UICONTROL diagramme de Gantt] lorsque le [!UICONTROL diagramme de Gantt] est exporté vers PDF. Lorsque le [!UICONTROL diagramme de Gantt] est exporté vers PDF, les affectations ne s’affichent que dans le mode Liste.

   * La période affichée sur le [!UICONTROL diagramme de Gantt].\

     Pour plus d’informations, voir [Affichage des informations dans le [!UICONTROL diagramme de Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md).

     L’affichage de la période dans le fichier d’exportation dépend de si vous sélectionnez **[!UICONTROL Ce que je vois]** ou **[!UICONTROL Plusieurs pages]** à une étape ultérieure.

1. (Facultatif) Pour inclure uniquement certaines tâches dans le PDF exporté, sélectionnez les tâches à inclure.

   Si vous ne sélectionnez aucune tâche, toutes les tâches sont incluses dans le PDF exporté.

   Par exemple, si vous affichez le [!UICONTROL diagramme de Gantt] pour un projet qui contient 50 tâches, mais que vous souhaitez afficher uniquement 10 tâches sur le [!UICONTROL diagramme de Gantt] exporté, sélectionnez les 10 tâches à afficher.

1. Cliquez sur l’icône de l’imprimante.\
   La boîte de dialogue **[!UICONTROL Exporter vers le PDF]** s’affiche.\
   ![(export_gantt_UI.png](assets/exported-gantt-ui-350x225.png)

1. Indiquez si vous souhaitez exporter uniquement ce que vous voyez ou l’intégralité du [!UICONTROL diagramme de Gantt] :

   * **[!UICONTROL Ce que je vois] :** exporte toutes les tâches (y compris toutes les sous-tâches) qui s’affichent à l’écran avant d’exporter jusqu’à 500 éléments. (Ce n&#39;est pas ce qui s&#39;affiche dans la section **[!UICONTROL Preview]** ; la section [!UICONTROL Preview] ne contient que des exemples de données.)

     Les sous-tâches sont incluses dans le PDF exporté même si la tâche parent est réduite et que les sous-tâches ne sont pas visibles. Pour inclure uniquement les tâches parentes, sélectionnez les tâches parentes à inclure et ne sélectionnez pas les sous-tâches.

     Vous pouvez utiliser le menu déroulant **[!UICONTROL Zoom vers]** ou l’outil de curseur pour afficher uniquement une partie du [!UICONTROL diagramme de Gantt], comme décrit dans la section [Affichage des informations dans le [!UICONTROL diagramme de Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md) .

   * **[!UICONTROL Plusieurs pages] :** exporte l’intégralité du [!UICONTROL diagramme de Gantt], même celui qui n’est pas visible sur l’écran actuel jusqu’à 500 éléments.\

     Vous pouvez utiliser le menu déroulant **[!UICONTROL Zoom sur]** ou l’outil de réglette pour déterminer la quantité d’informations affichées sur chaque page, comme décrit dans la section [Configurer l’affichage des informations sur le [!UICONTROL diagramme de Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md). Sélectionnez une option plus granulaire pour afficher plus de pages à exporter ou une option moins granulaire pour afficher moins de pages à exporter.

     >[!NOTE]
     >
     >Si vous devez exporter un [!UICONTROL diagramme de Gantt] contenant plus de 500 éléments, appliquez un filtre à la liste avant d’afficher le [!UICONTROL diagramme de Gantt] afin que moins de 500 éléments ou 250 pages s’affichent. Pour plus d’informations sur l’application d’un filtre, voir [Présentation des filtres](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).
     >
     >
     >Vous ne pouvez pas exporter l’intégralité du diagramme de Gantt dans les cas suivants :
     >
     >   
     >   
     >   * S’étend sur plus de 250 pages.
     >   * Lorsqu’il contient plus de 500 éléments




1. Si le PDF est imprimé après l’exportation vers PDF, dans le menu déroulant **[!UICONTROL Format de page]**, sélectionnez le format de papier sur lequel vous souhaitez imprimer.\
   Vous pouvez sélectionner **[!UICONTROL Lettre]**, **[!UICONTROL Juridique]**, **[!UICONTROL Livre]**, **[!UICONTROL A1]**, **[!UICONTROL A2]**, **[!UICONTROL A3]** (disponible uniquement pour certaines langues) ou **[!UICONTROL A4]**.
1. Dans la section **[!UICONTROL Orientation de page]**, indiquez si vous souhaitez que le PDF soit exporté en orientation paysage ou portrait.
1. Sélectionnez **[!UICONTROL Afficher la légende]** si vous souhaitez inclure la légende dans votre PDF exporté.
1. Cliquez sur **[!UICONTROL Export]**.

   Le pdf du [!UICONTROL diagramme de Gantt] est créé et téléchargé sur votre ordinateur.

   Notez la légende au bas du fichier exporté. Il explique uniquement les options que vous avez activées dans votre [!UICONTROL diagramme de Gantt] et qui sont disponibles dans votre liste de tâches.

   Par exemple, les jalons ne s’affichent dans la légende que si au moins une tâche est associée à un jalon.

   ![gantt_chart_with_updated__limited__legend.png](assets/gantt-chart-with-updated--limited--legend-350x271.png)
