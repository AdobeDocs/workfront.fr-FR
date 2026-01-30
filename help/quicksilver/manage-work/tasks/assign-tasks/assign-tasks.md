---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Affecter des tâches
description: Vous pouvez affecter des tâches aux utilisateurs et utilisatrices, fonctions ou équipes pour indiquer qui est responsable de l’exécution des tâches. Vous pouvez affecter une tâche à plusieurs ressources à la fois.
author: Lisa
feature: Work Management, Tasks
role: User
exl-id: 611b136e-2c3f-4eac-9d75-e8c12e06148d
source-git-commit: 885bdb0e28c2807f14cc3919a3057a4a48b2422d
workflow-type: tm+mt
source-wordcount: '2479'
ht-degree: 76%

---

# Attribuer des tâches

<!--Audited: 10/2025-->

<!--remove production/ preview and old/ new experience references at prod-->

<div class="preview">

Les informations surlignées sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de manière générale. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Les mêmes fonctionnalités seront également disponibles dans l’environnement de production pour tous les clients et clientes à partir d’une semaine à compter de la version préliminaire.

Pour plus d’informations, voir [Présentation de la version du deuxième trimestre 2026](/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-release-overview.md).

</div>

Vous pouvez affecter des tâches aux utilisateurs et aux utilisatrices, aux fonctions ou aux équipes pour indiquer qui est responsable de l’exécution des tâches. Vous pouvez affecter une tâche à plusieurs ressources à la fois.

>[!TIP]
>
>Vous pouvez affecter plusieurs utilisateurs et utilisatrices, fonctions ou équipes. Vous pouvez affecter uniquement les utilisateurs et utilisatrices, fonctions et équipes actifs.
>
>Si une personne, une fonction ou une équipe a été affectée avant d’être désactivée, elle reste affectée à l’élément de travail. Dans ce cas, nous vous recommandons ce qui suit :
>
>* Réaffectez la tâche aux ressources actives.
>* Associez les utilisateurs et utilisatrices d’une équipe désactivée à une équipe active et réaffectez l’élément de travail à l’équipe active.
>

Le nombre d’utilisateurs et d’utilisatrices à qui une tâche a été affectée et le planning de la personne propriétaire peuvent modifier les dates prévues pour une tâche, entraînant ainsi des modifications dans la chronologie du projet. Pour plus d’informations sur l’impact de l’affectation de plusieurs utilisateurs et utilisatrices à une tâche, consultez la section [Vue d’ensemble de la modification des affectations de tâches](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).

En plus de cet article, nous vous recommandons de lire les articles suivants pour plus d’informations sur l’affectation de tâches :

