---
product-area: resource-management
navigation-topic: use-the-gantt-chart
title: Niveler les ressources dans le [!UICONTROL Diagramme de Gantt]
description: Si la même ressource est affectée à deux tâches différentes, vous pouvez utiliser l'audit des ressources pour ajuster la chronologie des tâches afin qu'elles ne se produisent pas en même temps. Cet article fournit des informations sur la façon d'niveler des ressources dans le graphique Gantt.
author: Alina
feature: Work Management
exl-id: ba96c01d-03b8-4728-b5e3-b10d227f51b0
source-git-commit: c8987d036e1c1324618cb53ebcbb8fd7e4bcc6a4
workflow-type: tm+mt
source-wordcount: '620'
ht-degree: 81%

---

# Niveler les ressources dans le [!UICONTROL Diagramme de Gantt]

<!--Audited: 08/2025-->

Vous pouvez utiliser l&#39;audit des ressources pour ajuster la chronologie des tâches afin qu&#39;elles ne se produisent pas en même temps, au cas où les mêmes ressources seraient affectées à plusieurs tâches en même temps.

Le nivellement de vos ressources sur un projet a deux buts :

* Ajuster automatiquement l’affectation excessive de temps pour les cessionnaires.
* Créer automatiquement un planning des tâches réaliste pour un projet.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] paquet</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Workfront] licence</td> 
   <td> <p>[!UICONTROL Standard]</p>
   <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>[!UICONTROL Edit] l’accès aux Projets</p></td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>[!UICONTROL Manage] l’accès au projet</p>
</td> 
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
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>[!UICONTROL Edit] access to Projects</p> <p><b>NOTE</b>

If you still don't have access, ask your [!DNL Workfront] administrator if they set additional restrictions in your access level. For information on how a [!DNL Workfront] administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[!UICONTROL Manage] access to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table> -->

## Vue d’ensemble du nivellement des ressources

Si la même ressource est affectée à deux tâches différentes, vous pouvez utiliser le nivellement des ressources pour ajuster la chronologie des tâches afin qu’elles ne se déroulent pas en même temps.

Tenez compte des points suivants lors du nivellement des ressources sur un projet :

* Le nivellement des ressources s’applique uniquement à un seul projet. [!DNL Adobe Workfront] ne nivelle pas les ressources dans plusieurs projets à la fois.
* Si le **[!UICONTROL Type de durée]** sélectionné est **[!UICONTROL Piloté par l’effort]**, [!DNL Workfront] ne nivelle par les ressources.
* Lorsque plusieurs utilisateurs et utilisatrices sont affectés à la même tâche, le nivellement est annulé.
* Les conditions du type de **[!UICONTROL Contrainte de tâche]** ont la priorité sur le nivellement des ressources. Par exemple, si la [!UICONTROL Contrainte de tâche] sélectionnée est **[!UICONTROL Dates fixes]**, le nivellement des ressources ne modifie pas les dates de la tâche.
* Les relations d’antériorité ont la priorité sur le nivellement des ressources.
* Le **[!UICONTROL nivellement des ressources]** doit être défini sur **[!UICONTROL Manuel]** pour le projet afin d’ajuster le nivellement dans le [!UICONTROL Diagramme de Gantt]. Si vous disposez des autorisations de gestion pour le projet, le système peut niveler automatiquement les ressources si vous réglez le paramètre dans le projet et si vous sélectionnez **[!UICONTROL Automatique]** au lieu de **[!UICONTROL Manuel]** dans la zone **[!UICONTROL Modifier le projet]**.

  ![Mode de nivellement des ressources](assets/resource-leveling-mode-350x177.png)

* En tant que personne propriétaire du projet ou personne affectée à une tâche, vous pouvez définir un délai de nivellement pour une tâche afin d’indiquer qu’il est très probable que la tâche nécessite du temps supplémentaire. Pour plus d’informations sur l’ajout d’un délai de nivellement à une tâche, consultez [Mettre à jour le délai de nivellement d’une tâche](../../../manage-work/tasks/task-information/task-leveling-delay.md).

## Appliquer un nivellement des ressources au [!UICONTROL Diagramme de Gantt]

Vous pouvez utiliser le [!UICONTROL Diagramme de Gantt] de la liste des tâches pour niveler vos ressources.

1. Accédez au projet que vous souhaitez niveler.
1. Dans la zone **[!UICONTROL Tâches]**, cliquez sur l’icône **[!UICONTROL Diagramme de Gantt]**.

   Toutes les modifications sont automatiquement enregistrées lorsque l’option **[!UICONTROL Enregistrement automatique]** est activée. Elle est activée par défaut.

1. (Facultatif) Cliquez sur l’icône **[!UICONTROL Mode de] planification** et sélectionnez **[!UICONTROL Enregistrement manuel standard]** ou **[!UICONTROL Planification chronologique]** pour enregistrer vos modifications manuellement.

   >[!TIP]
   >
   >Vous ne pouvez pas niveler les ressources dans le [!UICONTROL Diagramme de Gantt] lorsque l’option [!UICONTROL Enregistrement automatique] est activée.

   ![Paramètre manuel activé](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. Cliquez sur le menu déroulant **[!UICONTROL Niveler les ressources]**.

   ![Level_resouces.png](assets/level-resouces.png)

1. Sélectionnez l’une des options suivantes :

   * **[!UICONTROL Niveler]** : applique un nivellement des ressources à la tâche sélectionnée.
   * **[!UICONTROL Effacer le nivellement]** : supprime tous les nivellements de ressources de la tâche sélectionnée.

   >[!NOTE]
   >
   >Vos ressources peuvent être surchargées si elles sont affectées à plusieurs tâches qui se produisent au cours de la même période.

1. (Facultatif et conditionnel) Si vous avez désactivé l’option Enregistrement automatique, cliquez sur les icônes **[!UICONTROL Annuler]** ou **[!UICONTROL Rétablir]** si vous souhaitez annuler ou dupliquer l’une des modifications.

   >[!TIP]
   >
   >Vous pouvez utiliser les raccourcis clavier suivants pour annuler ou rétablir des modifications du [!UICONTROL Diagramme de Gantt] :
   >
   >* [!DNL Mac] : utilisez [!UICONTROL Commande+Z] pour annuler et [!UICONTROL Commande+Maj+Z] pour rétablir.
   >* Windows : utilisez [!UICONTROL Ctrl+Z] pour annuler et [!UICONTROL Ctrl+Y] pour rétablir.


1. Cliquez sur **[!UICONTROL Enregistrer]** dans le coin supérieur droit du [!UICONTROL Diagramme de Gantt].

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
