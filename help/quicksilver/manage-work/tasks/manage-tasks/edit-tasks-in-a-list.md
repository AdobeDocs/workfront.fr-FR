---
product-area: projects
navigation-topic: manage-tasks
title: Editer les tâches dans une liste
description: Vous pouvez éditer les informations de la tâche dans une liste de tâches en éditant les champs affichés dans la liste. Pour plus d’informations sur d’autres méthodes de modification des tâches, voir Modifier les tâches.
author: Alina
feature: Work Management
exl-id: 2af81907-3657-459e-b780-65983e224ca8
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '2828'
ht-degree: 2%

---

# Editer les tâches dans une liste {#edit-tasks-in-a-list}

Vous pouvez éditer les informations de la tâche dans une liste de tâches en éditant les champs affichés dans la liste. Pour plus d’informations sur d’autres méthodes de modification des tâches, voir [Modifier les tâches](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

## Exigences d’accès

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
   <td> <p>Travail ou plus élevé</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modifier l’accès aux tâches et aux projets</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Attribuer ou des autorisations supérieures à la tâche et au projet</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Remarques sur la modification des tâches dans une liste {#considerations-about-editing-tasks-in-a-list}

La modification de tâches dans une liste permet d’apporter rapidement des modifications à plusieurs tâches simultanément, avec une vue claire de la manière dont vos modifications peuvent affecter la chronologie du projet.

Tenez compte des points suivants lors de l’édition de tâches dans une liste :

* Contrairement à l’obligation de gérer les autorisations de la tâche lors de son édition dans la zone de modification, vous ne pouvez modifier une tâche dans une liste que si vous disposez des autorisations de contribution pour la tâche. Vous pouvez ainsi modifier les informations limitées suivantes pour la tâche :

   * Description
   * Statut
   * Pourcentage d&#39;achèvement
   * Informations sur les formulaires personnalisés

      >[!NOTE]
      >
      >Vous ne pouvez modifier un champ personnalisé de tâche dans une liste que si vous êtes autorisé à mettre à jour le champ.

   * Heures de journal
   * Modifier les affectations
   * Affichage des informations financières
   * Ajouter des dépenses, des tâches ou des problèmes

* Vous pouvez modifier une tâche dans les listes suivantes :

   * La section Tâches du projet
   * La section Sous-tâches du projet
   * Un rapport de tâche

      >[!NOTE]
      >
      >Par défaut, Workfront enregistre automatiquement vos modifications dans les tâches de la section Sous-tâches ou dans un rapport de tâches.

* Vous pouvez contrôler le moment où Workfront enregistre les modifications que vous apportez aux tâches d’une liste. Vos modifications peuvent être enregistrées automatiquement ou vous pouvez les enregistrer manuellement.

   Pour plus d’informations sur la configuration lorsque Workfront enregistre les modifications que vous apportez aux tâches dans une liste, voir la section [Sélection d’une option d’enregistrement lors de l’édition de tâches dans une liste](#select-a-save-option-when-editing-tasks-in-a-list) dans cet article.

## Sélection d’une option d’enregistrement lors de l’édition de tâches dans une liste {#select-a-save-option-when-editing-tasks-in-a-list}

Vous pouvez décider où les modifications que vous apportez aux tâches d’une liste sont enregistrées automatiquement, au fur et à mesure, ou si vous souhaitez enregistrer manuellement chaque modification.

>[!IMPORTANT]
>
>Selon que vous enregistrez les tâches automatiquement ou manuellement, vous pouvez remplacer les informations d’une autre personne lorsque vous modifiez des tâches dans une liste. Pour plus d’informations sur la façon dont Workfront enregistre les modifications apportées aux tâches que vous effectuez en même temps que d’autres utilisateurs, voir [Aperçu de l’enregistrement des modifications simultanées dans une liste de tâches](../../../manage-work/tasks/manage-tasks/save-concurrent-changes-in-a-task-list.md).

Lorsque vous enregistrez vos modifications dans une liste pour un projet pour lequel les options Automatique ou Automatique et Changement sont sélectionnées comme Type de mise à jour, Workfront met à jour la chronologie du projet, ainsi que toutes les dépendances internes au projet et interprojets. Les calculs de chronologie peuvent prendre beaucoup de temps si le projet est volumineux ou s’il y a beaucoup de dépendances. Certaines méthodes de modification d’une liste de tâches peuvent être plus rapides que d’autres, selon la méthode que vous choisissez pour enregistrer vos modifications.

Vous pouvez contrôler le moment où Workfront enregistre les modifications que vous apportez aux tâches d’une liste. Les scénarios suivants existent : 

* Workfront peut enregistrer automatiquement les modifications après chaque mise à jour.

   Pour plus d’informations, voir la section [Modifier les tâches dans une liste et enregistrer automatiquement les modifications](#edit-tasks-in-a-list-and-automatically-save-changes) dans cet article.

* Vous pouvez contrôler le moment où vous appliquez plusieurs modifications à la fois en utilisant manuellement le bouton Enregistrer .

   Pour plus d’informations, voir la section [Modifier les tâches dans une liste et enregistrer manuellement les modifications](#edit-tasks-in-a-list-and-manually-save-changes) dans cet article.

### Modifier les tâches dans une liste et enregistrer automatiquement les modifications {#edit-tasks-in-a-list-and-automatically-save-changes}

>[!TIP]
>
>L’enregistrement de vos modifications et de toutes les dépendances de projet peut être plus lent si votre projet comporte plus de 2 000 tâches ou s’il comporte de nombreuses dépendances.

Tenez compte de ce qui suit lorsque vous enregistrez automatiquement les modifications de votre liste de tâches :

* Vous pouvez appliquer une vue personnalisée à la liste des tâches et modifier les champs associés aux tâches que vous avez accès à la mise à jour.
* Vous ne pouvez pas annuler les modifications enregistrées automatiquement. Il s’agit du paramètre par défaut.
* Workfront recalcule automatiquement la chronologie du projet et toutes les dépendances internes et interprojets à chaque modification, lorsque le type de mise à jour du projet est Automatique ou Automatique et Changement. Pour plus d’informations sur le type de mise à jour du projet, voir [Sélectionnez le type de mise à jour du projet.](../../../manage-work/projects/manage-projects/select-project-update-type.md).

Pour éditer les tâches dans une liste et enregistrer automatiquement les modifications :

1. Accédez au projet, puis cliquez sur le bouton **Tâches** .
1. Cliquez sur le bouton **Menu du mode Plan** ![](assets/qs-list-mode-or-save-mode-icon-small.png) en haut de la liste et assurez-vous que la variable **Enregistrement automatique** est sélectionnée.

   ![](assets/autosave-setting-enabled-quicksilver-task-list-350x308.png)

1. Modifiez les champs que vous êtes autorisé à mettre à jour manuellement.

   ![](assets/inline-editing-a-task-350x26.png)

1. (Facultatif) Appuyez sur **Échappement** pour annuler vos modifications.
1. Appuyez sur Entrée pour enregistrer les modifications apportées aux tâches et à la chronologie du projet.
1. (Facultatif) Cliquez avec le bouton droit sur une tâche que vous souhaitez modifier.

   Ou

   Cliquez sur le bouton **Plus** menu ![](assets/more-icon-task-list.png) à droite du nom de la tâche.

1. (Facultatif) Sélectionnez l’une des options suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Ouvrir dans un nouvel onglet</strong></td> 
      <td>Ouvre la tâche dans un nouvel onglet du navigateur. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Modifier</strong></td> 
      <td><p>Ouvre la <strong>Modifier la tâche</strong> dans laquelle vous pouvez modifier la tâche.</p><p>Pour plus d’informations sur la modification d’une tâche, voir <a href="#edit-tasks-in-a-list" class="MCXref xref">Editer les tâches dans une liste</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Supprimer</td> 
      <td><p>Supprime la tâche.</p><p>Pour plus d’informations sur la suppression de tâches, voir <a href="../../../manage-work/tasks/manage-tasks/delete-tasks.md" class="MCXref xref">Suppression de tâches</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Alinéa</td> 
      <td><p>Met la tâche en retrait d’un niveau. </p><p>Cette option s’affiche uniquement sur les tâches autonomes.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Supprimer un alinéa</td> 
      <td><p>Retrait la tâche d’un niveau. </p><p>Cette option s’affiche uniquement pour les tâches enfants. </p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Insérer une tâche ci-dessus</td> 
      <td>Insère une tâche au-dessus de la tâche sélectionnée.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Insérer la tâche ci-dessous</td> 
      <td>Insère une tâche sous la tâche sélectionnée</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dupliquer</td> 
      <td><p>Crée une version en double de la tâche au sein du même projet. </p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Copier sur</td> 
      <td><p>Copie la tâche vers un autre projet.</p><p>Pour plus d’informations sur la copie et la duplication de tâches, voir <a href="../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md" class="MCXref xref">Copier et dupliquer des tâches</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Déplacer vers</td> 
      <td><p>Déplace la tâche vers un autre projet.</p><p>Pour plus d’informations sur le déplacement des tâches, voir <a href="../../../manage-work/tasks/manage-tasks/move-tasks.md" class="MCXref xref">Déplacer les tâches</a>.</p></td> 
     </tr> 
    </tbody> 
   </table>

   Les modifications sont enregistrées automatiquement et vous ne pouvez pas les inverser.

### Modifier les tâches dans une liste et enregistrer manuellement les modifications {#edit-tasks-in-a-list-and-manually-save-changes}

Vous pouvez enregistrer manuellement les modifications que vous apportez aux tâches dans une liste. Lorsque vous enregistrez les modifications de cette manière, vous avez la possibilité de les inverser avant de les enregistrer.

>[!TIP]
>
>* Vous ne pouvez pas inverser les modifications que vous apportez aux tâches d’une liste lorsque vous les modifiez dans la section Sous-tâches ou dans un rapport de tâches.
>* Il n’existe aucune limite quant au nombre de modifications que vous pouvez inverser. Vous pouvez inverser toutes les tâches une par une jusqu’à ce que l’état d’origine des tâches soit atteint.
>


Tenez compte de ce qui suit lorsque vous enregistrez manuellement les modifications dans une liste de tâches :

* Pour enregistrer manuellement les modifications apportées à la liste des tâches, vous avez besoin d’autorisations pour gérer les tâches et le projet.
* Vous ne pouvez pas modifier le projet. L’option permettant de modifier le projet est désactivée.
* Vous ne pouvez pas mettre à jour les informations dans l’en-tête du projet. Vous ne pouvez effectuer que les opérations suivantes lorsque vous enregistrez manuellement les modifications dans la liste des tâches :

   * Abonnez-vous au projet.
   * Ajoutez le projet à votre liste de favoris.
   * Ouvrez une tâche en cliquant sur son nom dans la liste.

* Modifiez les tâches en bloc. L’icône Modifier est désactivée lors de la sélection de plusieurs tâches.
* Workfront déclenche des notifications sur les modifications que vous apportez aux tâches uniquement après avoir enregistré vos modifications.

Il existe deux manières d’enregistrer manuellement les modifications apportées aux tâches dans une liste. Ces deux méthodes sont décrites ci-dessous.

* [Enregistrer manuellement les modifications dans une liste de tâches lorsque vous sélectionnez l’option Enregistrer manuellement la norme](#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-standard-option)
* [Enregistrer manuellement les modifications dans une liste de tâches lorsque vous sélectionnez l’option Enregistrer manuellement la planification de la chronologie](#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-timeline-planning-option)

#### Enregistrer manuellement les modifications dans une liste de tâches lorsque vous sélectionnez l’option Enregistrer manuellement la norme {#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-standard-option}

>[!TIP]
>
>Si votre projet comporte plus de 2 000 tâches ou s’il comporte de nombreuses dépendances, il peut s’écouler un certain temps avant que les modifications que vous apportez à vos tâches soient visuellement identifiées et comment ces modifications affectent toutes les dépendances du projet. Dans ce cas, l’enregistrement de vos modifications peut prendre plus de temps si votre projet comporte plus de 2 000 tâches ou s’il comporte de nombreuses dépendances.

Tenez compte des points suivants lors de la mise à jour des tâches dans une liste après avoir sélectionné l’option d’enregistrement manuel de Standard :

* Vous pouvez appliquer une vue personnalisée à la liste des tâches et modifier les champs associés aux tâches que vous êtes autorisé à gérer dans cette vue.
* Workfront calcule la chronologie du projet et toutes les dépendances internes et interprojets après avoir cliqué sur Enregistrer, lorsque le type de mise à jour du projet est Automatique ou Automatique et Changement. Pour plus d’informations sur le type de mise à jour du projet, voir [Sélectionnez le type de mise à jour du projet.](../../../manage-work/projects/manage-projects/select-project-update-type.md).

Pour modifier les tâches d’une liste lors de la sélection de l’option d’enregistrement standard manuel :

1. Accédez à un projet, puis cliquez sur le bouton **Tâches** section .
1. Cliquez sur le bouton **Mode Plan** menu ![](assets/qs-list-mode-or-save-mode-icon-small.png) en haut de la liste et sélectionnez **Enregistrement manuel**, puis cliquez sur **Standard** > **Appliquer**.

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

   Un paramètre de barre d’outils s’affiche avec des options permettant d’annuler, de rétablir et d’enregistrer vos modifications.

   ![](assets/undo,-redo,-save,-and-cancel-widget-for-task-list-350x65.png)

1. Cliquez à l’intérieur des champs que vous êtes autorisé à mettre à jour manuellement. Le champ devient modifiable et vous pouvez apporter vos modifications.

   ![](assets/inline-editing-a-task-350x26.png)

1. Appuyez sur Entrée pour enregistrer temporairement les modifications que vous avez apportées.
1. (Facultatif) Cliquez sur le **Icône Annuler** ![](assets/undo-icon-on-task-list.png) pour annuler une modification et rétablir l’état d’origine d’un champ.
1. (Facultatif et conditionnel) Cliquez sur le bouton **Icône Rétablir** ![](assets/redo-icon-on-task-list.png) pour restaurer la modification annulée.

1. (Facultatif) Cliquez avec le bouton droit de la souris sur une tâche à modifier.

   Ou

   Cliquez sur le bouton **Plus** menu ![](assets/more-icon-task-list.png).

1. (Facultatif) Sélectionnez l’une des options suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Ouvrir dans un nouvel onglet</strong> </td> 
      <td>Ouvre la tâche dans un nouvel onglet du navigateur. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Supprimer</td> 
      <td>Pour plus d’informations sur la suppression de tâches, voir <a href="../../../manage-work/tasks/manage-tasks/delete-tasks.md" class="MCXref xref">Suppression de tâches</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Alinéa</td> 
      <td> <p>Met la tâche en retrait d’un niveau. </p> <p>Cette option s’affiche uniquement sur les tâches autonomes.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Supprimer un alinéa</td> 
      <td> <p>Retrait la tâche d’un niveau. </p> <p>Cette option s’affiche uniquement pour les tâches enfants. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Insérer une tâche ci-dessus</td> 
      <td>Insère une tâche au-dessus de la tâche sélectionnée.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Insérer la tâche ci-dessous</td> 
      <td>Insère une tâche sous la tâche sélectionnée</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dupliquer</td> 
      <td> <p>Crée une version en double de la tâche au sein du même projet. </p> <p>Pour plus d’informations sur la copie et la duplication de tâches, voir <a href="../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md" class="MCXref xref">Copier et dupliquer des tâches</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Workfront met à jour toutes les dépendances internes aux projets et interprojets lorsque vous modifiez la chronologie des tâches.
1. Cliquez sur **Enregistrer** lorsque vous souhaitez conserver vos modifications de tâche de manière permanente et enregistrer la chronologie du projet.

#### Enregistrer manuellement les modifications dans une liste de tâches lorsque vous sélectionnez l’option Enregistrer manuellement la planification de la chronologie {#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-timeline-planning-option}

L’enregistrement de vos modifications et de toutes les dépendances du projet est plus rapide. Cette option n’est pas disponible pour les projets comportant plus de 2 000 tâches.

>[!IMPORTANT]
>
>Nous vous recommandons d’utiliser cette option lors de l’édition d’une grande liste de tâches de plus de quelques centaines de personnes ayant de nombreuses dépendances. L’utilisation de cette option vous permet d’identifier visuellement vos modifications beaucoup plus rapidement que l’utilisation de l’option d’enregistrement manuel.

Tenez compte des points suivants lorsque vous utilisez l’option d’enregistrement manuel de la planification de la chronologie dans une liste de tâches :

* Vous ne pouvez pas appliquer l’option Enregistrement manuel de la planification de la chronologie aux projets comportant plus de 2 000 tâches.
* Vous ne pouvez pas appliquer une vue, un filtre ou un regroupement personnalisé à la liste des tâches. Les menus déroulants Affichage, Filtre et Regroupement , ainsi que l’icône Vue agile, sont désactivés. La vue appliquée par défaut contient un nombre limité de champs.
* La chronologie du projet et toutes les dépendances internes au projet sont calculées automatiquement après chaque modification lorsque le type de mise à jour du projet est Automatique ou Automatique et Changement.
* Les dépendances entre projets sont calculées après avoir cliqué sur Enregistrer, lorsque le type de mise à jour du projet est Automatique ou Automatique et Changement. Pour plus d’informations sur le type de mise à jour du projet, voir [Sélectionnez le type de mise à jour du projet.](../../../manage-work/projects/manage-projects/select-project-update-type.md).

Pour modifier des tâches dans une liste lors de l’utilisation de l’option d’enregistrement manuel de la planification de la chronologie :

1. Accédez à un projet, puis cliquez sur le bouton **Tâches** .
1. Cliquez sur le bouton **Mode Plan** menu ![](assets/qs-list-mode-or-save-mode-icon-small.png) en haut de la liste et sélectionnez **Enregistrement manuel**, puis cliquez sur **Planification de la chronologie**> **Appliquer**.

   Cette option est grisée pour les projets comportant plus de 2 000 tâches.

   ![](assets/manual-timeline-planning-setting-enabled-quicksilver-task-list-350x490.png)

   >[!TIP]
   >
   >Lorsque vous quittez cette page, Workfront réactive l’option d’enregistrement automatique.

   Notez les modifications suivantes dans la liste :

   * Les menus déroulants Affichage, Regroupement et Filtre sont supprimés et la vue est remplacée par les champs suivants :

      * Numéro de tâche
      * Nom de la tâche
      * Type de contrainte
      * Durée
      * Date de début prévue
      * Date d&#39;achèvement prévue
      * Tâches antérieures
      * Affectations
      * Statut
      * Pourcentage d&#39;achèvement
   * L’icône Agile view est supprimée.
   * Un paramètre de barre d’outils s’affiche avec des options permettant d’annuler, de rétablir et d’enregistrer vos modifications.

      ![](assets/undo,-redo,-save,-and-cancel-widget-for-task-list-350x65.png)


1. Modifiez les champs que vous êtes autorisé à mettre à jour manuellement.

   ![](assets/inline-editing-a-task-350x26.png)

1. Appuyez sur Entrée pour enregistrer temporairement les modifications que vous avez apportées.
1. (Facultatif) Cliquez sur le **Icône Annuler** ![](assets/undo-icon-on-task-list.png) pour annuler une modification et rétablir l’état d’origine d’un champ.
1. (Facultatif et conditionnel) Cliquez sur le bouton **Icône Rétablir** ![](assets/redo-icon-on-task-list.png) pour rétablir la modification que vous avez annulée.

1. (Facultatif) Cliquez avec le bouton droit sur une tâche à modifier.

   Ou

   Cliquez sur le bouton **Plus** menu ![](assets/more-icon-task-list.png).

1. Sélectionnez l’une des options suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Ouvrir dans un nouvel onglet</strong> </td> 
      <td>Ouvre la tâche dans un nouvel onglet du navigateur. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Supprimer</td> 
      <td>Pour plus d’informations sur la suppression de tâches, voir <a href="../../../manage-work/tasks/manage-tasks/delete-tasks.md" class="MCXref xref">Suppression de tâches</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Alinéa</td> 
      <td> <p>Met la tâche en retrait d’un niveau. </p> <p>Cette option s’affiche uniquement sur les tâches autonomes.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Supprimer un alinéa</td> 
      <td> <p>Retrait la tâche d’un niveau. </p> <p>Cette option s’affiche uniquement pour les tâches enfants. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Insérer une tâche ci-dessus</td> 
      <td>Insère une tâche au-dessus de la tâche sélectionnée.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Insérer la tâche ci-dessous</td> 
      <td>Insère une tâche sous la tâche sélectionnée</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dupliquer</td> 
      <td> <p>Crée une version en double de la tâche au sein du même projet. </p> <p>Pour plus d’informations sur la copie et la duplication de tâches, voir <a href="../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md" class="MCXref xref">Copier et dupliquer des tâches</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Workfront met à jour toutes les dépendances internes aux projets et interprojets lorsque vous modifiez la chronologie d’une tâche.
1. Cliquez sur **Enregistrer** lorsque vous souhaitez conserver vos modifications de tâche de manière permanente et enregistrer la chronologie du projet.

## Modifier une tâche dans une liste à l’aide du Résumé

1. Accédez au projet contenant les tâches à modifier.
1. Cliquez sur **Tâches** dans le panneau de gauche.

   La liste des tâches du projet s’affiche.

1. Cliquez sur le menu Plus ![](assets/more-icon-task-list.png) après le nom de la tâche, puis cliquez sur **Résumé ouvert**. Sélectionnez la tâche à modifier, puis cliquez sur le bouton **Icône Ouvrir le résumé** ![](assets/qs-open-summary-icon-in-new-toolbar-small.png) dans le coin supérieur droit de la liste.

   Le **Résumé** s’ouvre.

   ![](assets/qs-task-right-panel-in-a-task-list-350x328.png)

1. (Facultatif) Cliquez sur le **Icône X** dans le coin supérieur droit du résumé pour fermer le panneau et modifier les tâches en ligne.

   Suivez les étapes de modification d’une tâche dans une liste pour la modifier en ligne.

   Pour plus d’informations sur la modification de la tâche dans une liste, voir [Remarques sur la modification des tâches dans une liste](#considerations-about-editing-tasks-in-a-list) dans cet article.

1. (Facultatif) Saisissez une mise à jour pour la tâche dans la variable **Mises à jour** zone.
1. Cliquez sur l’une des icônes ou zones suivantes pour accéder à la tâche et modifier les informations au niveau de la tâche :

   | Documents | Cliquez sur **Cliquez ici pour ajouter** pour ajouter des documents à la tâche. |
   |---|---|
   | Détails | Cliquez sur pour mettre à jour les informations sur la tâche. |
   | Formulaires personnalisés | Cliquez pour ajouter ou supprimer le Forms personnalisé ou mettre à jour les informations des formulaires. |
   | Heures | Cliquez sur pour consigner les heures. |
   | Approbations | Cliquez sur pour ajouter les validations de tâche. |

   {style=&quot;table-layout:auto&quot;}

1. Cliquez sur le bouton Retour de votre navigateur pour revenir à la liste des tâches lorsque vous avez terminé la mise à jour de la tâche.

## Modifier les tâches en bloc

Vous pouvez modifier plusieurs tâches à la fois. Assurez-vous que vous disposez des autorisations de gestion pour les tâches afin de pouvoir les modifier.

1. Accédez à un projet contenant les tâches que vous souhaitez modifier en bloc.
1. Cliquez sur **Tâches** dans le panneau de gauche.
1. Assurez-vous que la variable **Enregistrement automatique** est sélectionnée.

   >[!IMPORTANT]
   >
   >Vous ne pouvez pas modifier les tâches en bloc lors de l’enregistrement manuel des tâches.

   Pour plus d’informations sur les façons d’enregistrer les modifications apportées aux tâches dans une liste, voir la section [Remarques sur la modification des tâches dans une liste](#considerations-about-editing-tasks-in-a-list) dans cet article.

1. Sélectionnez plusieurs tâches dans la liste des tâches.
1. Cliquez sur le bouton **Icône Modifier** ![](assets/qs-edit-icon.png).

   Le **Modifier les tâches** s’ouvre.

1. Indiquez les informations à modifier pour toutes les tâches sélectionnées.

   La modification des informations sur toutes les tâches est identique à la modification des informations sur une tâche. Si vous souhaitez modifier la durée de la tâche, les tâches sélectionnées doivent avoir la même contrainte de tâche ; dans le cas contraire, la variable **Durée** ne s’affiche pas.

   Pour plus d’informations sur la modification d’une tâche, voir [Modifier les tâches](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

   >[!NOTE]
   >
   >Les informations que vous modifiez sur toutes les tâches sélectionnées remplacent les informations existantes sur les tâches individuelles, à l’exception des **Affectations** champ . L’ajout d’une nouvelle personne désignée dans la modification en masse l’ajoute à toutes les tâches sélectionnées. Si d’autres personnes désignées sont affectées aux tâches sélectionnées, elles restent affectées en plus de celle ajoutée par modification en masse.

1. Cliquez sur **Forms personnalisée** pour modifier les formulaires personnalisés associés à toutes les tâches sélectionnées. Seuls les principaux formulaires personnalisés s’affichent dans la liste.

   Si les tâches sélectionnées ne comportent aucun formulaire personnalisé commun, aucun formulaire n’est répertorié dans cette section.

   Vous ne pouvez modifier que les champs des formulaires associés à toutes les tâches sélectionnées et que vous êtes autorisé à modifier.

1. (Facultatif) Dans la section Forms personnalisée , sélectionnez la variable **Recalculer des expressions personnalisées** pour vous assurer que tous les champs personnalisés calculés qui se trouvent sur les formulaires personnalisés joints aux tâches sélectionnées sont à jour.
1. Cliquez sur **Enregistrer les modifications**.

   Toutes les modifications que vous avez apportées sont désormais visibles sur toutes les tâches sélectionnées.

Pour plus d’informations sur la modification en masse de formulaires personnalisés, reportez-vous à la section &quot;Modification de plusieurs Forms personnalisés lors de la modification en masse d’objets&quot; dans [Gestion des formulaires personnalisés associés à des objets](../../../workfront-basics/work-with-custom-forms/manage-custom-forms-attached-to-objects.md).
