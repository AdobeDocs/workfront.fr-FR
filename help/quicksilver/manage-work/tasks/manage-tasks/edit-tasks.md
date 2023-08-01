---
product-area: projects
navigation-topic: manage-tasks
title: Modifier les tâches
description: Vous pouvez modifier les informations sur les tâches que vous avez créées ou sur lesquelles vous disposez des autorisations de contribution ou de gestion.
author: Alina
feature: Work Management, Tasks
role: User
exl-id: 572c6008-3a67-47ae-8f5d-6b871ef1f37b
source-git-commit: 5b7a5aff0f8bdf7cf8429ac29b50c3beaf4bd3b4
workflow-type: tm+mt
source-wordcount: '3712'
ht-degree: 4%

---

# Modifier les tâches

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: some information in this area is repeated in the following articles. If you need to update a fied, update it in both:</p>
<p>** Task finances in details</p>
<p>** Task information in overview)</p>
</div>
-->


Vous pouvez modifier les informations sur les tâches que vous avez créées ou sur lesquelles vous disposez des autorisations de contribution ou de gestion.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Travail ou plus élevé</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux tâches et aux projets</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> 
    <ul> 
     <li> <p>Attribuez des autorisations à une tâche pour modifier les informations suivantes dans la zone Détails de la tâche : </p>
     <ul>
     <li>Description</li>
     <li>Statut</li>
     </ul>  
      </li> 
     <li> <p>Gérer les autorisations d’une tâche pour modifier toutes les informations dans la zone Détails et la zone Modifier la tâche</p> </li> 
    </ul> 
    <ul> 
     <li> <p>Attribuer ou des autorisations supérieures au projet</p> </li> 
    </ul> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Restrictions relatives à la modification des tâches

Certaines restrictions peuvent vous empêcher de modifier des tâches.

Tenez compte des points suivants lors de la modification des tâches :

* La mise à jour des tâches déclenche des notifications pour les projets dont l’état est En cours. Pour éviter toute confusion pour les utilisateurs affectés aux tâches, limitez autant que possible les tâches de modification lorsque le projet est à l’état En cours .
* Vous ne pouvez pas modifier les tâches qui se trouvent dans un processus d’approbation. Vous pouvez uniquement consigner l’heure ou mettre à jour l’état d’une tâche dans un processus d’approbation.

  ![](assets/edit-task-in-approval-process-nwe-350x148.png)

