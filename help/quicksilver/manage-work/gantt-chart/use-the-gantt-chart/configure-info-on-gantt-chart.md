---
content-type: reference
product-area: setup
navigation-topic: use-the-gantt-chart
title: Configurer l’affichage des informations sur le graphique de [!UICONTROL Gantt]
description: Vous pouvez configurer l’affichage des informations dans le graphique de Gantt de la liste des tâches et dans le graphique de Gantt de la liste des projets.
author: Alina
feature: Work Management
exl-id: 465365a2-d94b-47b6-a393-16770fca2714
source-git-commit: 2db4a79cad71b550b7de573c5b27293b6582858f
workflow-type: tm+mt
source-wordcount: '918'
ht-degree: 100%

---

# Configurer l’affichage des informations sur le [!UICONTROL graphique de Gantt]

Vous pouvez configurer l’affichage des informations à la fois dans le [!UICONTROL graphique de Gantt] de la liste des tâches et dans le [!UICONTROL graphique de Gantt] de la liste des projets.

## Conditions d’accès

Vous devez disposer des éléments suivants pour suivre les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] formule*</td> 
   <td> <p>Tous </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td> 
   <td> <p>[!UICONTROL Review] ou niveau supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Accès [!UICONTROL View] ou un accès supérieur aux projets et aux tâches.</p> <p>Note : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration [!DNL Workfront] si des restrictions supplémentaires sont définies pour votre niveau d’accès. Pour plus d’informations sur la manière dont l’administration [!DNL Workfront] peut modifier votre niveau d’accès, consultez la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Accès [!UICONTROL View] ou un accès supérieur au projet.</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, consultez la section <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez l’administration de [!DNL Workfront].

## Comprendre les options d’affichage

