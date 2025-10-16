---
navigation-topic: use-the-gantt-chart
title: Exporter le graphique de Gantt au format PDF
description: Vous pouvez exporter le graphique Gantt vers un PDF. Ensuite, vous pouvez l’imprimer ou le joindre à un e-mail pour le partager avec d’autres utilisateurs.
author: Alina
feature: Work Management
exl-id: 91aad9e0-25c9-4eae-aa66-8aab763d3b76
source-git-commit: c8987d036e1c1324618cb53ebcbb8fd7e4bcc6a4
workflow-type: tm+mt
source-wordcount: '979'
ht-degree: 40%

---

# Exporter le [!UICONTROL graphique de Gantt] au format PDF

<!--Audited: 08/2025-->

Vous pouvez exporter le [!UICONTROL graphique Gantt] vers un PDF. Ensuite, vous pouvez l’imprimer ou le joindre à un e-mail pour le partager avec d’autres utilisateurs.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package [!UICONTROL Adobe Workfront]</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence [!UICONTROL Adobe Workfront]</td> 
   <td> <p>[!UICONTROL Light] ou version ultérieure</p>
   <p>[!UICONTROL Review] ou niveau supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès [!UICONTROL View] ou un accès supérieur aux projets et aux tâches.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>[!UICONTROL View] ou un accès supérieur au projet et aux tâches</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront] plan</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront] license</td> 
   <td> <p>New:[!UICONTROL Light] or higher</p>
   <p>Current:[!UICONTROL Review] or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>[!UICONTROL View] or higher access to Projects and Tasks</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[!UICONTROL View] or higher access to the project</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

## Exporter le [!UICONTROL graphique de Gantt]