* Vous pouvez modifier et ajouter des documents aux tâches d’un projet dont l’état est Terminé, Mort ou En attente d’approbation n’est activé que lorsque votre administrateur Workfront ou un administrateur de groupe a activé cette fonctionnalité dans la zone Préférences du projet. Pour plus d’informations sur la définition des préférences de projet, voir [Configuration des préférences de projet à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* Vous pouvez toujours modifier les informations suivantes sur une tâche lorsque le projet a été marqué Terminé, Mort ou se trouve dans un processus d’approbation :

   * Enregistrer des heures
   * Modifier les dépenses existantes
   * Joindre un formulaire personnalisé

## Modifier une tâche dans une liste

Vous pouvez éditer les informations de la tâche dans une liste de tâches, en sélectionnant les champs d&#39;édition intégrés affichés dans la vue de la liste.

Pour plus d’informations sur la modification des tâches dans les listes, voir [Editer les tâches dans une liste](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

## Modifier une tâche dans une liste à l’aide du Résumé

Vous pouvez modifier une tâche dans une liste à l’aide du panneau Résumé. Pour plus d’informations sur la modification d’une tâche dans le panneau Résumé, reportez-vous à la section &quot;Modifier une tâche dans le résumé&quot; de la section [Editer les tâches dans une liste](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md) article.

## Modifier une tâche dans la zone Modifier la tâche

Vous pouvez modifier une tâche à l’aide des zones Modifier la tâche ou Détails de la tâche. Les étapes suivantes décrivent la modification d’une tâche dans la zone Modifier la tâche.

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront.

1. Cliquez sur **Projets**, puis cliquez sur le nom d’un projet pour l’ouvrir.
1. Cliquez sur **Tâche** dans le panneau de gauche.
1. Cliquez sur la tâche à modifier.
1. (Conditionnel) Pour modifier des informations limitées sur une tâche, cliquez sur **Détails de la tâche** dans le panneau de gauche.

   ![](assets/nwe-task-details-expanded-350x273.png)

   Tenez compte des informations de modification dans les zones suivantes de la section Détails de la tâche :

   * **Vue d’ensemble**

     Cette zone est développée par défaut.

   * **Formulaires personnalisés**

     Les noms des formulaires douaniers ne s’affichent que s’il existe des formulaires personnalisés associés à l’objet.

   * **Finances**

   >[!NOTE]
   >
   >Selon la manière dont votre administrateur Workfront ou votre administrateur de groupe a modifié votre modèle de mise en page, les champs de la zone Détails de la tâche peuvent être réorganisés ou non. Pour plus d’informations, voir [Personnalisation de la vue Détails à l’aide d’un modèle de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   Pour plus d’informations sur les champs visibles dans la section Détails de la tâche, continuez à modifier la tâche dans la zone Modifier la tâche comme décrit ci-dessous.

   Pour modifier les informations de la section Détails , procédez comme suit :

   1. (Facultatif) Cliquez sur le **Réduire tout** icon ![](assets/collapse-all-icon.png) dans le coin supérieur droit pour réduire toutes les zones.
   1. (Facultatif et conditionnel) Lorsqu’une zone est réduite, cliquez sur le bouton **flèche pointant vers la droite** ![](assets/right-pointing-arrow.png) en regard de chaque zone pour développer la zone à modifier.
   1. Pour plus d’informations sur la modification des informations dans l’onglet Détails de la tâche, voir les articles suivants :

      * [Gestion des informations sur la tâche dans la zone Présentation des détails de la tâche](../../../manage-work/tasks/manage-tasks/task-information-in-overview.md)
      * [Gérer les finances des tâches dans la section Détails de la tâche](../../../manage-work/tasks/manage-tasks/task-finances-in-details.md)

   1. (Facultatif) S’il n’existe aucun formulaire personnalisé associé à la tâche, commencez à saisir le nom d’un formulaire dans le champ **Ajouter un formulaire personnalisé** puis sélectionnez-la lorsqu’elle s’affiche dans la liste, puis cliquez sur **Enregistrer les modifications**.
   1. (Facultatif) Cliquez sur le **Exporter** icon ![](assets/export.png) pour exporter les informations d’aperçu et de formulaires personnalisés vers un fichier de PDF, cliquez sur **Exporter**. Sélectionnez l’une des options suivantes :

      * Sélectionner tout (s’affiche uniquement lorsqu’au moins un formulaire personnalisé est joint)
      * Vue d’ensemble
      * Nom d’un ou de plusieurs formulaires personnalisés

      Le fichier du PDF est téléchargé sur votre ordinateur.

      ![](assets/export-issue-details-selection-box-with-export-button-350x418.png)

      Pour plus d’informations, voir [Exportation de formulaires personnalisés et de détails d’objet](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md).

1. (Conditionnel) Pour modifier toutes les informations relatives à la tâche, en tant qu’utilisateur avec les autorisations Gérer pour la tâche, cliquez sur le bouton **Plus** menu ![](assets/more-icon.png) en regard du nom de la tâche, puis cliquez sur **Modifier**.

   Ou

   Dans une liste de tâches, sélectionnez une tâche, puis cliquez sur le bouton **Modifier** icon ![](assets/edit-icon.png) en haut de la liste.

   La boîte de dialogue Modifier la tâche s’ouvre.

   >[!IMPORTANT]
   >
   >Pour afficher l’option Modifier , vous devez disposer des autorisations Gérer pour la tâche.

   Tous les champs de tâche sont disponibles dans la zone Modifier la tâche et sont regroupés par zones répertoriées dans le panneau de gauche.

   >[!NOTE]
   >
   >Selon la manière dont votre administrateur Workfront ou votre administrateur de groupe a modifié votre modèle de mise en page, les champs de la zone Détails de la tâche peuvent être réorganisés ou non. Pour plus d’informations, voir [Personnalisation de la vue Détails à l’aide d’un modèle de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   Pensez à spécifier des informations dans l’une des sections suivantes :

   * [Nom de la tâche](#task-name)
   * [Vue d’ensemble](#overview)
   * [Affectations](#assignments)
   * [Formulaires personnalisés](#Custom%C2%A0F)
   * [Finances](#finance)
   * [Paramètres](#settings)

   >[!NOTE]
   >
   >Selon la manière dont votre administrateur Workfront ou votre administrateur de groupe configure le modèle de mise en page, les champs de la zone Modifier la tâche peuvent être réorganisés ou non. Pour plus d’informations, voir [Personnalisation de la vue Détails à l’aide d’un modèle de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

### Nom de la tâche {#task-name}

1. Commencez à modifier votre tâche comme décrit ci-dessus.
1. Cliquez sur **Task Name** dans le panneau de gauche.

   ![](assets/nwe-task-name-section-edit-task-box-350x122.png)

1. Mettez à jour le nom de la tâche.

1. Cliquez sur **Enregistrer** ou passez aux sections suivantes.

### Vue d’ensemble {#overview}

1. Commencez à modifier votre tâche comme décrit ci-dessus.
1. Cliquez sur **Présentation** dans le panneau de gauche.

   ![](assets/nwe-overview-section-edit-task-box-350x257.png)

1. Mettez à jour les informations suivantes sur la tâche :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Description</td> 
      <td>Ajoutez des informations supplémentaires sur la tâche. </td> 
     </tr> 
     <tr> 
      <td colspan="2" role="rowheader"><span style="font-weight: bold;">Section Informations de base</span> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Statut</td> 
      <td> <p>Sélectionnez l’état de la tâche qui indique à quel stade de développement se trouve la tâche.</p> <p><b>CONSEIL</b>

   Vous pouvez mettre à jour l’état de la tâche dans l’en-tête de la tâche. </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Priorité</td> 
      <td> <p>Il s’agit d’un indicateur visuel qui vous permet de hiérarchiser vos tâches. </p> <p>Sélectionnez l’une des options suivantes : </p> 
       <ul> 
      <li> <p> Aucun</p> </li> 
      <li> <p> Faible </p> </li> 
      <li> <p>Normal </p> </li> 
      <li> <p>Élevé </p> </li> 
      <li> <p> Urgent </p> </li> 
       </ul> <p>Selon les préférences du projet sélectionnées par votre administrateur Workfront, les noms des priorités peuvent être différents pour vous. Pour plus d’informations sur les priorités des tâches, voir <a href="../../../manage-work/tasks/task-information/task-priority.md" class="MCXref xref">Mise à jour de la priorité des tâches</a>. </p> </td> 
     </tr> 
     <tr> 
      <td colspan="2" role="rowheader"><span style="font-weight: bold;">Section Dates et contraintes de tâche</span> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Contrainte de tâche</td> 
      <td> <p>Déterminez quand la tâche doit être terminée en spécifiant une contrainte de tâche. </p> <p>Sélectionnez l’une des options suivantes : </p> 
       <ul> 
      <li> <p><span>Dates fixes</span> </p> <p>Spécifiez un <strong>Démarrage planifié</strong> et un <strong>Date d’achèvement prévue</strong>. </p> </li> 
      <li> <p><span>Il Faut Commencer Le</span> </p> <p>Spécifiez un <strong>Date de début planifiée</strong>. </p> </li> 
      <li> <p><span>Il Faut Finir Le</span> </p> <p>Spécifiez un <strong>Date d’achèvement prévue</strong>. </p> </li> 
       </ul> 
       <ul> 
      <li> <p><span>Dès que possible</span></p> </li> 
      <li> <p><span>Aussi tard que possible</span></p> </li> 
      <li> <p><span>Première Heure Disponible</span></p> </li> 
      <li> <p> <span>Dernière Heure Disponible</span></p> </li> 
      <li> <p><span>Commencer Au Plus Tard</span> </p> </li> 
      <li> <p>Définition d’une date de début planifiée</p> </li> 
      <li> <p><span>Commencer Au Plus Tôt</span> </p> <p>Spécifiez un <strong>Date de début planifiée</strong>. </p> </li> 
      <li> <p> Terminer <span>Pas Plus Tard Que</span></p> <p>Spécifiez un <strong>Date d’achèvement prévue</strong>. </p> </li> 
      <li> <p> Terminer <span>Pas Plus Tôt Que</span></p> <p>Spécifiez un <strong>Date d’achèvement prévue</strong></p> </li> 
       </ul> <p>Pour plus d’informations sur la contrainte de tâche, voir <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Présentation de la contrainte de tâche</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Date et heure de validation</td> 
      <td> <p>Il s’agit de la date à laquelle l’utilisateur affecté à la tâche s’engage à ce qu’elle soit terminée. Cette valeur peut différer de la date d’achèvement planifiée. Seuls les cessionnaires peuvent modifier ce champ. Pour plus d’informations sur les dates de validation dans Workfront, voir <a href="../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">Présentation de la date de validation</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Date et heure de début planifiées</td> 
      <td> <p>Date à laquelle la tâche est planifiée pour commencer. La date de début prévue d'une tâche est définie et influencée par un certain nombre de facteurs :</p> 
       <ul> 
      <li>Selon la préférence système pour la date de début prévue de la tâche, la date de début d’une nouvelle tâche sur un projet peut être, par défaut, aujourd’hui, ou la date de début du projet. <span>L’administrateur du groupe associé au projet peut également définir cette préférence pour le groupe.</span> Pour plus d’informations sur les préférences de tâche au niveau du système ou du groupe, voir <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md" class="MCXref xref">Configuration des préférences de tâche et de problème à l’échelle du système</a>.</li> 
      <li>Selon les prédécesseurs de la tâche, Workfront choisit la date de début prévue comme prochaine date disponible après la fin ou le début de la relation précédente. Pour plus d’informations sur les relations de prédécesseur, voir <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">Présentation des prédécesseurs de tâches</a>.</li> 
      <li>Le chef de projet ou le propriétaire de la tâche peut définir manuellement la date de début prévue lorsque la contrainte de tâche est Dates fixes ou Doit démarrer. Pour plus d’informations sur les contraintes de tâche, voir <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Présentation de la contrainte de tâche</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Date et heure d’achèvement prévues</td> 
      <td> <p>Date d’achèvement prévue, comme indiqué lors de la planification de la tâche. La date d’achèvement prévue peut être définie par plusieurs facteurs :</p> 
       <ul> 
      <li>La date d'achèvement prévue est calculée à partir de la date de début prévue en ajoutant la Durée de la tâche à la date de début prévue. Lorsque le chef de projet ou Workfront spécifie la durée de la tâche, cela déclenche une mise à jour de la date d’achèvement prévue. Si la date planifiée change, c’est souvent parce que la Durée de a été mise à jour.</li> 
      <li>Le chef de projet ou le propriétaire de la tâche peut définir manuellement la date d’achèvement prévue lorsque la contrainte de tâche est Dates fixes ou Doit se terminer. Pour plus d’informations sur les contraintes de tâche, voir <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Présentation de la contrainte de tâche</a>.</li> 
      <li>Si le Type de durée de la tâche change et que le nombre de ressources sur les tâches change en même temps, la date d’achèvement prévue change également. Pour plus d’informations sur les types de durée, voir <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Présentation de la durée et du type de durée de la tâche</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Date et heure de début réelles</td> 
      <td> <p>Spécifiez une Date de début réelle pour la tâche. La valeur par défaut est généralement renseignée automatiquement lorsque vous définissez l’état de la tâche sur En cours. La date de début réelle peut également être modifiée manuellement par le chef de projet ou le propriétaire de la tâche. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Date et heure d’achèvement réelles</td> 
      <td> <p>Indiquez la date et l’heure réelles auxquelles la tâche s’achève. La date et l’heure par défaut auxquelles une tâche est terminée correspondent toujours à l’heure réelle à laquelle le statut devient Terminé. La date d’achèvement réelle peut également être modifiée manuellement par le chef de projet ou le propriétaire de la tâche. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><b>Section de temps de travail</b></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Effort de travail </td> 
      <td>

   <p>La quantité d’effort requise pour terminer la tâche. Votre chef de projet peut décider d’utiliser ce champ au lieu des Heures planifiées pour estimer l’effort nécessaire pour terminer une tâche. Ce champ n’est visible que lorsque les conditions suivantes sont remplies :</p> 
      <ul> 
      <li> <p>La tâche a un type de durée simple. </p> <p><b>CONSEIL</b>

   Si vous modifiez le type de durée de la tâche, ce champ devient grisé. </p> </li>
   <li>Votre chef de projet a activé le champ Utiliser l’effort de travail pour calculer automatiquement les heures planifiées de la tâche sur le projet. </li> 
      </ul> 
      <p>Sélectionnez l’une des options suivantes :</p> 
      <ul> 
      <li>Petite</li> 
      <li>Volume moyen <span style="font-weight: normal;">(il s’agit de la valeur par défaut pour une nouvelle tâche)</span></li> 
      <li>Grande</li> 
      </ul> 
      <p><b>NOTE</b>

   La mise à jour de la quantité d’effort peut mettre à jour la tâche Heures prévues. La mise à jour est immédiate si le type de mise à jour du projet est automatique. Lorsque le type de mise à jour du projet est Manuel, vous devez recalculer la chronologie pour afficher les heures planifiées mises à jour. </p>

   <p>Pour plus d’informations sur l’utilisation de l’effort de travail au lieu des heures planifiées pour estimer l’effort de tâche, voir <a href="../../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Présentation de l’effort de travail</a>. </p> 
    </td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **Enregistrer** ou passez aux sections suivantes.

### Affectations {#assignments}

1. Commencez à modifier votre tâche comme décrit ci-dessus.
1. Cliquez sur **Affectations** dans le panneau de gauche.

   ![](assets/nwe-assignments-section-edit-task-box-350x217.png)

1. Cliquez sur **Recherche de personnes, de rôles et d’équipes** et commencez à saisir le nom d’un utilisateur, d’un rôle ou d’une équipe que vous souhaitez affecter à la tâche, puis cliquez dessus ou appuyez sur Entrée lorsqu’il s’affiche dans la liste.

   >[!NOTE]
   >
   >Si le nom de l’utilisateur contient un caractère spécial, vous devez l’inclure dans le champ de recherche.

   >[!TIP]
   >
   >Vous pouvez affecter plusieurs utilisateurs, rôles de tâche ou équipes. Vous ne pouvez affecter que des utilisateurs, des rôles de tâche et des équipes principaux.
   >
   >Si un utilisateur, un rôle de tâche ou une équipe a été affecté avant d’être désactivé, il reste attribué à l’élément de travail. Dans ce cas, nous vous recommandons ce qui suit :
   >
   >* Réaffectez l’élément de travail aux principales ressources.
   >* Associez les utilisateurs d’une équipe désactivée à une équipe principale et réaffectez la tâche à l’équipe principale.

1. (Facultatif) Indiquez si une personne désignée est la personne désignée Principale sur la tâche, en sélectionnant **Propriétaire** bouton radio en regard de leur nom. Une équipe ne peut pas être la Principale personne désignée d’une tâche.
1. (Conditionnel et facultatif) Mettez à jour les champs suivants :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Type de durée</td> 
      <td> <p>Cela identifie la relation entre les éléments suivants : </p> 
       <ul> 
      <li> <p>Nombre de ressources affectées à une tâche </p> </li> 
      <li> <p>L’effort total requis pour terminer la tâche </p> </li> 
      <li> <p> Durée totale de la tâche. </p> </li> 
       </ul> <p>Votre administrateur Workfront <span> ou un administrateur de groupe</span> sélectionne le paramètre Type de durée par défaut pour les tâches de votre système ou de votre groupe. Pour plus d’informations sur la définition des paramètres par défaut d’un projet, voir <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configuration des préférences de projet à l’échelle du système</a>. </p> <p>Les types de durée vous permettent de définir des affectations de ressources cohérentes en fonction des besoins de la tâche. Pour plus d’informations sur le type de durée d’une tâche, voir <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Présentation de la durée et du type de durée de la tâche</a>. </p> <p>Sélectionnez l’une des options suivantes : </p> 
       <ul> 
      <li> <p>Calcul d'affectation </p> </li> 
      <li> <p> Calcul de travail </p> </li> 
      <li> <p>Piloté par l'effort </p> </li> 
      <li> <p>Simple</p> </li> 
       </ul> </td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader">Durée par occurrence</td> 
      <td> <p>Cette option s’affiche uniquement sur le parent des tâches récurrentes. Il affiche la durée de chaque tâche récurrente, telle que définie lors de la création de la tâche. Pour plus d’informations sur la création de tâches récurrentes, voir <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Créer des tâches récurrentes</a>. </p> <p> <b>NOTE</b>

   Les durées modifiées dans des tâches récurrentes individuelles n’affichent pas la valeur indiquée dans ce champ. </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Durée</td> 
      <td> 
      <div> 
      <div> 
      <p>Il s’agit de la durée pendant laquelle vous laissez une tâche ouverte avant qu’elle ne soit terminée. </p> 
      <p><b>IMPORTANT</b>

   Comme la durée de la tâche correspond généralement au temps entre le début planifié et les dates de fin planifiées, elle affecte la chronologie du projet.</p>

   <p>Pour indiquer la Durée de la tâche et l’unité de temps, procédez comme suit :</p> 
      <ul> 
      <li> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Saisissez la durée et sélectionnez l’unité de temps disponible dans le menu déroulant.</p> <p><b>CONSEIL</b></p>
      Lorsque vous mettez à jour la Durée des tâches dans une liste de tâches, vous pouvez utiliser l’abréviation pour l’unité de temps. </p> </li> 
      </ul> 
      <p> Vous pouvez choisir parmi les options de temps normal ou de temps écoulé dans le tableau suivant : </p> 
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
      <td>h</td> 
      </tr> 
      <tr> 
      <td>Jours. Il s’agit du paramètre par défaut. </td> 
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
      <td>EM</td> 
      </tr> 
      <tr> 
      <td>Heures écoulées</td> 
      <td>EH</td> 
      </tr> 
      <tr> 
      <td>Jours écoulés</td> 
      <td>ED</td> 
      </tr> 
      <tr> 
      <td>Semaines écoulées</td> 
      <td>EW</td> 
      </tr> 
      <tr> 
      <td>Mois écoulés</td> 
      <td>ET</td> 
      </tr> 
      </tbody> 
   </table>

   <p><b>NOTE</b>

   <p>Le temps écoulé est une unité de temps pour la durée d’une tâche. Il s’agit de l’heure entre la date de début planifiée et la date de fin planifiée d’une tâche qui comprend les jours fériés, les week-ends et les heures de congé. En d'autres termes, le temps écoulé est le passage des jours calendaires.

   Le temps régulier prend en compte les jours fériés, les week-ends et les jours de congé et les exclut de la Durée de la tâche. Pour plus d’informations sur la durée de la tâche, voir <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Présentation de la durée et du type de durée de la tâche</a>. </p>
   </div> 
   </div> </td> 
   </tr> 
   <tr> 
   <td role="rowheader">Heures prévues</td> 
   <td> <p>Indiquez le nombre d’heures planifiées de la tâche, en heures. Il s’agit du temps réel nécessaire aux personnes désignées de la tâche pour l’exécuter. Vous ne pouvez spécifier le nombre d’heures planifiées pour une tâche que lorsque le type de durée est défini sur Attribution calculée. Pour plus d’informations sur les types de durée, voir <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Présentation de la durée et du type de durée de la tâche</a>.</p> 
   <b>NOTE</b>
   <p>
   Lors de la création de tâches récurrentes, les Heures planifiées sont celles de chaque occurrence. Les Heures planifiées des tâches parentes sont le total de toutes les Heures planifiées de toutes les occurrences. Pour plus d’informations sur la création de tâches récurrentes, voir <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Créer des tâches récurrentes</a>.
   </p>

   </td> 
   </tr> 
   <tr> 
   <td role="rowheader">Allocation</td> 
   <td> <p>Si la contrainte de tâche est calculée Travail ou Effort piloté, spécifiez la variable <strong>% d’affectation</strong> (pourcentage d’attribution) pour chaque personne désignée. Il s’agit de la durée du planning de la personne désignée qu’elle peut consacrer à cette tâche. La modification du pourcentage d’affectation d’une personne désignée modifie les Heures planifiées d’une tâche. </p> <p>Lorsque la contrainte de tâche est simple, vous pouvez spécifier les éléments suivants :</p> 
      <ul> 
      <li> <p>Heures d’affectation de chaque personne désignée.</p> </li> 
      <li> <p>Heures planifiées de la tâche</p> </li> 
      <li> <p>Durée de la tâche</p> </li> 
      </ul> </td> 
   </tr> 
   <tr> 
   <td role="rowheader">Rôle du cessionnaire</td> 
   <td> <p>Sélectionnez un rôle dans la <strong>Le rôle du cessionnaire</strong> menu déroulant lorsque vous avez sélectionné une personne comme personne désignée. Il s’agit du rôle que le cessionnaire peut remplir pour cette tâche. </p> <p><b>CONSEIL</b>

   Seuls les rôles de tâche associés à chaque personne désignée dans son profil s’affichent dans le menu déroulant.</p> </td>
   </tr> 
      </tbody> 
      </table>

1. Cliquez sur **Enregistrer** ou passez aux sections suivantes.

### Formulaires personnalisés

Vous pouvez définir des formulaires personnalisés par défaut à associer automatiquement aux tâches lorsque les tâches sont ajoutées à un projet. Pour plus d’informations sur la configuration du projet afin d’inclure des formulaires personnalisés de tâche par défaut pour toutes les nouvelles tâches, voir la section &quot;Tâches&quot; de l’article . [Modification de projets](../../../manage-work/projects/manage-projects/edit-projects.md).

1. Commencez à modifier la tâche comme décrit ci-dessus.
1. Cliquez sur **Forms personnalisée** dans le panneau de gauche, ou cliquez sur le nom d’un formulaire personnalisé s’il est déjà joint.

   ![](assets/nwe-custom-forms-section-edit-task-box-350x127.png)

1. Cliquez sur **Ajouter un formulaire personnalisé** et sélectionnez le ou les formulaires personnalisés à associer à la tâche. Vous devez créer les formulaires personnalisés avant qu’ils ne soient disponibles pour la sélection dans ce champ. Seuls les principaux formulaires personnalisés s’affichent dans la liste.

   Pour plus d’informations sur la création de formulaires personnalisés, voir [Création ou modification d’un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).Vous pouvez ajouter jusqu’à dix formulaires personnalisés à une tâche.

1. (Conditionnel) Si vous avez joint un formulaire personnalisé à la tâche, modifiez les champs du formulaire. Vous devez spécifier tous les champs requis avant de pouvoir enregistrer la tâche.

   >[!NOTE]
   >
   >Selon la manière dont votre administrateur Workfront définit les autorisations pour les sections de votre formulaire personnalisé, tout le monde ne peut pas afficher ou modifier les mêmes champs sur un formulaire personnalisé donné. Les autorisations de modification des champs d’une section d’un formulaire personnalisé dépendent des autorisations dont vous disposez sur la tâche elle-même. Pour plus d’informations sur la définition des autorisations de tâche, voir [Partage d’une tâche](../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md).

1. Cliquez sur **Enregistrer** ou passez aux sections suivantes.

### Finances {#finance}

1. Commencez à modifier votre tâche, comme décrit dans la section [Modifier les tâches](#Edit2) dans cet article.
1. Cliquez sur **Finance** dans le panneau de gauche.

   ![](assets/nwe-finance-section-edit-task-box-350x298.png)

1. Mettez à jour les champs suivants :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Type de coût</td> 
      <td> <p>Indiquez le Type de coût de la tâche. Cela va déterminer comment le coût de la tâche est calculé, en fonction du nombre d’heures sur les tâches. </p> <p>Sélectionnez l’une des options suivantes : </p> 
       <ul> 
        <li> <p>Aucun coût</p> </li> 
        <li> <p>Fixe par heure </p> </li> 
        <li> <p> Utilisateur, par heure </p> </li> 
        <li> <p> Rôle par heure</p> </li> 
       </ul> <p>Pour plus d’informations sur le suivi des coûts, voir <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Suivi des coûts</a> . Votre administrateur Workfront ou un administrateur de groupe sélectionne le paramètre Type de coût par défaut pour les tâches de votre système ou de votre groupe. Pour plus d’informations sur la définition des paramètres par défaut d’un projet, voir <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configuration des préférences de projet à l’échelle du système</a> .</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Type de revenus</td> 
      <td> <p>Indiquez le Type de revenu de la tâche. Cela va déterminer comment est calculé le chiffre d’affaires de la tâche, en fonction du nombre d’heures sur les tâches. </p> <p>Sélectionnez l’une des options suivantes : </p> 
       <ul> 
      <li> <p> Non facturable </p> </li> 
      <li> <p>Utilisateur, par heure </p> </li> 
      <li> <p>Rôle par heure </p> </li> 
      <li> <p>Fixe par heure </p> </li> 
      <li> <p>Utilisateur par heure avec plafond </p> </li> 
      <li> <p>Rôle par heure avec plafond </p> </li> 
      <li> <p>Utilisateur, par heure plus fixe </p> </li> 
      <li> <p>Rôle par heure plus fixe </p> </li> 
      <li> <p>Revenus fixes </p> </li> 
       </ul> <p>Pour plus d’informations sur le suivi des recettes, voir<a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Présentation de la facturation et des recettes</a> . </p> <p>L’administrateur ou l’administrateur de groupe Workfront sélectionne le paramètre Type de revenu par défaut pour les tâches de votre système ou de votre groupe. Pour plus d’informations sur la définition des paramètres par défaut d’un projet, voir <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configuration des préférences de projet à l’échelle du système</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **Enregistrer** ou passez à la section suivante.

### Paramètres {#settings}

1. Commencez à modifier votre tâche, comme décrit dans la section [Modifier les tâches](#Edit2) dans cet article.
1. Cliquez sur **Paramètres** dans le panneau de gauche.

   ![](assets/nwe-settings-section-edit-task-box-350x304.png)

1. Mettez à jour les champs suivants :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Mode de suivi</td> 
      <td> <p>Indiquez le mode de suivi de l’état d’avancement de la tâche. </p> <p>Sélectionnez l’une des options suivantes : </p> 
       <ul> 
      <li> <p> Utilisateur doit mettre à jour </p> </li> 
      <li> <p>Utiliser l’heure </p> </li> 
      <li> <p>Ignorer avertissements de retard</p> </li> 
      <li> <p> Autocomplete </p> </li> 
      <li> <p>Tâche antérieure </p> </li> 
       </ul> <p>Pour plus d’informations sur le mode de suivi pour les tâches, voir <a href="../../../manage-work/tasks/task-information/task-tracking-mode.md" class="MCXref xref">Présentation du mode de suivi des tâches</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nivellement des ressources</td> 
      <td> <p>Sélectionnez la variable <strong>Exclure du niveau de ressource</strong> champ si vous souhaitez que les ressources affectées à la tâche soient exclues du niveau.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Délai de nivellement</td> 
      <td> <p>Indiquez le délai de mise à niveau, en heures. </p> <p> Pour plus d’informations sur le nivellement des retards, voir <a href="../../../manage-work/tasks/task-information/task-leveling-delay.md" class="MCXref xref">Mettre à jour le délai de niveau de tâche</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Processus d'approbation</td> 
      <td> <p>Sélectionnez un processus de validation à associer à la tâche. Votre administrateur Workfront doit définir des processus d’approbation au niveau du système avant de pouvoir les associer à des tâches. Un utilisateur disposant d’un accès administratif aux processus de validation peut également créer des processus de validation spécifiques à un groupe. </p> <p>Pour plus d’informations sur la création de processus d’approbation, voir <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md">Créer un processus d’approbation pour les tâches</a>. Tenez compte des points suivants lors de l’ajout de processus de validation : </p> 
       <ul>

   <li> <p>Seuls les principaux processus de validation s'affichent dans la liste. </p> </li>

   <li> <p>Les processus de validation à l’échelle du système et spécifiques aux groupes s’affichent dans la liste. Un processus de validation associé à un groupe autre que celui du projet ne s’affiche pas dans la liste. </p>

   <p><b>IMPORTANT</b>

   Si le groupe du projet change, le processus d’approbation spécifique au groupe précédemment joint devient un processus d’approbation à usage unique. Pour plus d’informations sur la façon dont les modifications apportées au groupe du projet ou au processus d’approbation affectent les paramètres d’approbation, voir <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md">Comment les modifications du processus d’approbation et de groupe affectent-elles les processus d’approbation affectés ?</a>. </p>

   </li>

   <li> <p>Vous pouvez définir des processus de validation par défaut qui seront automatiquement associés à des tâches lors de leur ajout à un projet. Pour plus d’informations sur la configuration du projet afin d’inclure les processus d’approbation de tâche par défaut, voir la section "Tâches" de l’article . <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Modification de projets</a>. </p> </li>

   <li> <p>Lors de la modification en masse de tâches, les scénarios suivants se présentent : </p> 
      <ul> 
      <li> <p>Lorsque vous sélectionnez plusieurs tâches d’un même groupe, les processus de validation au niveau du système et du groupe s’affichent dans ce champ. </p> </li> 
      <li> <p>Lorsque vous sélectionnez plusieurs tâches issues de différents groupes, seuls les processus de validation au niveau du système s’affichent dans ce champ. </p> </li> 
      <li> <p>Lorsque l’une des tâches est associée à un processus de validation à usage unique, celui-ci est remplacé par le processus d’approbation au niveau du système ou du groupe que vous sélectionnez. </p> </li>

   </ul> </li> 
      </ul> </td> 
     </tr> 
    </tbody> 
   </table>
    </li>

1. Cliquer sur **Enregistrer**.

<!--notes from the table: <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this bullet stays here although the sections it might appear in are QS only, so we can use the snippet for both Qs and classic)</p>       -->

## Modifier une tâche dans l’en-tête de la tâche (limité)

Vous pouvez modifier une quantité limitée d’informations dans l’en-tête de la tâche.

Votre administrateur système ou groupe peut personnaliser les champs affichés dans l’en-tête de la tâche. Pour plus d’informations, voir [Personnalisation des en-têtes d’objet à l’aide d’un modèle de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).


![](assets/qs-task-header-without-approvals-and-with-dependecies-350x17.png)

Par défaut, les champs suivants sont inclus dans l’en-tête du projet :

* Nom de la tâche
* Pourcentage d’achèvement
* Affectations
* Date et heure d’achèvement prévues

  >[!CAUTION]
  >
  >Certaines contraintes de tâche et d’autres dépendances peuvent vous empêcher de modifier ce champ. Pour plus d’informations sur les contraintes de tâche, voir [Présentation de la contrainte de tâche](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

* Statut
* Prenez des décisions d’approbation si vous êtes défini comme approbateur dans un processus d’approbation actuel.

## Modifier les tâches en bloc

Vous pouvez modifier les tâches en bloc dans une liste et mettre à jour toutes leurs informations en même temps que vous choisissez d’enregistrer automatiquement les modifications que vous apportez aux tâches de la liste.

Pour plus d’informations sur l’enregistrement des tâches en bloc, reportez-vous à la section &quot;Modifier les tâches en bloc&quot; de l’article. [Editer les tâches dans une liste](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).
