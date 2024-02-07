---
product-area: templates
keywords: tâche,valeurs par défaut,automate,création
navigation-topic: templates-navigation-topic
title: Modifier une tâche de modèle
description: Après avoir créé un modèle, vous pouvez modifier les informations relatives aux tâches du modèle. Les informations que vous mettez à jour sur une tâche de modèle sont associées à des tâches de projet une fois que vous avez utilisé le modèle pour créer un projet ou que vous avez joint le modèle à un projet.
author: Alina
feature: Work Management
exl-id: 2df8522e-7eee-4440-be0f-f7483c5acdb0
source-git-commit: 420a9c24695f950ad191431ca6c6848b7649f3b1
workflow-type: tm+mt
source-wordcount: '2384'
ht-degree: 4%

---

# Modifier une tâche de modèle

Après avoir créé un modèle, vous pouvez modifier les informations relatives aux tâches du modèle. Les informations que vous mettez à jour sur une tâche de modèle sont associées à des tâches de projet une fois que vous avez utilisé le modèle pour créer un projet ou que vous avez joint le modèle à un projet.

Pour plus d’informations sur la création d’un modèle, voir [Création d’un modèle de projet](../../../manage-work/projects/create-and-manage-templates/create-template.md).

Vous pouvez modifier la tâche de modèle ou modifier les tâches de modèle en bloc.

>[!NOTE]
>
>Vous ne pouvez pas modifier en bloc des tâches de modèle qui appartiennent à différents modèles. Vous ne pouvez modifier que les tâches de modèle qui appartiennent au même modèle.


## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td> <p>Quelconque</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Nouveau : Standard </p>
   <p>Actuel : formule </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Niveau d’accès</td> 
   <td> <p>Modifier l’accès aux modèles</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet </td> 
   <td> <p>Gérer les autorisations d’un modèle. </p> <p>Contribuez à la tâche de modèle ou à des autorisations supérieures.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Pour connaître votre plan, votre type de licence ou votre niveau d’accès, contactez votre administrateur Workfront. Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Conditions préalables

Avant de commencer, vous devez

* Créez un modèle.

  Pour plus d’informations sur la création d’un modèle, voir [Création d’un modèle de projet](../../../manage-work/projects/create-and-manage-templates/create-template.md).

## Tâche Modifier le modèle

Vous pouvez modifier une tâche de modèle à l’aide des zones Modifier la tâche de modèle ou Détails de la tâche de modèle. Les étapes suivantes décrivent la modification d’une tâche dans la zone Modifier la tâche du modèle .

{{step1-to-templates}}

1. Cliquez sur le nom d’un modèle pour l’ouvrir.
1. Cliquez sur **Tâches de modèle** dans le panneau de gauche.
1. Cliquez sur le nom d’une tâche de modèle dans la liste pour ouvrir la tâche de modèle.
1. (Facultatif) Pour modifier plusieurs tâches de modèle en bloc, sélectionnez plusieurs tâches de modèle, puis cliquez sur **Modifier** en haut de la liste des modèles.
1. (Conditionnel) Pour modifier des informations limitées sur une tâche de modèle, cliquez sur **Détails de la tâche de modèle** dans le panneau de gauche, accédez aux sections de la section Détails pour modifier les informations de chaque zone.
1. (Facultatif) Cliquez sur le **Réduire tout** icon ![](assets/collapse-all-icon.png) pour réduire toutes les zones.
1. Pour modifier les informations de la section Détails, cliquez sur le bouton **Modifier** icon ![](assets/edit-icon.png), puis sélectionnez l’une des zones ci-dessous ou cliquez sur **Tout modifier** pour modifier les informations dans toutes les zones :

   * Vue d’ensemble
   * Formulaires personnalisés

     Les noms des formulaires douaniers ne s’affichent que s’il existe des formulaires personnalisés associés à l’objet.

   * Finances

   >[!TIP]
   >
   >Pour plus d’informations sur tous les champs qui s’affichent dans la zone Détails, continuez à modifier tous les champs à l’aide de la zone Modifier la tâche du modèle ci-dessous.

