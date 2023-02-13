---
product-area: projects
navigation-topic: update-work-in-a-project
title: Mise à jour de la condition pour les tâches et les problèmes
description: La condition d’une tâche ou d’un problème est un indicateur qui y est placé pour indiquer comment elle se déroule. Il s’agit d’un état différent de celui de l’élément de travail, qui indique l’étape actuelle du développement de l’élément.
author: Alina
feature: Work Management
exl-id: 5d970af6-5996-4781-9b97-de02063dc32c
source-git-commit: 6bb6b834c5af8ad48179fc0d60b184d083b360e4
workflow-type: tm+mt
source-wordcount: '866'
ht-degree: 0%

---

# Mise à jour de la condition pour les tâches et les problèmes

La condition d’une tâche ou d’un problème est un indicateur qui y est placé pour indiquer comment elle se déroule. Il s’agit d’un état différent de celui de l’élément de travail, qui indique l’étape actuelle du développement de l’élément.

Vous pouvez définir la condition d’une tâche ou d’un problème automatiquement ou manuellement.

L’administrateur d’Adobe Workfront peut créer des conditions personnalisées pour votre environnement, comme décrit dans la section [Création ou modification d’une condition personnalisée](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md)

<!--You can manually update the Condition of a task or issue if you are assigned to it or if you have permissions to it, as described in the [Access requirements](#access-requirements) section of this article.-->

## Exigences d’accès {#access-requirements}

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> 
   
   For the current licenses:
   <ul><li><p>Standard for tasks</p></li>
   <li><p>Contributor or higher for issues</p></li></ul>


   For legacy licenses:
   <ul><li><p>Work or higher for tasks</p></li>
   <li><p>Request or higher for issues</p></li></ul>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to projects</p> <p>Edit access to tasks and issues </p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions on tasks and issues to view their Condition</p>
   <p>Manage permissions on tasks and issues to update the Condition</p>
    <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Travail ou plus pour les tâches</p>
   <p>Demande ou version ultérieure pour les problèmes</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Affichage ou accès supérieur aux projets</p> <p>Modifier l’accès aux tâches et aux problèmes </p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Affichage ou autorisations supérieures sur des tâches et des problèmes pour afficher leur condition</p>
   <p>Gérer les autorisations sur les tâches et les problèmes pour mettre à jour la condition</p>
    <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Localisation de la condition des tâches et des problèmes

Les conditions s’affichent sous la forme d’un indicateur associé à des tâches ou des problèmes. Elles peuvent également être associées à un nombre qui peut s’afficher dans les rapports au lieu du libellé. Pour plus d’informations sur l’association de conditions à des nombres, voir [Création ou modification d’une condition personnalisée](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

Vous pouvez localiser la condition des tâches et des problèmes dans les zones suivantes :

* Zone Tâche et publication Mises à jour , dans une mise à jour, lorsque vous êtes affecté à la tâche ou au problème.
* Rapports et listes lorsque vous affichez le champ Condition dans une vue ou un groupement.

>[!NOTE]
>
>Lorsque le mot &quot;condition&quot; s’affiche dans le champ Nom du champ d’un rapport Entrée de journal, cela indique que la condition d’un élément a été mise à jour. Lorsque le champ Condition est suivi dans les rapports Entrées du journal , les valeurs Nouveau et Ancien nombre affichent le numéro associé à la condition au lieu de son nom. Si une condition n’est pas définie à l’origine pour une tâche ou un problème et que vous la mettez à jour ultérieurement, l’entrée de journal qui capture la mise à jour affichera la valeur Ancien numéro du champ Condition comme suit : -2 147 483 648.

## Mettre automatiquement à jour la condition en mettant à jour l’état

Lorsque vous avez une tâche ou un problème, cliquez sur **Travailler dessus** , Démarrer la tâche ou Démarrer le problème, ou mettre à jour son état, la condition de la tâche ou du problème passe automatiquement à la condition par défaut associée à **En douceur**.

Pour plus d’informations sur l’utilisation d’une condition personnalisée comme condition par défaut, voir les articles  [Définition d’une condition personnalisée comme condition par défaut pour les tâches et les problèmes](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md) et [Définition d’une condition personnalisée comme condition par défaut pour les projets](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md).

Pour plus d’informations sur la modification de l’état de la tâche, voir [Mettre à jour le statut des tâches](../../../manage-work/projects/updating-work-in-a-project/update-task-status.md).

Pour plus d’informations sur la modification de l’état du problème, voir [Mettre à jour le statut du problème](../../../manage-work/projects/updating-work-in-a-project/update-issue-status.md).

Pour plus d’informations sur la définition du bouton Travailler dessus sur un bouton Démarrer la tâche ou Démarrer le problème, voir [Remplacez le bouton Travailler dessus par un bouton Démarrer](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).

## Mettre à jour manuellement la condition

Vous devez être affecté à une tâche ou au problème ou disposer des autorisations de gestion pour pouvoir définir la condition sur celle-ci.

La mise à jour de la condition d’une tâche ou d’un problème varie selon que vous y êtes affecté ou non :

* Vous pouvez mettre à jour la condition dans l’onglet Mises à jour ou dans une liste de tâches ou de problèmes si vous y êtes affecté.
* Vous ne pouvez mettre à jour la condition que dans une liste de tâches ou de problèmes si vous n’y êtes pas affecté, mais que vous disposez des autorisations de gestion nécessaires. Dans ce cas, vous ne pouvez pas mettre à jour la condition dans l’onglet Mise à jour de la tâche ou du problème.

Pour définir manuellement la condition d’une tâche ou d’un problème :

1. Accédez à une tâche ou à un problème qui vous a été assigné et pour lequel vous souhaitez définir la condition.

   Ou

   Accédez à la liste des tâches ou des problèmes pour lesquels vous disposez des autorisations de gestion , mais qui ne vous sont pas affectés.

1. Modifiez la condition du problème ou de la tâche comme suit :

   * Si vous êtes affecté à la tâche ou au problème et que vous disposez des autorisations de gestion , sur la **Mises à jour** , cliquez sur **Démarrer une nouvelle mise à jour**, sélectionnez la variable **Condition** qui reflète le mieux le déroulement de la tâche, entrez votre raison de modifier la condition dans la variable **Démarrer une nouvelle mise à jour** zone (facultatif) , puis cliquez sur **Mettre à jour**.

      ![](assets/change-condition-update-comment-350x141.png)

      >[!NOTE]
      >
      >Les conditions peuvent être personnalisées pour votre environnement. Vous pouvez donc trouver plus de trois options pour Condition dans votre environnement. Les noms des Conditions peuvent être différents de ceux répertoriés ci-dessus. Pour plus d’informations sur la personnalisation des conditions dans Workfront, voir [Création ou modification d’une condition personnalisée](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

      Pour plus d’informations sur les fonctionnalités supplémentaires disponibles lors de la mise à jour d’un élément de travail, voir [Mise à jour du travail](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

      <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><p>(NOTE: drafted because I can't do this anymore)</p><p>If you have Manage permissions to the task or issue but are not assigned to it, perhaps as a project manager, add the <strong>Condition</strong> column to any view you use in a task or issue list, then set the <strong>Condition</strong> in inline edit and press Enter.</p><p><img src="assets/change-condition-in-list-view-350x142.png" style="width: 350;height: 142;"></p><p>For information about adding a column to a view, see <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Views overview in Adobe Workfront</a>.</p></li>   
     -->
