---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Modification de plusieurs affectations d’utilisateurs dans une liste de tâches
description: Lors de la gestion des affectations de tâche, vous pouvez simultanément les modifier pour plusieurs tâches à la fois à l’aide de la fonction d’édition en bloc d’une liste de tâches.
author: Alina
feature: Work Management
exl-id: 04f7761f-da94-4858-85c5-8dc97bd78bee
source-git-commit: fb538c6511514eedf81f4b9be452d5f87e3f7577
workflow-type: tm+mt
source-wordcount: '976'
ht-degree: 0%

---

# Modification de plusieurs affectations d’utilisateurs dans une liste de tâches

<!--
<p>There is a similar article in Resource Scheduling and a similar one for Issues; when things change, you might need to update all 3</p>
-->

Lors de la gestion des affectations de tâche, vous pouvez simultanément les modifier pour plusieurs tâches à la fois à l’aide de la fonction d’édition en bloc d’une liste de tâches.

Cet article fait référence à la modification de plusieurs affectations d’utilisateurs pour plusieurs tâches dans une liste de tâches. Reportez-vous également aux articles suivants pour modifier des affectations sur plusieurs tâches dans d’autres zones :

* Pour plus d’informations sur l’affectation de tâches à l’aide de l’équilibreur de charge de travail, voir [Présentation de l’affectation de travail dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

Pour plus d’informations sur l’affectation d’une tâche à une ressource d’une liste, voir [Affecter des tâches](../../../manage-work/tasks/assign-tasks/assign-tasks.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Travail ou plus élevé</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modifier l’accès aux projets et tâches</p> <p>Affichage ou accès supérieur aux utilisateurs</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Attribution ou autorisations supérieures à des tâches</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>When to modify user assignments on tasks</h2>
<p>(NOTE: moved to the new article: /Content/Manage work/Tasks/Assign tasks/modify-task-assignments-overview.htm) </p>
<p>You might want to modify the user assignments for multiple tasks for a variety of reasons, including the following:</p>
<ul>
<li>Users join or leave your team</li>
<li> <p>A user takes a vacation that extends beyond task due dates</p> <note type="note">
When assigning users to work, their availability according to their schedules affects the Planned and Projected Dates of tasks. For information about schedules, see
<a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>.
</note> </li>
<li>A specific role or user is set as the assignee for multiple tasks and you want to quickly modify all items to be assigned to a different user or role</li>
</ul>
<p><strong>How removing assignees affects task hours and allocation percentages</strong></p>
<p>(NOTE: move to the new article: /Content/Manage work/Tasks/Assign tasks/modify-task-assignments-overview.htm) </p>
<p>Removing users can affect task hours and allocation percentages. The effect that removing a user has on the task depends on the Duration Type that was selected for the task. For information about Duration&nbsp;Type, see <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Overview of Task Duration and Duration Type</a>.</p>
<p>When you delete a user from a task with the following Duration&nbsp;Types:</p>
<ul>
<li> <p><strong>Simple:</strong> The planned hours assigned to that user are subtracted from the task's total planned hours.</p> <note type="important">
<span class="s1">This could negatively affect your project plan because it changes the total planned hours for the task and the project.</span>
</note> </li>
<li><span class="s1"><strong>Effort Driven:</strong> The allocation percentage does not change for other users.</span> </li>
<li><span class="s1"><strong>Calculated Assignment:</strong> The allocation percentages of other users are adjusted so that the total equals 100%.</span> </li>
<li><span class="s1"><strong>Calculated Work:</strong> The allocation percentage does not change for other users.</span> </li>
</ul>
</div>
-->

## Modification des affectations pour plusieurs tâches

1. Accédez à la liste contenant les tâches pour lesquelles vous souhaitez modifier les affectations.
1. (Facultatif) Créez un filtre pour afficher uniquement les tâches affectées à la personne désignée que vous souhaitez modifier.

   Par exemple, si votre projet contient un rôle spécifique comme responsable par défaut pour plusieurs tâches, vous pouvez créer un filtre pour afficher uniquement les tâches avec ce rôle comme responsable. Vous pouvez ensuite remplacer le rôle par un utilisateur spécifique.

   Pour plus d’informations sur la création d’un filtre, voir [Création ou modification de filtres](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).


1. Pour filtrer selon un rôle, sélectionnez **Rôles d’affectation**, puis cliquez sur **ID**.

   >[!TIP]
   >
   >N’utilisez pas la variable **Affecté à** champ . Cela permet de trouver uniquement le propriétaire Principal de la tâche au lieu des rôles pouvant lui être affectés.

   Ou

   Pour filtrer un utilisateur, sélectionnez **Affecter des utilisateurs,** puis cliquez sur **ID.**

   >[!TIP]
   >
   >N’utilisez pas la variable **Affecté à** champ . Cela permet de trouver uniquement le propriétaire Principal de la tâche au lieu des utilisateurs qui pourraient leur être affectés.

1. Sélectionnez les tâches pour lesquelles vous souhaitez modifier les affectations, puis cliquez sur le bouton **Modifier** icon ![](assets/edit-icon.png).

   La page Modifier les tâches s’affiche. Les éléments que vous modifiez s’affichent dans le coin supérieur gauche de la page.

1. Accédez au **Affectations** .
1. Pour ajouter ou supprimer des personnes désignées, effectuez l’une des opérations suivantes :

   >[!IMPORTANT]
   >
   >La suppression des personnes désignées peut affecter les heures de la tâche et les pourcentages d’attribution. Pour plus d’informations, voir la section [L’impact de la suppression des personnes désignées sur les heures de tâche et les pourcentages d’attribution](#how-removing-assignees-affects-task-hours-and-allocation-percentages) dans cet article.

   * Pour ajouter une nouvelle personne désignée :

      1. Dans le **Affectations** , sélectionnez **Cessionnaire**.

         Les informations communes à toutes les tâches sélectionnées s’affichent. Par exemple, si le même utilisateur est affecté à toutes les tâches, il s’affiche dans la variable **Cessionnaire** colonne . Si des informations ne sont pas communes aux tâches sélectionnées, aucune information ne s’affiche.

      1. Commencez à saisir le nom d’un utilisateur, d’un rôle ou d’une équipe, puis sélectionnez-le lorsqu’il s’affiche dans la liste. L’affectation est ajoutée et ne remplace pas les affectations actuelles sur les tâches sélectionnées.
      >[!TIP]
      >
      > * Vous pouvez affecter plusieurs utilisateurs, rôles de tâche ou équipes. Vous ne pouvez affecter que des utilisateurs, des rôles de tâche et des équipes principaux.
      >   
      > * Lors de l’ajout d’une affectation d’utilisateur, notez l’avatar, le rôle Principal de l’utilisateur ou son adresse électronique pour faire la distinction entre les utilisateurs portant des noms identiques. Les utilisateurs doivent être associés à au moins un rôle de tâche pour l’afficher à mesure que vous les ajoutez.

         > 
         >   Si un utilisateur, un rôle de tâche ou une équipe a été affecté avant d’être désactivé, il reste attribué à l’élément de travail. Dans ce cas, nous vous recommandons ce qui suit :
         >   
         >     * Réaffectez l’élément de travail aux principales ressources.
         >     * Associez les utilisateurs d’une équipe désactivée à une équipe principale et réaffectez l’élément de travail à l’équipe principale.



   * Pour supprimer des personnes désignées :

      1. Cliquez sur le bouton **Icône X** en regard du nom de la personne désignée que vous souhaitez supprimer si la personne désignée s’affiche dans la liste Affectations .

         Ou

         (Conditionnel) Si la personne désignée à supprimer ne s’affiche pas dans la section Affectations , car elle n’est affectée qu’à certaines des tâches que vous avez sélectionnées, cliquez sur **Supprimer le cessionnaire** et commencez à saisir le nom de la personne désignée à supprimer, puis cliquez sur le nom lorsqu’il apparaît dans la liste déroulante.
   * Pour supprimer tous les cessionnaires existants :

      1. Cliquez sur **Supprimer tous les cessionnaires existants**, puis cliquez sur **Oui, supprimer tous les cessionnaires**.

         Cela supprime non seulement les personnes désignées courantes (personnes désignées qui s’affichent dans la boîte de dialogue de modification), mais également toutes les personnes désignées pour toutes les tâches sélectionnées.
      La suppression des utilisateurs des tâches peut affecter les heures de la tâche et les pourcentages d’attribution.

      Pour plus d’informations, voir [Présentation de la modification des affectations de tâche](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).





1. (Facultatif) Modifiez l’une des options suivantes pour les personnes désignées :

   * (Conditionnel) **Attribution % ou heures**: Spécifiez un nouveau pourcentage d’attribution ou de nouvelles heures.

      >[!NOTE]
      >
      >Cette option ne peut être modifiée que si le type de durée est le même pour toutes les tâches en cours de modification. Lorsque le Type de durée est calculé sur Travail ou Effort, vous pouvez mettre à jour le % d’allocation. Lorsque le type de durée est simple, vous pouvez mettre à jour les Heures. Pour plus d’informations sur le type de durée, voir [Présentation de la durée et du type de durée de la tâche](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).
      Si le champ est vide, cela signifie que la valeur est différente selon les tâches ; vous pouvez toutefois le modifier.

   * **Propriétaire de la tâche**: Sélectionnez cette option pour que la personne désignée soit le propriétaire de la tâche pour toutes les tâches en cours de modification.
   * **Le rôle du cessionnaire**: Sélectionnez un rôle dans la liste déroulante. Si cette option n’est pas sélectionnée, Adobe Workfront sélectionne automatiquement le rôle Principal de l’utilisateur.

1. Cliquez sur **Enregistrez les modifications.**
