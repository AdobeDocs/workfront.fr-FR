---
product-area: templates
navigation-topic: templates-navigation-topic
title: Joindre un modèle à un projet
description: Vous pouvez joindre un modèle à un projet pendant la phase de création initiale du projet ou après sa création.
author: Alina
feature: Work Management
exl-id: bce9af59-5467-4458-b923-01bfa469e2d8
source-git-commit: 3d0a6932bda338af1e6b3dcba49bfc0ac486d919
workflow-type: tm+mt
source-wordcount: '1126'
ht-degree: 46%

---

# Joindre un modèle à un projet

<!-- Audited: 10/2025 -->

Vous pouvez joindre un modèle à un projet pendant la phase de création initiale du projet ou après sa création.

Pour plus d’informations sur la création d’un projet à partir d’un modèle, consultez [Créer un projet à l’aide d’un modèle](../../../manage-work/projects/create-projects/create-project-from-template.md).

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
    <p>Plan</p>
    </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès en modification aux projets </p> <p>Afficher l'accès aux modèles</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations de gestion pour le projet</p> <p>Autorisations Afficher ou supérieures pour le modèle</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
 
 <table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>New: Standard</p>
   <p>Or</p>
   <p>Current: Plan</p>
    </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Projects </p> <p>For information about project access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>.</p> <p>View access to&nbsp;Templates</p> <p>For information about template permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md" class="MCXref xref">Share a template</a>. </p> <p>For information about template access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">Grant access to templates</a>.</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create and modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the project</p> <p>For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>. </p> <p>View permissions or higher to the template</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Considerations when adding templates to projects</h2>
<p>(NOTE: moved this to an Overview article of its own) </p>
<p>Consider the following when adding templates to projects:</p>
<ul>
<li> <p>You can attach only active templates to projects. </p> </li>
<li> <p>You can attach a template to a project when the project is in a status of Complete, Dead, or in Pending Approval, only when your Adobe Workfront administrator <span>or a group administrator</span> has enabled this functionality in the Project&nbsp;Preferences area. For information about setting project preferences, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>. </p> </li>
<li> <p>Unless you exclude specific template tasks from being added in the attachment process, all template tasks are added to the existing project. </p> </li>
<li> <p>Most template settings are added to the project. </p> </li>
<li> <p>Some settings from the template automatically transfer to the project, unless you specifically mark them to be excluded. </p>
<div class="example" data-mc-autonum="<b>Example: </b>">
<span class="autonumber"><span><b>Example: </b></span></span>
<p>For example, these settings are added to the project:</p>
<ul>
<li>Start&nbsp;From field</li>
<li>Custom forms and the information on them</li>
<li>Queue Details </li>
<li>Financial settings </li>
</ul>
</div> </li>
</ul>
</div>
-->

## Joindre un modèle à un projet existant {#attach-a-template-to-an-existing-project}

Vous pouvez joindre un modèle à un projet à partir de la page du projet, d’une liste de projets ou d’un rapport.

{{step1-to-projects}}

1. Sur la page **Projets**, sélectionnez le projet auquel vous souhaitez joindre un modèle.

1. Cliquez sur l’icône **Plus** dans le menu déroulant ![Plus](assets/more-dropdown.png) à droite du nom du projet.

   ![icône Plus](assets/qs-more-icon-on-an-object.png)

   Ou

   Accédez à une liste ou à un rapport de projet et sélectionnez un projet, puis cliquez sur l’icône **Plus** dans le menu déroulant ![Plus](assets/more-dropdown.png) en haut de la liste.

   ![Menu Plus développé](assets/more-menu-expanded.png)

1. Cliquez sur **Joindre un modèle**. La zone **Joindre le modèle** s’affiche.

