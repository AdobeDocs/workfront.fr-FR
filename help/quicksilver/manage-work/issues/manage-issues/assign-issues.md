---
product-area: projects
navigation-topic: manage-issues
title: Attribuer les problèmes
description: Vous pouvez affecter des problèmes aux utilisateurs, aux rôles et aux équipes afin d’indiquer qui est responsable de l’exécution des problèmes. Pour obtenir des informations générales sur l’affectation de problèmes, consultez la présentation Modifier les affectations de problèmes .
author: Alina
feature: Work Management
role: User
exl-id: e2dce29e-7370-4580-8326-99c4437998bf
source-git-commit: 02a47566acd0fff151656fe2c5b59a6679748b15
workflow-type: tm+mt
source-wordcount: '1553'
ht-degree: 7%

---

# Attribuer les problèmes

<!--keep the rate card job role information always in yellow till it releases to production - check with Lisa - this might not apply to issues?! -->

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles dans l’ensemble. Il est disponible uniquement dans l’environnement Aperçu pour tous les clients ou dans l’environnement Production pour les clients qui ont activé les versions rapides.</span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation de versions rapides pour votre entreprise](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">Pour plus d’informations sur la version actuelle, voir [Présentation de la version du troisième trimestre 2024](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md).</span>

Vous pouvez affecter des problèmes aux utilisateurs, aux rôles et aux équipes afin d’indiquer qui est responsable de l’exécution des problèmes. Pour obtenir des informations générales sur l’affectation de problèmes, voir [Présentation de la modification des affectations de problème](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md).

>[!TIP]
>
>Vous pouvez affecter plusieurs utilisateurs, rôles de tâche ou équipes. Vous pouvez affecter uniquement les utilisateurs, les rôles de tâche et les équipes actifs.
>
>Si un utilisateur, un rôle de tâche ou une équipe a été affecté avant d’être désactivé, il reste attribué à l’élément de travail. Dans ce cas, nous vous recommandons ce qui suit :
>
>* Réaffectez la tâche aux ressources actives.
>* Associez les utilisateurs d’une équipe désactivée à une équipe active et réaffectez l’élément de travail à l’équipe active.

En plus de cet article, nous vous recommandons de lire les articles suivants pour plus d’informations sur l’attribution des problèmes :

* [Présentation de la modification des affectations de problème](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md)
* [Modification des problèmes](../../../manage-work/issues/manage-issues/edit-issues.md)
* [Modification des affectations d’utilisateurs pour plusieurs problèmes dans une liste](../../../manage-work/issues/manage-issues/edit-assignments-for-multiple-issues.md)
* [Création d’affectations avancées](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md)
* [Rendre des affectations intelligentes](../../../manage-work/tasks/assign-tasks/make-smart-assignments.md)
* [Présentation des affectations intelligentes](../../../manage-work/tasks/assign-tasks/smart-assignments.md)
* [Vue d’ensemble de l’affectation du travail dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)

Vous pouvez affecter un problème à une ou plusieurs ressources au niveau d’un problème individuel, ou vous pouvez affecter plusieurs ressources à plusieurs problèmes simultanément.

L’affectation de problèmes et de tâches est similaire dans Adobe Workfront. Pour obtenir des informations générales sur l’affectation de tâches, voir [Présentation de la modification des affectations de tâche](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td> <p>N’importe quelle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Révision ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux problèmes</p> <p>Affichage ou accès supérieur à Projets et tâches</p> <p>Si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur l’accès aux problèmes de votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Accorder l’accès aux problèmes</a>. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gestion des autorisations liées au problème</p> <p>Attribuez des autorisations à l’élément sur lequel vous copiez le problème avec la possibilité d’ajouter des problèmes.</p> <p> Pour plus d’informations sur l’octroi d’autorisations aux problèmes, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Partage d’un problème </a></p> <p>Pour plus d’informations sur la demande d’autorisations supplémentaires, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md">Accorder l’accès aux utilisateurs</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

* Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Considérations relatives à plusieurs affectations pour les rôles de tâche, les équipes et les utilisateurs

Tenez compte des points suivants lorsque vous affectez plusieurs ressources à une tâche :

* Les utilisateurs peuvent avoir plusieurs rôles de tâche associés à leur profil. Pour plus d’informations sur l’association d’utilisateurs à des rôles de tâche, voir [Modification du profil d’un utilisateur](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Les tâches ou les problèmes sont généralement assignés en premier à un ou plusieurs rôles ou équipes de tâches. Lorsque les projets sont prêts à démarrer, ils doivent peut-être également être affectés aux utilisateurs.

  Si une tâche ou un problème est assigné à un ou plusieurs rôles, puis que vous affectez également un utilisateur, Adobe Workfront décide quel rôle de tâche associer à l’utilisateur supplémentaire (le cas échéant) selon les règles suivantes :

   * Si un seul rôle de tâche est attribué et qu’il correspond au rôle de Principal de l’utilisateur, la tâche ou le problème est affecté uniquement à l’utilisateur qui remplit son rôle de Principal.
   * Si plusieurs rôles sont affectés et qu’au moins un des rôles correspond aux rôles secondaires de l’utilisateur, la tâche ou le problème est alors assigné à l’utilisateur qui remplit l’un de ses Autres rôles — que Workfront sélectionne au hasard s’il existe plusieurs correspondances — ainsi que les rôles supplémentaires affectés.
   * Si un ou plusieurs rôles de tâche sont affectés et qu’il n’y a aucune correspondance avec les rôles de l’utilisateur, la tâche ou le problème est affecté à la fois au rôle ou aux rôles ainsi qu’à l’utilisateur.

* Si une tâche ou un problème est assigné à une équipe et que vous affectez également un utilisateur, la tâche ou le problème reste assigné à l’équipe et à l’utilisateur.

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

## Attribuer un seul problème

1. Accédez à un problème que vous souhaitez affecter.
1. Cliquez sur **Attribuer à** dans le coin supérieur droit de l’en-tête du problème, dans la **Affectations** area

   Ou

   Cliquez sur le nom des affectations en cours, si le problème est déjà assigné.

   ![Bouton Attribuer à](assets/assign-to-button-in-header.png)

1. Utilisez l’une des méthodes suivantes :

   * Commencez à saisir le nom d’un utilisateur, d’un rôle ou d’une équipe que vous souhaitez affecter, puis cliquez dessus lorsqu’il apparaît dans la liste.

     Exemple d’image dans l’environnement de production :
     ![](assets/nwe-assignments-expanded-in-task-header-350x259.png)

     <span class="preview">Exemple d’image dans l’environnement Aperçu :</span>
     <span class="preview">![Recherche d’affectations](assets/smart-assignments-issue-header.png)</span>

   * (Conditionnel) Cliquez sur l’un des noms, rôles ou équipes dans les listes disponibles.
   * Cliquez sur **M&#39;affecter** pour l’affecter à vous-même
   * Cliquez sur **Avancé**.

     La création d’affectations avancées est similaire pour les tâches et les problèmes. Pour plus d’informations sur la façon d’effectuer des affectations avancées, voir [Création d’affectations avancées](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

     >[!TIP]
     >
     >Lors de l’ajout d’une affectation d’utilisateur, notez l’avatar, le rôle de Principal de l’utilisateur ou son adresse électronique pour faire la distinction entre les utilisateurs portant des noms identiques.
     >
     >Les utilisateurs doivent être associés à au moins un rôle de tâche pour l’afficher à mesure que vous les ajoutez.
     >
     >Pour pouvoir voir les adresses e-mail des utilisateurs et utilisatrices, le paramètre Afficher les coordonnées doit être activé dans votre niveau d’accès. Pour plus d’informations, voir [Accorder l’accès aux utilisateurs](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)
     >

     <!-- not sure if this applies to issues; if it does, add this to the TIP above: 
      ><span class="preview">When adding a job role assignment, you can search for the job role or location. Select a role from the Job roles list to use the default billing rate for the assignment, or select a Rate card job role to use the billing rate from the rate card. For more information on rate cards, see [Manage rate cards](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).</span>-->


1. Cliquez sur **Enregistrer** pour terminer l’attribution du problème.
1. (Facultatif) Cliquez sur le **Icône X** en regard du nom des affectations dans la zone Affectations de l’en-tête du problème pour supprimer une affectation.

## Attribuer un problème à une liste

Vous pouvez affecter des problèmes dans une liste ou un rapport lorsque l’un des champs d’affectation est visible dans la vue de la liste. Il s’agit d’une manière plus rapide d’affecter des problèmes.

Selon le champ visible dans la vue, vous pouvez affecter les entités suivantes au problème :

| Option | Entités affectées |
|---|---|
| **Attribuer à** | Attribuer un utilisateur |
| **Attribué** | Attribuer un utilisateur |
| **Affectations** | Affectez des utilisateurs, des rôles de tâche ou des équipes. |

Pour affecter des problèmes dans une liste :

1. Accédez à la liste des problèmes auxquels les champs Affectés à, Affectés ou Affectations sont affichés dans la vue.
1. Pour affecter des problèmes, effectuez l’une des opérations suivantes :

   * Cliquez dans le **Affecté à** ou **Attribué** et commencez à saisir le nom d’un utilisateur actif que vous souhaitez affecter au problème, puis cliquez dessus lorsqu’il s’affiche dans la liste.

     ![](assets/assigned-to-field-task-list-nwe.png)

   * Cliquez dans le **Affectations** et commencez à saisir le nom d’un utilisateur, d’un rôle de tâche ou d’une équipe active que vous souhaitez affecter au problème, puis cliquez dessus lorsqu’il s’affiche dans la liste.

     Exemple d’image dans l’environnement de production :
     ![](assets/assignments-field-task-list-nwe.png)

     <span class="preview">Exemple d’image dans l’environnement Aperçu :</span>
     ![Champ Affectations](assets/assignments-field-task-list-0424.png)

   >[!TIP]
   >
   >Lors de l’ajout d’une affectation d’utilisateur, notez l’avatar, le rôle de Principal de l’utilisateur ou son adresse électronique pour faire la distinction entre les utilisateurs portant des noms identiques.
   >
   >Les utilisateurs doivent être associés à au moins un rôle de tâche pour l’afficher à mesure que vous les ajoutez.
   >
   >Pour pouvoir voir les adresses e-mail des utilisateurs et utilisatrices, le paramètre Afficher les coordonnées doit être activé dans votre niveau d’accès. Pour plus d’informations, consultez [Accorder l’accès aux utilisateurs et utilisatrices](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).


1. (Conditionnel) Lorsqu’il est visible dans le champ Affectations , cliquez sur le bouton **Icône Personnes** ![](assets/teams.png) dans le coin supérieur droit de la zone affectations pour ouvrir la zone Affectations avancées et créer des affectations avancées. Pour plus d’informations, voir [Création d’affectations avancées](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

   >[!TIP]
   >
   >Vous ne pouvez pas effectuer d’affectations avancées à partir des champs Affecté à ou Affecté .

1. Après avoir ajouté les personnes désignées au problème, appuyez sur Entrée ou cliquez n’importe où sur la page pour enregistrer vos modifications.

## Attribuer des problèmes en bloc

1. Accédez à la liste des problèmes que vous souhaitez affecter en bloc.
1. Sélectionnez plusieurs problèmes dans la liste.
1. Cliquez sur le bouton **Icône Modifier** ![](assets/qs-edit-icon.png).

   La variable **Modification des problèmes** s’ouvre.

1. Dans le **Affectations** , sélectionnez la zone **Cessionnaire** puis commencez à saisir le nom d’un utilisateur, d’un rôle de tâche ou d’une équipe que vous souhaitez affecter à tous les problèmes.

   >[!IMPORTANT]
   >
   >Si l’un des problèmes est déjà affecté, les ressources que vous indiquez ici sont ajoutées aux problèmes au lieu de remplacer les ressources existantes sur les problèmes.

1. (Facultatif) Sélectionnez le bouton radio dans le **Propriétaire du problème** pour indiquer la ressource qui est la personne désignée principale ou le propriétaire du problème, lorsque vous affectez plusieurs ressources au problème. Cette option n’est pas disponible pour les équipes.
1. (Facultatif) Sélectionnez un rôle que l’utilisateur doit remplir sur le problème dans la **Choisir un rôle** dans le menu déroulant **Le rôle du cessionnaire** lorsque vous affectez des utilisateurs à des problèmes. Si vous ne sélectionnez pas de rôle, Workfront sélectionne automatiquement le rôle de Principal de l’utilisateur.

1. (Facultatif) Si vous souhaitez supprimer des personnes désignées existantes de tous les problèmes, effectuez l’une des opérations suivantes :

   1. Commencez à saisir le nom d’un utilisateur, d’un rôle ou d’une équipe à supprimer du problème, puis sélectionnez-le lorsqu’il apparaît dans la liste et cliquez sur **Supprimer le cessionnaire** pour ajouter d’autres personnes désignées à supprimer.
   1. Cliquez sur **Supprimer tous les cessionnaires existants** pour supprimer toutes les personnes désignées de tous les problèmes sélectionnés.

1. Cliquez sur **Enregistrer les modifications**.
1. (Facultatif et conditionnel) Lorsque les champs Affectés à ou Affectations s’affichent dans votre liste de problèmes, cliquez dans l’une de ces colonnes pour résoudre un problème, puis cliquez sur le bouton **Icône X** en regard du nom d’une personne désignée pour la supprimer du problème.
