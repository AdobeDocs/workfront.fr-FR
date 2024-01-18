---
product-area: templates
navigation-topic: templates-navigation-topic
title: Joindre un modèle à un projet
description: Vous pouvez joindre un modèle à un projet pendant la phase de création initiale du projet ou après sa création.
author: Alina
feature: Work Management
exl-id: bce9af59-5467-4458-b923-01bfa469e2d8
source-git-commit: 31ee3259167532e1e1efa75d635786762f6e476e
workflow-type: tm+mt
source-wordcount: '1138'
ht-degree: 0%

---

# Joindre un modèle à un projet

Vous pouvez joindre un modèle à un projet pendant la phase de création initiale du projet ou après sa création.

Pour plus d’informations sur la création d’un projet à l’aide d’un modèle, voir [Créer un projet à l’aide d’un modèle](../../../manage-work/projects/create-projects/create-project-from-template.md).

## Exigences d’accès

Pour effectuer les étapes décrites dans cet article, vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Quelconque </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modifier l’accès aux projets </p> <p>Pour plus d’informations sur l’accès au projet, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Accorder l’accès aux projets</a>.</p> <p>Affichage de l’accès aux modèles</p> <p>Pour plus d’informations sur les autorisations de modèle, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md" class="MCXref xref">Partager un modèle</a>. </p> <p>Pour plus d’informations sur l’accès aux modèles, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">Accorder l’accès aux modèles</a>.</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gestion des autorisations pour le projet</p> <p>Pour plus d’informations sur les autorisations de projet, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Partage d’un projet dans Adobe Workfront</a>. </p> <p>Affichage des autorisations ou supérieures au modèle</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

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

Vous pouvez joindre un modèle à un projet dans Workfront à partir de la page du projet ou d’une liste de projets ou d’un rapport.

1. Dans le projet auquel vous souhaitez joindre un modèle, cliquez sur le bouton **Plus** icon ![](assets/qs-more-icon-on-an-object.png) à droite du nom du projet

   ![](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   Ou

   Accédez à une liste de projets ou à un rapport et sélectionnez un projet, puis cliquez sur le bouton **Plus** icon ![](assets/qs-more-icon-on-an-object.png) en haut de la liste.

   ![](assets/more-menu-expanded-in-a-list-one-project-selected-nwe.png)


1. Cliquez sur **Joindre un modèle**.

   La zone Joindre un modèle s’affiche.

1. Commencez à saisir le nom du modèle que vous souhaitez joindre dans le champ **Modèles de recherche** puis cliquez dessus lorsqu’il s’affiche dans la liste.

   Ou

   Cliquez sur le nom d’un modèle dans le **Autres modèles** zone.

   Un aperçu du modèle s’affiche à droite et contient les informations suivantes sur le modèle :

   * Durée
   * Propriétaire
   * Le nombre de tâches de niveau supérieur (inclut une liste des trois premières tâches de niveau supérieur)
   * Nombre total de tâches
   * Noms des formulaires personnalisés joints

   ![](assets/attach-template-box-template-preview-area-nwe-350x282.png)

1. (Facultatif) Cliquez sur le **Favoris** icon ![](assets/favorites-icon-small.png) à gauche du nom du modèle pour le marquer comme favori. Le modèle est ainsi déplacé dans la liste Favoris.

   ![](assets/favorites-icon-on-template-list-in-attach-template-box-nwe-350x79.png)

1. (Facultatif) Cliquez sur le **Favoris** icon ![](assets/favorites-icon-selected.png) pour le supprimer à nouveau de la liste Favoris.
1. Cliquez sur **Personnalisation et ajout**.

   ![](assets/attach-template-large-box-nwe-350x262.png)

1. Mettez à jour les informations dans les sections suivantes avant de joindre le modèle (ou cliquez sur **Joindre un modèle** à tout moment) :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader" colspan="2"> <p role="rowheader" colspan="2">Section Tâches</p> <p role="rowheader" colspan="2"> <img src="assets/attach-template-large-box-tasks-section-nwe-350x289.png" style="width: 350;height: 289;"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Les tâches de modèle sélectionnées ci-dessous sont importées dans le projet. Désélectionnez ceux que vous souhaitez exclure. </td> 
      <td>Désélectionnez les tâches à exclure du modèle avant de l’associer au projet.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Sélectionnez la tâche de projet qui vous intéresse comme prédécesseur pour les tâches de ce modèle.</td> 
      <td> <p>Cliquez sur le champ pour afficher la liste des tâches du projet. Sélectionnez la tâche de projet qui doit être terminée avant que les tâches du modèle puissent commencer. Vous pouvez également ignorer cette étape et configurer des relations au sein du projet une fois le modèle joint. </p> <p> Sélectionnez la variable <strong>Type de dépendance</strong>, <strong>Étiquette</strong> et si vous souhaitez que le prédécesseur soit <strong>Enchaîné</strong> ou pas. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Sélectionnez la tâche de projet que vous souhaitez comme parent des tâches de ce modèle.</td> 
      <td> Sélectionnez la tâche de projet que vous souhaitez désigner comme tâche parente pour toutes les tâches de modèle. Si vous n’effectuez pas de sélection, toutes les tâches du modèle s’affichent à la fin des tâches du projet en cours. Vous pouvez ignorer cette étape et déplacer les tâches dans le projet une fois le modèle joint.</td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p role="rowheader" colspan="2">Section Options</p> <p role="rowheader" colspan="2"> <img src="assets/attach-template-large-box-options-section-nwe-350x78.png" style="width: 350;height: 78;"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Les éléments sélectionnés ci-dessous sont transférés vers le projet. Désélectionnez ceux que vous souhaitez exclure.</td> 
      <td> <p>Décochez les cases en regard des informations que vous souhaitez effacer du modèle avant de l’associer au projet. Ces informations ne sont pas transférées du modèle au projet. Pour plus d’informations sur chaque champ, voir <a href="../../../manage-work/projects/create-and-manage-templates/attach-template-to-project-overview.md" class="MCXref xref">Présentation de l’association d’un modèle à un projet</a>. </p> <p>Important : Si vous cochez la case <strong>Configuration des propriétés et des problèmes de la file d’attente</strong> , les détails de la file d’attente du modèle remplacent ceux du projet. Dans ce cas, les règles de routage, les rubriques de file d’attente et les groupes de rubriques du modèle sont ajoutés à ceux du projet. <br>Si le projet est configuré en tant que file d’attente des demandes et que le modèle que vous joignez au projet n’est pas configuré en tant que file d’attente des demandes, les informations de la file d’attente du projet sont supprimées si vous laissez la variable <strong>Configuration des propriétés et des problèmes de la file d’attente</strong> case cochée. <br>Si vous désélectionnez l’option <strong>Propriétés de la file d’attente et configuration des problèmes</strong> , tous les paramètres de configuration de la file d’attente du projet sont conservés et aucun paramètre de configuration de la file d’attente du modèle n’est joint. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p role="rowheader" colspan="2">Section Forms personnalisée</p> <p role="rowheader" colspan="2"> <img src="assets/attach-template-large-box-custom-forms-section-nwe-350x274.png" style="width: 350;height: 274;"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Forms personnalisée</td> 
      <td> <p>Lorsque des formulaires personnalisés sont joints au modèle, leurs noms s’affichent dans le panneau de gauche. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Facultatif) Mettez à jour les informations dans les formulaires personnalisés. Ces informations sont transférées au projet.

   >[!TIP]
   >
   >* Cette étape est obligatoire lorsque les formulaires personnalisés du modèle contiennent des champs obligatoires vides.
   >* Si les champs du modèle de formulaires personnalisés existent déjà sur le projet et contiennent des informations, ils conservent les informations déjà présentes sur le projet. Vous ne pouvez pas les modifier lors de l’association du modèle.

