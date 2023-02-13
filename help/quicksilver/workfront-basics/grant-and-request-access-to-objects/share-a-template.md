---
title: Partager un modèle
product-area: templates
navigation-topic: grant-and-request-access-to-objects
description: En tant qu’administrateur Adobe Workfront, vous pouvez accorder aux utilisateurs l’accès à l’affichage ou à la modification de modèles lorsque vous attribuez leur niveau d’accès. Un utilisateur doit disposer d’une licence Plan pour avoir accès aux modèles d’édition.
author: Alina
feature: Get Started with Workfront
exl-id: 19fb0de5-7db5-42a9-9f33-a4570acfeef8
source-git-commit: dd7f61fcd92a43303be356dd3209ec6da6a063dd
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 2%

---

# Partage d’un modèle

En tant qu’administrateur Adobe Workfront, vous pouvez accorder aux utilisateurs l’accès à l’affichage ou à la modification de modèles lorsque vous attribuez leur niveau d’accès. Un utilisateur doit disposer d’une licence Plan pour avoir accès aux modèles d’édition.

Pour plus d’informations sur l’octroi de l’accès aux modèles, voir [Accorder l’accès aux modèles](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md).

En plus du niveau d’accès que vous accordez, un utilisateur peut également recevoir des autorisations pour Afficher ou Gérer des modèles spécifiques d’autres utilisateurs qui les partagent .

>[!NOTE]
>
>Les niveaux d’autorisation fonctionnent dans les niveaux d’accès. Par exemple, un utilisateur ne peut pas recevoir les autorisations de gestion d’un modèle, si son niveau d’accès lui permet uniquement d’afficher les modèles.

Les autorisations sont spécifiques à un élément dans Workfront et définissent les actions que vous pouvez effectuer sur cet élément.

## Remarques concernant le partage d’un modèle

* Outre les considérations ci-dessous, reportez-vous également à la section [Présentation des autorisations de partage sur les objets](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).
* Par défaut, le créateur d’un modèle, ainsi que le propriétaire du modèle, disposent des autorisations de gestion du modèle. Pour plus d’informations sur la désignation d’un utilisateur comme propriétaire de modèle, voir [Modifier des modèles de projet](../../manage-work/projects/create-and-manage-templates/edit-templates.md).
* Vous pouvez partager les éléments suivants lors du partage d’un modèle :

   * Le modèle

      Pour plus d’informations sur le partage d’un modèle, voir [Partage de modèles de projet](../../manage-work/projects/create-and-manage-templates/share-project-template.md).

      Vous pouvez accorder les autorisations suivantes à un modèle :

      * Afficher

         ![](assets/view-on-template-262x221.png)

      * Gérer

         ![](assets/manage-on-template-225x280.png)
   * Les futurs projets créés à partir du modèle. Vous pouvez accorder les mêmes niveaux d’autorisation aux projets créés à partir d’un modèle que pour un projet individuel. 

      Pour plus d’informations sur le partage d’un projet à partir d’un modèle au niveau du modèle, voir [Partage de modèles de projet](../../manage-work/projects/create-and-manage-templates/share-project-template.md).