1. Accédez au [!UICONTROL graphique de Gantt] que vous souhaitez exporter au format PDF, comme décrit dans [Commencer avec le [!UICONTROL graphique de Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/get-started-with-gantt.md).
1. Configurez le [!UICONTROL graphique de Gantt] pour afficher les informations appropriées à exporter.

   >[!NOTE]
   >
   >Si vous exportez le [!UICONTROL graphique de Gantt] à partir d’une liste de projets, le fichier PDF contiendra uniquement les projets de la liste, et non les tâches de chaque projet. Si vous souhaitez exporter une liste de tâches, vous pouvez le faire à partir du projet auquel elles sont associées, ou en créant un rapport de tâches et en affichant les résultats du rapport dans la [!UICONTROL vue Gantt].

   Configurez l’une des informations suivantes :

   * Cliquez sur les icônes **Filtres**, **Affichage** et **Regroupement** au-dessus du [!UICONTROL graphique de Gantt] et ajoutez ou modifiez le filtre, la vue ou le regroupement existant appliqué à la liste des éléments du [!UICONTROL graphique de Gantt].

     Tous les filtres et regroupements sélectionnés dans la vue Liste sont conservés lors de l’affichage du [!UICONTROL graphique Gantt]. Les vues sont reflétées sur le [!UICONTROL graphique Gantt] exporté uniquement dans la liste qui s’affiche en regard du [!UICONTROL graphique Gantt] sur la première page. Les vues ne s’affichent pas sur le [!UICONTROL graphique de Gantt] lui-même.

     >[!TIP]
     >
     >Pour libérer de l&#39;espace pour le [!UICONTROL graphique Gantt], appliquez une vue contenant le moins de colonnes possible.

   * Sélectionnez l’option **Passer aux dates prévues** pour afficher les dates prévues plutôt que les dates prévues. Par défaut, les dates prévues s’affichent.

   * Cliquez sur l’icône **Paramètres** ![Icône Paramètres](assets/settings-icon.png) dans le coin supérieur droit du graphique Gantt et sélectionnez les informations à afficher. Une fois sélectionnées, ces informations sont incluses dans le fichier PDF Gantt exporté.

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
      * (Conditionnel) Dates Prévues
      * (Conditionnel) Dates Prévues

     Pour plus d’informations, voir [Configurer l’affichage des informations sur le [!UICONTROL graphique de Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

     >[!NOTE]
     >
     > Les affectations ne s’affichent pas sur le [!UICONTROL graphique de Gantt] lorsque le [!UICONTROL graphique de Gantt] est exporté au format PDF. Une fois exportées, les affectations ne sont affichées que dans la vue Liste.

   * Période affichée dans le [!UICONTROL graphique Gantt]. Son affichage dans le fichier d’exportation dépend de la sélection de **[!UICONTROL Ce que je vois]** ou **[!UICONTROL Plusieurs pages]** à une étape ultérieure.

     Pour plus d’informations, voir [Afficher des informations sur le [!UICONTROL graphique de Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md).



1. (Facultatif) Pour n’inclure que certaines tâches dans le PDF exporté, sélectionnez celles que vous souhaitez inclure. Si vous ne sélectionnez aucune tâche, toutes les tâches sont incluses dans le PDF exporté.

   Par exemple, si vous affichez le [!UICONTROL graphique de Gantt] pour un projet contenant 50 tâches, mais que vous souhaitez afficher uniquement 10 tâches sur le [!UICONTROL graphique de Gantt] exporté, sélectionnez les dix tâches à afficher.

1. Cliquez sur l’icône d’imprimante ![icône d’imprimante](assets/printer-icon.png) dans le coin supérieur droit du graphique Gantt.
La boîte de dialogue **[!UICONTROL Exporter vers PDF]** s’affiche.

   ![Boîte de dialogue Exporter vers PDF](assets/exported-gantt-ui-350x225.png)

1. Dans la section **Exporter**, sélectionnez l’une des options suivantes pour indiquer si vous souhaitez exporter uniquement ce que vous voyez ou l’ensemble du graphique [!UICONTROL Gantt] :

   * **[!UICONTROL Ce que je vois] :** exporte toutes les tâches (y compris toutes les sous-tâches) qui s’affichent à l’écran avant d’exporter jusqu’à 500 éléments. (Ce n’est pas ce qui s’affiche dans la section **[!UICONTROL Aperçu]** ; la section **Aperçu** contient uniquement des données d’exemple.)

     Les sous-tâches sont incluses dans le PDF exporté même si la tâche parent est réduite et que les sous-tâches ne sont pas visibles. Pour inclure uniquement les tâches parent, sélectionnez les tâches parent à inclure et ne sélectionnez pas de sous-tâches.

     >[!TIP]
     >
     >Vous pouvez utiliser l&#39;outil de zoom ou de curseur pour n&#39;afficher qu&#39;une partie du [!UICONTROL graphique Gantt], comme décrit dans la section [Affichage des informations dans le [!UICONTROL graphique Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md). Sélectionnez une option plus granulaire pour afficher davantage de pages à exporter ou sélectionnez une option moins granulaire pour afficher moins de pages à exporter.


   * **[!UICONTROL Pages multiples] :** exporte l’intégralité du [!UICONTROL graphique Gantt] (jusqu’à 500 éléments), y compris les éléments qui ne sont pas visibles sur l’écran actuel.

     >[!NOTE]
     >
     >* Si vous devez exporter un [!UICONTROL graphique de Gantt] contenant plus de 500 éléments, appliquez un filtre à la liste avant d’afficher le [!UICONTROL graphique de Gantt] afin que moins de 500 éléments ou 250 pages s’affichent. Pour plus d’informations sur l’application d’un filtre, voir [Vue d’ensemble des filtres](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).
     >
     >
     >* Vous ne pouvez pas exporter l&#39;ensemble du graphique Gantt dans les cas suivants :
     >   
     >   * Lorsqu’il s’étend sur plus de 250 pages.
     >   * Lorsqu’il contient plus de 500 éléments.


1. Si le PDF est imprimé après avoir été exporté vers PDF, sélectionnez la taille du papier sur lequel vous souhaitez imprimer dans le menu déroulant **[!UICONTROL Taille de la page]**.
Vous pouvez sélectionner l’une des options suivantes :

   * **[!UICONTROL Lettre]**
   * **[!UICONTROL Légal]**
   * **[!UICONTROL Grand livre]**
   * **[!UICONTROL A1]**
   * **[!UICONTROL A2]**
   * **[!UICONTROL A3]** (disponible uniquement pour certaines langues)
   * **[!UICONTROL A4]**
1. Dans la section **[!UICONTROL Orientation de page]**, choisissez si vous souhaitez que le PDF soit exporté en orientation paysage ou portrait.
1. Sélectionnez **[!UICONTROL Afficher la légende]** si vous souhaitez inclure la légende dans votre PDF exporté.
1. Cliquez sur **[!UICONTROL Exporter]**. Le fichier PDF est créé et téléchargé sur votre ordinateur.

   La légende au bas du fichier exporté explique uniquement les options que vous avez activées dans votre [!UICONTROL graphique Gantt] et qui sont disponibles dans votre liste de tâches. Par exemple, les jalons ne s’affichent dans la légende que si au moins une tâche est associée à un jalon.

   ![gantt_chart_with_updated__limited__legend.png](assets/gantt-chart-with-updated--limited--legend-350x271.png)