Le tableau suivant détaille les options d’affichage du [!UICONTROL graphique de Gantt] :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Actual Dates]</td> 
   <td> <img src="assets/actual-dates-in-gantt-183x213.png" alt="actual_dates_in_gantt.png" style="width: 183;height: 213;"> </td> 
   <td> <p>[!UICONTROL Actual Start Date] et [!UICONTROL Actual Completion Date] sont affichées avec une icône en forme de triangle. Si la [!UICONTROL Actual Completion Date] est nulle, seul la [!UICONTROL Actual Start Date] est affichée.</p> <p>Pour plus d’informations sur les dates de début et d’achèvement, voir <a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref">Vue d’ensemble de la [!UICONTROL Actual Completion Date] du projet</a> et <a href="../../../manage-work/projects/planning-a-project/project-actual-start-date.md" class="MCXref xref">Vue d’ensemble de la [!UICONTROL Actual Start Date] du projet</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assignments]</td> 
   <td> <img src="assets/assignments-in-gantt-312x203.png" alt="missions_in_gantt.png" style="width: 312;height: 203;"> </td> 
   <td> <p>Affiche les personnes cessionnaires des tâches.Placez la souris sur le lien <strong>[!UICONTROL Details]</strong> en regard du nom de la personne cessionnaire pour voir des informations plus détaillées à son sujet, y compris le pourcentage de son attribution à la tâche.</p> <p>Les personnes cessionnaires ne sont pas affichées sur le [!UICONTROL Gantt chart] lorsque le [!UICONTROL Gantt chart] est exporté au format PDF. Lorsque le [!UICONTROL Gantt chart] est exporté au format PDF, les personnes cessionnaires ne sont affichées que dans la liste des tâches.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Baseline]</td> 
   <td> <img src="assets/baselines-sandbox-gantt.png" alt="baselines_sandbox_gantt.png"> </td> 
   <td> <p>Aperçu du projet qui représente les éléments clés des données du projet incluses dans le plan de projet initial. Des références peuvent être prises en compte tout au long de la durée du projet. Lorsque vous activez l’affichage des références dans le [!UICONTROL Gantt chart], sélectionnez la référence que vous souhaitez afficher. Vous ne pouvez afficher qu’une référence à la fois sur le [!UICONTROL Gantt chart]. Celle-ci sera affichée sous la forme d’une barre grise.</p> <p>Pour plus d’informations sur les références, voir <a href="../../../manage-work/projects/create-projects/create-baselines.md" class="MCXref xref">Créer des références de projet</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Commit Date]</td> 
   <td> <img src="assets/commit-dates-sandbox-243x226.png" alt="commit_dates_sandbox.png" style="width: 243;height: 226;"> </td> 
   <td> <p>La date à laquelle une personne cessionnaire s’engage à ce que la tâche soit terminée est affichée avec un marqueur dans le [!UICONTROL Gantt chart]. </p> <p>Pour plus d’informations sur les dates d’engagement, voir la <a href="../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">Vue d’ensemble de la [!UICONTROL Commit Date]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL % Complete]</td> 
   <td> <img src="assets/percent-complete-gantt.png" alt="pourcentage_complet_gantt.png"> </td> 
   <td> Le pourcentage terminé de la tâche s’affiche dans la ligne de tâche.<br><br></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Critical Path]</td> 
   <td> <img src="assets/critical-path-2.png" alt="Critical_path_2.png"> </td> 
   <td>Les tâches susceptibles d’affecter la chronologie du projet sont considérées comme faisant partie du chemin d’accès critique et sont clairement marquées en rouge. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Milestone] Losanges</td> 
   <td> <img src="assets/milestone-diamonds.png" alt="milestone_diamonds.png"> </td> 
   <td> <p>Une icône en forme de losange s’affiche après la tâche associée à un jalon. Passez la souris sur un jalon pour afficher le nom et la date du jalon. L’administrateur ou l’administratrice [!DNL Workfront] détermine la couleur de chaque losange de jalon.</p> <p>Pour plus d’informations sur les jalons, voir <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md" class="MCXref xref">Créer un chemin jalonné</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Milestone] Lignes</td> 
   <td> <img src="assets/milestone-line-more-info-in-gantt-270x209.png" alt="milestone_line_more_info_in_gantt.png" style="width: 270;height: 209;"> </td> 
   <td> <p>Une ligne s’affiche après la tâche associée à un jalon. Passez la souris sur un jalon pour afficher le nom et la date du jalon. L’administrateur ou l’administratrice [!DNL Workfront] détermine la couleur de chaque ligne de jalon.</p> <p> Pour plus d’informations sur les jalons, voir <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md" class="MCXref xref">Créer un chemin jalonné</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Predecessors]</td> 
   <td> <img src="assets/predecessor-2-269x200.png" alt="predecessor_2.png" style="width: 269;height: 200;"> </td> 
   <td> <p>Ligne reliant une tâche à une autre et indiquant la relation antérieure entre les deux tâches. Pour mettre en surbrillance une ligne de tâche antérieure individuelle, passez la souris dessus. Cliquez dessus pour qu’elle reste en surbrillance. Vous ne pouvez mettre en surbrillance qu’une seule ligne de tâche antérieure à la fois.</p> <p>Une icône <strong>[!UICONTROL Predecessor]</strong> s’affiche en regard de toute tâche dont une relation antérieure s’étend sur plusieurs pages du graphique de Gantt ou de toute tâche liée à un projet transversal antérieur.</p> <p>Cliquez sur l’icône <strong>[!UICONTROL Predecessor]</strong> pour afficher toutes les tâches antérieures et ultérieures, ainsi que les détails de chaque tâche, tels que le nom de la tâche, le type de relation antérieure et les dates clés.</p> <p>Remarque : le [!UICONTROL Gantt Chart] dans une liste de projets affiche des informations sur les projets transversaux antérieurs. Pour plus d’informations sur la création de relations antérieures entre différents projets, voir <a href="../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md" class="MCXref xref">Créer des projets transversaux antérieurs</a>.</p> <p>Pour plus d’informations sur les tâches antérieures, voir <a href="../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md" class="MCXref xref">Appliquer les tâches antérieures</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Progress Status]</td> 
   <td> <p>[!UICONTROL On Time]<img src="assets/task-on-time--oct.-2017.png" alt="task_on_time__Oct._2017.png"></p> <p>[!UICONTROL Behind]<img src="assets/task-behind--oct.-2017.png" alt="task_behind__Oct._2017.png"></p> <p>[!UICONTROL At Risk]<img src="assets/task-at-risk.png" alt="task_at_risk.png"></p> <p>En retard<img src="assets/task-late-oct.2017.png" alt="task_late_Oct.2017.png"></p> </td> 
   <td> <p> </p> <p>Statut de progression actuelle d’une tâche donnée. </p> <p>Pour plus d’informations sur chaque type de [!UICONTROL Progress Status], voir <a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">Vue d’ensemble du [!UICONTROL Progress Status] de tâche</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Projected Dates]</td> 
   <td> <img src="assets/gantt-projected-dates-272x152.png" alt="gantt_projected_dates.png" style="width: 272;height: 152;"> </td> 
   <td> <p>Chronologie prévisionnelle indiquant la [!UICONTROL Projected Start] et les [!UICONTROL Completion dates] sur la base du travail actuellement terminé et du travail restant. </p> <p>Pour plus d’informations sur les dates d’achèvement prévisionnelles, voir <a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">Vue d’ensemble de la [!UICONTROL Projected Completion Date] pour les projets, les tâches et les problèmes</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configurer les options d’affichage

1. Accédez au [!UICONTROL Graphique de Gantt] de la liste des tâches ou au [!UICONTROL Graphique de Gantt] de la liste des projets.\
   Pour plus d’informations sur l’emplacement du [!UICONTROL Graphique de Gantt], voir [Commencer avec le [!UICONTROL Graphique de Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/get-started-with-gantt.md).

1. (Facultatif) Sélectionnez le paramètre **[!UICONTROL Passer aux dates prévisionnelles]** pour afficher les tâches en fonction de leurs [!UICONTROL Dates prévisionnelles]. Par défaut, les tâches sont affichées en fonction de leurs [!UICONTROL Dates prévues] dans le [!UICONTROL Graphique de Gantt].
1. Cliquez sur l’icône des options pour afficher la boîte de dialogue **[!UICONTROL Options]**.\
   ![Options.png](assets/options-350x129.png)

1. Sélectionnez les options de configuration que vous souhaitez afficher dans le [!UICONTROL Graphique de Gantt].

   >[!NOTE]
   > Toutes les options de configuration ne sont pas disponibles dans le [!UICONTROL Graphique de Gantt] de la liste des projets.

1. Cliquez n’importe où dans le [!UICONTROL Graphique de Gantt] pour fermer la boîte de dialogue **[!UICONTROL Options]**.