1. Commencez à saisir le nom du modèle à joindre dans le champ **Modèles de recherche**, puis cliquez dessus lorsqu’il s’affiche dans la liste.

   Ou

   Cliquez sur le nom d’un modèle dans la zone **Autres modèles**.

   Une prévisualisation du modèle s’affiche à droite et contient les informations suivantes sur le modèle :

   * Durée
   * Propriétaire
   * Le nombre de tâches de niveau supérieur (comprend une liste des 3 premières tâches de niveau supérieur)
   * Nombre total de tâches
   * Noms des formulaires personnalisés joints

   ![Joindre une zone de modèle](assets/attach-template-box-template-preview-area-nwe-350x282.png)

1. (Facultatif) Cliquez sur l’icône **Favoris** ![icône Favoris](assets/favorites-icon-small.png) à droite du nom du modèle pour le marquer comme favori et le déplacer vers la liste **Favoris**.

1. (Facultatif) Cliquez de nouveau sur l’icône **Favoris** ![Icône Favoris](assets/favorites-icon-selected.png) pour la supprimer de la liste **Favoris**.
1. Cliquez sur **Personnaliser et joindre**. Le panneau latéral **Joindre un modèle** s’ouvre.

1. (Facultatif) Mettez à jour les informations dans les sections suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader" colspan="2"> <p role="rowheader" colspan="2">Section Tâches</p> <p role="rowheader" colspan="2"> <img src="assets/attach-template-large-box-tasks-section-nwe-350x289.png" style="width: 350;height: 289;"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Les tâches de modèle sélectionnées ci-dessous sont importées dans le projet.Désélectionnez celles que vous souhaitez exclure. </td> 
      <td><p>Désélectionnez les tâches à exclure du modèle avant de l’associer au projet.</p>
      <p><b>CONSEIL</b></p>
      <p>Vous ne pouvez choisir qu'une seule tâche.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Sélectionnez la tâche de projet que vous souhaitez désigner comme tâche antérieure pour ce modèle.</td> 
      <td> <p>Cliquez dans la zone de champ pour afficher la liste des tâches du projet, puis sélectionnez la tâche qui doit se terminer avant que les tâches du modèle puissent commencer. Vous pouvez également ignorer cette étape et configurer des relations au sein du projet une fois le modèle joint. </p> <p> Sélectionnez les informations <strong>Type de dépendance</strong>, <strong>Délai</strong> et si vous souhaitez que le prédécesseur soit appliqué en cochant la case <strong>Appliquer le prédécesseur</strong>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Sélectionnez la tâche du projet que vous souhaitez comme parent dans ce modèle.</td> 
      <td> <p>Sélectionnez la tâche de projet que vous souhaitez désigner comme tâche parent pour toutes les tâches du modèle. Si vous ne faites pas de sélection, toutes les tâches de modèles apparaissent à la fin de vos tâches de projet actuelles. Vous pouvez ignorer cette étape et déplacer les tâches dans le projet une fois le modèle joint.</p>
      <p><b>NOTE</b></p>
      <p>Si vous avez sélectionné une tâche de modèle parent avec des enfants supplémentaires, seul le parent affichera la tâche du projet comme son prédécesseur une fois qu'elle aura été ajoutée au projet. Les tâches de modèles enfants n’affichent pas de prédécesseur.</p>
      <p>Si vous avez sélectionné uniquement une tâche de modèle enfant, la tâche de projet s'affichera comme son prédécesseur une fois qu'elle aura été ajoutée au projet. </p>

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p role="rowheader" colspan="2">Section Options</p> <p role="rowheader" colspan="2"> <img src="assets/attach-template-large-box-options-section-nwe-350x78.png" style="width: 350;height: 78;"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Les éléments sélectionnés ci-dessous sont transférés vers le projet. Désélectionnez ceux que vous souhaitez exclure.</td> 
      <td> <p>Décochez les cases correspondant aux informations que vous souhaitez exclure du modèle avant de les joindre au projet. Pour plus d’informations sur chaque champ, consultez <a href="../../../manage-work/projects/create-and-manage-templates/attach-template-to-project-overview.md" class="MCXref xref">Vue d’ensemble de l’ajout d’un modèle à un projet</a>. </p> <p>Important : si vous cochez la case <strong>Configuration des propriétés et des problèmes de file d’attente</strong>, les détails de la file d’attente du modèle remplacent ceux du projet. Dans ce cas, les règles de routage, les rubriques de file d’attente et les groupes de rubriques de file d’attente du modèle sont ajoutés à ceux du projet. <br>Si le projet est configuré comme une file d'attente des demandes et que le modèle que vous joignez au projet n'est pas configuré comme une file d'attente des demandes, les informations sur la file d'attente du projet sont supprimées si vous laissez la case <strong>Propriétés de la file d'attente et configuration des événements</strong> cochée. <br>Si vous désélectionnez la case <strong>Propriétés de la file d'attente et Configuration de l'événement</strong>, tous les paramètres de configuration de la file d'attente du projet sont conservés et aucun paramètre de configuration de la file d'attente du modèle n'est joint. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p role="rowheader" colspan="2">Section de formulaires personnalisés</p> <p role="rowheader" colspan="2"> <img src="assets/attach-template-large-box-custom-forms-section-nwe-350x274.png" style="width: 350;height: 274;"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Formulaires personnalisés</td> 
      <td> <p>Lorsque des formulaires personnalisés sont joints au modèle, leurs noms s’affichent dans le panneau de gauche. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Facultatif) Mettez à jour les informations dans les formulaires personnalisés. Ces informations sont transférées au projet.

   >[!TIP]
   >
   >* Cette étape est obligatoire lorsque les formulaires personnalisés du modèle contiennent des champs obligatoires vides.
   >* Si les champs du modèle de formulaires personnalisés existent déjà sur le projet et contiennent des informations, ils conservent les informations déjà présentes sur le projet. Vous ne pouvez pas les modifier lorsque vous joignez le modèle.

