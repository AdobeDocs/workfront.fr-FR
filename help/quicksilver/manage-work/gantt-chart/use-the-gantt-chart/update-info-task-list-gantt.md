---
product-area: projects
navigation-topic: use-the-gantt-chart
title: Mise à jour des informations dans le diagramme de Gantt de la liste des tâches
description: Le diagramme de Gantt de la liste des tâches affiche des détails sur les tâches qui se trouvent sur un projet ou un modèle.
author: Alina
feature: Work Management
exl-id: 0a8e6fd5-985c-49e5-842d-67ade29ee1c9
source-git-commit: e2f6eada24b4e48bce58189ec16447eda89f4a09
workflow-type: tm+mt
source-wordcount: '1036'
ht-degree: 1%

---

# Mise à jour des informations dans la liste des tâches [!UICONTROL Graphique Gantt]

La liste des tâches [!UICONTROL Graphique Gantt] affiche des détails sur les tâches qui se trouvent sur un projet ou un modèle.

Dans un modèle, la liste des tâches [!UICONTROL Graphique Gantt] reflète les mises à jour effectuées dans la liste des tâches du modèle au niveau de la tâche. Vous ne pouvez pas modifier la variable [!UICONTROL Graphique Gantt] associée à un modèle.

Dans un projet, vous pouvez mettre à jour les informations de tâche directement dans la liste des tâches. [!UICONTROL Graphique Gantt].

Cet article décrit les actions suivantes que vous pouvez effectuer directement dans la liste des tâches [!UICONTROL Graphique Gantt]:

* Modification de la durée de la tâche
* Création ou suppression de relations de prédécesseur
* Modification des dates de début et de fin de la tâche
* Mettre à jour le pourcentage terminé
* Ressources de projet de niveau

## Exigences d’accès

Pour suivre les étapes de cet article, vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Tous </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Accès à [!UICONTROL Modifier] aux projets et aux tâches</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre [!DNL Workfront] s’ils définissent des restrictions supplémentaires au niveau de votre accès. Pour plus d’informations sur la manière dont une [!DNL Workfront] l’administrateur peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Accès à [!UICONTROL Gérer] au projet et aux tâches </p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

## Modification de la durée de la tâche

1. Accédez au projet que vous souhaitez modifier.
1. Cliquez sur **[!UICONTROL Tâches]** dans le panneau de gauche.

   ![](assets/qs-tasks-area-highlighted-in-the-secondary-nav-350x206.png)

1. Cliquez sur le bouton **[!UICONTROL Graphique Gantt]** icône .

   ![Cliquez sur l’icône du diagramme de Gantt](assets/click-gantt-chart-icon.png)

   Toutes les modifications sont automatiquement enregistrées lorsque la variable **[!UICONTROL Enregistrement automatique]** est activée. Elle est activée par défaut.

1. (Facultatif) Cliquez sur le **[!UICONTROL Mode Plan]** et sélectionnez **[!UICONTROL Enregistrement manuel standard]** ou **[!UICONTROL Planification de la chronologie]** pour enregistrer vos modifications manuellement.

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. Passez la souris sur la chronologie d’une tâche et faites glisser l’indicateur de chronologie vers une date différente.
1. Déposez l’indicateur lorsque vous avez atteint la nouvelle date de fin appropriée pour la tâche.
1. (Facultatif et conditionnel) Si vous avez choisi d’enregistrer manuellement vos modifications, cliquez sur le bouton **[!UICONTROL Annuler]** ou &#x200B;**[!UICONTROL Rétablir]** si vous souhaitez annuler ou dupliquer l’une des modifications.

   >[!TIP]
   >
   >Vous pouvez utiliser les raccourcis clavier suivants pour annuler ou rétablir des modifications sur le graphique Gantt :
   >
   >   
   >   
   >   * [!DNL Mac]: Utilisation [!UICONTROL Commande + Z] pour annuler et [!UICONTROL Commande + Maj + Z] pour rétablir.
   >   * [!DNL Windows]: Utilisation [!UICONTROL Ctrl + Z] pour annuler et [!UICONTROL Ctrl + Y] pour rétablir.
   >   
   >

1. Cliquez sur **[!UICONTROL Enregistrer]** dans le coin supérieur droit du [!UICONTROL Graphique Gantt].

## Créer ou supprimer des relations de prédécesseur

1. Accédez au projet que vous souhaitez modifier.
1. Dans le **[!UICONTROL Tâches]** , cliquez sur la zone **[!UICONTROL Graphique Gantt]** icône .

   Le **[!UICONTROL Enregistrement automatique]** est sélectionnée par défaut, auquel cas toutes les modifications sont enregistrées automatiquement.

   ![Cliquez sur l’icône du diagramme de Gantt](assets/click-gantt-chart-icon.png)

