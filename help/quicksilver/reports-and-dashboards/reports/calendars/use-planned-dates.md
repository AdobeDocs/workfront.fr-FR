---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: Utilisation des dates prévues dans un rapport de calendrier
description: Un rapport de calendrier est un rapport dynamique qui fournit une représentation visuelle de votre travail. Vous pouvez utiliser les champs Date prévue dans un rapport de calendrier pour les tâches, les problèmes et les projets.
author: Lisa
feature: Reports and Dashboards
exl-id: 27bf6f03-2f6b-4556-a715-75c4a21bfbbb
source-git-commit: 78cfafe4c9a0fb846533c04da392a09dc1dbc9f1
workflow-type: tm+mt
source-wordcount: '621'
ht-degree: 92%

---

# Utiliser [!UICONTROL Dates prévues] dans un rapport de calendrier

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.</span> 
-->

Un rapport de calendrier est un rapport dynamique qui fournit une représentation visuelle de votre travail. Vous pouvez afficher les champs [!UICONTROL Date prévue] dans un rapport de calendrier pour les objets suivants :

* Tâches
* Problèmes
* Projets

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
   <td role="rowheader">[!DNL Adobe Workfront plan]</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td><p>Nouveau : Standard</p>
       <p>ou</p>
       <p>Actuel : formule</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès [!UICONTROL Edit] aux [!UICONTROL Reports], [!UICONTROL Dashboards] et [!UICONTROL Calendars]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td>[!UICONTROL Manage] l’accès au rapport de calendrier</td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurer le groupe d’éléments en production

Vous pouvez choisir la manière dont le groupe d’éléments doit s’afficher sur votre calendrier.

{{step1-to-calendars}}

1. Sélectionnez le calendrier auquel vous souhaitez ajouter un nouveau groupe d&#39;éléments.
Ou
Cliquez sur **[!UICONTROL + Nouveau calendrier]** puis saisissez le nom du calendrier.

   >[!NOTE]
   >
   >Pour créer un rapport de calendrier, vous devez disposer de l’accès Modifier aux rapports, tableaux de bord et calendriers dans votre niveau d’accès.

1. Sur la gauche, cliquez sur **[!UICONTROL Ajouter au calendrier]**, puis sur **[!UICONTROL Ajouter des éléments avancés]**.

1. Indiquez les informations suivantes :

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Name this group of items]</strong></td>
      <td>Saisissez un nom pour le groupe d’éléments.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Color]</strong></td>
      <td>Sélectionnez une couleur pour le groupe d’éléments. Tous les éléments s’affichent dans la couleur sélectionnée sur le rapport du calendrier.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Date Field]</strong></td>
      <td><p>Choisissez les <strong>[!UICONTROL Planned dates]</strong>. Pour plus d’informations sur les dates prévues, voir </p>
       <ul>
        <li><a href="../../../manage-work/projects/planning-a-project/project-planned-start-date.md" class="MCXref xref">Vue d’ensemble de la Date de début prévue du projet</a></li>
        <li><a href="../../../manage-work/tasks/task-information/task-planned-start-date.md" class="MCXref xref">Vue d’ensemble de la Date de début prévue de la tâche</a></li>
        <li><a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Vue d’ensemble de la Date d’achèvement prévue de la tâche</a></li>
        <li><a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">Définir la date d’achèvement prévue du projet</a><br></li>
       </ul></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Sur le calendrier, afficher</strong></td>
      <td><p>Choisissez le mode d’affichage des dates :</p>
       <ul>
        <li><strong>[!UICONTROL Start Date Only]</strong> : le calendrier affiche l’objet à une seule date.</li>
        <li><strong>[!UICONTROL End Date Only]</strong> : le calendrier affiche l’objet à une seule date.</li>
        <li><strong>[!UICONTROL Duration] (du début à la fin)</strong> : le calendrier affiche l’objet sur plusieurs jours.</li>
       </ul></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader"><strong>[!UICONTROL Switch to actual dates when available]</strong></td>
      <td><p>Le calendrier passe automatiquement aux dates réelles lorsqu’elles sont disponibles. <br>Sélectionnez <strong>[!UICONTROL Yes]</strong> ou <strong>[!UICONTROL No]</strong> pour passer aux dates effectives lorsqu’elles sont disponibles. Pour plus d’informations sur les dates effectives, consultez</p>
       <ul>
        <li><a href="../../../manage-work/projects/planning-a-project/project-actual-start-date.md" class="MCXref xref">Vue d’ensemble de la date de début effective du projet </a></li>
        <li><a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref">Vue d’ensemble de la date d’achèvement effective du projet </a></li>
       </ul></td>
     </tr>
    </tbody>
   </table>

1. Passez à la section suivante.

## Ajouter des objets au groupe d’éléments dans Production

Après avoir défini le mode d’affichage des éléments, vous devez ajouter au regroupement les objets que vous souhaitez voir apparaître sur le calendrier.

1. Dans la section **[!UICONTROL Que souhaitez-vous ajouter au calendrier ?]**, sélectionnez

   * **[!UICONTROL Tâches]**
   * **[!UICONTROL Projets]**
   * **[!UICONTROL Événements]**