1. Cliquez sur **Joindre un modèle.**
1. Cliquez sur **Annuler la pièce jointe** pour arrêter l’ajout du modèle.

   Ou

   Autorisez l’ajout de la pièce jointe pour joindre le modèle au projet.

   Après avoir joint le modèle, vous pouvez modifier le projet et ajuster les tâches, informations ou paramètres, le cas échéant.

1. (Facultatif) Dans le panneau de gauche, cliquez sur **Détails du projet**, puis **Aperçu** pour afficher le nom du modèle associé dans la zone **Relations du projet**.

   >[!TIP]
   >
   >Si vous joignez plusieurs modèles au projet, seul le modèle que vous avez joint en premier s’affichera dans ce champ. Pour plus d’informations, consultez la section [Joindre plusieurs modèles à un projet existant et afficher les informations relatives aux modèles](#attach-multiple-templates-to-an-existing-project-and-view-template-information) dans cet article.

1. (Facultatif) Supprimez les informations de modèle du projet auquel vous avez joint le modèle. Pour plus d’informations, consultez [Supprimer les informations sur les modèles d’un projet](../../../manage-work/projects/create-and-manage-templates/remove-template-from-project.md).

## Joindre plusieurs modèles à un projet existant et afficher les informations relatives aux modèles {#attach-multiple-templates-to-an-existing-project-and-view-template-information}

Vous pouvez joindre plusieurs modèles (un à la fois) au même projet en suivant les étapes décrites dans la section [Joindre un modèle à un projet existant](#attach-a-template-to-an-existing-project) dans cet article. Les tâches et autres informations de chaque modèle sont ainsi ajoutées au projet.

>[!TIP]
>
>Lorsque vous joignez plusieurs modèles à un projet, seul le modèle que vous avez joint en premier s’affiche dans la zone Détails du projet .

Pour afficher le modèle appliqué à un projet :

{{step1-to-projects}}

1. Sur la page **Projets**, sélectionnez le projet auquel est associé un modèle.

1. Cliquez sur **Détails du projet** dans le panneau de gauche.

1. Recherchez le nom du modèle associé au projet dans le champ **Modèle** au bas de la section **Présentation** sous **Relations du projet**.

   ![Informations de modèle sur un projet](assets/nwe-template-info-on-project-350x356.png)


