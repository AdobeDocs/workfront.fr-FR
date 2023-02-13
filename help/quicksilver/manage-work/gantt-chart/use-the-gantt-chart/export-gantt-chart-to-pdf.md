---
navigation-topic: use-the-gantt-chart
title: Exportation du diagramme de Gantt vers PDF
description: Vous pouvez exporter le diagramme de Gantt vers un PDF.
author: Alina
feature: Work Management
exl-id: 91aad9e0-25c9-4eae-aa66-8aab763d3b76
source-git-commit: 2db4a79cad71b550b7de573c5b27293b6582858f
workflow-type: tm+mt
source-wordcount: '965'
ht-degree: 0%

---

# Exportez le [!UICONTROL Graphique Gantt] à PDF

Vous pouvez exporter le [!UICONTROL Graphique Gantt] à un PDF.

Après l’exportation de la variable [!UICONTROL Graphique Gantt] pour PDF, vous pouvez l’imprimer ou le joindre à un email, afin de le partager avec d’autres utilisateurs.

## Exigences d’accès

Pour suivre les étapes de cet article, vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule [!UICONTROL Adobe Workfront]*</td> 
   <td> <p>Tous </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence [!UICONTROL Adobe Workfront]*</td> 
   <td> <p>[!UICONTROL Review] ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Accès à [!UICONTROL View] ou supérieur à Projects and Tasks</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre [!DNL Workfront] s’ils définissent des restrictions supplémentaires au niveau de votre accès. Pour plus d’informations sur la manière dont une [!DNL Workfront] l’administrateur peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>[!UICONTROL Affichage] ou accès supérieur au projet</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

## Exportez le [!UICONTROL Graphique Gantt]

