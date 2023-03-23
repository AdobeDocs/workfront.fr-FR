---
product-area: projects
navigation-topic: manage-projects
title: Modification de projets
description: Vous pouvez modifier un projet dans Adobe Workfront aussi souvent que nécessaire. Idéalement, vous devez modifier un projet lorsque celui-ci est à l’état Planification .
author: Alina
feature: Work Management
exl-id: a6a1f178-189a-4c41-835b-7726081a2b49
source-git-commit: addcff71ff067be22e9ee80f997af545293fa5db
workflow-type: tm+mt
source-wordcount: '7718'
ht-degree: 2%

---

# Modification de projets

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles dans l’ensemble. Il est disponible pour tous les clients de l’environnement Aperçu et pour un groupe sélectionné de clients de l’environnement Production.</span>

<!--
<p>***Linked to many articles,</p>
<p>The Resource Pools part also duplicates in the "Working with Resource Pools" article </p>
<p>The Update Type section is also documented in Selecting the Project Update Type article</p>
<p>Keep the reference link to the other article that also documents the Update Type) </p>
<p>(NOTE 2: information described here also exists in these articles:</p>
<p>** Project Overview area</p>
<p>**Manage project Finance area</p>
<p>If you need to update just one field, check to see if that field is also listed there and update in both places.)</p>
</div>
-->

Vous pouvez modifier un projet dans Adobe Workfront aussi souvent que nécessaire. Nous vous recommandons de modifier les projets au minimum après leur changement d’état sur Actuel, afin d’éviter toute confusion en envoyant des notifications sur les modifications à l’ensemble de l’équipe de projet. Idéalement, vous devez modifier un projet lorsque celui-ci est à l’état Planification . Pour plus d’informations sur l’équipe de projet, voir [Présentation de l’équipe de projet](../../../manage-work/projects/planning-a-project/project-team-overview.md).

## Exigences d’accès

<!--drafted - replace table at P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td><p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to projects, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> 
    <ul> 
     <li> <p>Contribute permissions to a project to edit it in the Project Details area </p> </li> 
     <li> <p>Manage permissions to a project to edit it in the Edit Project box</p> </li> 
    </ul> <p> For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modifier l’accès aux projets</p> <p>Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur l’accès aux projets, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Accorder l’accès aux projets</a>. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> 
    <ul> 
     <li> <p>Attribuez des autorisations à un projet pour le modifier dans la zone Détails du projet. </p> </li> 
     <li> <p>Gérer les autorisations d’un projet pour le modifier dans la zone Modifier le projet</p> </li> 
    </ul> <p> Pour plus d’informations sur les autorisations de projet, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Partage d’un projet dans Adobe Workfront</a>.</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Restrictions relatives à la modification de projets

Certaines restrictions peuvent vous empêcher de modifier des projets.

Tenez compte des points suivants lors de la modification de projets :

