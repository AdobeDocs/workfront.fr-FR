---
product-area: templates
keywords: task,defaults,automate,creation
navigation-topic: templates-navigation-topic
title: Modifier la tâche de modèle
description: Après avoir créé un modèle, vous pouvez modifier les informations relatives aux tâches du modèle. Les informations que vous mettez à jour sur une tâche de modèle sont associées à des tâches de projet une fois que vous avez utilisé le modèle pour créer un projet ou que vous avez joint le modèle à un projet.
author: Alina
feature: Work Management
exl-id: 2df8522e-7eee-4440-be0f-f7483c5acdb0
source-git-commit: c9fa6d97607990710e6c2a74f3b373d06201d721
workflow-type: tm+mt
source-wordcount: '7460'
ht-degree: 70%

---

# Modifier les tâches de modèles

<!--Audited: 11/2025-->

<!--take out production and preview references and new/ old experiences at release-->

<div class="preview">

Les informations surlignées sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de manière générale. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Les mêmes fonctionnalités seront également disponibles dans l’environnement de production pour tous les clients et clientes à partir d’une semaine à compter de la version préliminaire.

Pour plus d’informations, voir [Modernisation des interfaces](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).

</div>

Après avoir créé un modèle, vous pouvez modifier les informations des tâches de modèle. Les informations que vous mettez à jour sur une tâche de modèle sont associées à des tâches de projet une fois que vous avez utilisé le modèle pour créer un projet ou que vous avez joint le modèle à un projet.

Pour plus d’informations sur la création d’un modèle, voir [Créer un modèle de projet](../../../manage-work/projects/create-and-manage-templates/create-template.md).

Vous pouvez modifier une tâche de modèle à la fois ou modifier des tâches de modèle en bloc.

