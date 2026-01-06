---
title: Partager un projet
product-area: projects
navigation-topic: grant-and-request-access-to-objects
description: Votre administrateur ou administratrice Adobe Workfront peut vous accorder l’accès à l’affichage ou à la modification de projets lors de l’affectation de votre niveau d’accès. Pour plus d’informations, voir Accorder l’accès aux projets.
author: Courtney
feature: Get Started with Workfront
exl-id: eaeedff8-9114-40d9-8cd4-56996edc7dad
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '1574'
ht-degree: 60%

---

# Partager un projet

<!-- Audited: 1/2024 -->

Votre administrateur ou administratrice Adobe Workfront peut vous accorder l’accès à l’affichage ou à la modification de projets lors de l’affectation de votre niveau d’accès. Pour plus d’informations, voir [Accorder l’accès aux projets](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

Outre le niveau d’accès qui est accordé aux personnes, vous pouvez leur accorder des autorisations d’affichage, de contribution ou de gestion de projets spécifiques pour lesquels vous avez accès au partage.

Les autorisations sont spécifiques à un élément dans Workfront et définissent les actions que vous pouvez effectuer sur cet élément.


## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Standard</p> 
   <p>Travail ou supérieur</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès Affichage ou supérieur aux objets que vous souhaitez partager.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations d’affichage ou supérieures pour les objets que vous souhaitez partager.</p></td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Observations relatives au partage de projets

Outre les considérations ci-dessous, voir [Vue d’ensemble des autorisations de partage sur les objets](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

* Par défaut, le créateur ou la créatrice d’un projet dispose des autorisations nécessaires pour gérer le projet et est également propriétaire du projet. Si le projet est attribué à une autre personne propriétaire, cette personne dispose également des autorisations nécessaires pour gérer le projet. Lorsque le créateur ou créatrice (ou propriétaire) du projet partage le projet avec d’autres personnes, certaines autorisations leur sont accordées pour contrôler ce que ces personnes peuvent faire lorsqu’elles travaillent sur le projet.

  Cependant, si le propriétaire d’un projet ne dispose pas d’une licence de plan ou standard, il ne dispose pas d’un accès complet pour gérer le projet. Seul un utilisateur disposant d’une licence de plan ou standard peut disposer des autorisations pour gérer un projet. Pour plus d’informations, voir [Fonctionnement des niveaux d’accès et des autorisations](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

* Vous pouvez partager des projets individuellement ou partager plusieurs d’entre eux à la fois. Le partage de projets est identique au partage d’autres objets. Pour plus d’informations sur le partage d’éléments dans Workfront, voir [Partager un objet](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).
* Vous pouvez accorder les autorisations suivantes à un projet :

   * Afficher
   * Gérer
   * Contribuer

* Lorsque vous partagez un projet, toutes les tâches, tous les problèmes et tous les documents héritent des mêmes autorisations, sauf indication contraire.

  Pour plus d’informations sur la gestion de l’accès aux tâches et aux problèmes du projet en fonction des autorisations d’une personne sur le projet, voir la section [&#128279;](../../manage-work/projects/manage-projects/edit-projects.md#access) dans l’article [Modifier des projets](../../manage-work/projects/manage-projects/edit-projects.md).

  L’administrateur ou l’administratrice Workfront peut indiquer si les documents doivent hériter des autorisations des objets supérieurs dans le niveau d’accès de l’utilisateur ou de l’utilisatrice. Pour plus d’informations sur la restriction des autorisations héritées sur les documents, voir [Créer ou modifier des niveaux d’accès personnalisés](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* Vous pouvez supprimer les autorisations héritées d’un projet afin que les objets enfants ne les héritent pas. Pour plus d’informations sur la suppression des autorisations héritées des objets, voir [Supprimer des autorisations des objets](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

## Restrictions relatives aux différents types de licence

* Les utilisateurs et les utilisatrices disposant d’une licence Travail ne disposent pas des autorisations nécessaires pour gérer des projets. Pour les personnes chargées du travail, l’autorisation de partage la plus élevée est Contribuer.
* Les utilisateurs et les utilisatrices disposant d’une licence Demande peuvent afficher les informations d’un projet, mais leur accès au projet est limité.
* Une exception concernant la modification du statut d’un projet se produit lorsqu’une personne disposant des autorisations Afficher ou Contribuer est également incluse dans un processus d’approbation. Celle-ci peut approuver le projet, ce qui modifie le statut du projet, mais le statut est le statut prédéfini d’approbation ou de rejet.
* Pour pouvoir copier un projet, un utilisateur ou une utilisatrice doit également disposer de l’accès à la création de projets dans son niveau d’accès.

## Méthodes pour partager un projet {#ways-to-share-a-project}

Vous pouvez partager un projet de l’une des façons suivantes :

* Manuellement, effectuez l’une des opérations suivantes :

   * Ajouter des personnes à l’équipe du projet. Lorsque vous ajoutez des personnes à l’équipe du projet, elles obtiennent automatiquement les autorisations d’affichage du projet.\
     Pour plus d&#39;informations sur l&#39;ajout d&#39;utilisateurs à une équipe de projet, consultez la section Ajout d&#39;utilisateurs à une équipe de projet dans [présentation de l&#39;équipe de projet](../../manage-work/projects/planning-a-project/project-team-overview.md).
   * Partage individuel ou en passe des projets lors de l’utilisation de l’option **Partage**.

* Automatiquement en effectuant l’une des opérations suivantes :

   * Placer un projet dans un **Portfolio** ou **Programme** qui est déjà partagé avec d’autres. Les personnes disposent des mêmes autorisations pour le projet que pour le portfolio ou le programme.\
     Pour plus d’informations sur l’ajout d’un projet à un **Portfolio**, voir [Ajouter des projets à un portfolio](../../manage-work/portfolios/create-and-manage-portfolios/add-projects-to-portfolios.md).\
     Pour plus d’informations sur l’ajout d’un projet à un **Programme**, voir [Ajouter un projet à un programme](../../manage-work/portfolios/create-and-manage-programs/add-project-to-program.md).
Pour plus d’informations sur l’affichage des autorisations héritées sur un objet, voir [Afficher les autorisations héritées sur les objets](../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md).

   * Ajouter des entités au partage de projet sur un modèle utilisé pour créer le projet. Pour plus d’informations sur le partage de projets à partir de modèles, voir [Partager un modèle](../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).
   * Définir le modèle d’accès à un projet.

     >[!TIP]
     >
     >Lors de l’ajout ou de l’enregistrement d’un modèle, vous pouvez effacer les règles de partage de modéle de projet.

   * Modifiez un projet et définissez le paramètre **Lorsqu’une personne a accès à ce projet**.  Pour plus d’informations, voir [Modifier les projets](../../manage-work/projects/manage-projects/edit-projects.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: drafted because I created new article and linked it above) </p>
<p>To view what users have inherited the access on the project from a portfolio or a program, do the following:</p>
<ol style="list-style-type: lower-alpha;">
<li value="1">Go to a project whose sharing permissions you want to view. </li>
<li value="2"> Click the <strong>More</strong> menu <img src="assets/more-icon.png">, then click <strong>Sharing</strong>. </li>
<li value="3"> <p>Expand the <strong>Inherited Permissions</strong> list. </p> <p>This list displays the names of users that have access to either the portfolio or the program that the project belongs to and also have permissions to the project. </p>  </li>
</ol>
</div>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Go to a project whose sharing permissions you want for all projects you create from scratch. (NOTE: drafted because linked above)  </li>
<li value="2"> Click the More menu, then click <strong>Sharing</strong>. </li>
<li value="3"> <p>In the Project Access box that displays, near the upper-right corner, click the gear icon <img src="assets/gear-icon-settings.png">, then click <strong>Set as my project access template</strong>.</p> <p>The entities that are granted permissions on the selected project have the same permissions for all the projects you create from scratch in the future.</p> <p> The project access template overrides the sharing defaults granted to you by the Workfront administrator in your Access Level.<br>For more information about specifying sharing defaults for projects in the Access Level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>.</p> </li>
<li value="4">Click <strong>Save</strong>.</li>
</ol>
-->

## Partager un projet

{{step1-to-projects}}

1. Sur la page **Projets**, sélectionnez dans la liste le projet que vous souhaitez partager. La page du projet s’ouvre.

1. À droite du nom du projet, cliquez sur **Partager**. La boîte de dialogue **Partager[Nom du projet]** s’ouvre.

   ![bouton Partager le projet](assets/share-project.png)

1. Dans le champ **Accorder l’accès au projet à**, commencez à saisir le nom de l’utilisateur, de l’équipe, du rôle, du groupe ou de la société avec lequel vous souhaitez partager le projet, puis cliquez sur le nom lorsqu’il apparaît dans la liste déroulante.

   >[!TIP]
   >
   >Vous pouvez uniquement partager un projet avec des utilisateurs actifs, des équipes, des rôles ou des entreprises.


1. (Facultatif) Sélectionnez le menu déroulant **Qui a accès** et sélectionnez le niveau d’accès du projet :

   * **Seules les personnes invitées peuvent y accéder :** seuls les utilisateurs invités au projet peuvent y accéder (par défaut).
   * **Tout le monde peut afficher dans le système** : tous les utilisateurs du système peuvent afficher le projet sans invitation.

1. (Facultatif) Pour appliquer automatiquement les paramètres d’accès au projet que vous avez sélectionnés à tous les nouveaux projets, cliquez sur l’icône **Engrenage** ![Sélectionnez l’icône en forme d’engrenage](assets/gear-icon.png), puis cochez la case en ligne avec **Définir comme modèle d’accès à mon projet**.

   >[!NOTE]
   >
   >Le modèle d’accès au projet remplace les valeurs par défaut de partage qui vous ont été attribuées par l’administrateur ou l’administratrice Workfront de votre niveau d’accès.\
   >Pour plus d’informations sur la spécification des valeurs par défaut de partage pour les projets dans le niveau d’accès, voir [Accorder l’accès aux projets](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md)

   <!--
   >this note also appears in Understanding Project Permissions-->


1. Cliquez sur la liste déroulante située à droite du nom de l’utilisateur et sélectionnez son niveau d’autorisation pour ce projet :


   * **Afficher** : l’utilisateur peut réviser et partager le projet.
   * **Contribuer** : l’utilisateur peut effectuer des mises à jour, consigner des informations, apporter des modifications mineures et partager le projet (inclut également toutes les autorisations d’affichage).
   * **Gérer** : l’utilisateur dispose d’un accès complet au projet, sans droits d’administration, qui sont accordés au niveau d’accès (inclut également toutes les autorisations Afficher et Contribuer).

1. (Facultatif) Cliquez sur l’icône des options avancées en regard du niveau d’autorisation que vous avez accordé pour configurer des autorisations spécifiques sur le projet.

   ![Options d’autorisation avancées configurées](assets/advanced-permission-options.png)

1. (Facultatif) Pour partager rapidement le projet à l’aide d’un lien, cliquez sur **Copier le lien** puis transférez-le au destinataire.

1. Cliquer sur **Enregistrer**.

## Partage de projets en bloc

{{step1-to-projects}}

1. Sur la page **Projets**, cochez la case à gauche de chaque projet à partager, puis cliquez sur l’icône **Partager** ![Icône Partager](assets/share-icon.png) en haut de la page. La boîte de dialogue modale de partage s’ouvre.

   ![Partage en bloc de projets](assets/bulk-share-icon.png)

1. Dans le champ **Accorder l’accès au projet à**, commencez à saisir le nom de l’utilisateur, de l’équipe, du rôle, du groupe ou de la société avec lequel vous souhaitez partager les projets, puis cliquez sur le nom lorsqu’il apparaît dans la liste déroulante.

   >[!TIP]
   >
   >Vous pouvez uniquement partager des projets avec des utilisateurs actifs, des équipes, des rôles ou des entreprises.


1. (Facultatif) Sélectionnez le menu déroulant **Qui a accès** et sélectionnez le niveau d’accès du projet :

   * **Seules les personnes invitées peuvent y accéder :** seuls les utilisateurs invités aux projets peuvent y accéder (par défaut).
   * **Tout le monde peut afficher dans le système** : tous les utilisateurs du système peuvent afficher les projets sans invitation.


1. Cliquez sur la liste déroulante située à droite du nom de l’utilisateur et sélectionnez son niveau d’autorisation pour les projets :

   * **Affichage** : l’utilisateur peut réviser et partager les projets.
   * **Contribuer** : l’utilisateur peut effectuer des mises à jour, consigner des informations, apporter des modifications mineures et partager les projets (inclut également toutes les autorisations d’affichage).
   * **Gérer** : l’utilisateur dispose d’un accès complet aux projets sans droits d’administration, qui sont accordés au niveau d’accès (inclut également toutes les autorisations Afficher et Contribuer).

1. (Facultatif) Cliquez sur l’icône des options avancées en regard du niveau d’autorisation que vous avez accordé pour configurer des autorisations spécifiques sur les projets.

   ![Options d’autorisation avancées configurées](assets/advanced-permission-options.png)

1. Cliquer sur **Enregistrer**.


<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Configure default permissions for a project</h2>
<p>(NOTE: drafted because I added one more way to automatically share the project above in the bullet list and linked it to Edit Projects) </p>
<p>As a project owner, you can configure the default permissions for View, Manage, and Contribute access that are used when sharing  the project with others. When users share a project, the default permissions are used. Users can then adjust the default permissions when sharing the project, as described in <a title="Project Permissions" href="#ways-to-share-a-project" class="MCXref xref">Ways to share a project</a>. </p>
<p>To configure the default permissions that are included with each access level:</p>
<ol>
<li value="1">Go to the project where you want to set the default permissions.</li>
<li value="2"> <p>Click the More menu <img src="assets/more-icon.png">, then click <strong>Edit</strong>. <img src="assets/edit-icon.png"></p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
<li value="3">Click <strong>Access</strong> in the list on the left.</li>
<li value="4"> <p>In the <strong>When someone is given access to this PROJECT</strong> section, select permissions that you want to be available when users are given access to the project via sharing.</p> <p>Ensure that any permissions that you want to include in the selected access level are selected and deselect any permissions that you do not want to include in the selected permissions level.</p> <p>To view which permissions are available for each level, see  <a title="Project Permissions" href="#Understanding_Project_Permissions" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <note type="note">
The
<strong>Delete</strong> access in the
<strong>Manage</strong> permission level determines whether users can  delete the project itself. Users with
<strong>Manage</strong> access to the project can delete tasks and issues within the project regardless of whether this option is selected, if they have
<strong>Manage</strong> permissions to the tasks and issues.  
</note> </li>
<li value="5">Click <strong>Save Changes</strong>.</li>
</ol>
</div>
-->

## Options d’autorisation pour un projet

Le tableau suivant répertorie les autorisations que les utilisateurs et les utilisatrices peuvent accorder lors du partage d’un projet. Pour plus d’informations sur l’accès dont disposent les utilisateurs et les utilisatrices en fonction de leur licence, voir [Accorder l’accès aux projets](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Actions</strong> </p> </th> 
   <th> <p><strong>Gérer</strong> </p> </th> 
   <th> <p><strong>Contribuer</strong> </p> </th> 
   <th> <p><strong>Afficher</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Ajouter un formulaire personnalisé</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Mettre à jour les champs personnalisés</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Ajouter un processus d’approbation</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Approuver un projet</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Approuver les heures</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓  </p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Créer un projet</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Ajouter un ou plusieurs documents</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Ajouter un ou plusieurs problèmes</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Ajouter une ou plusieurs tâches</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Copier le projet</p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Supprimer projet</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Modifier les dates prévues</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Partager le projet</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Partager sur le système</p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Afficher projet</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Mises à jour / commentaires</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Modifier le statut</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Consigner les heures</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Modifier les affectations</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Gérer la ligne de base</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Gérer les risques*</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Gérer les finances*</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Ajouter/modifier les dépenses*</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Afficher les finances*</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Joindre modèle</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Enregistrer en tant que modèle</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Ajouter/modifier un business case</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Modifier les détails du projet</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Modifier le personnel</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Exporter vers MS Project</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Recalculer les finances / la chronologie*</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Définir les propriétés de file d’attente</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>  </p> </td> 
   <td> <p>    </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Modifier le projet en masse dans une liste</p> </td> 
   <td> <p>✓</p> </td> 
   <td>  </td> 
   <td>  </td> 
  </tr> 
 </tbody> 
</table>

&#42;Les personnes n’ayant pas accès aux données financières ne peuvent pas gérer les risques et les finances des projets, même si elles disposent de l’accès Éditer pour les projets. Pour plus d’informations sur l’accès aux données financières, voir [Accorder l’accès aux données financières](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