* Vous ne pouvez pas modifier les projets qui se trouvent dans un processus d’approbation, à l’exception de la durée de journalisation.
* Vous pouvez joindre des documents ou des modèles à un projet dont l’état est Terminé, Mort ou En attente d’approbation n’est actif que si votre administrateur Workfront ou un administrateur de groupe a activé cette fonctionnalité dans la zone Préférences du projet. Pour plus d’informations sur la définition des préférences de projet, voir [Configuration des préférences de projet à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* Vous ne pouvez modifier que les informations suivantes sur un projet dont l’état est Désactivé ou Terminé :

   * Modifier les dépenses existantes.
   * Ajouter, supprimer ou modifier des formulaires personnalisés.

## Modification d’un projet

En modifiant un projet, vous pouvez modifier les informations et les paramètres du projet, ainsi que les tâches et les problèmes liés au projet.

Certains paramètres mentionnés dans cet article peuvent être modifiés à partir de leur état par défaut par leur état dans le modèle à partir duquel le projet a été créé. Pour plus d’informations sur la modification de modèles, voir [Modifier des modèles de projet](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Projets**.
1. (Facultatif) Cliquez sur **Projets actifs** ou **Projets que je possède** dans le coin supérieur droit pour afficher les projets dont vous êtes le propriétaire ou les projets dont vous faites partie de l’équipe de projet.

   ![](assets/projects-on-my-own-buttons-350x302.png)

1. Cliquez sur le nom du projet à modifier pour ouvrir la page du projet.

   >[!NOTE]
   >
   >Si vous êtes administrateur de groupe, vous pouvez afficher et modifier les projets de votre groupe dans la zone Groupes , ainsi que dans la zone Projets . Pour plus d’informations, voir [Création et modification des projets d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

1. (Facultatif) Pour modifier des informations limitées sur un projet, cliquez sur **Détails du projet** dans le panneau de gauche.

   ![](assets/nwe-project-details-expanded-350x298.png)

   >[!NOTE]
   >
   >Selon la manière dont votre administrateur Workfront ou l’administrateur de groupe a modifié votre modèle de mise en page, les champs de la zone Détails du projet peuvent être réorganisés ou non. Pour plus d’informations, voir [Personnalisation de la vue Détails à l’aide d’un modèle de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   Pour modifier les informations de la section Détails , procédez comme suit :

   1. (Facultatif) Cliquez sur le **Réduire tout** dans le coin supérieur droit pour réduire toutes les zones.
   1. (Facultatif et conditionnel) Lorsqu’une zone est réduite, cliquez sur le bouton **flèche pointant vers la droite** ![](assets/right-pointing-arrow.png) en regard de chaque zone pour développer la zone à modifier.
   1. Pour plus d’informations sur la modification des informations dans l’onglet Détails du projet, voir les articles suivants :

      * [Gestion des informations dans la zone Aperçu du projet](../../../manage-work/projects/manage-projects/understand-project-overview-area.md)
      * [Gestion des informations dans la zone Finance du projet](../../../manage-work/projects/project-finances/manage-project-finance-area.md)
   1. (Facultatif) Pour joindre un formulaire personnalisé, commencez à saisir le nom d’un formulaire dans le champ **Ajouter un formulaire personnalisé** puis sélectionnez-la lorsqu’elle s’affiche dans la liste, puis cliquez sur **Enregistrer les modifications**.
   1. (Facultatif) Cliquez sur le **Exporter** icon ![](assets/export.png) pour exporter les informations d’aperçu et de formulaires personnalisés vers un fichier de PDF, cliquez sur **Exporter**. Sélectionnez l’une des options suivantes :

      * Sélectionner tout (s’affiche uniquement lorsqu’au moins un formulaire personnalisé est joint)
      * Vue d’ensemble
      * Nom d’un ou de plusieurs formulaires personnalisés

      Le fichier du PDF est téléchargé sur votre ordinateur.

      ![](assets/export-issue-details-selection-box-with-export-button-350x418.png)

      Pour plus d’informations, voir [Exportation de formulaires personnalisés et de détails d’objet](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md).
   Pour plus d’informations sur les champs visibles dans la section Détails du projet, passez à la modification du projet dans la zone Modifier le projet , comme décrit ci-dessous.
1. Pour modifier toutes les informations relatives au projet, cliquez sur le bouton **Plus** menu ![](assets/qs-more-menu.png) en regard du nom du projet, puis cliquez sur **Modifier**.

   Ou

   Dans une liste de projets, sélectionnez un projet, puis cliquez sur le bouton **Modifier** icon ![](assets/edit-icon.png) en haut de la liste.

   Le **Modifier le projet** s’ouvre.

   >[!IMPORTANT]
   >
   >Pour afficher l’option Modifier, vous devez disposer des autorisations de gestion du projet.

   Tous les champs de projet sont disponibles dans la zone Modifier le projet et sont regroupés par zones répertoriées dans le panneau de gauche.

   >[!NOTE]
   >
   >Selon la manière dont votre administrateur Workfront ou l’administrateur de groupe a modifié votre modèle de mise en page, les zones du panneau de gauche de la boîte de dialogue Modifier le projet ou les champs répertoriés dans ces zones peuvent être réorganisées ou ne pas s’afficher. Pour plus d’informations, voir [Personnalisation de la vue Détails à l’aide d’un modèle de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

1. (Conditionnel) Si vous avez cliqué sur la variable **Plus** puis **Modifier**, envisagez de mettre à jour les informations dans l’une des zones suivantes répertoriées dans le panneau de gauche :

   * [Nom du projet](#project-name)
   * [Vue d’ensemble](#overview)
   * [Formulaires personnalisés](#custom-forms)
   * [Finances](#finance)
   * [Paramètres du projet](#project-settings)
   * [Paramètres de la tâche](#task-settings)
   * [Paramètres de l&#39;événement](#issue-settings)
   * [Accès](#access)

   >[!NOTE]
   >
   >Selon la manière dont votre administrateur Workfront configure le modèle de mise en page pour la zone Détails du projet, les sections et les champs de la zone Modifier le projet peuvent être différents dans votre environnement. Pour plus d’informations, voir [Personnalisation de la vue Détails à l’aide d’un modèle de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

### Nom du projet {#project-name}

1. Commencez à modifier votre projet comme décrit ci-dessus.
1. Cliquez sur **Nom du projet** dans le panneau de gauche.

   ![](assets/nwe-project-name-in-edit-project-box-350x125.png)

1. Mettez à jour le nom du projet.

   Vous ne pouvez pas modifier le nom du projet lorsque vous modifiez des projets en bloc.

### Vue d’ensemble {#overview}

1. Commencez à modifier votre projet comme décrit ci-dessus.
1. Cliquez sur **Présentation** dans le panneau de gauche.

   ![](assets/nwe-overview-in-edit-project-box-350x172.png)

1. Mettez à jour les informations suivantes sur le projet :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Description</strong> </td> 
      <td> <p>Ajoutez des informations supplémentaires sur le projet.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Statut</strong> </td> 
      <td> <p>Sélectionnez l’état du projet. Vous ne pouvez pas marquer un projet comme terminé avant que toutes les tâches et tous les problèmes ne soient terminés. Pour plus d’informations sur les états d’un projet, voir <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md" class="MCXref xref">Accéder à la liste des états du projet système</a></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Priorité</strong> </td> 
      <td> <p> <p>Il s’agit simplement d’un indicateur visuel qui vous permet de hiérarchiser vos projets.</p> <p>Selon les préférences du projet sélectionnées par votre administrateur Workfront, les noms des priorités peuvent être différents pour vous. Pour plus d’informations sur la modification des priorités, voir <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md" class="MCXref xref">Créer et personnaliser des priorités</a></p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>URL</strong> </td> 
      <td> <p>Spécifiez un lien Web qui se rapporte aux informations sur ce projet.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Type de statut</strong> </td> 
      <td> <p>Effectuez une sélection parmi les types de condition suivants : 
       <ul> 
       <li><strong>Manuel :</strong> Le propriétaire du projet définit manuellement la condition sur le projet.</li> 
       <li><strong>État de progression :</strong> Workfront définit automatiquement la condition en fonction de l’état de progression des tâches sur le chemin critique. Pour plus d’informations sur la compréhension de l’état de progression, voir <a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">Présentation de l’état de progression de la tâche</a>.</li> 
       </ul><p>Votre administrateur Workfront<span> ou un administrateur de groupe</span> sélectionne la valeur par défaut du mode de calcul de la condition des projets pour votre système. <span>ou votre groupe</span>. Pour plus d’informations sur la définition des paramètres par défaut d’un projet, voir <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configuration des préférences de projet à l’échelle du système</a>. </p></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Condition</strong> </td> 
      <td> <p> <p>(S’affiche uniquement une fois que vous avez sélectionné <strong>Manuel</strong> pour le <strong>Type de condition</strong>) : Sélectionnez une condition pour indiquer le déroulement du projet. </p> <p>Pour plus d’informations sur la façon dont les conditions du projet peuvent être définies automatiquement ou manuellement, voir <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">Présentation de la condition et du type de condition du projet</a></p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Mode horaire</strong> </td> 
      <td> <p>Indiquez si le projet est planifié à partir de la date de début ou de la date de fin. Cette sélection détermine les dates planifiées des tâches du projet. 
       <ul> 
       <li><strong>Date de début</strong>: La première tâche du projet a par défaut la même date de début planifiée que le projet. Pour plus d’informations sur la date de début planifiée de la tâche, voir <a href="../../../manage-work/tasks/task-information/task-planned-start-date.md" class="MCXref xref">Présentation de la tâche Date de début planifiée</a>. La chronologie du projet est calculée à partir de la Date de début et la Date de fin du projet est calculée par le système, en fonction de la durée de toutes les tâches. </li> 
       <li><strong>Date d’achèvement</strong>: La dernière tâche du projet a la même date d’achèvement planifiée que celle du projet. La chronologie du projet est calculée à partir de la date de fin et la date de début du projet est calculée par le système, en soustrayant la durée de toutes les tâches de la date de fin du projet. </li> 
       </ul><p>Votre administrateur Workfront<span> ou un administrateur de groupe</span> sélectionne le paramètre Mode de planification par défaut pour votre système ou votre groupe. Pour plus d’informations sur la définition des paramètres par défaut d’un projet, voir <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configuration des préférences de projet à l’échelle du système</a>.</p></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Date et heure de début planifiées</strong> </td> 
      <td> <p> <p>Indiquez la date à laquelle vous sélectionnez <strong>Planifier à partir de la date de début</strong>. <br></p> <p>Il s’agit d’un champ en lecture seule lorsque vous sélectionnez <strong>Planifier à partir de la date de fin</strong>.<br></p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Date et heure d’achèvement prévues</strong> </td> 
      <td> <p>Indiquez la date à laquelle vous sélectionnez <strong>Planifier à partir de la date de fin</strong>. </p> <p>Il s’agit d’un champ en lecture seule lorsque vous sélectionnez <strong>Planifier à partir de la date de début</strong>.<br></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Portfolio</strong></td> 
      <td>Indique un Portfolio auquel le projet appartient. Vous devez d’abord créer un Portfolio avant qu’il ne s’affiche dans la liste déroulante. Seuls les principaux portefeuilles peuvent être associés à un projet. Pour plus d’informations sur la création de portfolios, voir <a href="../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md" class="MCXref xref">Création d’un portfolio </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Programme</strong></td> 
      <td> <p>Si vous avez sélectionné un Portfolio pour le projet, spécifiez un programme pour le projet. Certains Portfolios peuvent ne pas avoir de programmes. Vous devez d’abord créer un programme avant qu’il n’apparaisse dans cette liste déroulante. Seuls les programmes principaux peuvent être associés à un projet. </p> <p>Pour plus d’informations sur la création de programmes, voir <a href="../../../manage-work/portfolios/create-and-manage-programs/create-program.md" class="MCXref xref">Créer un programme</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Groupe</strong></td> 
      <td> <p> <p>Indiquez le nom du groupe associé au projet. </p>Champ obligatoire. Vous ne pouvez pas avoir de projet qui n’est pas associé à un groupe. </p> <p>Vous pouvez vous assurer que vous sélectionnez le groupe approprié en pointant dessus et en cliquant sur l’icône d’information. <img src="assets/info-icon.png"> qui s’affiche en regard de celle-ci. Une info-bulle s’affiche, répertoriant les informations relatives au groupe, telles que la hiérarchie des groupes au-dessus de celui-ci et ses administrateurs.</p> Par défaut, l’un des groupes suivants est automatiquement associé à un projet lors de sa création, sauf si vous spécifiez un autre groupe :</p> 
       <ul> 
       <li> <p><span>Lorsque le projet est créé à partir de la zone Projets , le groupe d’accueil du créateur du projet est associé au projet.</span> </p> <p>C’est également le cas lorsque le projet est créé à partir de la section Projets d’un portfolio ou d’un programme.</p> </li> 
       <li> <p>Lorsque le projet est créé à partir de la page principale d’un groupe dans la zone Configuration, ce groupe est associé au projet.</p> </li> 
       </ul> </p> <p> <img src="assets/group-details-widget-350x351.png" style="width: 350;height: 351;"> </p> 
       <p><b>NOTES</b></p>

   <ul>
      <li><p>Si le projet, ou ses tâches ou problèmes sont associés à un état personnalisé au niveau du groupe, la modification du groupe du projet peut entraîner la modification de l’état du projet, des tâches ou des problèmes pour qu’il corresponde au nouveau groupe.</p></li>
      <li><p>Si le projet, ou ses tâches ou problèmes sont déjà associés à un processus d’approbation au niveau du groupe à l’aide d’états personnalisés au niveau du groupe, la modification du groupe peut créer un conflit entre les états d’approbation du groupe précédent et ceux existant au niveau du système.</p>
      <p>Envisagez de supprimer les processus d’approbation au niveau du groupe sur le projet, ou ses tâches ou problèmes avant de mettre à jour le groupe.</p>
      <p>Pour plus d’informations sur la création de processus d’approbation au niveau du groupe, voir <a href="../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md" class="MCXref xref">Processus de validation au niveau du groupe</a>.</p>
      <p>Pour plus d’informations sur la création d’un état personnalisé au niveau du groupe, voir <a href="../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md" class="MCXref xref">Création ou modification d’un état de groupe</a></p></li></ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Entreprise</strong> </td> 
      <td> <p>Indiquez une société associée au projet. Vous devez créer une société avant de pouvoir l’associer à un projet. Seules les principales entreprises peuvent être associées à un projet. Pour plus d’informations sur la création d’entreprises, voir <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md" class="MCXref xref">Création et modification d’entreprises</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Propriétaire du projet</strong> </td> 
      <td> <p>Commencez à saisir le nom d’un utilisateur pour l’ajouter au projet, puis sélectionnez-le lorsqu’il s’affiche dans la liste. L’utilisateur est ajouté à l’équipe du projet et se voit attribuer automatiquement les autorisations de gestion du projet. L’utilisateur désigné comme propriétaire du projet doit être un utilisateur principal de Workfront.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Sponsor du projet</strong> </td> 
      <td> <p>Commencez à saisir le nom d’un utilisateur pour l’ajouter au projet, puis sélectionnez-le lorsqu’il s’affiche dans la liste. L’utilisateur est ajouté à l’équipe du projet et se voit attribuer automatiquement les autorisations d’affichage du projet. L’utilisateur désigné comme parrain de projet doit être un utilisateur principal de Workfront.<br></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Gestionnaire des ressources</strong> </td> 
      <td> <p> Commencez à saisir les noms des utilisateurs à ajouter au projet, puis sélectionnez-les lorsqu’ils s’affichent dans la liste. Les utilisateurs sont ajoutés à l’équipe du projet. Ils disposent automatiquement des autorisations de gestion du projet et peuvent affecter des ressources aux tâches et problèmes du projet. Les utilisateurs conservent les autorisations Gérer sur le projet même lorsqu’elles sont supprimées du champ Gestionnaire de ressources . Vous pouvez spécifier plusieurs gestionnaires de ressources.<br></p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Lors de la mise à jour des champs Propriétaire du projet, Parrain du projet et Gestionnaire de ressources, notez l’avatar, le rôle Principal de l’utilisateur ou son adresse électronique pour faire la distinction entre les utilisateurs portant des noms identiques. Les utilisateurs doivent être associés à au moins un rôle de tâche pour l’afficher à mesure que vous les ajoutez.

1. (Facultatif) Continuez à modifier les sections suivantes en fonction des informations que vous souhaitez modifier.

   Ou

   Cliquer sur **Enregistrer**.

### Formulaires personnalisés {#custom-forms}

Selon votre niveau d’accès et votre autorisation sur le projet, les scénarios suivants existent :

* Si vous ne disposez pas des autorisations Modifier le formulaire personnalisé sur le projet, vous ne pouvez pas modifier les champs des formulaires personnalisés joints. Vous ne pouvez afficher que les champs des formulaires personnalisés associés au projet.
* Si vous disposez de l’accès Affichage (et non Modifier) à une section sur un formulaire personnalisé, vous ne pouvez pas modifier les champs de cette section.
* Si vous n’avez pas accès à une section sur l’un des formulaires personnalisés associés au projet, la section ne s’affiche pas dans la zone Modifier le projet .

Lorsque vous sélectionnez plusieurs projets pour les modifier en bloc, les scénarios suivants se présentent :

* Si vous ne disposez pas des autorisations Modifier le formulaire personnalisé pour au moins un des projets sélectionnés, vous ne pouvez pas modifier les champs des formulaires personnalisés joints. Vous ne pouvez afficher que les champs des formulaires personnalisés joints
* Si vous disposez de l’accès Affichage (et non Modifier) à une section sur un formulaire personnalisé, vous ne pouvez pas modifier les champs de cette section. Vous pouvez uniquement afficher les champs de cette section.
* Si vous n’avez pas accès à une section sur l’un des formulaires personnalisés associés à au moins un des projets, la section ne s’affiche pas dans la zone Modifier les projets .

Pour plus d’informations sur l’accès aux formulaires personnalisés, consultez les articles suivants :

* [Partage d’un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md)
* [Ajout d’un saut de section à un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)

Pour modifier les informations sur les formulaires personnalisés :


1. Commencez à modifier votre projet comme décrit ci-dessus.
1. Cliquez sur **Forms personnalisée** dans le panneau de gauche.

   ![](assets/nwe-custom-forms-in-edit-project-box-350x170.png)

1. Cliquez sur le bouton **Ajouter un formulaire personnalisé** et sélectionnez un formulaire dans la liste pour le joindre au projet. Par défaut, les 40 premiers formulaires s’affichent par ordre alphabétique. Si le formulaire ne figure pas dans la liste, commencez à saisir son nom, puis sélectionnez-le lorsqu’il apparaît dans la liste.

   >[!NOTE]
   >
   >Vous devez créer les formulaires personnalisés avant qu’ils ne soient disponibles pour la sélection dans ce champ. Seuls les principaux formulaires personnalisés apparaissent dans la liste. Pour plus d’informations sur la création de formulaires personnalisés, voir [Création ou modification d’un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md). Vous pouvez ajouter jusqu’à dix formulaires personnalisés à un projet.


1. (Conditionnel) Si vous avez joint un formulaire personnalisé au projet, modifiez les champs du formulaire. Vous devez spécifier tous les champs requis avant de pouvoir enregistrer le projet.
1. (Facultatif) Cliquez sur le **Icône X** à droite du nom d’un formulaire personnalisé pour le supprimer, puis cliquez sur **Supprimer**.
1. (Facultatif) Continuez à modifier les sections suivantes, en fonction des informations que vous souhaitez modifier.

   Ou

   Cliquer sur **Enregistrer**.

### Finances {#finance}

Selon votre niveau d’accès et votre autorisation sur le projet, les scénarios suivants existent :

* Si vous disposez des autorisations Afficher les données financières et Afficher le financement sur le projet, vous ne pouvez afficher que les champs de la section Finance. Vous ne pouvez pas modifier les champs de cette section.
* Si vous disposez des autorisations Modifier pour le projet et Gérer les finances , vous pouvez mettre à jour les champs de cette section.

Lorsque vous sélectionnez plusieurs projets pour les modifier en bloc, les scénarios suivants existent :

* Si vous sélectionnez au moins un projet pour lequel vous disposez des autorisations Afficher le financement (au lieu de Gérer les finances), vous ne pouvez afficher que les champs de cette section pour tous les projets sélectionnés. Vous ne pouvez pas modifier les champs en masse dans la section Finance.
* Si vous sélectionnez au moins un projet pour lequel vous ne disposez d’aucune autorisation financière, cette section ne s’affiche pas du tout.

Pour modifier les champs de la zone Finance :


1. Commencez à modifier votre projet comme décrit ci-dessus.
1. Cliquez sur **Finance** dans le panneau de gauche.

   ![](assets/nwe-finance-in-edit-project-box-350x183.png)

1. Mettez à jour les informations financières suivantes pour le projet :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><strong>Devise</strong> </td> 
      <td> <p> <p>Indiquez la devise du projet, si elle est différente de la devise par défaut de votre système. Vous ne pouvez pas modifier la devise d’un projet s’il existe déjà des informations financières sur le projet. Ce champ n’est pas visible si vous avez uniquement la devise par défaut dans le système. </p> <p>Pour plus d’informations sur la devise, voir <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Configurer les taux de change</a>.<br></p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Budget</strong> </td> 
      <td> <p>Spécifiez un budget pour le projet.<br></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Méthode d'indice de performance</strong> </td> 
      <td> <p>Sélectionner <b>Basé sur l’heure</b>ou <b>Basé sur les coûts</b> pour indiquer si les mesures Valeur gagnée du projet (telles que l’indice de performance des coûts ou le coût réel estimé) sont calculées à l’aide des heures ou des coûts. </p> <p>Pour plus d’informations sur la méthode d’index de performance, voir <a href="../../../manage-work/projects/project-finances/set-pim.md" class="MCXref xref">Définition de la méthode d’index de performance (PIM)</a>. </p> <p>Votre administrateur Workfront<span> ou un administrateur de groupe</span> sélectionne le paramètre Méthode d’index de performance par défaut pour votre système ou votre groupe. Pour plus d’informations sur la définition des paramètres par défaut d’un projet, voir <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configuration des préférences de projet à l’échelle du système</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Estimation à l'achèvement</strong> </td> 
      <td> <p> <p>Indiquez comment Workfront doit calculer l’estimation à la fin (EAC). </p>
      Sélectionnez l’une des options suivantes : 
      <ul><li><b>Calculer au niveau du projet</b></li>
      <li><b>Regrouper depuis tâches/sous-tâches</b></li> </ul>
      <p>Pour plus d’informations sur la manière dont l’estimation à la fin est calculée, voir <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref">Calculer l’estimation à la fin (EAC)</a>.</p> <p>Votre administrateur Workfront ou de groupe sélectionne le paramètre par défaut Estimer à la fin pour votre système ou votre groupe. Pour plus d’informations sur la définition des paramètres par défaut d’un projet, voir <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configuration des préférences de projet à l’échelle du système</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Bénéfice prévu</strong> </td> 
      <td> <p>Estimez les avantages prévus du projet. Il est utilisé dans l’analyse de cas du projet et dans Portfolio Optimizer. Pour plus d’informations sur les avantages prévus d’un projet, voir <a href="../../../manage-work/projects/project-finances/project-planned-benefit.md" class="MCXref xref">Aperçu des avantages prévus du projet</a>. L’avantage planifié d’un projet est pris en compte lors du calcul de la valeur nette d’un projet. </p> <p>Pour plus d’informations, voir <a href="../../../manage-work/portfolios/portfolio-optimizer/manage-projects-in-portfolio-optimizer.md" class="MCXref xref">Gestion des projets dans Portfolio Optimizer</a> .<br></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Bénéfice réel</strong> </td> 
      <td> <p>Estimation des avantages réels du projet. Il s’agit d’un montant en devise qui représente l’avantage que votre société ou votre service gagnerait une fois ce projet terminé. </p> </td> 
     </tr> 
      <tr> 
      <td role="rowheader"><strong>Coûts fixes</strong> </td> 
      <td> <p>Indiquez le coût fixe du projet. C'est différent du coût du travail qui provient des heures sur le projet et du coût des dépenses qui provient du montant des dépenses sur le projet. Le coût fixe d'un projet est pris en compte dans le calcul de la valeur nette d'un projet et fait partie du coût budgété.<br></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Revenus fixes</strong> </td> 
      <td> <p>Indiquez les recettes fixes du projet.<br></p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Facultatif) Continuez à modifier les sections suivantes en fonction des informations que vous souhaitez modifier.

   Ou

   Cliquer sur **Enregistrer**.

### Paramètres du projet {#project-settings}

1. Commencez à modifier votre projet comme décrit ci-dessus.
1. Cliquez sur **Paramètres du projet** dans le panneau de gauche.

   ![](assets/nwe-project-settings-in-edit-project-box-350x380.png)

1. Mettez à jour les informations suivantes :

   <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
      <tr> 
      <td role="rowheader"><strong>Chemin jalonné</strong> </td> 
       <td> <p>Sélectionnez un chemin Milestone pour le projet. Seuls les principaux chemins de jalon s’affichent dans la liste.</p> <p>Pour plus d’informations sur les chemins d’accès Milestone, voir <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md" class="MCXref xref">Création d’un chemin de jalon</a>.</p> </td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>Mode d'achèvement</strong> </td> 
      <td> <p>Contrôle la manière dont le projet est marqué comme terminé. Sélectionnez l’une des options suivantes : 
       <ul> 
       <li><p><strong>Automatique</strong>: Le projet est marqué Terminé lorsque toutes les tâches et tous les problèmes sont terminés.</p><p>L’état du projet est automatiquement modifié en Terminé uniquement lorsque l’état du projet est Actuel lorsque les tâches sont terminées. </p></li> 
       <li><strong>Manuel</strong>: Vous devez sélectionner manuellement l’état Terminé du projet, une fois toutes les tâches et tous les problèmes terminés.</li> 
       </ul></p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader"><strong>Mode d'achèvement du sommaire</strong></td> 
       <td> <p>Contrôle la manière dont les tâches parents sont marquées comme étant terminées. Sélectionnez l’une des options suivantes : 
       <ul> 
       <li><strong>Automatique</strong>: Les tâches parentes sont marquées comme Terminé et elles mettent à jour leur pourcentage automatiquement, à mesure que les tâches enfants sont terminées et que le pourcentage d’enfants terminés est mis à jour. </li> 
       <li><strong>Manuel</strong>: Vous devez mettre à jour manuellement le pourcentage terminé et l’état des tâches parents, indépendamment des modifications apportées aux tâches enfants.</li> 
       </ul></p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader"><strong>Type de mise à jour</strong></td> 
       <td> <p>Contrôle le moment où les modifications que vous apportez à la chronologie du projet sont enregistrées dans le projet ou les tâches parents. Par exemple, les modifications suivantes apportées au projet déclenchent une mise à jour de la chronologie du projet : 
       <ul> 
       <li>Mise à jour des dates des tâches</li> 
       <li>Modifier les relations de prédécesseur des tâches</li> 
       <li><p>Modifiez les relations parent-enfant, en ajoutant ou en supprimant des affectations, en plus de modifier la contrainte de tâche ou le type de durée.</p><p>Lorsque les tâches sont mises à jour, leurs objets parents (tâches parents ou projet) sont mis à jour au moment indiqué par le Type de mise à jour. </p><p>Si les objets parents ne se mettent pas à jour immédiatement après la modification lors de la sélection de l’option Type de mise à jour "Automatique et En cas de modification" ou "Modifier uniquement", actualisez la page.</p><p>Sélectionnez l’une des options suivantes : </p><p>- <strong>Automatique et Activé</strong> (Paramètre par défaut) : La chronologie du projet est mise à jour chaque fois qu’une modification se produit dans le projet ou dans un autre projet dont le projet dépend (En cas de modification). La chronologie du projet est également mise à jour chaque nuit (automatique).</p><p>Il s’agit du paramètre recommandé pour ce champ, car il garantit que le projet est toujours à jour.</p><p>Lorsque vous effectuez une action sur une tâche ou un projet qui déclenche un nouveau calcul de frise chronologique, toutes les dates disponibles sont immédiatement affichées, ce qui vous permet de continuer à travailler. Sur les projets comportant plus de 100 tâches, les dates nécessitant des nouveaux calculs plus longs s’affichent brièvement comme point d’interrogation (entre 1 et 5 secondes, ou jusqu’à une minute pour les projets volumineux). Cela indique que le recalcul n'est pas encore terminé et que les dates peuvent être modifiées.</p><p>- <strong>Modifier uniquement</strong>: La chronologie du projet est mise à jour chaque fois qu’une modification se produit dans le projet ou dans un autre projet dont le projet dépend. Vous pouvez sélectionner cette option si des modifications se produisent rarement dans le projet ou dans d’autres projets dont dépend la chronologie.</p><p>- <strong>Automatique uniquement</strong>: La chronologie du projet est actualisée chaque nuit. la frise chronologique n’est pas mise à jour immédiatement après les modifications.</p><p>Vous pouvez sélectionner cette option si de nombreuses modifications se produisent chaque jour dans le projet ou dans d’autres projets dont dépend la chronologie. Sachez toutefois que vous avez choisi ce paramètre, car le projet ne se mettra pas à jour en même temps que les modifications sont effectuées.</p><p>- <strong>Manuel uniquement</strong>: La chronologie du projet n’est mise à jour que si vous sélectionnez l’option permettant de recalculer la chronologie. Pour plus d’informations sur le nouveau calcul manuel de la chronologie du projet, voir <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">Recalculer les calendriers du projet</a>. </p><p>Vous pouvez sélectionner cette option si vous apportez simultanément de nombreuses modifications au projet et si vous souhaitez que le recalcul de la chronologie se produise une fois toutes les modifications effectuées (plutôt qu’après chaque modification individuelle).</p></li> 
       </ul></p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader"><strong>Planification</strong> </td> 
       <td> <p>Sélectionnez un planning pour votre projet. Il doit s’agir du même planning que celui attribué à la plupart des personnes qui travaillent sur le projet. Vous devez créer un planning avant de pouvoir l’affecter à un projet ou à un utilisateur. Si vous n’avez pas créé de plannings personnalisés dans votre système, la planification par défaut est sélectionnée.</p> <p>Pour plus d’informations sur la création de plannings, voir <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Création d’un planning</a>. </p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader"><strong>Congés de l'utilisateur</strong> </td> 
       <td> <p>Détermine si le délai de désactivation du cessionnaire Principal d’une tâche ajuste les dates planifiées de la tâche sur le projet. </p><p>Votre administrateur Workfront<span> ou un administrateur de groupe</span> sélectionne la valeur par défaut de ce paramètre pour votre système. <span>ou votre groupe</span>. Pour plus d’informations sur la définition des paramètres par défaut d’un projet, voir <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configuration des préférences de projet à l’échelle du système</a>. </p><p>Sélectionnez l’une des options suivantes :<br>- <strong>Tenir compte du temps d’arrêt de l’utilisateur dans les durées de tâche</strong>: Lorsque vous sélectionnez cette option, les dates planifiées des tâches s’ajustent en fonction de l’heure de désactivation de la personne désignée Principal de la tâche, si l’heure de désactivation a lieu pendant la durée de la tâche. </p><p>Par exemple, si une tâche avec une contrainte de la date Dès que possible doit commencer le 1er juin et se terminer le 3 juin, et que la personne désignée Principal a le 2 juin marqué comme étant en pause, lorsque cette sélection est activée, les dates prévues de la tâche sont comprises entre le 1er et le 4 juin. Selon la contrainte de tâche, les scénarios suivants existent : </p> 
       <ul> 
       <li>Pour les contraintes de tâche liées à la planification à partir d’une date de début (dès que possible, l’heure disponible la plus tôt, le début le plus tôt possible, le début le plus tard, le début le plus tard), la date de début planifiée ne change pas, mais la date de fin planifiée change.</li> 
       <li>Pour les contraintes de tâche liées à la planification à partir d’une date d’achèvement (Aussi tard que possible, heure disponible la plus récente, Terminer au plus tôt, Terminer au plus tard, Doit se terminer le), la date d’achèvement planifiée ne change pas, mais la date de début planifiée change.</li> 
       <li>Pour les tâches avec une contrainte de dates fixes, ni la date de début planifiée ni la date de fin ne changent. </li> 
       </ul><p>La Durée de la tâche ne change pas lorsque vous sélectionnez ce paramètre. Seules les dates planifiées changent, en fonction de la contrainte de tâche. Pour plus d’informations sur la contrainte de tâche, voir <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Présentation de la contrainte de tâche</a>. </p><p>- <strong>Ignorer le temps d’arrêt des utilisateurs dans les durées de tâche</strong>: Lorsque vous sélectionnez cette option, les dates planifiées des tâches du projet restent telles que prévues initialement, même si le cessionnaire Principal de la tâche a expiré pendant la durée de la tâche. </p><p>Tenez compte des points suivants lors de la sélection des options de ce paramètre :</p> 
       <ul> 
       <li><p>L’option par défaut de ce paramètre pour un nouveau projet est identique à la préférence de projet au niveau du système. </p><p>Pour plus d’informations sur les préférences du projet au niveau du système, voir <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configuration des préférences de projet à l’échelle du système</a>. </p></li> 
       <li>Lorsque vous joignez un modèle à un projet existant, le paramètre du projet est mis à jour pour correspondre à celui du modèle. </li> 
       <li><p>Workfront décide des dates de tâche planifiées à ajuster en fonction de la valeur Contrainte de tâche de la tâche. En fonction de ce qui se passe, le début planifié ou la date d’achèvement prévu, ou les deux, peuvent être affectés, ou peuvent même rester identiques. Par exemple, si une tâche présente une contrainte de dates fixes, les dates ne s’ajustent pas lorsque le cessionnaire Principal a un délai d’expiration, même lorsque <strong>Tenir compte du temps d’arrêt de l’utilisateur dans les durées de tâche</strong> est sélectionnée. </p></li> 
       </ul></td> 
      </tr> 
      <tr> 
       <td role="rowheader"><strong>Mode de nivellement des ressources</strong> </td> 
       <td> <p> <p>Sélectionnez l’une des options suivantes :</p> <p>- <strong>Manuel</strong>: vous devez mettre à niveau manuellement vos ressources (il s’agit du paramètre par défaut).</p> <p>- <strong>Automatique</strong>: Workfront met à niveau vos ressources.</p> <p>Pour plus d’informations sur le niveau de ressource, voir <a href="../../../manage-work/gantt-chart/use-the-gantt-chart/level-resources-in-gantt.md" class="MCXref xref">Ressources de niveau dans le diagramme de Gantt </a>.</p> </p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"><strong>Risque</strong> </td> 
       <td> <p> <p>Définissez le niveau de risque de votre projet. Le risque n'est qu'un indicateur des risques que peut représenter un projet. Vous pouvez hiérarchiser l’exécution de vos projets en fonction du niveau de risque.</p> <p> <p>Envisagez de choisir parmi les niveaux de risque suivants :</p> <p>- Très faible</p> <p>- Faible</p> <p>- Moyen</p> <p>- Élevé</p> <p>- Très élevé</p> <p>Les niveaux de risques que vous indiquez ici ne peuvent pas être personnalisés.</p> <p>Elles ne sont pas liées aux risques potentiels qui peuvent se produire pendant la durée d’un projet et que vous devez enregistrer dans l’onglet Risques du projet, ou dans l’Analyse de cas. Pour plus d’informations sur les risques potentiels du projet, voir <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/edit-create-risk-types.md" class="MCXref xref">Modifier et créer des types de risque</a>. </p> </p> </p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"><strong>Pools de ressources</strong> </td> 
       <td> <p> <p>Spécifiez les groupes de ressources associés au projet. Les groupes de ressources sont des groupes d’utilisateurs qui sont nécessaires en même temps pour la fin d’un projet et qui permettent la planification du projet dans le planificateur de ressources. Pour plus d’informations sur les pools de ressources, voir <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Présentation des pools de ressources </a>. </p> <p>Lorsque vous modifiez des projets en bloc, seuls les groupes de ressources communs à tous les projets sélectionnés s’affichent dans ce champ. Si les projets sélectionnés n’ont aucun pool de ressources partagé, ce champ est vide. Les pools de ressources que vous spécifiez ici remplaceront les pools de ressources individuels des projets.</p> </p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <strong>Autoriser le remplacement des taux de facturation au niveau du projet par des taux de facturation au niveau de l'entreprise</strong></td> 
       <td>Sélectionnez cette option pour permettre aux taux de facturation au niveau de l’entreprise de remplacer les taux historiques des rôles de tâche, sauf si ces taux sont marqués comme facturés. L’activation de cette option remplace les taux de rôle de tâche historiques à moins qu’ils ne soient marqués comme facturés. <br>Pour plus d’informations, voir <a href="../../../manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md" class="MCXref xref">Remplacer les taux de facturation au niveau du projet par les taux de facturation au niveau de l’entreprise</a>.</td> 
      </tr> 
      <tr> 
       <td role="rowheader"><strong>L'approbation pour ce projet demande du temps</strong></td> 
       <td> <p> Sélectionnez cette option pour exiger du propriétaire du projet qu’il approuve l’heure de connexion au projet. Si vous utilisez des enregistrements de facturation et que vous sélectionnez cette option, seules les heures approuvées sur le projet apparaissent comme des heures facturables disponibles pour les enregistrements de facturation. La validation du temps sur le projet est indépendante de la validation des feuilles de temps. </p> <p>Pour plus d’informations sur le temps nécessaire à l’approbation d’un projet, voir <a href="../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md" class="MCXref xref">Requiert du temps pour approuver un projet</a>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"><strong>Filtrer les types d’heure</strong> et</span> <strong>Types d’heure</strong></td> 
       <td> <p> <p>Sélectionnez l’une des options suivantes :</p> 
       <ul> 
       <li> <p>Sélectionner <strong>Non</strong> pour rendre tous les types d’heures spécifiques au projet disponibles sur le projet. (Il s’agit de la sélection par défaut)</p> <p>Ou</p> </li> 
       <li>Sélectionner <strong>Oui</strong> pour rendre disponible uniquement un sous-ensemble des types d’heures spécifiques au projet, sélectionnez les types d’heures à rendre disponibles. (Maintenez la touche Maj enfoncée pour sélectionner plusieurs types d’heures.)</li> 
       <p>Si vous sélectionnez cette option, seuls les types d’heures que vous sélectionnez sont disponibles lors de la journalisation des heures sur le projet (ou sur les tâches et problèmes dans le projet). Vous devez sélectionner au moins une heure ; si vous sélectionnez cette option et que vous ne sélectionnez aucun type d’heure, tous les types d’heure sont disponibles sur le projet.</p> </ul>

   <p>Les mêmes sélections de type heure doivent être effectuées au niveau de chaque utilisateur pour que l’utilisateur puisse voir ces options de type heure sur le projet. Pour plus d’informations sur la définition des types d’heures au niveau de l’utilisateur, voir <a href="../../../timesheets/create-and-manage-timesheets/log-time.md" class="MCXref xref">Temps de connexion</a>. </p> </p> </td> 
      </tr> 
      <tr data-mc-conditions=""> 
       <td role="rowheader"><strong>Notification de rappel</strong> </td> 
       <td> <p> <p>Sélectionnez la notification de rappel à associer au projet. Pour que ce champ s’affiche lors de la modification d’un projet, vous devez configurer les notifications de rappel pour les projets. Pour plus d’informations sur la configuration des notifications de rappel, voir <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md"><a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">Configuration des notifications de rappel</a> .</a></p> </p> </td> 
      </tr> 
      <tr data-mc-conditions=""> 
       <td role="rowheader"><strong>Processus d'approbation</strong></td> 
       <td> <p>Sélectionnez le processus d’approbation à associer au projet. Votre administrateur Workfront doit définir des processus d’approbation au niveau du système avant de pouvoir les associer aux projets. <span>Un utilisateur disposant d’un accès administratif aux processus de validation peut également créer des processus de validation spécifiques à un groupe.</span> Pour plus d’informations sur la création de processus de validation, voir <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Créer un processus d’approbation pour les tâches</a>.</p> <p>Tenez compte des points suivants lors de l’ajout de processus de validation : </p> 
       <ul> 
       <li>Seuls les principaux processus de validation s'affichent dans la liste. </li> 
       <li> <p>Les processus de validation à l’échelle du système et spécifiques aux groupes s’affichent dans la liste. Un processus de validation associé à un groupe autre que celui du projet ne s’affiche pas dans la liste.</p> <p>Si le groupe associé au projet change, le processus d’approbation spécifique au groupe devient un processus d’approbation à usage unique. Pour plus d’informations sur la façon dont les modifications apportées au groupe du projet ou au processus d’approbation affectent les paramètres d’approbation, voir <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">Comment les modifications du processus d’approbation et de groupe affectent-elles les processus d’approbation affectés ?</a>. </p> </li> <!--(NOTE: this bullet stays here although the sections it might appear in are QS only, so we can use the snippet for both Qs and classic)-->
       <p>Lors de la modification en masse de projets, les scénarios suivants se présentent :</p> 
       <ul> 
       <li> <p>Lorsque vous sélectionnez des projets du même groupe, les processus de validation au niveau du système et du groupe s’affichent dans ce champ.</p> </li> 
       <li> <p>Lorsque vous sélectionnez des projets issus de différents groupes, seuls les processus de validation au niveau du système s’affichent dans ce champ.</p> </li> 
       <li> <p>Lorsque l’un des projets est associé à un processus de validation à usage unique, celui-ci est remplacé par le processus d’approbation au niveau du système ou du groupe que vous sélectionnez. </p> </li> 
      </ul> </td> 
      </tr> 
      <tr> 
      </tr> 
      </tbody> 
      </table>

1. (Facultatif) Continuez à modifier les sections suivantes en fonction des informations que vous souhaitez modifier.

   Ou

   Cliquer sur **Enregistrer**.

### Paramètres de la tâche {#task-settings}

Vous pouvez définir les valeurs par défaut qui seront associées à toutes les nouvelles tâches lorsque vous les ajoutez au projet.

Pour plus d’informations sur l’impact de ces paramètres sur la création de nouvelles tâches, voir la section [Tâche par défaut lors de l’ajout de tâches à un projet](../../../manage-work/tasks/create-tasks/create-tasks-overview.md#understa) dans l’article [Présentation de la création de tâches](../../../manage-work/tasks/create-tasks/create-tasks-overview.md).

1. Commencez à modifier votre projet comme décrit ci-dessus.
1. Cliquez sur **Paramètres de tâche** dans le panneau de gauche.

   ![](assets/nwe-task-settings-in-edit-project-box-350x211.png)

1. Dans le **Processus d’approbation par défaut de la tâche** sélectionnez la tâche Processus d’approbation que vous souhaitez associer à toutes les nouvelles tâches lorsque vous les ajoutez au projet.

   L’administrateur de Workfront (ou un utilisateur disposant d’un accès administratif aux processus de validation) doit créer un processus d’approbation au niveau du système pour une tâche avant de pouvoir l’associer à un projet. Seuls les principaux processus de validation s&#39;affichent dans la liste. Pour plus d’informations sur la création de processus de validation, voir [Créer un processus d’approbation pour les tâches](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md). Pour plus d’informations sur la façon dont les modifications apportées au groupe du projet ou au processus d’approbation affectent les paramètres d’approbation, voir [Comment les modifications du processus d’approbation et de groupe affectent-elles les processus d’approbation affectés ?](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md).

   Lors de la modification en masse de projets, les scénarios suivants se présentent :

   * Lorsque vous sélectionnez plusieurs projets d’un même groupe, les processus d’approbation des tâches au niveau du système et spécifiques au groupe s’affichent dans ce champ.
   * Lorsque vous sélectionnez plusieurs projets de différents groupes, seuls les processus d’approbation des tâches au niveau du système s’affichent dans ce champ.

1. Dans le **Task Default Custom Forms** sélectionnez le ou les formulaires personnalisés à associer à toutes les nouvelles tâches lorsque vous les ajoutez au projet. Vous devez créer les formulaires personnalisés avant qu’ils ne soient disponibles pour la sélection dans ce champ. Seuls les principaux formulaires personnalisés s’affichent dans la liste. Pour plus d’informations sur la création de formulaires personnalisés, voir [Création ou modification d’un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md). Vous pouvez associer jusqu’à dix formulaires personnalisés à une tâche.
1. (Facultatif) Sélectionnez **Utiliser l’effort de travail pour calculer automatiquement les heures planifiées de la tâche** si vous souhaitez activer la gestion de l’effort de tâche à l’aide de l’effort de travail au lieu des heures planifiées.

   ![](assets/nwe-work-effort-on-projects-350x182.png)

1. (Conditionnel et facultatif) Si vous avez sélectionné Utiliser l’effort de travail pour calculer automatiquement les heures planifiées de la tâche, cliquez sur le menu déroulant pour chaque niveau d’effort et sélectionnez un pourcentage pour chaque niveau. Les valeurs en pourcentage suivantes sont des valeurs par défaut :

   | Taille | Pourcentage |
   |---|---|
   | Petite | 25% |
   | Moyen | 50% |
   | Grande | 75% |

   >[!TIP]
   >
   >Lorsque le type de mise à jour du projet est défini sur Automatique et que vous sélectionnez ce paramètre, les Heures planifiées des tâches sont mises à jour en fonction de la durée de la tâche et du pourcentage de l’effort de travail, si elles sont définies sur zéro. Pour plus d’informations sur l’utilisation de l’effort de travail pour planifier l’effort d’une tâche, voir [Présentation de l’effort de travail](../../../manage-work/tasks/task-information/work-effort.md).

1. (Facultatif) Continuez à modifier les sections suivantes en fonction des informations que vous souhaitez modifier.

   Ou

   Cliquer sur **Enregistrer**.

### Paramètres de l&#39;événement {#issue-settings}

1. Commencez à modifier votre projet comme décrit ci-dessus.
1. Cliquez sur **Paramètres de problème** dans le panneau de gauche.

   ![](assets/nwe-issue-settings-in-edit-project-box-350x306.png)

1. (Facultatif) Désélectionnez l’option **Autoriser les utilisateurs à ajouter des problèmes en ligne** . Il est sélectionné par défaut.

   Lorsque vous désélectionnez cette option, les utilisateurs ne peuvent pas ajouter de problèmes en ligne au projet ou aux tâches dans la section Problèmes .

   >[!TIP]
   >
   >Désélectionnez cette option si vous souhaitez obliger les utilisateurs à remplir les champs New Issue Fields ou les formulaires personnalisés associés aux nouveaux problèmes. L’activation de la saisie de problèmes en ligne permet aux utilisateurs de contourner les champs Nouveau problème et les formulaires personnalisés lors de la création de problèmes. Pour plus d’informations sur la définition des champs et des formulaires personnalisés pour de nouveaux problèmes, voir [Création d’une file d’attente de requête](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

   Lorsque vous désélectionnez cette option, les utilisateurs autorisés à ajouter des problèmes au projet ou aux tâches peuvent le faire comme suit :

   * Cliquez sur Nouveau problème en haut de la liste des problèmes dans la section Problèmes du projet ou des tâches.
   * Lorsque le projet est configuré en tant que file d’attente des demandes, il peut saisir une nouvelle demande dans la zone Demandes .

   >[!NOTE]
   >
   >Lorsque vous modifiez des projets en bloc, ce paramètre est activé si au moins un projet est activé et s’il est désactivé si tous les projets sélectionnés sont désactivés.

   <!--drafted for bulk edit projects: the statement above needs to be corrected when the new UI for bulk edit projects is updated; not sure if we'll need to describe this at all or we can cover this in  a "Considerations" mini section inside the Editing in bulk section below- ??? -->

1. (Facultatif) Continuez à modifier les sections suivantes en fonction des informations que vous souhaitez modifier.

   Ou

   Cliquer sur **Enregistrer**.

### Accès {#access}

1. Commencez à modifier votre projet comme décrit ci-dessus.
1. Cliquez sur **Accès** dans le panneau de gauche.

   ![](assets/nwe-access-in-edit-project-box-350x262.png)

1. Spécifiez les **Accès** informations relatives au projet :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><strong>Lorsqu’une personne est affectée à une tâche</strong></td> 
      <td><p>Sélectionner parmi <strong>Affichage</strong>, <strong>Contribuez,</strong> ou <strong>Gérer</strong> accès à une tâche. L’utilisateur affecté à une tâche se voit automatiquement octroyer cet accès à la tâche.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><strong>Accordez également l’accès au projet</strong></td> 
      <td><p>Sélectionner parmi <strong>Affichage</strong>, <strong>Contribution</strong>ou <strong>Gérer</strong> accès au projet. L’utilisateur affecté à une tâche se voit également automatiquement octroyer cet accès au projet.<br></p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><strong>Lorsqu’une personne est affectée à un problème</strong></td> 
      <td><p>Sélectionner parmi <strong>Affichage</strong>, <strong>Contribuez,</strong> ou <strong>Gérer</strong> accès à un problème. L’utilisateur affecté à un problème se voit automatiquement octroyer cet accès au problème. Pour plus d’informations, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Partage d’un problème </a>.<br></p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><strong>Accordez également l’accès au projet</strong></td> 
      <td><p>Sélectionner parmi <strong>Affichage</strong>, <strong>Contribution</strong>ou <strong>Gérer</strong> accès au projet. L’utilisateur affecté à un problème se voit également automatiquement octroyer cet accès au projet.<br></p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><strong>Lorsqu’une personne envoie une demande : Accorder leur accès</strong></td> 
      <td><p>Sélectionner parmi <strong>Affichage</strong>, <strong>Contribution</strong>ou <strong>Gérer</strong> accès à la requête. Lorsque le projet est également une file d’attente de demandes et qu’un utilisateur envoie une demande au projet, il se voit accorder cet accès à la demande qu’il a envoyée. Pour plus d’informations sur la configuration d’un projet en tant que file d’attente de requêtes, voir <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Création d’une file d’attente de requête</a>.<br></p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><strong>Les personnes appartenant à la même entreprise hériteront d'autorisations identiques pour toutes les demandes</strong></td> 
      <td><p>Sélectionnez ce champ si vous souhaitez que les personnes de la même société aient le même accès à toutes les demandes du projet, qu’elles les aient soumises ou non.<br></p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Lorsqu’une personne a accès à ce projet : Donnez-leur accès à ...</strong></td> 
      <td><p>Sélectionnez les options d’accès que vous souhaitez que les utilisateurs disposent sur le projet, si le projet est partagé avec eux. Sélectionnez les options d’accès spécifiques si elles sont désignées comme <strong>Visionneuses</strong>, <strong>Contributeurs</strong>ou <strong>Chefs</strong> lors du partage du projet avec eux. </p><p>Le <strong>Supprimer</strong> dans le <strong>Gérer</strong> le niveau d’autorisation détermine si les utilisateurs peuvent supprimer le projet lui-même. Utilisateurs avec <strong>Gérer</strong> l’accès au projet peut supprimer des tâches et des problèmes au sein du projet, que cette option soit sélectionnée ou non, s’ils disposent de <strong>Gérer</strong> autorisations pour les tâches et les problèmes. </p></td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquer sur **Enregistrer**.

## Modification d’un projet dans l’en-tête du projet (limitée)

Vous pouvez modifier un nombre limité d’informations dans l’en-tête du projet.

L’administrateur du système ou du groupe peut personnaliser les champs affichés dans l’en-tête du projet.

![](assets/project-header-350x18.png)

Par défaut, les champs suivants sont inclus dans l’en-tête du projet.

* Nom du projet
* Propriétaire du projet
* Date et heure d’achèvement prévues

   >[!NOTE]
   >
   >Vous ne pouvez modifier ce champ que lorsque le projet est planifié à partir de la date de fin. Lorsque le projet est planifié à partir de la date de début, Workfront calcule la date et l’heure de fin planifiées en fonction de la durée des tâches.

* Condition

   >[!NOTE]
   >
   >Vous ne pouvez modifier ce champ que lorsque le type de condition du projet est Manuel. Lorsque le type de condition est défini sur Etat de progression, Workfront calcule la condition en fonction de l’état d’avancement des tâches. Pour plus d’informations, voir [Présentation de la condition et du type de condition du projet](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

* Statut
* Prenez des décisions d’approbation si vous êtes défini comme approbateur dans un processus d’approbation actuel.

## Modifier des projets en bloc

Vous pouvez modifier des projets en bloc et mettre à jour les informations de tous les projets sélectionnés en même temps.


Les informations que vous modifiez sur tous les projets sélectionnés remplacent les informations existantes sur les projets individuels, à l’exception du champ Gestionnaire de ressources .

L’ajout d’un nouveau gestionnaire de ressources lors de la modification de projets en bloc ajoute ce gestionnaire à tous les projets sélectionnés. Si d’autres gestionnaires de ressources sont associés aux projets sélectionnés, ils restent sur les projets en plus de celui ajouté par modification en masse.

La modification en bloc de projets varie en fonction de l’environnement dans lequel vous choisissez de les mettre à jour.

### Modifier des projets en bloc dans l’environnement de production

Pour modifier des projets en bloc :

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront.

1. Cliquez sur **Projets**.
1. Sélectionnez plusieurs projets dans la liste.
1. Cliquez sur **Modifier**.

   Le **Modifier des projets** s’ouvre.

   ![](assets/edit-projects-in-bulk-nwe-350x303.png)

1. Renseignez les sections suivantes pour tous les projets sélectionnés :

   * **Vue d’ensemble**

      Pour plus d’informations, voir [Présentation](#overview) dans cet article.

   * **Finances**

      Pour plus d’informations, voir [Finance](#finance) dans cet article.

   * **Portfolio**

      Pour plus d’informations, reportez-vous à la section &quot;Association de projet&quot; dans la section [Présentation](#overview) dans cet article.

   * **Paramètres**

      Pour plus d’informations, voir [Paramètres du projet](#project-settings) dans cet article.

   * **Accès**

      Pour plus d’informations, voir [Accès](#access) dans cet article.

   * **Formulaires personnalisés**

      Pour plus d’informations, passez à l’étape 7 ci-dessous.

      <!--   
     <p>(NOTE:&nbsp;make sure this stays accurate)</p>   
     -->

   * **Tâches**

      Pour plus d’informations, voir [Paramètres de tâche](#task-settings) dans cet article.

   * **Événements**

      Pour plus d’informations, voir   [Paramètres de problème](#issue-settings) dans cet article.

   * **Commentaire**

      Pour plus d’informations, reportez-vous à l’étape 9 ci-dessous.

      <!--   
     <p>(NOTE: ensure this step stays accurate)</p>   
     -->


1. (Facultatif) Dans la zone Paramètres, sélectionnez l’une des options suivantes :

   * **Recalculer les coûts et les recettes**: Sélectionnez cette option pour recalculer les coûts et les recettes sur tous les projets sélectionnés.
   * **Recalculer les chronologies**: Sélectionnez cette option pour recalculer les Chronologies de tous les projets sélectionnés.
   * **Recalculer les Fiches d’évaluation**: Sélectionnez cette option pour recalculer les valeurs de la Fiche d’évaluation pour tous les projets sélectionnés.

   ![recalculate_cost__scorecards__etc_in_bulk_edit_for_projects.PNG](assets/recalculate-costs--scorecards--etc-in-bulk-edit-for-projects-350x225.png)

1. Cliquez sur **Forms personnalisée** pour modifier les formulaires personnalisés joints à tous les projets sélectionnés.

   Si les projets sélectionnés ne comportent aucun formulaire personnalisé commun, aucun formulaire n’est répertorié dans cette section.

   Vous ne pouvez modifier que les champs des formulaires associés à tous les projets sélectionnés et que vous êtes autorisé à modifier.

1. (Facultatif) Dans la section Forms personnalisée , sélectionnez la variable **Recalculer des expressions personnalisées** pour vous assurer que tous les champs personnalisés calculés qui se trouvent sur le Forms personnalisé joint aux projets sélectionnés sont à jour.

   >[!IMPORTANT]
   >
   >Il est recommandé de ne pas sélectionner plus de 500 projets à la fois lorsque vous recalculez les expressions personnalisées.

1. (Facultatif) Cliquez sur **Commentaire**, sélectionnez ensuite la zone Publier une mise à jour pour chaque projet et indiquez un commentaire à afficher dans le flux de mises à jour du projet dans le champ disponible, puis effectuez l’une des opérations suivantes :

   * Cliquez sur le bouton **Personnes** icon ![](assets/people-icon-updates-classic.png) pour baliser un utilisateur qui sera informé de votre commentaire.
   * Cliquez sur le bouton **Verrouiller** icon ![](assets/lock-icon-open-updates-classic.png) pour limiter vos commentaires aux seuls membres de votre société.

   Ce commentaire est visible pour toutes les personnes ayant accès à l’affichage du projet et ayant accès à l’affichage des notes.

1. Cliquez sur **Enregistrer les modifications**.

   Toutes les modifications que vous avez apportées sont désormais visibles sur tous les projets sélectionnés.

<div class="preview">

### Modification de projets en bloc dans l’environnement Aperçu

Tenez compte des points suivants lors de la modification de projets en bloc dans l’environnement Aperçu :

* Lorsque vous sélectionnez des projets dont les valeurs sont différentes pour le même champ, le champ affiche un indicateur &quot;Plusieurs valeurs&quot; dans la zone Modifier les projets . Les champs qui sont des cases à cocher, des boutons radio et des bascules sont associés à un indicateur &quot;Plusieurs valeurs&quot;.

   ![](assets/multiple-values-indicator-dates-bulk-edit-projects.png)

* Outre l&#39;indicateur &quot;Valeurs multiples&quot;, lorsque les options sélectionnées sont différentes sur au moins un des projets sélectionnés, les champs comportant plusieurs options s&#39;affichent de l&#39;une des manières suivantes :

   * Les champs de case à cocher comportent une ligne au lieu d’une case à cocher pour l’option qui est cochée pour certains projets, mais pas pour tous les projets sélectionnés.

      ![](assets/multiple-values-indicator-check-boxes-bulk-edit-projects.png)

   * Les champs de type Bascule s’affichent en grisé avec le bouton activer/désactiver au milieu pour l’option activée pour certains projets sélectionnés, mais pas pour tous.

   ![](assets/multiple-values-highlighted-bulk-edit-projects.png)

   * Les champs de type Bouton radio dont certaines options sont sélectionnées mais pas toutes affichent tous les boutons radio vides.

      ![](assets/multiple-values-indicator-radio-buttons-bulk-edit-projects.png)


* Lorsque vous mettez à jour une option dans un champ à plusieurs options (un champ qui s’affiche sous la forme d’un ensemble de bascules ou de cases à cocher, par exemple), toutes les autres options doivent correspondre entre les projets sélectionnés.

   >[!IMPORTANT]
   >
   >Par exemple, vous pouvez avoir un champ de case à cocher comportant trois cases à cocher (Option 1, Option 2 et Option 3) et l’option 1 n’est pas cochée pour tous les projets, tandis que les options 2 et 3 sont cochées pour certains projets et décochées pour les autres que vous avez sélectionnés. Si vous souhaitez cocher l’option 1 pour tous les projets, vous devez également faire correspondre les options 2 et 3 pour tous les projets sélectionnés avant de pouvoir enregistrer vos modifications. Vous devez donc les sélectionner ou les désélectionner afin qu’ils puissent correspondre à tous les projets sélectionnés. Si vous ne modifiez aucune des options, vous pouvez enregistrer le champ tel quel et les projets conservent leur sélection actuelle pour toutes les options.

* Lorsque vous sélectionnez plusieurs projets appartenant à différents groupes, les états qui s’affichent dans le champ Statut sont des états au niveau du système et non des états au niveau du groupe.

Pour modifier des projets dans l’environnement Aperçu :

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront.
1. Cliquez sur **Projets**.
1. Sélectionnez plusieurs projets dans la liste.
1. Cliquez sur le bouton **Modifier** icon ![](assets/edit-icon.png) en haut de la liste.
Le **Modifier des projets** s’ouvre.

   ![](assets/edit-projects-in-bulk-modal-unshimmed.png)

Selon la manière dont votre administrateur Workfront ou l’administrateur de groupe a modifié votre modèle de mise en page, les zones du panneau de gauche de la boîte de dialogue Modifier le projet ou les champs répertoriés dans ces zones peuvent être réorganisées ou ne pas s’afficher. Pour plus d’informations, voir [Personnalisation de la vue Détails à l’aide d’un modèle de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

1. Cliquez sur **Présentation** pour modifier des informations générales sur les projets sélectionnés.  Pour plus d’informations sur la modification de la zone Aperçu, voir la section [Présentation](#overview) dans cet article.

   >[!TIP]
   >
   >Les champs que vous modifiez s’affichent avec un arrière-plan clair violet.

1. Cliquez sur **Forms personnalisée** pour modifier, ajouter ou remplacer des formulaires personnalisés associés aux projets sélectionnés.

   Les formulaires personnalisés joints à tous les projets sélectionnés s’affichent dans la variable **Formulaires personnalisés en commun** dans la section **Forms personnalisée** zone.

   ![](assets/custom-forms-in-common-unshimmed.png)

   >[!TIP]
   >
   >   Les noms des formulaires communs à tous les projets sélectionnés s’affichent dans le panneau de gauche de la zone Modifier les projets .

1. Commencez à saisir le nom d’un formulaire personnalisé dans le champ **Ajouter un formulaire personnalisé** champ .


   ![](assets/forms-already-attached-indication-in-bulk-editing-projects-unshimmed.png)

   Les formulaires personnalisés déjà joints aux projets sélectionnés s’affichent dans la variable **Formulaires attachés** dans la section **Ajouter un formulaire personnalisé** champ .

   Les formulaires personnalisés supplémentaires pouvant être associés à des projets, mais qui ne sont associés à aucun des projets sélectionnés s’affichent dans la variable **Forms à ajouter** dans la section **Ajouter un formulaire personnalisé** champ .

1. Cliquez pour sélectionner le formulaire personnalisé supplémentaire dans le **Ajouter un formulaire personnalisé** ou **Forms à ajouter** sous-sections lorsqu’elle s’affiche dans la liste.

   Lorsqu’un formulaire personnalisé est déjà joint à certains des projets sélectionnés, une indication indique à côté du nom du formulaire combien de projets le formulaire est déjà sélectionné lors de l’ajout d’un formulaire.

1. (Facultatif) Cliquez sur le **x** à droite du nom d’un formulaire personnalisé, puis cliquez sur **Supprimer** pour la supprimer de tous les projets sélectionnés.

   >[!CAUTION]
   >
   >La suppression de formulaires personnalisés entraîne la perte de toutes les informations de champs personnalisés existantes sur les formulaires. Cette opération ne peut pas être récupérée.

   Pour plus d’informations sur la modification de formulaires personnalisés, voir la section [Forms personnalisée](#custom-forms) dans cet article.

1. Cliquez sur **Finance** pour modifier les informations financières de tous les projets sélectionnés.
Pour plus d’informations sur la modification de la zone Finance, voir la section [Finance](#finance) dans cet article.
1. Cliquez sur **Paramètres du projet** pour modifier les paramètres de tous les projets sélectionnés.
Pour plus d’informations sur la modification de la zone Paramètres du projet, voir la section [Paramètres du projet](#project-settings) dans cet article.
1. Cliquez sur **Paramètres de tâche** pour modifier les paramètres de la tâche pour tous les projets sélectionnés.
Pour plus d’informations sur la modification de la zone Paramètres de tâche, voir la section [Paramètres de tâche](#task-settings) dans cet article.
1. Cliquez sur **Paramètres de problème** pour modifier les paramètres de problème pour tous les projets sélectionnés.
Pour plus d’informations sur la modification de la zone Paramètres du problème, voir la section [Paramètres de problème](#issue-settings) dans cet article.
1. Cliquez sur **Accès** pour modifier les paramètres d’accès de tous les projets sélectionnés.
Pour plus d’informations sur la modification de la zone Accès, voir la section [Accès](#access) dans cet article.
1. (Facultatif) Pour supprimer toutes les informations que vous avez ajoutées dans la zone Modifier les projets, passez la souris sur un champ modifié, puis cliquez sur le bouton **x** Ignorer l’icône en haut à droite du champ.

   ![](assets/discard-icon-for-field-edit-projects-in-bulk-unshimmed.png)

1. (Facultatif) Cliquez sur **Annuler** au bas de la **Modification de projets** pour supprimer toutes les modifications apportées à tous les projets.
1. Cliquer sur **Enregistrer**.

</div>

