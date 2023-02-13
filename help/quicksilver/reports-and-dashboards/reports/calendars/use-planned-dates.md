---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: Utilisation des dates planifiées dans un rapport de calendrier
description: Un rapport Calendrier est un rapport dynamique qui fournit une représentation visuelle de votre travail. Vous pouvez utiliser les champs Date planifiée dans un rapport de calendrier pour les tâches, les problèmes et les projets.
author: Lisa
feature: Reports and Dashboards
exl-id: 27bf6f03-2f6b-4556-a715-75c4a21bfbbb
source-git-commit: e5a3024b1657942cd7abdfff76a7a6795127a4f5
workflow-type: tm+mt
source-wordcount: '661'
ht-degree: 2%

---

# Utilisation [!UICONTROL Dates planifiées] dans un rapport calendaire

Un rapport Calendrier est un rapport dynamique qui fournit une représentation visuelle de votre travail. Vous pouvez utiliser [!UICONTROL Date planifiée] dans un rapport de calendrier pour les objets suivants :

* Tâches
* Événements
* Projets

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

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
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Paramétrages du niveau d'accès*</strong></td> 
   <td> <p>Accès à [!UICONTROL Modifier] aux [!UICONTROL Rapports], aux [!UICONTROL Tableaux de bord] et aux [!UICONTROL Calendriers]</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre [!DNL Workfront] s’ils définissent des restrictions supplémentaires au niveau de votre accès. Pour plus d’informations sur la manière dont une [!DNL Workfront] l’administrateur peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet</strong></td> 
   <td> <p>[!UICONTROL Gérer] accès au rapport Calendrier</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

## Configurer le groupe d’éléments

Vous pouvez choisir le mode d’affichage du groupe d’éléments dans votre calendrier.

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront], puis cliquez sur **[!UICONTROL Calendriers]**.

1. Sélectionnez le calendrier auquel vous souhaitez ajouter un nouveau groupe d’éléments.\
   Ou\
   Cliquez sur **[!UICONTROL + Nouveau calendrier]** et saisissez le nom du calendrier.

   >[!NOTE]
   >
   >Pour créer un rapport de calendrier, vous devez disposer des droits d’édition sur les rapports, les tableaux de bord et les calendriers de votre niveau d’accès.

1. Sur la gauche, cliquez sur **[!UICONTROL Ajouter au calendrier]**, puis cliquez sur **[!UICONTROL Ajout d’éléments avancés]**.

1. Indiquez les informations suivantes :

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Nommer ce groupe d’éléments]</strong></td>
      <td>Saisissez le nom du groupe d’éléments.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Color]</strong></td>
      <td>Sélectionnez une couleur pour le groupe d’éléments. Tous les éléments s’affichent dans la couleur sélectionnée sur le rapport du calendrier.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Champ de date]</strong></td>
      <td><p>Choisir <strong>[!UICONTROL Dates planifiées]</strong>. Pour plus d’informations sur les dates planifiées, voir </p>
       <ul>
        <li><a href="../../../manage-work/projects/planning-a-project/project-planned-start-date.md" class="MCXref xref">Présentation du projet Date de début prévue</a></li>
        <li><a href="../../../manage-work/tasks/task-information/task-planned-start-date.md" class="MCXref xref">Présentation de la tâche Date de début planifiée</a></li>
        <li><a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Présentation de la date d’achèvement planifiée de la tâche</a></li>
        <li><a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">Définition de la date d’achèvement prévue du projet</a><br></li>
       </ul></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Sur le calendrier, afficher</strong></td>
      <td><p>Choisissez le mode d’affichage des dates :</p>
       <ul>
        <li><strong>[!UICONTROL Date De Démarrage Uniquement]</strong>: Le calendrier affiche l’objet à une seule date.</li>
        <li><strong>[!UICONTROL Date De Fin Uniquement]</strong>: Le calendrier affiche l’objet à une seule date.</li>
        <li><strong>[!UICONTROL Durée] (du début à la fin)</strong>: Le calendrier affiche l’objet sur une période de plusieurs jours.</li>
       </ul></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader"><strong>[!UICONTROL Basculer vers des dates réelles lorsqu’elles sont disponibles]</strong></td>
      <td><p>Le calendrier passe automatiquement aux dates réelles lorsqu’elles sont disponibles. <br>Choisir <strong>[!UICONTROL Oui]</strong> ou <strong>[!UICONTROL No]</strong> pour passer aux dates réelles lorsque cela est possible. Pour plus d’informations sur les dates réelles, voir</p>
       <ul>
        <li><a href="../../../manage-work/projects/planning-a-project/project-actual-start-date.md" class="MCXref xref">Présentation de la date de début réelle du projet </a></li>
        <li><a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref">Présentation du projet Date d’achèvement réelle </a></li>
       </ul></td>
     </tr>
    </tbody>
   </table>

1. Passez à la section suivante.

## Ajouter des objets au groupe d’éléments

Une fois que vous avez configuré l’affichage des éléments, vous devez ajouter au regroupement les objets que vous souhaitez voir sur le calendrier.

1. Dans le **[!UICONTROL Que souhaitez-vous ajouter au calendrier ?]** , sélectionnez

   * **[!UICONTROL Tâches]**
   * **[!UICONTROL Projets]**
   * **[!UICONTROL Événements]**

1. Cliquez sur **[!UICONTROL Ajout de tâches]**, **[!UICONTROL Ajouter des projets]** ou **[!UICONTROL Ajout de problèmes]**, selon le type d’objet que vous ajoutez au calendrier.\
   ![Sélectionner un objet pour le calendrier](assets/field-name.png)

1. Dans le menu déroulant, commencez à saisir le nom du champ, puis sélectionnez la source du champ de l’objet que vous souhaitez afficher dans le calendrier (par exemple, **[!UICONTROL Tâches en retard]**).
1. Définissez une instruction de condition pour le regroupement de calendrier.

   ![Instruction de condition](assets/condition-statement-calendar.png)

   Pour en savoir plus sur la définition de conditions, voir [Modificateurs de filtre et de condition](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. (Facultatif) Spécifiez des objets supplémentaires pour le regroupement de calendrier en répétant les étapes 1 à 4.
1. Dans le **[!UICONTROL Définissez les étiquettes Tâches/Projets/Problèmes sur ...]** , sélectionnez le libellé des objets de ce groupe de calendrier.

   >[!NOTE]
   >
   >Si les options d’étiquette par défaut ne sont pas disponibles pour un certain objet, le nom de l’objet s’affiche à la place. Par exemple, lorsque la variable [!UICONTROL Tâche parente] le libellé est sélectionné et aucune tâche parent n&#39;est associée à l&#39;objet, [!DNL Adobe Workfront] affiche le nom de l’objet que vous affichez dans le calendrier.

1. Cliquer sur **[!UICONTROL Enregistrer]**.