1. Cliquez sur **Joindre un modèle.**
1. Cliquez sur **Annuler la pièce jointe** pour arrêter de joindre le modèle.

   Ou

   Autoriser la fin de la pièce jointe pour ajouter le modèle au projet.

   Après avoir joint le modèle, vous pouvez modifier le projet et ajuster les tâches, informations ou paramètres, le cas échéant.

1. (Facultatif) Cliquez sur **Détails du projet**, puis **Présentation** pour afficher le nom du modèle que vous avez joint dans le **Relations avec le projet** zone.

   >[!TIP]
   >
   >Si vous joignez plusieurs modèles au projet, seul le modèle que vous avez joint s’affiche en premier dans ce champ. Pour plus d’informations, voir [Ajout de plusieurs modèles à un projet existant et affichage des informations de modèle](#attach-multiple-templates-to-an-existing-project-and-view-template-information) dans cet article.

1. (Facultatif) Supprimez les informations de modèle du projet auquel vous avez joint le modèle. Pour plus d’informations, voir [Suppression des informations de modèle d’un projet](../../../manage-work/projects/create-and-manage-templates/remove-template-from-project.md).

## Ajout de plusieurs modèles à un projet existant et affichage des informations de modèle {#attach-multiple-templates-to-an-existing-project-and-view-template-information}

Vous pouvez joindre plusieurs modèles (un par un) au même projet, en suivant les étapes décrites dans la section . [Joindre un modèle à un projet existant](#attach-a-template-to-an-existing-project) dans cet article. Les tâches et autres informations de chaque modèle sont ainsi ajoutées au projet.

>[!TIP]
>
>Lorsque vous joignez plusieurs modèles à un projet, seul celui que vous avez joint s’affiche pour la première fois dans la zone Détails du projet .

Pour comprendre quel modèle est appliqué à un projet :

1. Accédez à un projet auquel est associé un modèle.
1. Cliquez sur **Détails du projet** dans le panneau de gauche.
1. Recherchez le nom du modèle associé au projet dans la section **Modèle** au bas du champ **Présentation** section sous **Relations avec le projet** .

   ![](assets/nwe-template-info-on-project-350x356.png)


