---
product-area: projects
navigation-topic: manage-tasks
title: Présentation de l'enregistrement des modifications simultanées dans une liste de tâches
description: Lorsque vous modifiez des tâches dans une liste, vous pouvez utiliser des paramètres d’enregistrement distincts pour indiquer si vous souhaitez que vos modifications soient enregistrées automatiquement ou manuellement lorsque vous modifiez les tâches d’une liste.
author: Alina
feature: Work Management
exl-id: dff52425-4711-40a8-8f40-205d75c506ef
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 98%

---

# Vue d’ensemble de l’enregistrement des modifications simultanées dans une liste de tâches

Lorsque vous modifiez des tâches dans une liste, vous pouvez utiliser des paramètres d’enregistrement distincts pour indiquer si vous souhaitez que vos modifications soient enregistrées automatiquement ou manuellement lorsque vous modifiez les tâches d’une liste.

Pour plus d’informations sur la modification des tâches dans une liste de tâches, voir l’article [Modifier les tâches d’une liste](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

Parfois, des conflits peuvent apparaître si deux personnes effectuent des modifications sur les mêmes tâches.

Tenez compte des éléments suivants lorsque vous modifiez des tâches dans une liste de tâches :

* Adobe Workfront enregistre immédiatement les modifications que vous apportez aux tâches lorsque vous choisissez d’enregistrer vos modifications automatiquement si le type de mise à jour du projet est Automatique ou Automatique ou En cas de modification. Pour plus d’informations sur le type de mise à jour des projets, voir [Sélectionner le type de mise à jour du projet](../../../manage-work/projects/manage-projects/select-project-update-type.md).
* Workfront met à jour les informations de la liste sur laquelle vous travaillez toutes les minutes avec les modifications que d’autres utilisateurs et utilisatrices peuvent apporter ailleurs dans le système. Cela vous garantit de toujours disposer des informations les plus récentes sur les tâches.

Les scénarios suivants se produisent lorsque plusieurs utilisateurs et utilisatrices modifient les mêmes tâches :

* **Une personne enregistre automatiquement les modifications dans une liste de tâches et une autre le fait manuellement** : si une personne A enregistre des modifications manuellement alors que la personne B modifie les mêmes tâches mais enregistre ses modifications automatiquement, les modifications apportées par la personne B sont mises à jour dans la liste de la personne A chaque minute. En cas de conflit entre les modifications apportées par les deux personnes, celle qui enregistre manuellement (personne A) reçoit un message d’avertissement avant de pouvoir enregistrer ses modifications. Le message d’avertissement indique les éléments pour lesquels les modifications sont contradictoires. À ce moment-là, la personne A peut choisir de conserver ses modifications (ce qui remplace les modifications apportées par la personne B) ou de les rejeter (ce qui conserve les modifications apportées par la personne B).

>[!NOTE]
>
>Lorsque vous choisissez de rejeter vos modifications, cela s’applique à toutes les modifications et non pas seulement à celles qui sont en conflit avec les modifications effectuées par l’autre personne.

* **Plusieurs personnes enregistrent manuellement les modifications d’une liste de tâches** : si plusieurs personnes qui modifient les tâches d’une liste enregistrent manuellement en même temps, Workfront enregistre les modifications apportées par la personne qui enregistre en premier. L’enregistrement de ces modifications ne devrait pas entraîner de conflits. Workfront compare ensuite les modifications apportées par toutes les autres personnes avec les informations déjà enregistrées et affiche un avertissement sur les modifications conflictuelles aux autres personnes avant qu’elles puissent enregistrer leurs informations.

>[!IMPORTANT]
>
>Lorsque vous choisissez de conserver vos modifications par rapport à toutes les autres modifications, toutes vos modifications sont enregistrées, sauf si les tâches que vous avez modifiées ont été supprimées par une autre personne. Dans ce cas, le message d’avertissement vous informe que les modifications apportées aux tâches supprimées sont perdues.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
<p class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted - when replaced with the above live section; does it need an edit??) </p>
<div>
<p>When editing tasks in a list, you can select whether you want each change to be saved automatically or if you want to manually save multiple changes at one time by clicking the Save button. This depends on whether you enable the Autosave setting in the task list or not. </p>
<p>For information about editing tasks in a task list, see the article <a href="../../../manage-work/tasks/manage-tasks/edit-tasks.md" class="MCXref xref" xrefformat="{para}">Edit tasks</a>. </p>
<p>Sometimes, conflicts might appear if two users are making changes on the same tasks. </p>
<p>Consider the following when editing tasks in a task list: </p>
<ul>
<li>Workfront saves the changes you make to tasks immediately when you have enabled the Autosave setting. </li>
<li>Workfront updates the information on the list you are working on every minute with changes that other users might make anywhere else in the system. This ensures that you always get the latest information on the tasks. </li>
</ul>
<p>The following scenarios exist when multiple users are editing the same tasks:</p>
<ul>
<li>One user has Autosave disabled and another has it enabled: If a user (User A) has disabled the Autosave setting and is editing the task list while User B is editing the same tasks but they have enabled the Autosave setting, the live changes made by User B are updated on the list for User A every minute. If there are conflicts between the changes made by the two users, the user with the Autosave setting disabled (User A) sees a warning message before they can save their changes, that shows the items that have those conflicting changes. At this time, User A can choose whether they should keep their changes (which overwrites the changes made by User B), or discard them (which keeps the changes made by User B.) </li>
</ul> <note type="note">
When you select to discard the changes you made, this applies to all the changes and not just to those that have conflicts with the edits made by another user.
</note>
<ul>
<li>Several users have disabled the Autosave setting: If several users that have disabled the Autosave setting are making changes at the same time, Workfront saves the changes made by the user who saves first. Saving these changes should not encounter any conflicts. Workfrontthen compares the changes made by all the other users with the information that it already saved and displays a warning about the conflicting changes to the other users before they can save their information. </li>
</ul> <note type="important">
When you select to keep your changes over all other changes, your changes are saved, unless the tasks you made changes to were deleted by another user. In this case, the warning message informs you that the changes you made to the deleted tasks are lost.
</note>
</div>
</div>
-->
