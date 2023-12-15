---
content-type: overview
navigation-topic: grant-and-request-access-to-objects
title: Présentation des autorisations de partage sur les objets
description: Vous pouvez partager ou supprimer des autorisations pour un objet que vous avez créé ou un objet qui a été partagé avec vous.
author: Alina
feature: Get Started with Workfront
exl-id: 7c14702e-ac55-4266-88a7-f31618f84218
source-git-commit: ca4da5302198d8fffc8b706baa3b3aeaa1f738e3
workflow-type: tm+mt
source-wordcount: '1165'
ht-degree: 0%

---

# Présentation des autorisations de partage sur les objets

<!-- Audited: 12/2023 -->

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Redundancy here with the article Permissions for shared objects?</p>
-->
Lors du partage d’un objet avec une personne du système, vous pouvez accorder au destinataire l’une des autorisations suivantes : afficher, contribuer et gérer.

Il n’est pas nécessaire d’être administrateur Adobe Workfront pour partager des autorisations sur les objets auxquels vous avez accès, mais ces autorisations fonctionnent selon les niveaux d’accès définis par l’administrateur Workfront.

Vous pouvez partager ou supprimer des autorisations pour un objet que vous avez créé ou un objet qui a été partagé avec vous. Lorsque vous n’êtes pas le créateur de l’objet, vous devez disposer de l’accès Partager sur l’objet que vous souhaitez partager dans votre niveau d’accès, en plus des droits Partager sur l’objet. Pour plus d’informations sur les niveaux d’accès, voir [Nouveaux niveaux d’accès - Aperçu](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md) ou [Présentation des niveaux d’accès](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

>[!NOTE]
>
>Un administrateur Workfront peut ajouter ou supprimer des autorisations à n’importe quel élément du système, pour tous les utilisateurs, sans en être le propriétaire.

## Objets que vous pouvez partager dans Workfront

Vous pouvez partager les objets suivants dans Workfront avec d’autres utilisateurs :

* **Projets**: pour plus d’informations, voir [Partage d’un projet dans Adobe Workfront](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

* **Modèles**: pour plus d’informations, voir [Partage de modèles de projet](../../manage-work/projects/create-and-manage-templates/share-project-template.md).

* **Portfolios**: pour plus d’informations, voir [Partage d’un portfolio](../../workfront-basics/grant-and-request-access-to-objects/share-a-portfolio..md).

* **Programmes**: pour plus d’informations, voir [Partager un programme](../../workfront-basics/grant-and-request-access-to-objects/share-a-program.md) .

* **Tâche**: pour plus d’informations, voir [Partage d’une tâche](../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md).

* **Problèmes**: pour plus d’informations, voir [Partage d’un problème](../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md).

* **Documents**: pour plus d’informations, voir [Partager un document](../../workfront-basics/grant-and-request-access-to-objects/document-permissions.md).

* **Dossiers de documents**: pour plus d’informations, voir [Partage d’un dossier de document](../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

* **Bons à tirer**: pour plus d’informations, voir [Partage d’un bon à tirer dans Workfront](/help/quicksilver/review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

* **Rapports, tableaux de bord et calendriers**: pour plus d’informations, voir [Partage de rapports, de tableaux de bord et de calendriers](../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md). Consultez également les articles suivants :

   * [Partage d’un rapport dans Adobe Workfront](../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md)
   * [Partage d’un tableau de bord](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md)
   * [Partage d’un rapport de calendrier](../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md)

* **Filtres, vues et regroupements**: pour plus d’informations, voir [Partager un filtre, une vue ou un regroupement](../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).

* **Formules**: pour plus d’informations, voir [Partage d’un plan dans le planificateur de scénarios](../../scenario-planner/share-a-plan.md).

  Cela nécessite une licence supplémentaire.

* **Objectifs**: pour plus d’informations, voir [Partage d’un objectif dans les objectifs Workfront](../../workfront-goals/workfront-goals-settings/share-a-goal.md).

  Cela nécessite une licence supplémentaire.

## Observations relatives au partage d’objets

* Vous ne pouvez partager que le même niveau ou un niveau inférieur d’autorisations que vous avez sur l’objet .

  Par exemple, si vous disposez des autorisations de contribution sur l’objet, vous ne pouvez pas accorder à un autre utilisateur les autorisations de Gérer sur cet objet.

* Vous ne pouvez pas partager un objet avec un niveau d’autorisation supérieur au niveau d’accès d’un utilisateur.

  Par exemple, si un utilisateur dispose de l’accès Affichage aux projets dans son niveau d’accès, vous ne pouvez pas lui accorder les autorisations Gérer sur un projet.
* Un utilisateur autorisé à au moins afficher un objet peut le partager avec un autre.
* Vous pouvez partager des objets avec des utilisateurs, des rôles de tâche, des équipes, des groupes ou des entreprises actifs.

  >[!NOTE]
  >
  >Vous ne pouvez partager un plan ou un objectif qu’avec d’autres utilisateurs actifs. Cela nécessite des licences supplémentaires.
  >
  >
  >Pour plus d’informations, voir :
  >
  >* [Partage d’un plan dans le planificateur de scénarios](../../scenario-planner/share-a-plan.md)
  >* [Partage d’un objectif dans les objectifs Workfront](../../workfront-goals/workfront-goals-settings/share-a-goal.md)

## Limites du partage

Vous pouvez partager un objet avec jusqu’à 100 entités (utilisateurs, équipes, groupes, rôles de tâche, entreprises). Nous vous recommandons de partager des objets avec des groupes, des équipes ou des entreprises plutôt qu’avec des utilisateurs individuels afin d’éviter cette limite.

## Partage des autorisations pour les objets

Le tableau suivant illustre le niveau des autorisations que vous pouvez sélectionner lors du partage d’un objet. Tous les objets ne disposent pas de tous ces paramètres. Vous pouvez accorder à une autre entité des autorisations pour Afficher ou Gérer un objet. Si vous partagez un projet, une tâche ou un problème, vous pouvez également accorder des autorisations pour y contribuer.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Afficher</strong></td> 
   <td> <p>Vous pouvez effectuer les actions suivantes sur l’objet :</p> 
    <ul> 
     <li><p>Affichage de l’objet</p></li> 
     <li><p>Ajouter des documents à l’objet</p></li> 
     <li><p>Affichage des informations financières sur l’objet</p></li> 
     <li> <p>Partage de l’objet<br></p> <p>Lorsque vous partagez l’objet, vous pouvez octroyer aux autres utilisateurs le même niveau d’autorisation que celui dont vous disposez uniquement sur l’objet, et non plus à un niveau supérieur.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Contribuer</strong></td> 
   <td> <p>Vous pouvez effectuer les actions suivantes sur l’objet :</p> 
    <ul> 
     <li>Toutes les actions sont incluses avec l’autorisation Afficher .</li> 
     <li>Ajouter des dépenses à celle-ci</li> 
     <li>Ajouter des problèmes (s’il s’agit d’une tâche ou d’un projet)</li> 
     <li>Ajouter des tâches à ce projet (s’il s’agit d’un projet)</li> 
     <li>Modifier le Forms personnalisé dessus</li> 
     <li>Journal des heures sur l’objet</li> 
     <li>Rendre des affectations dedans</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Gérer</strong></td> 
   <td> <p>Vous pouvez effectuer les actions suivantes sur l’objet :</p> 
    <ul> 
     <li>Toutes les actions incluses avec les autorisations Afficher et Contribuer</li> 
     <li>Supprimer</li> 
     <li>Gérer les informations financières dans celle-ci</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Rendre ceci public aux utilisateurs externes</strong></td> 
   <td> <p>Toute personne sans compte Workfront peut afficher l’objet en cliquant sur un lien vers celui-ci. Cette option n’est pas disponible pour tous les objets.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Rendre ceci visible sur tout le système.</strong></td> 
   <td> <p>L’objet peut être trouvé dans les recherches et consulté par toute personne disposant d’un compte Workfront.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Présentation des autorisations héritées et de la hiérarchie des objets

### Autorisations héritées des objets parents {#permissions-inherited-from-parent-objects}

Les autorisations dans Workfront sont héritées de manière hiérarchique. Cela signifie que si vous accordez des autorisations à un utilisateur sur un objet parent, il obtient les mêmes autorisations sur les objets enfants qui lui sont associés par défaut.

Par exemple, si vous attribuez à un utilisateur des autorisations de contribution pour un projet, il dispose des autorisations de contribution pour toutes les tâches et problèmes (objets enfants) associés à ce projet.

En suivant l’exemple ci-dessus, vous ne pouvez pas restreindre les autorisations aux objets enfants. Si vous ne souhaitez pas que l’utilisateur dispose d’autorisations de contribution pour les objets enfants associés au projet, vous devez supprimer manuellement les autorisations héritées des objets, puis ajuster les autorisations pour chaque utilisateur, y compris les paramètres avancés. 

Pour plus d’informations sur la hiérarchie et l’interdépendance des objets dans Workfront, reportez-vous à la section [Interdépendance et hiérarchie des objets](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#interdependency-and-hierarchy-of-objects) dans l’article [Présentation des objets Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

>[!NOTE]
>
>Votre administrateur Workfront peut désactiver les autorisations héritées pour les documents de votre niveau d’accès. Pour plus d’informations sur la désactivation des autorisations héritées pour les documents de niveau d’accès, voir [Création ou modification de niveaux d’accès personnalisés](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

### Autorisations acquises grâce aux appartenances organisationnelles  {#permissions-acquired-through-organizational-memberships}

Si vous accordez des autorisations Gérer à un groupe d’utilisateurs sur un objet et que vous accordez des autorisations Afficher à un utilisateur individuel de ce groupe sur le même objet, l’utilisateur dispose du niveau d’autorisation le plus élevé (Gérer) accordé via l’appartenance à un groupe sur l’objet. 

Si vous souhaitez accorder des autorisations moindres à un utilisateur qui fait déjà partie d’une entité organisationnelle (Groupe, Équipe, Rôle de tâche ou Société) avec un niveau d’autorisation supérieur, vous devez supprimer les autorisations de l’entité organisationnelle et ajouter individuellement des utilisateurs avec un niveau d’autorisation inférieur.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Remove permissions from objects</h2>
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">AL: draft/ hide this div when Becky makes Remove permissions from objects live and replace with the drafted content with the link at the top of this section</p>
<p>You can remove permissions from objects you have access to Share. Removing permissions from objects is identical for all objects that can be shared.&nbsp;</p> <note type="note">
&nbsp;You cannot remove permissions when you share items in bulk. You can remove permissions only when selecting individual items.&nbsp;
</note>
<p>To remove permissions from objects consider the following:&nbsp;</p>
<ul>
<li><a href="#remove-entities-from-the-sharing-list-of-an-object" class="MCXref xref">Remove entities from the sharing list of an object</a> </li>
<li><a href="#remove-inherited-permissions" class="MCXref xref">Remove inherited permissions</a> </li>
<li><a href="#make-an-object-private" class="MCXref xref">Make an object private</a> </li>
</ul>
<p><strong>Remove entities from the sharing list of an object</strong></p>
<p>You can remove entities from the sharing list of an object to remove their permissions from the object.</p>
<p>To remove permissions from objects:&nbsp;</p>
<ol>
<li value="1">Navigate to an object on which you want to modify the permissions.</li>
<li value="2">Click the <strong>Actions</strong> menu, then click <strong>Sharing</strong>.<br>For example, on a project, click <strong>Project Actions</strong>, then <strong>Sharing</strong>.&nbsp;</li>
<li value="3">Click the <strong>x</strong> next to the name of a user, team, group, company, job role to remove them.<br></li>
<li value="4">In the <strong><User Name>'s Workfront access will be removed from this</strong> drop-down menu, select whether you want their access to be removed just from the object you have selected, or from all children objects associated with it.<br>The following scenarios exist:
<ul>
<li>If you remove the entity only from the object, that entity loses their permissions on the object, and their inherited permissions to the children objects. If they are granted permissions to the children items individually, they retain the same permissions on all children objects associated with it when you select this option.&nbsp;</li>
<li>If you remove the entity from the object and all the children objects, that entity loses their permissions to the object as well as all children objects, even when they have been given individual permission on each child object.&nbsp;</li>
</ul></li>
<li value="5">Click <strong>Save</strong>.</li>
</ol>
<p> <p><strong>Remove inherited permissions</strong></p> </p>
<p>Inherited permissions can be removed from objects allowing for owners to specifically&nbsp;identify who will get access to children objects regardless of the access of a user to a parent object. Only users with Manage permission are able to remove inherited permissions.</p>
<p>To remove inherited permissions:</p>
<ol>
<li value="1">Navigate to an object to which you have Manage permissions. <br>For example, navigate to a task.</li>
<li value="2">Go to the sharing list as described in the <a href="#Share" class="MCXref xref">Overview of sharing permissions on objects</a> section in this article. </li>
<li value="3">Select the <strong>X</strong>&nbsp;mark next to <strong>Inherited Permission</strong>&nbsp;on the sharing box to remove&nbsp;anyone listed there.<br><br>This ensures that no one who is granted permissions to the parent object (for example, the project) has permissions to this task by default. You must list&nbsp; individual entities in the sharing list of the task to grant permissions on the task.<br><note type="note">
You cannot remove individual entities from the Inherited Permissions list. You can only disable the Inherited Permissions for all entities listed.
</note></li>
<li value="4">Click <strong>Save</strong>.&nbsp;</li>
</ol>
<p><strong>Make an object private</strong></p>
<p>If you have shared an object system-wide, or you have shared it with external uses by making it public, you can make it private again by removing the system-wide or public permissions.&nbsp;</p>
<p>For more information about making an object available system-wide, or publicly, see the section <a href="#Share" class="MCXref xref">Overview of sharing permissions on objects</a> in this article.</p>
<p>To make an object private:</p>
<ol>
<li value="1">Go to the object you want to make private.<br>For example, navigate to a report.</li>
<li value="2">Click <strong>Report Actions</strong>, then <strong>Sharing</strong>.<br><br></li>
<li value="3">Click <strong>Remove public access</strong> to remove the access of external users to viewing the report.</li>
<li value="4">Click <strong>Remove system-wide access</strong> to stop sharing it with all Workfront users.&nbsp;</li>
<li value="5">Click <strong>Save</strong>.</li>
</ol>
</div>
-->

## Partager un objet

Pour plus d’informations sur le partage d’objets, voir [Partager un objet](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

## Suppression des autorisations des objets

Pour plus d’informations sur la suppression des autorisations des objets, voir [Suppression des autorisations des objets](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

## Demande d’autorisations pour les objets

Lorsque quelqu’un vous envoie un lien vers un objet que vous ne disposez pas des autorisations de Afficher, ou lorsque vous avez des autorisations inférieures sur un objet et que vous souhaitez demander un niveau supérieur d’autorisations, vous pouvez demander des autorisations sur l’objet. 

Vous pouvez demander l’accès à un objet à toute personne disposant de l’autorisation Partager sur l’objet . 

Pour plus d’informations sur la demande d’autorisations pour des objets, voir [Demande d’accès aux objets](../../workfront-basics/grant-and-request-access-to-objects/request-access.md).
