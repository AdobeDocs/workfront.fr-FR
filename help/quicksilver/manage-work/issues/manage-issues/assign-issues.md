---
product-area: projects
navigation-topic: manage-issues
title: Attribuer des problèmes
description: Vous pouvez affecter des problèmes aux utilisateurs et utilisatrices, aux rôles et aux équipes afin d’indiquer qui est responsable de la résolution des problèmes. Pour obtenir des informations générales sur l’affectation de problèmes, consultez la Vue d’ensemble de la modification des affectations de problèmes.
author: Lisa
feature: Work Management
role: User
exl-id: e2dce29e-7370-4580-8326-99c4437998bf
source-git-commit: 0358e79bd606d0035959bba2a47256456b529b18
workflow-type: tm+mt
source-wordcount: '1366'
ht-degree: 78%

---

# Attribuer des problèmes

<!--Audited: 10/2024-->

<!--<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with  a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div> -->

Vous pouvez affecter des problèmes aux utilisateurs et utilisatrices, aux rôles et aux équipes afin d’indiquer qui est responsable de la résolution des problèmes. Pour obtenir des informations générales sur l’affectation de problèmes, consultez la [Vue d’ensemble de la modification des affectations de problèmes](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md).

>[!TIP]
>
>Vous pouvez affecter plusieurs utilisateurs et utilisatrices, fonctions ou équipes. Vous pouvez affecter uniquement les utilisateurs et utilisatrices, fonctions et équipes actifs.
>
>Si une personne, une fonction ou une équipe a été affectée avant d’être désactivée, elle reste affectée à l’élément de travail. Dans ce cas, nous vous recommandons ce qui suit :
>
>* Réaffectez la tâche aux ressources actives.
>* Associez les utilisateurs et utilisatrices d’une équipe désactivée à une équipe active et réaffectez l’élément de travail à l’équipe active.

Outre cet article, nous vous recommandons de lire les articles suivants pour plus d’informations sur l’affectation des problèmes :

* [Vue d’ensemble de la modification des affectations de problèmes](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md)
* [Modifier des problèmes](../../../manage-work/issues/manage-issues/edit-issues.md)
* [Modifier des affectations d’utilisateurs et d’utilisatrices pour plusieurs problèmes dans une liste](../../../manage-work/issues/manage-issues/edit-assignments-for-multiple-issues.md)
* [Créer des affectations avancées](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md)
* [Créer des affectations intelligentes](../../../manage-work/tasks/assign-tasks/make-smart-assignments.md)
* [Vue d’ensemble des affectations intelligentes](../../../manage-work/tasks/assign-tasks/smart-assignments.md)
* [Vue d’ensemble de l’affectation de travail dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)

Vous pouvez affecter un problème à une ou plusieurs ressources au niveau d’un problème spécifique, ou vous pouvez affecter plusieurs ressources à plusieurs problèmes simultanément.

