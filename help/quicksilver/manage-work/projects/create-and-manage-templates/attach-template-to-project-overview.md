---
content-type: overview
product-area: templates
keywords: remplacer,champ,remplacé
navigation-topic: templates-navigation-topic
title: Vue d’ensemble d’un modèle joint à un projet
description: Lorsque vous joignez un modèle à un projet existant, vous modifiez certaines informations du projet en fonction de celles du modèle. Certaines informations du projet restent inchangées.
author: Alina
feature: Work Management
exl-id: 7f0137b6-ce8e-4b66-ad55-e6dc2aae09d9
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '1258'
ht-degree: 95%

---

# Vue d’ensemble d’un modèle joint à un projet

Lorsque vous joignez un modèle à un projet existant, vous modifiez certaines informations du projet en fonction de celles du modèle. Certaines informations du projet restent inchangées.

Pour plus d’informations sur la façon de joindre un modèle à un projet, voir [Joindre un modèle à un projet](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

## Éléments à prendre en compte concernant l’ajout de modèles à des projets

Tenez compte des éléments suivants lorsque vous ajoutez des modèles aux projets :

* Vous ne pouvez joindre que des modèles actifs aux projets.
* Vous pouvez joindre un modèle à un projet lorsque le statut du projet est défini sur Terminé, À l’arrêt ou En attente d’approbation, uniquement lorsque votre administrateur Adobe Workfront ou un administrateur de groupe a activé cette fonctionnalité dans les Préférences du projet. Pour plus d’informations sur la définition des préférences de projet, voir [Configurer des préférences de projet à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* À moins que vous n’excluiez des tâches de modèle spécifiques dans le processus d’association, toutes les tâches de modèle sont ajoutées au projet existant.
* La plupart des paramètres de modèle sont ajoutés au projet. Certains paramètres de projet sont conservés. Pour plus d’informations, voir la section [Comprendre les modifications apportées aux champs de projet lors de l’association d’un modèle](#understand-changes-to-project-fields-when-attaching-a-template) dans cet article.

## Comprendre les modifications apportées aux champs de projet lors de l’association d’un modèle {#understand-changes-to-project-fields-when-attaching-a-template}

>[!IMPORTANT]
>
>L’association d’un modèle à un projet n’est pas la même chose que la création d’un projet à partir d’un modèle. Lorsque vous créez un projet à partir d’un modèle, tous les champs de modèle sont transférés vers le nouveau projet. L’association d’un modèle ne modifie pas certains champs du projet existant.

Certains paramètres de modèle sont automatiquement transférés vers le projet, sauf si vous les marquez spécifiquement pour qu’ils soient exclus pendant l’association au modèle. Lorsque vous les marquez pour qu’ils soient exclus, les valeurs des champs du projet sont conservées.

Cependant, tous les champs de projet ne sont pas disponibles pour la gestion lors du processus d’association d’un modèle à un projet. Pour plus d’informations, voir [Joindre un modèle à un projet](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

Le tableau suivant décrit la valeur par défaut des champs de projet lorsque vous associez un modèle et les champs que vous pouvez gérer pendant le processus d’association pour remplacer le comportement par défaut :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>champ</td> 
   <td>Ce qui se passe par défaut dans le processus d’association d’un modèle</td> 
   <td>Possibilité de gérer les mises à jour des champs dans le processus d’association </td> 
  </tr> 
  <tr> 
   <td>Description</td> 
   <td>Les informations du projet sont conservées</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Statut</p> </td> 
   <td>Les informations du projet sont conservées</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>URL</td> 
   <td>Transféré à partir du modèle, si le champ est vide sur le projet</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Priorité</td> 
   <td>Les informations du projet sont conservées</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Type de condition</td> 
   <td>Les informations du projet sont conservées</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Mode horaire</td> 
   <td>Les informations du projet sont conservées</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Dates prévues</td> 
   <td>Changement possible en fonction des tâches ajoutées</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Dates effectives</td> 
   <td>Changement possible en fonction des tâches ajoutées</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Portfolio</td> 
   <td>Les informations du projet sont conservées</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Programme</td> 
   <td>Les informations du projet sont conservées</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Groupe</td> 
   <td>Les informations du projet sont conservées</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Entreprise</td> 
   <td>Transféré à partir du modèle, si le champ est vide sur le projet</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Heures prévues</td> 
   <td>Changement possible en fonction des tâches ajoutées</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Propriétaire du projet</td> 
   <td>Transféré à partir du modèle, si le champ est vide sur le projet</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Sponsor du projet</td> 
   <td>Transféré à partir du modèle, si le champ est vide sur le projet</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Gestionnaire des ressources</td> 
   <td>Ajouté à la liste des gestionnaires de ressources existants sur le projet</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Formulaires personnalisés</td> 
   <td>Ajouté au projet, en plus des formulaires déjà présents sur le projet</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Budget</td> 
   <td>Les informations du projet sont conservées</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Devise</td> 
   <td>Les informations du projet sont conservées</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>MIP</td> 
   <td>Les informations du projet sont conservées</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>CRE</td> 
   <td>Les informations du projet sont conservées</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Bénéfice prévu</td> 
   <td>Les informations du projet sont conservées</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Bénéfice réel</td> 
   <td>Les informations du projet sont conservées</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Chemin jalonné</td> 
   <td>Transféré à partir du modèle, si le champ est vide sur le projet</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Mode d'achèvement</td> 
   <td>Les informations du projet sont conservées</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Mode d'achèvement du sommaire</td> 
   <td>Les informations du projet sont conservées</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Type de mise à jour</td> 
   <td>Les informations du projet sont conservées</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Planning</td> 
   <td>Les informations du projet sont conservées</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Congés de l’utilisateur ou de l’utilisatrice
</td> 
   <td>Les informations du projet sont conservées</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Mode de nivellement des ressources</td> 
   <td>Les informations du projet sont conservées</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Risque (champ de projet)</td> 
   <td>Les informations du projet sont conservées</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Pools de ressources</td> 
   <td>Ajouté à la liste des groupes de ressources existants sur le projet</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Types d'heures</td> 
   <td> <p>Si cette option est désélectionnée pendant le processus d’association, le paramètre Types d’heures sur le projet reste inchangé. </p> <p>Si cette option est sélectionnée, le paramètre du modèle est transféré vers le projet. Si le filtrage Type d’heure est défini sur Oui sur le projet et le modèle, les types d’heures du modèle sont ajoutés à ceux du projet.</p> </td> 
   <td> <p> </p> <p> </p> <p> </p> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>Notifications de rappel</td> 
   <td> <p>Ajouté à la liste des rappels existants sur le projet. </p> <p>Si cette option est désélectionnée pendant le processus d’association, les notifications de rappel du projet restent inchangées. </p> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Processus d'approbation de tâche par défaut</td> 
   <td>Les informations du projet sont conservées</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Formulaires personnalisés de tâche par défaut</td> 
   <td>Les informations du projet sont conservées</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Effort de travail</td> 
   <td>Les informations du projet sont conservées</td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td><span>Autoriser les utilisateurs et utilisatrices à ajouter des problèmes en ligne</span> </td> 
   <td><span>Les informations du projet sont conservées</span> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tous les paramètres</td> 
   <td>Les paramètres du modèle remplacent ceux du projet.</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tâches</td> 
   <td>Ajout au bas de la liste des tâches, en plus des tâches de projet existantes</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Documents</td> 
   <td>Ajout au projet, en plus des documents de projet existants</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Risques (objets dans la zone Risques du projet)</td> 
   <td>Ajout au projet, en plus des risques existants du projet </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Processus d’approbation</td> 
   <td>Transféré à partir du modèle</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Taux de facturation</td> 
   <td> <p>Transféré depuis le modèle en plus des taux de facturation existants sur le projet. </p> <p>S’il existe un taux différent pour la même fonction sur le projet et le modèle, le taux sur le projet reste inchangé. </p> </td> 
   <td> <p> </p> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>Enregistrements de facturation</td> 
   <td>Les informations du projet sont conservées</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Frais</td> 
   <td>Transféré à partir du modèle en plus des dépenses existantes sur le projet</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Informations financières</td> 
   <td> <p>Lorsque cette option est sélectionnée dans le processus de pièce jointe, les champs suivants sont transférés ou ajoutés au projet : </p> 
    <ul> 
     <li> <p>Coûts fixes</p> <p>Lorsque l’option est sélectionnée, le coût fixe du projet mis à jour est calculé à l’aide de la formule suivante :</p> <p><code>Updated Project Fixed Cost = Original Project Fixed Cost + Template Fixed Cost</code> </p> </li> 
     <li> <p>Revenus fixes</p> <p>Lorsque cette option est sélectionnée, les revenus fixes du projet mis à jour sont calculés à l’aide de la formule suivante :</p> <p><code>Updated Project Fixed Revenue = Original Project Fixed Revenue + Template Fixed Revenue </code> </p> </li> 
     <li> <p>Type de coût pour les tâches</p> <p>Transféré à partir du modèle</p> </li> 
     <li> <p>Type de revenu pour les tâches</p> <p>Transféré à partir du modèle</p> </li> 
    </ul> <p>Si ce champ est désélectionné pendant le processus de mise en pièce jointe, les événements suivants se produisent :</p> 
    <ul> 
     <li> <p>Le coût fixe et les revenus fixes du projet sont conservés.</p> </li> 
     <li> <p>Les types de coût et de revenu des tâches ajoutées à partir du modèle sont définis sur Aucun coût et Non facturable.</p> </li> 
    </ul> </td> 
   <td> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>Heures</td> 
   <td>Les informations du projet sont conservées</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Détails de la file d’attente, groupes de rubriques, rubriques de la file d’attente, règles de transmission</td> 
   <td> <p>Transféré à partir du modèle</p> <p>Si vous sélectionnez l’option <strong>Propriétés de file d’attente et configuration des problèmes</strong> pendant le processus d’association, les détails de la file d’attente du modèle remplacent ceux du projet. Dans ce cas, les règles de routage, les rubriques de file d’attente et les groupes de rubriques de file d’attente du modèle sont ajoutés à ceux du projet. <br>Si le projet est configuré en tant que file d’attente des demandes et que le modèle que vous joignez au projet n’est pas configuré en tant que file d’attente des demandes, les informations de la file d’attente du projet sont supprimées si vous laissez la case <strong>Propriétés de file d’attente et configuration des problèmes</strong> cochée. <br>Si vous décochez la case <strong>Propriétés de file d’attente et configuration des problèmes</strong>, tous les paramètres de configuration de la file d’attente du projet sont conservés et aucun paramètre de configuration de la file d’attente du modèle n’est joint.</p> </td> 
   <td> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>Contraintes de tâche</td> 
   <td> <p>Transféré à partir du modèle </p> <p>Si cette option est désélectionnée pendant le processus d’association, les contraintes de tâche sont définies sur Aussi Tôt Que Possible ou Aussi Tard Que Possible en fonction le paramètre « Planifier à partir de » du projet. </p> </td> 
   <td> <p> </p> <p> </p> <p style="text-align: center;">✓</p> </td> 
  </tr> 
  <tr> 
   <td>Tâches antérieures</td> 
   <td> <p>Transféré à partir du modèle</p> <p>Si cette option est désélectionnée pendant le processus d’association, toutes les connexions d’antériorité entre les tâches du modèle sont supprimées.</p> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Options de partage</td> 
   <td> <p>Si cette option est désélectionnée pendant le processus d’association, les autorisations de projet restent inchangées.</p> <p>Si cette option est sélectionnée pendant le processus d’association, les autorisations de modèle sont ajoutées ou remplacent celles du projet. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemple : </b></span></span>si l’utilisateur ou l’utilisatrice A dispose de l’autorisation d’affichage sur le projet, mais qu’il ou elle dispose de l’autorisation de gestion sur le modèle, après avoir joint le modèle, l’utilisateur ou l’utilisatrice A aura accès en gestion au projet.</p> </td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>



<!--WRITER
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<div>
<h2> </h2>
<h2>Understand changes to project fields when attaching a template</h2> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted and replaced with the table above, per Anna)</p>
-->
<!--
<p>Some template settings automatically transfer to the project, unless you specifically mark them to be excluded during the template attachment process. When you mark them to be excluded, the project field values are preserved. </p> <note type="important">
Not all project fields are available to manage in the process of attaching a template to a project. For information, see
<a href="../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md" class="MCXref xref">Attach a template to a project</a>.
</note>
<p>The following scenarios exist when attaching a template to an existing project: </p>
<ul>
<li> <p><a href="#project-fields-that-are-empty-and-the-template-information-updates-them" class="MCXref xref">Project fields that are empty and the template information updates them</a> </p> </li>
<li> <p><a href="#project-fields-that-are-populated-and-the-template-information-overwrites-them" class="MCXref xref">Project fields that are populated and the template information overwrites them</a> </p> </li>
<li> <p><a href="#project-fields-that-are-populated-and-they-remain-unchanged-after-attaching-the-template" class="MCXref xref">Project fields that are populated and they remain unchanged after attaching the template</a> </p> </li>
</ul> <note type="important">
Attaching a template to a project is not the same as creating a project from a template. When you create a project from a template all template fields transfer to the new project. Attaching a template leaves some of the existing project's fields unchanged.
</note>
<p><strong>Project fields that are empty and the template information updates them</strong></p>
<p>Most project fields that are empty are populated with template information when attaching the template to an existing project. </p>
<p><strong>Project fields that are populated and the template information overwrites them</strong></p>
<p>The following fields always overwrite or update existing project information with template information when you attach a template to the project and they cannot be managed during attaching the template: </p>
<ul>
<li> <p><b>Resource manager</b>: The template Resource Managers are added to the list of existing resource managers on the project.</p> </li>
</ul>
<ul>
<li> <p><b>Financial Information</b>: You can indicate whether you want financial information to transfer from the template or to keep the existing financial information on the project in the process of attaching a template. However, when the Financial Information option is selected to indicate that you intend to keep the information from the template, the following fields are updated on the project: </p>
<ul>
<li> <p> The updated Fixed Cost of the project is calculated using the following formula:</p> <p><code>Updated Project Fixed Cost = Original Project Fixed Cost + Template Fixed Cost</code> </p> </li>
<li> <p>The updated Fixed Revenue of the project is calculated using the following formula:</p> <p><code>Updated Project Fixed Revenue = Original Project Fixed Revenue + Template Fixed Revenue </code> </p> </li>
</ul> </li>
</ul>
<ul>
<li> <p><b>Filter Hour Types</b> </p> </li>
</ul>
<ul>
<li> <p><b>Access settings</b> </p> </li>
</ul>
<ul>
<li> <p><b>Custom Forms</b>: Template custom forms are added to the project, in addition to existing project custom forms. If the fields from the template custom forms already exist on the project and contain information, they preserve the information already on the project. You cannot edit them during attaching the template. </p> </li>
</ul>
<ul>
<li> <p><b>Start From</b> </p> </li>
</ul>
<p><strong>Project fields that are populated and they remain unchanged after attaching the template</strong></p>
<p>The following fields remain unchanged on the project, even if they are also populated on the template, and they cannot be managed during attaching the template: </p>
<ul>
<li> <p style="font-weight: bold;">URL</p> </li>
<li> <p style="font-weight: bold;">Project Owner</p> </li>
<li> <p style="font-weight: bold;">Project Sponsor</p> </li>
<li> <p style="font-weight: bold;">Group</p> </li>
<li> <p style="font-weight: bold;">Company</p> </li>
<li> <p style="font-weight: bold;">Currency</p> </li>
<li> <p style="font-weight: bold;">Milestone Path</p> </li>
<li> <p><b>Completion Mode</b> </p> </li>
<li> <p style="font-weight: bold;">Resource Pool</p> </li>
<li> <p style="font-weight: bold;">Tasks Settings fields</p> </li>
<li class="preview" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p style="font-weight: bold;">Issue Settings fields</p> </li>
</ul>
</div>
<p> </p>
</div>
-->


