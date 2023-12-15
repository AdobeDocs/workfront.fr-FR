---
title: Configuration des préférences de projet pour un groupe
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
description: Si vous êtes administrateur de groupe et qu’un administrateur Adobe Workfront déverrouille une préférence de projet pour tous les groupes du système, vous pouvez configurer cette préférence pour que votre groupe affecte tous les projets suivants créés par votre groupe.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: c69097fb-99e4-441b-9599-fd8af2dd7116
source-git-commit: fb1c7ade6622db391e0dac54f37603efe9dc0a58
workflow-type: tm+mt
source-wordcount: '2658'
ht-degree: 2%

---

# Configuration des préférences de projet pour un groupe

Si vous êtes administrateur de groupe et qu’un administrateur Adobe Workfront déverrouille une préférence de projet pour tous les groupes du système, vous pouvez configurer cette préférence pour que votre groupe affecte tous les projets suivants créés par votre groupe.

S’il existe des groupes au-dessus du groupe que vous gérez, leurs administrateurs peuvent également le faire pour votre groupe. Il en va de même pour les administrateurs de Workfront (pour n’importe quel groupe).

>[!NOTE]
>
>* En règle générale, une préférence déverrouillée reste déverrouillée indéfiniment. Si l’administrateur Workfront le reverrouille, le paramètre système prend à nouveau effet et les paramètres de la préférence accordée par les administrateurs du groupe sont perdus.
>* Les préférences définies pour le groupe associé à un projet sont prioritaires sur celles définies pour le groupe d’accueil de l’utilisateur qui crée le projet.
>* Certaines préférences au niveau du groupe affectent les modèles de projet que vous créez pour le groupe. Pour plus d’informations, voir la section [Affichage, utilisation et création de modèles pour votre groupe à partir de la zone Groupes](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#view) dans l’article [Créer et modifier des modèles de projet de groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).
>
>* Une fois qu’un administrateur Workfront a déverrouillé une préférence au niveau du système, vous pouvez la configurer, puis la verrouiller pour vous assurer que tous les membres de votre groupe et de ses sous-groupes utilisent la même configuration. Cela est parallèle à la possibilité qu’un administrateur de Workfront a de configurer et de verrouiller une préférence pour tous les utilisateurs du système. Pour plus d’informations, voir [Verrouillage ou déverrouillage d’un projet, d’une tâche ou d’une préférence d’émission pour les sous-groupes](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).
>

La configuration au niveau du groupe est également possible pour les préférences de tâche et de problème, ainsi que pour les préférences de feuille de temps et d’heure. Pour plus d’informations, voir [Configuration des préférences de tâche et de problème pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md) et [Configuration des préférences de feuille de temps et d’heure pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

Pour plus d’informations sur la façon dont un administrateur Workfront déverrouille une préférence de projet, voir [Verrouillage ou déverrouillage des préférences de projet pour tous les groupes du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

## Exigences d’accès

Les étapes de cet article doivent être les suivantes :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Workfront*</td> 
   <td>Quelconque</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> <p>Vous devez être un administrateur de groupe du groupe ou un administrateur Workfront. Pour plus d’informations, voir <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administrateurs de groupe</a> et <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Octroi d’un accès administratif complet à un utilisateur</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Si vous devez savoir quel plan ou type de licence vous avez, contactez votre administrateur Workfront.

## Configuration d’une préférence de projet déverrouillé pour un groupe

>[!TIP]
>
>Si vous êtes administrateur de Workfront, vous pouvez ignorer les étapes 1 à 4 en accédant à Configuration > Préférences du projet > Projets, puis en recherchant le nom du groupe dans la zone supérieure de la page.

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Dans le panneau de gauche, cliquez sur **Groupes** ![](assets/groups-icon.png).

1. Cliquez sur le nom du groupe dont vous souhaitez configurer les préférences du projet.
1. Dans le panneau de gauche, cliquez sur **Préférences du projet**.
1. Sur la page qui s’affiche, passez à l’une des quatre sections répertoriées ci-dessous pour configurer les préférences pour l’état du projet, les chronologies, les cas d’entreprise et la vie après la mort.

   >[!TIP]
   >
   >Si vous passez la souris sur une préférence et qu’une info-bulle s’affiche pour vous indiquer qu’elle est verrouillée, vous pouvez demander à votre administrateur Workfront de la déverrouiller pour tous les groupes de l’organisation.

* [État du projet](#project-status)
* [Chronologies](#timelines)
* [Analyses de cas](#business-cases)
* [Reprise après une période d&#39;inactivité](#life-after-death)

### Statut de projet {#project-status}

Configurez l’une des préférences suivantes pour les projets nouvellement créés associés au groupe :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody>

<tr><td>Autoriser les utilisateurs à créer des projets sans utiliser de modèle</td>
<td><p>Cette préférence permet aux utilisateurs de créer des projets sans utiliser de modèle lors de la création d’un projet à partir des zones suivantes :</p>
<ul>
<li><p>Utilisation de l’option Nouveau projet dans une liste de projets</p></li>

<li><p>Convertir un problème en projet à partir de la page du problème</p></li>
</ul>

<p>Cette préférence est activée par défaut au niveau du système.</p>
<p><b>NOTE</b></p>
<p>Lorsqu’un utilisateur appartient à plusieurs groupes avec des préférences différentes, il est autorisé à créer un projet sans modèle si au moins l’un de leurs groupes a cette préférence activée.</p>
</td></tr>
  <tr> 
   <td role="rowheader">Définissez l’état du nouveau projet sur</td> 
   <td> <p>Déterminez l’état des nouveaux projets.</p> <p><b>REMARQUE</b>   
     <ul> 
      <li>Si vous ou un autre administrateur Workfront masquez l’état sélectionné ici, l’état par défaut passe au premier état de la liste des états.</li> 
     </ul> 
     <ul> 
      <li data-mc-conditions="SnippetConditions-wf-groups.groups">Pour les préférences de projet de groupe, vous ne pouvez sélectionner qu’un état verrouillé ou un état obligatoire comme état par défaut.</li> 
      <li> <p>Si un état de groupe ou système verrouillé est défini comme état par défaut et qu’une personne le déverrouille par la suite, le système tente de le remplacer par un état verrouillé du même type.</p> <p>S’il n’en trouve pas, il recherche un statut requis :</p> 
       <ul> 
        <li>Si un état obligatoire correspond à l’état par défaut déverrouillé, l’état requis devient l’état par défaut, même s’il est déverrouillé.</li> 
        <li>Si aucun des états requis n’équivaut à l’état par défaut déverrouillé, le premier état requis dans la liste des états devient l’état par défaut.</li> 
       </ul> <p>Pour plus d’informations sur les états requis, voir les articles <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md" class="MCXref xref" data-mc-variable-override="">Accéder à la liste des états des projets système</a>, <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md" class="MCXref xref" data-mc-variable-override="">Accéder à la liste des états des tâches système</a>, et <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref" data-mc-variable-override="">Accéder à la liste des statuts des problèmes système</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Calculer le pourcentage terminé selon</td> 
   <td> <p>Le pourcentage d’achèvement d’un projet ou d’une tâche parente repose sur l’état d’avancement global des tâches. Ces informations peuvent être calculées en fonction de la Durée ou des Heures planifiées des tâches d’un projet.</p> <p>Si vous sélectionnez Durée, la Durée de chaque tâche d’un projet détermine le pourcentage global de réalisation pour le projet, et la Durée de chaque sous-tâche détermine le pourcentage global de réalisation pour sa tâche parent.</p> <p>Si vous sélectionnez Durée, veillez à spécifier les heures types par jour de travail et les jours types de travail par semaine dans la section Chronologies . Workfront utilise ces informations lors du calcul du pourcentage de réalisation d’une tâche en fonction de la durée. </p> <p>Si vous sélectionnez Heures planifiées, assurez-vous que le montant des heures planifiées est défini pour toutes les tâches de chaque projet et que le montant n’est pas nul.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrer automatiquement la Condition du projet en fonction du statut d'avancement</td> 
   <td> <p>Cette préférence permet aux utilisateurs de définir manuellement la condition d’un projet (sur la cible, à risque, en danger) ou de configurer automatiquement la condition (état de progression) par Workfront en fonction de la progression du projet dans la chronologie. Pour plus d’informations sur la condition des projets, voir <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref" data-mc-variable-override="">Présentation de la condition et du type de condition du projet</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Créer automatiquement des lignes de base</p> </td> 
   <td> <p>Cette préférence crée automatiquement une ligne de base (instantané) des détails de la tâche et du projet lorsque l’état du projet passe à Actuel. Pour plus d’informations sur la création de lignes de base, voir <a href="../../../manage-work/projects/create-projects/create-baselines.md" class="MCXref xref" data-mc-variable-override="">Création de lignes de base de projet</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Méthode d’indice de performance </p> </td> 
   <td> <p>La méthode d’index de performance (PIM) du projet contrôle la méthode utilisée par Workfront pour calculer les mesures de valeur acquise, telles que l’indice de performance des coûts (IPC) et l’estimation à la fin (EAC). Pour plus d’informations, voir <a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref" data-mc-variable-override="">Calculer l’indice de performance des coûts (IPC)</a>et <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">Calculer l’estimation à la fin (EAC)</a></p> 
    <ul> 
     <li><strong>Basé sur l’heure</strong>: Workfront utilise les heures planifiées pour calculer les mesures de performances telles que le taux d’endettement annuel et l’indice des prix à la consommation. Lorsque le PIM est calculé en fonction des heures, le CAE s’affiche sous la forme d’un nombre d’heures. Assurez-vous que vous disposez d’une valeur pour Heures planifiées, autre que zéro.</li> 
     <li> <p><strong>Basé sur les coûts</strong>: Workfront utilise le coût de la main-d’oeuvre planifiée pour calculer des mesures de performances telles que le CCE et l’IPC. Assurez-vous que vos rôles de tâche ou utilisateurs sont associés aux taux de coût par heure. Lorsque le PIM est calculé en fonction des coûts, le contrôle qualité s’affiche sous la forme d’une valeur monétaire.</p> <p>Le chef de projet peut modifier ce paramètre au niveau du projet, à l’aide de la zone Finance dans Détails du projet. Pour plus d’informations, voir <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">Gestion des informations dans la zone Finance du projet</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Estimation à l'achèvement </p> </td> 
   <td> <p>Déterminez les données utilisées par Workfront pour calculer l’estimation à la fin (EAC) qui représente le coût total prévu d’un projet.</p> 
    <ul> 
     <li><strong>Calcul au niveau du projet</strong>: le champ EAC de la tâche et du projet parents est déterminé en saisissant Heures réelles ou Coût réel de la main-d’oeuvre dans les formules EAC. Ce calcul inclut les Heures réelles ou les Coûts et Dépenses ajoutés directement à la tâche ou au projet parent.</li> 
     <li> <p><strong>Cumul à partir de tâches/sous-tâches</strong>: les champs de contrôle d’accès de la tâche parent et du projet sont déterminés en additionnant les champs de contrôle d’accès de chaque tâche enfant. Ce calcul exclut les Heures réelles ou les Coûts et dépenses réels ajoutés directement à la tâche ou au projet parent.</p> <p>Le chef de projet peut modifier ce paramètre au niveau du projet, à l’aide de la zone Finance dans Détails du projet. Pour plus d’informations, voir <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">Gestion des informations dans la zone Finance du projet</a>.</p> </li> 
    </ul> <p>Pour plus d’informations sur le mode de calcul du CAE, voir <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">Calculer l’estimation à la fin (EAC)</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Chronologies {#timelines}

Configurez l’une des préférences suivantes pour les projets nouvellement créés associés au groupe :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Planifier à partir de</td> 
   <td> <p>Déterminez si les nouveaux projets sont planifiés à partir de la date de début ou de la date de fin au moment de leur création.</p> 
    <ul> 
     <li><strong>Date de début</strong>: les nouvelles tâches sont définies par défaut sur la Contrainte de tâche Dès que possible et les gestionnaires de projet sont invités à fournir une Date de début planifiée pour le projet.</li> 
     <li><strong>Date d’achèvement</strong>: les nouvelles tâches prennent par défaut la valeur Contrainte de tâche aussi tardive que possible et les gestionnaires de projet sont invités à indiquer une date d’achèvement planifiée pour le projet.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Congés de l'utilisateur</td> 
   <td> <p>Déterminez si le délai de désactivation du cessionnaire Principal d’une tâche ajuste les dates prévues pour cette tâche sur un projet.</p> 
    <ul> 
     <li> <p><strong>Tenir compte du temps d’arrêt de l’utilisateur dans les durées de tâche</strong>: tout temps de congé planifié pour le cessionnaire Principal d’une tâche ajuste les dates planifiées de la tâche si le temps de congé survient pendant la durée de la tâche. Il s’agit du paramètre par défaut. </p> <p>Par exemple, si une tâche dont la contrainte est définie sur Dès que possible doit commencer le 1er juin et se terminer le 3 juin, et que la personne désignée par le Principal a marqué le 2 juin pour la période de congé, les dates prévues de la tâche s’ajustent du 1er au 4 juin.</p> <p><b>IMPORTANT</b>: la durée de la tâche ne change pas lorsque vous sélectionnez ce paramètre. Seules les dates planifiées changent, en fonction de la contrainte de tâche.</p> </li> 
     <li><strong>Ignorer le temps d’arrêt des utilisateurs dans les durées de tâche</strong>: les dates prévues de chaque tâche sur un projet restent comme initialement prévues, même si le cessionnaire Principal d’une tâche a un délai d’expiration pendant sa durée.</li> 
    </ul> <p>Tenez compte des points suivants lors de la sélection des options de ce paramètre :</p> 
    <ul> 
     <li>Lorsque vous modifiez ce paramètre, seuls les projets et les modèles créés après la modification héritent du paramètre mis à jour. </li> 
     <li> <p>La valeur Task Constraint de la tâche détermine les dates de tâche planifiées à ajuster : </p> 
      <ul> 
       <li>Date de début planifiée</li> 
       <li>Date d'achèvement prévue</li> 
       <li>Les deux dates</li> 
       <li>Ni l'une ni l'autre. </li> 
      </ul> <p>Par exemple, si une tâche présente une contrainte de dates fixes, les dates ne s’ajustent pas lorsque le cessionnaire Principal a un délai d’expiration, même si l’option Prendre en compte le délai d’expiration de l’utilisateur dans la durée de la tâche est sélectionnée. Pour plus d’informations sur les contraintes de tâche, voir <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref" data-mc-variable-override="">Présentation de la contrainte de tâche</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>Les chronologies du projet seront automatiquement recalculées.</strong> </p> </td> 
   <td> <p>Déterminez quand la chronologie d’un projet est recalculée. Pour plus d’informations sur le nouveau calcul de la chronologie du projet, voir <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">Recalculer les calendriers du projet</a>.</p> <p>Les options suivantes sont activées par défaut. Vous pouvez sélectionner un ou plusieurs des paramètres suivants :</p> 
    <ul> 
     <li> <p><strong>Chaque nuit</strong>: sélectionnez cette option pour recalculer les chronologies de projet toutes les nuits. Les modifications que vous apportez au projet susceptibles d’affecter la chronologie ne sont pas immédiatement visibles. Workfront ​ ​ recalcule les chronologies la nuit uniquement pour les projets pour lesquels les deux conditions suivantes sont remplies :</p> <p> 
       <ul> 
        <li>avoir un état actuel ;</li> 
        <li>ont eu une mise à jour au cours des 3 derniers mois ;</li> 
       </ul> </p> </li> 
     <li> <p><strong>Lorsque la portée d’un projet change</strong>: sélectionnez cette option pour recalculer immédiatement les échéances du projet en cas de changement de portée du projet. Pour plus d’informations sur ce qui constitue un changement de portée d’un projet, voir <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">Recalculer les calendriers du projet</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>Lorsque plusieurs utilisateurs sont affectés à une tâche, utilisez le planning de la fonction</strong> </p> </td> 
   <td> <p>Si aucun planning n’est affecté à un projet ou si aucun planning n’est affecté aux utilisateurs affectés à ses tâches, Workfront utilise le planning par défaut du système pour calculer la chronologie des tâches.</p> <p>Si vous affectez plusieurs utilisateurs à la même tâche dans un projet, un planning est affecté (et qu’un planning est également affecté aux utilisateurs affectés aux tâches), Workfront utilise les plannings suivants :</p> 
    <ul> 
     <li><strong>Attribution de Principal</strong>: Workfront utilise le planning de l’affectation de Principal sur la tâche pour calculer les chronologies.</li> 
     <li><strong>Projet</strong>: Workfront utilise le planning du projet pour calculer la chronologie de chaque tâche.</li> 
    </ul> <p>Pour plus d’informations sur les plannings, voir <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" data-mc-variable-override="">Création d’un planning</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Calculs de ligne de temps </p> </td> 
   <td> 
    <ul> 
     <li><strong>Heures types par jour de travail</strong>: définissez le nombre d’heures par jour de travail standard pour les utilisateurs qui travailleront sur des projets. La valeur par défaut est de 8 heures.</li> 
    </ul> 
    <ul> 
     <li><strong>Jours de travail standard par semaine</strong>: définissez la semaine de travail standard pour les utilisateurs qui vont travailler sur des projets. La valeur par défaut est de 5 jours.</li> 
    </ul> <p>Ces 2 options convertissent les jours en heures ou les semaines en jours.</p> <p>Par exemple, si vous avez une tâche avec 8 heures planifiées et que la durée est calculée sur la base des heures planifiées, Workfront convertit ces heures en jours afin d’afficher la durée en jours.</p> <p>À partir du champ Jours de travail standard par semaine , Workfront calcule la valeur de l’équivalent à temps complet (FTE) pour votre système. C’est ce que Workfront utilise lors du calcul des allocations pour les utilisateurs.</p> <p>Ces valeurs sont utilisées lorsque vous planifiez les calendriers des projets, la planification des ressources ou la journalisation du temps par rapport aux projets. </p> <p>Elles ne sont pas utilisées lorsque vous définissez des feuilles de temps pour les utilisateurs du système, comme décrit dans la section <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref" data-mc-variable-override="">Configuration des préférences de feuille de temps et d’heure</a>.</p> <p><b>REMARQUE</b>: les administrateurs de Workfront ne peuvent pas déverrouiller les préférences de calcul de la chronologie.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p><strong>Trimestres personnalisés</strong> </p> </td> 
   <td> <p>Configurez des trimestres annuels personnalisés pour les utilisateurs qui vont travailler sur des projets. Les trimestres personnalisés sont généralement des trimestres qui ne correspondent pas à la répartition traditionnelle des trimestres au cours d'une année civile. Vous pouvez ajouter plusieurs quartiers personnalisés. Pour plus d’informations, voir <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref" data-mc-variable-override="">Activation des trimestres personnalisés pour les projets</a>.</p> <p><b>REMARQUE</b>: les administrateurs Workfront ne peuvent pas déverrouiller les préférences Trimestres personnalisés.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Dossiers commerciaux {#business-cases}

Vous pouvez créer un Business Case pour les projets nouvellement créés associés au groupe afin d’envoyer des demandes de projet. Vous pouvez définir des préférences afin de déterminer les zones visibles sur le **Analyse de cas** formulaire. Nous vous recommandons d’activer ces options afin que d’autres outils, tels que Portfolio Optimizer, soient correctement mis à jour. Pour plus d’informations sur ce que chaque champ affiche, voir [Définition d’un cas d’entreprise : index des articles](../../../manage-work/projects/define-a-business-case/define-business-case.md).

Une fois que l’administrateur Workfront a activé les sections de l’analyse de cas, un propriétaire de projet peut créer une analyse de cas au niveau du projet. Pour plus d’informations sur la création d’un cas d’entreprise, voir [Création d’une analyse de cas pour un projet](../../../manage-work/projects/define-a-business-case/create-business-case.md).

### Reprise après une période d&#39;inactivité  {#life-after-death}

Configurez l’une des préférences suivantes pour les projets nouvellement créés associés au groupe :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p><strong>Une fois qu’un projet a été marqué comme terminé, les utilisateurs peuvent toujours</strong> </p> </td> 
   <td> <p>Déterminez les règles de votre organisation (ou groupe, si vous configurez les préférences d’un projet pour un groupe) pour déterminer si une tâche ou un problème peut être supprimé une fois le statut du projet marqué Terminé.</p> 
    <ul> 
     <li><strong>Suppression de tâches</strong>: permet aux utilisateurs de supprimer des tâches d’un projet une fois le projet marqué Terminé.<br></li> 
     <li><strong>Suppression de problèmes</strong>: permet aux utilisateurs de supprimer des problèmes d’un projet une fois le projet marqué Terminé.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>Une fois qu’un projet est marqué comme terminé, mort ou en attente d’approbation, les personnes peuvent toujours</strong> </p> </td> 
   <td> <p>Déterminez les règles de votre organisation (ou groupe, si vous configurez les préférences d’un projet pour un groupe) concernant les tâches, les problèmes, les documents et autres objets dans un projet une fois que l’état du projet a été marqué. <strong>Terminer</strong>, <strong>Mort</strong>, ou est <strong>En attente d’approbation</strong>.</p> 
    <ul> 
     <li><strong>Ajouter et modifier des tâches</strong> Permet aux utilisateurs de : 
      <ul> 
       <li>Modifiez les tâches d’un projet une fois que le projet a été marqué Terminé, Mort ou En attente d’approbation. Cela inclut l’ajout d’heures et la modification des entrées de dépenses sur une tâche.</li> 
       <li>Ajoutez des tâches à un projet.</li> 
      </ul></li> 
     <li><strong>Ajout et modification de problèmes</strong>: permet aux utilisateurs de : 
      <ul> 
       <li>Modifiez les problèmes d’un projet une fois que le projet a été marqué Terminé, Mort ou Autorisation en attente.</li> 
       <li>Ajoutez des problèmes à un projet une fois que le projet a été marqué Terminé ou Mort. (Vous ne pouvez pas ajouter de problèmes à un projet en attente d’approbation.)</li> 
      </ul></li> 
     <li> <p><strong>Ajouter des documents au projet et à ses tâches et problèmes</strong>: permet aux utilisateurs d’ajouter des documents à un projet (ou d’ajouter des documents à des tâches et à des problèmes au sein du projet) une fois le projet marqué Terminé ou Mort.</p> <p>Cette option ne s’applique pas aux projets en attente de validation.</p> </li> 
     <li> <p><strong>Ajout de modèles</strong>: permet aux utilisateurs de joindre des modèles à un projet une fois que le projet a été marqué Terminé ou Mort.</p> <p>Cette option ne s’applique pas aux projets en attente de validation.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