1. (Facultatif) Cliquez sur le **[!UICONTROL Mode Plan]** et sélectionnez **[!UICONTROL Enregistrement manuel standard]** ou **[!UICONTROL Planification de la chronologie]** pour enregistrer vos modifications manuellement.

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. Pour créer une relation de prédécesseur, cliquez sur le point de départ d’une tâche et faites-la glisser jusqu’au point de fin de la tâche.
1. Pour supprimer une relation de prédécesseur, cliquez sur une ligne de prédécesseur qui connecte deux tâches pour la sélectionner, puis appuyez sur **[!UICONTROL Supprimer]** sur votre clavier.\
   ![Delete_prédécesseur.png](assets/delete-predecessor-350x152.png)

1. (Facultatif et conditionnel) Si vous avez choisi d’enregistrer vos modifications manuellement, cliquez sur le bouton **[!UICONTROL Annuler]** ou &#x200B;**[!UICONTROL Rétablir]** si vous souhaitez annuler ou dupliquer l’une des modifications.

   >[!TIP]
   >
   >Vous pouvez utiliser les raccourcis clavier suivants pour annuler ou rétablir des modifications sur le graphique Gantt :
   >
   >   
   >   
   >   * [!DNL Mac]: Utilisation [!UICONTROL Commande + Z] pour annuler et [!UICONTROL Commande + Maj + Z] pour rétablir.
   >   * [!DNL Windows]: [!UICONTROL Utiliser Ctrl + Z] pour annuler et [!UICONTROL Ctrl + Y] pour rétablir.
   >   
   >

1. Cliquer sur **[!UICONTROL Enregistrer]** .

## Modification des dates de début et de fin de la tâche

1. Accédez au projet que vous souhaitez modifier.
1. Dans le **[!UICONTROL Tâches]** , cliquez sur la zone **[!UICONTROL Graphique Gantt]** icône .

   Toutes les modifications sont automatiquement enregistrées lorsque la variable **[!UICONTROL Enregistrement automatique]** est activée. Elle est activée par défaut.

   ![Cliquez sur l’icône du diagramme de Gantt](assets/click-gantt-chart-icon.png)

1. (Facultatif) Cliquez sur le **[!UICONTROL Mode Plan]** et sélectionnez **[!UICONTROL Enregistrement manuel standard]** ou **[!UICONTROL Planification de la chronologie]** pour enregistrer vos modifications manuellement.

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. Pointez sur le centre de la tâche et recherchez la flèche multidirectionnelle.
1. Cliquez sur la tâche et faites-la glisser jusqu’à la date de votre choix.

   ![Change_start_end_date.png](assets/change-start-end-date.png)

1. Si vous modifiez la date de la tâche d’une manière qui affecte la contrainte de tâche, cliquez sur **[!UICONTROL Accepter]** pour tenir compte du changement de contrainte de tâche.

   >[!NOTE]
   >
   >Si la tâche présente l’une des contraintes suivantes, le système met à jour la variable [!UICONTROL Contrainte de tâche] to [!UICONTROL Ne plus commencer plus tôt] Que si le projet est planifié à partir de la variable [!UICONTROL Date de début] ou [!UICONTROL Terminer au plus tard] si le projet est planifié à partir de la fonction [!UICONTROL Date d’achèvement]:
   >
   >   
   >   
   >   * [!UICONTROL Aussi Tôt Que Possible]
   >   * [!UICONTROL Aussi Tard Que Possible]
   >   * [!UICONTROL Première Heure Disponible]
   >   * [!UICONTROL Dernière Heure Disponible]
   >   
   >   
   >Dans certains cas, les relations de prédécesseur peuvent empêcher les tâches de commencer plus tôt, et le déplacement de la tâche n’est pas autorisé.

1. (Facultatif et conditionnel) Si vous avez choisi d’enregistrer vos modifications manuellement, cliquez sur le bouton **[!UICONTROL Annuler]** ou &#x200B;**[!UICONTROL Rétablir]** si vous souhaitez annuler ou dupliquer l’une des modifications.

   >[!TIP]
   >
   >Vous pouvez utiliser les raccourcis clavier suivants pour annuler ou rétablir des modifications sur le [!UICONTROL Graphique Gantt]:
   >
   >   
   >   
   >   * [!DNL Mac]: Utilisation [!UICONTROL Commande + Z] pour annuler et [!UICONTROL Commande + Maj + Z] pour rétablir.
   >   * [!DNL Windows]: Utilisation [!UICONTROL Ctrl + Z] pour annuler et [!UICONTROL Ctrl + Y] pour rétablir.
   >   
   >

1. Cliquer sur **[!UICONTROL Enregistrer]**.

