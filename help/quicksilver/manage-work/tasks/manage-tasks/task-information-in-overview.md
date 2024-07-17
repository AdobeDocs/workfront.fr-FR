---
product-area: projects
navigation-topic: manage-tasks
title: Gérer les informations des tâches dans la zone Vue d’ensemble des détails de la tâche
description: Gérer les informations des tâches dans la zone Vue d’ensemble des détails de la tâche
author: Alina
feature: Work Management
exl-id: 4980b28f-914d-4cf9-813f-14983aac660b
source-git-commit: 5b7a5aff0f8bdf7cf8429ac29b50c3beaf4bd3b4
workflow-type: tm+mt
source-wordcount: '2089'
ht-degree: 64%

---

# Gérer les informations des tâches dans la zone Vue d’ensemble des détails de la tâche

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: some of the information (fields) in this article is also in the Edit tasks article; if you need to update one field, do it in both articles)</p>
-->

Vous pouvez afficher ou modifier les informations d’une tâche en accédant à la zone Aperçu de la section Détails de la tâche . Il existe un nombre limité de champs que vous pouvez afficher ou modifier dans cette zone. Pour plus d&#39;informations sur la modification de toutes les informations d&#39;une tâche, voir [Modifier les tâches](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

Cet article décrit comment afficher ou modifier des informations dans la zone Aperçu des détails de la tâche. Pour plus d’informations sur la mise à jour d’autres zones de Détails de la tâche , voir les articles suivants :

* [Gérer les finances des tâches dans la section Détails de la tâche](../../../manage-work/tasks/manage-tasks/task-finances-in-details.md)
* [Ajouter un formulaire personnalisé à un objet](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md)
* [Gérer les formulaires personnalisés attachés aux objets](../../../workfront-basics/work-with-custom-forms/manage-custom-forms-attached-to-objects.md)

## Conditions d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <caption style="text-align: left;">
   * Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront. 
 </caption> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Plan Adobe Workfront<b>*</b> </p> </td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront<b> license*</b> </p> </td> 
   <td> <p>Travail ou supérieure</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Configurations des niveaux d’accès*</strong> </td> 
   <td> <p>Affichage ou accès supérieur à Projets et tâches</p> <p>Si vous disposez du niveau d’accès correct, mais que vous ne pouvez toujours pas modifier la section Détails de la tâche, demandez à votre Adobe Workfront s’il définit des restrictions supplémentaires dans votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice de Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Autorisations d’objets</strong> </p> </td> 
   <td> <p>Autorisations Contribute ou supérieures pour le projet</p> <p>Afficher les autorisations pour la tâche pour afficher les informations dans la section Détails . </p> 
   <p>Autorisations Contribute pour la tâche de mettre à jour les informations suivantes dans la section Détails :</p>

<ul>
   <li>Description</li>
   <li>Statut</li>
   </ul>

<p>Gérez les autorisations pour que la tâche mette à jour toutes les informations dans la section Détails .</p> </td> 
  </tr> 
 </tbody> 
</table>

## Modifiez les informations de la tâche dans la section Présentation des détails de la tâche .

