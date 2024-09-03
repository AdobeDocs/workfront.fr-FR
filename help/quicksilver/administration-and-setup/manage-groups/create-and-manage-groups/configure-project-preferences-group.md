---
title: Configuration des préférences de projet pour un groupe
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
description: Si vous êtes administrateur ou administratrice de groupes et qu’un administrateur ou une administratrice Adobe Workfront déverrouille une préférence de projet pour tous les groupes du système, vous pouvez configurer cette préférence pour votre groupe afin qu’elle affecte tous les projets créés ultérieurement par votre groupe.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: c69097fb-99e4-441b-9599-fd8af2dd7116
source-git-commit: bd1a66950c6e16ef7eb05d385bd99fc2d3be35cc
workflow-type: tm+mt
source-wordcount: '2654'
ht-degree: 99%

---

# Configurer les préférences de projet pour un groupe

Si vous êtes administrateur ou administratrice de groupes et qu’un administrateur ou une administratrice Adobe Workfront déverrouille une préférence de projet pour tous les groupes du système, vous pouvez configurer cette préférence pour votre groupe afin qu’elle affecte tous les projets créés ultérieurement par votre groupe.

S’il existe des groupes au-dessus du groupe que vous gérez, leurs administrateurs et administratrices peuvent également le faire pour votre groupe. Il en va de même pour les administrateurs et administratrices de Workfront (pour n’importe quel groupe).

