---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: Utilisation de dates prévues dans un rapport de calendrier
description: Un rapport de calendrier est un rapport dynamique qui fournit une représentation visuelle de votre travail. Vous pouvez utiliser les champs Date projetées dans un rapport de calendrier pour les tâches, les problèmes et les projets.
author: Lisa
feature: Reports and Dashboards
exl-id: 39e16f0b-c10d-429e-9eb5-d4847c7e4ed9
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '605'
ht-degree: 88%

---

# Utiliser les [!UICONTROL dates projetées] dans un rapport de calendrier

Un rapport de calendrier est un rapport dynamique qui fournit une représentation visuelle de votre travail. Vous pouvez utiliser les champs Date projetée dans un rapport de calendrier pour les objets suivants :

* Tâches
* Problèmes
* Projets

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès aux rapports, tableaux de bord et calendriers</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td>Gérer l’accès au rapport de calendrier</td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurer le groupe d’éléments

Vous pouvez choisir la manière dont le groupe d’éléments doit s’afficher sur votre calendrier.

{{step1-to-calendars}}

1. Sélectionnez le calendrier dans lequel vous souhaitez ajouter un nouveau groupe d&#39;éléments, cliquez sur le menu Plus, puis sur **Modifier**.
Ou
Cliquez sur **[!UICONTROL + Nouveau calendrier]** saisissez le nom du projet, puis cliquez sur **[!UICONTROL Ajouter des éléments avancés]**.

   >[!NOTE]
   >
   >Vous devez avoir un accès en [!UICONTROL modification] à [!UICONTROL Rapports], [!UICONTROL Tableaux de bord], et [!UICONTROL Calendriers] dans votre niveau d’accès pour créer un rapport de calendrier.

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
      <td><p>Choisissez <strong>[!UICONTROL Projected dates]</strong>. Pour plus d’informations sur les dates projetées, voir </p>
       <ul>
        <li><a href="../../../manage-work/projects/planning-a-project/project-projected-start-date.md" class="MCXref xref">Vue d’ensemble de la Date de début prévisionnelle du projet</a></li>
        <li><a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">Vue d’ensemble de la date d’achèvement prévue pour les projets, les tâches et les problèmes</a><br></li>
       </ul></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL On the calendar, show]</strong></td>
      <td><p>Choisissez le mode d’affichage des dates :</p>
       <ul>
        <li><strong>[!UICONTROL Start Date Only]</strong> : le calendrier affiche l’objet à une seule date.</li>
        <li><strong>[!UICONTROL End Date Only]</strong> : le calendrier affiche l’objet à une seule date.</li>
        <li><strong>[!UICONTROL Duration] (du début à la fin)</strong> : le calendrier affiche l’objet sur plusieurs jours.</li>
       </ul></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader"><strong>[!UICONTROL Switch to Actual Dates when available]</strong></td>
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
   * **[!UICONTROL Congés]**
1. Cliquez sur **[!UICONTROL Ajouter des tâches]**, **[!UICONTROL Ajouter des projets]** ou **[!UICONTROL Ajouter des problèmes]**, selon le type d’objet que vous ajoutez au calendrier.

1. Dans le menu déroulant, commencez à saisir le nom du champ, puis sélectionnez la source du champ de l’objet que vous souhaitez afficher sur le calendrier (par exemple, **[!UICONTROL Tâches en retard]**).
1. Définissez une condition pour le regroupement de calendrier.


   ![Sélectionner un objet pour le calendrier](assets/calendar-field-name.png)
Pour en savoir plus sur la définition de conditions, voir [Modificateurs de filtre et de condition](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. (Facultatif) Spécifiez des objets supplémentaires pour le groupe de calendriers en répétant les étapes 1 à 4.
1. Dans le champ **[!UICONTROL Définissez les libellés des Tâches/Projets/Problèmes sur ...]**, sélectionnez le libellé des objets de ce regroupement de calendrier.

   >[!NOTE]
   >
   >Si les options relatives aux libellés par défaut ne sont pas disponibles pour un objet donné, le nom de l’objet est affiché à la place. Par exemple, lorsque le libellé [!UICONTROL Tâche parent] est sélectionné et qu’aucune tâche parent n’est associée à l’objet, [!DNL Adobe Workfront] affiche le nom de l’objet affiché dans le calendrier.

   ![définir les libellés de la tâche](assets/set-task-labels.png)

1. Cliquer sur **[!UICONTROL Enregistrer]**.