1. (Conditionnel) Pour modifier toutes les informations relatives à la tâche de modèle, cliquez sur le bouton **Plus** menu ![](assets/qs-more-icon-on-an-object.png) en regard du nom de la tâche de modèle, puis cliquez sur **Modifier**.

   La variable **Modifier la tâche du modèle** s’affiche.

   >[!TIP]
   >
   >Vous pouvez également sélectionner une tâche de modèle dans une liste, puis cliquer sur Modifier pour ouvrir la zone Modifier la tâche de modèle .

   ![](assets/edit-template-tasks-box-classic-350x356.png)

1. Pensez à spécifier des informations dans l’une des sections suivantes :

   * [Vue d’ensemble](#overview)
   * [Finances](#finance)
   * [Paramètres](#settings)
   * [Affectations](#assignments)
   * [Formulaires personnalisés](#custom-forms)
   * [Commentaire](#comment)

### Vue d’ensemble {#overview}

1. Commencez à modifier une tâche de modèle comme décrit ci-dessus.
1. Cliquez sur **Présentation**.

   ![edit_task_overview.png](assets/edit-task-overview-350x438.png)

1. Mettez à jour l’un des éléments suivants :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Nom</strong> </td> 
      <td>Spécifiez un nom pour la tâche de modèle. Ce champ ne s’affiche pas lors de l’édition groupée de tâches de modèle.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Description</strong> </td> 
      <td>Ajoutez des informations supplémentaires sur la tâche de modèle.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>URL</strong> </td> 
      <td>Spécifiez un lien Web qui se rapporte aux informations sur la tâche de modèle.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Priorité</strong> </td> 
      <td> <p>Il s’agit d’un indicateur visuel qui vous permet de prioriser vos tâches de modèle. </p> <p>Sélectionnez l’une des options suivantes :</p> 
       <ul> 
        <li> <p><strong>Aucun</strong> </p> </li> 
        <li> <p><strong>Faible</strong> </p> </li> 
        <li> <p> <b>Normal</b></p> </li> 
        <li> <p><b>Élevée</b> </p> </li> 
        <li> <p><b>Urgent</b> </p> </li> 
       </ul> <p>Selon les préférences du projet sélectionnées par votre administrateur Workfront, les noms des priorités peuvent être différents pour vous. Pour plus d’informations sur la modification des priorités, voir <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md" class="MCXref xref">Créer et personnaliser des priorités</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Type de durée</strong> </td> 
      <td> <p>La future tâche créée à partir de ce modèle aura ce type de durée. <br>Le type de durée identifie la relation entre les éléments suivants :</p> <p>- nombre de ressources affectées à une tâche</p> <p>: effort total requis pour terminer la tâche</p> <p>: durée totale de la tâche. </p> <p>Les types de durée vous permettent de définir des affectations de ressources cohérentes en fonction des besoins de la tâche. Pour plus d’informations sur le type de durée d’une tâche, voir <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Présentation de la durée et du type de durée de la tâche</a>.</p> <p>Sélectionnez l’une des options suivantes :</p> 
       <ul> 
        <li> <p style="font-weight: bold;"><span style="font-weight: normal;">Attribution calculée</span> </p> </li> 
        <li> <p style="font-weight: bold;"><span style="font-weight: normal;">Travail calculé</span> </p> </li> 
        <li> <p style="font-weight: bold;"><span style="font-weight: normal;">Effort piloté</span> </p> </li> 
        <li> <p style="font-weight: bold;"><span style="font-weight: normal;">Simple</span> <br> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Durée</strong> </td> 
      <td> <p>Indiquez la Durée des tâches futures, en minutes, heures, jours, semaines ou mois. La durée de la tâche créée à partir de ce modèle sera spécifiée ici dans la tâche ultérieure.</p> <p>Par défaut, Workfront mesure la durée en jours. Il s’agit de la durée pendant laquelle la tâche doit rester incomplète avant d’être terminée. Vous ne pouvez pas spécifier la durée d’une tâche lorsque la variable <strong>Type de durée</strong> de la tâche est <strong>Simple</strong>, ou lorsque la variable <strong>Contrainte de tâche</strong> is <strong>Dates fixes</strong>.</p> <p><b>IMPORTANT</b></p> <p>La durée correspond généralement au temps entre le début planifié et les dates de fin planifiées d’une tâche de modèle. Pour cette raison, elle affecte la chronologie du modèle. Cela détermine la chronologie du futur projet créé à partir du modèle. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Heures planifiées</strong> </td> 
      <td> <p>Indiquez le nombre d’heures planifiées pour la tâche à venir sur le projet créé avec ce modèle. Il s’agit du temps réel nécessaire aux personnes désignées de la tâche pour l’exécuter. Vous pouvez uniquement spécifier le nombre d’heures planifiées d’une tâche lorsque la variable <strong>Type de durée</strong> est défini sur <strong>Attribution calculée</strong>. </p> </td> 
     </tr>

   <tr> 
      <td role="rowheader"><strong>Contrainte de tâche</strong> </td> 
      <td> <p>La tâche sur le projet créé à partir de ce modèle aura cette contrainte. Les contraintes de tâche déterminent à quel moment une tâche doit être terminée. </p> <p>Sélectionnez l’une des options suivantes :</p> 
       <ul> 
        <li><strong>Dates fixes</strong>. Spécifiez un <strong>Démarrage planifié</strong> et un <strong>Date d’achèvement prévue.</strong></li> 
        <li><strong>Doit démarrer le</strong>. Spécifiez un <strong>Date de début planifiée.</strong></li> 
        <li><strong>Doit Terminer le</strong>. Spécifiez un <strong>Date d’achèvement prévue</strong>.</li> 
        <li><strong>Dès que possible</strong> </li> 
        <li><strong>Aussi tard que possible</strong> </li> 
        <li style="font-weight: bold;"><strong>Heure disponible la plus tôt</strong> </li> 
        <li style="font-weight: bold;"><strong>Dernière heure disponible</strong> </li> 
        <li>Ne Démarrez Pas Plus Tard Que . Spécifiez un <strong>Date de début planifiée</strong>.</li> 
        <li><strong>Ne Commencer Pas Au Plus Tôt</strong>. Spécifiez un <strong>Date de début planifiée</strong>.</li> 
        <li><strong>Terminer au plus tard</strong>. Spécifiez un <strong>Date d’achèvement prévue</strong>.</li> 
        <li><strong>Terminer au plus tôt</strong>. Spécifiez un <strong>Date d’achèvement prévue</strong>.</li> 
       </ul> <p>Pour plus d’informations sur la contrainte de tâche, voir <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Présentation de la contrainte de tâche</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span style="font-weight: bold;">Jour de début</span><span style="font-weight: normal;"> (facultatif et conditionnel)</span> </td> 
      <td> <p> Vous pouvez spécifier le Jour de début d’une tâche de modèle uniquement lorsque la contrainte de tâche est l’une des suivantes :</p> 
       <ul> 
        <li>Il Faut Commencer Le</li> 
        <li>Ne Commencer Pas Au Plus Tôt</li> 
        <li>Commencer Au Plus Tard</li> 
        <li>Dates fixes</li> 
       </ul> <p>Cela correspondra à la date dans la chronologie du futur projet à laquelle la tâche démarrera. Pour toutes les autres contraintes, Workfront calcule le Jour de début en fonction de la dépendance du prédécesseur entre les tâches. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Jour d’achèvement</strong><span style="font-weight: normal;"> (facultatif et conditionnel)</span> </td> 
      <td> <p> Vous ne pouvez spécifier le jour de fin d’une tâche de modèle que lorsque la contrainte de tâche est l’une des suivantes :</p> 
       <ul style="list-style-type: circle;"> 
        <li>Il Faut Finir Le</li> 
        <li>Finir Au Plus Tôt</li> 
        <li>Finir Au Plus Tard</li> 
        <li>Dates fixes</li> 
       </ul> <p>Cela correspondra à la date dans la chronologie du futur projet à laquelle la tâche sera terminée. Pour toutes les autres contraintes, Workfront calcule le jour d’achèvement en fonction de la durée et de la dépendance de prédécesseur. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Facultatif) Continuez à modifier les sections suivantes en fonction des informations que vous souhaitez modifier.

   Ou

   Cliquez sur **Enregistrer les modifications**.

### Finances {#finance}

1. Commencez à modifier une tâche comme décrit ci-dessus.
1. Cliquez sur **Finance**.

   ![edit_task_finance.png](assets/edit-task-finance-350x216.png)

1. Mettez à jour l’un des éléments suivants :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Type de coût</strong> </td> 
      <td> <p>Indiquez le Type de coût de la tâche à venir. Cela va déterminer comment le coût de la tâche est calculé, en fonction du nombre d'heures sur les tâches. </p> <p>Sélectionnez l’une des options suivantes :</p> 
       <ul> 
        <li> <p style="font-weight: normal;"><span>Aucun coût</span> </p> </li> 
        <li> <p style="font-weight: normal;"><span>Fixe Horaire</span> </p> </li> 
        <li> <p style="font-weight: normal;"><span>Heure de l’utilisateur</span> </p> </li> 
        <li> <p style="font-weight: normal;"><span>Heure du rôle</span> </p> </li> 
       </ul> <p>Pour plus d’informations sur le suivi des coûts, voir <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Suivi des coûts</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Type de revenu</strong> </td> 
      <td> <p>Indiquez le Type de revenu pour la tâche à venir. Cela va déterminer comment est calculé le chiffre d’affaires de la tâche, en fonction du nombre d’heures sur les tâches.</p> <p style="font-weight: normal;">Sélectionnez l’une des options suivantes : </p> 
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
       </ul> <p>Pour plus d’informations sur le suivi des recettes, voir <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Présentation de la facturation et des recettes</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Facultatif) Continuez à modifier les sections suivantes en fonction des informations que vous souhaitez modifier.

   Ou

   Cliquez sur **Enregistrer les modifications**.

### Paramètres {#settings}

1. Commencez à modifier une tâche comme décrit ci-dessus.
1. Cliquez sur **Paramètres**.

   ![](assets/edit-template-tasks-settings-classic-350x231.png)

1. Mettez à jour l’un des éléments suivants :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
   <tr> 
      <td role="rowheader"><p><b>Jalon</b></p></strong> </td> 
      <td> <p>Sélectionnez un jalon à associer à la tâche de modèle sélectionnée.</p>

   <p><b>IMPORTANT</b></p>
   <p>Vous devez associer un chemin de jalon à un modèle pour que ce champ s’affiche. Pour plus d’informations, voir <a href="../create-and-manage-templates/edit-templates.md">Modifier des modèles de projet</a>.</p> 
   </td> 
     </tr>
     <tr> 
      <td role="rowheader"><strong>Mode de suivi</strong> </td> 
      <td> <p>Indiquez le mode de suivi de l’état d’avancement de la tâche à venir. </p> <p>Sélectionnez l’une des options suivantes :</p> 
       <ul> 
        <li> <p><strong>L’utilisateur doit mettre à jour</strong> </p> </li> 
        <li> <p><strong>Utiliser l’heure</strong> </p> </li> 
        <li> <p><strong>Ignorer les avertissements tardifs</strong> </p> </li> 
        <li> <p><strong>Autocomplete</strong> </p> </li> 
        <li> <p><strong>Prédécesseur</strong> </p> </li> 
       </ul> <p>Pour plus d’informations sur le mode de suivi pour les tâches, voir <a href="../../../manage-work/tasks/task-information/task-tracking-mode.md" class="MCXref xref">Présentation du mode de suivi des tâches</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Processus d’approbation</strong> </td> 
      <td> <p>Sélectionnez le processus de validation que vous souhaitez associer à la tâche de modèle. Votre administrateur Workfront doit définir des processus d’approbation des tâches au niveau du système avant de pouvoir les associer à des tâches de modèle. <span>Un utilisateur disposant d’un accès administratif aux processus de validation peut également créer des processus de validation spécifiques à un groupe.</span> Pour plus d’informations sur la création de processus de validation, voir <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Créer un processus d’approbation pour les tâches</a>.</p> <p>Tenez compte des points suivants lors de l’ajout de processus de validation : </p> 
       <ul> 
       <li>Seuls les processus de validation actifs s'affichent dans la liste. </li> 
       <li> <p>Les processus de validation à l’échelle du système et spécifiques aux groupes s’affichent dans la liste. Les processus de validation associés à un groupe autre que celui du modèle ne s'affichent pas dans la liste.</p> <p>Important : Si le groupe associé au modèle change, le processus de validation spécifique au groupe devient un processus de validation à usage unique. Pour plus d’informations sur la façon dont les modifications apportées au groupe du projet ou au processus d’approbation affectent les paramètres d’approbation, voir <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">Comment les modifications du processus d’approbation et de groupe affectent-elles les processus d’approbation affectés ?</a>. </p> </li> 
       <li> <p>Si vous avez ajouté un processus d’approbation à usage unique, il s’affiche sous la forme "&lt;custom&gt;" dans ce champ. Pour plus d’informations, voir <a href="../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md" class="MCXref xref">Associer un processus d’approbation nouveau ou existant au travail</a>. </p> <!--<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this will be valid only for Classic when they edit the Edit Template box in NWE)</p>--> </li> 
       <li> <p>Lors de la modification en masse de tâches de modèle, les scénarios suivants existent :</p> 
       <ul> 
       <li> <p>Lorsque vous sélectionnez des tâches de modèle dans le même groupe de modèles, les processus de validation au niveau du système et du groupe s’affichent dans ce champ.</p> </li> 
       <li> <p>Lorsque vous sélectionnez des tâches de modèle dans différents groupes de modèles, seuls les processus de validation au niveau du système s’affichent dans ce champ.</p> </li> 
       <li> <p>Lorsque l’une des tâches du modèle est associée à un processus de validation à usage unique, il est remplacé par le niveau système. <span>ou processus d’approbation au niveau du groupe</span> vous sélectionnez . </p> </li> 
       </ul> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Notifications de rappel</strong> </td> 
      <td> <p>Sélectionnez les notifications de rappel que vous souhaitez joindre à la tâche de modèle. Elles seront jointes aux futures tâches du projet créé à partir de ce modèle. L’administrateur système doit configurer les notifications de rappel avant de pouvoir les sélectionner sur une tâche. Pour plus d’informations sur la configuration des notifications de rappel, voir <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">Configuration des notifications de rappel</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Facultatif) Continuez à modifier les sections suivantes en fonction des informations que vous souhaitez modifier.

   Ou

   Cliquez sur **Enregistrer les modifications**.

### Affectations {#assignments}

1. Commencez à modifier une tâche comme décrit ci-dessus.
1. Cliquez sur **Affectations**.

   ![assignment_edit_tasks.png](assets/assignments-edit-tasks-350x87.png)

1. Cliquez sur **Ajouter un cessionnaire** pour ajouter une nouvelle personne désignée à la tâche de modèle. Vous pouvez affecter des utilisateurs, des rôles ou des équipes à une tâche. Vous pouvez avoir plusieurs personnes désignées sur une tâche. Les tâches futures auront les mêmes ressources qui leur seront affectées lorsqu’elles seront créées à partir de cette tâche de modèle.
1. (Facultatif) Si vous avez plusieurs personnes désignées, sélectionnez la variable **Propriétaire** Bouton radio pour indiquer quel utilisateur ou rôle est considéré comme propriétaire de la tâche ou cessionnaire du Principal. Workfront marque le premier utilisateur ou rôle de tâche que vous affectez à une tâche de modèle en tant que propriétaire ou cessionnaire de Principal.
1. (Conditionnel et facultatif) Si votre contrainte de tâche est Basée sur le travail calculé ou l’effort, indiquez la variable **% d’affectation** (pourcentage d’attribution) pour chaque personne désignée. Il s’agit de la durée du planning de la personne désignée qu’elle peut consacrer à cette tâche. La modification du pourcentage d’affectation d’une personne désignée modifie les Heures planifiées d’une tâche.
1. (Conditionnel et facultatif) Si votre contrainte de tâche est simple, spécifiez la variable **Heures** de chaque cessionnaire

   Ou

   Indiquez le nombre total de **Heures planifiées** pour la tâche de modèle. Cela répartit le total des heures de manière égale entre tous les cessionnaires.

1. (Conditionnel et facultatif) Si votre contrainte de tâche est simple, spécifiez la variable **Durée** de la tâche de modèle en jours. Cela deviendra la durée de la tâche créée à partir de ce modèle.
1. (Facultatif) Sélectionnez un rôle dans le **Le rôle du cessionnaire** menu déroulant. Il s’agit du rôle que le cessionnaire peut remplir pour cette tâche future. Seuls les rôles de tâche associés à chaque personne désignée dans son profil s’affichent dans le menu déroulant.
1. (Facultatif) Continuez à modifier les sections suivantes en fonction des informations que vous souhaitez modifier.

   Ou

   Cliquez sur **Enregistrer les modifications**.

### Formulaires personnalisés {#custom-forms}

Vous pouvez définir des formulaires personnalisés par défaut à associer automatiquement aux tâches lorsque les tâches sont ajoutées à un projet. Pour plus d’informations sur la configuration du projet afin d’inclure des formulaires personnalisés de tâche par défaut, reportez-vous à la section &quot;Tâches&quot; de l’article . [Modification de projets](../../../manage-work/projects/manage-projects/edit-projects.md).

1. Commencez à modifier une tâche comme décrit ci-dessus. test
1. Cliquez sur **Forms personnalisée**.

   ![custom_forms_edit_task.png](assets/custom-forms-edit-task-350x136.png)

1. Sélectionnez le ou les formulaires personnalisés à associer à la tâche de modèle. Vous devez créer les formulaires personnalisés avant qu’ils ne soient disponibles pour la sélection dans ce champ. Seuls les formulaires personnalisés actifs s’affichent dans la liste. Pour plus d’informations sur la création de formulaires personnalisés, voir [Création ou modification d’un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md). Vous pouvez ajouter jusqu’à dix formulaires personnalisés à une tâche de modèle. Les formulaires sont automatiquement ajoutés aux tâches créées à partir du modèle.
1. (Conditionnel et facultatif) Si vous avez joint un formulaire personnalisé à la tâche de modèle, modifiez les champs du formulaire. Vous devez spécifier tous les champs requis avant de pouvoir enregistrer la tâche de modèle.

   >[!NOTE]
   >
   >Selon la manière dont votre administrateur Workfront définit les autorisations pour les sections de votre formulaire personnalisé, tout le monde ne peut pas afficher ou modifier les mêmes champs sur un formulaire personnalisé donné. Les autorisations de modification des champs d’une section d’un formulaire personnalisé dépendent des autorisations dont vous disposez sur la tâche de modèle ou la tâche à venir.\
   >Pour plus d’informations sur la définition des autorisations sur les sections d’un formulaire personnalisé, voir [Partage d’un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).\
   >Pour plus d’informations sur la définition des autorisations de tâche, voir [Partage d’une tâche](../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md).\
   >Pour plus d’informations sur la définition des autorisations de modèle, voir [Partager un modèle](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

1. (Facultatif) Continuez à modifier la section suivante, en fonction des informations que vous souhaitez modifier.

   Ou

   Cliquez sur **Enregistrer les modifications**.

### Commentaire {#comment}

1. Commencez à modifier une tâche comme décrit ci-dessus.
1. Cliquez sur **Commentaire**.

   ![comment_edit_task.png](assets/comment-edit-task-350x138.png)

1. Spécifiez un commentaire à afficher dans le flux de mises à jour de la tâche de modèle dans le champ disponible. Ce commentaire est visible pour toutes les personnes disposant de l’accès Affichage au modèle et à la tâche de modèle et ayant accès à l’affichage des notes.
1. Cliquez sur **Enregistrer les modifications**.

   Vos modifications seront envoyées pour cette tâche de modèle.

   Lorsque vous ou un autre utilisateur créez un projet à partir de ce modèle, tous les paramètres que vous avez appliqués aux tâches du modèle deviennent les paramètres des tâches du projet.
