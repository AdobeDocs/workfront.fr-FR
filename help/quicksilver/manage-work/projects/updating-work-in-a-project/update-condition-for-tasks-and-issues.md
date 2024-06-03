---
product-area: projects
navigation-topic: update-work-in-a-project
title: Mettre à jour la condition des tâches et des problèmes
description: La condition d’une tâche ou d’un problème est un indicateur qui y est placé pour indiquer comment elle se déroule. Il s’agit d’un état différent de celui de l’élément de travail, qui indique l’étape actuelle du développement de l’élément.
author: Alina
feature: Work Management
exl-id: 5d970af6-5996-4781-9b97-de02063dc32c
source-git-commit: 330ee20ad14ea7409db1c6f627ed6aa0e0c5c014
workflow-type: tm+mt
source-wordcount: '1032'
ht-degree: 6%

---

# Mettre à jour la condition des tâches et des problèmes

{{highlighted-preview}}

La condition d’une tâche ou d’un problème est un indicateur qui y est placé pour indiquer comment elle se déroule. Il s’agit d’un état différent de celui de l’élément de travail, qui indique l’étape actuelle du développement de l’élément.

Vous pouvez définir la condition d’une tâche ou d’un problème automatiquement ou manuellement.

Les valeurs de condition auxquelles nous faisons référence dans cet article sont disponibles par défaut dans Workfront. Votre administrateur Adobe Workfront peut créer des conditions personnalisées pour votre environnement, comme décrit dans la section [Création ou modification d’une condition personnalisée](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

## Conditions d’accès {#access-requirements}

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td>

Pour les nouvelles licences :
<ul><li><p>Standard pour les tâches</p></li>
   <li><p>Contributeur ou version ultérieure pour les problèmes</p></li></ul>


Pour les licences actuelles :
<ul><li><p>Travail ou plus pour les tâches</p></li>
   <li><p>Demande ou version ultérieure pour les problèmes</p></li></ul>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Affichage ou accès supérieur aux projets</p> <p>Modifier l’accès aux tâches et aux problèmes </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Affichage ou autorisations supérieures sur des tâches et des problèmes pour afficher leur condition</p>
   <p>Gérer les autorisations sur les tâches et les problèmes pour mettre à jour la condition</p>
  </td> 
  </tr> 
 </tbody> 
</table>

* Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront. Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Conditions préalables

Vous devez être affecté à une tâche ou à un problème pour pouvoir mettre à jour manuellement sa condition.

## Localisation de la condition des tâches et des problèmes

Les conditions s’affichent sous la forme d’un indicateur associé à des tâches ou des problèmes. Elles peuvent également être associées à un nombre qui peut s’afficher dans les rapports au lieu du libellé. Pour plus d’informations sur l’association de conditions à des nombres, voir [Création ou modification d’une condition personnalisée](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

Vous pouvez localiser la condition des tâches et des problèmes dans les zones suivantes de Workfront :

* <span class="preview">La page Détails , une fois qu’un administrateur de Workfront ou de groupe l’a ajoutée à votre modèle de mise en page. Pour plus d’informations, voir [Personnalisation de la vue Détails à l’aide d’un modèle de mise en page](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md). </span>

* <span class="preview">L’en-tête d’une tâche ou d’un problème, après qu’un administrateur de Workfront ou de groupe l’ait ajoutée à votre modèle de mise en page. Pour plus d’informations, voir [Personnalisation des en-têtes d’objet à l’aide d’un modèle de mise en page](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md). </span>

* Le panneau Résumé, une fois qu’un administrateur de Workfront ou de groupe l’a ajouté à votre modèle de mise en page. Pour plus d’informations, voir [Personnalisation de l’accueil et du résumé à l’aide d’un modèle de mise en page](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md).

* Rapports et listes lorsque vous affichez le champ Condition dans une vue ou un groupement.

  >[!NOTE]
  >
  >Lorsque le mot &quot;condition&quot; s’affiche dans le champ Nom du champ d’un rapport Entrée de journal, cela indique que la condition d’un élément a été mise à jour. Lorsque le champ Condition est suivi dans les rapports Entrées du journal , les valeurs Nouveau et Ancien nombre affichent le numéro associé à la condition au lieu de son nom. Si une condition n’est pas définie à l’origine pour une tâche ou un problème et que vous la mettez à jour ultérieurement, l’entrée de journal qui capture la mise à jour affichera la valeur Ancien numéro du champ Condition comme suit : -2 147 483 648.

## Mettre automatiquement à jour la condition en mettant à jour l’état

Lorsque vous avez une tâche ou un problème, cliquez sur **Travailler dessus** , Démarrer la tâche ou Démarrer le problème, ou mettre à jour son état, la condition de la tâche ou du problème passe automatiquement à la condition par défaut associée à **En douceur**.

Pour plus d’informations sur l’utilisation d’une condition personnalisée comme condition par défaut, voir les articles  [Définir une condition personnalisée comme condition par défaut pour les tâches et les problèmes](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md) et [Définir une condition personnalisée comme condition par défaut pour les projets](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md).

Pour plus d’informations sur la modification de l’état de la tâche, voir [Mettre à jour le statut des tâches](../../../manage-work/projects/updating-work-in-a-project/update-task-status.md).

Pour plus d’informations sur la modification de l’état du problème, voir [Mettre à jour le statut du problème](../../../manage-work/projects/updating-work-in-a-project/update-issue-status.md).

Pour plus d’informations sur la définition du bouton Travailler dessus sur un bouton Démarrer la tâche ou Démarrer le problème, voir [Remplacez le bouton Travailler dessus par un bouton Démarrer](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).

## Mettre à jour manuellement la condition

Vous devez être affecté à une tâche ou au problème ou disposer des autorisations de gestion pour pouvoir définir la condition sur celle-ci.

Vous pouvez mettre à jour manuellement la condition d’une tâche ou d’un problème dans un rapport de tâche ou de problème ou une liste lorsque vous affichez le champ Condition dans la vue.

>[!NOTE]
>
>Vous pouvez demander à votre administrateur système ou de groupe d’ajouter le champ Condition à votre panneau Résumé, afin de faciliter sa mise à jour dans différentes zones de Workfront.
>
>Pour plus d’informations, voir les articles suivants :
>
>* [Aperçu du résumé](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)
>* [Personnalisation de l’accueil et du résumé à l’aide d’un modèle de mise en page](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md).


<!--old Condition update - in the commenting stream: 
Updating the Condition of a task or issue differs depending on whether you are assigned to it or not:

* If you are using the legacy commenting experience, you can update the Condition in the Updates tab or in a list of tasks or issues if you are assigned to them. This is not supported in the new commenting experience. For information, see [New commenting experience](/help/quicksilver/product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 
* You can update the Condition in a list of tasks or issues if you are not assigned to them, only if you have Manage permissions to them. In this case, you cannot update the Condition in the Update tab of the task or issue. -->

Pour mettre à jour manuellement la condition d’une tâche ou d’un problème, effectuez l’une des opérations suivantes :

<div class="preview">

1. Pour mettre à jour la condition d’une tâche ou d’un problème dans l’en-tête de la tâche ou du problème :

   1. (Conditionnel) Si votre administrateur Workfront ou de groupe a ajouté le champ Condition à l’en-tête de tâche ou de problème de votre modèle de mise en page, cliquez sur le bouton **Condition** dans l’en-tête et sélectionnez l’une des options suivantes :
      * Tout est en ordre
      * Certaines inquiétudes
      * Obstacles majeurs

      ![](assets/condition-in-task-header.png)
   1. Cliquez sur Entrée pour enregistrer la condition.

1. Pour mettre à jour la condition d’une tâche ou d’un problème dans la section Détails de la tâche ou du problème :

   1. (Conditionnel) Si votre administrateur Workfront ou de groupe a ajouté le champ Condition à la section Détails d’une tâche ou d’un problème dans votre modèle de mise en page, cliquez sur **Détails** dans le panneau de gauche, puis cliquez sur le bouton **Condition** et sélectionnez l’une des options suivantes :
      * Tout est en ordre
      * Certaines inquiétudes
      * Obstacles majeurs
1. Cliquez sur **Enregistrer les modifications**. La condition de la tâche ou du problème est mise à jour.

</div>

Pour mettre à jour la condition d’une tâche ou d’un problème dans un rapport ou une liste :

1. Accédez à la liste des tâches ou problèmes auxquels vous disposez des autorisations de gestion . Assurez-vous que la variable **Condition** est visible dans la vue de la liste.

1. Mettez à jour le **Condition** du problème ou de la tâche en ligne, en double-cliquant sur la condition existante et en sélectionnant une nouvelle valeur dans le menu déroulant.

   ![](assets/condition-drop-down-values-in-task-list.png)

   >[!NOTE]
   >
   >Les conditions peuvent être personnalisées pour votre environnement. Vous pouvez donc trouver plus de trois options pour Condition dans votre environnement. Les noms des Conditions peuvent être différents de ceux répertoriés ci-dessus. Pour plus d’informations sur la personnalisation des conditions dans Workfront, voir [Création ou modification d’une condition personnalisée](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).


1. Presse **Entrée** sur votre clavier ou cliquez en dehors du champ Condition pour enregistrer la nouvelle tâche ou émettre la condition.

<!--   
<li><p>(NOTE: drafted because I can't do this anymore)</p><p>If you have Manage permissions to the task or issue but are not assigned to it, perhaps as a project manager, add the <strong>Condition</strong> column to any view you use in a task or issue list, then set the <strong>Condition</strong> in inline edit and press Enter.</p><p><img src="assets/change-condition-in-list-view-350x142.png" style="width: 350;height: 142;"></p><p>For information about adding a column to a view, see <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md">Views overview in Adobe Workfront</a>.</p></li>   
     -->


