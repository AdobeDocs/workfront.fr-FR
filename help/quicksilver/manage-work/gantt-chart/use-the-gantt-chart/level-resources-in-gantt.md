---
product-area: resource-management
navigation-topic: use-the-gantt-chart
title: Ressources de niveau dans  [!UICONTROL Graphique Gantt]
description: Informations sur la manière de mettre les ressources à niveau dans le diagramme de Gantt.
author: Alina
feature: Work Management
exl-id: ba96c01d-03b8-4728-b5e3-b10d227f51b0
source-git-commit: 980e6c2cea2ceb98abda6b98811e734d895ad274
workflow-type: tm+mt
source-wordcount: '592'
ht-degree: 0%

---

# Ressources de niveau dans [!UICONTROL Graphique Gantt]

L’nivellement de vos ressources sur un projet a deux objectifs :

* Pour ajuster automatiquement la sur-affectation du temps pour les personnes désignées.
* Pour créer automatiquement un planning de tâches réaliste pour un projet.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Quelconque </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Accès à [!UICONTROL Modifier] dans Projets</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès à , demandez à votre [!DNL Workfront] s’ils définissent des restrictions supplémentaires au niveau de votre accès. Pour plus d’informations sur la manière dont une [!DNL Workfront] l’administrateur peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Accès à [!UICONTROL Gérer] au projet</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

## Présentation du niveau des ressources

Si la même ressource est affectée à deux tâches différentes, vous pouvez utiliser le niveau de ressource pour ajuster la chronologie des tâches afin qu’elles ne se produisent pas en même temps.

Tenez compte des points suivants lors de l’nivellement des ressources sur un projet :

* Le niveau de ressource s’applique uniquement à un projet. [!DNL Adobe Workfront] ne met pas à niveau les ressources sur plusieurs projets à la fois.
* If **[!UICONTROL Effort piloté]** est sélectionné en tant que **[!UICONTROL Type de durée]**, [!DNL Workfront] ne met pas les ressources à niveau.
* Lorsque plusieurs utilisateurs sont affectés à la même tâche, le niveau est annulé.
* Conditions du type de **[!UICONTROL Contrainte de tâche]** prévaudra sur le niveau des ressources. Par exemple, si **[!UICONTROL Dates fixes]** est sélectionné en tant que [!UICONTROL Contrainte de tâche], le niveau de ressource ne modifie pas les dates de la tâche.
* Les relations avec les prédécesseurs auront la priorité sur le niveau des ressources.
* **[!UICONTROL Niveau des ressources]** doit être défini sur **[!UICONTROL Manuel]** pour le projet afin d’ajuster le niveau dans la variable [!UICONTROL Graphique Gantt]. Si vous disposez des autorisations de gestion du projet, vous pouvez configurer le système de niveau automatique des ressources en ajustant ce paramètre sur le projet et en sélectionnant **[!UICONTROL Automatique]** au lieu de **[!UICONTROL Manuel]** dans le **[!UICONTROL Modifier le projet]** de la boîte.

  ![](assets/resource-leveling-mode-350x177.png)

* En tant que propriétaire du projet, ou responsable de la tâche, vous pouvez introduire un délai de mise à niveau pour une tâche afin d’indiquer qu’il y a de grandes chances que la tâche puisse nécessiter un temps supplémentaire. Pour plus d’informations sur l’ajout d’un délai de niveau à une tâche, voir [Mettre à jour le délai de niveau de tâche](../../../manage-work/tasks/task-information/task-leveling-delay.md).

## Appliquez le niveau de ressource dans le [!UICONTROL Graphique Gantt]

Vous pouvez utiliser la liste des tâches [!UICONTROL Graphique Gantt] pour mettre vos ressources à niveau.

1. Accédez au projet que vous souhaitez mettre à niveau.
1. Dans le **[!UICONTROL Tâche]** , cliquez sur la zone **[!UICONTROL Graphique Gantt]** Icône

   Toutes les modifications sont automatiquement enregistrées lorsque la variable **[!UICONTROL Enregistrement automatique]** est activée. Elle est activée par défaut.

1. (Facultatif) Cliquez sur le **[!UICONTROL Planifier] mode** et sélectionnez **[!UICONTROL Enregistrement manuel standard]** ou **[!UICONTROL Planification chronologique]** pour enregistrer vos modifications manuellement.

   >[!TIP]
   >
   >Vous ne pouvez pas mettre à niveau les ressources dans la variable  [!UICONTROL Graphique Gantt] lorsque la variable [!UICONTROL Enregistrement automatique] est activée.

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. Cliquez sur le bouton **[!UICONTROL Ressources de niveau]** menu déroulant.

   ![Level_resources.png](assets/level-resouces.png)

1. Sélectionnez l’une des options suivantes :

   * **[!UICONTROL Niveau maintenant]**: applique un niveau de ressource à la tâche sélectionnée.
   * **[!UICONTROL Effacer le niveau]**: supprime tous les niveaux de ressource de la tâche sélectionnée.

   >[!NOTE]
   >
   >Vos ressources peuvent être surchargées si elles sont affectées à plusieurs tâches qui se produisent pendant la même période.

1. (Facultatif et conditionnel) Si vous avez désactivé l’option d’enregistrement automatique, cliquez sur le bouton **[!UICONTROL Annuler]** ou &#x200B;**[!UICONTROL Rétablir]** si vous souhaitez annuler ou dupliquer l’une des modifications.

   >[!TIP]
   >
   >Vous pouvez utiliser les raccourcis clavier suivants pour annuler ou rétablir des modifications sur le [!UICONTROL Graphique Gantt]:
   >
   >* [!DNL Mac]: utilisez [!UICONTROL Commande + Z] pour annuler et [!UICONTROL Commande + Maj + Z] pour rétablir.
   >* Windows : utilisez [!UICONTROL Ctrl + Z] pour annuler et [!UICONTROL Ctrl + Y] pour rétablir.


1. Cliquez sur **[!UICONTROL Enregistrer]** dans le coin supérieur droit du [!UICONTROL Graphique Gantt].

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Overview of Leveling Delay</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: moved to its own article: /Content/Manage work/Tasks/Task information/task-leveling-delay.htm) </p>
<p>At times, there might be conflicts between task schedules on a project. You can level resources or address resource conflicts by rescheduling resources and tasks so that all tasks can be completed within a realistic schedule. </p>
<p>As the project manager, or the task assignee, you can also add a Leveling Delay on individual tasks to account for any resource or scheduling conflicts. In other words, a task might be scheduled with a delay to ensure that when Adobe Workfront levels the tasks a more realistic schedule overcomes resource conflicts.</p>
<p>To manually add a Leveling Delay to a task:</p>
<ol>
<li value="1">Navigate to a task for which you want to add a Leveling Delay.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click the <strong>More icon</strong> to the right of the task name, then click <strong>Edit</strong>. </p>  </li>
<li value="3">Click <strong>Settings</strong>.<br></li>
<li value="4">Specify the <strong>Leveling Delay</strong>, in hours.<br>This is the time that the resource will be delayed starting the task due to resource conflicts.</li>
<li value="5">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->