>[!NOTE]
>
>Vous ne pouvez pas modifier en masse des tâches de modèle qui appartiennent à différents modèles. Vous ne pouvez modifier en masse que les tâches de modèle appartenant au même modèle.

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
   <p>Plan </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuration du niveau d’accès</td> 
   <td> <p>Modifier l’accès aux modèles</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet </td> 
   <td> <p>Autorisations de gestion pour un modèle. </p> <p>Vous ne pouvez pas partager une tâche de modèle. </p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, consultez la section [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
   <td> <p>Standard </p>
   <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level</td> 
   <td> <p>Edit access to Templates</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions </td> 
   <td> <p>Manage permissions for a template. </p> <p>You cannot share a template task. </p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Conditions préalables

Avant de commencer, vous devez

* Créez un modèle.

  Pour plus d’informations sur la création d’un modèle, voir [Créer un modèle de projet](../../../manage-work/projects/create-and-manage-templates/create-template.md).

## Modifier les tâches de modèles

La modification des tâches de modèle diffère selon l’environnement que vous choisissez pour modifier les tâches.

### Modification des tâches de modèle dans l’environnement de production

>[!NOTE]
>
><span class="preview">Certains clients peuvent modifier les tâches de modèle dans leurs environnements de production de la même manière qu’ils les modifient dans leur environnement de prévisualisation.</span>
>
><span class="preview">Pour plus d’informations sur la modification des tâches dans l’environnement de prévisualisation, consultez la section [Modifier les tâches de modèle dans l’environnement de prévisualisation](#edit-template-tasks-in-the-preview-environment) dans cet article. </span>


Vous pouvez modifier une tâche de modèle à l&#39;aide des zones Modifier la tâche de modèle ou Détails de la tâche de modèle.

{{step1-to-templates}}

1. Cliquez sur le nom d’un modèle pour l’ouvrir.
1. Cliquez sur **Tâches de modèle** dans le panneau de gauche.
1. Cliquez sur le nom d’une tâche de modèle dans la liste pour ouvrir la tâche de modèle.
1. Pour modifier des informations limitées sur la tâche de modèle, procédez comme suit :
   1. (Facultatif) Cliquez sur **Mises à jour** dans le panneau de gauche pour ajouter des mises à jour à la tâche de modèle. Les mises à jour des tâches de modèle ne sont pas transférées aux tâches de projet lorsque le modèle est utilisé pour créer un projet.
   1. (Facultatif) Cliquez sur **Documents** dans le panneau de gauche pour ajouter des documents à la tâche de modèle. Les documents seront transférés aux tâches du projet lorsque vous utiliserez le modèle pour créer le projet.
   1. (Le cas échéant) Pour modifier des informations limitées sur une tâche de modèle, cliquez sur **Détails sur la tâche de modèle** dans le panneau de gauche, puis accédez aux zones de la section Détails pour modifier les informations de chaque zone.
   1. (Facultatif) Effectuez l’une des opérations suivantes :
      * Cliquez sur l’icône **Tout réduire** ![Tout réduire](assets/collapse-all-icon.png) pour réduire toutes les zones.
      * Cliquez sur l’icône **Modifier** ![Modifier](assets/edit-icon.png), puis sélectionnez l’une des zones ci-dessous, ou cliquez sur **Modifier tout** pour modifier les informations de toutes les zones :

         * Vue d’ensemble
         * Forms personnalisé
Les noms des formulaires de douane s’affichent uniquement si des formulaires personnalisés sont joints à la tâche de modèle.
         * Finances

        >[!TIP]
        >
        >Pour plus d’informations sur tous les champs qui s’affichent dans la zone Détails , continuez à modifier tous les champs à l’aide de la zone Modifier la tâche de modèle , comme décrit ci-dessous.

   1. (Facultatif) Cliquez sur la section **Sous-tâches** dans le panneau de gauche pour ajouter des enfants à la tâche de modèle. L’ajout de sous-tâches pour les tâches de modèle est similaire à l’ajout de sous-tâches de projet. Pour plus d’informations, reportez-vous à la section « Création de sous-tâches à partir de la section Sous-tâches de la tâche » de l’article [Création de sous-tâches](/help/quicksilver/manage-work/tasks/create-tasks/create-subtasks.md).
   1. (Facultatif) Cliquez sur **Dépenses** dans le panneau de gauche et ajoutez des dépenses aux tâches de modèle. Les dépenses liées aux tâches de modèle sont transférées vers les tâches de projets futurs lorsque le modèle est utilisé pour créer un projet.
   1. (Facultatif) Cliquez sur **Approbations** dans le panneau de gauche pour créer des approbations ou joindre des approbations globales ou au niveau du groupe aux tâches de modèle. Les approbations sont transférées vers des tâches de projets futurs.
   1. (Facultatif) Cliquez sur la section **Prédécesseurs** dans le panneau de gauche pour ajouter des prédécesseurs pour les tâches de modèle. L’ajout de prédécesseurs de tâche de modèle est similaire à l’ajout de prédécesseurs de tâche de projet. Pour plus d’informations, voir [Créer une relation de prédécesseur à l’aide de la zone Prédécesseurs](/help/quicksilver/manage-work/tasks/use-prdcssrs/create-predecessors-in-predecessors-area.md).

1. (Facultatif) Pour modifier plusieurs tâches de modèle en masse, sélectionnez plusieurs tâches de modèle, puis cliquez sur **Modifier** en haut de la liste des modèles.
1. (Conditionnel) Pour modifier toutes les informations relatives à la tâche du modèle ou à plusieurs tâches en même temps, cliquez sur les tâches pour les sélectionner dans une liste, puis cliquez sur l&#39;icône **Modifier** ![Modifier](assets/edit-icon.png) en haut de la liste.

   La zone **Modifier la tâche de modèle** s’affiche dans la nouvelle expérience.

   ![Nouvelle expérience pour Modifier la tâche de modèle](assets/edit-template-task-box-unshimmed.png)

   >[!TIP]
   >
   >Vous pouvez également sélectionner une tâche de modèle dans une liste, puis cliquer sur **Modifier** à droite du nom de la tâche de modèle dans l’en-tête, pour ouvrir la zone **Modifier la tâche de modèle**.

   Continuez à modifier la tâche de modèle comme décrit dans la section [&#x200B; Modifier une tâche de modèle à l’aide de la nouvelle expérience &#x200B;](#edit-a-template-task-using-the-new-experience) de cet article.

1. (Facultatif) Cliquez sur **Revenir à l’ancienne expérience** au bas de la zone **Modifier la tâche de modèle** pour ouvrir la zone **Modifier la tâche de modèle** dans l’ancienne expérience.

   ![Modifier la tâche de modèle](assets/edit-template-tasks-box-classic-350x356.png)

1. Pensez à spécifier des informations dans l’une des sections suivantes :

   * [Vue d’ensemble](#overview)
   * [Finances](#finance)
   * [Paramètres](#settings)
   * [Affectations](#assignments)
   * [Formulaires personnalisés](#custom-forms)
   * [Commentaire](#comment)

1. Continuez à modifier la tâche de modèle comme décrit dans la section [&#x200B; Modifier une tâche de modèle à l’aide de l’ancienne expérience &#x200B;](#edit-a-template-task-using-the-old-experience) de cet article.

#### Modifier une tâche de modèle à l’aide de l’ancienne expérience

##### Vue d’ensemble {#overview}

1. Commencez à modifier une tâche de modèle comme décrit ci-dessus.
1. Cliquez sur **Vue d’ensemble**.

   ![edit_task_overview.png](assets/edit-task-overview-350x438.png)

1. Mettez à jour l’un des éléments suivants :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Nom</strong> </td> 
      <td>Attribuez un nom à la tâche de modèle. Ce champ ne s’affiche pas lors de la modification de tâches de modèle en masse.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Description</strong> </td> 
      <td>Ajoutez des informations supplémentaires sur la tâche de modèle.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>URL</strong> </td> 
      <td>Spécifiez un lien web qui se rapporte aux informations sur la tâche de modèle.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Priorité</strong> </td> 
      <td> <p>Il s’agit d’un indicateur visuel qui vous permet de hiérarchiser vos tâches de modèle. </p> <p>Sélectionnez l’une des options suivantes :</p> 
       <ul> 
        <li> <p><strong>Aucune</strong> </p> </li> 
        <li> <p><strong>Faible</strong> </p> </li> 
        <li> <p> <b>Normale</b></p> </li> 
        <li> <p><b>Élevée</b> </p> </li> 
        <li> <p><b>Urgente</b> </p> </li> 
       </ul> <p>Selon les préférences du projet sélectionnées par votre administrateur ou administratrice Workfront, les noms des priorités peuvent être différents pour vous. Pour plus d’informations sur la modification des priorités, voir <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md" class="MCXref xref">Créer et personnaliser des priorités</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Type de durée</strong> </td> 
      <td> <p>La future tâche créée à partir de ce modèle aura ce type de durée. <br>Le type de durée identifie la relation entre les éléments suivants :</p> <p>- nombre de ressources affectées à une tâche</p> <p>- effort total requis pour terminer la tâche</p> <p>- durée totale de la tâche. </p> <p>Les types de durée vous permettent de définir des affectations de ressources cohérentes en fonction des besoins de la tâche. Pour plus d’informations sur le type de durée d’une tâche, voir <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Vue d’ensemble de la durée de la tâche et du type de durée</a>.</p> <p>Sélectionnez l’une des options suivantes :</p> 
       <ul> 
        <li> <p style="font-weight: bold;"><span style="font-weight: normal;">Calcul d’affectation</span> </p> </li> 
        <li> <p style="font-weight: bold;"><span style="font-weight: normal;">Calcul de travail</span> </p> </li> 
        <li> <p style="font-weight: bold;"><span style="font-weight: normal;">Piloté par l’effort</span> </p> </li> 
        <li> <p style="font-weight: bold;"><span style="font-weight: normal;">Simple</span> <br> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Durée</strong> </td> 
      <td> <p>Indiquez la durée des tâches futures, en minutes, heures, jours, semaines ou mois. La durée de la tâche créée à partir de ce modèle sera spécifiée ici.</p> <p>Par défaut, Workfront mesure la durée en jours. Il s’agit de la durée pendant laquelle vous laissez la tâche incomplète avant qu’elle soit terminée. Vous ne pouvez pas spécifier la durée d’une tâche lorsque le <strong>Type de durée</strong> de la tâche est <strong>Simple</strong>, ou lorsque la <strong>Contrainte de tâche</strong> est <strong>Dates fixes</strong>.</p> <p><b>IMPORTANT</b></p> <p>La durée correspond généralement au temps écoulé entre les dates de début et d’achèvement prévues d’une tâche de modèle. Elle affecte donc la chronologie du modèle. Cela détermine la chronologie du futur projet créé à partir du modèle. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Nombre d’heures prévues</strong> </td> 
      <td> <p>Indiquez le nombre d’heures prévues pour la tâche à venir sur le projet créé avec ce modèle. Il s’agit de la durée réelle nécessaire aux personnes cessionnaires de la tâche pour l’exécuter. Vous pouvez uniquement spécifier le nombre d’heures prévues d’une tâche lorsque le <strong>type de durée</strong> est défini sur <strong>Calcul d’affectation</strong>. </p> </td> 
     </tr>

   <tr> 
      <td role="rowheader"><strong>Contrainte de tâche</strong> </td> 
      <td> <p>La tâche sur le projet créé à partir de ce modèle aura cette contrainte. Les contraintes de tâche déterminent à quel moment une tâche doit être terminée. </p> <p>Sélectionnez l’une des options suivantes :</p> 
       <ul> 
        <li><strong>Dates fixes</strong>. Spécifiez une <strong>Date de début prévue</strong> et une <strong>Date d’achèvement prévue</strong>.</li> 
        <li><strong>Il faut commencer le</strong>. Spécifiez une <strong>Date de début prévue</strong>.</li> 
        <li><strong>Il faut finir le</strong>. Spécifiez une <strong>Date d’achèvement prévue</strong>.</li> 
        <li><strong>Aussi tôt que possible</strong> </li> 
        <li><strong>Aussi tard que possible</strong> </li> 
        <li style="font-weight: bold;"><strong>Première heure disponible</strong> </li> 
        <li style="font-weight: bold;"><strong>Dernière heure disponible</strong> </li> 
        <li>Commencer au plus tard. Spécifiez une <strong>Date de début prévue</strong>.</li> 
        <li><strong>Commencer Au Plus Tôt</strong>. Spécifiez une <strong>Date de début prévue</strong>.</li> 
        <li><strong>Finir Au Plus Tard</strong>. Spécifiez une <strong>Date d’achèvement prévue</strong>.</li> 
        <li><strong>Finir Au Plus Tôt</strong>. Spécifiez une <strong>Date d’achèvement prévue</strong>.</li> 
       </ul> <p>Pour plus d’informations sur la contrainte de tâche, voir <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Vue d’ensemble de la contrainte de tâche</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span style="font-weight: bold;">Jour de début</span><span style="font-weight: normal;"> (facultatif et le cas échéant)</span> </td> 
      <td> <p> Vous ne pouvez spécifier le Jour de début d'une tâche de modèle que lorsque la Contrainte de tâche est l'une des suivantes :</p> 
       <ul> 
        <li>Il Faut Commencer Le</li> 
        <li>Commencer Au Plus Tôt</li> 
        <li>Commencer Au Plus Tard</li> 
        <li>Dates fixes</li> 
       </ul> <p>Cela correspondra à la date dans la chronologie du futur projet à laquelle la tâche démarrera. Pour toutes les autres contraintes, Workfront calcule le Jour de début en fonction de la dépendance d’antériorité entre les tâches. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Jour d’achèvement</strong><span style="font-weight: normal;"> (facultatif et le cas échéant)</span> </td> 
      <td> <p> Vous ne pouvez spécifier le jour d’achèvement d’une tâche de modèle que lorsque la contrainte de tâche est l’une des suivantes :</p> 
       <ul style="list-style-type: circle;"> 
        <li>Il Faut Finir Le</li> 
        <li>Finir Au Plus Tôt</li> 
        <li>Finir Au Plus Tard</li> 
        <li>Dates fixes</li> 
       </ul> <p>Cela correspondra à la date dans la chronologie du futur projet à laquelle la tâche sera terminée. Pour toutes les autres contraintes, Workfront calcule le jour d’achèvement en fonction de la durée et de la dépendance des tâches antérieures. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Facultatif) Continuez à modifier les sections suivantes, en fonction des informations que vous souhaitez modifier.

   Ou

   Cliquez sur **Enregistrer les modifications**.

##### Finances {#finance}

1. Commencez à modifier une tâche de modèle comme décrit ci-dessus.
1. Cliquez sur **Finances**.

   ![edit_task_finance.png](assets/edit-task-finance-350x216.png)

1. Mettez à jour l’un des éléments suivants :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Type de coût</strong> </td> 
      <td> <p>Indiquez le type de coût de la tâche à venir. Cette option détermine la manière dont le coût de la tâche est calculé, sur la base du nombre d’heures consacrées à la tâche. </p> <p>Sélectionnez l’une des options suivantes :</p> 
       <ul> 
        <li> <p style="font-weight: normal;"><span>Aucun coût</span> </p> </li> 
        <li> <p style="font-weight: normal;"><span>Fixe par heure</span> </p> </li> 
        <li> <p style="font-weight: normal;"><span>Utilisateur ou utilisatrice, par heure</span> </p> </li> 
        <li> <p style="font-weight: normal;"><span>Rôle par heure</span> </p> </li> 
       </ul> <p>Pour plus d’informations sur le suivi des coûts, consultez la section <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Suivi des coûts</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Type de revenu</strong> </td> 
      <td> <p>Indiquez le type de revenu pour la tâche à venir. Cela détermine comment le revenu de la tâche est calculé en fonction du nombre d’heures passées sur les tâches.</p> <p style="font-weight: normal;">Sélectionnez l’une des options suivantes : </p> 
       <ul> 
        <li> <p style="font-weight: normal;">Non facturable</p> </li> 
        <li> <p style="font-weight: normal;">Utilisateur, par heure</p> </li> 
        <li> <p style="font-weight: normal;">Rôle par heure</p> </li> 
        <li> <p style="font-weight: normal;">Fixe par heure</p> </li> 
        <li> <p style="font-weight: normal;">Utilisateur par heure avec limite</p> </li> 
        <li> <p style="font-weight: normal;">Rôle par heure avec limite</p> </li> 
        <li> <p style="font-weight: normal;">Utilisateur, par heure plus fixe</p> </li> 
        <li> <p style="font-weight: normal;">Rôle par heure plus fixe</p> </li> 
        <li> <p style="font-weight: normal;">Revenus fixes</p> </li> 
       </ul> <p>Pour plus d’informations sur le suivi des revenus, consultez la section <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Vue d’ensemble de la facturation et des revenus</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Facultatif) Continuez à modifier les sections suivantes, en fonction des informations que vous souhaitez modifier.

   Ou

   Cliquez sur **Enregistrer les modifications**.

##### Paramètres {#settings}

1. Commencez à modifier une tâche de modèle comme décrit ci-dessus.
1. Cliquez sur **Paramètres**.

   ![Modifier les paramètres de la tâche de modèle](assets/edit-template-tasks-settings-classic-350x231.png)

1. Mettez à jour l’un des éléments suivants :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
   <tr> 
      <td role="rowheader"><p><b>Jalon</b></p></strong> </td> 
      <td> <p>Sélectionnez un jalon à associer à la tâche de modèle sélectionnée.</p>

   <p><b>IMPORTANT</b></p>
   <p>Vous devez associer un chemin jalonné à un modèle pour que ce champ s’affiche. Pour plus d’informations, consultez la section <a href="../create-and-manage-templates/edit-templates.md">Modifier des modèles de projet</a>.</p> 
   </td> 
     </tr>
     <tr> 
      <td role="rowheader"><strong>Mode de suivi</strong> </td> 
      <td> <p>Indiquez le mode de suivi du statut de progression de la tâche à venir. </p> <p>Sélectionnez l’une des options suivantes :</p> 
       <ul> 
        <li> <p><strong>Utilisateur ou utilisatrice doit mettre à jour</strong>. </p> </li> 
        <li> <p><strong>Supposer à l’heure</strong> </p> </li> 
        <li> <p><strong>Ignorer avertissements de retard</strong> </p> </li> 
        <li> <p><strong>Conclusion automatique</strong> </p> </li> 
        <li> <p><strong>Tâche antérieure</strong> </p> </li> 
       </ul> <p>Pour plus d’informations sur le mode de suivi des tâches, consultez la section <a href="../../../manage-work/tasks/task-information/task-tracking-mode.md" class="MCXref xref">Vue d’ensemble du mode de suivi des tâches</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Processus d’approbation</strong> </td> 
      <td> <p>Sélectionnez le processus d’approbation que vous souhaitez associer à la tâche de modèle. Votre administrateur ou votre administratrice Workfront doit définir des processus d’approbation des tâches au niveau du système avant de pouvoir les associer à des tâches de modèle. <span>Un utilisateur ou une utilisatrice disposant d’un accès administratif aux processus d’approbation peut également créer des processus d’approbation spécifiques à un groupe.</span>Pour plus d’informations sur la création de processus d’approbation, voir <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Créer un processus d’approbation pour les éléments de travail</a>.</p> <p>Tenez compte des éléments suivants lorsque vous ajoutez des processus d’approbation : </p> 
       <ul> 
       <li>Seuls les processus d’approbation actifs sont affichés dans la liste. </li> 
       <li> <p>Les processus d’approbation à l’échelle du système et spécifiques au groupe s’affichent dans la liste. Les processus d’approbation associés à un groupe autre que celui du modèle ne s’affichent pas dans la liste.</p> <p>Important : si le groupe associé au modèle change, le processus d’approbation spécifique au groupe devient un processus d’approbation à usage unique. Pour plus d’informations sur la façon dont les modifications apportées au groupe du projet ou au processus d’approbation affectent les paramètres d’approbation, voir la section <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">Effets des modifications du processus d’approbation et de groupe sur les processus d’approbation affectés</a>. </p> </li> 
       <li> <p>Si vous avez ajouté un processus d’approbation à usage unique, il s’affiche sous la forme « &lt;Personnalisé&gt; » dans ce champ. Pour plus d’informations, voir <a href="../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md" class="MCXref xref">Associer un processus d’approbation nouveau ou existant au travail</a>. </p> <!--<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this will be valid only for Classic when they edit the Edit Template box in NWE)</p>--> </li> 
       <li> <p>Lors de la modification en masse de tâches de modèle, les scénarios suivants existent :</p> 
       <ul> 
       <li> <p>Lorsque vous sélectionnez des tâches de modèle dans le même groupe de modèles, les processus d’approbation au niveau du système et du groupe s’affichent dans ce champ.</p> </li> 
       <li> <p>Lorsque vous sélectionnez des tâches de modèle dans différents groupes de modèles, seuls les processus d’approbation au niveau du système s’affichent dans ce champ.</p> </li> 
       <li> <p>Lorsque l’une des tâches de modèle est associée à un processus d’approbation à usage unique, il est remplacé par le <span>processus d’approbation au niveau du système ou au niveau du groupe</span> que vous sélectionnez. </p> </li> 
       </ul> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Notifications de rappel</strong> </td> 
      <td> <p>Sélectionnez les notifications de rappel que vous souhaitez joindre à la tâche de modèle. Elles seront jointes aux futures tâches du projet créé à partir de ce modèle. L’administrateur ou administratrice système doit configurer les notifications de rappel avant que vous ne puissiez les sélectionner sur une tâche. Pour plus d’informations sur la configuration des notifications de rappel, voir <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">Configurer des notifications de rappel</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Facultatif) Continuez à modifier les sections suivantes, en fonction des informations que vous souhaitez modifier.

   Ou

   Cliquez sur **Enregistrer les modifications**.

##### Affectations {#assignments}

1. Commencez à modifier une tâche de modèle comme décrit ci-dessus.
1. Cliquez sur **Affectations**.

   ![assignments_edit_tasks.png](assets/assignments-edit-tasks-350x87.png)

1. Cliquez sur **Ajouter une personne cessionnaire** pour ajouter une nouvelle personne cessionnaire à la tâche de modèle. Vous pouvez affecter des personnes, des rôles ou des équipes à une tâche. Vous pouvez avoir plusieurs personnes cessionnaires sur une tâche. Les tâches futures auront les mêmes ressources qui leur seront affectées lorsqu’elles seront créées à partir de cette tâche de modèle.
1. (Facultatif) Si vous avez plusieurs personnes cessionnaires, sélectionnez le bouton radio **Propriétaire** pour indiquer quel personne ou rôle est considéré comme propriétaire de la tâche ou cessionnaire principal. Workfront marque la première personne ou fonction que vous affectez à une tâche de modèle comme propriétaire ou cessionnaire principal.
1. (Conditionnel et facultatif) Si votre **Type de durée** est **Calcul de travail** ou **Piloté par l&#39;effort**, spécifiez le **Pourcentage d&#39;affectation** (pourcentage d&#39;affectation) pour chaque personne désignée. Il s’agit de la durée dans le planning de la personne cessionnaire qui peut être consacrée à cette tâche. La modification du pourcentage d’affectation d’une personne cessionnaire modifie le nombre d’heures prévues d’une tâche.
1. (Conditionnel et facultatif) Si votre **Type de durée** est **Simple**, spécifiez les **Heures** de chaque personne désignée

   Ou

   Indiquez le nombre total d’**heures prévues** pour la tâche de modèle. Cela répartit le nombre total d’heures de manière égale entre toutes les personnes cessionnaires.

1. (Conditionnel et facultatif) Si votre **Type de durée** est Simple, spécifiez le **Durée** de la tâche de modèle en jours. Cela deviendra la durée de la tâche créée à partir de ce modèle.
1. (Facultatif) Sélectionnez un rôle dans le menu déroulant des **rôles de la personne cessionnaire**. Il s’agit du rôle que la personne cessionnaire peut remplir pour cette tâche future. Seules les fonctions associées à chaque personne cessionnaire dans son profil s’affichent dans le menu déroulant.
1. (Facultatif) Continuez à modifier les sections suivantes, en fonction des informations que vous souhaitez modifier.

   Ou

   Cliquez sur **Enregistrer les modifications**.

##### Formulaires personnalisés {#custom-forms}

Vous pouvez définir des formulaires personnalisés à joindre automatiquement par défaut aux tâches lorsque les tâches sont ajoutées à un projet. Pour plus d’informations sur la configuration du projet afin d’inclure les formulaires personnalisés de tâche par défaut, consultez la section « Tâches » de l’article [Modifier des projets](../../../manage-work/projects/manage-projects/edit-projects.md).

Vous pouvez également ajouter des formulaires personnalisés aux tâches futures d’un projet lorsque celui-ci sera créé à partir d’un modèle, en ajoutant les formulaires personnalisés aux tâches de modèle.

1. Commencez à modifier une tâche de modèle comme décrit ci-dessus.
1. Cliquez sur **Formulaires personnalisés**.

   ![custom_forms_edit_task.png](assets/custom-forms-edit-task-350x136.png)

1. Sélectionnez le ou les formulaires personnalisés à associer à la tâche de modèle.

   Vous devez créer les formulaires personnalisés avant qu’ils ne puissent être sélectionnés dans ce champ.
Seuls les formulaires personnalisés actifs s’affichent dans la liste.
Pour plus d’informations sur la création de formulaires personnalisés, voir [Créer un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
Vous pouvez ajouter jusqu’à dix formulaires personnalisés à une tâche de modèle.
Les formulaires sont automatiquement ajoutés aux tâches créées à partir du modèle.
1. (Le cas échéant et facultatif) Si vous avez joint un formulaire personnalisé à la tâche de modèle, modifiez les champs du formulaire concernés. Vous devez spécifier tous les champs requis avant de pouvoir enregistrer la tâche de modèle.

   >[!NOTE]
   >
   >Selon la manière dont votre équipe d’administration Workfront définit les autorisations pour les sections de votre formulaire personnalisé, tout le monde ne peut pas afficher ou modifier les mêmes champs sur un formulaire personnalisé donné. Les autorisations de modifier les champs d’une section d’un formulaire personnalisé dépendent des autorisations que vous avez sur la tâche de modèle ou la tâche future.\
   >Pour plus d’informations sur la configuration des autorisations pour des sections d’un formulaire personnalisé, consultez la section [Partager un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).\
   >Pour plus d’informations sur la configuration des autorisations pour une tâche, voir [Partager une tâche](../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md).\
   >Pour plus d’informations sur la configuration des autorisations pour un modèle, voir [Partager un modèle](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

1. (Facultatif) Continuez à modifier la section suivante, en fonction des informations que vous souhaitez modifier.

   Ou

   Cliquez sur **Enregistrer les modifications**.

##### Commentaire {#comment}

1. Commencez à modifier une tâche de modèle comme décrit ci-dessus.
1. Cliquez sur **Commentaire**.

   ![comment_edit_task.png](assets/comment-edit-task-350x138.png)

1. Dans le champ disponible, entrez le commentaire que vous souhaitez afficher dans le flux de mises à jour de la tâche de modèle. Ce commentaire est visible par toutes les personnes ayant un accès en affichage au modèle et à la tâche de modèle, ainsi qu’ayant un accès à l’affichage des notes.
1. Cliquez sur **Enregistrer les modifications**.

   Lorsque vous ou une autre personne créez un projet à partir de ce modèle, tous les paramètres que vous avez appliqués aux tâches de modèle deviennent les paramètres des tâches du projet.

#### Modifier une tâche de modèle à l’aide de la nouvelle expérience

Après avoir ouvert la zone **Modifier la tâche de modèle** dans la nouvelle expérience , pensez à spécifier des informations dans l’une des sections suivantes :

* [Nom de la tâche de modèle](#template-task-name)
* [Vue d’ensemble](#overview-1)
* [Affectations](#assignments-1)
* [Finances](#finance-1)
* [Formulaires personnalisés](#custom-forms-1)
* [Paramètres](#settings-1)
* [Commentaire](#comment-1)

##### Nom de tâche de modèle

>[!TIP]
>
>La section Nom de la tâche de modèle n’est pas disponible lors de la modification de tâches de modèle en bloc.


1. Commencez à modifier une tâche de modèle comme décrit ci-dessus.
1. Dans la zone Modifier la tâche de modèle, cliquez sur **Nom de la tâche de modèle** et ajoutez un nom pour la tâche de modèle.

   Cette vue n’est pas disponible lors de la modification de tâches de modèle en bloc.

1. (Facultatif) Continuez à modifier les sections suivantes, en fonction des informations que vous souhaitez modifier.

   Ou

   Cliquer sur **Enregistrer**.

##### Vue d’ensemble {#overview-1}

1. Commencez à modifier une tâche de modèle comme décrit ci-dessus.
1. Dans la zone **Modifier la tâche de modèle**, cliquez sur **Aperçu** dans le panneau de gauche.

   ![Section de présentation de la modification de la tâche de modèle](assets/template-task-edit-overview.png)

1. Mettez à jour l’un des éléments suivants :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Description</strong> </td> 
      <td>Ajoutez des informations supplémentaires sur la tâche de modèle.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Priorité</strong> </td> 
      <td> <p>Il s’agit d’un indicateur visuel qui vous permet de hiérarchiser vos tâches de modèle. </p> <p>Sélectionnez l’une des options suivantes :</p> 
       <ul> 
        <li> <p><strong>Aucune</strong> </p> </li> 
        <li> <p><strong>Faible</strong> </p> </li> 
        <li> <p> <b>Normale</b></p> </li> 
        <li> <p><b>Élevée</b> </p> </li> 
        <li> <p><b>Urgente</b> </p> </li> 
       </ul> <p>Selon les préférences du projet sélectionnées par votre administrateur ou administratrice Workfront, les noms des priorités peuvent être différents pour vous. Pour plus d’informations sur la modification des priorités, voir la section <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md" class="MCXref xref">Créer et personnaliser des priorités</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Contrainte de tâche</strong> </td> 
      <td> <p>La tâche sur le projet créé à partir de ce modèle aura cette contrainte. Les contraintes de tâche déterminent à quel moment une tâche doit être terminée. </p> <p>Sélectionnez l’une des options suivantes :</p> 
       <ul> 
        <li><strong>Dates fixes</strong>. Spécifiez une <strong>Date de début prévue</strong> et une <strong>Date d’achèvement prévue</strong>.</li> 
        <li><strong>Il faut commencer le</strong>. Spécifiez une <strong>Date de début prévue</strong>.</li> 
        <li><strong>Il faut finir le</strong>. Spécifiez une <strong>Date d’achèvement prévue</strong>.</li> 
        <li><strong>Aussi tôt que possible</strong> </li> 
        <li><strong>Aussi tard que possible</strong> </li> 
        <li style="font-weight: bold;"><strong>Première heure disponible</strong> </li> 
        <li style="font-weight: bold;"><strong>Dernière heure disponible</strong> </li> 
        <li>Commencer au plus tard. Spécifiez une <strong>Date de début prévue</strong>.</li> 
        <li><strong>Commencer Au Plus Tôt</strong>. Spécifiez une <strong>Date de début prévue</strong>.</li> 
        <li><strong>Finir Au Plus Tard</strong>. Spécifiez une <strong>Date d’achèvement prévue</strong>.</li> 
        <li><strong>Finir Au Plus Tôt</strong>. Spécifiez une <strong>Date d’achèvement prévue</strong>.</li> 
       </ul> <p>Pour plus d’informations sur la contrainte de tâche, voir <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Vue d’ensemble de la contrainte de tâche</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span style="font-weight: bold;">Jour de début</span><span style="font-weight: normal;"> (facultatif et le cas échéant)</span> </td> 
      <td> <p> Vous ne pouvez spécifier le Jour de début d'une tâche de modèle que lorsque la Contrainte de tâche est l'une des suivantes :</p> 
       <ul> 
        <li>Il Faut Commencer Le</li> 
        <li>Commencer Au Plus Tôt</li> 
        <li>Commencer Au Plus Tard</li> 
        <li>Dates fixes</li> 
       </ul> <p>Cela correspondra à la date dans la chronologie du futur projet à laquelle la tâche démarrera. Pour toutes les autres contraintes, Workfront calcule le Jour de début en fonction de la dépendance d’antériorité entre les tâches. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Jour d’achèvement</strong><span style="font-weight: normal;"> (facultatif et le cas échéant)</span> </td> 
      <td> <p> Vous ne pouvez spécifier le jour d’achèvement d’une tâche de modèle que lorsque la contrainte de tâche est l’une des suivantes :</p> 
       <ul style="list-style-type: circle;"> 
        <li>Il Faut Finir Le</li> 
        <li>Finir Au Plus Tôt</li> 
        <li>Finir Au Plus Tard</li> 
        <li>Dates fixes</li> 
       </ul> <p>Cela correspondra à la date dans la chronologie du futur projet à laquelle la tâche sera terminée. Pour toutes les autres contraintes, Workfront calcule le jour d’achèvement en fonction de la durée et de la dépendance des tâches antérieures. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>URL</strong> </td> 
      <td>Spécifiez un lien web qui se rapporte aux informations sur la tâche de modèle.</td> 
     </tr>

   <tr> 
      <td role="rowheader"><strong>Effort de travail</strong> </td> 
      <td>Choisissez l’une des options suivantes :
      <ul><li>Petite</li>
      <li>Moyen</li>
      <li>Grande</li></ul>

   <p><b>IMPORTANT</b></p>
      <p>Le champ Effort de travail s’affiche lors de la modification d’une tâche de modèle uniquement lorsque vous sélectionnez le paramètre <b> Utiliser l’effort de travail pour calculer automatiquement le nombre d’heures prévues de la tâche </b> lors de la modification du modèle.</p>

   </td> 
     </tr> 
     </tbody> 
   </table>

1. (Facultatif) Continuez à modifier les sections suivantes, en fonction des informations que vous souhaitez modifier.

   Ou

   Cliquer sur **Enregistrer**.

##### Affectations {#assignments-1}

1. Commencez à modifier une tâche de modèle comme décrit ci-dessus.
1. Dans la zone **Modifier la tâche de modèle**, cliquez sur **Affectations** dans le panneau de gauche.

   ![La tâche de modèle modifie les affectations](assets/template-task-edit-assignments.png)

1. Dans le champ **Rechercher des personnes, des rôles ou des équipes**, commencez à saisir le nom d’une personne désignée, puis sélectionnez-la lorsqu’elle s’affiche dans la liste

   Ou

   Cliquez sur **Me l’affecter** pour vous affecter la tâche de modèle.
1. Pensez à mettre à jour les informations suivantes :

   <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody>

   <tr> 
         <td role="rowheader"><strong>Type de durée</strong> </td> 
         <td> <p>La future tâche créée à partir de ce modèle aura ce type de durée. <br> Le type de durée identifie la relation entre les éléments suivants :</p> 
         <ul>
         <li><p>Nombre de ressources affectées à une tâche</p> </li>
         <li><p>Effort total requis pour terminer la tâche</p></li> 
         <li><p>Durée totale de la tâche </p></li></ul> <p>Les types de durée vous permettent de définir des affectations de ressources cohérentes en fonction des besoins de la tâche. Pour plus d’informations sur le type de durée d’une tâche, voir <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Vue d’ensemble de la durée de la tâche et du type de durée</a>.</p> <p>Sélectionnez l’une des options suivantes :</p> 
         <ul> 
         <li> <p style="font-weight: bold;"><span style="font-weight: normal;">Calcul d’affectation</span> </p> </li> 
         <li> <p style="font-weight: bold;"><span style="font-weight: normal;">Calcul de travail</span> </p> </li> 
         <li> <p style="font-weight: bold;"><span style="font-weight: normal;">Piloté par l’effort</span> </p> </li> 
         <li> <p style="font-weight: bold;"><span style="font-weight: normal;">Simple</span> <br> </p> </li> 
         </ul> </td> 
      </tr> 
      <tr> 
         <td role="rowheader"><strong>Durée</strong> </td> 
         <td> <p>Indiquez la durée des tâches futures, en minutes, heures, jours, semaines ou mois. La durée de la tâche créée à partir de ce modèle sera spécifiée ici.</p> <p>Par défaut, Workfront mesure la durée en jours. Il s’agit de la durée pendant laquelle vous laissez la tâche incomplète avant qu’elle soit terminée. Vous ne pouvez pas spécifier la durée d’une tâche lorsque le <strong>Type de durée</strong> de la tâche est <strong>Simple</strong>, ou lorsque la <strong>Contrainte de tâche</strong> est <strong>Dates fixes</strong>.</p> <p><b>IMPORTANT</b></p> <p>La durée correspond généralement au temps écoulé entre les dates de début et d’achèvement prévues d’une tâche de modèle. Elle affecte donc la chronologie du modèle. Cela détermine la chronologie du futur projet créé à partir du modèle. </p> </td> 
      </tr> 
      <tr> 
         <td role="rowheader"><strong>Nombre d’heures prévues</strong> </td> 
         <td> <p>Indiquez le nombre d’heures prévues pour la tâche à venir sur le projet créé avec ce modèle. Il s’agit de la durée réelle nécessaire aux personnes cessionnaires de la tâche pour l’exécuter. Vous pouvez uniquement spécifier le nombre d’heures prévues d’une tâche lorsque le <strong>type de durée</strong> est défini sur <strong>Calcul d’affectation</strong>. </p> </td> 
      </tr> 
   </tbody> 
      </table>

1. (Facultatif) Continuez à modifier les sections suivantes, en fonction des informations que vous souhaitez modifier.

   Ou

   Cliquer sur **Enregistrer**.

##### Finances {#finance-1}

1. Commencez à modifier une tâche de modèle comme décrit ci-dessus.
1. Dans la zone **Modifier la tâche de modèle**, cliquez sur **Finances** dans le panneau de gauche.

   ![Section Modifier les finances de la tâche de modèle](assets/template-task-edit-finance.png)

1. Mettez à jour l’un des éléments suivants :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Type de coût</strong> </td> 
      <td> <p>Indiquez le type de coût de la tâche à venir. Cette option détermine la manière dont le coût de la tâche est calculé, sur la base du nombre d’heures consacrées à la tâche. </p> <p>Sélectionnez l’une des options suivantes :</p> 
       <ul> 
        <li> <p style="font-weight: normal;"><span>Aucun coût</span> </p> </li> 
        <li> <p style="font-weight: normal;"><span>Fixe par heure</span> </p> </li> 
        <li> <p style="font-weight: normal;"><span>Utilisateur ou utilisatrice, par heure</span> </p> </li> 
        <li> <p style="font-weight: normal;"><span>Rôle par heure</span> </p> </li> 
       </ul> <p>Pour plus d’informations sur le suivi des coûts, consultez la section <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Suivi des coûts</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Type de revenu</strong> </td> 
      <td> <p>Indiquez le type de revenu pour la tâche à venir. Cela détermine comment le revenu de la tâche est calculé en fonction du nombre d’heures passées sur les tâches.</p> <p style="font-weight: normal;">Sélectionnez l’une des options suivantes : </p> 
       <ul> 
        <li> <p style="font-weight: normal;">Non facturable</p> </li> 
        <li> <p style="font-weight: normal;">Utilisateur, par heure</p> </li> 
        <li> <p style="font-weight: normal;">Rôle par heure</p> </li> 
        <li> <p style="font-weight: normal;">Fixe par heure</p> </li> 
        <li> <p style="font-weight: normal;">Utilisateur par heure avec limite</p> </li> 
        <li> <p style="font-weight: normal;">Rôle par heure avec limite</p> </li> 
        <li> <p style="font-weight: normal;">Utilisateur, par heure plus fixe</p> </li> 
        <li> <p style="font-weight: normal;">Rôle par heure plus fixe</p> </li> 
        <li> <p style="font-weight: normal;">Revenus fixes</p> </li> 
       </ul> <p>Pour plus d’informations sur le suivi des revenus, consultez la section <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Vue d’ensemble de la facturation et des revenus</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Facultatif) Continuez à modifier les sections suivantes, en fonction des informations que vous souhaitez modifier.

   Ou

   Cliquer sur **Enregistrer**.

##### Formulaires personnalisés {#custom-forms-1}

Vous pouvez définir des formulaires personnalisés à joindre automatiquement par défaut aux tâches lorsque les tâches sont ajoutées à un projet. Pour plus d’informations sur la configuration du projet afin d’inclure les formulaires personnalisés de tâche par défaut, consultez la section « Tâches » de l’article [Modifier des projets](../../../manage-work/projects/manage-projects/edit-projects.md).

Vous pouvez également ajouter des formulaires personnalisés aux tâches futures d’un projet lorsque celui-ci sera créé à partir d’un modèle, en ajoutant les formulaires personnalisés aux tâches de modèle.

1. Commencez à modifier une tâche de modèle comme décrit ci-dessus.
1. Dans la zone **Modifier la tâche de modèle**, cliquez sur **Forms personnalisé** dans le panneau de gauche.

   ![Section Modifier les formulaires personnalisés de la tâche de modèle](assets/template-task-edit-custom-forms.png)

1. Sélectionnez le ou les formulaires personnalisés à associer à la tâche de modèle.

   Vous devez créer les formulaires personnalisés avant qu’ils ne puissent être sélectionnés dans ce champ.
Seuls les formulaires personnalisés actifs sont affichés dans la liste.

   Pour plus d’informations sur la création de formulaires personnalisés, voir [Créer un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

   Vous pouvez ajouter jusqu’à dix formulaires personnalisés à une tâche de modèle.
Les formulaires sont automatiquement ajoutés aux tâches créées à partir du modèle.
1. (Le cas échéant et facultatif) Si vous avez joint un formulaire personnalisé à la tâche de modèle, modifiez les champs du formulaire concernés. Vous devez spécifier tous les champs requis avant de pouvoir enregistrer la tâche de modèle.

   >[!NOTE]
   >
   >Selon la manière dont votre équipe d’administration Workfront définit les autorisations pour les sections de votre formulaire personnalisé, tout le monde ne peut pas afficher ou modifier les mêmes champs sur un formulaire personnalisé donné. Les autorisations de modifier les champs d’une section d’un formulaire personnalisé dépendent des autorisations que vous avez sur la tâche de modèle ou la tâche future.\
   >Pour plus d’informations sur la configuration des autorisations pour des sections d’un formulaire personnalisé, consultez la section [Partager un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).\
   >Pour plus d’informations sur la configuration des autorisations pour une tâche, voir [Partager une tâche](../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md).\
   >Pour plus d’informations sur la configuration des autorisations pour un modèle, voir [Partager un modèle](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

1. (Facultatif) Continuez à modifier la section suivante, en fonction des informations que vous souhaitez modifier.

   Ou

   Cliquer sur **Enregistrer**.

##### Paramètres {#settings-1}

1. Commencez à modifier une tâche de modèle comme décrit ci-dessus.
1. Dans la boîte de dialogue **Modifier la tâche de modèle**, cliquez sur **Paramètres** dans le panneau de gauche.

   ![Section des paramètres de modification de la tâche de modèle](assets/template-task-edit-settings.png)

1. Mettez à jour l’un des éléments suivants :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
   <tr> 
      <td role="rowheader"><p><b>Jalon</b></p></strong> </td> 
      <td> <p>Sélectionnez un jalon à associer à la tâche de modèle sélectionnée.</p>

   <p><b>IMPORTANT</b></p>
   <p>Vous devez associer un chemin jalonné à un modèle pour que ce champ s’affiche. Pour plus d’informations, consultez la section <a href="../create-and-manage-templates/edit-templates.md">Modifier des modèles de projet</a>.</p> 
   </td> 
     </tr>
     <tr> 
      <td role="rowheader"><strong>Mode de suivi</strong> </td> 
      <td> <p>Indiquez le mode de suivi du statut de progression de la tâche à venir. </p> <p>Sélectionnez l’une des options suivantes :</p> 
       <ul> 
        <li> <p><strong>Utilisateur ou utilisatrice doit mettre à jour</strong>. </p> </li> 
        <li> <p><strong>Supposer à l’heure</strong> </p> </li> 
        <li> <p><strong>Ignorer avertissements de retard</strong> </p> </li> 
        <li> <p><strong>Conclusion automatique</strong> </p> </li> 
        <li> <p><strong>Tâche antérieure</strong> </p> </li> 
       </ul> <p>Pour plus d’informations sur le mode de suivi des tâches, consultez la section <a href="../../../manage-work/tasks/task-information/task-tracking-mode.md" class="MCXref xref">Vue d’ensemble du mode de suivi des tâches</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Notifications de rappel</strong> </td> 
      <td> <p>Sélectionnez les notifications de rappel que vous souhaitez joindre à la tâche de modèle. Elles seront jointes aux futures tâches du projet créé à partir de ce modèle. L’administrateur ou administratrice système doit configurer les notifications de rappel avant que vous ne puissiez les sélectionner sur une tâche. Pour plus d’informations sur la configuration des notifications de rappel, voir <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">Configurer des notifications de rappel</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Processus d’approbation</strong> </td> 
      <td> <p>Sélectionnez le processus d’approbation que vous souhaitez associer à la tâche de modèle. Votre administrateur ou votre administratrice Workfront doit définir des processus d’approbation des tâches au niveau du système avant de pouvoir les associer à des tâches de modèle. <span>Un utilisateur ou une utilisatrice disposant d’un accès administratif aux processus d’approbation peut également créer des processus d’approbation spécifiques à un groupe.</span>Pour plus d’informations sur la création de processus d’approbation, voir <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Créer un processus d’approbation pour les éléments de travail</a>.</p> <p>Tenez compte des éléments suivants lorsque vous ajoutez des processus d’approbation : </p> 
       <ul> 
       <li>Seuls les processus d’approbation actifs sont affichés dans la liste. </li> 
       <li> <p>Les processus d’approbation à l’échelle du système et spécifiques au groupe s’affichent dans la liste. Les processus d’approbation associés à un groupe autre que celui du modèle ne s’affichent pas dans la liste.</p> <p>Important : si le groupe associé au modèle change, le processus d’approbation spécifique au groupe devient un processus d’approbation à usage unique. Pour plus d’informations sur la façon dont les modifications apportées au groupe du projet ou au processus d’approbation affectent les paramètres d’approbation, voir la section <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">Effets des modifications du processus d’approbation et de groupe sur les processus d’approbation affectés</a>. </p> </li> 
       <li> <p>Si vous avez ajouté un processus d’approbation à usage unique, il s’affiche sous la forme « &lt;Personnalisé&gt; » dans ce champ. Pour plus d’informations, voir <a href="../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md" class="MCXref xref">Associer un processus d’approbation nouveau ou existant au travail</a>. </p>  </li> 
       <li> <p>Lors de la modification en masse de tâches de modèle, les scénarios suivants existent :</p> 
       <ul> 
       <li> <p>Lorsque vous sélectionnez des tâches de modèle dans le même groupe de modèles, les processus d’approbation au niveau du système et du groupe s’affichent dans ce champ.</p> </li> 
       <li> <p>Lorsque vous sélectionnez des tâches de modèle dans différents groupes de modèles, seuls les processus d’approbation au niveau du système s’affichent dans ce champ.</p> </li> 
       <li> <p>Lorsque l’une des tâches de modèle est associée à un processus d’approbation à usage unique, il est remplacé par le <span>processus d’approbation au niveau du système ou au niveau du groupe</span> que vous sélectionnez. </p> </li> 
       </ul> </li> 
       </ul> </td> 
     </tr>

   </tbody> 
   </table>

1. (Facultatif) Continuez à modifier les sections suivantes, en fonction des informations que vous souhaitez modifier.

   Ou

   Cliquer sur **Enregistrer**.

##### Commentaire {#comment-1}

1. Commencez à modifier une tâche de modèle comme décrit ci-dessus.
1. Dans la zone **Modifier la tâche de modèle**, cliquez sur **Commentaire** dans le panneau de gauche.

   ![Section Modifier le commentaire de la tâche de modèle](assets/template-task-edit-comment.png)

1. Dans la zone **Ajouter une mise à jour à la tâche de modèle**, indiquez un commentaire que vous souhaitez afficher dans le flux de mises à jour de la tâche de modèle dans le champ disponible. Ce commentaire est visible par toutes les personnes ayant un accès en affichage au modèle et à la tâche de modèle, ainsi qu’ayant un accès à l’affichage des notes.
1. Cliquer sur **Enregistrer**.

   Lorsque vous ou une autre personne créez un projet à partir de ce modèle, tous les paramètres que vous avez appliqués aux tâches de modèle deviennent les paramètres des tâches du projet.


<div class="preview">

### Modifier les tâches de modèles dans l’environnement de Prévisualisation

Vous pouvez modifier une tâche de modèle à l&#39;aide des zones Modifier la tâche de modèle ou Détails de la tâche de modèle.

{{step1-to-templates}}

1. Cliquez sur le nom d’un modèle pour l’ouvrir.
1. Cliquez sur **Tâches de modèle** dans le panneau de gauche.
1. Cliquez sur le nom d’une tâche de modèle dans la liste pour ouvrir la tâche de modèle.
1. Pour modifier des informations limitées sur la tâche de modèle, procédez comme suit :
   1. (Facultatif) Cliquez sur **Mises à jour** dans le panneau de gauche pour ajouter des mises à jour à la tâche de modèle. Les mises à jour des tâches de modèle ne sont pas transférées aux tâches de projet lorsque le modèle est utilisé pour créer un projet.
   1. (Facultatif) Cliquez sur **Documents** dans le panneau de gauche pour ajouter des documents à la tâche de modèle. Les documents seront transférés aux tâches du projet lorsque vous utiliserez le modèle pour créer le projet.
   1. (Le cas échéant) Pour modifier des informations limitées sur une tâche de modèle, cliquez sur **Détails sur la tâche de modèle** dans le panneau de gauche, puis accédez aux zones de la section Détails pour modifier les informations de chaque zone.
   1. (Facultatif) Effectuez l’une des opérations suivantes :
      * Cliquez sur l’icône **Tout réduire** ![Tout réduire](assets/collapse-all-icon.png) pour réduire toutes les zones.
      * Cliquez sur l’icône **Modifier** ![Modifier](assets/edit-icon.png), puis sélectionnez l’une des zones ci-dessous, ou cliquez sur **Modifier tout** pour modifier les informations de toutes les zones :

         * Vue d’ensemble
         * Forms personnalisé
Les noms des formulaires de douane s’affichent uniquement si des formulaires personnalisés sont joints à la tâche de modèle.
         * Finances

        >[!TIP]
        >
        >Pour plus d’informations sur tous les champs qui s’affichent dans la zone Détails , continuez à modifier tous les champs à l’aide de la zone Modifier la tâche de modèle , comme décrit ci-dessous.

   1. (Facultatif) Cliquez sur la section **Sous-tâches** dans le panneau de gauche pour ajouter des enfants à la tâche de modèle. L’ajout de sous-tâches pour les tâches de modèle est similaire à l’ajout de sous-tâches de projet. Pour plus d’informations, reportez-vous à la section « Création de sous-tâches à partir de la section Sous-tâches de la tâche » de l’article [Création de sous-tâches](/help/quicksilver/manage-work/tasks/create-tasks/create-subtasks.md).
   1. (Facultatif) Cliquez sur **Dépenses** dans le panneau de gauche et ajoutez des dépenses aux tâches de modèle. Les dépenses liées aux tâches de modèle sont transférées vers les tâches de projets futurs lorsque le modèle est utilisé pour créer un projet.
   1. (Facultatif) Cliquez sur **Approbations** dans le panneau de gauche pour créer des approbations ou joindre des approbations globales ou au niveau du groupe aux tâches de modèle. Les approbations sont transférées vers des tâches de projets futurs.
   1. (Facultatif) Cliquez sur la section **Prédécesseurs** dans le panneau de gauche pour ajouter des prédécesseurs pour les tâches de modèle. L’ajout de prédécesseurs de tâche de modèle est similaire à l’ajout de prédécesseurs de tâche de projet. Pour plus d’informations, voir [Créer une relation de prédécesseur à l’aide de la zone Prédécesseurs](/help/quicksilver/manage-work/tasks/use-prdcssrs/create-predecessors-in-predecessors-area.md).

1. (Conditionnel) Pour modifier toutes les informations relatives à une tâche de modèle ou à plusieurs tâches en même temps, cliquez sur les tâches pour les sélectionner dans une liste, puis cliquez sur l’icône **Modifier** ![Modifier](assets/edit-icon.png) en haut de la liste.

   La zone **Modifier la tâche de modèle** s’affiche.

   ![Nouvelle expérience pour Modifier la tâche de modèle](assets/edit-template-task-box-unshimmed.png)

   >[!TIP]
   >
   >Vous pouvez également sélectionner une tâche de modèle dans une liste, puis cliquer sur **Modifier** à droite du nom de la tâche de modèle dans l’en-tête, pour ouvrir la zone **Modifier la tâche de modèle**.

1. Pensez à spécifier des informations dans l’une des sections suivantes :

* [Nom de la tâche de modèle](#template-task-name)
* [Vue d’ensemble](#overview-2)
* [Affectations](#assignments-2)
* [Finances](#finance-2)
* [Formulaires personnalisés](#custom-forms-2)
* [Paramètres](#settings-2)
* [Commentaire](#comment-2)

1. Continuez à modifier les tâches de modèles comme décrit dans les sections ci-dessous.

#### Nom de tâche de modèle

>[!TIP]
>
>La section Nom de la tâche de modèle n’est pas disponible lors de la modification de tâches de modèle en bloc.


1. Commencez à modifier une tâche de modèle comme décrit ci-dessus.
1. Dans la zone Modifier la tâche de modèle, cliquez sur **Nom de la tâche de modèle** et ajoutez un nom pour la tâche de modèle.

   Cette vue n’est pas disponible lors de la modification de tâches de modèle en bloc.

1. (Facultatif) Continuez à modifier les sections suivantes, en fonction des informations que vous souhaitez modifier.

   Ou

   Cliquer sur **Enregistrer**.

#### Vue d’ensemble {#overview-2}

1. Commencez à modifier une tâche de modèle comme décrit ci-dessus.
1. Dans la zone **Modifier la tâche de modèle**, cliquez sur **Aperçu** dans le panneau de gauche.

   ![Section de présentation de la modification de la tâche de modèle](assets/template-task-edit-overview.png)

1. Mettez à jour l’un des éléments suivants :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Description</strong> </td> 
      <td>Ajoutez des informations supplémentaires sur la tâche de modèle.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Priorité</strong> </td> 
      <td> <p>Il s’agit d’un indicateur visuel qui vous permet de hiérarchiser vos tâches de modèle. </p> <p>Sélectionnez l’une des options suivantes :</p> 
       <ul> 
        <li> <p><strong>Aucune</strong> </p> </li> 
        <li> <p><strong>Faible</strong> </p> </li> 
        <li> <p> <b>Normale</b></p> </li> 
        <li> <p><b>Élevée</b> </p> </li> 
        <li> <p><b>Urgente</b> </p> </li> 
       </ul> <p>Selon les préférences du projet sélectionnées par votre administrateur ou administratrice Workfront, les noms des priorités peuvent être différents pour vous. Pour plus d’informations sur la modification des priorités, voir la section <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md" class="MCXref xref">Créer et personnaliser des priorités</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Contrainte de tâche</strong> </td> 
      <td> <p>La tâche sur le projet créé à partir de ce modèle aura cette contrainte. Les contraintes de tâche déterminent à quel moment une tâche doit être terminée. </p> <p>Sélectionnez l’une des options suivantes :</p> 
       <ul> 
        <li><strong>Dates fixes</strong>. Spécifiez une <strong>Date de début prévue</strong> et une <strong>Date d’achèvement prévue</strong>.</li> 
        <li><strong>Il faut commencer le</strong>. Spécifiez une <strong>Date de début prévue</strong>.</li> 
        <li><strong>Il faut finir le</strong>. Spécifiez une <strong>Date d’achèvement prévue</strong>.</li> 
        <li><strong>Aussi tôt que possible</strong> </li> 
        <li><strong>Aussi tard que possible</strong> </li> 
        <li style="font-weight: bold;"><strong>Première heure disponible</strong> </li> 
        <li style="font-weight: bold;"><strong>Dernière heure disponible</strong> </li> 
        <li>Commencer au plus tard. Spécifiez une <strong>Date de début prévue</strong>.</li> 
        <li><strong>Commencer Au Plus Tôt</strong>. Spécifiez une <strong>Date de début prévue</strong>.</li> 
        <li><strong>Finir Au Plus Tard</strong>. Spécifiez une <strong>Date d’achèvement prévue</strong>.</li> 
        <li><strong>Finir Au Plus Tôt</strong>. Spécifiez une <strong>Date d’achèvement prévue</strong>.</li> 
       </ul> <p>Pour plus d’informations sur la contrainte de tâche, voir <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Vue d’ensemble de la contrainte de tâche</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span style="font-weight: bold;">Jour de début</span><span style="font-weight: normal;"> (facultatif et le cas échéant)</span> </td> 
      <td> <p> Vous ne pouvez spécifier le Jour de début d'une tâche de modèle que lorsque la Contrainte de tâche est l'une des suivantes :</p> 
       <ul> 
        <li>Il Faut Commencer Le</li> 
        <li>Commencer Au Plus Tôt</li> 
        <li>Commencer Au Plus Tard</li> 
        <li>Dates fixes</li> 
       </ul> <p>Cela correspondra à la date dans la chronologie du futur projet à laquelle la tâche démarrera. Pour toutes les autres contraintes, Workfront calcule le Jour de début en fonction de la dépendance d’antériorité entre les tâches. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Jour d’achèvement</strong><span style="font-weight: normal;"> (facultatif et le cas échéant)</span> </td> 
      <td> <p> Vous ne pouvez spécifier le jour d’achèvement d’une tâche de modèle que lorsque la contrainte de tâche est l’une des suivantes :</p> 
       <ul style="list-style-type: circle;"> 
        <li>Il Faut Finir Le</li> 
        <li>Finir Au Plus Tôt</li> 
        <li>Finir Au Plus Tard</li> 
        <li>Dates fixes</li> 
       </ul> <p>Cela correspondra à la date dans la chronologie du futur projet à laquelle la tâche sera terminée. Pour toutes les autres contraintes, Workfront calcule le jour d’achèvement en fonction de la durée et de la dépendance des tâches antérieures. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>URL</strong> </td> 
      <td>Spécifiez un lien web qui se rapporte aux informations sur la tâche de modèle.</td> 
     </tr>

   <tr> 
      <td role="rowheader"><strong>Effort de travail</strong> </td> 
      <td>Choisissez l’une des options suivantes :
      <ul><li>Petite</li>
      <li>Moyen</li>
      <li>Grande</li></ul>

   <p><b>IMPORTANT</b></p>
      <p>Le champ Effort de travail s’affiche lors de la modification d’une tâche de modèle uniquement lorsque vous sélectionnez le paramètre <b> Utiliser l’effort de travail pour calculer automatiquement le nombre d’heures prévues de la tâche </b> lors de la modification du modèle.</p>

   </td> 
     </tr> 
     </tbody> 
   </table>

1. (Facultatif) Continuez à modifier les sections suivantes, en fonction des informations que vous souhaitez modifier.

   Ou

   Cliquer sur **Enregistrer**.

#### Affectations {#assignments-2}

1. Commencez à modifier votre tâche de modèle comme décrit ci-dessus.
1. Cliquez sur **Affectations** dans le panneau de gauche.

   La zone **Affectations** s’ouvre.

   ![Affectations sur les tâches de modèles](assets/assignments-edit-template-tasks-box.png)

1. Commencez à saisir le nom d’un utilisateur, d’une fonction ou d’une équipe dans le champ **Rechercher des personnes, un rôle ou une équipe**, puis sélectionnez-les lorsqu’elles s’affichent dans la liste.

1. Mettez à jour les informations suivantes :

   <table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">Type de durée</td> 
   <td> <p>Cela identifie la relation entre les éléments suivants : </p> 
   <ul> 
   <li> <p>Nombre de ressources affectées à une tâche </p> </li> 
   <li> <p>Effort total requis pour terminer la tâche </p> </li> 
   <li> <p> Durée totale de la tâche. </p> </li> 
   </ul> <p>Votre administrateur Workfront ou un administrateur de groupes sélectionne le paramètre Type de durée par défaut pour les tâches de votre système ou de votre groupe. Pour plus d'informations sur la définition des paramètres par défaut du projet, voir <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md" class="MCXref xref">Configurer les préférences de tâches et de problèmes à l'échelle du système</a>. </p> <p>Les types de durée vous permettent de définir des affectations de ressources cohérentes en fonction des besoins de la tâche. Pour plus d’informations sur le type de durée d’une tâche, voir <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Vue d’ensemble de la durée de la tâche et du type de durée</a>. </p> <p>Sélectionnez l’une des options suivantes : </p> 
   <ul> 
   <li> <p>Calcul d'affectation </p> </li> 
   <li> <p> Calcul de travail </p> </li> 
   <li> <p>Piloté par l'effort </p> </li> 
   <li> <p>Simple</p> </li> 
   </ul> </td> 
   </tr> 
   <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td role="rowheader">Durée par occurrence</td> 
   <td> <p>Cela s’affiche uniquement sur le parent des tâches récurrentes. La durée de chaque tâche récurrente est affichée, telle que définie lors de la création de la tâche. Pour plus d’informations sur la création de tâches récurrentes, voir <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Créer des tâches récurrentes</a>. </p> <p> <b>NOTE</b>

   Les durées modifiées dans des tâches récurrentes individuelles n’affichent pas la valeur indiquée dans ce champ. </p> </td>
   </tr> 
   <tr> 
   <td role="rowheader">Durée</td> 
   <td> 
   <div> 
   <div> 
   <p>Il s’agit de la durée pendant laquelle vous laissez une tâche ouverte avant qu’elle soit terminée. </p> 
   <p><b>IMPORTANT</b></p>
   <p>Comme la durée de la tâche correspond généralement à la durée entre les dates de début et d’achèvement prévues, elle affecte la chronologie du projet.</p> 
   <p>Pour indiquer la durée de la tâche et l’unité de temps, procédez comme suit :</p> 
   <ul> 
   <li> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Saisissez la durée et sélectionnez l’unité de temps disponible dans le menu déroulant.</p> <p><b>CONSEIL</b></p>
   Lorsque vous mettez à jour la durée des tâches dans une liste de tâches, vous pouvez utiliser l’abréviation pour l’unité de temps. </p> </li> 
   </ul> 
   <p> Vous pouvez choisir parmi les options de temps normal ou de temps écoulé dans le tableau suivant : </p> 
   <table style="table-layout:auto"> 
   <col> 
   <col data-mc-conditions=""> 
   <tbody> 
   <tr> 
   <td>Unité de temps</td> 
   <td>Abréviation</td> 
   </tr> 
   <tr> 
   <td>Minutes</td> 
   <td>L</td> 
   </tr> 
   <tr> 
   <td>Heures</td> 
   <td>H</td> 
   </tr> 
   <tr> 
   <td>Jours. Il s’agit de la valeur par défaut. </td> 
   <td>Dés</td> 
   </tr> 
   <tr> 
   <td>Semaines</td> 
   <td>S</td> 
   </tr> 
   <tr> 
   <td>Mois</td> 
   <td>M</td> 
   </tr> 
   <tr> 
   <td>Minutes écoulées</td> 
   <td>ME</td> 
   </tr> 
   <tr> 
   <td>Heures écoulées</td> 
   <td>HE</td> 
   </tr> 
   <tr> 
   <td>Jours écoulés</td> 
   <td>JE</td> 
   </tr> 
   <tr> 
   <td>Semaines écoulées</td> 
   <td>SE</td> 
   </tr> 
   <tr> 
   <td>Mois écoulés</td> 
   <td>TE</td> 
   </tr> 
   </tbody> 
   </table>

   <p><b>NOTE</b>

   <p>Le temps écoulé est une unité de temps pour la durée d’une tâche. Il s’agit de la durée entre la date de début et la date d’achèvement prévues d’une tâche qui comprend les jours fériés, les week-ends et les jours de congé. En d’autres termes, le temps écoulé est le nombre de jours calendaires écoulés.

   Le temps normal prend en compte les jours fériés, les week-ends et les jours de congé et les exclut de la durée de la tâche. Pour plus d’informations sur la durée de la tâche, voir <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Vue d’ensemble de la durée de la tâche et du type de durée</a>. </p>
   </div> 
   </div> </td> 
   </tr> 
   <tr> 
   <td role="rowheader">Heures prévues</td> 
   <td> <p>Spécifiez le nombre d’heures prévues pour la tâche, en heures. Il s’agit de la quantité de temps réel nécessaire aux personnes assignées à la tâche pour la terminer. Vous ne pouvez spécifier le nombre d'heures prévues pour une tâche que lorsque le type de durée est défini sur Calcul d'affectation. Pour plus d’informations sur les types de durée, voir <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Vue d’ensemble de la durée de la tâche et du type de durée</a>.</p> 
   <b>NOTE</b>
   <p>
   Lors de la création de tâches récurrentes, les heures prévues sont celles de chaque occurrence. Les heures prévues des tâches parent correpondent au nombre total d’heures prévues de toutes les occurrences. Pour plus d’informations sur la création de tâches récurrentes, voir <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Créer des tâches récurrentes</a>.
   </p>

   </td> 
   </tr> 
   <tr> 
   <td role="rowheader">Allocation</td> 
   <td> <p>Si la contrainte de tâche est Calcul de travail ou Piloté par l’effort, spécifiez la variable <strong>% d’affectation</strong> (pourcentage d’affectation) pour chaque personne cessionnaire. Il s’agit de la durée dans le planning de la personne cessionnaire qui peut être consacrée à cette tâche. La modification du pourcentage d’affectation d’une personne cessionnaire modifie le nombre d’heures prévues d’une tâche. </p> <p>Lorsque la contrainte de tâche est simple, vous pouvez spécifier les éléments suivants :</p> 
   <ul> 
   <li> <p>Nombre d’heures d’affectation de chaque personne cessionnaire.</p> </li> 
   <li> <p>Nombre d’heures prévues de la tâche.</p> </li> 
   <li> <p>Durée de la tâche.</p> </li> 
   </ul> </td> 
   </tr> 
   <tr> 
   <td role="rowheader">Rôle du cessionnaire</td> 
   <td> <p>Sélectionnez un rôle dans le menu déroulant <strong>Rôle de la personne cessionnaire</strong> lorsque vous avez sélectionné une personne comme personne cessionnaire. Il s’agit du rôle que la personne cessionnaire peut remplir pour cette tâche. </p> <p><b>CONSEIL</b>

   Seules les fonctions associées à chaque personne cessionnaire dans son profil s’affichent dans le menu déroulant.</p> </td>
   </tr> 
   </tbody> 
   </table>

1. Cliquez sur **Enregistrer** ou passez aux sections suivantes.

#### Finances {#finance-2}

1. Commencez à modifier une tâche de modèle comme décrit ci-dessus.
1. Dans la zone **Modifier la tâche de modèle**, cliquez sur **Finances** dans le panneau de gauche.

   ![Section Modifier les finances de la tâche de modèle](assets/template-task-edit-finance.png)

1. Mettez à jour l’un des éléments suivants :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Type de coût</strong> </td> 
      <td> <p>Indiquez le type de coût de la tâche à venir. Cette option détermine la manière dont le coût de la tâche est calculé, sur la base du nombre d’heures consacrées à la tâche. </p> <p>Sélectionnez l’une des options suivantes :</p> 
       <ul> 
        <li> <p style="font-weight: normal;"><span>Aucun coût</span> </p> </li> 
        <li> <p style="font-weight: normal;"><span>Fixe par heure</span> </p> </li> 
        <li> <p style="font-weight: normal;"><span>Utilisateur ou utilisatrice, par heure</span> </p> </li> 
        <li> <p style="font-weight: normal;"><span>Rôle par heure</span> </p> </li> 
       </ul> <p>Pour plus d’informations sur le suivi des coûts, consultez la section <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Suivi des coûts</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Type de revenu</strong> </td> 
      <td> <p>Indiquez le type de revenu pour la tâche à venir. Cela détermine comment le revenu de la tâche est calculé en fonction du nombre d’heures passées sur les tâches.</p> <p style="font-weight: normal;">Sélectionnez l’une des options suivantes : </p> 
       <ul> 
        <li> <p style="font-weight: normal;">Non facturable</p> </li> 
        <li> <p style="font-weight: normal;">Utilisateur, par heure</p> </li> 
        <li> <p style="font-weight: normal;">Rôle par heure</p> </li> 
        <li> <p style="font-weight: normal;">Fixe par heure</p> </li> 
        <li> <p style="font-weight: normal;">Utilisateur par heure avec limite</p> </li> 
        <li> <p style="font-weight: normal;">Rôle par heure avec limite</p> </li> 
        <li> <p style="font-weight: normal;">Utilisateur, par heure plus fixe</p> </li> 
        <li> <p style="font-weight: normal;">Rôle par heure plus fixe</p> </li> 
        <li> <p style="font-weight: normal;">Revenus fixes</p> </li> 
       </ul> <p>Pour plus d’informations sur le suivi des revenus, consultez la section <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Vue d’ensemble de la facturation et des revenus</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Facultatif) Continuez à modifier les sections suivantes, en fonction des informations que vous souhaitez modifier.

   Ou

   Cliquer sur **Enregistrer**.

#### Formulaires personnalisés {#custom-forms-2}

Vous pouvez définir des formulaires personnalisés à joindre automatiquement par défaut aux tâches lorsque les tâches sont ajoutées à un projet. Pour plus d’informations sur la configuration du projet afin d’inclure les formulaires personnalisés de tâche par défaut, consultez la section « Tâches » de l’article [Modifier des projets](../../../manage-work/projects/manage-projects/edit-projects.md).

Vous pouvez également ajouter des formulaires personnalisés aux tâches futures d’un projet lorsque celui-ci sera créé à partir d’un modèle, en ajoutant les formulaires personnalisés aux tâches de modèle.

1. Commencez à modifier une tâche de modèle comme décrit ci-dessus.
1. Dans la zone **Modifier la tâche de modèle**, cliquez sur **Forms personnalisé** dans le panneau de gauche.

   ![Section Modifier les formulaires personnalisés de la tâche de modèle](assets/template-task-edit-custom-forms.png)

1. Sélectionnez le ou les formulaires personnalisés à associer à la tâche de modèle.

   Vous devez créer les formulaires personnalisés avant qu’ils ne puissent être sélectionnés dans ce champ.
Seuls les formulaires personnalisés actifs sont affichés dans la liste.

   Pour plus d’informations sur la création de formulaires personnalisés, voir [Créer un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

   Vous pouvez ajouter jusqu’à dix formulaires personnalisés à une tâche de modèle.
Les formulaires sont automatiquement ajoutés aux tâches créées à partir du modèle.
1. (Le cas échéant et facultatif) Si vous avez joint un formulaire personnalisé à la tâche de modèle, modifiez les champs du formulaire concernés. Vous devez spécifier tous les champs requis avant de pouvoir enregistrer la tâche de modèle.

   >[!NOTE]
   >
   >Selon la manière dont votre équipe d’administration Workfront définit les autorisations pour les sections de votre formulaire personnalisé, tout le monde ne peut pas afficher ou modifier les mêmes champs sur un formulaire personnalisé donné. Les autorisations de modifier les champs d’une section d’un formulaire personnalisé dépendent des autorisations que vous avez sur la tâche de modèle ou la tâche future.\
   >Pour plus d’informations sur la configuration des autorisations pour des sections d’un formulaire personnalisé, consultez la section [Partager un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).\
   >Pour plus d’informations sur la configuration des autorisations pour une tâche, voir [Partager une tâche](../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md).\
   >Pour plus d’informations sur la configuration des autorisations pour un modèle, voir [Partager un modèle](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

1. (Facultatif) Continuez à modifier la section suivante, en fonction des informations que vous souhaitez modifier.

   Ou

   Cliquer sur **Enregistrer**.

#### Paramètres {#settings-2}

1. Commencez à modifier une tâche de modèle comme décrit ci-dessus.
1. Dans la boîte de dialogue **Modifier la tâche de modèle**, cliquez sur **Paramètres** dans le panneau de gauche.

   ![Section des paramètres de modification de la tâche de modèle](assets/template-task-edit-settings.png)

1. Mettez à jour l’un des éléments suivants :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
   <tr> 
      <td role="rowheader"><p><b>Jalon</b></p></strong> </td> 
      <td> <p>Sélectionnez un jalon à associer à la tâche de modèle sélectionnée.</p>

   <p><b>IMPORTANT</b></p>
   <p>Vous devez associer un chemin jalonné à un modèle pour que ce champ s’affiche. Pour plus d’informations, consultez la section <a href="../create-and-manage-templates/edit-templates.md">Modifier des modèles de projet</a>.</p> 
   </td> 
     </tr>
     <tr> 
      <td role="rowheader"><strong>Mode de suivi</strong> </td> 
      <td> <p>Indiquez le mode de suivi du statut de progression de la tâche à venir. </p> <p>Sélectionnez l’une des options suivantes :</p> 
       <ul> 
        <li> <p><strong>Utilisateur ou utilisatrice doit mettre à jour</strong>. </p> </li> 
        <li> <p><strong>Supposer à l’heure</strong> </p> </li> 
        <li> <p><strong>Ignorer avertissements de retard</strong> </p> </li> 
        <li> <p><strong>Conclusion automatique</strong> </p> </li> 
        <li> <p><strong>Tâche antérieure</strong> </p> </li> 
       </ul> <p>Pour plus d’informations sur le mode de suivi des tâches, consultez la section <a href="../../../manage-work/tasks/task-information/task-tracking-mode.md" class="MCXref xref">Vue d’ensemble du mode de suivi des tâches</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Notifications de rappel</strong> </td> 
      <td> <p>Sélectionnez les notifications de rappel que vous souhaitez joindre à la tâche de modèle. Elles seront jointes aux futures tâches du projet créé à partir de ce modèle. L’administrateur ou administratrice système doit configurer les notifications de rappel avant que vous ne puissiez les sélectionner sur une tâche. Pour plus d’informations sur la configuration des notifications de rappel, voir <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">Configurer des notifications de rappel</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Processus d’approbation</strong> </td> 
      <td> <p>Sélectionnez le processus d’approbation que vous souhaitez associer à la tâche de modèle. Votre administrateur ou votre administratrice Workfront doit définir des processus d’approbation des tâches au niveau du système avant de pouvoir les associer à des tâches de modèle. <span>Un utilisateur ou une utilisatrice disposant d’un accès administratif aux processus d’approbation peut également créer des processus d’approbation spécifiques à un groupe.</span>Pour plus d’informations sur la création de processus d’approbation, voir <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Créer un processus d’approbation pour les éléments de travail</a>.</p> <p>Tenez compte des éléments suivants lorsque vous ajoutez des processus d’approbation : </p> 
       <ul> 
       <li>Seuls les processus d’approbation actifs sont affichés dans la liste. </li> 
       <li> <p>Les processus d’approbation à l’échelle du système et spécifiques au groupe s’affichent dans la liste. Les processus d’approbation associés à un groupe autre que celui du modèle ne s’affichent pas dans la liste.</p> <p>Important : si le groupe associé au modèle change, le processus d’approbation spécifique au groupe devient un processus d’approbation à usage unique. Pour plus d’informations sur la façon dont les modifications apportées au groupe du projet ou au processus d’approbation affectent les paramètres d’approbation, voir la section <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">Effets des modifications du processus d’approbation et de groupe sur les processus d’approbation affectés</a>. </p> </li> 
       <li> <p>Si vous avez ajouté un processus d’approbation à usage unique, il s’affiche sous la forme « &lt;Personnalisé&gt; » dans ce champ. Pour plus d’informations, voir <a href="../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md" class="MCXref xref">Associer un processus d’approbation nouveau ou existant au travail</a>. </p>  </li> 
       <li> <p>Lors de la modification en masse de tâches de modèle, les scénarios suivants existent :</p> 
       <ul> 
       <li> <p>Lorsque vous sélectionnez des tâches de modèle dans le même groupe de modèles, les processus d’approbation au niveau du système et du groupe s’affichent dans ce champ.</p> </li> 
       <li> <p>Lorsque vous sélectionnez des tâches de modèle dans différents groupes de modèles, seuls les processus d’approbation au niveau du système s’affichent dans ce champ.</p> </li> 
       <li> <p>Lorsque l’une des tâches de modèle est associée à un processus d’approbation à usage unique, il est remplacé par le <span>processus d’approbation au niveau du système ou au niveau du groupe</span> que vous sélectionnez. </p> </li> 
       </ul> </li> 
       </ul> </td> 
     </tr>

   </tbody> 
   </table>

1. (Facultatif) Continuez à modifier les sections suivantes, en fonction des informations que vous souhaitez modifier.

   Ou

   Cliquer sur **Enregistrer**.

#### Commentaire {#comment-2}

1. Commencez à modifier une tâche de modèle comme décrit ci-dessus.
1. Dans la zone **Modifier la tâche de modèle**, cliquez sur **Commentaire** dans le panneau de gauche.

   ![Section Modifier le commentaire de la tâche de modèle](assets/template-task-edit-comment.png)

1. Dans la zone **Ajouter une mise à jour à la tâche de modèle**, indiquez un commentaire que vous souhaitez afficher dans le flux de mises à jour de la tâche de modèle dans le champ disponible. Ce commentaire est visible par toutes les personnes ayant un accès en affichage au modèle et à la tâche de modèle, ainsi qu’ayant un accès à l’affichage des notes.
1. Cliquer sur **Enregistrer**.

   Lorsque vous ou une autre personne créez un projet à partir de ce modèle, tous les paramètres que vous avez appliqués aux tâches de modèle deviennent les paramètres des tâches du projet.

</div>