* [Vue d’ensemble de la modification des affectations de tâches](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md)
* [Vue d’ensemble des affectations intelligentes](../../../manage-work/tasks/assign-tasks/smart-assignments.md)
* [Créer des affectations intelligentes](../../../manage-work/tasks/assign-tasks/make-smart-assignments.md)
* [Créer des affectations avancées](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md)
* [Modifier plusieurs affectations d’utilisateurs et d’utilisatrices dans une liste de tâches](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md)
* [Modifier des tâches](../../../manage-work/tasks/manage-tasks/edit-tasks.md)
* [Vue d’ensemble de la planification d’un projet](../../../manage-work/projects/planning-a-project/plan-project.md)
* [Vue d’ensemble de la date d’achèvement prévue de la tâche](../../../manage-work/tasks/task-information/task-planned-completion-date.md)
* [Définir la date d’achèvement prévue du projet](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md)
* [Configurer les préférences du projet à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)
* [Vue d’ensemble de l’affectation de travail dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td>Licence Adobe Workfront</td> 
   <td> <p>Standard</p>
   <p>Travail ou supérieur</p>
   </td> 
  </tr> 
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès aux projets et tâches</p> <p>Accès en affichage de niveau supérieur aux utilisateurs et utilisatrices</p> </td> 
  </tr> 
  <tr> 
   <td>Autorisations d’objet</td>
   <td>Autorisations de contribution ou de niveau supérieur pour une tâche</td>
  </tr>
 </tbody>
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considérations relatives à plusieurs affectations pour les fonctoins, les équipes et les utilisateurs et utilisatrices

Tenez compte des points suivants lorsque vous affectez plusieurs ressources à un élément de travail :

* Les utilisateurs et utilisatrices peuvent avoir plusieurs fonctions associées à leur profil. Pour plus d’informations sur l’affectation de fonctions à des utilisateurs et utilisatrices, consultez la section [Modifier le profil d’un utilisateur ou d’une utilisatrice](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Si vous affectez plusieurs utilisateurs et utilisatrices à une tâche ou à un problème, la première personne sélectionnée est désignée automatiquement comme propriétaire de la tâche ou du problème.
Pour plus d’informations sur la modification de cette option, consultez les informations sur l’option « Principal » dans l’article [Créer des affectations avancées](create-advanced-assignments.md).

* Une équipe ne peut pas être une désignée comme cessionnaire principale pour une tâche ou un problème. Seules une personne ou une fonction peuvent être désignées comme cessionnaire principale sur une tâche ou un problème.

<!-- If a task is assigned to multiple teams, the primary team sees the Work On It button. waiting on team to verify if this is true. (Courtney)
You cannot make a team be a Primary on a task/ issue. (Alina) -->

* Les tâches et les problèmes d’un projet peuvent être affectés en premier à une ou plusieurs équipes ou fonctions. Lorsque le projet est prêt à démarrer, il doit ausi être affecté à des utilisateurs et des utilisatrices :

  <table>
  <col> 
  <col> 
  <tbody>
  <tr>
   <td>Équipes</td>
   <td>Si une tâche est affectée à une équipe et à un utilisateur ou une utilisatrice, la tâche reste affectée à l’équipe et à l’utilisateur ou l’utilisatrice, même si cette personne n’est pas membre de l’équipe.</td>
  </tr>
  <tr>
   <td>Fonctions</td>
   <td><p>Si vous affectez une tâche ou un problème à une ou plusieurs fonctions et à un utilisateur ou à une utilisatrice, suivez les règles suivantes pour affecter cette fonction à l’utilisateur ou à l’utilisatrice supplémentaire :</p>
     <ul>
      <li>Si une seule fonction est affectée et qu’elle correspond au rôle principal de l’utilisateur ou de l’utilisatrice (configuré dans son profil), la tâche ou le problème est affecté(e) uniquement à cet utilisateur ou à cette utilisatrice.</li>
      <li>Si plusieurs fonctions sont affectées et qu’au moins l’une d’elles correspond à une fonction de l’utilisateur ou de l’utilisatrice, la tâche ou le problème est affecté(e) à cet utilisateur ou à cette utilisatrice (la fonction est choisie de manière aléatoire s’il y a plusieurs correspondances), ainsi que tout autre fonction affectée.</li>
      <li>Si au moins une fonction est affectée et qu’aucune correspondance n’est trouvée avec les fonctions de l’utilisateur ou de l’utilisatrice, la tâche ou le problème est affecté(e) à la fois à la fonction ou aux fonctions et à l’utilisateur ou l’utilisatrice.</li>
     </ul>
   <p>Pour plus d’informations sur la fonction principale ou les autres fonctions d’un utilisateur ou d’une utilisatrice, consultez la section <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md">Modifier le profil d’un utilisateur ou d’une utilisatrice</a>.</p>
   </td> 
     </tr>
  </tbody>
  </table>

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Considerations for multiple user assignments and using schedules</h2>
<p>(NOTE: moved to the Modify task assignments overview standalone article)</p>
<p>You can assign multiple resources to a task. When you assign a user to a task, Workfront uses the user's schedule to calculate the planned dates for the task which ultimately determine the timeline of the project. Using the schedule of the user takes into account their time off, holidays, and weekend days which are considered non-working days when task activity cannot occur. </p>
<p>When you assign multiple users to a task, your Workfront administrator <span>or a group administrator</span> determines which one of the following schedules Workfront uses to determine the planned dates of the tasks, based on schedules: </p>
<ul>
<li> <p><strong>The Primary Assignee's schedule</strong>: this is the schedule associated with the user designated as the task Owner.</p> <p>For information about associating users with schedules, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.</p> </li>
<li><strong>The Project's schedule</strong>: this is the schedule associated with the project. For adding a schedule to a project, see <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.</li>
</ul>
<p>For information about setting up which schedule a project uses in the case of multiple assignments, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>. </p>
</div>
-->

## Affecter une seule tâche

1. Accédez à une tâche que vous souhaitez affecter.
1. Cliquez sur **Affecter à** dans le champ **Affectations** dans l’en-tête de la tâche.

   Ou

   Cliquez sur le nom des affectations si la tâche est déjà affectée.

   ![Affectations](assets/assignments-from-task-header-0825.png)

1. Utilisez l’une des méthodes suivantes :

   * Commencez à saisir le nom d’un utilisateur, d’une fonction ou d’une équipe à affecter, puis cliquez dessus lorsqu’il apparaît dans la liste.

     >[!TIP]
     >
     >Lors de l’ajout d’une affectation d’utilisateur ou d’utilisatrice, notez l’avatar, le rôle principal de l’utilisateur ou de l’utilisatrice ou son adresse e-mail, pour faire la distinction entre les utilisateurs et utilisatrices portant le même nom. Les utilisateurs et utilisatrices doivent être associés à au moins une fonction pour l’afficher à mesure que vous les ajoutez.
     >
     >Pour que les utilisateurs et utilisatrices puissent afficher les e-mails de leurs utilisateurs et utilisatrices, le paramètre Afficher les coordonnées doit être activé dans votre niveau d’accès. Pour plus d’informations, voir [Accorder l’accès aux utilisateurs et aux utilisatrices](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

   * (Conditionnel) Cliquez sur l’un des noms figurant dans les listes **Utilisateurs et équipes** ou **Fonctions** lorsqu’ils s’affichent. Consultez [Vue d’ensemble des affectations intelligentes](../../../manage-work/tasks/assign-tasks/smart-assignments.md) pour en savoir plus.

     Vous pouvez commencer à saisir le nom d’un utilisateur ou d’une utilisatrice, d’une équipe, ou d’une fonction pour l’affecter à la tâche, puis sélectionner le nom lorsqu’il s’affiche dans la liste.

   * Cliquez sur **Avancé**.

     Pour plus d’informations sur la façon d’effectuer des affectations avancées, consultez la section [Créer des affectations avancées](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

1. Cliquer sur **Enregistrer**.
1. (Facultatif et le cas échéant) Cliquez sur l’**icône X** à côté du nom de l’affectation dans le panneau de droite de la tâche pour supprimer une affectation, si vous avez cliqué sur **Avancé**.

## Affectation d’une tâche dans une liste lors de sa modification sur la ligne

Vous pouvez affecter des tâches dans une liste ou un rapport lorsque l’un des champs d’affectation est visible dans la vue de la liste. C’est un moyen plus rapide d’affecter des tâches. Cet article décrit comment modifier des affectations pour une tâche dans une liste. Pour plus d’informations sur la modification de plusieurs affectations pour plusieurs tâches dans une liste, consultez la section [Modifier plusieurs affectations d’utilisateurs et d’utilisatrices dans une liste de tâches](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md).

Selon le champ visible dans la vue, vous pouvez affecter les entités suivantes à la tâche :

| champ | Entités affectées |
|---|---|
| **Affecter à** | Affecter un utilisateur ou une utilisatrice |
| **Affecté** | Affecter un utilisateur ou une utilisatrice |
| **Affectations** | Affecter des utilisateurs et des utilisatrices, des fonctions ou des équipes |

Pour affecter des tâches dans une liste, procédez comme suit :

1. Accédez à la liste des tâches dans laquelle les champs « Affecté à », « Affecté » ou « Affectations » sont affichés.
1. (Facultatif) Cliquez sur le menu déroulant **Enregistrement automatique** et sélectionnez l’une des options suivantes :

   | Option | Description des options |
   |---|---|
   | Enregistrement automatique | Les modifications que vous apportez aux tâches sont automatiquement enregistrées et ne peuvent pas être annulées. |
   | Enregistrement manuel | Vous devez enregistrer vos modifications manuellement. Vous pouvez annuler vos modifications avant de les enregistrer. |
   | Planification chronologique | Vous devez enregistrer vos modifications manuellement. Vous pouvez annuler vos modifications avant de les enregistrer. L’enregistrement de vos modifications et de toutes les dépendances du projet est plus rapide que lors de la sélection de l’enregistrement manuel. |

   Pour plus d’informations sur l’enregistrement des tâches lorsque vous les modifiez dans une liste, voir la section [Modifier les tâches dans une liste](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

1. Pour affecter des tâches, effectuez l’une des opérations suivantes :

   * Cliquez dans les champs **Affecté à** ou **Affecté** et commencez à saisir le nom d’une personne active que vous souhaitez affecter à la tâche, puis cliquez dessus lorsqu’il s’affiche dans la liste.
   * Cliquez dans le champ **Affectations** et commencez à saisir le nom d’une personne, d’une fonction ou d’une équipe active à affecter à la tâche, puis cliquez dessus lorsqu’il s’affiche dans la liste.

     >[!TIP]
     >
     >Lors de l’ajout d’une affectation d’utilisateur ou d’utilisatrice, notez l’avatar, le rôle principal de l’utilisateur ou de l’utilisatrice ou son adresse e-mail, pour faire la distinction entre les utilisateurs et utilisatrices portant le même nom. Les utilisateurs et utilisatrices doivent être associés à au moins une fonction pour l’afficher à mesure que vous les ajoutez.
     >
     >Pour que les utilisateurs et utilisatrices puissent afficher les e-mails de leurs utilisateurs et utilisatrices, le paramètre Afficher les coordonnées doit être activé dans votre niveau d’accès. Pour plus d’informations, voir [Accorder l’accès aux utilisateurs et utilisatrices](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)

     <!--<span class="preview">When adding a job role assignment, you can search for the job role or location. Select a Job role to use the default billing rate for the assignment, or select a Rate Card job role to use the billing rate from the rate card. For more information on rate cards, see [Manage rate cards](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).</span>-->


1. (Conditionnel) Dans le champ Affectations, cliquez sur **Avancé** au bas de la liste, ou sur l&#39;**icône Personnes** ![icône Personnes](assets/teams.png) dans le coin supérieur droit de la zone Affectations, pour ouvrir la zone **Affectations avancées** et créer des affectations avancées.

   Pour plus d’informations, voir la section [Créer des affectations avancées](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

   >[!TIP]
   >
   >Vous ne pouvez pas créer d’affectations avancées à partir des champs Affecté à ou Affecté.

1. Après avoir ajouté les personnes cessionnaires à la tâche, appuyez sur Entrée ou cliquez n’importe où sur la page pour enregistrer vos modifications si vous avez sélectionné Enregistrement automatique. Sinon, cliquez sur **Enregistrer**.

## Affecter plusieurs tâches en bloc à partir d’une liste

L’affectation de plusieurs tâches en bloc à partir d’une liste diffère selon l’environnement choisi.

### Attribuez plusieurs tâches en bloc à partir d’une liste dans l’environnement de production .

1. Accédez à la liste des tâches que vous souhaitez affecter en masse.
1. (Le cas échéant) Assurez-vous que l’option **Enregistrement automatique** est sélectionnée si vous vous trouvez dans la liste des tâches d’un projet.

   >[!IMPORTANT]
   >
   >Vous ne pouvez pas modifier les tâches en masse lors de l’enregistrement manuel des tâches sur un projet.

1. Sélectionnez plusieurs tâches dans la liste des tâches.
1. Cliquez sur **Modifier**.

   La boîte de dialogue **Modifier les tâches** s’ouvre dans la nouvelle expérience .

1. Continuez à affecter les tâches à l’aide de la nouvelle expérience.

   Pour plus d’informations, consultez la section [Affecter plusieurs tâches en bloc à partir d’une liste dans la nouvelle expérience](#assign-multiple-tasks-in-bulk-from-a-list-in-the-new-experience) dans cet article.

1. (Facultatif) Cliquez sur **Revenir à l’ancienne expérience** au bas de la zone **Modifier les tâches** pour ouvrir l’ancienne expérience.

1. (Conditionnel) Dans l’ancienne expérience, dans la zone **Affectations**, sélectionnez la zone **Personne désignée**, puis commencez à saisir le nom d’un utilisateur, d’une fonction ou d’une équipe que vous souhaitez affecter à toutes les tâches.

   >[!IMPORTANT]
   >
   >Si l’une des tâches est déjà affectée, les ressources que vous indiquez ici sont ajoutées aux tâches au lieu de remplacer les ressources existantes sur les tâches.

1. (Facultatif) Sélectionnez la case d’option dans la colonne **Personne propriétaire de la tâche** pour indiquer la ressource qui est la personne cessionnaire principale ou la personne propriétaire de la tâche, lorsque vous affectez plusieurs ressources à la tâche. Cette option n’est pas disponible pour les équipes.
1. (Le cas échéant) Spécifiez le **% d’affectation** pour chaque ressource affectée à la tâche si toutes les tâches sélectionnées ont un type de durée Piloté par l’effort ou Calcul d’affectation. Cela indique le temps que ces ressources doivent consacrer à l’exécution de la tâche. Cette option n’est disponible que pour les utilisateurs et utilisatrices et les fonctions.

   Ou

   Indiquez le nombre d’**heures** pour chaque ressource affectée à la tâche si toutes les tâches que vous avez sélectionnées ont un type de durée Simple. Le total des heures pour toutes les ressources doit être égal au nombre d’heures prévues pour la tâche.

   >[!IMPORTANT]
   >
   >Vous ne pouvez pas spécifier le pourcentage d’affectation ni le nombre d’heures par ressource si les tâches que vous avez sélectionnées ont des types de durée différents ou si les tâches que vous avez sélectionnées ont des types de durée différents.

   Pour plus d’informations sur le type de durée des tâches, voir la section [Vue d’ensemble de la durée de la tâche et du type de durée](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

1. (Facultatif) Sélectionnez un rôle que l’utilisateur ou l’utilisatrice doit remplir dans la tâche à partir du menu déroulant **Choisir un rôle** dans la colonne **Rôle de la personne cessionnaire** lorsque vous affectez des personnes à des tâches. Si vous ne sélectionnez pas de rôle, Workfront sélectionne automatiquement le rôle principal de l’utilisateur ou l’utilisatrice.

1. (Facultatif) Si vous souhaitez supprimer des personnes cessionnaires existantes de toutes les tâches, effectuez l’une des opérations suivantes :

   1. Commencez par saisir le nom d’une personne, d’un rôle ou d’une équipe à supprimer de la tâche, puis sélectionnez-le lorsqu’il apparaît dans la liste et cliquez sur **Supprimer la personne cessionnaire** pour supprimer d’autres personnes cessionnaires.
   1. Cliquez sur **Supprimer toutes les personnes cessionnaires existantes** pour supprimer toutes les personnes cessionnaires de toutes les tâches sélectionnées.

1. Cliquez sur **Enregistrer les modifications**.
1. (Facultatif et le cas échéant) Lorsque les champs Affecté à ou Affectations s’affichent dans la liste des tâches, cliquez dans l’une de ces colonnes pour une tâche, puis cliquez sur **l’Icône X** en regard du nom d’une personne cessionnaire pour la supprimer de la tâche.


#### Affectez plusieurs tâches en bloc à partir d’une liste dans la nouvelle expérience

1. Accédez à la liste des tâches que vous souhaitez affecter en masse.
1. (Le cas échéant) Assurez-vous que l’option **Enregistrement automatique** est sélectionnée si vous vous trouvez dans la liste des tâches d’un projet.

   >[!IMPORTANT]
   >
   >Vous ne pouvez pas modifier les tâches en masse lors de l’enregistrement manuel des tâches sur un projet.

1. Sélectionnez plusieurs tâches dans la liste des tâches.
1. Cliquez sur **Modifier**.

   La boîte de dialogue **Modifier les tâches** s’ouvre.

1. Dans la zone **Affectations**, commencez à saisir le nom des utilisateurs, des équipes ou des rôles dans le champ **Rechercher des personnes, des rôles ou des équipes** fourni, puis cliquez dessus lorsqu’ils s’affichent dans la liste

   Ou

   Cliquez sur **Me l’affecter** pour l’affecter à vous-même.

   >[!IMPORTANT]
   >
   >Si l’une des tâches est déjà affectée, les ressources que vous indiquez ici sont ajoutées aux tâches au lieu de remplacer les ressources existantes sur les tâches.

1. Cliquez dans le champ **Type de durée** et choisissez un type de durée.

   Pour plus d’informations sur le type de durée des tâches, voir la section [Vue d’ensemble de la durée de la tâche et du type de durée](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

1. (Conditionnel) Selon le **Type de durée** que vous avez sélectionné, mettez à jour les champs suivants :

   * Durée
   * Heures prévues

     Pour plus d’informations, voir [Modifier des tâches](/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md).

1. (Facultatif) Si vous souhaitez supprimer des personnes désignées existantes de toutes les tâches, cliquez sur le **x** en regard de leur nom dans le champ **Rechercher des personnes, des rôles ou des équipes**.

1. Cliquer sur **Enregistrer**.
1. (Facultatif et conditionnel) Lorsque les champs **Affecté à** ou **Affectations** s’affichent dans votre liste de tâches, cliquez dans l’une de ces colonnes pour une tâche, puis cliquez sur l’icône **X** en regard du nom d’une personne désignée pour la supprimer de la tâche.

<div class="preview">

### Affectez plusieurs tâches en bloc à partir d’une liste dans l’environnement Aperçu

1. Accédez à la liste des tâches que vous souhaitez affecter en masse.
1. (Le cas échéant) Assurez-vous que l’option **Enregistrement automatique** est sélectionnée si vous vous trouvez dans la liste des tâches d’un projet.

   >[!IMPORTANT]
   >
   >Vous ne pouvez pas modifier les tâches en masse lors de l’enregistrement manuel des tâches sur un projet.

1. Sélectionnez plusieurs tâches dans la liste des tâches.
1. Cliquez sur **Modifier**.

   La boîte de dialogue **Modifier les tâches** s’ouvre.

1. Dans la zone **Affectations**, commencez à saisir le nom des utilisateurs, des équipes ou des rôles dans le champ **Rechercher des personnes, des rôles ou des équipes** fourni, puis cliquez dessus lorsqu’ils s’affichent dans la liste

   >[!IMPORTANT]
   >
   >Si l’une des tâches est déjà affectée, les ressources que vous indiquez ici sont ajoutées aux tâches au lieu de remplacer les ressources existantes sur les tâches.

1. Renseignez les champs suivants pour les tâches sélectionnées :

   * Pointez sur le nom de l’affectation, puis cliquez sur **Créer un Principal** pour indiquer quelle personne désignée est le propriétaire de la tâche.
   * **Type de durée**

     Pour plus d’informations sur le type de durée des tâches, voir la section [Vue d’ensemble de la durée de la tâche et du type de durée](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

   * **Durée**
   * **Nombre d’heures prévues**

     Pour plus d’informations, voir [Modifier des tâches](/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md).

1. (Facultatif) Si vous souhaitez supprimer des personnes désignées existantes de toutes les tâches, cliquez sur le **x** en regard de leur nom dans le champ **Rechercher des personnes, des rôles ou des équipes**.

1. Cliquer sur **Enregistrer**.
1. (Facultatif et conditionnel) Lorsque les champs **Affecté à** ou **Affectations** s’affichent dans votre liste de tâches, cliquez dans l’une de ces colonnes pour une tâche, puis cliquez sur l’icône **X** en regard du nom d’une personne désignée pour la supprimer de la tâche.

</div>

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Considerations about unassigning tasks</h2>
<p>(NOTE: moved this to the new article: /Content/Manage work/Tasks/Assign tasks/modify-task-assignments-overview.htm)</p>
<p>You can remove assignments from one task at a time, or you can remove assignments from multiple tasks in bulk.</p>
<p>For more information about removing assignments from tasks in bulk, see <a href="../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md" class="MCXref xref">Modify multiple user assignments in a task list</a>. </p>
<p>Consider the following when removing assignments from tasks: </p>
<ul>
<li>When you unassign a user from a task, the task remains assigned to the job role that the user fulfilled on the task.</li>
<li>When you unassign a job role or a team from a task, the task remains unassigned if it is not assigned to any other resources. </li>
</ul>
</div>
-->


