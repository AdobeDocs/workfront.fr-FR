---
product-area: projects
navigation-topic: manage-tasks
title: Modifier les tâches dans une liste
description: Vous pouvez modifier les informations des tâches dans une liste de tâches en modifiant les champs affichés dans la liste. Vous devez définir le mode de planification dans une liste de tâches afin d’indiquer comment vous souhaitez que vos modifications soient enregistrées dans Workfront. Vous pouvez enregistrer vos modifications manuellement ou automatiquement.
author: Alina
feature: Work Management
exl-id: 2af81907-3657-459e-b780-65983e224ca8
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '2851'
ht-degree: 63%

---

# Modifier les tâches dans une liste {#edit-tasks-in-a-list}

<!-- Audited: 10/2025 -->

<!--

<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div> -->

Vous pouvez modifier les informations des tâches dans une liste de tâches en modifiant les champs affichés dans la liste. Pour obtenir des informations sur d’autres façons de modifier des tâches, voir la section [Modifier les tâches](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

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
   <td> <p>Standard<p>
   <p>Travail ou supérieur</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès aux tâches et aux projets</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations Contribuer ou supérieures pour la tâche et le projet</p></td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>New: Standard<p>
   <p>Current: Work or higher</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute or higher permissions to the task and the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Remarques concernant la modification des tâches dans une liste {#considerations-about-editing-tasks-in-a-list}

La modification de tâches dans une liste est un moyen rapide d’apporter des modifications à plusieurs tâches simultanément, avec une vue claire de la manière dont vos modifications peuvent affecter la chronologie du projet.

Tenez compte des points suivants lorsque vous modifiez des tâches dans une liste :

* Contrairement à la nécessité de disposer d’autorisations Gérer pour la tâche lors de sa modification dans la zone de modification, vous ne pouvez modifier une tâche dans une liste que si vous disposez des autorisations Contribuer pour la tâche. Vous pouvez ainsi modifier les informations limitées suivantes pour la tâche :

   * Description
   * Statut
   * Pourcentage d’achèvement
   * Informations sur les formulaires personnalisés

     >[!NOTE]
     >
     >Vous ne pouvez modifier un champ personnalisé de tâche dans une liste que si vous disposez des autorisations pour mettre à jour le champ.

   * Consigner les heures
   * Modifier les affectations
   * Afficher les informations financières
   * Ajouter des dépenses, des tâches ou des problèmes

* Vous pouvez modifier une tâche dans les listes suivantes :

   * La section Tâches du projet.
   * La section Sous-tâches du projet.
   * Un rapport de tâche

     >[!NOTE]
     >
     >Par défaut, Workfront enregistre automatiquement vos modifications apportées aux tâches dans la section Sous-tâches ou dans un rapport de tâche.

* Vous pouvez déterminer à quel moment Workfront enregistre les modifications apportées aux tâches dans une liste en définissant le mode de planification avant de commencer à modifier les tâches.

  Vous pouvez choisir entre l’enregistrement dans Workfront des modifications que vous apportez en procédant comme suit :

   * Automatiquement, après chaque modification
   * Manuellement, uniquement après avoir cliqué sur Enregistrer.

  Pour plus d’informations sur la configuration du moment où Workfront enregistre les modifications apportées aux tâches d’une liste, reportez-vous à la section [Modifier le mode de planification avant de modifier les tâches d’une liste](#modify-plan-mode-before-editing-tasks-in-a-list) de cet article.

* Les autres personnes doivent actualiser leurs pages avant de pouvoir afficher les mises à jour apportées à une tâche.

## Modifier le mode Plan avant de modifier des tâches dans une liste

Vous pouvez décider si les modifications apportées aux tâches d&#39;une liste sont enregistrées automatiquement au fur et à mesure ou si vous souhaitez enregistrer manuellement chaque modification. Pour ce faire, vous devez modifier le mode Plan dans une liste de tâches avant de modifier les tâches.

>[!IMPORTANT]
>
>Selon que vous enregistrez les tâches automatiquement ou manuellement, sachez que vous risquez de remplacer les informations d’une autre personne lorsque vous modifiez des tâches dans une liste. Pour plus d’informations, voir [Présentation de l’enregistrement des modifications simultanées dans une liste de tâches](../../../manage-work/tasks/manage-tasks/save-concurrent-changes-in-a-task-list.md).

Lorsque vous enregistrez vos modifications dans une liste pour un projet pour lequel les options Automatique ou Automatique et En cas de modification sont sélectionnées comme Type de mise à jour, Workfront met à jour la chronologie du projet, ainsi que toutes les dépendances internes au projet et interprojets. Les calculs de chronologie peuvent prendre beaucoup de temps si le projet est volumineux ou s’il existe de nombreuses dépendances. Certaines méthodes de modification d’une liste de tâches peuvent être plus rapides que d’autres, selon la méthode que vous choisissez pour enregistrer vos modifications.

Vous pouvez contrôler le moment où Workfront enregistre les modifications que vous apportez aux tâches d’une liste. Les scénarios suivants sont possibles :

* Workfront peut enregistrer automatiquement les modifications après chaque mise à jour.

  Pour plus d’informations, consultez la section [Définir le mode de planification pour enregistrer automatiquement les modifications](#set-the-plan-mode-to-automatically-save-changes) dans cet article.

* Vous pouvez contrôler le moment où vous appliquez plusieurs modifications à la fois en utilisant manuellement le bouton Enregistrer.

  Pour plus d’informations, consultez la section [Définir le mode de planification pour enregistrer manuellement les modifications](#set-the-plan-mode-to-manually-save-changes) dans cet article.

### Définir le mode Plan pour enregistrer automatiquement les modifications

>[!TIP]
>
>L’enregistrement de vos modifications et de toutes les dépendances de projet peut être plus lent si votre projet comporte plus de 2 000 tâches ou s’il comporte de nombreuses dépendances.

Tenez compte de ce qui suit lorsque vous enregistrez automatiquement les modifications de votre liste de tâches :

* Vous pouvez appliquer une vue personnalisée à la liste des tâches et modifier les champs associés aux tâches auxquelles vous avez accès pour la mise à jour.
* Vous ne pouvez pas annuler les modifications enregistrées automatiquement. Il s’agit du paramètre par défaut.
* Lorsque le type de mise à jour du projet est Automatique ou Automatique et en cas de modification, Workfront recalcule automatiquement la chronologie du projet et toutes les dépendances internes au projet et interprojets après chaque modification. Pour plus d’informations sur le type de mise à jour du projet, voir [Sélectionner le type de mise à jour du projet.](../../../manage-work/projects/manage-projects/select-project-update-type.md).

Pour modifier les tâches dans une liste et enregistrer automatiquement les modifications :

{{step1-to-projects}}

1. Sélectionnez un projet sur la page **Projets**.
1. Dans le panneau de gauche, cliquez sur la section **Tâches**.

1. Cliquez sur l’icône **Mode Plan** ![Icône Mode Plan](assets/plan-mode-icon.png) en haut de la liste et assurez-vous que l’option **Enregistrement automatique** est sélectionnée.

   ![Activer le paramètre d’enregistrement automatique](assets/autosave-setting-enabled-quicksilver-task-list-350x308.png)

1. Modifiez les champs pour lesquels vous avez les autorisations de mise à jour manuelle.

1. (Facultatif) Appuyez sur **Échap** pour annuler vos modifications.
1. Appuyez sur la touche **Entrée** (Windows) ou **Retour** (Mac) du clavier pour enregistrer les modifications apportées aux tâches et à la chronologie du projet.
1. (Facultatif) Cliquez avec le bouton droit de la souris sur une tâche à modifier.

   Ou

   Cliquez sur le menu **Plus** ![](assets/more-icon-task-list.png) à droite du nom de la tâche.

1. (Facultatif) Sélectionnez l’une des options suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Ouvrir dans un nouvel onglet</td> 
      <td>Ouvre la tâche dans un nouvel onglet du navigateur. </td> 
     </tr> 
          <tr> 
      <td role="rowheader">Insérer une tâche ci-dessus</td> 
      <td>Insère une tâche au-dessus de la tâche sélectionnée.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Insérer la tâche ci-dessous</td> 
      <td>Insère une tâche sous la tâche sélectionnée.</td> 
     </tr>
     <tr> 
      <td role="rowheader">Modifier</td> 
      <td><p>Ouvre la boîte de dialogue Modifier la tâche, dans laquelle vous pouvez modifier la tâche.</p><p>Pour plus d’informations sur la modification d’une tâche, voir <a href="#edit-tasks-in-a-list" class="MCXref xref">Modifier les tâches dans une liste</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Supprimer</td> 
      <td><p>Supprime la tâche.</p><p>Pour plus d’informations sur la suppression de tâches, voir <a href="../../../manage-work/tasks/manage-tasks/delete-tasks.md" class="MCXref xref">Supprimer des tâches</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Alinéa</td> 
      <td><p>Met en retrait la tâche d’un niveau. </p><p>Cette option s’affiche uniquement sur les tâches autonomes.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Supprimer un alinéa</td> 
      <td><p>Met la tâche en retrait d’un niveau. </p><p>Cette option s’affiche uniquement pour les tâches enfant. </p></td> 
     </tr>  
     <tr> 
      <td role="rowheader">Dupliquer</td> 
      <td><p>Crée une version en double de la tâche au sein du même projet. </p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Copier vers...</td> 
      <td><p>Copie la tâche vers un autre projet.</p><p>Pour plus d’informations sur la copie et la duplication de tâches, voir <a href="../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md" class="MCXref xref">Copier et dupliquer des tâches</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Déplacer vers...</td> 
      <td><p>Déplace la tâche vers un autre projet.</p><p>Pour plus d’informations sur le déplacement de tâches, voir <a href="../../../manage-work/tasks/manage-tasks/move-tasks.md" class="MCXref xref">Déplacer des tâches</a>.</p></td> 
     </tr> 
    </tbody> 
   </table>

### Définir le mode Plan pour enregistrer manuellement les modifications {#edit-tasks-in-a-list-and-manually-save-changes}

Vous pouvez enregistrer manuellement les modifications que vous apportez aux tâches dans une liste. Lorsque vous enregistrez les modifications de cette manière, vous pouvez les inverser avant de les enregistrer.

>[!TIP]
>
>* Vous ne pouvez pas inverser les modifications que vous apportez aux tâches d’une liste lorsque vous les modifiez dans la section Sous-tâches ou dans un rapport de tâches.
>* Le nombre de modifications que vous pouvez inverser est illimité. Vous pouvez tous les inverser un par un jusqu’à ce que vous atteigniez le statut d’origine des tâches.
>

Tenez compte de ce qui suit lorsque vous enregistrez manuellement les modifications dans une liste de tâches :

* Pour enregistrer manuellement les modifications apportées à la liste des tâches, vous avez besoin d’autorisations pour gérer les tâches et le projet.
* Vous ne pouvez pas modifier le projet. L’option permettant de modifier le projet est désactivée.
* Vous ne pouvez pas mettre à jour les informations dans l’en-tête du projet. Vous ne pouvez effectuer que les opérations suivantes lorsque vous enregistrez manuellement les modifications apportées à la liste des tâches :

   * Vous abonner au projet.
   * Ajouter le projet à votre liste de favoris.
   * Ouvrez une tâche en cliquant sur son nom dans la liste.

* Modifiez les tâches en bloc. L’icône Modifier est désactivée lors de la sélection de plusieurs tâches.
* Workfront déclenche des notifications sur les modifications que vous apportez aux tâches uniquement après avoir enregistré vos modifications.

Il existe deux manières d’enregistrer manuellement les modifications apportées à des tâches dans une liste :

* [Enregistrer manuellement les modifications apportées à une liste de tâches en sélectionnant l’option standard Enregistrement manuel](#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-standard-option)
* [Enregistrer manuellement les modifications apportées à une liste de tâches en sélectionnant l’option de planification chronologique Enregistrement manuel](#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-timeline-planning-option)

#### Enregistrer manuellement les modifications apportées à une liste de tâches en sélectionnant l’option standard Enregistrement manuel {#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-standard-option}

>[!TIP]
>
>Si votre projet contient plus de 2 000 tâches ou s’il comporte de nombreuses dépendances, il peut s’écouler un certain temps avant de visualiser les modifications de tâches ainsi que leurs effets sur toutes les dépendances du projet. Dans ce cas, l’enregistrement de vos modifications peut prendre plus de temps que prévu.

Tenez compte des points suivants si vous mettez à jour des tâches dans une liste après avoir sélectionné l’option standard Enregistrement manuel :

* Vous pouvez appliquer une vue personnalisée à la liste des tâches et modifier les champs associés aux tâches pour lesquelles vous disposez de l’autorisation de gérer dans cette vue.
* Lorsque le type de mise à jour du projet est Automatique ou Automatique et En cas de modification, Workfront calcule la chronologie du projet et toutes les dépendances internes au projet et interprojets après avoir cliqué sur Enregistrer. Pour plus d’informations sur le type de mise à jour du projet, voir [Sélectionner le type de mise à jour du projet](../../../manage-work/projects/manage-projects/select-project-update-type.md).

Pour modifier les tâches d’une liste en sélectionnant l’option standard Enregistrement manuel :

{{step1-to-projects}}

1. Sélectionnez un projet sur la page **Projets**.

1. Dans le panneau de gauche, cliquez sur la section **Tâches**.

1. Cliquez sur l’icône **Mode de planification** ![Icône Mode de planification](assets/plan-mode-icon.png) en haut de la liste.

1. Dans la boîte de dialogue **Mode Plan**, sélectionnez **Enregistrement manuel**, puis cliquez sur **Standard**.

   ![Activer le paramètre d’enregistrement manuel](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. Cliquez sur **Appliquer**. Un paramètre de barre d’outils s’affiche avec des options permettant d’annuler, de rétablir et d’enregistrer vos modifications.

   ![Barre d’outils Enregistrement manuel](assets/undo,-redo,-save,-and-cancel-widget-for-task-list-350x65.png)

1. Cliquez à l’intérieur d’un champ pour lequel vous disposez de l’autorisation de mettre à jour manuellement. Le champ devient modifiable et vous pouvez apporter vos modifications.

1. Appuyez sur **Entrée** (Windows) ou **Retour** (Mac) sur votre clavier pour enregistrer temporairement les modifications que vous avez apportées.

1. (Facultatif) Cliquez sur l’icône **Annuler** ![Icône Annuler](assets/undo-icon-on-task-list.png) pour annuler une modification et rétablir un champ à son état d’origine.

1. (Facultatif et conditionnel) Cliquez sur l’icône **Rétablir** ![Icône Rétablir](assets/redo-icon-on-task-list.png) pour restaurer la modification que vous avez annulée.

1. (Facultatif) Cliquez avec le bouton droit de la souris sur une tâche à modifier.

   Ou

   Cliquez sur le menu **Plus** ![](assets/more-icon-task-list.png).

1. (Facultatif) Sélectionnez l’une des options suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Ouvrir dans un nouvel onglet</td> 
      <td>Ouvre la tâche dans un nouvel onglet du navigateur. </td> 
     </tr> 
          <tr> 
      <td role="rowheader">Insérer une tâche ci-dessus</td> 
      <td>Insère une tâche au-dessus de la tâche sélectionnée.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Insérer la tâche ci-dessous</td> 
      <td>Insère une tâche sous la tâche sélectionnée.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Supprimer</td> 
      <td>Pour plus d’informations sur la suppression de tâches, voir <a href="../../../manage-work/tasks/manage-tasks/delete-tasks.md" class="MCXref xref">Supprimer des tâches</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Alinéa</td> 
      <td> <p>Met en retrait la tâche d’un niveau. </p> <p>Cette option s’affiche uniquement sur les tâches autonomes.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Supprimer un alinéa</td> 
      <td> <p>Met la tâche en retrait d’un niveau. </p> <p>Cette option s’affiche uniquement pour les tâches enfant. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dupliquer</td> 
      <td> <p>Crée une version en double de la tâche au sein du même projet. </p> <p>Pour plus d’informations sur la copie et la duplication de tâches, voir <a href="../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md" class="MCXref xref">Copier et dupliquer des tâches</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Workfront met à jour toutes les dépendances inter-projets et dans les projets lorsque vous modifiez la chronologie des tâches.
1. Cliquez sur **Enregistrer** lorsque vous souhaitez conserver vos modifications de tâche de manière permanente et enregistrer la chronologie du projet.

#### Enregistrer manuellement les modifications apportées à une liste de tâches en sélectionnant l’option de planification chronologique Enregistrement manuel {#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-timeline-planning-option}

L’enregistrement de vos modifications et de toutes les dépendances du projet est plus rapide. Cette option n’est pas disponible pour les projets comportant plus de 2 000 tâches.

>[!IMPORTANT]
>
>Nous vous recommandons d’utiliser cette option lors de la modification d’une grande liste de tâches de plus de quelques centaines ayant de nombreuses dépendances. L’utilisation de cette option vous permet d’identifier visuellement vos modifications beaucoup plus rapidement que l’utilisation de l’option d’enregistrement manuel.

Tenez compte des points suivants lorsque vous utilisez l’option d’enregistrement manuel de la planification de la chronologie dans une liste de tâches :

* Vous ne pouvez pas appliquer l’option d’enregistrement manuel de la planification de la chronologie aux projets comportant plus de 2 000 tâches.
* Vous ne pouvez pas appliquer une vue personnalisée, un filtre personnalisé ou un regroupement personnalisé à la liste des tâches. Les menus déroulants Vue, Filtre et Regroupement, ainsi que l’icône de la vue Agile, sont désactivés. La vue appliquée par défaut contient un nombre limité de champs.
* La chronologie du projet et toutes les dépendances internes au projet sont calculées automatiquement après chaque modification lorsque le type de mise à jour du projet est Automatique ou Automatique et En cas de modification.
* Lorsque le type de mise à jour du projet est Automatique ou Automatique et En cas de modification, les dépendances entre projets sont calculées après que vous avez cliqué sur Enregistrer. Pour plus d’informations sur le type de mise à jour du projet, voir [Sélectionner le type de mise à jour du projet](../../../manage-work/projects/manage-projects/select-project-update-type.md).

Pour modifier des tâches dans une liste lors de l’utilisation de l’option d’enregistrement manuel de la planification de la chronologie :


{{step1-to-projects}}

1. Sélectionnez un projet sur la page **Projets**.

1. Dans le panneau de gauche, cliquez sur la section **Tâches**.

1. Cliquez sur l’icône **Mode de planification** ![Icône Mode de planification](assets/plan-mode-icon.png) en haut de la liste.

1. Dans la boîte de dialogue **Mode Plan**, sélectionnez **Enregistrement manuel**, puis cliquez sur **Planification de la chronologie**.

   ![Appliquer le paramètre Planification chronologique](assets/manual-timeline-planning-setting-enabled-quicksilver-task-list-350x490.png)

   >[!TIP]
   >
   >L’option **Planification temporelle** est grisée pour les projets comportant plus de 2 000 tâches.

1. Cliquez sur **Appliquer**.

   Les modifications suivantes sont apportées à la liste :

   * Les menus déroulants Vue, Regroupement et Filtre sont supprimés et la vue est remplacée par les champs suivants :

      * Numéro de tâche
      * Nom de la tâche
      * Type de contrainte
      * Durée
      * Date de début prévue
      * Date d&#39;achèvement prévue
      * Tâches antérieures
      * Affectations
      * Statut
      * Pourcentage d’achèvement

   * L’icône de la vue Agile est supprimée.
   * Un paramètre de barre d’outils s’affiche avec des options permettant d’annuler, de rétablir et d’enregistrer vos modifications.

     ![Barre d’outils Enregistrement manuel](assets/undo,-redo,-save,-and-cancel-widget-for-task-list-350x65.png)

1. Modifiez les champs pour lesquels vous avez les autorisations de mise à jour manuelle.

1. Appuyez sur **Entrée** (Windows) ou **Retour** (Mac) sur votre clavier pour enregistrer temporairement les modifications que vous avez apportées.
1. (Facultatif) Cliquez sur l’icône **Annuler** ![Icône Annuler](assets/undo-icon-on-task-list.png) pour annuler une modification et rétablir un champ à son état d’origine.
1. (Facultatif et conditionnel) Cliquez sur l’icône **Rétablir** ![Icône Rétablir](assets/redo-icon-on-task-list.png) pour rétablir la modification que vous avez annulée.

1. (Facultatif) Cliquez avec le bouton droit de la souris sur une tâche à modifier.

   Ou

   Cliquez sur le menu **Plus** ![](assets/more-icon-task-list.png).

1. Sélectionnez l’une des options suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Ouvrir dans un nouvel onglet</td> 
      <td>Ouvre la tâche dans un nouvel onglet du navigateur. </td> 
     </tr> 
          <tr> 
      <td role="rowheader">Insérer une tâche ci-dessus</td> 
      <td>Insère une tâche au-dessus de la tâche sélectionnée.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Insérer la tâche ci-dessous</td> 
      <td>Insère une tâche sous la tâche sélectionnée.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Supprimer</td> 
      <td>Pour plus d’informations sur la suppression de tâches, voir <a href="../../../manage-work/tasks/manage-tasks/delete-tasks.md" class="MCXref xref">Supprimer des tâches</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Alinéa</td> 
      <td> <p>Met en retrait la tâche d’un niveau. </p> <p>Cette option s’affiche uniquement sur les tâches autonomes.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Supprimer un alinéa</td> 
      <td> <p>Met la tâche en retrait d’un niveau. </p> <p>Cette option s’affiche uniquement pour les tâches enfant. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dupliquer</td> 
      <td> <p>Crée une version en double de la tâche au sein du même projet. </p> <p>Pour plus d’informations sur la copie et la duplication de tâches, voir <a href="../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md" class="MCXref xref">Copier et dupliquer des tâches</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Workfront met à jour toutes les dépendances internes aux projets et inter-projets lorsque vous modifiez la chronologie d’une tâche.
1. Cliquez sur **Enregistrer** lorsque vous souhaitez conserver vos modifications de tâche de manière permanente et enregistrer la chronologie du projet.

## Modifier une tâche dans une liste à l’aide du résumé

{{step1-to-projects}}

1. Sélectionnez un projet sur la page **Projets**.

1. Dans le panneau de gauche, cliquez sur la section **Tâches**. La liste des tâches du projet s’affiche.

1. Sélectionnez la tâche à modifier, puis cliquez sur l’icône **Ouvrir le résumé** ![Ouvrir le résumé](assets/task-summary-icon.png) dans le coin supérieur droit de la liste. Le panneau **Résumé de la tâche** s’ouvre.

1. (Facultatif) Saisissez une mise à jour pour la tâche dans la zone **Mises à jour**.
1. Cliquez sur l’une des icônes ou zones suivantes pour accéder à la tâche et modifier les informations à l’échelle de la tâche :

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Documents</td> 
      <td>Ajoutez des documents à la tâche. </td> 
     </tr> 
          <tr> 
      <td role="rowheader">Formulaires personnalisés</td> 
      <td>Ajouter ou supprimer des formulaires personnalisés ou mettre à jour les informations des formulaires.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Heures</td> 
      <td>Consigner les heures.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Approbations</td> 
      <td>Ajoutez les validations de tâche.</td> 
     </tr> 
     <tr> 
    </tbody> 
   </table>

1. Cliquez sur le **X** dans le coin supérieur droit du panneau pour le fermer.

## Modifier les tâches en bloc

Vous pouvez modifier plusieurs tâches à la fois. Assurez-vous que vous disposez des autorisations de gestion pour les tâches afin de pouvoir les modifier.

{{step1-to-projects}}

1. Sélectionnez un projet sur la page **Projets**.
1. Dans le panneau de gauche, cliquez sur la section **Tâches**.

1. Cliquez sur l’icône **Mode Plan** ![Icône Mode Plan](assets/plan-mode-icon.png) en haut de la liste et assurez-vous que l’option **Enregistrement automatique** est sélectionnée.

   ![Activer le paramètre d’enregistrement automatique](assets/autosave-setting-enabled-quicksilver-task-list-350x308.png)

   >[!IMPORTANT]
   >
   >Vous ne pouvez pas modifier des tâches en bloc lors de l’enregistrement manuel de tâches.

1. Sélectionnez plusieurs tâches dans la liste des tâches.
1. (Facultatif) Cliquez sur le menu **Plus** ![Plus](assets/more-icon.png) en haut de la liste des tâches, puis **Recalculer les expressions** pour mettre à jour toutes les informations des champs calculés personnalisés.
1. Cliquez sur l’icône **Modifier** ![Modifier](assets/qs-edit-icon.png). La boîte de dialogue **Modifier les tâches** s’ouvre dans la nouvelle expérience .

   La modification des informations de toutes les tâches est identique à la modification des informations d’une tâche.

   Pour plus d’informations sur la modification d’une tâche, voir [Modifier les tâches](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

1. (Conditionnel) Dans la nouvelle expérience, procédez comme suit :

   1. Indiquez les informations à modifier pour toutes les tâches sélectionnées dans l’une des zones suivantes :

      * Vue d’ensemble
      * Affectations
      * Formulaires personnalisés
      * Finances
      * Paramètres
      * Paramètres
      * Commentaire

      >[!NOTE]
      >
      >* Les informations que vous modifiez sur toutes les tâches sélectionnées remplacent les informations existantes sur chaque tâche, à l’exception du champ **Affectations**. L’ajout d’une nouvelle personne cessionnaire dans la modification en masse l’ajoute à toutes les tâches sélectionnées. Si d’autres personnes cessionnaires sont affectées aux tâches sélectionnées, elles restent affectées en plus de celle ajoutée par modification en bloc.
      >* Si vous souhaitez modifier la durée de la tâche, les tâches sélectionnées doivent avoir la même contrainte de tâche. Sinon, le champ **Durée** n’est pas renseigné.
      >
      >* Seuls les formulaires personnalisés actifs sont affichés dans la liste. Si les tâches sélectionnées ne comportent aucun formulaire personnalisé commun, aucun formulaire n’est répertorié dans cette section.
      >* Vous ne pouvez modifier que les champs des formulaires joints à toutes les tâches sélectionnées et que vous êtes autorisé à modifier.  Pour plus d’informations sur la modification en bloc de formulaires personnalisés, voir [Gérer les formulaires personnalisés joints à des objets](../../../workfront-basics/work-with-custom-forms/manage-custom-forms-attached-to-objects.md).

   1. Cliquer sur **Enregistrer**.
   1. (Facultatif) Cliquez sur **Revenir à l’ancienne expérience** au bas de la zone **Modifier les tâches**.

1. (Conditionnel) Dans l’ancienne expérience, procédez comme suit :

   1. Indiquez les informations à modifier pour toutes les tâches sélectionnées dans l’une des zones suivantes :

      * Vue d’ensemble
      * Paramètres
      * Affectations
      * Formulaires personnalisés
      * Commentaire

   1. (Facultatif) Dans la section **Custom Forms**, sélectionnez l’option **Recalculer les expressions personnalisées** pour vous assurer que tous les champs calculés personnalisés des formulaires personnalisés joints aux tâches sélectionnées sont à jour.
   1. Cliquez sur Enregistrer les modifications. **** Toutes les modifications que vous avez apportées sont désormais visibles sur toutes les tâches sélectionnées.