1. Accédez au [!UICONTROL Graphique Gantt] que vous souhaitez exporter vers PDF, comme décrit dans la section [Prise en main de la fonction [!UICONTROL Graphique Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/get-started-with-gantt.md).
1. Assurez-vous que vous avez configuré la variable [!UICONTROL Graphique Gantt] pour afficher les informations appropriées avant de les exporter.

   >[!NOTE]
   >
   >Si vous exportez la variable [!UICONTROL Graphique Gantt] à partir d’une liste de projets, le fichier du PDF contient uniquement les projets de la liste, et non les tâches de chaque projet. Si vous souhaitez exporter une liste de tâches, vous pouvez le faire à partir du projet auquel elles sont associées, ou en créant un rapport de tâches et en affichant les résultats du rapport dans la [!UICONTROL Vue Gantt].

   Vous pouvez configurer les informations suivantes :

   * Filtres, vues et regroupements selon vos besoins dans la liste des tâches. Les filtres et les groupes sélectionnés en mode Liste sont conservés lors de l’affichage de la variable [!UICONTROL Graphique Gantt]. Les vues sont répercutées sur l’exportation [!UICONTROL Graphique Gantt] uniquement dans la liste affichée en regard de la fonction [!UICONTROL Graphique Gantt] sur la première page. Les vues ne s’affichent pas sur la [!UICONTROL Graphique Gantt] elle-même.

      >[!TIP]
      >
      >Pour accorder plus d’espace au [!UICONTROL Graphique Gantt] lui-même, appliquez une vue qui contient le moins de colonnes possible.

   * Options de configuration de la variable [!UICONTROL Graphique Gantt]. Par exemple, vous pouvez activer les jalons, les dates, [!UICONTROL lignes de base]ou [!UICONTROL percent complete] pour apparaître sur le [!UICONTROL Graphique Gantt].

      Pour plus d’informations, voir   [Configurez l’affichage des informations sur le [!UICONTROL Graphique Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

      >[!NOTE]
      >
      > Les affectations ne s’affichent pas sur la page [!UICONTROL Graphique Gantt] lorsque la variable [!UICONTROL Graphique Gantt] est exporté vers PDF. Lorsque la variable [!UICONTROL Graphique Gantt] est exportée vers PDF, les affectations s’affichent uniquement en mode Liste.

   * La période affichée sur la page [!UICONTROL Graphique Gantt].\

      Pour plus d’informations, voir [Affichage des informations dans le [!UICONTROL Graphique Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md).

      L’affichage de la période dans le fichier d’exportation dépend de la sélection ou non de la **[!UICONTROL Ce que je vois]** ou **[!UICONTROL Plusieurs pages]** dans une étape ultérieure.

1. (Facultatif) Pour inclure uniquement certaines tâches dans le PDF exporté, sélectionnez les tâches à inclure.

   Si vous ne sélectionnez aucune tâche, toutes les tâches sont incluses dans le PDF exporté.

   Par exemple, si vous affichez le [!UICONTROL Graphique Gantt] pour un projet qui contient 50 tâches, mais que vous souhaitez afficher uniquement 10 tâches sur le [!UICONTROL Graphique Gantt], sélectionnez les 10 tâches à afficher.

1. Cliquez sur l’icône de l’imprimante.\
   Le **[!UICONTROL Exporter vers le PDF]** s’affiche.\
   ![export_gantt_UI.png](assets/exported-gantt-ui-350x225.png)

1. Indiquez si vous souhaitez n’exporter que ce que vous voyez ou l’ensemble [!UICONTROL Graphique Gantt]:

   * **[!UICONTROL Ce que je vois]:** Exporte toutes les tâches (y compris toutes les sous-tâches) qui s’affichent à l’écran avant d’exporter jusqu’à 500 éléments. (Ce n’est pas ce qui s’affiche dans la **[!UICONTROL Aperçu]** section; la valeur [!UICONTROL Aperçu] ne contient que des exemples de données.)

      Les sous-tâches sont incluses dans le PDF exporté même si la tâche parent est réduite et que les sous-tâches ne sont pas visibles. Pour inclure uniquement les tâches parentes, sélectionnez les tâches parentes à inclure et ne sélectionnez pas les sous-tâches.

      Vous pouvez utiliser la variable **[!UICONTROL Zoom sur]** pour afficher uniquement une partie de la [!UICONTROL Graphique Gantt], comme décrit dans [Affichage des informations dans le [!UICONTROL Graphique Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md) .

   * **[!UICONTROL Plusieurs pages]:** Exporte l’intégralité de la variable [!UICONTROL Graphique Gantt], même ce qui n’est pas visible sur l’écran actuel, jusqu’à 500 éléments.\

      Vous pouvez utiliser la variable **[!UICONTROL Zoom sur]** menu déroulant ou l’outil de curseur pour déterminer la quantité d’informations affichées sur chaque page, comme décrit dans la section [Configurez l’affichage des informations sur le [!UICONTROL Graphique Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md). Sélectionnez une option plus granulaire pour afficher plus de pages à exporter ou une option moins granulaire pour afficher moins de pages à exporter.

      >[!NOTE]
      >
      >Si vous devez exporter un [!UICONTROL Graphique Gantt] qui contient plus de 500 éléments, appliquez un filtre à la liste avant d’afficher la variable [!UICONTROL Graphique Gantt] afin que moins de 500 éléments ou 250 pages s’affichent. Pour plus d’informations sur l’application d’un filtre, voir  [Présentation des filtres dans [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).
      >
      >
      >Vous ne pouvez pas exporter l’intégralité du diagramme de Gantt dans les cas suivants :
      >
      >   
      >   
      >   * S’étend sur plus de 250 pages.
      >   * Lorsqu’il contient plus de 500 éléments





1. Si le PDF est imprimé après l’exportation vers PDF, dans la variable **[!UICONTROL Format de page]** dans le menu déroulant, sélectionnez la taille du papier à imprimer.\
   Vous pouvez sélectionner **[!UICONTROL Lettre]**, **[!UICONTROL Mentions légales]**, **[!UICONTROL Journal]**, **[!UICONTROL A1]**, **[!UICONTROL A2]**, **[!UICONTROL A3]** (disponible uniquement pour certaines langues) ou **[!UICONTROL A4]**.
1. Dans le **[!UICONTROL Orientation de page]** , choisissez si vous souhaitez que le PDF soit exporté en orientation paysage ou portrait.
1. Sélectionner **[!UICONTROL Afficher la légende]** si vous souhaitez inclure la légende dans votre PDF exporté.
1. Cliquez sur **[!UICONTROL Exporter]**.

   Le pdf du fichier [!UICONTROL Graphique Gantt] est créé et téléchargé sur votre ordinateur.

   Notez la légende au bas du fichier exporté. Cela explique uniquement les options que vous avez activées dans votre [!UICONTROL Graphique Gantt] et qui sont disponibles dans votre liste de tâches.

   Par exemple, les jalons ne s’affichent dans la légende que si au moins une tâche est associée à un jalon.

   ![gantt_chart_with_updated__limited__legend.png](assets/gantt-chart-with-updated--limited--legend-350x271.png)
