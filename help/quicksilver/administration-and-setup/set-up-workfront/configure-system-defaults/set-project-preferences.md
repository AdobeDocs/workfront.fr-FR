---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Configuration des préférences du projet à l’échelle du système
description: En tant que personne membre de l’administration  [!DNL Adobe Workfront] , vous pouvez configurer les préférences par défaut pour tous les projets créés dans l’ensemble du système. Ces préférences ont un impact sur le comportement du projet, de la tâche et du problème.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 1a1affed-1b06-442c-98b2-9f360eee767b
source-git-commit: caaba90f4cdd835e1a1fddf16bcefa30995cca0d
workflow-type: tm+mt
source-wordcount: '2539'
ht-degree: 96%

---

# Configurer les préférences du projet à l’échelle du système

<!--Audited: 12/2023-->

En tant que personne membre de l’administration [!DNL Adobe Workfront], vous pouvez configurer les préférences par défaut pour tous les projets créés dans l’ensemble du système. Ces préférences ont un impact sur le comportement du projet, de la tâche et du problème.

>[!NOTE]
>
>Par défaut, ces préférences sont verrouillées et les administrateurs et administratrices de groupes ne peuvent pas les modifier au niveau du groupe, sauf si vous les déverrouillez pour tous les groupes du système. Pour plus d’informations, consultez la section [Verrouiller ou déverrouiller des préférences de projet pour tous les groupes du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>[!DNL Adobe Workfront] plan</p></td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td><p>Nouvelle : [!UICONTROL Standard]</p>
   Ou
   <p>Actuelle : [!UICONTROL Plan]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurer des préférences de projet pour l’ensemble de l’entreprise

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **[!UICONTROL Préférences du projet]** > **[!UICONTROL Projets]**.

1. Sur la page des **préférences du projet**, continuez avec l’une des 4 sections répertoriées ci-dessous pour configurer les préférences des [!UICONTROL Statuts du projet], [!UICONTROL Chronologies], [!UICONTROL Business cases], et [!UICONTROL Reprises après une période d’inactivité].
1. Si vous souhaitez que tous les groupes de l’organisation utilisent les mêmes préférences de projet, assurez-vous que chaque préférence soit verrouillée ![](assets/lock-toggle-button.png) (il s’agit de la valeur par défaut).

   >[!IMPORTANT]
   >
   >Lorsqu’une préférence de projet est verrouillée, toutes les modifications que vous apportez à cette préférence sont héritées par tous les groupes du système. Il est important de communiquer avec les utilisateurs et les utilisatrices et les groupes de votre organisation pour vous assurer que tous les besoins sont pris en compte dans la configuration des préférences du projet.

   Pour plus d’informations sur le déverrouillage d’une préférence afin que tous les groupes puissent la configurer et la gérer eux-mêmes, consultez la section [Verrouiller ou déverrouiller des préférences de projet pour tous les groupes du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

1. Cliquer sur **[!UICONTROL Enregistrer]**.

* [[!UICONTROL Statut de projet]](#project-status)
* [[!UICONTROL Chronologies]](#timelines)
* [[!UICONTROL Business cases]](#business-cases)
* [[!UICONTROL Reprise après une période d’inactivité]](#life-after-death)

### Statut de projet {#project-status}

Configurez l’une des préférences suivantes pour les projets nouvellement créés dans tout le système :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Allow users to create projects without using a template]</td> 
   <td>  <p>Cette préférence permet aux utilisateurs et aux utilisatrices de créer des projets sans utiliser de modèle lors de la création d’un projet à partir des zones suivantes : </p>
      <ul>
        <li>
        <p>Utiliser l’option [!UICONTROL New Project] dans une liste de projets</p>
        </li>
          <li>
          <p>Convertir un problème en projet à partir de la page du problème</p>
          </li>
         </ul>
        <p>Cette préférence est activée par défaut. </p> 
        <p><b>NOTE</b></p>
        <p> Un administrateur ou une administratrice de groupes peut modifier cette préférence pour un groupe. Lorsqu’un utilisateur ou une utilisatrice appartient à plusieurs groupes avec des préférences différentes, cette personne peut créer un projet sans modèle si cette préférence est activée pour son groupe principal.</p> 
        </td> 
  </tr>
  <tr> 
   <td role="rowheader">[!UICONTROL Set new project's status to]</td> 
   <td> <p>Déterminez le statut des nouveaux projets.</p>  <p><b>NOTE</b>  
     <ul> 
      <li>Si vous ou un autre administrateur ou une autre administratrice [!DNL Workfront] masquez le statut sélectionné ici, le statut par défaut passe au premier statut de la liste des statuts.</li> 
     </ul> 
     <ul> 
      <li> <p>Si un statut de groupe ou de système verrouillé est défini comme statut par défaut et qu’une personne le déverrouille par la suite, le système tente de le remplacer par un statut verrouillé du même type.</p> <p>S’il n’en trouve pas, il recherche un statut obligatoire :</p> 
       <ul> 
        <li>Si un statut obligatoire correspond au statut par défaut déverrouillé, le statut obligatoire devient le statut par défaut, même s’il est déverrouillé.</li> 
        <li>Si aucun des statuts obligatoires n’équivaut au statut par défaut déverrouillé, le premier statut obligatoire de la liste des statuts devient le statut par défaut.</li> 
       </ul> <p>Pour plus d’informations sur les statuts requis, voir les articles <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md" class="MCXref xref" data-mc-variable-override="">Accéder à la liste des statuts des projets système</a>, <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md" class="MCXref xref" data-mc-variable-override="">Accéder à la liste des statuts des tâches système</a>, et <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref" data-mc-variable-override="">Accéder à la liste des statuts des problèmes système</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calculate Percent Complete based on]</td> 
   <td> <p>Workfront calcule le pourcentage d’achèvement d’un projet ou d’une tâche mère à l’aide du pourcentage d’achèvement de chaque tâche du projet et soit de la durée, soit des heures planifiées de chaque tâche.</p><p>Le pourcentage d’achèvement de chaque tâche est défini manuellement par les personnes désignées.</p><p>Vous pouvez choisir ici si Workfront utilisera la Durée ou les Heures planifiées des tâches pour calculer le pourcentage de réalisation des projets.</p> <p>Si vous sélectionnez [!UICONTROL Duration], la durée de toutes les tâches d’un projet détermine le pourcentage terminé global du projet, et la durée de toutes les sous-tâches détermine le pourcentage terminé global de sa tâche parent.</p> <p>Si vous sélectionnez [!UICONTROL Duration], veillez à spécifier les [!UICONTROL Typical hours per work day] et les [!UICONTROL Typical work days per week] dans la section [!UICONTROL Timelines]. [!DNL Workfront] utilise ces informations lors du calcul du pourcentage terminé d’une tâche en fonction de la durée. </p> <p>Si vous sélectionnez [!UICONTROL Planned Hours], assurez-vous que toutes les tâches de chaque projet ont le [!UICONTROL Planned Hours] défini et que le montant n’est pas nul.</p><p>Pour plus d’informations, voir <a href="/help/quicksilver/manage-work/tasks/task-information/project-percent-complete.md">Présentation du pourcentage de projet terminé</a>.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Automatically set the project's Condition based on the Progress Status]</td> 
   <td> <p>Cette préférence permet aux utilisateurs et utilisatrices de définir manuellement le [!UICONTROL Condition] d’un projet sur [!UICONTROL On Target], [!UICONTROL At Risk], [!UICONTROL In Trouble] ou que [!DNL Workfront] définisse le [!UICONTROL Condition] (statut de la progression) automatiquement en fonction de la progression du projet dans la chronologie. Pour plus d’informations sur le statut des projets, voir <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref" data-mc-variable-override="">Vue d’ensemble du statut et du type de statut des projets</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Create baselines automatically]</p> </td> 
   <td> <p>Cette préférence crée automatiquement une référence (instantané) des détails de la tâche et du projet lorsque le statut du projet passe à [!UICONTROL Current]. Pour plus d’informations sur la création de références, voir <a href="../../../manage-work/projects/create-projects/create-baselines.md" class="MCXref xref" data-mc-variable-override="">Créer des références de projet</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Performance Index Method] </p> </td> 
   <td> <p>La méthode d’index de performance (PIM) du projet contrôle la méthode que [!DNL Workfront] utilise pour calculer les mesures de valeur obtenue, telles que [!UICONTROL Cost Performance Index] (ICP) et [!UICONTROL Estimate At Completion] (EAC). Pour plus d’informations, voir <a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref" data-mc-variable-override="">Calcul de l’[!UICONTROL Cost Performance Index] (ICP)</a> et <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">[!UICONTROL Calculate Estimate At Completion] (EAC)</a>.</p> 
    <ul> 
     <li><strong>[!UICONTROL Hour based]</strong> : [!DNL Workfront] utilise le [!UICONTROL Planned Hours] pour calculer des mesures de performances telles que l’EAC et l’ICP. Lorsque le PIM est calculé en fonction des heures, l’EAC s’affiche sous la forme d’un nombre d’heures. Assurez-vous que la valeur du [!UICONTROL Planned Hours] n’est pas nulle.</li> 
     <li> <p><strong>[!UICONTROL Cost-based]</strong> : [!DNL Workfront] utilise le [!UICONTROL Planned Labor Cost] pour calculer des mesures de performances telles que l’EAC et l’ICP. Assurez-vous que vos fonctions ou utilisateurs et utilisatrices sont associés à des taux de coût par heure. Lorsque le PIM est calculé en fonction des coûts, l’EAC s’affiche sous forme de valeur monétaire.</p> <p>La personne gestionnaire de projet peut modifier ce paramètre au niveau du projet, à l’aide de la zone [!UICONTROL Finance] dans [!UICONTROL Project Details]. Pour plus d’informations, voir <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">Gérer les informations dans la zone [!UICONTROL Finance] du projet</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Estimate at Completion ]</p> </td> 
   <td> <p>Contrôle les données que [!DNL Workfront] utilise pour calculer l’[!UICONTROL Estimate at Completion] (EAC), qui correspond au coût total planifié de votre projet.</p> 
    <ul> 
     <li><strong>[!UICONTROL Calculate at project level]</strong> : l’EAC de la tâche parent et du projet parent est déterminé en saisissant les [!UICONTROL Actual Hours] ou le [!UICONTROL Actual Labor Cost] dans les formules EAC. Le calcul inclut les [!UICONTROL Actual Hours] ou [!UICONTROL Costs and Expenses] ajoutés directement à la tâche parent ou au projet parent.</li> 
     <li> <p><strong>[!UICONTROL Roll up from tasks/subtasks]</strong> : l’EAC de la tâche et du projet parents est déterminé en additionnant l’EAC de toutes les tâches enfants. Ce calcul exclut les [!UICONTROL Actual Hours] ou les [!UICONTROL Actual Costs and Expenses] ajoutés directement à la tâche ou au projet parent.</p> <p>La personne responsable de la gestion de projet peut modifier ce paramètre au niveau du projet, à l’aide de la zone [!UICONTROL Finance] dans [!UICONTROL Project Details]. Pour plus d’informations, voir <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">Gérer les informations dans la zone [!UICONTROL Finance] du projet</a>.</p> </li> 
    </ul> <p>Pour plus d’informations sur le mode de calcul de l’EAC, voir <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">Calculer le [!UICONTROL Estimate At Completion] (CRE)</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Chronologies {#timelines}

Configurez l’une des préférences suivantes pour les projets nouvellement créés dans tout le système :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Schedule From]</td> 
   <td> <p>Déterminez si les nouveaux projets sont planifiés à partir de la date de début ou de la date d’achèvement au moment de leur création.</p> 
    <ul> 
     <li><strong>[!UICONTROL Start Date]</strong> : les nouvelles tâches sont définies par défaut sur la contrainte de tâche [!UICONTROL As Soon As Possible]. Les personnes responsables de la gestion de projet sont invitées à indiquer une [!UICONTROL Planned Start Date] pour le projet.</li> 
     <li><strong>[!UICONTROL Completion Date]</strong> : les nouvelles tâches sont définies par défaut sur la contrainte de tâche [!UICONTROL As Late As Possible]. Les personnes responsables de la gestion de projet sont invitées à indiquer une [!UICONTROL Planned Completion Date] pour le projet.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL User Time Off]</td> 
   <td> <p>Ce paramètre détermine si les congés de la personne cessionnaire principale d’une tâche modifient les dates prévues pour cette tâche dans le projet.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Consider user time off in task durations]</strong> : tous les congés planifiés pour la personne cessionnaire principale d’une tâche impactent les dates prévues de la tâche si les congés surviennent pendant la durée de la tâche. Il s’agit du paramètre par défaut. </p> <p>Par exemple, si une tâche dont la contrainte est définie sur [!UICONTROL As Soon As Possible] doit commencer le 1er juin et se terminer le 3 juin, et que la personne cessionnaire principale a enregistré des congés pour le 2 juin, les dates prévues de la tâche passent du 1er au 4 juin.</p> <p><b>IMPORTANT</b> :</p> <p>La durée de la tâche ne change pas lorsque vous sélectionnez ce paramètre. Seules les dates prévues changent, en fonction de la contrainte de tâche.</p> </li> 
     <li><strong>[!UICONTROL Ignore user time off in task durations]</strong> : les dates prévues de chaque tâche sur un projet restent comme initialement prévues, même si la personne cessionnaire principale d’une tâche a des congés pendant sa durée.</li> 
    </ul> <p>Tenez compte des points suivants lors de la sélection des options de ce paramètre :</p> 
    <ul> 
     <li>Lorsque vous modifiez ce paramètre, seuls les projets et les modèles créés après la modification héritent du paramètre mis à jour. </li> 
     <li> <p>La valeur Contrainte de tâche de la tâche détermine les dates de tâche prévues à ajuster : </p> 
      <ul> 
       <li>Date de début planifiée</li> 
       <li>Date d'achèvement prévue</li> 
       <li>Les deux dates.</li> 
       <li>Ni l’une ni l’autre. </li> 
      </ul> <p>Par exemple, si une tâche présente une contrainte de [!UICONTROL Fixed Dates], les dates ne s’ajustent pas lorsque la personne cessionnaire principale prend des congés, même si l’option [!UICONTROL Consider user time off in task duration] est sélectionnée. Pour plus d’informations sur les contraintes de tâche, voir <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref" data-mc-variable-override="">Vue d’ensemble des contraintes de tâche</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Project timelines are automatically re-calculated]</p> </td> 
   <td> <p>Déterminez quand la chronologie d’un projet est recalculée. Pour plus d’informations sur le nouveau calcul de la chronologie d’un projet, voir <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">Recalculer les chronologies d’un projet</a>.</p> <p>Les options suivantes sont activées par défaut. Vous pouvez sélectionner un ou plusieurs des paramètres suivants :</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Every night]</strong> : sélectionnez cette option pour recalculer les chronologies d’un projet toutes les nuits. Les modifications que vous apportez au projet susceptibles d’affecter la chronologie ne sont pas immédiatement visibles. [!DNL Workfront​​​] recalcule les chronologies la nuit uniquement pour les projets pour lesquels les deux conditions suivantes sont remplies :</p> <p> 
       <ul> 
        <li>Ont le statut [!UICONTROL Current]</li> 
        <li>Une mise à jour a eu lieu au cours des 3 derniers mois.</li> 
        <li>Possèdent l’un de ces types de mise à jour :</li>
        <ul>
        <li>Automatique et en cas de modification</li>
        <li>Modification uniquement</li>
        <li>Automatique uniquement</li> 
      </ul>       
    <b>CONSEIL :</b>
    <p>Les projets dont le type de mise à jour est Manuel uniquement ne sont pas affectés par ce paramètre.</p>
    <li> <p><strong>Lorsque l’étendue d’un projet change</strong> : sélectionnez cette option pour recalculer immédiatement les chronologies d’un projet en cas de changement d’étendue du projet. Pour plus d’informations sur ce qui constitue un changement d’étendue d’un projet, voir <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">Recalculer les chronologies d’un projet</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL When multiple users are assigned to a task use the schedule of the]</p> </td> 
   <td> <p>Si aucun planning n’est affecté à un projet ou si aucun planning n’est affecté aux personnes affectées à ses tâches, [!DNL Workfront] utilise le planning par défaut du système pour calculer la chronologie des tâches.</p> <p>Si vous affectez plusieurs personnes à la même tâche dans un projet, que le projet comporte un planning affecté et que les personnes affectées aux tâches disposent également d’un planning, [!UICONTROL Workfront] utilise les plannings suivants :</p> 
    <ul> 
     <li><strong>[!UICONTROL Primary Assignment]</strong> : [!DNL Workfront] utilise le planning de l’affectation principale sur la tâche pour calculer les chronologies.</li> 
     <li><strong>[!UICONTROL Project]</strong> : [!DNL Workfront] utilise le planning du projet pour calculer la chronologie de chaque tâche.</li> 
    </ul> <p>Pour plus d’informations sur les plannings, voir <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" data-mc-variable-override="">Créer un planning</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Timeline Calculations] </p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL Typical hours per work day]</strong> : définissez le nombre d’heures par jour de travail standard pour les personnes qui travailleront sur des projets. La valeur par défaut est de 8 heures.</li> 
    </ul> 
    <ul> 
     <li><strong>[!UICONTROL Typical work days per week]</strong> : définissez la semaine de travail standard pour les personnes qui travaillent sur des projets. La valeur par défaut est de 5 jours.</li> 
    </ul> <p>Ces 2 options convertissent les jours en heures ou les semaines en jours.</p> <p>Par exemple, si vous avez une tâche avec 8 heures prévues et que la durée est calculée en fonction du nombre d’heures prévues, [!DNL Workfront] convertit ces heures en jours afin d’afficher la durée en jours.</p> <p>Dans le champ [!UICONTROL work days per week], [!DNL Workfront] calcule la valeur de l’équivalent temps complet (FTE) de votre système. C’est ce que [!DNL Workfront] utilise lors du calcul des attributions pour les personnes.</p> <p>Ces valeurs sont utilisées lorsque vous planifiez les chronologies des projets, la budgetisation des ressources ou que vous consignez des heures par rapport aux projets. </p> <p>Elles ne sont pas utilisées lorsque vous définissez des feuilles de temps pour les personnes du système, comme décrit dans la section <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref" data-mc-variable-override="">[!UICONTROL Configure] les préférences de feuille de temps et d’heure</a>.</p> <p><b>REMARQUE</b></p> <p>[!DNL Workfront] Les administrateurs et administratrices ne peuvent pas déverrouiller les préférences [!UICONTROL Timeline Calculations].</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Custom Quarters]</p> </td> 
   <td> <p>Configurez des trimestres annuels personnalisés pour les personnes qui vont travailler sur des projets. Les trimestres personnalisés sont généralement des trimestres qui ne correspondent pas à la répartition traditionnelle des trimestres au cours d’une année civile. Vous pouvez ajouter plusieurs trimestres personnalisés. Pour plus d’informations, voir <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref" data-mc-variable-override="">Activer des trimestres personnalisés pour les projets</a>.</p>  <p><b>REMARQUE</b> : </p><p>[!DNL Workfront] Les administrateurs et administratrices ne peuvent pas déverrouiller les préférences [!UICONTROL Custom Quarters].</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Analyses de rentabilité] {#business-cases}

Vous pouvez créer une analyse de rentabilité pour les projets nouvellement créés dans tout le système afin d’envoyer des demandes de projet. Vous pouvez définir des préférences afin de déterminer les zones visibles sur le formulaire **[!UICONTROL Analyse de rentabilité]**. Nous vous recommandons d’activer ces options afin que d’autres outils, tels que l’[!UICONTROL Optimisateur de portfolio], se mettent à jour correctement. Pour plus d’informations sur ce que chaque champ affiche, voir [Définir une analyse de rentabilité : index des articles](../../../manage-work/projects/define-a-business-case/define-business-case.md).

Une fois que l’équipe d’administration [!DNL Workfront] a activé les sections sur l’[!UICONTROL analyse de rentabilité], le ou la propriétaire du projet peut créer une analyse de rentabilité au niveau du projet. Pour plus d’informations sur la création d’une analyse de rentabilité, voir [Créer une analyse de rentabilité pour un projet](../../../manage-work/projects/define-a-business-case/create-business-case.md).

### [!UICONTROL Reprise après une période d’inactivité] {#life-after-death}

Configurez l’une des préférences suivantes pour les projets nouvellement créés dans tout le système :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL After a project has been marked as Complete, people can still] </p> </td> 
   <td> <p>Déterminez les règles de votre organisation (ou groupe, si vous configurez les préférences d’un projet pour un groupe) pour spécifier si un objet (tâche ou problème) peut être supprimé une fois que le statut du projet a été marqué comme [!UICONTROL Complete].</p> 
    <ul> 
     <li><strong>[!UICONTROL Delete Tasks]</strong> : permet aux utilisateurs et utilisatrices de supprimer des tâches d’un projet une fois le projet marqué comme [!UICONTROL Complete].<br></li> 
     <li><strong>[!UICONTROL Delete Issues]</strong> : permet aux utilisateurs et utilisatrices de supprimer des problèmes d’un projet une fois le projet marqué comme [!UICONTROL Complete].</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL After a Project is marked Complete, Dead, or it is Pending Approval, people can still]</p> </td> 
   <td> <p>Déterminez les règles de votre organisation (ou groupe, si vous configurez les préférences d’un projet pour un groupe) concernant les tâches, les problèmes, les documents et autres objets dans un projet une fois que le statut du projet a été marqué comme <strong>[!UICONTROL Complete]</strong>, <strong>[!UICONTROL Dead]</strong>, ou <strong>[!UICONTROL Pending Approval]</strong>.</p> 
    <ul> 
     <li><strong>[!UICONTROL Add and edit tasks]</strong> : permet aux utilisateurs et utilisatrices d’effectuer les opérations suivantes :
      <ul>
       <li>Modifiez les tâches d’un projet une fois que le projet a été marqué comme [!UICONTROL Complete], [!UICONTROL Dead] ou [!UICONTROL Pending Approval]. Cela inclut l’ajout d’heures et la modification des entrées relatives aux dépenses sur une tâche.</li>
       <li>Ajouter des tâches à un projet.</li>
      </ul></li> 
     <li><strong>[!UICONTROL Add and edit issues]</strong> : permet aux utilisateurs et utilisatrices d’effectuer les opérations suivantes :
      <ul>
       <li>Modifiez les problèmes d’un projet une fois que le projet a été marqué comme [!UICONTROL Complete], [!UICONTROL Dead] ou [!UICONTROL Pending Approval].</li>
       <li>Ajoutez des problèmes à un projet une fois que le projet a été marqué comme [!UICONTROL Complete] ou [!UICONTROL Dead]. (Vous ne pouvez pas ajouter de problèmes à un projet [!UICONTROL Pending Approval].)</li>
      </ul></li> 
     <li> <p><strong>[!UICONTROL Add documents to the project and to its tasks and issues]</strong> : permet aux utilisateurs et utilisatrices d’ajouter des documents à un projet (ou d’ajouter des documents à des tâches et à des problèmes au sein du projet) une fois le projet marqué comme [!UICONTROL Complete] ou [!UICONTROL Dead].</p> <p>Cette option ne s’applique pas aux projets en attente d’approbation.</p> </li> 
     <li> <p><strong>[!UICONTROL Attach templates]</strong> : permet aux utilisateurs et utilisatrices de joindre des modèles à un projet une fois que le projet a été marqué comme [!UICONTROL Complete] ou [!UICONTROL Dead].</p> <p>Cette option ne s’applique pas aux projets en attente d’approbation.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
