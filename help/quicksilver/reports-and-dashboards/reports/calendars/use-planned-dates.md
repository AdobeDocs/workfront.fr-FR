---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: Utiliser les dates prévues dans un rapport de calendrier
description: Un rapport de calendrier est un rapport dynamique qui fournit une représentation visuelle de votre travail. Vous pouvez utiliser les champs Date prévue dans un rapport de calendrier pour les tâches, les problèmes et les projets.
author: Lisa
feature: Reports and Dashboards
exl-id: 27bf6f03-2f6b-4556-a715-75c4a21bfbbb
source-git-commit: e5a3024b1657942cd7abdfff76a7a6795127a4f5
workflow-type: tm+mt
source-wordcount: '663'
ht-degree: 100%

---

# Utiliser [!UICONTROL Dates prévues] dans un rapport de calendrier

Un rapport de calendrier est un rapport dynamique qui fournit une représentation visuelle de votre travail. Vous pouvez afficher les champs [!UICONTROL Date prévue] dans un rapport de calendrier pour les objets suivants :

* Tâches
* Problèmes
* Projets

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
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurations du niveau d’accès*</strong></td> 
   <td> <p>[!UICONTROL Edit] l’accès aux [!UICONTROL Reports], aux [!UICONTROL Dashboards] et aux [!UICONTROL Calendars]</p> <p>Remarque : si vous n’avez toujours pas accès, demandez à votre administrateur ou à votre administratrice [!DNL Workfront] si des restrictions supplémentaires ont été définies pour votre niveau d’accès. Pour plus d’informations sur la manière dont l’administration [!DNL Workfront] peut modifier votre niveau d’accès, consultez la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet</strong></td> 
   <td> <p>[!UICONTROL Manage] l’accès au rapport de calendrier</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice [!DNL Workfront].

## Configurer le groupe d’éléments

Vous pouvez choisir la manière dont le groupe d’éléments doit s’afficher sur votre calendrier.

1. Cliquez sur l’icône **[!UICONTROL Menu Principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront], puis cliquez sur **[!UICONTROL Calendriers]**.

1. Sélectionnez le calendrier auquel vous souhaitez ajouter un nouveau groupe d’éléments.\
   Ou\
   Cliquez sur **[!UICONTROL + Nouveau calendrier]** et saisissez le nom du calendrier.

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

## Ajouter des objets au groupe d’éléments

Après avoir défini le mode d’affichage des éléments, vous devez ajouter au regroupement les objets que vous souhaitez voir apparaître sur le calendrier.

1. Dans la section **[!UICONTROL Que souhaitez-vous ajouter au calendrier ?]**, sélectionnez

   * **[!UICONTROL Tâches]**
   * **[!UICONTROL Projets]**
   * **[!UICONTROL Événements]**

1. Cliquez sur **[!UICONTROL Ajouter des tâches]**, **[!UICONTROL Ajouter des projets]** ou **[!UICONTROL Ajouter des problèmes]**, selon le type d’objet que vous ajoutez au calendrier.\
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
