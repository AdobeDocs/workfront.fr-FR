---
navigation-topic: use-the-gantt-chart
title: Exporter le graphique de Gantt au format PDF
description: Vous pouvez exporter le diagramme de Gantt vers un PDF. Après avoir exporté le diagramme de Gantt vers PDF, vous pouvez l’imprimer ou le joindre à un email pour le partager avec d’autres utilisateurs.
author: Alina
feature: Work Management
exl-id: 91aad9e0-25c9-4eae-aa66-8aab763d3b76
source-git-commit: 3097aca9b8fd856bbf3f91a354b5083fa7b23830
workflow-type: tm+mt
source-wordcount: '1045'
ht-degree: 66%

---

# Exporter le [!UICONTROL graphique de Gantt] au format PDF

<!--Audited: 09/2024-->

Vous pouvez exporter le [!UICONTROL graphique de Gantt] au format PDF.

Après l’export du [!UICONTROL graphique de Gantt] au format PDF, vous pouvez l’imprimer ou le joindre à un e-mail, afin de le partager avec d’autres utilisateurs et utilisatrices.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

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
   <td> <p>Nouveau :[!UICONTROL Lumière] ou version ultérieure</p>
   <p>Actuel :[!UICONTROL Révision] ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Accès [!UICONTROL View] ou un accès supérieur aux projets et aux tâches.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Accès [!UICONTROL View] ou un accès supérieur au projet.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations, voir [Exigences d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Exporter le [!UICONTROL graphique de Gantt]

1. Accédez au [!UICONTROL graphique de Gantt] que vous souhaitez exporter au format PDF, comme décrit dans [Commencer avec le [!UICONTROL graphique de Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/get-started-with-gantt.md).
1. Vérifiez que vous avez configuré le [!UICONTROL graphique de Gantt] pour afficher les informations appropriées avant de les exporter.

   >[!NOTE]
   >
   >Si vous exportez le [!UICONTROL graphique de Gantt] à partir d’une liste de projets, le fichier PDF contiendra uniquement les projets de la liste, et non les tâches de chaque projet. Si vous souhaitez exporter une liste de tâches, vous pouvez le faire à partir du projet auquel elles sont associées, ou en créant un rapport de tâches et en affichant les résultats du rapport dans la [!UICONTROL vue Gantt].

   Configurez l’une des informations suivantes :

   * Cliquez sur les icônes **Filtres**, **Affichage** et **Groupement** au-dessus du [!UICONTROL Graphique de Gantt] et ajoutez ou modifiez le filtre, la vue ou le regroupement existant appliqué à la liste des éléments dans le [!UICONTROL Graphique de Gantt].

     Tous les filtres et regroupements sélectionnés en mode Liste sont conservés lors de l’affichage du [!UICONTROL diagramme de Gantt]. Les vues ne sont reflétées sur le [!UICONTROL diagramme de Gantt] exporté que dans la liste qui s’affiche en regard du [!UICONTROL diagramme de Gantt] sur la première page. Les vues ne s’affichent pas sur le [!UICONTROL graphique de Gantt] lui-même.

     >[!TIP]
     >
     >Pour accorder plus de place au [!UICONTROL graphique de Gantt] lui-même, appliquez une vue qui contient le moins de colonnes possible.

   * Sélectionnez l’option **Passer aux dates prévues** pour afficher les dates prévues plutôt que les dates prévues. Par défaut, les dates planifiées s’affichent.

   * Cliquez sur l’icône **Paramètres** ![](assets/settings-icon.png) dans le coin supérieur droit du graphique Gantt et sélectionnez les informations à afficher dans le graphique Gantt. Une fois cette information sélectionnée, elle est incluse dans le fichier du PDF Gantt exporté.

     Sélectionnez l’une des options suivantes :

      * Dates effectives
      * Affectations
      * Niveau de référence
      * Date d’engagement
      * % effectué
      * Chemin critique
      * Losanges de jalons
      * Lignes de jalons
      * Tâches antérieures
      * Statut de progression
      * Dates prévues

     Pour plus d’informations, voir [Configurer l’affichage des informations sur le [!UICONTROL graphique de Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

     >[!NOTE]
     >
     > Les affectations ne s’affichent pas sur le [!UICONTROL graphique de Gantt] lorsque le [!UICONTROL graphique de Gantt] est exporté au format PDF. Lorsque le [!UICONTROL graphique de Gantt] est exportée au format PDF, les affectations s’affichent uniquement en vue Liste.

   * La période affichée sur le [!UICONTROL diagramme de Gantt].

     Pour plus d’informations, voir [Afficher des informations sur le [!UICONTROL graphique de Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md).

     La période s’affiche dans le fichier d’exportation selon que vous avez sélectionné par la suite **[!UICONTROL Ce que je vois]** ou **[!UICONTROL Plusieurs pages]**.

1. (Facultatif) Pour inclure uniquement certaines tâches dans le PDF exporté, sélectionnez les tâches à inclure.

   Si vous ne sélectionnez aucune tâche, toutes les tâches sont incluses dans le PDF exporté.

   Par exemple, si vous affichez le [!UICONTROL graphique de Gantt] pour un projet contenant 50 tâches, mais que vous souhaitez afficher uniquement 10 tâches sur le [!UICONTROL graphique de Gantt], sélectionnez les dix tâches à afficher.

1. Cliquez sur l’icône d’imprimante ![](assets/printer-icon.png) dans le coin supérieur droit du graphique Gantt.
La boîte de dialogue **[!UICONTROL Exporter vers le PDF]** s’affiche.

   ![exported_gantt_UI.png](assets/exported-gantt-ui-350x225.png)

1. Dans la section **Export** , sélectionnez l’une des options suivantes pour indiquer si vous souhaitez exporter uniquement ce que vous voyez ou l’intégralité du [!UICONTROL diagramme de Gantt] :

   * **[!UICONTROL Ce que je vois] :** exporte toutes les tâches (y compris toutes les sous-tâches) qui s’affichent à l’écran avant d’exporter jusqu’à 500 éléments. (Ce n’est pas ce qui s’affiche dans la section **[!UICONTROL Prévisualisation]** ; la section [!UICONTROL Prévisualisation] ne contient que des données d’exemple.)

     Les sous-tâches sont incluses dans le PDF exporté même si la tâche parent est réduite et que les sous-tâches ne sont pas visibles. Pour inclure uniquement les tâches parent, sélectionnez les tâches parent à inclure et ne sélectionnez pas de sous-tâches.

     >[!TIP]
     >
     >Vous pouvez utiliser le menu déroulant **[!UICONTROL Zoom vers]** ou l’outil de curseur pour afficher uniquement une partie du [!UICONTROL diagramme de Gantt], comme décrit dans la section [Affichage des informations dans le [!UICONTROL diagramme de Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md).


   * **[!UICONTROL Plusieurs pages] :** exporte l’intégralité du [!UICONTROL diagramme de Gantt], même celui qui n’est pas visible sur l’écran actuel jusqu’à 500 éléments.

     >[!NOTE]
     >
     >* Vous pouvez utiliser le menu déroulant **[!UICONTROL Zoom sur]** ou l’outil de curseur pour déterminer la quantité d’informations affichées sur chaque page, comme décrit dans [Configurer l’affichage des informations sur le [!UICONTROL graphique de Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md). Sélectionnez une option plus granulaire pour afficher davantage de pages à exporter, ou une option moins granulaire pour afficher moins de pages à exporter.
     >
     >* Si vous devez exporter un [!UICONTROL graphique de Gantt] contenant plus de 500 éléments, appliquez un filtre à la liste avant d’afficher le [!UICONTROL graphique de Gantt], de façon à ce que moins de 500 éléments ou 250 pages s’affichent. Pour plus d’informations sur l’application d’un filtre, voir [Vue d’ensemble des filtres](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).
     >
     >
     >* Vous ne pouvez pas exporter l’intégralité du graphique de Gantt dans les cas suivants :
     >   
     >   * S’il s’étend sur plus de 250 pages.
     >   * S’il contient plus de 500 éléments.


1. Si le PDF est imprimé après l’exportation vers PDF, dans le menu déroulant **[!UICONTROL Format de page]**, sélectionnez le format de papier sur lequel vous souhaitez imprimer.
Vous pouvez sélectionner l’une des options suivantes :

   * **[!UICONTROL Lettre]**
   * **[!UICONTROL Legal]**
   * **[!UICONTROL Ledger]**
   * **[!UICONTROL A1]**
   * **[!UICONTROL A2]**
   * **[!UICONTROL A3]** (disponible uniquement pour certaines langues)
   * **[!UICONTROL A4]**
1. Dans la section **[!UICONTROL Orientation de page]**, choisissez si vous souhaitez que le PDF soit exporté en orientation paysage ou portrait.
1. Sélectionnez **[!UICONTROL Afficher la légende]** si vous souhaitez inclure la légende dans votre PDF exporté.
1. Cliquez sur **[!UICONTROL Exporter]**.

   Le PDF du [!UICONTROL graphique de Gantt] est créé et téléchargé sur votre ordinateur.

   Remarquez la légende au bas du fichier exporté. Elle explique uniquement les options que vous avez activées dans votre [!UICONTROL graphique de Gantt] et qui sont disponibles dans votre liste de tâches.

   Par exemple, les jalons ne s’affichent dans la légende que si au moins une tâche est associée à un jalon.

   ![gantt_chart_with_updated__limited__legend.png](assets/gantt-chart-with-updated--limited--legend-350x271.png)