1. Cliquez sur **[!UICONTROL Ajouter des tâches]**, **[!UICONTROL Ajouter des projets]** ou **[!UICONTROL Ajouter des problèmes]**, selon le type d’objet que vous ajoutez au calendrier.
   ![Sélection d’un objet pour le calendrier](assets/field-name.png)

1. Dans le menu déroulant, commencez à saisir le nom du champ, puis sélectionnez la source du champ de l’objet que vous souhaitez afficher dans le calendrier (par exemple, **[!UICONTROL Tâches en retard]**).
1. Définissez une condition pour le regroupement de calendrier.

   ![Instruction de condition](assets/condition-statement-calendar.png)

   Pour en savoir plus sur la définition de conditions, voir [Modificateurs de filtre et de condition](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. (Facultatif) Spécifiez des objets supplémentaires pour le groupe de calendriers en répétant les étapes 1 à 4.
1. Dans le champ **[!UICONTROL Définissez les libellés des Tâches/Projets/Problèmes sur ...]**, sélectionnez le libellé des objets de ce regroupement de calendrier.

   >[!NOTE]
   >
   >Si les options relatives aux libellés par défaut ne sont pas disponibles pour un objet donné, le nom de l’objet est affiché à la place. Par exemple, lorsque le libellé [!UICONTROL Tâche parent] est sélectionné et qu’aucune tâche parent n’est associée à l’objet, [!DNL Adobe Workfront] affiche le nom de l’objet affiché dans le calendrier.

1. Cliquer sur **[!UICONTROL Enregistrer]**.

<!--

## Set up the group of items in Preview

You can choose how you want the group of items to display on your calendar.

{{step1-to-calendars}}

1. Select the calendar you want to add a new group of items to.
   Or
   Click **[!UICONTROL + New Calendar]** and enter the calendar name.

   >[!NOTE]
   >
   >You must have Edit access to Reports, Dashboards, and Calendars in your access level to create a calendar report.

1. On the left, click **[!UICONTROL Add to Calendar]**, then click **[!UICONTROL Add advanced items]**.

1. Specify the following:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Name this group of items]</strong></td>
      <td>Type a name for the group of items.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Color]</strong></td>
      <td>Select a color for the group of items. All items display in the selected color on the calendar report.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Date Field]</strong></td>
      <td><p>Choose <strong>[!UICONTROL Planned dates]</strong>. For more information on planned dates, see </p>
       <ul>
        <li><a href="../../../manage-work/projects/planning-a-project/project-planned-start-date.md" class="MCXref xref">Overview of the project Planned Start Date</a></li>
        <li><a href="../../../manage-work/tasks/task-information/task-planned-start-date.md" class="MCXref xref">Overview of the task Planned Start Date</a></li>
        <li><a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Overview of the task Planned Completion Date</a></li>
        <li><a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">Set the project Planned Completion Date</a><br></li>
       </ul></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>On the calendar, show</strong></td>
      <td><p>Choose how you want the dates to show:</p>
       <ul>
        <li><strong>[!UICONTROL Start Date Only]</strong>: The calendar displays the object on a single date.</li>
        <li><strong>[!UICONTROL End Date Only]</strong>: The calendar displays the object on a single date.</li>
        <li><strong>[!UICONTROL Duration] (Start to End)</strong>: The calendar displays the object over a span of days.</li>
       </ul></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader"><strong>[!UICONTROL Switch to actual dates when available]</strong></td>
      <td><p>The calendar automatically switches to actual dates when they are available. <br>Choose <strong>[!UICONTROL Yes]</strong> or <strong>[!UICONTROL No]</strong> to switch to actual dates when available. For more information on Actual Dates, see</p>
       <ul>
        <li><a href="../../../manage-work/projects/planning-a-project/project-actual-start-date.md" class="MCXref xref">Overview of the project Actual Start Date </a></li>
        <li><a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref">Overview of the project Actual Completion Date </a></li>
       </ul></td>
     </tr>
    </tbody>
   </table>

1. Continue to the following section.

## Add objects to the group of items in Preview

After you set up how you want items to display, you need to add the objects you want to see on the calendar to the grouping.

1. In the **[!UICONTROL What would you like to add to the calendar?]** section, select

   * **[!UICONTROL Tasks]**
   * **[!UICONTROL Projects]**
   * **[!UICONTROL Issues]**

1. Click **[!UICONTROL Add Tasks]**, **[!UICONTROL Add Projects]**, or **[!UICONTROL Add Issues]**, depending on the object type you are adding to the calendar.
   ![Select object for calendar](assets/field-name.png)

1. In the drop-down menu, begin typing the field name, then select the field source of the object you want to display on the calendar (for example, **[!UICONTROL Late Tasks]**).
1. Set a condition statement for the calendar grouping.

   ![Condition statement](assets/condition-statement-calendar.png)

   To learn about setting conditions, see [Filter and condition modifiers](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. (Optional) Specify additional objects for the calendar grouping by repeating Steps 1-4.
1. In the **[!UICONTROL Set the Tasks/Projects/Issues labels to be the...]** field, select how the objects in this calendar grouping are labeled in the calendar.

   >[!NOTE]
   >
   >If the default label options are not available for a certain object, the object name is shown instead. For example, when the [!UICONTROL Parent Task] label is selected and there is no parent task associated with the object, [!DNL Adobe Workfront] displays the object name you are viewing in the calendar.

1. Click **[!UICONTROL Save]**. 

-->