---
content-type: overview
navigation-topic: grant-and-request-access-to-objects
title: Vue d’ensemble du partage des autorisations sur les objets
description: Vous pouvez partager ou supprimer des autorisations pour un objet que vous avez créé ou un objet qui a été partagé avec vous.
author: Courtney
feature: Get Started with Workfront
exl-id: 7c14702e-ac55-4266-88a7-f31618f84218
source-git-commit: 97f5adc8811a3be7be23137a82d10d45b76ec605
workflow-type: tm+mt
source-wordcount: '1332'
ht-degree: 82%

---

# Vue d’ensemble du partage des autorisations sur les objets

<!-- Audited: 12/2023 -->

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Redundancy here with the article Permissions for shared objects?</p>
-->
Lors du partage d’un objet avec une personne du système, vous pouvez accorder à la personne destinataire l’une des autorisations suivantes : afficher, contribuer et gérer.

Il n’est pas nécessaire d’être administrateur ou administratrice Adobe Workfront pour partager des autorisations sur les objets auxquels vous avez accès, mais ces autorisations fonctionnent selon les niveaux d’accès définis par l’administrateur ou administratrice Workfront.

Vous pouvez partager ou supprimer des autorisations pour un objet que vous avez créé ou un objet qui a été partagé avec vous. Lorsque vous n’êtes pas la personne ayant créé l’objet, vous devez disposer de l’accès Partager sur l’objet que vous souhaitez partager dans votre niveau d’accès, en plus des autorisations Partager sur l’objet. Pour plus d’informations sur les niveaux d’accès, voir [Vue d’ensemble des nouveaux niveaux d’accès](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md) ou [Vue d’ensemble des niveaux d’accès](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

>[!NOTE]
>
>Une équipe d’administration Workfront peut ajouter ou supprimer des autorisations à tous les éléments du système, pour toutes les personnes, sans être la personne propriétaire de ces éléments.

## Objets que vous pouvez partager dans Workfront.

Vous pouvez partager les objets suivants dans Workfront avec d’autres personnes :

* **Projets** : pour plus d’informations, voir [Partager un projet dans Adobe Workfront](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

* **Modèles** : pour plus d’informations, voir [Partager des modèles de projet](../../manage-work/projects/create-and-manage-templates/share-project-template.md).

* **Portfolios** : pour plus d’informations, voir [Partager un portfolio](../../workfront-basics/grant-and-request-access-to-objects/share-a-portfolio.md).

* **Programmes** : pour plus d’informations, voir [Partager un programme](../../workfront-basics/grant-and-request-access-to-objects/share-a-program.md).

* **Tâches** : pour plus d’informations, voir [Partager une tâche](../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md).

* **Problèmes** : pour plus d’informations, voir [Partager un problème](../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md).

* **Documents** : pour plus d’informations, voir [Partager un document](../../workfront-basics/grant-and-request-access-to-objects/document-permissions.md).

* **Dossiers de documents** : pour plus d’informations, voir [Partager un dossier de documents](../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

* **Épreuves** : pour plus d’informations, voir [Partager un épreuve dans Workfront](/help/quicksilver/review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

* **Rapports, tableaux de bord et calendriers** : pour plus d’informations, voir [Partager des rapports, des tableaux de bord et des calendriers](../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).  Consultez également les articles suivants :

   * [Partager un rapport dans Adobe Workfront](../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md)
   * [Partager un tableau de bord](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md)
   * [Partager un rapport de calendrier](../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md)

* **Filtres, vues et regroupements** : pour plus d’informations, voir [Partager un filtre, une vue ou un regroupement](../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).

* **Plans** : pour plus d’informations, voir [Partager un plan dans le planificateur de scénarios](../../scenario-planner/share-a-plan.md).

  Cette fonction nécessite une licence supplémentaire.

* **Objectifs** : pour plus d’informations, voir [Partager un objectif dans les Objectifs Workfront](../../workfront-goals/workfront-goals-settings/share-a-goal.md).

  Cette fonction nécessite une licence supplémentaire.

## Remarques relatives au partage d’objets

* Vous ne pouvez partager que le niveau d’autorisations que vous avez sur l’objet ou un niveau inférieur.

  Par exemple, si vous disposez des autorisations de contribution sur l’objet, vous ne pouvez pas accorder à une autre personne les autorisations de gestion sur cet objet.

* Vous ne pouvez pas partager un objet avec un niveau d’autorisation supérieur au niveau d’accès d’une personne.

  Par exemple, si une personne dispose de l’accès Afficher aux projets dans son niveau d’accès, vous ne pouvez pas lui accorder les autorisations de gestion sur un projet.
* Une personne autorisée à au moins afficher un objet peut le partager avec une autre personne.
* Vous pouvez partager des objets avec des personnes, des fonctions, des équipes, des groupes et des entreprises actifs.

  >[!NOTE]
  >
  >Vous ne pouvez partager un plan ou un objectif qu’avec d’autres utilisateurs et utilisatrices actifs. Cela nécessite des licences supplémentaires.
  >
  >
  >Pour plus d’informations, voir ce qui suit :
  >
  >* [Partager un plan dans le planificateur de scénarios](../../scenario-planner/share-a-plan.md)
  >* [Partager un objectif dans les Objectifs Workfront](../../workfront-goals/workfront-goals-settings/share-a-goal.md)

* Workfront envoie des notifications aux utilisateurs lorsque vous partagez un objet avec eux. Les notifications sont envoyées lorsque ces deux paramètres sont activés :

   * Les notifications électroniques **Partage d’objet pour l’utilisateur** et **Partage d’objet pour l’équipe** sont activées dans la zone Configuration par un administrateur système ou un administrateur de groupe. Pour plus d’informations, consultez l’article [Configurer les notifications d’événements pour tous les utilisateurs et les utilisatrices du système](/help/quicksilver/administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).
   * Les notifications **Quelqu&#39;un partage un objet avec moi** et **Quelqu&#39;un partage un objet avec mon équipe** sont activées dans la page de profil de l&#39;utilisateur. Pour plus d’informations, voir [Modifier vos propres notifications par e-mail](/help/quicksilver/workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

  Les paramètres au niveau du système ou du groupe doivent d’abord être activés avant de pouvoir activer les paramètres de notification pour l’utilisateur.

## Limites du partage

* Vous pouvez partager un objet avec jusqu’à 100 entités (personnes, équipes, groupes, fonctions, entreprises). Nous vous recommandons de partager des objets avec des groupes, des équipes ou des entreprises plutôt qu’avec des utilisateurs et utilisatrices individuels afin d’éviter cette limite.
* Un utilisateur dont le niveau d’accès ne permet pas d’accéder aux données financières ne peut pas accorder un accès qui permettrait à d’autres utilisateurs d’afficher les données financières. Cela inclut l’accès aux projets qui afficheraient des données financières ou la modification d’un niveau d’accès pour permettre l’affichage des données financières.


## Partager des autorisations sur les objets

Le tableau suivant illustre le niveau des autorisations que vous pouvez sélectionner lors du partage d’un objet. Tous les objets ne disposent pas de tous ces paramètres. Vous pouvez accorder à une autre entité des autorisations pour Afficher ou Gérer un objet. Si vous partagez un projet, une tâche ou un problème, vous pouvez également accorder des autorisations pour y contribuer.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Afficher</strong></td> 
   <td> <p>Vous pouvez effectuer les actions suivantes sur l’objet :</p> 
    <ul> 
     <li><p>Afficher l’objet</p></li> 
     <li><p>Ajouter des documents à l’objet</p></li> 
     <li><p>Ajoutez les problèmes à l’objet (s’il s’agit d’une tâche ou d’un projet)</p></li> 
     <li><p>Afficher des informations financières sur l’objet</p></li> 
     <li> <p>Partager l’objet<br></p> <p>Lorsque vous partagez l’objet, vous pouvez octroyer à d’autres personnes le même niveau d’autorisation que celui dont vous disposez sur l’objet, et non pas un niveau supérieur.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Contribuer</strong></td> 
   <td> <p>Vous pouvez effectuer les actions suivantes sur l’objet :</p> 
    <ul> 
     <li>Toutes les actions incluses avec l’autorisation d’affichage.</li> 
     <li>Y ajouter des dépenses</li> 
     <li>Y ajouter des tâches (projet)</li> 
     <li>Y modifier les formulaires personnalisés</li> 
     <li>Consigner des heures sur l’objet</li> 
     <li>Y réaliser des affectations</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Gérer</strong></td> 
   <td> <p>Vous pouvez effectuer les actions suivantes sur l’objet :</p> 
    <ul> 
     <li>Toutes les actions incluses avec les autorisations d’affichage et de contribution</li> 
     <li>Le supprimer.</li> 
     <li>Y gérer les informations financières</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Rendre ceci public pour les personnes externes</strong></td> 
   <td> <p>Toute personne ne disposant pas d’un compte Workfront peut afficher l’objet en cliquant sur un lien menant à celui-ci. Ceci n’est pas disponible pour tous les objets.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Rendre ceci visible sur tout le système.</strong></td> 
   <td> <p>L’objet se trouve dans les recherches et est visible par les utilisateurs disposant d’un compte Workfront.</p><p><b>Remarque </b> : les utilisateurs disposant de licences de contributeur ou de demandeur ne peuvent pas voir les projets, même si ce paramètre est activé. </td> 
  </tr> 
 </tbody> 
</table>

## Présentation des autorisations héritées et de la hiérarchie des objets

### Autorisations héritées des objets parent {#permissions-inherited-from-parent-objects}

Les autorisations dans Workfront sont héritées de manière hiérarchique. Cela signifie que, si vous accordez des autorisations à une personne sur un objet parent, elle obtient les mêmes autorisations sur les objets enfant qui lui sont associés par défaut.

Par exemple, si vous attribuez à une personne des autorisations de contribution à un projet, celle-ci dispose des autorisations de contribution sur toutes les tâches et tous les problèmes (objets enfant) associés à ce projet.

Dans l’exemple ci-dessus, vous ne pouvez pas restreindre les autorisations sur les objets enfant. Si vous ne souhaitez pas que la personne dispose d’autorisations de contribution sur les objets enfant associés au projet, vous devez supprimer manuellement les autorisations héritées des objets, puis ajuster les autorisations pour chaque personne, y compris les paramètres avancés.

Pour plus d’informations sur la hiérarchie et l’interdépendance des objets dans Workfront, voir la section [Interdépendance et hiérarchie des objets](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#interdependency-and-hierarchy-of-objects) dans l’article [Vue d’ensemble des objets Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

>[!NOTE]
>
>Votre administrateur Workfront peut désactiver les autorisations héritées pour les documents dans votre niveau d’accès.  Pour plus d&#39;informations sur la désactivation des autorisations héritées pour les documents dans le niveau d&#39;accès, voir [Créer ou modifier des niveaux d&#39;accès personnalisés](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

### Autorisations acquises par le biais des appartenances au sein de l’organisation   {#permissions-acquired-through-organizational-memberships}

Si vous accordez des autorisations de gestion à un groupe de personnes sur un objet et des autorisations d’affichage à une personne de ce groupe sur le même objet, la personne dispose du niveau d’autorisation le plus élevé (Gérer) accordé sur l’objet via l’appartenance au groupe.

Si vous souhaitez accorder des autorisations inférieures à une personne qui fait déjà partie d’une entité organisationnelle (Groupe, Équipe, Fonction ou Société) avec un niveau d’autorisation supérieur, vous devez supprimer les autorisations de l’entité organisationnelle et ajouter individuellement les personnes avec un niveau d’autorisation inférieur.


<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Remove permissions from objects</h2>
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">AL: draft/ hide this div when Becky makes Remove permissions from objects live and replace with the drafted content with the link at the top of this section</p>
<p>You can remove permissions from objects you have access to Share. Removing permissions from objects is identical for all objects that can be shared.  </p> <note type="note">
  You cannot remove permissions when you share items in bulk. You can remove permissions only when selecting individual items.  
</note>
<p>To remove permissions from objects consider the following:  </p>
<ul>
<li><a href="#remove-entities-from-the-sharing-list-of-an-object" class="MCXref xref">Remove entities from the sharing list of an object</a> </li>
<li><a href="#remove-inherited-permissions" class="MCXref xref">Remove inherited permissions</a> </li>
<li><a href="#make-an-object-private" class="MCXref xref">Make an object private</a> </li>
</ul>
<p><strong>Remove entities from the sharing list of an object</strong></p>
<p>You can remove entities from the sharing list of an object to remove their permissions from the object.</p>
<p>To remove permissions from objects:  </p>
<ol>
<li value="1">Navigate to an object on which you want to modify the permissions.</li>
<li value="2">Click the <strong>Actions</strong> menu, then click <strong>Sharing</strong>.<br>For example, on a project, click <strong>Project Actions</strong>, then <strong>Sharing</strong>.  </li>
<li value="3">Click the <strong>x</strong> next to the name of a user, team, group, company, job role to remove them.<br></li>
<li value="4">In the <strong><User Name>'s Workfront access will be removed from this</strong> drop-down menu, select whether you want their access to be removed just from the object you have selected, or from all children objects associated with it.<br>The following scenarios exist:
<ul>
<li>If you remove the entity only from the object, that entity loses their permissions on the object, and their inherited permissions to the children objects. If they are granted permissions to the children items individually, they retain the same permissions on all children objects associated with it when you select this option.  </li>
<li>If you remove the entity from the object and all the children objects, that entity loses their permissions to the object as well as all children objects, even when they have been given individual permission on each child object.  </li>
</ul></li>
<li value="5">Click <strong>Save</strong>.</li>
</ol>
<p> <p><strong>Remove inherited permissions</strong></p> </p>
<p>Inherited permissions can be removed from objects allowing for owners to specifically  identify who will get access to children objects regardless of the access of a user to a parent object. Only users with Manage permission are able to remove inherited permissions.</p>
<p>To remove inherited permissions:</p>
<ol>
<li value="1">Navigate to an object to which you have Manage permissions. <br>For example, navigate to a task.</li>
<li value="2">Go to the sharing list as described in the <a href="#Share" class="MCXref xref">Overview of sharing permissions on objects</a> section in this article. </li>
<li value="3">Select the <strong>X</strong>  mark next to <strong>Inherited Permission</strong>  on the sharing box to remove  anyone listed there.<br><br>This ensures that no one who is granted permissions to the parent object (for example, the project) has permissions to this task by default. You must list   individual entities in the sharing list of the task to grant permissions on the task.<br><note type="note">
You cannot remove individual entities from the Inherited Permissions list. You can only disable the Inherited Permissions for all entities listed.
</note></li>
<li value="4">Click <strong>Save</strong>.  </li>
</ol>
<p><strong>Make an object private</strong></p>
<p>If you have shared an object system-wide, or you have shared it with external uses by making it public, you can make it private again by removing the system-wide or public permissions.  </p>
<p>For more information about making an object available system-wide, or publicly, see the section <a href="#Share" class="MCXref xref">Overview of sharing permissions on objects</a> in this article.</p>
<p>To make an object private:</p>
<ol>
<li value="1">Go to the object you want to make private.<br>For example, navigate to a report.</li>
<li value="2">Click <strong>Report Actions</strong>, then <strong>Sharing</strong>.<br><br></li>
<li value="3">Click <strong>Remove public access</strong> to remove the access of external users to viewing the report.</li>
<li value="4">Click <strong>Remove system-wide access</strong> to stop sharing it with all Workfront users.  </li>
<li value="5">Click <strong>Save</strong>.</li>
</ol>
</div>
-->

## Partager un objet

Pour plus d’informations sur le partage d’objets, voir la section [Partager un objet](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

## Supprimer les autorisations des objets

Pour plus d’informations sur la suppression des autorisations des objets, voir la section [Supprimer des autorisations des objets](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

## Demander des autorisations sur les objets

Lorsqu’une personne vous envoie un lien vers un objet pour lequel vous ne disposez pas d’autorisations d’affichage, ou lorsque vous disposez d’autorisations inférieures sur un objet et que vous souhaitez demander un niveau d’autorisation supérieur, vous pouvez demander des autorisations sur l’objet.

Vous pouvez demander l’accès à un objet à toute personne disposant d’une autorisation de partage sur l’objet.

Pour plus d’informations sur la demande d’autorisations sur des objets, voir la section [Demander l’accès à des objets](../../workfront-basics/grant-and-request-access-to-objects/request-access.md).