>[!NOTE]
>
>* En règle générale, une préférence déverrouillée reste déverrouillée indéfiniment. Si l’administrateur ou l’administratrice Workfront la verrouille à nouveau, le paramètre système prend à nouveau effet et les paramètres de la préférence définie par les administrateurs et administratrices de groupes sont perdus.
>* Les préférences définies pour le groupe associé à un projet sont prioritaires sur celles définies pour le groupe principal de l’utilisateur ou de l’utilisatrice qui crée le projet.
>* Certaines préférences au niveau du groupe affectent les modèles de projet que vous créez pour le groupe. Pour plus d’informations, voir la section [Afficher, utiliser et créer des modèles pour votre groupe à partir de la zone Groupes](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#view) dans l’article [Créer et modifier des modèles de projet d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).
>
>* Une fois qu’un administrateur ou une administratrice Workfront a déverrouillé une préférence au niveau du système, vous pouvez la configurer, puis la verrouiller pour vous assurer que toutes les personnes membres de votre groupe et de ses sous-groupes utilisent la même configuration. Ceci vient en parallèle de la capacité qu’a un administrateur ou une administratrice Workfront de configurer et de verrouiller une préférence pour tous les utilisateurs et utilisatrices du système. Pour plus d’informations, voir [Verrouiller ou déverrouiller une préférence de projet, de tâche ou de problème pour les sous-groupes](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).
>

La configuration à l’échelle des groupes est également possible pour les préférences des tâches et des problèmes, ainsi que pour les préférences des feuilles de temps et des heures. Pour plus d’informations, voir [Configurer les préférences des tâches et des problèmes pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md) et [Configurer les préférences des feuilles de temps et des heures pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront déverrouille une préférence de projet, voir [Verrouiller ou déverrouiller des préférences de projet pour tous les groupes du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des éléments suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Workfront*</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> <p>Vous devez faire partie de l’équipe d’administration de groupe pour le groupe ou de l’équipe d’administration Workfront. Pour plus d’informations, voir <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administrateurs et administratrices de groupe</a> et <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Octroyer un accès administratif complet à un utilisateur ou une utilisatrice</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Si vous devez connaître le plan ou le type de licence vous possédez, contactez votre administrateur ou votre administratrice Workfront.

+++

## Configurer une préférence de projet déverrouillée pour un groupe

>[!TIP]
>
>Si vous êtes un administrateur ou une administratrice Workfront, vous pouvez ignorer les étapes 1 à 4 en accédant à Configuration > Préférences de projet > Projets, puis en recherchant le nom du groupe dans la zone en haut de la page.

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Groupes** ![](assets/groups-icon.png).

1. Cliquez sur le nom du groupe dont vous souhaitez configurer les préférences de projet.
1. Dans le panneau de gauche, cliquez sur **Préférences de projet**.
1. Sur la page qui s’affiche, accédez à l’une des quatre sections listées ci-dessous pour configurer les préférences de Statut du projet, de Chronologies, de Business cases et de Reprise après une période d’inactivité.

   >[!TIP]
   >
   >Si vous passez la souris sur une préférence et qu’une info-bulle s’affiche pour vous indiquer qu’elle est verrouillée, vous pouvez demander à votre administrateur ou à votre administratrice Workfront de la déverrouiller pour tous les groupes de l’organisation.

* [Statut du projet](#project-status)
* [Chronologies](#timelines)
* [Business cases](#business-cases)
* [Reprise après une période d&#39;inactivité](#life-after-death)

### Statut de projet {#project-status}

Configurez l’une des préférences suivantes pour les projets nouvellement créés, associés au groupe :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody>

<tr><td>Autoriser les utilisateurs à créer des projets sans utiliser de modèle</td>
<td><p>Cette préférence permet aux utilisateurs et aux utilisatrices de créer des projets sans utiliser de modèle lors de la création d’un projet à partir des zones suivantes :</p>
<ul>
<li><p>Utiliser l’option Nouveau projet dans une liste de projets</p></li>

<li><p>Convertir un problème en projet à partir de la page du problème</p></li>
</ul>

<p>Cette préférence est activée par défaut au niveau du système.</p>
<p><b>NOTE</b></p>
<p>Lorsqu’une personne appartient à plusieurs groupes avec des préférences différentes, elle est autorisée à créer un projet sans modèle si cette préférence est activée pour au moins un de leurs groupes.</p>
</td></tr>
  <tr> 
   <td role="rowheader">Définir un nouveau statut pour le projet à</td> 
   <td> <p>Déterminez le statut des nouveaux projets.</p> <p><b>NOTE</b>   
     <ul> 
      <li>Si vous ou une autre personne chargée de l’administration de Workfront masquez le statut sélectionné ici, le statut par défaut passe au premier statut de la liste des statuts.</li> 
     </ul> 
     <ul> 
      <li data-mc-conditions="SnippetConditions-wf-groups.groups">Pour les préférences de projet de groupe, vous ne pouvez sélectionner qu’un statut verrouillé ou un statut obligatoire comme statut par défaut.</li> 
      <li> <p>Si un statut de groupe ou de système verrouillé est défini comme statut par défaut et qu’une personne le déverrouille par la suite, le système tente de le remplacer par un statut verrouillé du même type.</p> <p>S’il n’en trouve pas, il recherche un statut obligatoire :</p> 
       <ul> 
        <li>Si un statut obligatoire correspond au statut par défaut déverrouillé, le statut obligatoire devient le statut par défaut, même s’il est déverrouillé.</li> 
        <li>Si aucun des statuts obligatoires n’équivaut au statut par défaut déverrouillé, le premier statut obligatoire de la liste des statuts devient le statut par défaut.</li> 
       </ul> <p>Pour plus d’informations sur les statuts obligatoires, voir les articles <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md" class="MCXref xref" data-mc-variable-override="">Accéder à la liste des statuts des projets système</a>, <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md" class="MCXref xref" data-mc-variable-override="">Accéder à la liste des statuts des tâches système</a>, et <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref" data-mc-variable-override="">Accéder à la liste des statuts des problèmes système</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Calculer le pourcentage d’achèvement en fonction des points suivants</td> 
   <td> <p>Le pourcentage d’achèvement d’un projet ou d’une tâche parent repose sur la progression globale des tâches. Ces informations peuvent être calculées en fonction de la Durée ou du Nombre d’heures prévues des tâches d’un projet.</p> <p>Si vous sélectionnez Durée, la durée de chaque tâche d’un projet détermine le pourcentage global d’achèvement pour le projet, et la durée de chaque sous-tâche détermine le pourcentage d’achèvement global pour sa tâche parent.</p> <p>Si vous sélectionnez Durée, veillez à spécifier les heures types par jour de travail et les jours de travail types par semaine dans la section Chronologies. Workfront utilise ces informations lors du calcul du pourcentage d’achèvement d’une tâche en fonction de la durée. </p> <p>Si vous sélectionnez Nombre d’heures prévues, assurez-vous que le montant des heures prévues est défini pour toutes les tâches de chaque projet et que le montant n’est pas nul.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrer automatiquement la Condition du projet en fonction du statut d'avancement</td> 
   <td> <p>Cette préférence permet aux utilisateurs et utilisatrices de définir manuellement la condition d’un projet (Dans les temps, En danger, En difficulté) ou d’amener Workfront à configurer automatiquement la condition (statut de la progression) en fonction de la progression du projet dans la chronologie. Pour plus d’informations sur la condition des projets, voir la section <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref" data-mc-variable-override="">Vue d’ensemble de la condition et du type de condition du projet</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Créer automatiquement des lignes de base</p> </td> 
   <td> <p>Cette préférence crée automatiquement une référence (instantané) des détails de la tâche et du projet lorsque le statut du projet passe à Actuel. Pour plus d’informations sur la création de références, voir la section <a href="../../../manage-work/projects/create-projects/create-baselines.md" class="MCXref xref" data-mc-variable-override="">Créer des références de projet</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Méthode d'indice de performances </p> </td> 
   <td> <p>La méthode d’indice de performances (PIM) du projet contrôle la méthode utilisée par Workfront pour calculer les mesures de valeur acquise, telles que l’indice coûts/performances (CPI) et l’estimation à l’achèvement (EAC). Pour plus d’informations, voir les sections <a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref" data-mc-variable-override="">Calculer l’Indice Coûts Performances (CPI)</a> et <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">Calculer l’estimation à l’achèvement (EAC)</a>.</p> 
    <ul> 
     <li><strong>Basé sur les heures</strong> : Workfront utilise le nombre d’heures prévues pour calculer les mesures de performances telles que l’EAC et le CPI. Lorsque le PIM est calculé en fonction des heures, l’EAC s’affiche sous la forme d’un nombre d’heures. Assurez-vous de disposer d’une valeur non nulle pour le nombre d’heures prévues.</li> 
     <li> <p><strong>Basé sur les coûts</strong> : Workfront utilise le coût prévu de main-d’œuvre pour calculer des mesures de performances telles que l’EAC et le CPI. Assurez-vous que vos fonctions ou utilisateurs et utilisatrices sont associés à des taux de coût par heure. Lorsque le PIM est calculé en fonction des coûts, l’EAC s’affiche sous forme de valeur monétaire.</p> <p>La personne responsable de la gestion de projet peut modifier ce paramètre au niveau du projet, à l’aide de la zone Finances dans Détails du projet. Pour plus d’informations, voir la section <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">Gérer des informations dans la zone Finances du projet</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Estimation à l'achèvement </p> </td> 
   <td> <p>Déterminez les données que WorkFront utilise pour calculer l’estimation à l’achèvement (EAC), ce qui correspond au coût total projeté d’un projet.</p> 
    <ul> 
     <li><strong>Calculer au niveau du projet</strong> : l’EAC pour la tâche et le projet parent est déterminé à l’aide des heures effectives ou du coût réel de main-d’œuvre dans les formules EAC. Ce calcul inclut les heures effectives ou les coûts et dépenses ajoutés directement à la tâche ou au projet parent.</li> 
     <li> <p><strong>Regrouper depuis tâches/sous-tâches</strong> : l’EAC pour la tâche et le projet parent est déterminé en additionnant l’EAC pour chaque tâche enfant. Le calcul inclut les heures effectives ou les coûts et les dépenses réels ajoutés directement à la tâche ou au projet parent.</p> <p>La personne responsable de la gestion de projet peut modifier ce paramètre au niveau du projet, à l’aide de la zone Finances dans Détails du projet. Pour plus d’informations, voir la section <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">Gérer des informations dans la zone Finances du projet</a>.</p> </li> 
    </ul> <p>Pour plus d’informations sur le mode de calcul de l’EAC, voir la section <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">Calculer l’estimation à l’achèvement (EAC)</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Chronologies {#timelines}

Configurez l’une des préférences suivantes pour les projets nouvellement créés, associés au groupe :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Planifier à partir de</td> 
   <td> <p>Déterminez si les nouveaux projets sont planifiés à partir de la date de début ou de la date d’achèvement au moment de leur création.</p> 
    <ul> 
     <li><strong>Date de début</strong> : les nouvelles tâches sont définies par défaut sur la Contrainte de tâche Aussi Tôt que Possible et les personnes responsables de la gestion de projet sont invitées à fournir une date de début prévue pour le projet.</li> 
     <li><strong>Date d’achèvement</strong> : les nouvelles tâches prennent par défaut la Contrainte de tâche Aussi Tard Que Possible et les personnes responsables de la gestion de projet sont invitées à indiquer une date d’achèvement prévue pour le projet.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Congés de l’utilisateur ou de l’utilisatrice
</td> 
   <td> <p>Ce paramètre détermine si les congés de la personne cessionnaire principale d’une tâche modifient les dates prévues pour cette tâche dans le projet.</p> 
    <ul> 
     <li> <p><strong>Tenir compte des congés de l’utilisateur ou de l’utilisatrice dans les durées de tâche</strong> : tous les congés planifiés pour la personne cessionnaire principale d’une tâche impactent les dates prévues de la tâche si les congés surviennent pendant la durée de la tâche. Il s’agit du paramètre par défaut. </p> <p>Par exemple, si une tâche dont la contrainte est définie sur Aussi Tôt que Possible doit commencer le 1er juin et se terminer le 3 juin, et que la personne cessionnaire principale a enregistré des congés pour le 2 juin, les dates prévues de la tâche passent du 1er au 4 juin.</p> <p><b>IMPORTANT</b> : la durée de la tâche ne change pas lorsque vous sélectionnez ce paramètre. Seules les dates prévues changent, en fonction de la contrainte de tâche.</p> </li> 
     <li><strong>Ignorer les congés des personnes dans les durées de tâche</strong> : les dates prévues de chaque tâche sur un projet restent comme initialement prévues, même si la personne cessionnaire principale d’une tâche a des congés pendant sa durée.</li> 
    </ul> <p>Tenez compte des points suivants lors de la sélection des options de ce paramètre :</p> 
    <ul> 
     <li>Lorsque vous modifiez ce paramètre, seuls les projets et les modèles créés après la modification héritent du paramètre mis à jour. </li> 
     <li> <p>La valeur Contrainte de tâche de la tâche détermine les dates de tâche prévues à ajuster : </p> 
      <ul> 
       <li>Date de début planifiée</li> 
       <li>Date d'achèvement prévue</li> 
       <li>Les deux dates.</li> 
       <li>Ni l’une ni l’autre. </li> 
      </ul> <p>Par exemple, si une tâche présente une contrainte de dates fixes, les dates ne s’ajustent pas lorsque la personne cessionnaire principale a des congés, même si l’option Prendre en compte les congés des personnes dans la durée de la tâche est sélectionnée. Pour plus d’informations sur les contraintes de tâche, voir <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref" data-mc-variable-override="">Vue d’ensemble des contraintes de tâche</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>Les chronologies du projet seront recalculées automatiquement</strong>. </p> </td> 
   <td> <p>Déterminez quand la chronologie d’un projet est recalculée. Pour plus d’informations sur le nouveau calcul de la chronologie d’un projet, voir <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">Recalculer les chronologies d’un projet</a>.</p> <p>Les options suivantes sont activées par défaut. Vous pouvez sélectionner un ou plusieurs des paramètres suivants :</p> 
    <ul> 
     <li> <p><strong>Chaque nuit</strong> : sélectionnez cette option pour recalculer les chronologies d’un projet toutes les nuits. Les modifications que vous apportez au projet susceptibles d’affecter la chronologie ne sont pas immédiatement visibles. Workfront recalcule les chronologies la nuit uniquement pour les projets pour lesquels les deux conditions suivantes sont remplies :</p> <p> 
       <ul> 
        <li>Le statut est défini sur Actif.</li> 
        <li>Une mise à jour a eu lieu au cours des 3 derniers mois.</li> 
       </ul> </p> </li> 
     <li> <p><strong>Lorsque l’étendue d’un projet change</strong> : sélectionnez cette option pour recalculer immédiatement les chronologies d’un projet en cas de changement d’étendue du projet. Pour plus d’informations sur ce qui constitue un changement d’étendue d’un projet, voir <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">Recalculer les chronologies d’un projet</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>Lorsque plusieurs personnes affectées à une tâche utilisent le planning</strong> </p> </td> 
   <td> <p>Si aucun planning n’est affecté à un projet ou si aucun planning n’est affecté aux personnes affectées à ses tâches, Workfront utilise le planning par défaut du système pour calculer la chronologie des tâches.</p> <p>Si vous affectez plusieurs personnes à la même tâche dans un projet auquel un planning est affecté (et qu’un planning est également affecté aux personnes affectées aux tâches), Workfront utilise les plannings suivants :</p> 
    <ul> 
     <li><strong>Affectation principale</strong> : Workfront utilise le planning de l’affectation principale sur la tâche pour calculer les chronologies.</li> 
     <li><strong>Projet</strong> : Workfront utilise le planning du projet pour calculer la chronologie de chaque tâche.</li> 
    </ul> <p>Pour plus d’informations sur les plannings, voir <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" data-mc-variable-override="">Créer un planning</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Calculs de la chronologie </p> </td> 
   <td> 
    <ul> 
     <li><strong>Heures types par jour de travail</strong> : définissez le nombre d’heures par jour de travail standard pour les personnes qui travailleront sur des projets. La valeur par défaut est de 8 heures.</li> 
    </ul> 
    <ul> 
     <li><strong>Jours de travail standard par semaine</strong> : définissez la semaine de travail standard pour les personnes qui vont travailler sur des projets. La valeur par défaut est de 5 jours.</li> 
    </ul> <p>Ces 2 options convertissent les jours en heures ou les semaines en jours.</p> <p>Par exemple, si vous avez une tâche avec 8 heures prévues et que la durée est calculée sur la base des heures prévues, Workfront convertit ces heures en jours afin d’afficher la durée en jours.</p> <p>À partir du champ Jours ouvrables standard par semaine, Workfront calcule la valeur de l’équivalent temps complet pour votre système. C’est ce que Workfront utilise lors du calcul des allocations pour les personnes.</p> <p>Ces valeurs sont utilisées lorsque vous planifiez les chronologies des projets, la budgetisation des ressources ou que vous consignez des heures par rapport aux projets. </p> <p>Elles ne sont pas utilisées lorsque vous définissez des feuilles de temps pour les personnes du système, comme décrit dans la section <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref" data-mc-variable-override="">Configurer les préférences de feuilles de temps et d’heures</a>.</p> <p><b>NOTE</b> : les administrateurs et administratrices Workfront ne peuvent pas déverrouiller les préférences de calcul des chronologies.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p><strong>Trimestres personnalisés</strong> </p> </td> 
   <td> <p>Configurez des trimestres annuels personnalisés pour les personnes qui vont travailler sur des projets. Les trimestres personnalisés sont généralement des trimestres qui ne correspondent pas à la répartition traditionnelle des trimestres au cours d’une année civile. Vous pouvez ajouter plusieurs trimestres personnalisés. Pour plus d’informations, voir <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref" data-mc-variable-override="">Activer des trimestres personnalisés pour les projets</a>.</p> <p><b>NOTE</b> : les administrateurs et administratrices Workfront ne peuvent pas déverrouiller les préférences des trimestres personnalisés.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Dossiers commerciaux {#business-cases}

Vous pouvez créer un business case pour les projets nouvellement créés associés au groupe afin d’envoyer des demandes de projet. Vous pouvez définir des préférences afin de déterminer les zones visibles sur le formulaire du **business case**. Nous vous recommandons d’activer ces options afin que d’autres outils, tels que l’optimisateur de portfolio, soient correctement mis à jour. Pour plus d’informations sur ce que chaque champ affiche, voir [Définir un business case : index des articles](../../../manage-work/projects/define-a-business-case/define-business-case.md).

Une fois que l’administration Workfront a activé les sections du business case, une personne propriétaire de projet peut créer un business case au niveau du projet. Pour plus d’informations sur la création d’un business case, consultez la section [Créer un business case pour un projet](../../../manage-work/projects/define-a-business-case/create-business-case.md).

### Reprise après une période d&#39;inactivité  {#life-after-death}

Configurez l’une des préférences suivantes pour les projets nouvellement créés, associés au groupe :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p><strong>Après qu’un projet a été marqué comme Terminé, les personnes peuvent toujours effectuer les actions suivantes :</strong> </p> </td> 
   <td> <p>Déterminer les règles de votre entreprise (ou groupe, si vous configurez les préférences d’un projet pour un groupe) relatives à la suppression d’une tâche ou d’un problème une fois le statut du projet marqué comme Terminé.</p> 
    <ul> 
     <li><strong>Supprimer des tâches</strong> : permet aux utilisateurs et utilisatrices de supprimer des tâches d’un projet une fois le projet marqué comme Terminé.<br></li> 
     <li><strong>Supprimer des problèmes</strong> : permet aux utilisateurs et utilisatrices de supprimer des problèmes d’un projet une fois le projet marqué comme Terminé.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>Après qu’un projet a été marqué comme Terminé ou Inactif, ou s’il est en attente d’approbation, les personnes peuvent toujours effectuer les actions suivantes :</strong> </p> </td> 
   <td> <p>Déterminer les règles de votre entreprise (ou groupe, si vous configurez les préférences d’un projet pour un groupe) relatives aux tâches, aux problèmes, aux documents et aux autres éléments d’un projet une fois le statut du projet marqué comme <strong>Terminé</strong>, <strong>Inactif</strong> ou <strong>En attente d’approbation</strong>.</p> 
    <ul> 
     <li><strong>Ajouter et modifier des tâches</strong> : permet aux utilisateurs et utilisatrices d’effectuer les actions suivantes : 
      <ul> 
       <li>Modifier les tâches d’un projet une fois celui-ci marqué comme Terminé, Inactif ou En attente d’approbation. Cela inclut l’ajout d’heures et la modification des entrées relatives aux dépenses sur une tâche.</li> 
       <li>Ajouter des tâches à un projet.</li> 
      </ul></li> 
     <li><strong>Ajouter et modifier des problèmes</strong> : permet aux utilisateurs et utilisatrices d’effectuer les actions suivantes : 
      <ul> 
       <li>Modifier les problèmes d’un projet une fois celui-ci marqué comme Terminé, Inactif ou En attente d’approbation.</li> 
       <li>Ajouter des problèmes à un projet une fois celui-ci marqué comme Terminé ou Inactif (vous ne pouvez pas ajouter de problèmes à un projet en attente d’approbation).</li> 
      </ul></li> 
     <li> <p><strong>Ajouter des documents au projet et à ses tâches et problèmes</strong> : permet aux utilisateurs et utilisatrices d’ajouter des documents à un projet (ou d’ajouter des documents à des tâches et à des problèmes au sein du projet) une fois le projet marqué comme Terminé ou Inactif.</p> <p>Cette option ne s’applique pas aux projets en attente d’approbation.</p> </li> 
     <li> <p><strong>Joindre des modèles</strong> : permet aux utilisateurs et utilisatrices de joindre des modèles à un projet une fois celui-ci marqué comme Terminé ou Inactif.</p> <p>Cette option ne s’applique pas aux projets en attente d’approbation.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
