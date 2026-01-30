---
product-area: projects
navigation-topic: update-work-in-a-project
title: Mettre à jour la condition pour les tâches et les événements
description: La condition d’une tâche ou d’un problème est un indicateur qui y est placé pour indiquer son déroulement. Il s’agit d’un statut différent de celui de l’élément de travail, qui indique l’étape actuelle du développement de l’élément.
author: Alina
feature: Work Management
exl-id: 5d970af6-5996-4781-9b97-de02063dc32c
source-git-commit: 885bdb0e28c2807f14cc3919a3057a4a48b2422d
workflow-type: tm+mt
source-wordcount: '1070'
ht-degree: 79%

---

# Mettre à jour la condition pour les tâches et les problèmes

<!--Audited: 07/2024-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers, or in the Production environment for customers who enabled fast releases.</span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">For information about the current release, see [Third Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md).</span>-->

La condition d’une tâche ou d’un problème est un indicateur qui y est placé pour indiquer son déroulement. Il s’agit d’un statut différent de celui de l’élément de travail, qui indique l’étape actuelle du développement de l’élément.

Vous pouvez définir la condition d’une tâche ou d’un problème automatiquement ou manuellement.

Les valeurs de condition auxquelles nous faisons référence dans cet article sont disponibles par défaut dans Workfront. Votre administrateur ou administratrice Adobe Workfront peut créer des conditions personnalisées pour votre environnement, comme décrit dans [Créer ou modifier une condition personnalisée](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

## Conditions d’accès {#access-requirements}

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
   <td> 
   <ul><li><p>Standard pour les tâches</p></li>
   <li><p>Contribution ou licence supérieure pour les problèmes</p></li></ul>
  <p>Ou</p>
   <ul><li><p>Travail ou licence supérieure plus pour les tâches</p></li>
   <li><p>Demande ou niveau supérieur pour les problèmes</p></li></ul>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès en affichage ou supérieur aux projets</p> <p>Accès en modification aux tâches et aux problèmes </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations d’affichage ou supérieures sur les tâches et les problèmes afin de visualiser leur condition</p>
   <p>Autorisations de contribution sur les tâches et les événements pour mettre à jour la condition</p>
  </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> 
   New:
   <ul><li><p>Standard for tasks</p></li>
   <li><p>Contributor or higher for issues</p></li></ul>
   Current:
   <ul><li><p>Work or higher for tasks</p></li>
   <li><p>Request or higher for issues</p></li></ul>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>View or higher access to projects</p> <p>Edit access to tasks and issues </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions on tasks and issues to view their Condition</p>
   <p>Contribute permissions on tasks and issues to update the Condition</p>
  </td> 
  </tr> 
 </tbody> 
</table>-->

## Conditions préalables

Une tâche ou un problème doit vous être affecté pour pouvoir mettre à jour manuellement sa condition.

## Localiser la condition des tâches et des problèmes

Les conditions s’affichent sous la forme d’un indicateur associé à des tâches ou des problèmes. Elles peuvent également être associées à un nombre qui peut s’afficher dans les rapports au lieu du libellé. Pour plus d’informations sur l’association de conditions à des nombres, voir [Créer ou modifier une condition personnalisée](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

Vous pouvez retrouver la condition des tâches et des problèmes dans les zones suivantes de Workfront :

* La page Détails, une fois qu’un administrateur Workfront ou de groupe l’a ajoutée à votre modèle de mise en page. Pour plus d’informations, voir [Personnaliser la vue Détails à l’aide d’un modèle de mise en page](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

* En-tête d’une tâche ou d’un événement, ajouté par un administrateur Workfront ou un administrateur de groupes à votre modèle de mise en page. Pour plus d’informations, voir [Personnaliser les en-têtes d’objets à l’aide d’un modèle de mise en page](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

* Panneau Résumé, une fois qu’un administrateur ou une administratrice Workfront ou de groupes l’a ajouté à votre modèle de mise en page. Pour plus d’informations, voir [Personnaliser le panneau Résumé à l’aide d’un modèle de disposition](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md).

* Rapports et listes lorsque vous affichez le champ Condition dans une vue ou un regroupement.

  >[!NOTE]
  >
  >Lorsque le mot « condition » s’affiche dans le champ Nom du champ d’un rapport Entrée de journal, cela indique que la condition d’un élément a été mise à jour. Lorsque le champ Condition est suivi dans les rapports Entrées de journal, les valeurs Nouveau et Ancien nombre affichent le numéro associé à la condition au lieu de son nom. Si une condition n’est pas définie à l’origine pour une tâche ou un problème et que vous la mettez à jour ultérieurement, l’entrée de journal qui capture la mise à jour affichera la valeur Ancien numéro du champ Condition comme suit : -2 147 483 648.

## Mettre automatiquement à jour la condition en mettant à jour le statut

Lorsque une tâche ou un problème vous est affecté et que vous cliquez sur **Travailler dessus**, Démarrer la tâche ou Démarrer le problème, ou mettre à jour son statut, la condition de la tâche ou du problème passe automatiquement à la condition par défaut associée à **Tout est en ordre**.

Pour plus d’informations sur l’utilisation d’une condition personnalisée comme condition par défaut, voir les articles [Définir une condition personnalisée comme condition par défaut pour les tâches et les problèmes](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md) et [Définir une condition personnalisée comme condition par défaut pour les projets](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md).

Pour plus d’informations sur la modification du statut de la tâche, voir [Mettre à jour le statut de la tâche](../../../manage-work/projects/updating-work-in-a-project/update-task-status.md).

Pour plus d’informations sur la modification du statut du problème, voir [Mettre à jour le statut du problème](../../../manage-work/projects/updating-work-in-a-project/update-issue-status.md).

Pour plus d’informations sur la définition du bouton Travailler dessus sur un bouton Démarrer la tâche ou Démarrer le problème, voir [Remplacer le bouton Travailler dessus par un bouton Démarrer](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).

## Mettre à jour manuellement la condition

Une tâche ou au problème doit vous être affecté ou vous devez disposer des autorisations de gestion pour pouvoir définir sa condition.

Vous pouvez mettre à jour manuellement la condition d’une tâche ou d’un problème dans un rapport de tâche ou de problème ou une liste lorsque vous affichez le champ Condition dans la vue.

>[!NOTE]
>
>Vous pouvez demander à l’administrateur de votre système ou de votre groupe d’ajouter le champ Condition à votre panneau Résumé ou aux pages d’en-tête de tâche ou d’événement ou de Détails.
>
>Pour plus d’informations, consultez les articles suivants :
>
>* [Vue d’ensemble du résumé](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)
>* [Personnaliser le panneau Résumé à l’aide d’un modèle de disposition](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md).


<!--old Condition update - in the commenting stream: 
Updating the Condition of a task or issue differs depending on whether you are assigned to it or not:

* If you are using the legacy commenting experience, you can update the Condition in the Updates tab or in a list of tasks or issues if you are assigned to them. This is not supported in the new commenting experience. For information, see [New commenting experience](/help/quicksilver/product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 
* You can update the Condition in a list of tasks or issues if you are not assigned to them, only if you have Manage permissions to them. In this case, you cannot update the Condition in the Update tab of the task or issue. -->

Vous pouvez mettre à jour manuellement le statut des tâches et des événements dans différentes zones de Workfront. Les sections suivantes décrivent comment mettre à jour manuellement le statut des tâches et des événements.

### Mettre à jour la condition d’une tâche ou d’un événement dans l’en-tête de la tâche ou de l’événement

1. (Le cas échéant) Si votre administrateur ou administratrice Workfront ou de groupes a ajouté le champ Condition à l’en-tête de la tâche ou du problème de votre modèle de mise en page, cliquez sur le champ **Condition** dans l’en-tête et sélectionnez l’une des options suivantes :
   * Tout est en ordre
   * Certaines inquiétudes
   * Obstacles majeurs

   ![Condition dans l’en-tête de la tâche](assets/condition-in-task-header-0925.png)

<!--1. Click Enter to save the Condition.-->

### Mettez à jour le statut d’une tâche ou d’un événement dans la section Détails de la tâche ou de l’événement

1. (Le cas échéant) Si votre administrateur ou administratrice Workfront ou de groupes a ajouté le champ Condition à la section Détails d’une tâche ou d’un problème dans votre modèle de mise en page, cliquez sur **Détails** dans le panneau de gauche, puis cliquez sur **Condition de tâche** ou **Condition de problème** et sélectionnez l’une des options suivantes :
   * Tout est en ordre
   * Certaines inquiétudes
   * Obstacles majeurs
1. Cliquez sur Enregistrer les modifications. **&#x200B;**&#x200B;La condition de la tâche ou du problème est mise à jour.

### Mettre à jour le statut d&#39;une tâche ou d&#39;un événement dans un rapport ou une liste

1. Accédez à la liste des tâches ou problèmes auxquels vous disposez des autorisations de gestion. Assurez-vous que le champ **Condition** est visible dans la vue de la liste.

1. Mettez à jour la **Condition** du problème ou de la tâche en ligne, en double-cliquant sur la condition existante et en sélectionnant une nouvelle valeur dans le menu déroulant.

   ![Valeurs de condition dans la liste des tâches](assets/condition-values-in-task-list-0925.png)

   >[!NOTE]
   >
   >Les conditions peuvent être personnalisées en fonction de votre environnement. Il est donc possible que vous trouviez plus de trois options pour les conditions dans votre environnement. Les noms des conditions peuvent être différents de ceux énumérés ci-dessus. Pour plus d’informations sur la personnalisation des conditions dans Workfront, voir [Créer ou modifier une condition personnalisée](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

1. Appuyez sur la touche **Entrée** de votre clavier ou cliquez en dehors du champ Condition pour enregistrer la nouvelle condition de la tâche ou du problème.

   >[!NOTE]
   >
   >Dans l’affichage Condition par défaut, le champ **Condition** est un type de champ qui ne peut pas être modifié en ligne. Lorsque vous ajoutez le champ **Condition** séparément à une vue, il est modifiable. Pour plus d’informations sur la modification en ligne, voir [Modification en ligne d’éléments d’une liste dans Adobe Workfront](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md).

<!--   
<li><p>(NOTE: drafted because I can't do this anymore)</p><p>If you have Manage permissions to the task or issue but are not assigned to it, perhaps as a project manager, add the <strong>Condition</strong> column to any view you use in a task or issue list, then set the <strong>Condition</strong> in inline edit and press Enter.</p><p><img src="assets/change-condition-in-list-view-350x142.png" style="width: 350;height: 142;"></p><p>For information about adding a column to a view, see <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md">Views overview in Adobe Workfront</a>.</p></li>   
     -->


