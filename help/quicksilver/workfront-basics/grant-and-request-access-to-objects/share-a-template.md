---
title: Partager un modèle
product-area: templates
navigation-topic: grant-and-request-access-to-objects
description: En tant que personne membre de l’administration Adobe Workfront, vous pouvez accorder aux utilisateurs et aux utilisatrices l’accès à l’affichage ou à la modification des modèles lorsque vous leur attribuez un niveau d’accès. Un utilisateur ou une utilisatrice doit disposer d’une licence Plan pour avoir accès à l’option de modification des modèles.
author: Courtney
feature: Get Started with Workfront
exl-id: 19fb0de5-7db5-42a9-9f33-a4570acfeef8
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '584'
ht-degree: 92%

---

# Partager un modèle

En tant que personne membre de l’administration Adobe Workfront, vous pouvez accorder aux utilisateurs et aux utilisatrices l’accès à l’affichage ou à la modification des modèles lorsque vous leur attribuez un niveau d’accès. Un utilisateur ou une utilisatrice doit disposer d’une licence Plan pour avoir accès à l’option de modification des modèles.

Pour plus d’informations sur l’octroi d’un accès aux modèles, consultez la section [Accorder un accès aux modèles](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md).

En plus des accès que vous accordez, un utilisateur ou une utilisatrice peut aussi se voir attribuer des droits pour afficher ou gérer des modèles spécifiques que partagent d’autres utilisateurs et utilisatrices.

>[!NOTE]
>
>Les niveaux d’autorisation fonctionnent à l’intérieur des niveaux d’accès. Ainsi, un utilisateur ou une utilisatrice ne peut pas se voir accorder les droits de gestion d’un modèle si son accès est limité uniquement à l’affichage de ceux-ci.

Les autorisations sont spécifiques à un élément dans Workfront et définissent les actions que vous pouvez effectuer sur cet élément.

## Éléments à prendre en compte lors du partage d’un modèle

* Outre les considérations ci-dessous, voir [Vue d’ensemble des autorisations de partage sur les objets](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).
* Toute personne créant ou possédant un modèle dispose par défaut des droits de gestion de ce modèle. Pour plus d’informations sur la désignation d’un utilisateur ou d’une utilisatrice en tant que propriétaire du modèle, consultez la section [Modifier les modèles de projet](../../manage-work/projects/create-and-manage-templates/edit-templates.md).
* Vous pouvez partager les éléments suivants lors du partage d’un modèle :

   * Modèle

     Pour plus d’informations sur la manière de partager un modèle, consultez la section [Partager des modèles de projet](../../manage-work/projects/create-and-manage-templates/share-project-template.md).

     Vous pouvez accorder les autorisations suivantes à un modèle :

      * Afficher
      * Gérer

   * Futurs projets créés à l’aide du modèle. Vous pouvez accorder aux projets créés à partir d’un modèle les mêmes niveaux d’autorisation qu’à un projet individuel.

     Pour plus d’informations sur la manière de partager un projet à partir d’un modèle au niveau du modèle, consultez la section [Partager des modèles de projet](../../manage-work/projects/create-and-manage-templates/share-project-template.md).

* En partageant un modèle ou un projet issu de ce modèle, les autorisations attribuées se transmettent par défaut à tous les objets enfant associés au modèle ou au projet.

  Pour plus d’informations sur la hiérarchie des objets dans Workfront, voir   [Comprendre les objets dans Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

* Quand un modèle est partagé, toutes les tâches, les documents qui y sont inclus, et les problèmes des projets futurs créés à partir de ce modèle reçoivent automatiquement les mêmes droits d’accès, sauf exceptions spécifiées.

  Pour plus d’informations sur la gestion de l’accès aux modèles de tâches et de problèmes sur un projet en fonction des droits d’un utilisateur ou d’une utilisatrice sur ce projet, consultez la section [Accès](../../manage-work/projects/create-and-manage-templates/edit-templates.md#access) dans l’article [Modifier les modèles de projet](../../manage-work/projects/create-and-manage-templates/edit-templates.md).

* L’administrateur ou l’administratrice Workfront peut indiquer si les documents doivent hériter des autorisations des objets supérieurs dans le niveau d’accès de l’utilisateur ou de l’utilisatrice. Pour plus d’informations sur la restriction des autorisations héritées sur les documents, voir [Créer ou modifier des niveaux d’accès personnalisés](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* Vous ne pouvez pas partager des tâches de modèles individuellement. Le partage d’un modèle partage également les tâches de modèle. Le partage du projet à partir du modèle partage également les futures tâches du projet.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Share a template</h2>
<p>(NOTE: drafted because this is also linked above: Share project templates >> which is an article in the Manage Work section>> Templates)  </p>
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
<li><strong>No access</strong>: You can specify which users will not have any access to the template.<br>This option is available only when bulk sharing projects from templates.  </li>
<li><strong>View</strong>: Users with these permissions can view projects created from the template.</li>
<li><strong>Contribute</strong>: Users with these permissions can contribute to projects created from the template  </li>
<li><strong>Manage</strong>: Users with these permissions can manage or delete projects created from this template.<br><img src="assets/share-project-from-template-350x268.png" alt="share_project_from_template.png" style="width: 350;height: 268;"></li>
</ul></li>
<li value="4">(Optional) Click <strong>Advanced Settings</strong> to fine-tune your settings for each level of permissions. </li>
<li value="5">Click <strong>Save</strong>.</li>
</ol>
</div>
-->

## Paramètres avancés pour le partage des modèles

Le tableau suivant indique les autorisations que vous pouvez accorder aux utilisateurs et utilisatrices lorsque les droits d’affichage et de gestion leur sont aussi accordés. Pour les instructions sur le partage d’un modèle, consultez la section [Partager un modèle](../../manage-work/projects/create-and-manage-templates/share-project-template.md#share) dans l’article [Partager des modèles de projet](../../manage-work/projects/create-and-manage-templates/share-project-template.md).

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
   <td>  </td> 
  </tr> 
  <tr> 
   <td>Supprimer</td> 
   <td>✓</td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td>Modifier les détails du modèle</td> 
   <td>✓</td> 
   <td>  </td> 
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
   <td>  </td> 
   <td>✓</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Ajouter des documents</p> <p>Conseil : il arrive que des personnes ajoutent des documents à un modèle de projet en pensant les avoir ajoutés à un projet. Vous pouvez éviter cela pour vos personnes destinataires en désactivant ce paramètre.</p> </td> 
   <td>  </td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

Pour comprendre les autorisations que vous accordez aux utilisateurs et aux utilisatrices pour les projets créés à partir d’un modèle, consultez la section [Partager un projet dans Adobe Workfront](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).
