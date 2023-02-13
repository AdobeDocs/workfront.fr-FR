---
product-area: projects
navigation-topic: manage-tasks
title: Aperçu de l’enregistrement des modifications simultanées dans une liste de tâches
description: Lorsque vous modifiez des tâches dans une liste, vous pouvez utiliser des paramètres d’enregistrement distincts pour indiquer si vous souhaitez que vos modifications soient enregistrées automatiquement lors de la modification manuelle des tâches dans une liste.
author: Alina
feature: Work Management
exl-id: dff52425-4711-40a8-8f40-205d75c506ef
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 0%

---

# Aperçu de l’enregistrement des modifications simultanées dans une liste de tâches

Lorsque vous modifiez des tâches dans une liste, vous pouvez utiliser des paramètres d’enregistrement distincts pour indiquer si vous souhaitez que vos modifications soient enregistrées automatiquement lors de la modification manuelle des tâches dans une liste.

Pour plus d’informations sur la modification des tâches dans une liste de tâches, voir l’article [Editer les tâches dans une liste](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

Parfois, des conflits peuvent apparaître si deux utilisateurs apportent des modifications à la même tâche.

Tenez compte des points suivants lors de l’édition de tâches dans une liste de tâches :

* Adobe Workfront enregistre les modifications que vous apportez aux tâches immédiatement lorsque vous choisissez d’enregistrer vos modifications automatiquement si le type de mise à jour du projet est Automatique ou Automatique ou Changement. Pour plus d’informations sur le type de mise à jour du projet, voir [Sélectionnez le type de mise à jour du projet.](../../../manage-work/projects/manage-projects/select-project-update-type.md).
* Workfront met à jour les informations de la liste sur laquelle vous travaillez chaque minute avec les modifications que d’autres utilisateurs peuvent apporter n’importe où ailleurs dans le système. Vous obtenez ainsi toujours les informations les plus récentes sur les tâches.

Les scénarios suivants se produisent lorsque plusieurs utilisateurs modifient les mêmes tâches :

* **Un utilisateur enregistre automatiquement les modifications dans une liste de tâches et un autre manuellement**: Si un utilisateur (l’utilisateur A) enregistre manuellement les modifications pendant que l’utilisateur B modifie les mêmes tâches, mais enregistre automatiquement les modifications apportées, les modifications en direct effectuées par l’utilisateur B sont mises à jour toutes les minutes dans la liste de l’utilisateur A. En cas de conflit entre les modifications effectuées par les deux utilisateurs, l’utilisateur qui enregistre manuellement (utilisateur A) voit un message d’avertissement avant de pouvoir enregistrer les modifications. Le message d’avertissement affiche les éléments présentant les modifications en conflit. Actuellement, l’utilisateur A peut choisir de conserver ses modifications (qui remplacent les modifications apportées par l’utilisateur B) ou de les ignorer (qui conserve les modifications apportées par l’utilisateur B).

>[!NOTE]
>
>Lorsque vous choisissez d’ignorer les modifications que vous avez apportées, cela s’applique à toutes les modifications et pas seulement à celles qui ont un conflit avec les modifications effectuées par un autre utilisateur.

* **Plusieurs utilisateurs enregistrent manuellement les modifications dans une liste de tâches**: Si plusieurs utilisateurs qui apportent des modifications aux tâches d’une liste enregistrent manuellement en même temps, Workfront enregistre les modifications effectuées par l’utilisateur qui enregistre en premier. L’enregistrement de ces modifications ne doit pas rencontrer de conflit. Workfront compare ensuite les modifications effectuées par tous les autres utilisateurs avec les informations qu’il a déjà enregistrées et affiche un avertissement sur les modifications en conflit pour les autres utilisateurs avant qu’ils puissent enregistrer leurs informations.

>[!IMPORTANT]
>
>Lorsque vous choisissez de conserver vos modifications par rapport à toutes les autres modifications, toutes celles-ci sont enregistrées, sauf si les tâches dans lesquelles vous avez apporté des modifications ont été supprimées par un autre utilisateur. Dans ce cas, le message d’avertissement vous informe que les modifications que vous avez apportées aux tâches supprimées sont perdues.

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
