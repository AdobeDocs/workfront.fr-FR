---
product-area: resource-management
navigation-topic: use-the-gantt-chart
title: Ressources de niveau dans le [!UICONTROL diagramme de Gantt]
description: Informations sur la manière de mettre les ressources à niveau dans le diagramme de Gantt.
author: Alina
feature: Work Management
exl-id: ba96c01d-03b8-4728-b5e3-b10d227f51b0
source-git-commit: 980e6c2cea2ceb98abda6b98811e734d895ad274
workflow-type: tm+mt
source-wordcount: '592'
ht-degree: 15%

---

# Ressources de niveau dans le [!UICONTROL diagramme de Gantt]

L’nivellement de vos ressources sur un projet a deux objectifs :

* Pour ajuster automatiquement la sur-affectation du temps pour les personnes désignées.
* Pour créer automatiquement un planning de tâches réaliste pour un projet.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] forfait*</td> 
   <td> <p>N’importe quelle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Workfront] licence*</td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Accès à [!UICONTROL Modifier] dans Projets</p> <p><b>NOTE</b>

Si vous ne disposez toujours pas d’un accès, demandez à votre équipe d’administration [!DNL Workfront] si elle a défini des restrictions supplémentaires pour votre niveau d’accès. Pour plus d’informations sur la manière dont un administrateur ou une administratrice [!DNL Workfront] peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Accès à [!UICONTROL Gérer] au projet</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice [!DNL Workfront].

## Présentation du niveau des ressources

Si la même ressource est affectée à deux tâches différentes, vous pouvez utiliser le niveau de ressource pour ajuster la chronologie des tâches afin qu’elles ne se produisent pas en même temps.

Tenez compte des points suivants lors de l’nivellement des ressources sur un projet :

* Le niveau de ressource s’applique uniquement à un projet. Par conséquent, [!DNL Adobe Workfront] ne met pas à niveau les ressources sur plusieurs projets à la fois.
* Si **[!UICONTROL Effort Driven]** est sélectionné en tant que **[!UICONTROL Type de durée]**, [!DNL Workfront] ne met pas les ressources à niveau.
* Lorsque plusieurs utilisateurs sont affectés à la même tâche, le niveau est annulé.
* Les conditions du type **[!UICONTROL Contrainte de tâche]** ont la priorité sur le niveau des ressources. Par exemple, si l’option **[!UICONTROL Dates fixes]** est sélectionnée en tant que [!UICONTROL Contrainte de tâche], le niveau de ressource ne modifie pas les dates de la tâche.
* Les relations avec les prédécesseurs auront la priorité sur le niveau des ressources.
* **[!UICONTROL Resource Level]** doit être défini sur **[!UICONTROL Manuel]** pour le projet afin d’ajuster le niveau dans le [!UICONTROL diagramme de Gantt]. Si vous disposez des autorisations de gestion du projet, vous pouvez configurer le système pour qu’il mette automatiquement au niveau les ressources en ajustant ce paramètre sur le projet et en sélectionnant **[!UICONTROL Automatique]** au lieu de **[!UICONTROL Manuel]** dans la zone **[!UICONTROL Modifier le projet]**.

  ![](assets/resource-leveling-mode-350x177.png)

* En tant que propriétaire du projet, ou responsable de la tâche, vous pouvez introduire un délai de mise à niveau pour une tâche afin d’indiquer qu’il y a de grandes chances que la tâche puisse nécessiter un temps supplémentaire. Pour plus d’informations sur l’ajout d’un délai de mise à niveau à une tâche, voir [Mise à jour du délai de mise à niveau de la tâche](../../../manage-work/tasks/task-information/task-leveling-delay.md).

## Appliquer un niveau de ressource dans le [!UICONTROL diagramme de Gantt]

Vous pouvez utiliser le [!UICONTROL diagramme de Gantt] de la liste des tâches pour mettre à niveau vos ressources.

1. Accédez au projet que vous souhaitez mettre à niveau.
1. Dans la zone **[!UICONTROL Tâches]**, cliquez sur l&#39;icône **[!UICONTROL Graphique de Gantt]** .

   Toutes les modifications sont enregistrées automatiquement lorsque l’option **[!UICONTROL Enregistrement automatique]** est activée. Cette option est activée par défaut.

1. (Facultatif) Cliquez sur l’icône **[!UICONTROL Plan] mode** et sélectionnez **[!UICONTROL Enregistrement manuel standard]** ou **[!UICONTROL Planification de la chronologie]** pour enregistrer vos modifications manuellement.

   >[!TIP]
   >
   >Vous ne pouvez pas mettre à niveau les ressources dans le [!UICONTROL diagramme de Gantt] lorsque l’option [!UICONTROL Enregistrement automatique] est activée.

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. Cliquez sur le menu déroulant **[!UICONTROL Level Resources]** .

   ![Level_resources.png](assets/level-resouces.png)

1. Sélectionnez l’une des options suivantes :

   * **[!UICONTROL Level Now]** : applique le niveau de ressource à la tâche sélectionnée.
   * **[!UICONTROL Effacer le niveau]** : supprime tous les niveaux de ressources de la tâche sélectionnée.

   >[!NOTE]
   >
   >Vos ressources peuvent être surchargées si elles sont affectées à plusieurs tâches qui se produisent pendant la même période.

1. (Facultatif et conditionnel) Si vous avez désactivé l’option d’enregistrement automatique, cliquez sur les icônes **[!UICONTROL Annuler]** ou &#x200B;**[!UICONTROL Rétablir]** si vous souhaitez annuler ou dupliquer l’une des modifications.

   >[!TIP]
   >
   >Vous pouvez utiliser les raccourcis clavier suivants pour annuler ou rétablir des modifications sur le [!UICONTROL diagramme de Gantt] :
   >
   >* [!DNL Mac] : utilisez [!UICONTROL Commande + Z] pour annuler et [!UICONTROL Commande + Maj + Z] pour rétablir.
   >* Windows : utilisez [!UICONTROL Ctrl + Z] pour annuler et [!UICONTROL Ctrl + Y] pour rétablir.


1. Cliquez sur **[!UICONTROL Enregistrer]** dans le coin supérieur droit du [!UICONTROL diagramme de Gantt].

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