* Lorsque vous partagez un modèle ou un projet créé à partir du modèle, les utilisateurs héritent par défaut des mêmes autorisations pour tous les objets enfants associés au modèle ou au projet.

   Pour plus d’informations sur la hiérarchie des objets dans Workfront, voir  [Présentation des objets dans Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

* Lorsque vous partagez un modèle, toutes les tâches et tous les documents du modèle, ainsi que les problèmes relatifs au futur projet créé à partir du modèle, héritent des mêmes autorisations, sauf indication contraire.

   Pour plus d’informations sur la gestion de l’accès aux tâches de modèle et sur les problèmes du projet en fonction des autorisations d’un utilisateur sur le projet, voir la section [Accès](../../manage-work/projects/create-and-manage-templates/edit-templates.md#access) dans l’article [Modifier des modèles de projet](../../manage-work/projects/create-and-manage-templates/edit-templates.md).

* L’administrateur de Workfront peut indiquer si les documents doivent hériter des autorisations des objets de niveau supérieur au niveau d’accès de l’utilisateur. Pour plus d’informations sur la restriction des autorisations héritées sur les documents, voir [Création ou modification de niveaux d’accès personnalisés](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Share a template</h2>
<p>(NOTE: drafted because this is also linked above: Share project templates >> which is an article in the Manage Work section>> Templates)&nbsp;</p>
<ol>
<li value="1"> <p>Go to the template you want to share with other entities, click <strong>Template Actions</strong>, then <strong>Template Sharing</strong>.<br>Or</p> <p>Navigate to a list of templates, and select multiple templates from the list, then click <strong>Share Template</strong>.</p> <note type="note">
If you select multiple templates, you cannot view who already has permissions to the individual templates.
</note> </li>
<li value="2"> <p>Start typing the name of a user, group, team, job role, or company that you want to share the template with in the <strong>Give template access to</strong> or <strong>Edit template access for</strong> fields.</p> <p>Select them when they appear in the list.</p> <note type="tip">
You can share an object only with active users, teams,
<span>roles,</span> or companies.
</note> </li>
<li value="3">From the drop-down menu, select which level of permissions you want to grant:<br>
<ul>
<li><p><strong>View it</strong>: Users with these permissions are able to view the template and create a project using it, or attach it to an existing project.</p><p><img src="assets/template-permissions-350x197.png" alt="template_permissions.png" style="width: 350;height: 197;"></p></li>
<li><strong>Manage it</strong>: Users with these permissions are able to edit or delete the template.</li>
</ul></li>
<li value="4">(Optional) Click <strong>Advanced Settings</strong> to fine-tune your settings for each level of permissions.</li>
<li value="5">Click <strong>Save</strong>.</li>
</ol>
<h2>Share a project at the template level</h2>
<p>You can share the future projects that are created using a template with users at the template level.</p>
<ol>
<li value="1"> <p>Go to the template whose future projects you want to share with other entities, click <strong>Template Actions</strong>, then <strong>Project Sharing</strong>.</p> <p>Or</p> <p>Navigate to a list of templates, and select multiple templates from the list, then click <strong>Share Project</strong>.</p> <note type="note">
If you select multiple templates, you cannot view who already has project permissions to the individual templates.
</note> </li>
<li value="2"> <p>Start typing and then select the name of a user, group, team, job role, or company with whom you want to share future projects created from the template in the <strong>Give project access to</strong> or <strong>Edit template access for</strong> fields.</p> <note type="tip">
You can share an object only with active users, teams,
<span>roles,</span> or companies.
</note> </li>
<li value="3">From the drop-down menu, select which level of permissions you want to grant.<br>Select from the following:<br>
<ul>
<li><strong>No access</strong>: You can specify which users will not have any access to the template.<br>This option is available only when bulk sharing projects from templates.&nbsp;</li>
<li><strong>View</strong>: Users with these permissions can view projects created from the template.</li>
<li><strong>Contribute</strong>: Users with these permissions can contribute to projects created from the template&nbsp;</li>
<li><strong>Manage</strong>: Users with these permissions can manage or delete projects created from this template.<br><img src="assets/share-project-from-template-350x268.png" alt="share_project_from_template.png" style="width: 350;height: 268;"></li>
</ul></li>
<li value="4">(Optional) Click <strong>Advanced Settings</strong> to fine-tune your settings for each level of permissions. </li>
<li value="5">Click <strong>Save</strong>.</li>
</ol>
</div>
-->

## Paramètres avancés pour le partage de modèles

Le tableau suivant affiche les autorisations que vous pouvez accorder aux utilisateurs lorsqu’ils peuvent afficher ou gérer un modèle. Pour obtenir des instructions sur le partage d’un modèle, reportez-vous à la section [Partage d’un modèle](../../manage-work/projects/create-and-manage-templates/share-project-template.md#share) dans l’article [Partage de modèles de projet](../../manage-work/projects/create-and-manage-templates/share-project-template.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Actions</th> 
   <th>Gérer</th> 
   <th>Afficher</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Copier</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Supprimer</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Modifier les détails du modèle</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Afficher modèle</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Partager</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Partager sur le système</td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Ajouter des documents</p> <p>Conseil : Parfois, les gens ajoutent des documents à un modèle de projet en pensant qu’ils les ajoutent à un projet. Vous pouvez empêcher cela pour vos destinataires en désactivant ce paramètre.</p> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

Pour comprendre les autorisations que vous accordez aux utilisateurs pour des projets créés à partir d’un modèle, reportez-vous à la section [Partage d’un projet dans Adobe Workfront](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).