## Mettre à jour le pourcentage terminé

1. Accédez au projet que vous souhaitez modifier.
1. Dans le **[!UICONTROL Tâches]** , cliquez sur la zone **[!UICONTROL Graphique Gantt]** icône .

   ![Cliquez sur l’icône du diagramme de Gantt](assets/click-gantt-chart-icon.png)

   Toutes les modifications sont automatiquement enregistrées lorsque la variable **[!UICONTROL Enregistrement automatique]** est activée. Elle est activée par défaut.

1. (Facultatif) Cliquez sur le **[!UICONTROL Mode Plan]** et sélectionnez **[!UICONTROL Enregistrement manuel standard]** ou **[!UICONTROL Planification de la chronologie]** pour enregistrer vos modifications manuellement.
1. Double-cliquez sur le nombre de pourcentage dans la tâche et saisissez le nombre.

   >[!IMPORTANT]
   >
   >Vous devez avoir [!UICONTROL % terminé] sélectionné dans le [!UICONTROL Options] afin de mettre à jour le pourcentage terminé. Pour ce faire, cliquez sur le bouton **[!UICONTROL Options]** et sélectionnez **[!UICONTROL % terminé]**.
   >
   >
   >![update_percent_complete.png](assets/update-percent-complete-350x175.png)   >
   >

1. (Facultatif et conditionnel) Si vous avez choisi d’enregistrer vos modifications manuellement, cliquez sur le bouton **[!UICONTROL Annuler]** ou &#x200B;**[!UICONTROL Rétablir]** si vous souhaitez annuler ou dupliquer l’une des modifications.

   >[!TIP]
   >
   >Vous pouvez utiliser les raccourcis clavier suivants pour annuler ou rétablir des modifications sur le [!UICONTROL Graphique Gantt]:
   >
   >   
   >   
   >   * [!DNL Mac]: Utilisation [!UICONTROL Commande + Z] pour annuler et [!UICONTROL Commande + Maj + Z] pour rétablir.
   >   * [!DNL Windows]: Utilisation [!UICONTROL Ctrl + Z] pour annuler et [!UICONTROL Ctrl + Y] pour rétablir.
   >   
   >

1. Cliquez sur **[!UICONTROL Enregistrer]** dans le coin supérieur droit du [!UICONTROL Graphique Gantt].

## Ressources de projet de niveau

Vous pouvez utiliser la liste des tâches [!UICONTROL Graphique Gantt] pour mettre vos ressources à niveau.

Pour plus d’informations sur le nivellement des ressources dans la variable [!UICONTROL Graphique Gantt], voir [Ressources de niveau dans [!UICONTROL Graphique Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/level-resources-in-gantt.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE:&nbsp;this is drafted because I moved the whole content to the article linked above)</p>
<ol>
<li value="1">Go to the project you want to level.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> In the <strong>Tasks</strong> area, click the <strong>Gantt chart</strong> icon.</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">All changes are saved automatically when the <strong>Autosave</strong> option is enabled. It is enabled by default. </p> </li>
<li value="3">
<div>
<p data-mc-conditions="QuicksilverOrClassic.Quicksilver">(Optional) Click the <strong>Plan mode</strong> icon and select <strong>Manual save Standard</strong> or <strong>Timeline Planning</strong> to save your changes manually.</p> <note type="tip">
You cannot level resources in the Gantt chart when the Autosave option is enabled.
</note>
<p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png" style="width: 350;height: 493;"> </p>
</div> </li>
<li value="4"> <p>Click the <strong>Level Resources</strong> drop-down menu.</p> <p> <img src="assets/level-resouces.png" alt="Level_resouces.png"> </p> </li>
<li value="5">Select one of following options:
<ul>
<li><strong>Level Now</strong>: Applies resource leveling to the selected task.</li>
<li><p><strong>Clear Leveling</strong>: Removes all resource leveling from the selected task.</p></li>
</ul><note type="note">
Your resources might be overallocated if they are assigned to multiple tasks which occur during the same time frame.
</note></li>
<li value="6"> <p>(Optional and conditional) If you have disabled the Autosave option, click the <strong>Undo</strong> or<strong>Redo</strong> icons if you want to cancel or duplicate any of the changes. </p> <note type="tip">
<p>You can use the following keyboard shortcuts to undo or redo changes on the Gantt chart:</p>
<ul>
<li>Mac: Use Command + Z to undo and Command + Shift + Z to redo.</li>
<li>Windows: Use Ctrl + Z to undo and Ctrl + Y to redo.</li>
</ul>
</note> </li>
<li value="7">Click <strong>Save</strong> in the upper-right corner of the Gantt chart.</li>
</ol>
</div>
-->

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode"> </h2>
-->