L’affectation d’événements et de tâches est similaire dans Adobe Workfront. Pour obtenir des informations générales sur l’affectation de tâches, consultez la section [Vue d’ensemble de la modification des affectations de tâches](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article. 

<table style="table-layout:auto"> 
 <col> 
 </col>
 <tbody> 
  <tr> 
   <td>Package Adobe Workfront</td> 
   <td> <p>Tous </p> </td> 
  </tr> 
  <tr> 
   <td>Licence Adobe Workfront</td> 
   <td> <p>Contributeur ou version ultérieure</p>
   <p>Révision ou supérieur</p> </td> 
  </tr> 
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès aux problèmes</p> <p>Accédez en lecture seule ou à un niveau supérieur aux Projets et Tâches pour affecter un événement.</p> </td> 
  </tr> 
  <tr> 
   <td>Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations liées aux problèmes</p> <p> Afficher les autorisations ou supérieures pour le projet ou la tâche contenant l’événement lors de l’affectation d’un événement</p><p>Accordez des autorisations ou supérieures au projet ou à la tâche où se trouve le problème lors de l’affectation de plusieurs problèmes.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considérations relatives à plusieurs affectations pour les fonctoins, les équipes et les utilisateurs et utilisatrices

Tenez compte des points suivants lorsque vous affectez plusieurs ressources à un élément de travail :

* Les utilisateurs et utilisatrices peuvent avoir plusieurs fonctions associées à leur profil. Pour plus d’informations sur l’association d’utilisateurs et d’utilisatrices à des fonctions, consultez la section [Modifier le profil d’un utilisateur ou d’une utilisatrice](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Les tâches et les problèmes sont généralement affectés en premier à une ou plusieurs fonctions ou équipes. Lorsque les projets sont prêts à démarrer, ils doivent peut-être également être affectés aux utilisateurs et utilisatrices.

  Si une tâche ou un problème est assigné à une ou plusieurs fonctions, puis que vous affectez également un utilisateur ou une utilisatrice, Adobe Workfront décide quelle fonction associer à l’utilisateur ou à l’utilisatrice supplémentaire (le cas échéant) selon les règles suivantes :

   * Si une seule fonction est attribuée et qu’elle correspond au rôle principal de l’utilisateur ou de l’utilisatrice, la tâche ou le problème est affecté(e) uniquement à l’utilisateur ou à l’utilisatrice qui remplit son rôle principal.
   * Si plusieurs rôles sont affectés et qu’au moins un des rôles correspond aux rôles secondaires de l’utilisateur ou de l’utilisatrice, la tâche ou le problème est alors assigné(e) à l’utilisateur ou à l’utilisatrice qui remplit l’un de ses autres rôles (que Workfront sélectionne au hasard s’il existe plusieurs correspondances) ainsi que les rôles supplémentaires affectés.
   * Si une ou plusieurs fonctions sont affectées et qu’il n’y a aucune correspondance avec les rôles de l’utilisateur ou de l’utilisatrice, la tâche ou le problème est affecté à la fois au ou aux rôles et à l’utilisateur ou l’utilisatrice.

* Si une tâche ou un problème est affecté à une équipe et que vous affectez également un utilisateur ou une utilisatrice, la tâche ou le problème reste affecté(e) à la fois à l’équipe et à l’utilisateur ou à l’utilisatrice.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2> </h2>
<h2>Considerations about removing assignments from issues</h2> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted and moved to Modify issue assignments overview article)</p>
<p>You can remove assignments from one issue at a time, or you can remove assignments from multiple issues in bulk.</p>
<p>For more information about removing assignments from issues in bulk, see <a href="../../../manage-work/issues/manage-issues/edit-assignments-for-multiple-issues.md" class="MCXref xref">Modify user assignments for multiple issues in a list</a>. </p>
<p>Consider the following when removing assignments from issues: </p>
<ul>
<li>When you unassign a user from an issue, the issue remains assigned to the job role that the user fulfilled on the issue.</li>
<li>When you unassign a job role or a team from an issue, the issue remains unassigned if it is not assigned to any other resources. </li>
</ul>
</div>
-->

## Attribuer un seul événement dans l’en-tête de l’événement

1. Accédez au problème que vous souhaitez affecter.
1. Cliquez sur **Affecter à** dans le coin supérieur droit de l’en-tête du problème, dans la zones **Affectations**.

   Ou

   Cliquez sur le nom des affectations en cours, si le problème est déjà affecté.

   ![Bouton Affecter à](assets/assign-to-button-in-header.png)

1. Utilisez l’une des méthodes suivantes :

   * Commencez à saisir le nom d’un utilisateur ou d’une utilisatrice, d’un rôle ou d’une équipe que vous souhaitez affecter, puis cliquez sur celui-ci lorsqu’il apparaît dans la liste.

     ![Recherche d’affectations](assets/smart-assignments-issue-header.png)

   * (Le cas échéant) Cliquez sur l’un des noms, rôles ou équipes dans les listes disponibles.
   * Cliquez sur **Me l’affecter** pour vous l’affecter à vous-même.
   * Cliquez sur **Avancé**.

     La création d’affectations avancées est similaire pour les tâches et les problèmes. Pour plus d’informations sur la création d’affectations avancées, voir [Créer des affectations avancées](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

     >[!TIP]
     >
     >Lors de l’ajout d’une affectation d’utilisateur ou d’utilisatrice, notez l’avatar, le rôle principal de l’utilisateur ou de l’utilisatrice ou son adresse e-mail, pour faire la distinction entre les utilisateurs et utilisatrices portant le même nom.
     >
     >Les utilisateurs et utilisatrices doivent être associés à au moins une fonction pour l’afficher à mesure que vous les ajoutez.
     >
     >Pour que les utilisateurs et utilisatrices puissent afficher les e-mails de leurs utilisateurs et utilisatrices, le paramètre Afficher les coordonnées doit être activé dans votre niveau d’accès. Pour plus d’informations, voir [Accorder l’accès aux utilisateurs et utilisatrices](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
     >

     <!-- this doesn't apply to issues; if it does, add this to the TIP above: 
      ><span class="preview">When adding a job role assignment, you can search for the job role or location. Select a role from the Job roles list to use the default billing rate for the assignment, or select a Rate card job role to use the billing rate from the rate card. For more information on rate cards, see [Manage rate cards](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).</span>-->


1. Cliquez sur **Enregistrer** pour terminer l’affectation du problème.
1. (Facultatif) Cliquez sur l’**icône X** en regard du nom des affectations dans la zone Affectations de l’en-tête du problème pour supprimer une affectation.

## Attribuer un événement en le modifiant sur la ligne dans une liste

Vous pouvez affecter des problèmes dans une liste ou un rapport lorsque l’un des champs d’affectation est visible dans la vue de la liste. Il s’agit d’une méthode plus rapide pour attribuer des problèmes.

Selon le champ visible dans la vue, vous pouvez affecter les entités suivantes au problème :

| Option | Entités affectées |
|---|---|
| **Affecter à** | Affecter un utilisateur ou une utilisatrice |
| **Affecté** | Affecter un utilisateur ou une utilisatrice |
| **Affectations** | Affectez des utilisateurs et utilisatrices, des fonctions ou des équipes. |

Pour affecter des problèmes dans une liste :

1. Accédez à la liste des problèmes dont les champs Affecté à, Affecté ou Affectations sont affichés dans la vue.
1. Pour affecter des problèmes, effectuez l’une des opérations suivantes :

   * Cliquez dans le champ **Affecté à** ou **Affecté** et commencez à saisir le nom d’une personne active que vous souhaitez affecter au problème, puis cliquez sur le nom lorsqu’il apparaît dans la liste.

     ![Affecté au champ](assets/assigned-to-field-task-list-nwe.png)

   * Cliquez dans le champ **Affectations** et commencez à saisir le nom d’une personne active, d’une fonction ou d’une équipe active que vous souhaitez affecter au problème, puis cliquez sur le nom lorsqu’il apparaît dans la liste.

     ![Champ Affectations](assets/assignments-field-0825.png)

   >[!TIP]
   >
   >Lors de l’ajout d’une affectation d’utilisateur ou d’utilisatrice, notez l’avatar, la fonction principale de la personne ou son adresse e-mail pour faire la distinction entre les personnes portant des noms identiques.
   >
   >Les utilisateurs et utilisatrices doivent être associés à au moins une fonction pour l’afficher à mesure que vous les ajoutez.
   >
   >Pour que les utilisateurs et utilisatrices puissent afficher les e-mails de leurs utilisateurs et utilisatrices, le paramètre Afficher les coordonnées doit être activé dans votre niveau d’accès. Pour plus d’informations, voir [Accorder l’accès aux utilisateurs et aux utilisatrices](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

1. (Conditionnel) Dans le champ Affectations, cliquez sur **Avancé** au bas de la liste, ou sur l&#39;**icône Personnes** ![icône Personnes](assets/teams.png) dans le coin supérieur droit de la zone Affectations, pour ouvrir la zone Affectations avancées et créer des affectations avancées. Pour plus d’informations, voir la section [Créer des affectations avancées](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

   >[!TIP]
   >
   >Vous ne pouvez pas créer d’affectations avancées à partir des champs Affecté à ou Affecté.

1. Après avoir ajouté les personnes désignées au problème, appuyez sur la touche Entrée ou cliquez n’importe où sur la page pour enregistrer vos modifications.

## Attribuer un événement dans la zone Modifier l&#39;événement

Vous pouvez affecter un événement lors de sa modification dans la zone Modifier l&#39;événement .

Pour plus d’informations, consultez la section « Affectations » de l’article [Modifier les événements](/help/quicksilver/manage-work/issues/manage-issues/edit-issues.md).

## Affecter des problèmes en bloc

<!--
Assigning issues in bulk is different depending on what environment you choose to do this. 

### Assign issues in bulk in the Production environment 

1. Go to a list of issues that you want to assign in bulk. 
1. Select several issues in the list. 
1. Click the **Edit icon** ![Edit icon](assets/qs-edit-icon.png).

   The **Edit Issues** dialog box opens.

1. In the **Assignments** area, select the **Assignee** box, then start typing the name of a user, job role, or team that you want to assign to all the issues.

   >[!IMPORTANT]
   >
   >If any of the issues is already assigned, the resources you indicate here are added to the issues instead of replacing the existing resources on the issues. 
   
1. (Optional) Select the radio button in the **Issue Owner** column to indicate which resource is the primary assignee or the Owner of the issue, when you assign more than one resource to the issue. This is not available for teams. 
1. (Optional) Select a role that the user should fulfill on the issue from the **Pick a role** drop-down menu in the **Assignee's Role** column when you assign users to issues. If you do not select a role, Workfront automatically selects the user's Primary Role. 

1. (Optional) If you want to remove existing assignees from all issues do one of the following:

   1. Start typing the name of a user, role, or team you want to remove from the issue, then select it when it appears on the list and click **Remove Assignee** to add additional assignees to remove. 
   1. Click **Remove All Existing Assignees** to remove all assignees from all selected issues.

1. Click **Save Changes**.
1. (Optional and conditional) When the Assigned to or the Assignments fields display in your list of issues, click inside one of these columns for an issue, then click the **X icon** next to the name of an assignee to remove it from the issue.

<div class="preview">

### Assign issues in bulk in the Preview environment

-->

1. Accédez à la liste des problèmes que vous souhaitez affecter en bloc.
1. Sélectionnez plusieurs problèmes dans la liste.
1. Cliquez sur l’icône **Modifier** ![Modifier](assets/qs-edit-icon.png).

   La boîte de dialogue **Modifier les problèmes** s’ouvre.

1. Cliquez sur **Affectations** dans le panneau de gauche, et dans la zone **Affectations**, commencez à saisir le nom d’un utilisateur, d’un rôle ou d’une équipe dans le champ **Rechercher des personnes, des rôles ou des équipes**, puis cliquez dessus lorsqu’il s’affiche dans la liste

   Ou

   Cliquez sur **Me l’affecter** pour vous affecter les problèmes.

   >[!IMPORTANT]
   >
   >Si l’un des problèmes est déjà affecté, les ressources que vous indiquez ici y sont ajoutées. Les ressources existantes ne sont pas remplacées sur les problèmes.

1. (Facultatif) Si vous souhaitez supprimer des personnes désignées existantes de tous les événements, cliquez sur le **x** en regard de leur nom.

1. (Facultatif) Mettez à jour le champ **heures prévues**. Pour plus d’informations, voir [Modifier les événements](/help/quicksilver/manage-work/issues/manage-issues/edit-issues.md).

1. Cliquer sur **Enregistrer**.
1. (Facultatif et conditionnel) Lorsque les champs **Affecté à** ou **Affectations** s’affichent dans votre liste d’événements, cliquez dans l’une de ces colonnes pour un événement, puis cliquez sur l’icône **X** en regard du nom d’une personne désignée pour le supprimer de l’événement.


