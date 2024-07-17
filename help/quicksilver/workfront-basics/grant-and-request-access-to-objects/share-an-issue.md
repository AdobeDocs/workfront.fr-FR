---
product-area: projects
navigation-topic: grant-and-request-access-to-objects
title: Partager un problème
description: Votre administrateur Adobe Workfront permet aux utilisateurs d’accéder aux problèmes d’affichage ou de modification lorsqu’ils attribuent des niveaux d’accès. Pour plus d’informations sur l’octroi de l’accès aux problèmes, voir Octroi de l’accès aux problèmes.
author: Alina
feature: Get Started with Workfront
exl-id: 91ee72e0-20a9-4b06-9f80-a343dd4fbe06
source-git-commit: dd7f61fcd92a43303be356dd3209ec6da6a063dd
workflow-type: tm+mt
source-wordcount: '695'
ht-degree: 8%

---

# Partager un problème

Votre administrateur Adobe Workfront permet aux utilisateurs d’accéder aux problèmes d’affichage ou de modification lorsqu’ils attribuent des niveaux d’accès. Pour plus d’informations sur l’octroi de l’accès aux problèmes, voir [Octroi de l’accès aux problèmes](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md).

Outre le niveau d’accès que les utilisateurs reçoivent, vous pouvez leur accorder des autorisations pour Afficher, Contribute ou Gérer des problèmes spécifiques que vous avez accès au partage. Pour plus d’informations sur les niveaux d’accès et les autorisations, voir [Comment les niveaux d’accès et les autorisations fonctionnent ensemble](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

Les autorisations sont spécifiques à un élément dans Workfront et définissent les actions que vous pouvez effectuer sur cet élément.

## Considérations sur les problèmes de partage

Outre les considérations ci-dessous, reportez-vous également à la section [Présentation des autorisations de partage sur les objets](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

>[!NOTE]
>
>Un administrateur Workfront peut ajouter ou supprimer des autorisations à n’importe quel élément du système, pour tous les utilisateurs, sans en être le propriétaire.

* Par défaut, le créateur d’un problème dispose des autorisations Manage (Gérer).
* Vous pouvez partager des problèmes individuellement ou plusieurs d’entre eux à la fois. Les problèmes de partage sont identiques au partage d’autres éléments dans Workfront. Pour plus d’informations sur le partage d’éléments dans Workfront, voir [Partage d’un objet](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).
* Vous pouvez accorder les autorisations suivantes à un problème : 

   * Afficher

     ![view_on_issue.png](assets/view-on-issue-221x216.png)

   * Gérer

     ![manage_on_issues.png](assets/manage-on-issues-179x199.png)

   * Contribuer\
     ![contribuer_on_issue.png](assets/contribute-on-issue-156x205.png)

* Lorsque vous partagez un problème, tous les documents associés au problème héritent des mêmes autorisations.

  L’administrateur de Workfront peut indiquer si les documents doivent hériter des autorisations des objets de niveau supérieur au niveau d’accès de l’utilisateur. Pour plus d’informations sur la limitation des autorisations héritées sur les documents, voir [Création ou modification de niveaux d’accès personnalisés](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* Vous pouvez supprimer les autorisations héritées d’un problème. Pour plus d’informations, voir [Suppression des autorisations des objets](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

## Méthodes de partage d’un problème

* Manuellement, ce qui revient à partager n’importe quel autre objet dans Workfront. Pour plus d’informations sur le partage d’objets dans Workfront, voir [Partage d’un objet](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).
* Automatiquement, en effectuant l’une des opérations suivantes :

   * Spécifiez les autorisations sur l’un des objets parents du problème : projet, programme ou portfolio. Les problèmes héritent des autorisations de leurs objets parents. Pour plus d’informations sur l’affichage des autorisations héritées sur les objets, voir [Affichage des autorisations héritées sur les objets](../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md).
   * Ajoutez des entités au partage de projet sur un modèle utilisé pour créer le projet sur lequel porte le problème. Pour plus d’informations sur le partage de projets à partir de modèles, voir [Partage d’un modèle](../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

   * Spécifiez les autorisations pour tous les problèmes d’un projet lorsque vous le modifiez. Pour plus d’informations sur la gestion de l’accès aux problèmes ou aux requêtes du projet en fonction des autorisations d’un utilisateur sur le projet, reportez-vous à la section [](../../manage-work/projects/manage-projects/edit-projects.md#access) de l’article [Modifier les projets](../../manage-work/projects/manage-projects/edit-projects.md).

     >[!TIP]
     >
     >Si vous ne spécifiez pas les autorisations de problème que les utilisateurs doivent posséder lorsqu’ils sont affectés aux problèmes du projet, ils reçoivent par défaut les mêmes autorisations que celles dont ils disposent sur le projet.

   * Spécifiez les autorisations que les utilisateurs reçoivent sur les problèmes qu’ils envoient dans une file d’attente de demandes lors de la création d’une file d’attente de demandes. Pour plus d’informations, voir [Création d’une file d’attente de requêtes](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

     >[!IMPORTANT]
     >
     >Les autorisations sont accordées différemment selon que le projet est publié ou non en tant que file d’attente de demandes :
     >
     >   
     >   
     >   * Lorsqu’un utilisateur envoie une demande à un projet publié en tant que file d’attente de demandes, les utilisateurs Contact de Principal et Entré par se voient accorder l’autorisation spécifiée.
     >   * Lorsqu’un utilisateur envoie une requête à un projet qui n’est pas publié en tant que file d’attente de requêtes, le contact de Principal (s’il est différent de Entré par l’utilisateur) se voit accorder l’autorisation spécifiée, et l’utilisateur Entré par se voit octroyer les autorisations de gestion du problème.
     >   
     >

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Automatically share an issue at the project level</h2>
<p>(NOTE: this info duplicates in Edit projects - linked there instead (above).)&nbsp;</p>
<p>As the Project Owner, you can grant permissions automatically to users as the issues are added to a project.</p>
<ol>
<li value="1">Go to the project whose issues you want to share automatically.</li>
<li value="2"> Click the More menu <img src="assets/more-icon.png">, then click <strong>Edit</strong>. </li>
<li value="3">In the <strong>Edit Project</strong> box that displays, click <strong>Access</strong>.</li>
<li value="4">In the <strong>When someone is assigned to an ISSUE</strong> field, select from the following permissions levels:
<ul>
<li><strong>View</strong></li>
<li><strong>Contribute</strong></li>
<li><strong>Manage</strong><br>Now, when someone is assigned to an issue on the selected project, they are granted the specified permissions to the issue.&nbsp;</li>
</ul></li>
<li value="5">(Optional) Select the <strong>Also grant ... access to the project</strong> field to also grant View, Contribute, or Manage permissions to the projects to the user assigned to the issue</li>
<li value="6">In the <strong>When someone submits a REQUEST ...</strong> field, select from the following permissions levels:
<ul>
<li><strong>View</strong></li>
<li><strong>Contribute</strong></li>
<li><p><strong>Manage</strong></p><note type="important">
<p>Permissions are granted differently depending on whether or not the project is published as a request queue:</p>
<ul>
<li>When a user submits a request to a project published as a request queue, the Primary Contact and Entered By users are granted the permission specified.</li>
<li>When a user submits a request to a project not published as a request queue, the Primary Contact (if different from Entered By user) is granted the permission specified, and the Entered By user is granted Manage permissions to the issue.</li>
</ul>
</note></li>
</ul></li>
<li value="7"> <p>(Optional) Select the <strong>People from the same company will inherit the same permissions for all requests</strong> field.</p> <p>People from the same company as the user submitting the request are granted the same permissions on the requests as the user.&nbsp;</p> </li>
<li value="8">Click <strong>Save Changes</strong>.</li>
</ol>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Automatically share an issue in request queues</h2>
<p>(NOTE: drafted because it's duplicated from Create a Request Queue which is linked above)&nbsp;</p>
<p>As the Project Owner, you can grant permissions automatically to users as the issues are submitted to a request queue.</p>
<ol>
<li value="1">Go to the project whose issues you want to share automatically.</li>
<li value="2">Click <strong>Edit Project</strong>.</li>
<li value="3">Click <strong>More</strong> then click <strong>Queue Setup</strong>. </li>
<li value="4"> <p>On the <strong>Queue Details</strong> sub-tab, in the drop-down menu under <strong>When someone makes a request, automatically grant</strong>, select from the following permissions levels:</p>
<ul>
<li><strong>View Access</strong> </li>
<li><strong>Contribute Access</strong> </li>
<li> <p><strong>Manage Access</strong> </p> </li>
</ul> <p>Now, when someone submits a request to the selected project, they are granted the specified permissions to the request.</p> </li>
<li value="5"> <p>(Optional) Select the <strong>People from the same company will inherit the same permissions for all requests</strong>.</p> <p>People from the same company as the user submitting the request are granted the same permissions on the requests as the user.&nbsp;</p> </li>
<li value="6">Click <strong>Save</strong>.</li>
</ol>
</div>
-->

## Autorisations de problème

Le tableau suivant affiche les autorisations que vous pouvez accorder aux utilisateurs lorsqu’ils peuvent afficher, Contribute ou gérer un problème :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Actions</strong> </td> 
   <td><strong>Gérer</strong> </td> 
   <td><strong>Contribute</strong> </td> 
   <td><strong>Afficher</strong> </td> 
  </tr> 
  <tr> 
   <td> <p>Ajouter des problèmes</p> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Supprimer </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Joindre un formulaire personnalisé</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Modifier les champs personnalisés</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Approuver le problème</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Ajouter Un Processus D’Approbation</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Ajouter des documents</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Copier le problème*</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Déplacer événement</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Consigner les heures</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Convertir en projet*</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Assignation</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Mises à jour/commentaires</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Modifier les dates planifiées</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Créer des affectations</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Partager</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Partager sur le système</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

&#42;Contrôlé par les niveaux d’accès et les autorisations du projet.
