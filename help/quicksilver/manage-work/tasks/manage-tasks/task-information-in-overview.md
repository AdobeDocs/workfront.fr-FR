---
product-area: projects
navigation-topic: manage-tasks
title: Gestion des informations sur la tâche dans la zone Présentation des détails de la tâche
description: Gestion des informations sur la tâche dans la zone Présentation des détails de la tâche
author: Alina
feature: Work Management
exl-id: 4980b28f-914d-4cf9-813f-14983aac660b
source-git-commit: 7e591a8eb801da463f05b574c091f68278974ad7
workflow-type: tm+mt
source-wordcount: '2072'
ht-degree: 5%

---

# Gestion des informations sur la tâche dans la zone Présentation des détails de la tâche

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: some of the information (fields) in this article is also in the Edit tasks article; if you need to update one field, do it in both articles)</p>
-->

Vous pouvez afficher ou modifier les informations d’une tâche en accédant à la zone Aperçu de la section Détails de la tâche . Il existe un nombre limité de champs que vous pouvez afficher ou modifier dans cette zone. Pour plus d’informations sur la modification de toutes les informations d’une tâche, voir [Modifier les tâches](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

Cet article décrit comment afficher ou modifier des informations dans la zone Aperçu des détails de la tâche. Pour plus d’informations sur la mise à jour d’autres zones de Détails de la tâche , voir les articles suivants :

* [Gérer les finances des tâches dans la section Détails de la tâche](../../../manage-work/tasks/manage-tasks/task-finances-in-details.md)
* [Ajout d’un formulaire personnalisé à un objet](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md)
* [Gestion des formulaires personnalisés associés à des objets](../../../workfront-basics/work-with-custom-forms/manage-custom-forms-attached-to-objects.md)

## Exigences d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <caption style="text-align: left;">
   *Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront. 
 </caption> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront<b> plan*</b> </p> </td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront<b> license*</b> </p> </td> 
   <td> <p>Travail ou plus élevé</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Paramétrages du niveau d'accès*</strong> </td> 
   <td> <p>Affichage ou accès supérieur à Projets et tâches</p> <p>Si vous disposez du niveau d’accès correct, mais que vous ne pouvez toujours pas modifier la section Détails de la tâche, demandez à votre Adobe Workfront s’il définit des restrictions supplémentaires dans votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Autorisations d’objet</strong> </p> </td> 
   <td> <p>Attribuer ou des autorisations supérieures au projet</p> <p>Afficher les autorisations pour la tâche pour afficher les informations dans la section Détails . </p> <p>Gérez les autorisations de mise à jour de la tâche dans la section Détails .</p> </td> 
  </tr> 
 </tbody> 
</table>

## Modifiez les informations de la tâche dans la section Présentation des détails de la tâche .

1. Accédez à une tâche que vous souhaitez afficher ou modifier.
1. Cliquez sur **Détails de la tâche** dans le panneau de gauche .
1. Accédez au **Présentation** pour afficher plus d’informations sur la tâche.

   Par défaut, l’ Aperçu est le premier champ de la section Détails de la tâche, et il est développé.

   >[!NOTE]
   >
   >Selon la manière dont votre administrateur Workfront ou votre administrateur de groupe configure notre modèle de mise en page, les champs de la section Détails de la tâche peuvent être réorganisés ou non. Pour plus d’informations, voir [Personnalisation de la vue Détails à l’aide d’un modèle de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

1. Cliquez sur le bouton **Modifier** icon ![](assets/edit-icon.png) dans le coin supérieur droit de la section Détails, puis cliquez sur **Présentation**.

   >[!TIP]
   >
   >Vous ne pouvez pas modifier des champs générés automatiquement par Workfront ou qui ne sont pas autorisés à être modifiés.

1. Modifiez n’importe quel champ disponible pour modification, en cliquant une seule fois sur le champ ou en cliquant sur **+Ajouter** pour ajouter des informations à un champ vide.
1. Affichez ou modifiez l’un des champs suivants répertoriés.

   Tous les champs ne sont pas modifiables.  

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Description</td> 
      <td> <p>Informations supplémentaires sur la tâche</p> </td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader">Numéro de référence</td> 
      <td>Il s’agit d’une valeur unique pour la tâche générée par Workfront pour tous les objets du système. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>Les utilisateurs disposant des autorisations Gérer pour une tâche peuvent spécifier un lien vers une page interne ou externe dans ce champ.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Statut</td> 
      <td> <p>Sélectionnez l’état de la tâche qui indique à quel stade de développement se trouve la tâche.</p> <p>Conseil : Vous pouvez mettre à jour l’état de la tâche dans l’en-tête de la tâche. </p> </td> 
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
     <tr> 
      <td role="rowheader">Durée</td> 
      <td> 
       <div> 
        <div> 
         <p>Il s’agit de la durée pendant laquelle vous laissez une tâche ouverte avant qu’elle ne soit terminée. </p> 
         <p>Important : Comme la durée de la tâche correspond généralement au temps entre le début planifié et les dates de fin planifiées, elle affecte la chronologie du projet.</p> 
         <p>Pour indiquer la Durée de la tâche et l’unité de temps, procédez comme suit :</p> 
         <ul> 
          <li> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Saisissez la durée et sélectionnez l’unité de temps disponible dans le menu déroulant.</p> </li> </ul>

   <p><strong>CONSEIL</strong></p> <p> Lorsque vous mettez à jour la Durée des tâches dans une liste de tâches, vous pouvez utiliser l’abréviation pour l’unité de temps. </p>      <p> Vous pouvez choisir parmi les options de temps normal ou de temps écoulé dans le tableau suivant : </p> 
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
            <td>Jours. Il s’agit de la valeur par défaut. </td> 
            <td>Dés</td> 
           </tr> 
           <tr> 
            <td>Semaines</td> 
            <td>M</td> 
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
         <p><strong>NOTE</strong> </p>
         <p> Le temps écoulé est une unité de temps pour la durée d’une tâche. Il s’agit de l’heure entre la date de début planifiée et la date de fin planifiée d’une tâche qui comprend les jours fériés, les week-ends et les heures de congé. En d'autres termes, le temps écoulé est le passage des jours calendaires. Le temps régulier prend en compte les jours fériés, les week-ends et les jours de congé et les exclut de la Durée de la tâche. Pour plus d’informations sur la durée de la tâche, voir <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Présentation de la durée et du type de durée de la tâche</a>. </p> 
         <p> 
         <!--You cannot specify the Duration of a task when the Duration Type of the task is Simple, or when the Task Constraint is Fixed Dates. (NOTE: Anna said this is now possible for all duration types in the Assignments area. It's not here, but to clear confusion, I am drafting this out of here.)--></p> 
        </div> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Durée prévisionnelle</td> 
      <td> <p>Différence en jours entre la date de début prévue et la date d’achèvement prévue. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Durée réelle</td> 
      <td> <p>Différence en jours entre la date de début réelle et la date de fin réelle. C'est le temps qu'il a fallu pour terminer le travail. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Heures planifiées</td> 
      <td> <p>Indiquez le nombre d’heures planifiées de la tâche, en heures. Il s’agit du temps réel nécessaire aux personnes désignées de la tâche pour l’exécuter. Vous ne pouvez spécifier le nombre d’heures planifiées pour une tâche que lorsque le type de durée est défini sur Attribution calculée. Pour plus d’informations sur les types de durée, voir <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Présentation de la durée et du type de durée de la tâche</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Heures effectives</td> 
      <td>Heures consignées par les utilisateurs sur la tâche. </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Effort de travail </td> 
      <td> 
       <div> 
        <p>La quantité d’effort requise pour terminer la tâche. Votre chef de projet peut décider d’utiliser ce champ au lieu des Heures planifiées pour estimer l’effort nécessaire pour terminer une tâche. Ce champ n’est visible que lorsque les conditions suivantes sont remplies :</p> 
        <ul> 
         <li> <p>La tâche a un type de durée simple. </p> <p>Conseil : Si vous modifiez le type de durée de la tâche, ce champ devient grisé. </p> </li> 
         <li>Votre chef de projet a activé le champ Utiliser l’effort de travail pour calculer automatiquement les heures planifiées de la tâche sur le projet. </li> 
        </ul> 
        <p>Sélectionnez l’une des options suivantes :</p> 
        <ul> 
         <li>Petite</li> 
         <li>Volume moyen <span style="font-weight: normal;">(il s’agit de la valeur par défaut d’une nouvelle tâche)</span></li> 
         <li>Grande</li> 
        </ul> 
        <p><strong>NOTE</strong></p> 
        <p> La mise à jour du volume d’effort peut mettre à jour la tâche Heures prévues. La mise à jour est immédiate si le type de mise à jour du projet est automatique. Lorsque le type de mise à jour du projet est Manuel, vous devez recalculer la chronologie pour afficher les heures planifiées mises à jour. </p> 
        <p>Pour plus d’informations sur l’utilisation de l’effort de travail au lieu des heures planifiées pour estimer l’effort de tâche, voir <a href="../../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Présentation de l’effort de travail</a>. </p> 
       </div> </td> 
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
      <td role="rowheader">Date de début prévue</td> 
      <td> <p>Date à laquelle la tâche est planifiée pour commencer. La date de début prévue d'une tâche est définie et influencée par un certain nombre de facteurs :</p> 
       <ul> 
        <li>Selon la préférence système pour la date de début prévue de la tâche, la date de début d’une nouvelle tâche sur un projet peut être, par défaut, aujourd’hui, ou la date de début du projet. <span>L’administrateur du groupe associé au projet peut également définir cette préférence pour le groupe.</span> Pour plus d’informations sur les préférences de tâche au niveau du système ou du groupe, voir <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md" class="MCXref xref">Configuration des préférences de tâche et de problème à l’échelle du système</a>.</li> 
        <li>Selon les prédécesseurs de la tâche, Workfront choisit la date de début prévue comme prochaine date disponible après la fin ou le début de la relation précédente. Pour plus d’informations sur les relations de prédécesseur, voir <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">Présentation des prédécesseurs de tâches</a>.</li> 
        <li>Le chef de projet ou le propriétaire de la tâche peut définir manuellement la date de début prévue lorsque la contrainte de tâche est Dates fixes ou Doit démarrer. Pour plus d’informations sur les contraintes de tâche, voir <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Présentation de la contrainte de tâche</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Date de début prévisionnelle</td> 
      <td> <p>Date "réelle" du début de la tâche en fonction de l’état d’avancement et de l’achèvement des tâches précédentes. Il s’agit d’un champ calculé que vous ne pouvez pas modifier manuellement.</p> <p> La date de début prévue et la date de début prévue commencent par être les mêmes, lorsqu’un projet est planifié pour la première fois. La date de début prévue peut s’éloigner du début prévu, si le projet évolue et que la tâche n’est pas encore lancée. Pour plus d’informations sur les dates de début prévues, voir <a href="../../../manage-work/projects/planning-a-project/project-projected-start-date.md" class="MCXref xref">Présentation du projet Date de début prévue</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Date de début réelle</td> 
      <td> <p>Spécifiez une Date de début réelle pour la tâche. La valeur par défaut est généralement renseignée automatiquement lorsque vous définissez l’état de la tâche sur En cours. La date de début réelle peut également être modifiée manuellement par le chef de projet ou le propriétaire de la tâche. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Date d’achèvement prévue</td> 
      <td> <p>Date d’achèvement prévue, comme indiqué lors de la planification de la tâche. La date d’achèvement prévue peut être définie par plusieurs facteurs :</p> 
       <ul> 
        <li>La date d'achèvement prévue est calculée à partir de la date de début prévue en ajoutant la Durée de la tâche à la date de début prévue. Lorsque le chef de projet ou Workfront spécifie la durée de la tâche, cela déclenche une mise à jour de la date d’achèvement prévue. Si la date planifiée change, c’est souvent parce que la Durée de a été mise à jour.</li> 
        <li>Le chef de projet ou le propriétaire de la tâche peut définir manuellement la date d’achèvement prévue lorsque la contrainte de tâche est Dates fixes ou Doit se terminer. Pour plus d’informations sur les contraintes de tâche, voir <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Présentation de la contrainte de tâche</a>.</li> 
        <li>Si le Type de durée de la tâche change et que le nombre de ressources sur les tâches change en même temps, la date d’achèvement prévue change également. Pour plus d’informations sur les types de durée, voir <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Présentation de la durée et du type de durée de la tâche</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Date d'achèvement prévisionnelle</td> 
      <td> <p>Date "réelle" du moment où la tâche doit être terminée en fonction de l’état d’avancement des tâches précédentes et des mises à jour de l’état d’avancement de la tâche par la personne désignée. Il s’agit d’un champ calculé que vous ne pouvez pas modifier manuellement.</p> <p> La date d’achèvement prévue et la date d’achèvement prévue commencent par être la même, lorsqu’un projet est planifié pour la première fois. La date d’achèvement prévue peut s’éloigner de la fin planifiée, si le projet évolue et que la tâche n’est pas encore lancée. Pour plus d’informations sur les dates de fin prévues, voir <a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">Présentation de la date d’achèvement prévue pour les projets, tâches et problèmes</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Date d’achèvement réelle</td> 
      <td> <p>Spécifiez la date et l’heure réelles auxquelles la tâche se termine. La date et l’heure par défaut auxquelles une tâche est terminée correspondent toujours à l’heure réelle à laquelle le statut devient Terminé. La date d’achèvement réelle peut également être modifiée manuellement par le chef de projet ou le propriétaire de la tâche. </p> </td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader">Date d'engagement</td> 
      <td> <p>Il s’agit de la date à laquelle l’utilisateur affecté à la tâche s’engage à ce qu’elle soit terminée. Cette valeur peut différer de la date d’achèvement planifiée. Seuls les cessionnaires peuvent modifier ce champ. Pour plus d’informations sur les dates de validation dans Workfront, voir <a href="../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">Présentation de la date de validation</a>.</p> </td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader">Date d’entrée</td> 
      <td>Date à laquelle la tâche a été créée.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Entré par</td> 
      <td>Personne qui a créé la tâche.</td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader">Date de dernière mise à jour</td> 
      <td> <p>Date de la dernière mise à jour de la tâche. </p> <p>Conseil : Workfront enregistre une date de mise à jour chaque fois qu’une personne modifie et enregistre une tâche.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dernière mise à jour par</td> 
      <td> <p>Personne qui a mis la tâche à jour pour la dernière fois.</p> </td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader">Fréquence de récurrence</td> 
      <td> <p>Cette option s’affiche uniquement sur le parent des tâches récurrentes. Il s’agit de la fréquence à laquelle les tâches de la périodicité se produisent. Pour plus d’informations sur la création de tâches récurrentes, voir <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Créer des tâches récurrentes</a>. </p> </td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader">Durée par occurrence</td> 
      <td> <p>Cette option s’affiche uniquement sur le parent des tâches récurrentes. Il affiche la durée de chaque tâche récurrente. Pour plus d’informations sur la création de tâches récurrentes, voir <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Créer des tâches récurrentes</a>. </p> <p><strong>NOTE</strong></p> <p> Les durées modifiées dans des tâches récurrentes individuelles n’affichent pas la valeur indiquée dans ce champ. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted, to keep it focused JUST on the Overview section and not others.) </p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Custom Forms</strong> to add or forms or edit information on the existing custom forms.&nbsp;</p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Expand any of the existing custom forms to edit them, or start typing in the <strong>Add custom form</strong> box in the upper-right corner to add a new form. </p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about adding or editing custom forms, see the following articles:</p>
   -->

   <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md" class="MCXref xref">Add a custom form to an object</a> </li>   
     -->

   <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="../../../workfront-basics/work-with-custom-forms/manage-custom-forms-attached-to-objects.md" class="MCXref xref">Manage custom forms attached to objects</a> </li>   
     -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Click&nbsp;<strong>Finance</strong>, then <strong>Edit Finance</strong> to view or edit financial information for the task. </p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Expand the <strong>Finance</strong> area in the Details section, then double-click any editable field to update it. </p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about editing financial information for a task, see <a href="../../../manage-work/tasks/manage-tasks/task-finances-in-details.md" class="MCXref xref">Manage task finances in the Task Details section</a>. </p>
   -->

1. Cliquez sur **Enregistrer les modifications**.