1. Accédez à une tâche que vous souhaitez afficher ou modifier.
1. Cliquez sur **Détails de la tâche** dans le panneau de gauche .
1. Accédez à la zone **Overview** pour afficher plus d’informations sur la tâche.

   Par défaut, l’ Aperçu est le premier champ de la section Détails de la tâche, et il est développé.

   >[!NOTE]
   >
   >Selon la manière dont votre administrateur Workfront ou votre administrateur de groupe configure notre modèle de mise en page, les champs de la section Détails de la tâche peuvent être réorganisés ou non. Pour plus d’informations, voir [Personnaliser la vue Détails à l’aide d’un modèle de disposition](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

1. Cliquez sur l’icône **Modifier** ![](assets/edit-icon.png) dans le coin supérieur droit de la section Détails, puis cliquez sur **Aperçu**.

   >[!TIP]
   >
   >Vous ne pouvez pas modifier des champs générés automatiquement par Workfront ou qui ne sont pas autorisés à être modifiés.

1. Modifiez n’importe quel champ disponible pour modification, en cliquant une seule fois sur le champ ou en cliquant sur **+Ajouter** pour ajouter des informations à un champ vide.
1. Affichez ou modifiez les champs suivants répertoriés.

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
      <td> <p>Sélectionnez le statut de la tâche qui indique à quelle étape de développement se trouve la tâche.</p> <p>Conseil : Vous pouvez mettre à jour l’état de la tâche dans l’en-tête de la tâche. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Priorité</td> 
      <td> <p>Il s’agit d’un indicateur visuel qui vous permet de hiérarchiser vos tâches. </p> <p>Sélectionnez l’une des options suivantes : </p> 
       <ul> 
        <li> <p> Aucun</p> </li> 
        <li> <p> Faible </p> </li> 
        <li> <p>Normal </p> </li> 
        <li> <p>Élevé </p> </li> 
        <li> <p> Urgent </p> </li> 
       </ul> <p>Selon les préférences du projet sélectionnées par votre administrateur ou administratrice Workfront, les noms des priorités peuvent être différents pour vous. Pour plus d’informations sur les priorités des tâches, voir <a href="../../../manage-work/tasks/task-information/task-priority.md" class="MCXref xref">Mettre à jour la priorité des tâches</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Type de durée</td> 
      <td> <p>Permet d’identifier la relation entre les éléments suivants : </p> 
       <ul> 
        <li> <p>Le nombre de ressources affectées à une tâche. </p> </li> 
        <li> <p>L’effort total nécessaire à la réalisation de la tâche. </p> </li> 
        <li> <p> La durée totale de la tâche. </p> </li> 
       </ul> <p>Votre administrateur ou administratrice de Workfront <span> ou de groupe</span> sélectionne le paramètre Type de durée par défaut pour les tâches de votre système ou de votre groupe. Pour plus d’informations sur la définition des paramètres par défaut d’un projet, consultez la section <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurer les préférences des projets à l’échelle du système</a>. </p> <p>Les types de durée vous permettent de définir des affectations de ressources cohérentes en fonction des besoins de la tâche. Pour plus d’informations sur le type de durée d’une tâche, consultez la section <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Vue d’ensemble de la durée et du type de durée des tâches</a>. </p> <p>Sélectionnez l’une des options suivantes : </p> 
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
         <p>Il s’agit de la durée pendant laquelle vous laissez une tâche en cours avant qu’elle ne soit terminée. </p> 
         <p>Important : Comme la durée de la tâche correspond généralement au temps entre le début planifié et les dates de fin planifiées, elle affecte la chronologie du projet.</p> 
         <p>Pour indiquer la durée de la tâche et l’unité de temps, procédez comme suit :</p> 
         <ul> 
          <li> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Saisissez la durée et sélectionnez une unité de temps dans le menu déroulant.</p> </li> </ul>

   <p><strong>CONSEIL</strong></p> <p> Lorsque vous mettez à jour la durée des tâches dans une liste de tâches, vous pouvez utiliser l’abréviation pour l’unité de temps. </p>      <p> Vous pouvez choisir parmi les options de temps normal ou de temps écoulé dans le tableau suivant : </p> 
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
            <td>JoursIl s’agit du paramètre par défaut. </td> 
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
         <p> Le temps écoulé est une unité de temps pour la durée d’une tâche. Il s’agit de l’heure entre la date de début prévue et la date d’achèvement prévue d’une tâche qui comprend les jours fériés, les week-ends et les congés. En d'autres termes, le temps écoulé est le passage des jours calendaires. Le temps régulier prend en compte les jours fériés, les week-ends et les congés et les exclut de la durée de la tâche. Pour plus d’informations sur la durée de la tâche, voir <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Vue d’ensemble de la durée et du type de durée de la tâche</a>. </p> 
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
      <td> <p>Indiquez le nombre d’heures prévues de la tâche. Il s’agit du temps effectif nécessaire aux personnes assignées à la tâche pour l’achever. Vous ne pouvez spécifier le nombre d’heures prévues pour une tâche que lorsque le type de durée est défini sur Calcul d’affectation. Pour plus d’informations sur les types de durée, voir <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Vue d’ensemble de la durée ou du type de durée des tâches</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Heures effectives</td> 
      <td>Heures consignées par les utilisateurs sur la tâche. </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Effort de travail </td> 
      <td> 
       <div> 
        <p>Quantité d’effort requise pour terminer la tâche. La personne en charge du projet peut décider d’utiliser ce champ au lieu du nombre d’heures prévues pour estimer l’effort nécessaire pour terminer une tâche. Ce champ n’est visible que lorsque les conditions suivantes sont remplies :</p> 
        <ul> 
         <li> <p>La tâche a un type de durée simple. </p> <p>Conseil : Si vous modifiez le type de durée de la tâche, ce champ devient grisé. </p> </li> 
         <li>La personne en charge du projet a activé le champ Effort de travail pour calculer automatiquement le champ Nombre d’heures prévues detâche du projet. </li> 
        </ul> 
        <p>Sélectionnez l’une des options suivantes :</p> 
        <ul> 
         <li>Petite</li> 
         <li>Moyenne <span style="font-weight: normal;">(il s’agit de la valeur par défaut pour une nouvelle tâche)</span></li> 
         <li>Grande</li> 
        </ul> 
        <p><strong>NOTE</strong></p> 
        <p> La mise à jour de la quantité d’effort peut mettre à jour le nombre d’heures prévues de la tâche. La mise à jour est immédiate si le type de mise à jour du projet est automatique. Lorsque le type de mise à jour du projet est Manuel, vous devez recalculer la chronologie pour afficher le nombre d’heures prévues mis à jour. </p> 
        <p>Pour plus d’informations sur l’utilisation de l’effort de travail au lieu du nombre d’heures prévues pour estimer l’effort de tâche, voir <a href="../../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Vue d’ensemble de l’effort de travail</a>. </p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Contrainte de tâche</td> 
      <td> <p>Déterminez quand la tâche doit être terminée en spécifiant une contrainte de tâche. </p> <p>Sélectionnez l’une des options suivantes : </p> 
       <ul> 
        <li> <p><span>Dates fixes</span> </p> <p>Indiquez un <strong>Démarrage prévu</strong> et une <strong>date d’achèvement prévue</strong>. </p> </li> 
        <li> <p><span>Doit commencer le</span> </p> <p>Indiquez une <strong>date de début prévue</strong>. </p> </li> 
        <li> <p><span>Doi se terminer le</span> </p> <p>INdiquez une <strong>date d’achèvement prévue</strong>. </p> </li> 
       </ul> 
       <ul> 
        <li> <p><span>Le plus tôt possible</span></p> </li> 
        <li> <p><span>Le plus tard possible</span></p> </li> 
        <li> <p><span>Première Heure Disponible</span></p> </li> 
        <li> <p> <span>Dernière heure disponible</span></p> </li> 
        <li> <p><span>Commencer au plus tard le</span> </p> </li> 
        <li> <p>Indiquer une date de début prévue</p> </li> 
        <li> <p><span>Commencer au plus tôt le</span> </p> <p>Indiquez une <strong>date de début prévue</strong>. </p> </li> 
        <li> <p> Finir <span>au plus tard le</span></p> <p>Indiquez une <strong>date d’achèvement prévue</strong>. </p> </li> 
        <li> <p> Finir <span>au plus tôt le</span></p> <p>Indiquer une <strong>date d’achèvement prévue</strong></p> </li> 
       </ul> <p>Pour plus d’informations sur la contrainte de tâche, voir <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Vue d’ensemble de la contrainte de tâche</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Date de début prévue</td> 
      <td> <p>Date à laquelle le début de la tâche est prévu. La date de début prévue d’une tâche est définie et influencée par un certain nombre de facteurs :</p> 
       <ul> 
        <li>Selon la préférence système pour la date de début prévue de la tâche, la date de début d’une nouvelle tâche d’un projet peut être la date du jour, ou la date de début du projet, par défaut. <span>L’équipe d’administration du groupe associé au projet peut également définir cette préférence pour le groupe.</span> Pour plus d’informations sur les préférences de tâche au niveau du système ou du groupe, voir <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md" class="MCXref xref">Configuration des préférences de tâche et de problème à l’échelle du système</a>.</li> 
        <li>Selon les prédécesseurs de la tâche, Workfront choisit la date de début prévue comme prochaine date disponible après la fin ou le début des prédécesseurs ou selon la relation entre les prédecesseurs. Pour plus d’informations sur les relations entre les prédécesseurs, voir <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">Vue d’ensemble des prédécesseurs de tâches</a>.</li> 
        <li>La personne en charge du projet ou propriétaire de la tâche peut définir manuellement la date de début prévue lorsque la contrainte de tâche est Dates fixes ou Doit commencer le. Pour plus d’informations sur les contraintes de tâche, voir <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Vue d’ensemble de la contrainte de tâche</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Date de début prévisionnelle</td> 
      <td> <p>Date "réelle" du début de la tâche en fonction de l’état d’avancement et de l’achèvement des tâches précédentes. Il s’agit d’un champ calculé que vous ne pouvez pas modifier manuellement.</p> <p> La date de début prévue et la date de début prévue commencent par être les mêmes, lorsqu’un projet est planifié pour la première fois. La date de début prévue peut s’éloigner du début prévu, si le projet évolue et que la tâche n’est pas encore lancée. Pour plus d’informations sur les dates de début prévues, voir <a href="../../../manage-work/projects/planning-a-project/project-projected-start-date.md" class="MCXref xref">Présentation de la date de début prévue du projet</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Date de début réelle</td> 
      <td> <p>Indiquez une date de début effective de la tâche. La valeur par défaut est généralement renseignée automatiquement lorsque vous définissez le statut de la tâche sur En cours. La date de début effective peut également être modifiée manuellement par la personne en charge du projet ou propriétaire de la tâche. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Date d’achèvement prévue</td> 
      <td> <p>Date d’achèvement anticipée, comme indiqué lors de la planification de la tâche. La date d’achèvement prévue peut être définie par plusieurs facteurs :</p> 
       <ul> 
        <li>La date d’achèvement prévue est calculée à partir de la date de début prévue en ajoutant la durée de la tâche à la date de début prévue. Lorsque la personne en charge du projet ou Workfront spécifie la durée de la tâche, cela déclenche une mise à jour de la date d’achèvement prévue. Si la date prévue change, c’est souvent parce que la durée a été mise à jour.</li> 
        <li>La personne en charge du projet ou propriétaire de la tâche peut définir manuellement la date d’achèvement prévue lorsque la contrainte de tâche est Dates fixes ou Doit se terminele. Pour plus d’informations sur les contraintes de tâche, voir <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Vue d’ensemble de la contrainte de tâche</a>.</li> 
        <li>Si le type de durée de la tâche et que le nombre de ressources sur les tâches changent en même temps, la date d’achèvement prévue change également. Pour plus d’informations sur les types de durée, voir <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Vue d’ensemble de la durée et du type de durée des tâches</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Date d'achèvement prévisionnelle</td> 
      <td> <p>Date "réelle" du moment où la tâche doit être terminée en fonction de l’état d’avancement des tâches précédentes et des mises à jour de l’état d’avancement de la tâche par la personne désignée. Il s’agit d’un champ calculé que vous ne pouvez pas modifier manuellement.</p> <p> La date d’achèvement prévue et la date d’achèvement prévue commencent par être la même, lorsqu’un projet est planifié pour la première fois. La date d’achèvement prévue peut s’éloigner de la fin planifiée, si le projet évolue et que la tâche n’est pas encore lancée. Pour plus d’informations sur les dates d’achèvement prévues, voir <a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">Présentation de la date d’achèvement prévue pour les projets, les tâches et les problèmes</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Date d’achèvement réelle</td> 
      <td> <p>Indiquez la date et l’heure effectives auxquelles la tâche s’achève. La date et l’heure par défaut auxquelles une tâche est terminée correspondent toujours à l’heure effective à laquelle le statut devient Terminé. La date d’achèvement effective peut également être modifiée manuellement par la personne en charge du projet ou propriétaire de la tâche. </p> </td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader">Date d'engagement</td> 
      <td> <p>Il s’agit de la date à laquelle la personne affectée à la tâche s’engage à la terminer. Cette valeur peut différer de la date d’achèvement prévue. Seules les personnes assignées peuvent modifier ce champ. Pour plus d’informations sur les dates d’engagement, consultez <a href="../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">Vue d’ensemble de la date d’engagement</a>.</p> </td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader">Date d’entrée</td> 
      <td>Date de création de la tâche.</td> 
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
