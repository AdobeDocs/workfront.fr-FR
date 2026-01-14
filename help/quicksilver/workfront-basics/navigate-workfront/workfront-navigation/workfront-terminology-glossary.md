---
content-type: reference
navigation-topic: workfront-navigation
title: 'Glossaire de la terminologie  [!DNL Adobe Workfront] '
description: Le glossaire  [!DNL Adobe Workfront]  répertorie les termes couramment utilisés dans l’interface et les rapports  [!DNL Adobe Workfront]. You can use the glossary when you want to find the definition of concepts you see in the [!UICONTROL Workfront] , et s’avère utile si vous essayez de comprendre la signification de concepts  [!DNL Workfront]  définis dans la documentation  [!DNL Workfront] .
author: Alina
feature: Get Started with Workfront
exl-id: 758072b3-775e-4771-9ae9-da0b38580c93
source-git-commit: 8f7249e08268a8cb784d4c0ecc8c534542fa80cf
workflow-type: tm+mt
source-wordcount: '21561'
ht-degree: 92%

---


# Glossaire de la terminologie [!DNL Adobe Workfront]

<!--Audited: 12/2023-->

>[!IMPORTANT]
>
>Cet article doit servir de référence pour comprendre les termes que vous pouvez rencontrer dans l’application [!DNL Adobe Workfront], dans la documentation [!DNL Workfront] ou, en général, dans la planification et la gestion du travail. Nous mettons actuellement à jour ces informations et il se peut donc que ce tableau ne soit pas complet. Nous supprimerons cet avertissement lorsque ces informations seront considérées comme exhaustives.

Le tableau suivant répertorie les termes fréquemment utilisés dans Adobe Workfront :

## A - C

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Nom de l'objet</strong></th> 
   <th><strong>Description</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Access Level]</td> 
   <td>Profil d’utilisateur ou d’utilisatrice qui détermine comment cette personne peut interagir avec différents objets et outils dans Workfront.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Active Task]</td> 
   <td>Tâche incomplète dans un projet en cours sur laquelle aucune une tâche antérieure n’empêche de travailler et qui n’a pas de contrainte de tâche avec une date de début prévue ultérieure. En d’autres termes, vous pouvez travailler sur la tâche aujourd’hui.</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Activity]</td> 
   <td>Dans [!DNL Workfront Goals], une activité est un indicateur de progression pour un objectif. Il peut s’agir d’une barre de progression que vous mettez à jour manuellement ou d’un projet associé à l’objectif. Vous ne pouvez pas afficher d’activités dans un rapport et vous ne pouvez pas y accéder via l’API [!DNL Workfront]. Pour plus d’informations sur les activités, voir <a href="../../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md" class="MCXref xref">Commencer avec les résultats et les activités dans les Objectifs Adobe Workfront</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Actual Cost]</td> 
   <td> <p>Pour les tâches et les problèmes, il s’agit du coût associé aux heures effectives consignées par rapport au coût par heure de la ressource affectée à la tâche ou au problème. Pour les projets, il s’agit du total des [!UICONTROL Actual Costs] provenant des tâches et des problèmes du projet. Pour plus d’informations, voir <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Suivre les coûts</a>.</p>

<p>Les calculs de [!UICONTROL Actual Cost] prennent en compte les [!UICONTROL Legacy Actual Hours]. Pour plus d'informations, consultez la section « [!UICONTROL Heures réelles] » ou « [!UICONTROL Heures réelles héritées] » de ce tableau. </p>   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Actual Expense Cost]</td> 
   <td> <p>Somme des [!UICONTROL Actual Amounts] pour toutes les dépenses enregistrées pour un projet ou une tâche.</p> <b>EXEMPLE</b>
   <p>Si vous créez une dépense pour la tâche 1 et que vous saisissez 600,00 $ dans le champ [!UICONTROL Actual Amount], le [!UICONTROL Actual Expense Cost] de cette tâche est de 600,00 $. </p> 
   <p>Pour un projet, [!DNL Workfront] utilise la formule suivante pour calculer le [!UICONTROL Actual Expense Cost] :</p> <p><code>Project Actual Expense Cost = SUM (All Project Actual Expense Costs) + SUM (All Tasks Actual Expense Costs) + Project Fixed Cost</code> <br> </p> 
   <!--
     <p>Important: If the value in the Actual Amount field for an expense is negative, Workfront will ignore that expense record. For example, if the value in the Planned Amount field is $200.00 but the value in the Actual Amount field is -$300.00, the system will ignore this entire expense record which means you would not include the $200.00 planned value or the -$300.00 actual value in any calculations for Planned Expense Cost or Actual Expense Cost. (drafting this because not sure if this is still correct)</p>
    --> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Actual Hours]</td> 
   <td> <p>Dans un rapport de projet, de tâche ou d’événement, les [!UICONTROL Actual Hours] correspondent à la somme de toutes les heures consignées dans le projet, la tâche ou l’événement après mai 2021.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemple : </b></span></span>si, dans l’onglet [!UICONTROL Updates] de la tâche 1, vous cliquez sur « Consigner des heures » et que vous saisissez 25 heures, les heures effectives de la tâche 1 = 25 heures. </p> <p>[!DNL Workfront] calcule les [!UICONTROL Actual Hours] pour les tâches ou les projets parents à l’aide des formules suivantes :</p> 
    <ul> 
     <li> <p><code>For parent tasks = children [!UICONTROL Actual Hours] + [!UICONTROL Actual Hours] on the parent task. </code> </p> </li> 
     <li> <p><code>For projects = [!UICONTROL Actual Hours] logged on the project + [!UICONTROL Actual Hours] logged on standalone or children tasks in the project + [!UICONTROL Actual Hours] logged on issues in the project</code>  </p> </li> 
    </ul> 
   <p>Voir aussi <strong>[!UICONTROL Heures effectives héritées]</strong>.
    <p>Pour plus d'informations, voir <a href="/help/quicksilver/manage-work/tasks/task-information/actual-hours.md">Afficher les heures réelles</a>.</p>
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Actual Labor Cost]</td> 
   <td> <p>[!UICONTROL Actual Cost] associé à la main-d’œuvre investie dans une tâche ou un projet. </p> <p>Pour une tâche, [!DNL Workfront] calcule le [!UICONTROL Actual Labor Cost] à l’aide de la formule suivante :</p> <p><code>Task [!UICONTROL Actual Labor Cost] = Number of [!UICONTROL Actual Hours] on the task * User or Job Role [!UICONTROL Hourly Cost Rate]</code> </p> <p>Si la tâche a un [!UICONTROL Cost Type] de [!UICONTROL User Hourly], [!DNL Workfront] utilise le taux de l’utilisateur ou de l’utilisatrice. Si la tâche a un [!UICONTROL Cost Type] de [!UICONTROL Role Hourly], [!DNL Workfront] utilise le taux de la fonction pour calculer le [!UICONTROL Actual Labor Cost]. </p> <p>Pour un projet, [!DNL Workfront] utilise la formule suivante pour calculer le [!UICONTROL Actual Labor Cost] :</p> <p><code>Project [!UICONTROL Actual Labor Cost] = SUM(All Tasks [!UICONTROL Actual Labor Cost]) </code> </p> <p>Pour plus d’informations, voir <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Suivre les coûts</a>.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemple : </b></span></span>par exemple, si un utilisateur ou une utilisatrice consigne 5 heures pour une tâche avec un [!UICONTROL Cost Type] de [!UICONTROL User Hourly] et que son taux horaire est de 100 $, le [!UICONTROL Actual Labor Cost] est de 500 $.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Actual Revenue] </td> 
   <td> <p>[!UICONTROL Actual Revenue] d’un projet ou d’une tâche correspond au montant d’argent associé aux [!UICONTROL Actual Hours] du projet ou de la tâche. </p> <p>Pour plus d’informations sur le suivi des revenus dans [!DNL Workfront], voir <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Vue d’ensemble de la facturation et des revenus</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Actual Start]</td> 
   <td>Date et heure auxquelles un utilisateur ou une utilisatrice modifie un objet en cours sur le travail qui lui est affecté.</td> 
  </tr> 
  <!--<tr> 
 <td>A type of work process that is unplanned.</td> 
 -->
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Additional Schedules</td> 
    <td>An additional preset to be used for a new user group.</td> 
   </tr>
  --> 
  <tr> 
   <td>Méthodologie [!UICONTROL Agile]</td> 
   <td>Type de méthodologie basée sur l’évolution collaborative des besoins et des solutions avec des équipes interfonctionnelles. Il encourage la flexibilité et le changement selon une chronologie définie.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Agile Team]</td> 
   <td>Diffère d’une équipe traditionnelle, car elle récupère ses travaux futurs à partir d’une liste d’attente et travaille sur ceux-ci sur une période définie appelée [!UICONTROL Iteration].</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL All My Teams]</td> 
   <td> <p>Lorsqu’il est référencé dans les [!UICONTROL filters], ce champ affiche soit les utilisateurs et utilisatrices appartenant à l’une des équipes auxquelles appartient l’utilisateur ou utilisatrice connecté, soit les éléments de travail affectés à l’une des équipes auxquelles appartient l’utilisateur ou utilisatrice connecté. </p> <p>Il est recommandé d’utiliser ce champ dans un filtre afin de rendre les rapports plus génériques lors de leur partage avec d’autres utilisateurs et utilisatrices. Ainsi, vous pouvez créer un seul rapport qui affichera des informations différentes en fonction de la personne qui se connecte pour les afficher, car les informations sont toujours personnalisées pour l’utilisateur ou utilisatrice connecté. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Allocation Date]</td> 
   <td> <p>Vous trouverez ce champ dans les types de rapports suivants :</p> 
    <ul> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates</li>
     --> 
     <li>[!UICONTROL Project] (données financières)</li> 
     <li>[!UICONTROL Budgeted Hour]</li> 
    </ul> <p>Pour un<!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        Resource Estimates or 
      </MadCap:conditionalText>
     -->rapport [!UICONTROL Project (Financial Data)] : </p> 
    <ul> 
     <li>Créez ce rapport lorsque vous essayer de comprendre<!--
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
         how resources are budgeted for work, or 
       </MadCap:conditionalText>
      --> le montant des [!UICONTROL Planned Hours] affectées à vos ressources.</li> 
     <li> <p>La [!UICONTROL Allocation Date] est le premier jour (dimanche) d’une semaine au cours duquel l’attribution d’une [!UICONTROL Job Role] à une tâche commence. Une ressource ([!UICONTROL Job Role]) peut comporter autant de [!UICONTROL Allocation Dates] que de semaines au cours de la [!UICONTROL Duration] des tâches auxquelles elle est affectée. Si les tâches s’étendent sur plusieurs mois, le premier jour d’un mois peut également devenir une [!UICONTROL Allocation Date], si elle tombe dans la [!UICONTROL Duration] de la tâche.</p> <p>Par exemple, vous pouvez avoir une [!UICONTROL Job Role] affectée à une tâche qui s’étend sur 3 semaines et qui comprend 90 [!UICONTROL Planned Hours]. Ces heures sont réparties uniformément pendant la durée de la tâche, ce qui fait que chaque jour attribue 6 [!UICONTROL Planned Hours] à votre fonction :</p> <p><em> [!UICONTROL Daily Planned Hours] = [!UICONTROL Total Planned Hours]/ Nombre [!UICONTROL Work Days] pendant la [!UICONTROL Duration] de la tâche </em> </p> <p>Par conséquent, il existe trois [!UICONTROL Allocation Dates], une pour chaque dimanche de chaque semaine pendant la [!UICONTROL Duration] de la tâche, chacune associée à un certain nombre d’[!UICONTROL Planned Hours].<br>Si la tâche commence au milieu de la dernière semaine d’un mois et se termine deux semaines après le début d’un nouveau mois, la tâche aura quatre [!UICONTROL Allocation Dates] : une pour chaque dimanche de chaque semaine pendant la [!UICONTROL Duration] de la tâche, et une pour le premier jour du nouveau mois.</p> <p>Pour tirer le meilleur parti de ces informations, nous vous recommandons de créer un <!--
        <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          Resource Estimates or a 
        </MadCap:conditionalText>
       --> rapport de projet (données financières), d’ajouter un regroupement par matrice pour la [!UICONTROL Allocation Date], puis de regrouper les résultats chaque semaine, chaque mois, chaque trimestre ou chaque année pour obtenir les données les plus précises.<br>Pour plus d’informations sur la création d’un regroupement par matrice, consultez l’article <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md" class="MCXref xref">Créer un rapport de matrice</a>.</p> </li> 
    </ul> <p>Les informations financières sont renseignées dans les rapports [!UICONTROL Project (Financial Data)] uniquement lorsque les données qui y sont associées ont moins de 5 ans. Par exemple, si une fonction a été affectée à une tâche en janvier 2015 et qu’aujourd’hui nous sommes le septembre 2021, un champ financier comme la [!UICONTROL Allocation Date] de la fonction n’est pas renseignée dans le rapport [!UICONTROL Project (Financial Data)]. </p> 
    <div> 
     <p>Pour un rapport [!UICONTROL Budgeted Hour] :</p> 
     <ul> 
      <li>Créez ce rapport lorsque vous essayez de comprendre le nombre d’[!UICONTROL Budgeted Hours] qui est alloué à vos ressources ou à vos projets dans le planificateur de ressources.</li> 
      <li> <p>La [!UICONTROL Allocation Date] est le premier jour (un dimanche) de la semaine pour lequel vous avez budgété les heures dans le [!UICONTROL Resource Planner]. </p> <p><b>CONSEIL</b></p> <p>Si une semaine s’étend sur deux mois, elle génère deux lignes dans le rapport : l’une correspondant au premier jour de la semaine (le dimanche de la première semaine qui dure le premier mois), et la seconde ligne affiche le premier jour du second mois. </p> <p>Si, par exemple, vous allouez 8 heures à un utilisateur ou une utilisatrice pour la semaine du 30 juin (dimanche) au 6 juillet (samedi), les deux lignes indiquent une [!UICONTROL Allocation Date] du 30 juin et du 1er juillet. </p> </p> <p>Pour plus d’informations sur la budgétisation des ressources dans le [!DNL Resource Planner], voir l’article <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Établir un budget de ressources dans le [!DNL Resource Planner] à l’aide des vues [!UICONTROL Project] et [!UICONTROL Role]</a>.</p> <p>Pour plus d’informations sur la création d’un rapport [!UICONTROL Budgeted Hour], voir <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref">Rapport : heures budgétées</a>. </p> </li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Announcements]</td> 
   <td> <p>Un moyen de communiquer aux utilisateurs et utilisatrices les informations dans le système. Ces informations proviennent souvent de [!DNL Workfront] à l’administrateur ou administratrice ou bien de l’administrateur ou administratrice à l’utilisateur ou utilisatrice. </p> <p>Pour plus d’informations, voir <a href="../../../administration-and-setup/get-started-wf-administration/view-send-announcements.md" class="MCXref xref">Envoyer des annonces</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL App Integration]</td> 
   <td>Une application représente le plus souvent un connecteur vers une application logicielle, mais peut également représenter des fonctions spéciales qui manipulent des données.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Approver Decision]</td> 
   <td> <p>Dans le rapport [!UICONTROL Proof Approval], ce champ affiche les décisions d’approbation d’épreuve pour les épreuves qui ne sont plus actives.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Approver stage]</td> 
   <td>Dans le [!UICONTROL Proof Approval report], ce champ affiche des informations sur l’étape actuelle des épreuves.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Approval]</td> 
   <td> <p>Un élément de travail donné, tel qu’une tâche, un document ou une feuille de temps, peut exiger qu’une personne en charge de la supervision ou une autre personne valide l’élément de travail. Ce processus d’autorisation est appelé approbation. </p> <p>Pour plus d’informations, voir <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">Vue d’ensemble du processus d’approbation</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Approval date]</td> 
   <td>Dans le rapport [!UICONTROL Proof Approval], ce champ affiche la date à laquelle une épreuve a été approuvée.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Approver]</td> 
   <td>Un utilisateur, une utilisatrice ou une fonction qui doit approuver un élément de travail donné, ou l’utilisateur ou utilisatrice qui approuve les saisies d’heures sur les feuilles de temps.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assigned To]</td> 
   <td> <p>Dans un rapport de [!UICONTROL Task or Issue], ce champ affiche la personne propriétaire de la tâche ou du problème, ou la personne [!UICONTROL Primary Assignee]. Vous pouvez également filtrer ou regrouper en fonction de ce champ.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assignment]</td> 
   <td>Personne, fonction ou équipe affectée à un problème ou à une tâche. Les projets, portfolios ou programmes ne peuvent pas avoir d’affectations.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assignments]</td> 
   <td> <p>Dans un rapport de [!UICONTROL Task] ou de [!UICONTROL Issue], ce champ affiche la liste de toutes les entités (utilisateurs et utilisatrices, fonctions, équipes) affectées à la tâche ou au problème. Vous pouvez filtrer selon ce champ à l’aide des champs [!UICONTROL Assignment Users] et [!UICONTROL Assignment Roles]. Vous pouvez filtrer selon l’équipe affectée à la tâche ou au problème à l’aide du champ Équipe. Vous ne pouvez pas regrouper un rapport en fonction de ce champ.</p> <p>Les éléments de travail qui ont été placés dans la [!UICONTROL Recycle Bin] continueront à s’afficher dans certains rapports qui font référence à l’objet [!UICONTROL Assignment] dans lequel un modificateur de filtre [!DNL OR] est utilisé.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assignment Roles]</td> 
   <td>
   <p>Dans un rapport de [!UICONTROL Task] ou de [!UICONTROL Issue], ce champ affiche des informations sur les fonctions affectées aux tâches ou problèmes. Ce champ affiche les [!UICONTROL Primary Owners], ainsi que d’autres fonctions affectées à des tâches ou à des problèmes.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assignment Status]</td> 
   <td> <p>Dans un rapport d’affectation, de tâche ou de problème, le [!UICONTROL Assignment Status] indique si les personnes affectées à un élément de travail ont cliqué sur le bouton [!UICONTROL Work On It] ou [!UICONTROL Done] pour accepter ou terminer le travail. Il existe les [!UICONTROL Assignment Statuses] suivants :</p> 
    <ul> 
     <li><b>[!UICONTROL Requested]</b> : la personne a été affectée à la tâche ou au problème, mais n’a pas cliqué sur le bouton [!UICONTROL Work On It] pour commencer à travailler.</li> 
     <li><b>[!UICONTROL Working]</b> : la personne a cliqué sur le bouton [!UICONTROL Work On It] et travaille actuellement sur l’élément. </li> 
     <li><b>[!UICONTROL Done]</b> : la personne a cliqué sur le bouton [!UICONTROL Done] et a terminé de travailler sur l’élément. </li> 
    </ul> <p>Pour plus d’informations, voir <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/work-on-it-and-done-buttons-accept-complete-work.md" class="MCXref xref">Vue d’ensemble des boutons [!UICONTROL Work On It] et [!UICONTROL Done]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assignment Teams]</td> 
   <td>
   <p>Dans un rapport de [!UICONTROL Task] ou de [!UICONTROL Issue], ce champ affiche des informations sur les équipes affectées aux tâches ou problèmes. Le champ affiche les [!UICONTROL Primary Owners], ainsi que d’autres équipes affectées à des tâches ou des problèmes. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assignment Users]</td> 
   <td>
   <p>Dans un rapport de [!UICONTROL Task] ou de [!UICONTROL Issue], ce champ affiche des informations sur les utilisateurs et utilisatrices affectés aux tâches ou problèmes. Ce champ affiche les [!UICONTROL Primary Owners], ainsi que d’autres utilisateurs et utilisatrices affectés à des tâches ou des problèmes. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Attribute]</td> 
   <td>Un attribut est une caractéristique d’un objet [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Audit Area]</td> 
   <td> <p>Les audits sont des messages système qui enregistrent une action survenue dans Workfront. Les types d’audit suivants sont enregistrés :</p> 
    <ul> 
     <li>[!UICONTROL Scope Change]</li> 
     <li>[!UICONTROL Attachment Action]</li> 
     <li>[!UICONTROL General Edit]</li> 
     <li>[!UICONTROL Status Change]</li> 
     <li>[!UICONTROL Note]</li> 
     <li>[!UICONTROL Combined Entry]</li> 
     <li>[!UICONTROL Error Entry]</li> 
     <li>[!UICONTROL Status Change]</li> 
     <li>[!UICONTROL Subscription Change]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Audit Trail]</td> 
   <td>Collection de notes générée automatiquement par les événements qui font l’objet d’un suivi par le biais des modifications enregistrées ([!UICONTROL Audit Areas]). Chaque note enregistre qui a fait l’action, ce qui a été fait, et quand cela a été fait.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Automatic And On Change]</td> 
   <td> <p>Un des types [!UICONTROL Project Update]. Cela recalculera la chronologie prévisionnelle et prévue du projet lors de l’exécution du processus de recalcul nocturne et lors de toute mise à jour du projet ou des tâches du projet. </p> <p>Pour plus d’informations, voir <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Sélectionner le type de mise à jour du projet</a>.</p> </td> 
  </tr>

<tr> 
   <td><p>Disponibilité</p></td> 
   <td> <p>Ce terme est utilisé par rapport à la « disponibilité de l’utilisateur ou de l’utilisatrice » ou à la « disponibilité de la ressource » et illustre le temps pendant lequel la ressource (utilisateur ou utilisatrice, ou fonction) est disponible pour travailler. </p> 
   <p>Workfront calcule la disponibilité des utilisateurs et des utilisatrices à l’aide de plusieurs champs et selon les paramètres des préférences de gestion des ressources de votre système. Pour plus d’informations, consultez la section <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configurer les préférences de la gestion des ressources</a>. </p>
   <p>Pour plus d’informations sur la disponibilité des ressources, consultez la section <a href="../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md">Commencer avec la gestion des ressources.</a></p>
   Le terme « capacité » est également utilisé pour désigner la disponibilité des ressources. 
   </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Automatic Only]</td> 
   <td> <p>Un des types [!UICONTROL Project Update]. Les chronologies prévisionnelles et prévues sont de nouveau calculées lorsque le processus de recalcul nocturne s’exécute.</p> <p>Pour plus d’informations, consultez la section <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Sélectionner le type de mise à jour du projet</a>.</p> </td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL BAU]</td> 
   <td>Travail « business as usual » (BAU) qui contribue à la réalisation des principaux objectifs quotidiens de l’entreprise.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Backlog]</td> 
   <td>La zone dans un environnement Agile où les nouveaux problèmes sont conservés jusqu’à ce qu’ils soient prêts à être traités.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Baseline]</td> 
   <td>Source de données par rapport à laquelle mesurer les itérations dans un environnement Agile.</td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL Billable Expense]</td> 
   <td> <p>Dépense marquée comme facturable au client ou à la cliente. Il peut s’agir d’une dépense prévue ou d’une dépense effective.</p> <p>Les champs Coût prévu des dépenses facturables et Coût réel des dépenses facturables peuvent être ajoutés aux vues et aux rapports. Ils n’apparaissent pas sur les pages de détails du projet ou de la tâche.</p>
   <p>Vous trouverez ces champs dans les types de rapports suivants :</p>
   <ul>
   <li>Niveau de référence</li>
   <li>Modèle</li>
   <li>Projet (données financières)</li>
   </ul>
   <p>Pour plus d’informations sur le marquage d’une dépense comme facturable, voir <a href="/help/quicksilver/manage-work/projects/project-finances/manage-project-expenses.md">Gérer les dépenses du projet</a>.</p>
   </td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL Billing Record]</td> 
   <td> <p>Enregistre les revenus, les heures ou les dépenses qui peuvent être facturés. Ces informations peuvent être utilisées pour créer des factures dans un système comptable externe.</p> <p>Pour plus d’informations, consultez la section <a href="../../../manage-work/projects/project-finances/create-billing-records.md">Créer des enregistrements de facturation</a>. </p> 
   </td> 
  </tr>

<tr> 
   <td>Statut de l’enregistrement de facturation</td> 
   <td> <p>Dans un rapport sur les enregistrements de facturation ou les heures, le statut d’un enregistrement de facturation indique si celui-ci a été facturé ou non. La suppression d’un projet ou la modification du nombre d’heures liées à un enregistrement de facturation Facturé est impossible. Pour plus d’informations, consultez la section <a href="../../../manage-work/projects/project-finances/create-billing-records.md" >Créer des enregistrements de facturation</a>.</p>  
   </td> 
  </tr>


<tr> 
   <td>[!UICONTROL Branding]</td> 
   <td><p>Processus de personnalisation [!DNL Workfront] pour donner à l’interface l’apparence de votre entreprise en utilisant vos couleurs et logos.</p><p><strong>NOTE</strong><br> : si votre entreprise a été intégrée à [!DNL Adobe Experience Cloud], le branding n’est pas disponible.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Breadcrumbs]</td> 
   <td> <p>Zone située en haut de la page qui indique l’emplacement hiérarchique de l’utilisateur ou de l’utilisatrice dans l’application.</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Pour plus d’informations, consultez la section <a href="../../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md" class="MCXref xref">Vue d’ensemble des chemins de navigation</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Budget Status]</td> 
   <td> <p>Ce champ est obsolète. Toute information que ce champ peut afficher est liée à une fonctionnalité supprimée par [!DNL Workfront] et le champ ne peut pas être mis à jour. </p> <p>Ce champ indique si le projet a été ajouté au [!UICONTROL Capacity Planner] et si le calcul du budget est terminé. Le [!UICONTROL Capacity Planner] a été supprimé de [!DNL Workfront]. </p> 
    <ul> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">If the project is  not added to the capacity planner, its value is <i>Not Included</i>.  </li>
     --> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">If the project is  added to the Capacity Planner but is excluded from the budget calculation,  the value is <i>Included but not Calculated</i>.  </li>
     --> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> If the project is  added to the Capacity Planner and included in the budget calculation, the value is <i>Included and Calculated</i>. </li>
     --> 
    </ul> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Breakdown]</td> 
   <td> <p>Dans Workfront Planning, vous pouvez afficher les enregistrements connectés dans la vue chronologique d'un enregistrement à l'aide de la fonction Répartition. </p>
   <p>La répartition des enregistrements en fonction de leurs connexions vous permet d'afficher la chronologie d'autres enregistrements connectés et de comprendre comment ils peuvent affecter les performances et les échéances de vos enregistrements. </p>
   <p>Les enregistrements connectés s’affichent imbriqués sous leur enregistrement respectif. </p>
   <p>Pour plus d’informations, consultez <a href="/help/quicksilver/planning/views/manage-the-timeline-view.md">Gérer la vue chronologique</a>. </p>
   </td> 
    </tr>

<tr> 
   <td>[!UICONTROL Budgeted Completion Date]</td> 
   <td> <p>Ce champ est obsolète. Toute information que ce champ peut afficher est liée à une fonctionnalité supprimée par [!DNL Workfront]. Ce champ ne peut pas être mis à jour. </p>
   <p> Ce champ est toujours visible dans les rapports et listes de [!UICONTROL project].</p>  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Budgeted Cost]</td>

<td> <p>Il s’agit du coût associé aux ressources de budget pour un projet. </p>
   <p>Le champ s’affiche dans les zones suivantes de [!DNL Workfront] sous les noms suivants :</p>
   <ul>
   <li><strong>[!UICONTROL Budgeted Cost]</strong> : dans le panneau [!UICONTROL Business Case Summary]</li>
   <li><strong>[!UICONTROL Cost]</strong> : dans les zones d’[!UICONTROL Utilization] lors de l’affichage des informations par [!UICONTROL Cost]</li>
   <li><strong>[!UICONTROL Project Budgeted Cost]</strong> : dans les listes et les rapports</li>
   </ul>   
    <p>Le [!UICONTROL Budgeted Cost] du projet est calculé à l’aide de la formule suivante :</p> 
    <p><code>[!UICONTROL Project Budgeted Cost] (or [!UICONTROL Budgeted Cost]) = [!UICONTROL Budgeted Expense Cost] + [!UICONTROL Budgeted Labor Cost] + [!UICONTROL Fixed Cost] of the project</code> </p> 
    <p>Pour plus d’informations sur le calcul du [!UICONTROL Budgeted Cost] et pour comprendre les différents noms de ce concept dans [!DNL Workfront], consultez la section <a href="../../../manage-work/projects/project-finances/budgeted-cost.md" class="MCXref xref">Calculer le coût budgété du projet</a>. </p>
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Budgeted Hours]</td> 
   <td> <p>Heures budgétées pour le travail que les ressources doivent accomplir dans le cadre des projets. Ce champ fait référence aux heures budgétées dans la zone [!UICONTROL Resource Budgeting] du [!UICONTROL Business Case] (ou dans le [!UICONTROL Resource Planner]) pour le projet ou pour les ressources du projet.</p> <p>Pour plus d’informations, consultez la section <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Comprendre le [!UICONTROL Budgeted Labor Cost] et les [!UICONTROL Budgeted Hours] pour les projets</a>. </p> 
    <!-- 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Hours that were formerly budgeted in the Legacy Resource Estimates area of a project (or in the Capacity Planner)</p>
    <p>Important: This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p>
  -->
    <p> Pour plus d’informations sur la budgétisation des utilisateurs et utilisatrices dans le [!DNL Resource Planner], voir l’article <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Budgéter des ressources dans le [!DNL Resource Planner] à l’aide des vues [!UICONTROL Project] et [!UICONTROL Role]</a>. </p> 
    <p>Les heures budgétées dans la zone [!UICONTROL Resource Budgeting] du [!UICONTROL Business Case] ou du [!UICONTROL Resource Planner] s’affichent dans les zones suivantes de [!DNL Workfront] et avec les noms suivants :</p> 
     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td><strong>Nom d’affichage [!UICONTROL Budgeted Hours]</strong></td> 
        <td><strong>Zones des [!DNL Workfront]</strong></td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Hours]</td> 
        <td>Zone [!UICONTROL Resource Budgeting] du [!UICONTROL Business Case]</td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL BDG]</td> 
        <td>[!UICONTROL Resource Planner] vu par [!UICONTROL Hours]</td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Budgeted Hours]</td> 
        <td> <p>Vue des [!UICONTROL Hours] du rapport d’utilisation</p> <p>Pour plus d’informations sur le rapport d’[!UICONTROL Utilization], voir l’article <a href="../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md" class="MCXref xref">Vue d’ensemble du rapport d’[!UICONTROL Resource Utilization]</a>.</p> </td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Bud. Hours]</td> 
        <td> <p>Rapport d’[!UICONTROL Budgeted Hour]</p><p>L’objet [!UICONTROL Budgeted Hour] du rapport Heure budgétée fait référence à des informations relatives à un outil de gestion des ressources obsolète. Seul le champ « [!UICONTROL Bud. Hours] » de ce rapport fait référence aux heures budgétées dans le [!UICONTROL Resource Planner] ou la zone [!UICONTROL Resource Budgeting] du [!UICONTROL Business Case] du projet. </p> <p>Pour plus d’informations sur la création d’un rapport, voir l’article <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Créer un rapport personnalisé</a>.</p> </td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Resource Planner Budgeted Hours] </td> 
        <td> <p>Mentionnées dans les rapports suivants :</p>
        <ul>
        <li>Rapport de [!UICONTROL Project]
        <li>Rapport de [!UICONTROL Project (Financial Data)]
        <li>Rapport de [!UICONTROL Task]
        <li>Rapport de [!UICONTROL Issue]
        <li>Rapport d’[!UICONTROL Budgeted Hour]</li>
        </ul>
         <p>Pour plus d’informations sur la création d’un rapport, voir l’article <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Créer un rapport personnalisé</a>.</p> </td> 
       </tr> 
      </tbody> 
     </table> 
    <p>Toute autre mention des [!UICONTROL Budgeted Hours] dans [!DNL Adobe Workfront] fait référence aux heures budgétées à l’aide de fonctionnalités obsolètes qui ont été supprimées de Workfront. Il s’agit de champs en lecture seule qui ne sont pas mis à jour avec les informations actuelles lorsque vous utilisez les outils de budget des ressources actuelles. </p>
    <!--<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate the Budgeted Hours from theResource Planner in the areas and reports listed below. </p>
     <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Planner Hours view (in the BDG column)</li>
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Utilization report Hours view</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Budgeting area of the Business Case (in the Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report (the Bud. Hours field refers to hours budgeted for users; the Pln. Bud. Hours field refers to hours budgeted for roles or projects)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report (in the Project: Budgeted Hours field) </li>
        </ul>
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The fields listed below display in the reports listed and are hours formerly budgeted in the  Capacity Planner or the Legacy Resource Estimates area of the Business Case.</p>
         <p>Important: The Capacity Planner and Legacy  Resource Estimates have been removed from Workfront. You cannot update any information that might display in these fields.</p>
        <ul>
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Capacity Planner</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Legacy  Resource Estimates area of the Business Case (in the Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report (in the Bud. Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report (in the Budgeted Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project report (in the Budgeted Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project (Financial  Data) report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Task  report (in the Project: Budgeted Hours field)</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Issue report (in the Project: Budgeted Hours field)</li>
      </ul> --> 
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Budgeted Labor Cost]</td> 
   <td> <p>Il s’agit du coût associé aux heures que vous, en tant que personne responsable des ressources, consacrez à vos fonctions pour le travail qu’elles doivent effectuer sur les projets. </p> <p>Le [!UICONTROL Budgeted Labor Cost] d’un rapport de projet est calculé à l’aide de la formule suivante :</p> <p><code style="font-style: normal;">[!UICONTROL Budgeted Labor Cost] = SUM([!UICONTROL Job Role Cost] per [!UICONTROL Hour] * [!UICONTROL Budgeted Hours] per [!UICONTROL Job Role])</code> </p> <p>Ce champ peut faire référence aux éléments suivants :</p> 
    <ul> 
     <li> <p>Coûts de la main-d’oeuvre affichés dans la zone [!UICONTROL Resource Budgeting] du [!UICONTROL Business Case] ou dans le [!UICONTROL Resource Planner] qui sont associés au coût des fonctions sur un projet. Pour plus d’informations sur le calcul du [!UICONTROL Budgeted Labor Cost], voir l’article <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">[!UICONTROL Understand Budgeted Labor Cost] et les [!UICONTROL Budgeted Hours] pour les projets</a></p> </li> 
     <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>Coûts de la main-d’oeuvre affichés dans la zone [!UICONTROL Resource Budgeting] du [!UICONTROL Business Case] qui reflètent les [!UICONTROL People Costs] estimés dans une initiative liée au projet à partir du [!DNL Scenario Planner] lorsque vous utilisez le planificateur de scénarios pour budgéter les ressources de votre projet. Pour plus d’informations sur les initiatives, voir <a href="../../../scenario-planner/initiatives-overview.md" class="MCXref xref">Vue d’ensemble des initiatives dans le planificateur de scénarios</a>. </p> <p>Le [!DNL Scenario Planner] nécessite une licence supplémentaire. Pour plus d’informations sur le [!DNL Workfront Scenario Planner], voir <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">Vue d’ensemble du [!DNL Scenario Planner]</a>. </p> </li> 
     <p>Il s’affiche dans les zones suivantes sous les noms suivants :</p>
   <ul>
   <li><strong>[!UICONTROL Budgeted Labor Cost]</strong> : dans la zone [!UICONTROL Resource Budgeting] du [!UICONTROL Business Case].
   <li><strong>[!UICONTROL Budgeted Cost]</strong> : dans la vue [!UICONTROL Cost] du rapport d’[!UICONTROL Utilization]
   <p>Pour plus d’informations, voir <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">Afficher des informations sur l’utilisation des ressources</a>.</p>
   <li><strong>[!UICONTROL BDG]</strong> : dans les vues de projet [!DNL Resource Planner] ou [!DNL Role], lors de l’affichage par coût
   <li><strong>[!DNL Resource Planner Budgeted Labor Cost]</strong>: dans les rapports suivants : 
   <ul>
    <li>Rapport de [!UICONTROL Project]</li>
    <li>Rapport de [!UICONTROL Project (Financial Data)]</li>
    <li>Rapport de [!UICONTROL Task]</li>
    <li>Rapport de [!UICONTROL Issue]</li>
    <li>Rapport d’[!UICONTROL Budgeted Hour]</li> 
    </ul>
    <p>Pour plus d’informations sur la création d’un rapport, voir l’article <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Créer un rapport personnalisé</a>.</p>
    <!--
          <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Labor costs for hours budgeted in the Legacy Resource Estimates area of a project (or in the Capacity Planner). This was available only in Adobe Workfront Classic. </p>
           <p>Important: This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p>
       </li> 
    </ul> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate the Budgeted Labor Cost field based on the hours budgeted in the Resource Planner in the following areas and reports in  Workfront: </p>
        <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Planner Cost view (in the BDG column)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Utilization report Cost view (in the Budgeted Cost column)</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Budgeting area of the Business Case </li>
         </ul> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate the Budgeted Labor Cost associated with resources budgeted in the Resource Planner in the Resource Planner Resource Budgeted Cost field in the following reports: </p>
       <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report </li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Task  report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Issue report</li>
         </ul> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate a Budgeted Labor Cost field that contains information from a tool that has been deprecated in the reports listed below. You can no longer update the fields displayed in these reports and budgeting your resources on the projects does not update them: </p>
        <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report </li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Task  report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Issue report</li>
         </ul>      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about calculating the Budgeted Labor Cost, see the article <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Understand Budgeted Labor Cost and Budgeted Hours for projects</a>  .  </p>
    --> 
    </td> 
   </tr> 
   <tr> 
   <td>[!UICONTROL Budgeted Start Date]</td> 
  <td> <p>Ce champ est obsolète. Toute information que ce champ peut afficher est liée à une fonctionnalité supprimée par [!DNL Workfront]. Ce champ ne peut pas être mis à jour.</p>
  <p>Ces zones ont été supprimées de [!DNL Workfront]. </p> 
  <p>Le champ est toujours visible dans les rapports et listes de [!UICONTROL project].</p>
   <!--
   <p>This field shows the date when the budgeting of resources starts, as defined in the Legacy Resource Estimates area of the Business Case of a project, or the Capacity Planner.</p>
   -->   
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Burndown Chart]</td> 
   <td>Graphique en courbes qui fournit une représentation visuelle des tâches terminées et restantes.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Business Case]</td> 
   <td> <p>Outil utilisé pour évaluer si un projet doit être transféré du statut [!UICONTROL Idea] vers le statut [!UICONTROL Planning]. En d’autres termes, un [!UICONTROL business case] permet à l’organisation de décider s’il est utile de lancer et de terminer le projet ou non, en particulier lors de la comparaison de projets avec d’autres dans un portfolio.</p> <p>Pour plus d’informations, voir <a href="../../../manage-work/projects/define-a-business-case/create-business-case.md" class="MCXref xref">Créer un [!UICONTROL Business Case] pour un projet</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Business Case Budgeted Hours]</td> 
   <td> <p>Ce champ est obsolète. Toute information que ce champ peut afficher est liée à une fonctionnalité supprimée par [!DNL Workfront]. Ce champ ne peut pas être mis à jour.</p> <p>Ce champ est toujours visible dans les listes et rapports de [!UICONTROL task] et de projet. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calculated Assignment]</td> 
   <td> <p>Un des [!UICONTROL Duration Types] de la tâche. Cela permet de calculer le pourcentage d’une journée de travail de 8 heures affectée à la tâche par l’utilisateur ou l’utilisatrice, en fonction de la [!UICONTROL Duration] de la tâche et du [!UICONTROL Work Required].</p> <p>Pour plus d’informations, voir <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Vue d’ensemble de la [!UICONTROL Duration] et du [!UICONTROL Duration Type]</a> de la tâche.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calculated Work]</td> 
   <td> <p>Un des [!UICONTROL Duration Types] de la tâche. Cela permet de calculer le [!UICONTROL Work Required] d’une tâche, en fonction de la [!UICONTROL Duration] et des pourcentages de [!UICONTROL Assignment] de l’utilisateur ou de l’utilisatrice (qui sont basés sur une journée de travail de 8 heures).</p> <p>Pour plus d’informations, voir <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Vue d’ensemble de la [!UICONTROL Duration] et du [!UICONTROL Duration Type] de la tâche</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendar]</td> 
   <td> <p>Dans Workfront, un rapport de calendrier est un rapport dynamique dans lequel les utilisateurs peuvent afficher la date et d’autres détails importants d’un événement, y compris la date d’échéance, le statut du travail et l’utilisateur auquel l’événement est affecté.</p> <p> Pour plus d’informations sur les rapports de calendrier, voir <a href="../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md" class="MCXref xref">Vue d’ensemble des rapports de calendrier</a>.</p>
   <p> Dans Workfront Planning, une vue Calendrier est un type d'affichage pour un type d'enregistrement qui affiche des enregistrements dans un calendrier. Vous devez disposer d'une licence supplémentaire pour accéder à Workfront Planning. </p>
    </td> 
  </tr> 
   <tr> 
   <td>[!UICONTROL Can Start]</td> 
   <td> <p>Ce champ indique si une tâche est prête à être démarrée. Lorsque la tâche peut être commencée, le champ[!UICONTROL Can Start] de la tâche est défini sur [!UICONTROL True]. </p> <p>Pour plus d’informations, voir <a href="../../../manage-work/tasks/task-information/can-start-task-overview.md" class="MCXref xref">Vue d’ensemble de « [!UICONTROL Can Start] » pour les tâches</a>.</p> 
   <!--
     <p>(NOTE: everything below is drafted because I created a new article linked above with all this information - it was getting kind of too big for just a table cell)</p>
    --> <!--
     <p>Workfront checks for the following things before it marks a task as True for the Can Start field:<br></p>
    --> 
    <!--
     <ul> 
      <li> If the task has a parent, it checks to see if the value of Can Start for the parent it set to True. If the value for the parent is False, then all the subtasks have the value of Can Start set to False, as well.  </li> 
      <li> It also checks to see if the predecessors of the task as well as the predecessors of their parents are complete. If they are complete, the Can Start value for the task is set to True. If any of the task predecessors or their parents' predecessors are not complete, or have a status of Complete-Pending Approval, then the Can Start value for the task is set to False.  </li> 
     </ul>
    --> 
    <!--
     <p>For information about task predecessors, see <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">Overview of task predecessors</a>.</p>
    --> <!--
     <p>Tip: If the Dependency Type between a task and its predecessors is Start-Start, the predecessor must start before the predecessor relationship is considered resolved and the successor tasks can start. For information about dependency types, see <a href="../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md" class="MCXref xref">Overview of task dependency types</a>. </p>
    --> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Capacity</td> 
    <td>The total availability (measure in either hours or FTE) of a designated user, resource pool, team, rob role, or company.</td> 
   </tr>
  -->

<tr> 
   <td> <p>Capacité</p> </td> 
   <td> <p>Temps disponible d’une ressource lorsqu’elle peut être affectée au travail. Voir « Disponibilité ». </p></td> 
  </tr>

<tr> 
   <td> <p>[!UICONTROL Category]</p> </td> 
   <td> <p>Une catégorie est un formulaire personnalisé. Vous pouvez créer des rapports pour cet objet et les afficher dans d’autres rapports d’objet. Tous les objets ne peuvent pas comporter de formulaire personnalisé ou de catégorie. Les objets suivants peuvent avoir un formulaire personnalisé :<br></p> 
    <ul> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Task]</li> 
     <li>[!UICONTROL Issue]</li> 
     <li>[!UICONTROL Portfolio]</li> 
     <li>[!UICONTROL Document]</li> 
     <li>[!UICONTROL Expense]</li> 
     <li>[!UICONTROL Program]</li> 
     <li>[!UICONTROL User]</li> 
     <li>[!UICONTROL Company]</li> 
     <li>[!UICONTROL Iteration]</li></ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Category Name]</td> 
   <td> <p>Quand vous l’ajoutez comme colonne dans l’affichage de l’un des objets suivants, la liste de tous les formulaires personnalisés liés à ces objets s’affiche :</p> 
    <ul> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Task]<br></li> 
     <li>[!UICONTROL Issue]<br></li> 
     <li>[!UICONTROL Portfolio]<br></li> 
     <li>[!UICONTROL Document]<br></li> 
     <li>[!UICONTROL Expense]<br></li> 
     <li>[!UICONTROL Program]<br></li> 
     <li>[!UICONTROL User]<br></li> 
     <li>[!UICONTROL Company]</li> 
     <li>[!UICONTROL Iteration]</li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Change Management]</td> 
   <td>Un domaine de pratique axé sur la définition, la compréhension et l’adaptation des travaux prévus aux changements des facteurs de portée, de calendrier, de coût et de ressources.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Change Order]</td> 
   <td>Type de problème soulevé dans un projet, décrivant un changement demandé de la portée convenue.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Change Only]</td> 
   <td>L’un des [!UICONTROL Update Types] du projet. Les chronologies [!UICONTROL Project Projected] et [!UICONTROL Planned] sont mises à jour uniquement lorsque des modifications sont apportées aux tâches ou au projet.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Change Order]</td> 
   <td> <p>L’un des types de [!UICONTROL Issue], indique généralement qu’une quantité de travail non prévue doit être effectuée avant que le projet ne soit terminé.</p> <p>Pour plus d’informations sur les types de [!UICONTROL Issue], consultez la section « Types de problèmes par défaut » dans l’article <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md" class="MCXref xref">Personnaliser des types de problèmes par défaut</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Child Task]</td> 
   <td>Tâche qui est une [!UICONTROL Subtask] d’une [!UICONTROL Parent Task] du ([!UICONTROL Summary Task]).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Children]</td> 
   <td>Collection de [!UICONTROL Subtasks] d’une [!UICONTROL Parent Task] du ([!UICONTROL Summary Task]).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Coaching] et [!UICONTROL Training]</td> 
   <td>Modules d’apprentissage, certifications, normes ou communauté de pratique.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Commit]</td> 
   <td>Outil de communication permettant aux utilisateurs et aux utilisatrices de définir les attentes concernant les livrables des tâches.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Commit Date]</td> 
   <td>Outil de communication permettant aux utilisateurs et aux utilisatrices de définir les attentes autour des livrables des tâches.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Communication] et [!UICONTROL Reporting]</td> 
   <td>Normes pour examiner les exceptions et l’intégrité d’un projet, d’un programme ou d’un portfolio</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Company]</td> 
   <td> <p>Une [!UICONTROL Company] est une entité organisationnelle dans [!DNL Workfront]. </p> 
   <p> Vous pouvez associer un utilisateur ou une utilisatrice ou un projet à une seule entreprise. Pour plus d’informations, consultez la section <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md">Créer et modifier des entreprises</a>.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Completion date]</td> 
   <td> <p>Date à laquelle un projet, une tâche ou un problème doit être terminé. Il existe plusieurs types de [!UICONTROL Completion dates] dans [!DNL Workfront] :</p> 
    <ul> 
     <li>[!UICONTROL Actual Completion Date]. Pour plus d’informations, consultez la section <a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref">Vue d’ensemble de la [!UICONTROL Actual Completion Date] du projet </a>.</li> 
     <li>[!UICONTROL Planned Completion Date]. Pour plus d’informations, consultez la section <a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">Définir la [!UICONTROL Planned Completion Date] du projet</a> et <a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Vue d’ensemble de la [!UICONTROL Planned Completion Date] de la tâche</a>.</li> 
     <li>[!UICONTROL Projected Completion Date]. Pour plus d’informations, consultez la <a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">Vue d’ensemble de la [!UICONTROL Projected Completion Date] pour les projets, les tâches et les problèmes</a>.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Completion Day]</td> 
   <td>Le jour, par rapport au début du [!UICONTROL Template], où une [!UICONTROL Template Task] ou un [!UICONTROL Template] est censé arriver à son terme.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Completion Mode]</td> 
   <td> <p>Cela indique comment un projet sera marqué comme [!UICONTROL Complete]. Il peut avoir deux valeurs :</p> 
    <ul> 
     <li>[!UICONTROL Manual] : un utilisateur ou une utilisatrice doit définir le statut du projet sur [!UICONTROL Complete].</li> 
     <li>[!UICONTROL Automatic] : le statut du projet passe automatiquement à [!UICONTROL Complete] lorsque toutes les tâches du projet sont entièrement terminées et que tous les problèmes sont résolus.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Condition]</td> 
   <td> <p>Il s’agit d’une représentation visuelle de la progression d’une tâche, d’un problème ou d’un projet.</p> <p>Pour les projets, la condition peut être définie manuellement par le ou la propriétaire du projet ou automatiquement par [!DNL Workfront], en fonction du statut de la progression du projet. </p> <p>Les valeurs possibles pour la condition du projet sont les suivantes :</p> 
    <ul> 
     <li>[!UICONTROL On Target]</li> 
     <li>[!UICONTROL At Risk]</li> 
     <li>[!UICONTROL In Trouble]</li> 
    </ul> <p>Pour plus d’informations sur les conditions du projet, consultez l’article <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">Vue d’ensemble de la [!UICONTROL Project Condition] et du [!UICONTROL Condition Type]</a>.</p>
     <p>Vous pouvez associer un nombre aux conditions de tâche et de problème pour l’afficher dans les rapports. Les listes ci-dessous affichent les noms et les nombres par défaut des conditions de tâche et de problème. Votre administrateur ou administratrice système peut mettre à jour les noms des conditions et ajouter de nouvelles conditions avec des nombres différents. Une fois qu’un nombre est associé à une condition, il ne peut pas être modifié.  </p> 
     <p>Pour les tâches, la condition est définie manuellement par le ou la propriétaire de la tâche. Les valeurs possibles pour la condition de tâche sont les suivantes :</p> 
    <ul> 
     <li>[!UICONTROL Going Smoothly] (0)<br></li> 
     <li> [!UICONTROL Some Concerns] (1)<br></li> 
     <li>[!UICONTROL Major Roadblocks] (2)</li> 
    </ul> <p>Pour plus d’informations sur les conditions de tâche, consultez l’article <a href="../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md" class="MCXref xref">Mettre à jour la [!UICONTROL Condition] pour les tâches et les problèmes</a>.</p> <p>Pour les problèmes, la condition est définie manuellement par le ou la propriétaire du problème. Les valeurs possibles pour la condition du problème sont les suivantes :<br></p> 
    <ul> 
     <li>[!UICONTROL Going Smoothly] (0)<br></li> 
     <li>[!UICONTROL Some Concerns] (1)<br></li> 
     <li>[!UICONTROL Major Roadblocks] (2)</li> 
    </ul> 
   <p><b>NOTE</b></p>
    <p>Lorsque le champ [!UICONTROL Condition] est suivi dans les rapports [!UICONTROL Journal Entry], les valeurs [!UICONTROL New] et [!UICONTROL Old Number Values] affichent le nombre associé à la condition au lieu de son nom. Si une condition n’est pas définie à l’origine pour une tâche ou un problème et que vous la mettez à jour par la suite, l’entrée du journal qui capture la mise à jour affichera la [!UICONTROL Old Number Value] du champ [!UICONTROL Condition] comme étant de -2,147,483,648. Voir aussi« [!UICONTROL New Number Value] », « [!UICONTROL Old Number Value] », et « [!UICONTROL Journal Entry] » dans cet article. </p> 
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Condition Update]</td> 
   <td> <p>Ce champ présente la condition actuelle des tâches, des projets ou des problèmes. Cette option affiche les mises à jour les plus récentes fournies par les propriétaires des tâches, projets ou problèmes dans le champ [!UICONTROL Update Status], ainsi que la nouvelle condition.</p> <p>Les commentaires effectués sur les mises à jour de condition ne s’affichent pas dans la colonne [!UICONTROL Condition Update] ; seule la mise à jour principale s’affiche.</p> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Types d’enregistrements connectés]</td> 
   <td> <p>Dans Workfront Planning, vous pouvez créer une connexion entre l’un des éléments suivants : </p>
   <ul>
   <li>Deux types d’enregistrements</li>
   <li>Un type d’enregistrement et un type d’objet Workfront</li>
   <li>Un type d’enregistrement et une ressource Adobe Experience Manager</li></ul>
   <p>La connexion de types d'enregistrement permet d'afficher les informations d'un enregistrement ou d'un type d'objet sur un autre.</p>
   <p>Pour plus d’informations, voir <a href="/help/quicksilver/planning/architecture/connect-record-types-overview.md"> Présentation des types d’enregistrements connectés </a>  </p>
  <p>Workfront Planning requiert une licence supplémentaire. </p>
 </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Enregistrements connectés]</td> 
   <td> <p>Dans Workfront Planning, après avoir connecté deux types d'enregistrements, vous pouvez connecter deux enregistrements individuels de ces types l'un à l'autre.  </p>
   <p>La connexion d'enregistrements vous permet d'afficher les informations d'un enregistrement ou d'un objet d'une autre application sur un autre enregistrement.</p>
   <p>Pour plus d’informations, voir <a href="/help/quicksilver/planning/records/connected-records-overview.md">Présentation des enregistrements connectés</a>. </p>

<p>Workfront Planning requiert une licence supplémentaire. </p>
 </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Connections]</td> 
   <td> <p>Dans Workfront Planning, les connexions peuvent faire référence à des types d'enregistrements connectés ou à des enregistrements connectés. Workfront Planning requiert une licence supplémentaire.</p> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Constraint Date]</td> 
   <td> <p>Si vous utilisez une [!UICONTROL Task Constraint] liée à une date spécifique, telle que [!UICONTROL Must Start On], cette date spécifique devient la [!UICONTROL Constraint Date] de la tâche.</p> <p>Les contraintes de tâche suivantes mettent à jour le champ [!UICONTROL Constraint Date] :</p> 
    <ul> 
     <li>[!UICONTROL Must Start On]</li> 
     <li>[!UICONTROL Must Finish On]</li> 
     <li>[!UICONTROL Start No Later Than]</li> 
     <li>[!UICONTROL Start No Earlier Than]</li> 
    </ul> <p><b>CONSEIL</b></p>   
     <ul> 
      <li> <p>Une tâche avec une [!UICONTROL Constraint] de [!UICONTROL Fixed Dates] n’a pas de [!UICONTROL Constraint Date]. </p> </li> 
      <li> <p> La [!UICONTROL Constraint Date] peut être affichée uniquement dans un rapport ou une vue personnalisée.</p> </li> 
     </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Constraint Day]</td> 
   <td> <p>Si vous appliquez une contrainte de tâche à une tâche de modèle qui est associée à une date précise, comme « Doit commencer le », cette date précise devient alors la contrainte de la tâche de modèle.</p> <p>Les contraintes de tâche suivantes mettent à jour le champ [!UICONTROL Constraint Day] :</p> 
    <ul> 
     <li>[!UICONTROL Must Start On]</li> 
     <li>[!UICONTROL Must Finish On]</li> 
     <li>[!UICONTROL Start No Later Than]</li> 
     <li>[!UICONTROL Start No Earlier Than]</li> 
    </ul> <p><b>CONSEIL</b></p> <p>  [!UICONTROL Constraint Day] n’est visible que dans un rapport ou une vue personnalisée. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Constraint Type]</td> 
   <td> <p>La tendance de planification d’une tâche. Par exemple, [!UICONTROL As Soon as Possible] planifiera le début d’une tâche dès que possible, et [!UICONTROL Finish No Later Than] planifiera une tâche pour qu’elle se termine au plus tard à la [!UICONTROL Constraint Date].</p> <p>Pour plus d’informations, consultez la section <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Vue d’ensemble de la [!UICONTROL Task Constraint]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Contextual Menu]</td> 
   <td>Un menu, situé à gauche de l’écran, dans lequel les éléments changent en fonction du contenu actif. Par exemple, lorsqu’un utilisateur ou une utilisatrice consulte un projet, le [!UICONTROL Contextual Menu] affiche les liens vers les informations et les outils liés au projet.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converted Issue Originator]</td> 
   <td>Champ d’un rapport sur les projets ou sur les tâches qui affiche des informations sur l’utilisateur ou sur l’utilisatrice qui est le [!UICONTROL Primary Contact] d’un problème lorsque le problème est converti en projet ou en tâche. Ce champ s’affiche également dans la section [!UICONTROL Project Details] où il indique le nom du [!UICONTROL Primary Contact] du problème converti. Consultez aussi dans cet article la section « [!UICONTROL Primary Contact] ».</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Cost]</td> 
   <td> <p>Le montant à dépenser pour la réalisation d’un projet, d’une tâche ou d’un problème. </p> <p>Vous pouvez suivre différents types de coûts de la main-d’œuvre, des dépenses et les risques liés au projet. Pour plus d’informations sur le suivi des coûts dans [!DNL Workfront], consultez la section <a href="../../../manage-work/projects/project-finances/track-costs.md">Suivre les coûts</a>.</p> 
   </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Cost Performance Index (CPI)]</td> 
   <td> <p>L’[!UICONTROL Cost Performance Index (CPI)] décrit la relation au niveau du projet ou de la tâche entre le coût prévu et le coût réel. Les personnes responsables de projet examinent cette mesure pour identifier les tâches ou les projets qui effectuent actuellement le suivi de sous ou sur-coût à un moment donné. Le coût peut être mesuré en heures ou en devise, selon votre [!UICONTROL Performance Index Method (PIM)].</p> 
    <p> Pour plus d'informations, voir <a href="/help/quicksilver/manage-work/projects/project-finances/calculate-cpi.md">Calculer l'indice Coûts Performance (ICP)</a>.</p>

</td> 
  </tr>

<tr> 
   <td>[!UICONTROL Cost Schedule Performance Index (CSI)]</td> 
   <td> <p>L’[!UICONTROL Cost Schedule Performance Index (CSI)] est un calcul automatique qui combine l’[!UICONTROL Cost Performance Index (CPI)] et l’[!UICONTROL Schedule Performance Index (SPI)] en une mesure générale qui équilibre les coûts et le planning. Si vous multipliez ces valeurs, une seule mesure peut expliquer un planning prolongé à un budget réduit ou vice versa. Les chefs de projet peuvent l’utiliser pour déterminer l’intégrité générale d’un projet ou d’une tâche lorsque le coût est sacrifié pour établir un calendrier à mi-parcours d’un projet.</p> 
    <p> Pour plus d'informations, voir <a href="/help/quicksilver/manage-work/projects/project-finances/calculate-csi.md">Calculer l'indice Coûts Horaire Performance</a>.</p>
    </td> 
  </tr>



<tr> 
   <td>[!UICONTROL Cost Type]</td> 
   <td>Pour une tâche, le [!UICONTROL Cost Type] détermine la manière dont la tâche produira les coûts. Voici quelques exemples : [!UICONTROL Fixed Hourly], [!UICONTROL User Hourly], et [!UICONTROL User Hourly plus Fixed]. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cross-Project Dependencies]</td> 
   <td> <p>Une tâche d’un projet dépend d’une tâche d’un autre projet.</p> <p>Pour plus d’informations, consultez la section <a href="../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md" class="MCXref xref">Créer des projets transversaux antérieurs</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Custom Data]</td> 
   <td> <p>Données propres à une organisation. Les organisations peuvent personnaliser l’application [!DNL Workfront] en créant des formulaires et des champs personnalisés. Ces informations personnalisées peuvent servir à établir des rapports sur les KPI, les audits et la composition de la requête. </p> <p>Les [!UICONTROL Custom Data] peuvent être liées à :</p> 
    <ul> 
     <li>[!UICONTROL Projects]</li> 
     <li>[!UICONTROL Tasks]</li> 
     <li>[!UICONTROL Users]</li> 
     <li>[!UICONTROL Companies]</li> 
     <li>[!UICONTROL Issues]</li> 
     <li>[!UICONTROL Documents]</li> 
     <li>[!UICONTROL Expenses]</li> 
     <li>[!UICONTROL Portfolios]</li> 
     <li>[!UICONTROL Programs]</li> 
     <li>[!UICONTROL Iterations]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custom Data Type]</td> 
   <td>L’option permettant de spécifier si un champ de [!UICONTROL Custom Data] est stocké dans la base de données sous forme de texte, de date, de numéro ou de devise.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custom Display Type]</td> 
   <td>Le type d’affichage d’un champ personnalisé. Par exemple, [!UICONTROL Drop-Down], [!UICONTROL Text Field], [!UICONTROL Text Area], [!UICONTROL Radio Buttons], etc.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custom Field]</td> 
   <td>Parmi les choix disponibles pour l’utilisateur ou l’utilisatrice se trouvent des valeurs de données personnalisées lui offrant la possibilité de sélectionner diverses options. Les options personnalisées sont valides uniquement sur les [!UICONTROL Drop-Down], [!UICONTROL Multi-Select Drop-Down], [!UICONTROL Radio Buttons] et [!UICONTROL Checkboxes].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custom Form Label]</td> 
   <td>Lorsque vous utilisez un type d’affichage personnalisé avec des options personnalisées, il s’agit du texte de l’interface utilisateur qui s’affiche dans le menu déroulant, les cases à cocher ou les cases d’option de cette option personnalisée.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custom Value]</td> 
   <td>Lorsque vous utilisez un champ personnalisé avec des options personnalisées, il s’agit de la valeur qui sera stockée dans la base de données pour une option particulière.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custom View]</td> 
   <td>Définition des champs de données ou des colonnes qui s’affichent pour chaque objet d’une liste.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Customer]</td> 
   <td>Une organisation qui utilise une instance de Workfront.</td> 
  </tr> 
 </tbody> 
</table>

## D - F

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nom de l'objet</th> 
   <th>Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Dashboards]</td> 
   <td> <p> Vous pouvez ajouter ce champ dans un rapport ou dans une vue de l’objet de rapport afin d’afficher les tableaux de bord sur lesquels le rapport est listé. </p> <p> Vous pouvez également utiliser ce champ pour filtrer les rapports listés sur un tableau de bord spécifique. </p> <p> Pour plus d’informations sur l’inclusion des informations des tableaux de bord dans les rapports d’objets de rapport, voir la section « Comprendre les rapports listés sur les tableaux de bord » de l’article <a href="../../../reports-and-dashboards/reports/report-usage/access-organize-reports.md" class="MCXref xref">Accéder aux rapports et organiser les rapports</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data Type]</td> 
   <td>Voir « [!UICONTROL Custom Data Type] ».</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Days Late]</td> 
   <td> <p>Ce champ présente une différence de date entre [!UICONTROL Planned Start] et [!UICONTROL Today] si la [!UICONTROL Actual Completion Date] est manquante.</p> <p>Affiche également une différence de date entre [!UICONTROL Actual Completion] et [!UICONTROL Planned Completion], s’il y a une [!UICONTROL Actual Completion Date].</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Default Schedule]</td> 
   <td> <p>Heures de travail par défaut personnalisables à affecter aux utilisateurs, aux utilisatrices et aux projets au sein d’une organisation. </p> <p>Les horaires sont utilisés pour calculer les dates prévues, de début et d’achèvement des tâches qui sont affectées aux utilisateurs et aux utilisatrices.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Deliverable]</td> 
   <td>Biens ou services quantifiables qui doivent être fournis à la fin d’un projet.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Demand Management]</td> 
   <td>Notation et hiérarchisation des processus d’entrée.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Department Goals]</td> 
   <td>Objectifs propres à un service spécifique qui se concentrent sur l’amélioration des mesures opérationnelles au sein du service.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dependency]</td> 
   <td>Lien entre deux tâches qui nécessitent qu’une tâche change de statut avant que l’autre tâche change également.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dependency Type]</td> 
   <td> <p>Type de relation de planification entre une tâche et ses tâches antérieures. Par exemple, [!UICONTROL Finish-Start], qui nécessite que la première tâche soit Terminée avant que la seconde tâche puisse démarrer.</p> <p>Pour plus d’informations, consultez <a href="../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md" class="MCXref xref">Vue d’ensemble des types de dépendance des tâches</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Document]</td> 
   <td>Tout fichier joint à un objet dans [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Document Version]</td> 
   <td> <p>Chaque fois que le même document est chargé vers le même objet, un numéro de version lui est attribué. Les utilisateurs et les utilisatrices peuvent afficher et modifier plusieurs options pour une version précédente d’un document.</p> <p>Pour plus d’informations, consultez <a href="../../../documents/managing-documents/manage-document-versions.md" class="MCXref xref">Gérer les versions des documents</a>.</p> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Due Date]</td> 
   <td> <p>Date d’échéance d’une tâche ou d’un événement. La date d'échéance d'une tâche ou d'un événement est identique à la date d'achèvement prévue.</p>
    <p>La date d'échéance de la tâche et de l'événement est visible dans les listes et rapports de tâches et d'événements.</p> 
    <p>Voir aussi Date d’achèvement prévue dans ce tableau. 
    </td> 
  </tr>
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Duration]</td> 
   <td> <p>La fenêtre de temps allouée à la réalisation d’une tâche ou d’un projet (déterminée par le nombre de jours entre le [!UICONTROL Planned Start] et la Date d’achèvement prévue).</p> 
    <ul> 
     <li>Pour les tâches, la Durée est un champ modifiable si le Type de durée de la tâche n’est pas Simple. Si le Type de durée de la tâche est Simple ou si la Contrainte de tâche est définie sur Dates fixes, la Durée est un calcul effectué par Workfront.</li> 
     <li>Pour les problèmes, la Durée est toujours un champ modifiable et doit représenter une estimation du nombre de jours nécessaires à la résolution du problème.</li> 
     <li>Pour les projets, la durée est un calcul réalisé par [!DNL Workfront] et représente la différence en jours entre le début planifié de la première tâche et la [!UICONTROL Planned Completion] de la dernière tâche du projet.</li> 
    </ul> <p>Pour plus d’informations sur la différence entre [!UICONTROL Duration] et [!UICONTROL Planned Duration] pour les tâches, consultez l’article <a href="../../../manage-work/tasks/task-information/planned-duration-vs-duration-for-tasks.md">Différence entre [!UICONTROL Planned Duration] et [!UICONTROL Duration] pour les tâches</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Duration in Minutes]</td> 
   <td>Ce champ affiche les mêmes informations que le champ de [!UICONTROL Duration], mais en minutes plutôt qu’en jours. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc,QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Duration per Occurrence]</td> 
   <td> <p>Ce champ s’affiche dans les zones [!UICONTROL Task Details] et [!UICONTROL Edit Task] d’une tâche parent de tâches récurrentes. La durée de chaque tâche récurrente s’affiche. Pour plus d’informations sur la création de tâches récurrentes, consultez la section <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Créer des tâches récurrentes</a>. </p> <p> <span>Les durées modifiées dans des tâches récurrentes individuelles n’affichent pas la valeur indiquée dans ce champ.</span> </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Duration Type]</td> 
   <td> <p>Ce champ de tâche montre comment le travail requis pour terminer la tâche est affecté aux personnes cessionnaires pendant toute la durée de la tâche. Il représente la relation entre la [!UICONTROL Duration] de la tâche, le [!UICONTROL Work Required] et le nombre d’heures, ou l’[!UICONTROL Allocation], que les ressources affectées doivent consacrer à la tâche pour la mener à bien. </p> <p>Ce champ apparaît dans l’onglet [!UICONTROL Details] d’une tâche. </p> <p>Les options pour le type de durée d’une tâche sont les suivantes :</p> 
    <ul> 
     <li>[!UICONTROL Calculated assignment]</li> 
     <li>[!UICONTROL Calculated Work]</li> 
     <li>[!UICONTROL Effort Driven]</li> 
     <li>[!UICONTROL Simple]</li> 
    </ul> <p>Pour plus d’informations, consultez la section <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Vue d’ensemble de la [!UICONTROL Duration] et du [!UICONTROL Duration Type] </a>.</p> 
    —&gt; </td> 
   </tr> 
   <tr> 
   <td>[!UICONTROL Duration Unit]</td> 
   <td>Unité utilisée pour mesurer le temps dans une recherche avancée.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Effort Driven]</td> 
   <td>Relation entre le nombre d’utilisateurs et d’utilisatrices et le temps nécessaire à l’exécution de la tâche. La durée totale prévue pour terminer la tâche diminue à mesure que vous ajoutez d’autres utilisateurs et utilisatrices, mais la durée de la tâche reste la même. En prenant pour exemple une tâche telle que décortiquer un tonneau de cacahuètes, l’ajout de personnes supplémentaires réduira le temps prévu, mais la durée en jours-personnes restera la même.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Elapsed Time]</td> 
   <td> <p>[!UICONTROL Elapsed time] est une unité de temps pour la [!UICONTROL Duration] d’une tâche. Il s’agit du temps écoulé entre la [!UICONTROL Planned Start Date] et la [!UICONTROL Planned Completion Date] d’une tâche, y compris les jours fériés, les week-ends et les congés. En d’autres termes, le temps écoulé est le nombre de jours calendaires écoulés. </p> <p>[!DNL Workfront] prend en charge les unités de temps écoulé suivantes pour la durée de la tâche :</p> 
    <ul> 
     <li> <p>[!UICONTROL Elapsed Minutes]</p> </li> 
     <li> <p>[!UICONTROL Elapsed Hours]</p> </li> 
     <li> <p>[!UICONTROL Elapsed Days]</p> </li> 
     <li> <p>[!UICONTROL Elapsed Weeks]</p> </li> 
     <li> <p>[!UICONTROL Elapsed Months]</p> </li> 
    </ul> <p>Pour plus d’informations sur la durée de la tâche, y compris le temps écoulé, consultez la section <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Vue d’ensemble de la [!UICONTROL Duration] et du [!UICONTROL Duration Type]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL End Date]</td> 
   <td> <p> Il s’agit, dans un rapport sur les [!UICONTROL Rate], de la date de fin de validité d’un nouveau taux de facturation pour une fonction au niveau du projet. Pour calculer les revenus du projet, les heures associées au projet qui se trouvent avant cette date sont multipliées par ce taux de facturation. </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Engagement]</td> 
   <td>L’[!UICONTROL Work Performance Indicator] (WPI) indique le déclin de l’engagement et de la confiance envers la tâche, le projet, l’équipe ou l’organisation. Il vous indique qu’il faut raviver cette confiance et cet engagement. Le WPI est mesuré en posant les questions simples suivantes : « Avez-vous compris ce que l’on attendait de vous ? Le travail qui vous a été confié a-t-il fait progresser l’organisation ? Avez-vous fait du bon travail ? »</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Enterprise Goals]</td> 
   <td>Objectifs interfonctionnels qui contribuent aux mesures des objectifs de l’entreprise.</td> 
  </tr>

<tr> 
   <td>[!UICONTROL Estimate at Completion]</td> 
   <td><p>En tant que mesure de performances du projet, l'Estimation à l'achèvement représente le coût total projeté de votre projet ou tâche une fois qu'il est terminé.</p>
   <p>En tant que paramètre de projet, il vous permet de définir comment la valeur CRE doit être calculée.</p>
   <p>Pour plus d'informations, voir <a href="/help/quicksilver/manage-work/projects/project-finances/calculate-eac.md">Calculer l'estimation à l'achèvement (CRE)</a>. </p>
   </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Estimated Due Date]</td> 
   <td>Dans les rapports de projet, de tâche et d'événement, l'Échéance estimée correspond à la date à laquelle Workfront estime que l'élément doit être terminé.</td> 
  </tr>


<tr> 
   <td>[!UICONTROL Event]</td> 
   <td>Toute modification dans un projet ou une tâche.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Event Handler]</td> 
   <td>Tâches automatisées survenant lorsque des événements se produisent. Une notification électronique automatisée en est un bon exemple.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Event notification]</td> 
   <td>E-mail généré à partir d’un gestionnaire d’événements.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Expenses]</td> 
   <td>Coût des tâches ou des projets non lié à la main d’œuvre.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL External]</td> 
   <td> <p>En règle générale, il s’agit d’un type de licence, ou d’un utilisateur ou d’une utilisatrice disposant d’une telle licence. Un utilisateur ou une utilisatrice disposant de ce type de licence peut uniquement consulter les informations du système. Cela ne permet pas de participer activement au travail.</p> <p>Pour plus d’informations, consultez la vue d’ensemble des licences <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL External System]</td> 
   <td>Tout service ou logiciel stocké et géré en dehors du système d’enregistrement désigné.</td> 
  </tr>

<tr> 
   <td>[!UICONTROL Field]</td> 
   <td><p>Tout objet Workfront ou les informations qui lui sont associées, telles qu’elles apparaissent dans la base de données. </p>
   <p>Par exemple, « projet », « utilisateur ou utilisatrice » et « heure » sont à la fois des objets Workfront et des champs. « Nom », « statut », « propriétaire » et « date de début » sont des champs Workfront associés aux objets ci-dessus. </p>

<p>En ce qui concerne les objets, les termes « objets » et « champs » peuvent être interchangeables.</p>
   <p>Dans le cadre de la création de rapports, les « champs » se rapportent aux objets ou aux informations sur l’objet que vous souhaitez capturer dans le rapport.</p>

<p><b>NOTE</b></p>

<p>Dans les rapports de type texte, les champs font référence aux objets ou à leurs informations tels qu’ils apparaissent dans la base de données.</p>
   <p>Il arrive que le nom affiché dans l’interface utilisateur soit différent du nom du champ de la base de données. Par exemple, « problème » est le nom de l’objet dans l’interface de Workfront, mais « opTask » est le nom de l’objet (ou du champ) dans la base de données Workfront. </p> 
   <p> Il est important d’utiliser le champ tel qu’il apparaît dans la base de données lors de l’écriture d'un rapport en mode texte, d’une vue, d’un filtre, d’un regroupement ou lors de la création d'un champ calculé.</p>

<p>Pour plus d’informations, consultez <a href="../../../wf-api/general/api-explorer.md">Explorateur d’API</a> et <a href="../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md">Vue d’ensemble du mode texte</a>.</p>

<p>Par défaut, Workfront est fourni avec un ensemble de champs qui définissent les objets et leurs informations. Vous pouvez également créer des champs personnalisés pour définir des objets, mais vous ne pouvez pas créer d’objets personnalisés.</p>

<p>Dans Workfront Planning, vous pouvez créer des champs personnalisés pour tous les types d’enregistrements. Les types d’enregistrements Workfront sont fournis avec un nombre très limité de champs. Vous devez créer tous les champs à partir de zéro et les associer à des types d’enregistrements. Pour plus d’informations, voir <a href="/help/quicksilver/planning/fields/fields-overview.md">Présentation des champs</a>. </p> <p>Workfront Planning requiert une licence supplémentaire. </p>   
  </tr>
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Filter]</td> 
   <td> <p>Un des principaux blocs de création d’un rapport ou d’un élément de liste qui définit les informations affichées à l’écran. Pour plus d’informations sur les éléments de création de rapports, consultez <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">Éléments de rapport : filtres, vues et regroupements</a>.</p> <p>Le filtre détermine les résultats qui s’affichent dans un rapport ou dans la liste des panneaux [!DNL Workfront], comme les projets, les tâches ou les problèmes.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Financial Work Management]</td> 
   <td>Traitement des données sur les coûts, les dépenses et les revenus liés à la main-d’œuvre dans [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fixed Cost]</td> 
   <td>Vous pouvez définir un montant fixe de coût pour un projet. Il fait partie du [!UICONTROL Planned Cost] du projet, qui représente le montant dont vous avez besoin pour terminer le projet. Pour plus d’informations sur les coûts, consultez <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Suivre les coûts</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fixed Revenue]</td> 
   <td>Vous pouvez définir un montant fixe des revenus pour un projet. Il fait partie des [!UICONTROL Planned Revenue] du projet, qui représente le montant que vous pourriez obtenir si vous terminez le projet. Pour plus d’informations sur les revenus, consultez <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Vue d’ensemble de la facturation et du revenu</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Flags]</td> 
   <td> <p> Il s’agit du même champ que [!UICONTROL Status Icons], mais il est disponible uniquement pour les vues suivantes : </p> 
    <ul> 
     <li> [!UICONTROL Templates] </li> 
     <li> [!UICONTROL Expenses] </li> 
    </ul> <p> Pour plus d’informations, consultez l’article <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">Icônes de statut intégrées dans les vues</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder]</td> 
   <td>Les dossiers permettent d’organiser les documents ou les rapports associés à un objet.</td> </tr>
  <tr>
  <td>[!UICONTROL FTE] (Full Time Equivalent)</td> 
   <td>Il s’agit de l’équivalent temps complet qui indique la durée de disponibilité d’une ressource pour le travail.
   Le champ [!UICONTROL FTE] s’affiche dans les zones suivantes : 
  <ul>
   <li> Profil de l’utilisateur ou de l’utilisatrice, lors de la modification ou de la création de l’utilisateur ou de l’utilisatrice </li>
   <li> [!UICONTROL Resource Planner] </li>
   <li> [!UICONTROL Scenario Planner] (nécessite une licence supplémentaire pour le planificateur de scénarios Workfront) </li>
   <li> Listes et rapports d’utilisateur et utilisatrice </li> </ul>

<p>L’[!UICONTROL FTE] doit être un nombre décimal maximum de 1 et ne peut pas être égal à 0. </p>
   <p> Un [!UICONTROL FTE] de 1 (qui est la valeur par défaut du champ [!UICONTROL FTE] d’un utilisateur ou d’une utilisatrice, tel que défini dans son profil) signifie qu’une ressource (utilisateur ou utilisatrice, ou rôle) accomplit le nombre entier d’heures en fonction du planning qui calcule sa disponibilité. </p>
   <p>Votre équipe d’administration Workfront décide du planning à utiliser pour déterminer la disponibilité de l’utilisateur ou utilisatrice.  </p>
   <ul>
   <li> Lorsque le [!UICONTROL Default Schedule] est utilisé, Workfront utilise l’[!UICONTROL FTE] de l’utilisateur ou de l’utilisatrice figurant dans son profil pour calculer la disponibilité. </li>
   <li> Lorsque le planning de l’utilisateur ou de l’utilisatrice est utilisé, Workfront utilise ses congés, la valeur [!UICONTROL Work Time] et les heures du [!UICONTROL Default Schedule] pour calculer l’[!UICONTROL FTE] de l’utilisateur ou de l’utilisatrice. </li> </ul>

<p>Pour plus d’informations, voir <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configurer les préférences de gestion des ressources</a>.  </p>
   <p>Pour plus d’informations sur la création de plannings dans [!DNL Workfront], voir <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md">Créer un planning</a>. </p>

<p><b>NOTE</b></p>
   <p>Pour tous les calculs dans le [!UICONTROL Scenario Planner], Workfront utilise la valeur suivante : 1 [!UICONTROL FTE] = 8 heures.</p>
   <p>Pour plus d’informations, voir <a href="../../../scenario-planner/get-started-with-scenario-planning.md">Commencer avec le [!UICONTROL Scenario Planner]</a>. </p>
   </td> </tr> 
   </tbody> 
   </table>

<!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Task field used by the planner to set how the work required is allocated to the assignees across the duration.</p>
<!--
FTE
The designated full time equivalency for users. A full-time user should have 100% FTE and part-time user should have a percentage that equals their working hours. 
-->

## G - I

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nom de l'objet</th> 
   <th>Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Gantt Chart]</td> 
   <td> <p>Chronologie visuelle des dates du projet dans une vue Calendrier basée sur les dates prévues ou prévisionnelles au fur et à mesure que les tâches du projet sont planifiées.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Goal]</td> 
   <td><p>Il existe deux concepts liés aux objectifs dans [!DNL Workfront] : </p> 
    <ul> 
     <li> <p><b>Objectifs du projet</b> : ensemble d’objectifs commerciaux convenus par les parties prenantes d’un projet. Les objectifs du projet font partie du business case d’un projet. </p> <p>Vous ne pouvez pas afficher les objectifs du projet dans des listes ou des rapports, mais vous pouvez y accéder via l’API. </p> <p>Pour plus d’informations sur les objectifs du projet de business case, voir <a href="../../../manage-work/projects/define-a-business-case/create-business-case-goals.md">Créer des objectifs de business case</a>. </p> </li> 
     <li> <p><b>Objectifs stratégiques</b> : un objectif stratégique est un objectif que vous créez pour planifier votre stratégie de travail pour une période donnée. Vous pouvez créer ces types d’objectifs en utilisant les [!DNL Workfront Goals]. Votre entreprise doit acheter une licence supplémentaire et vous devez avoir accès à cette fonctionnalité pour pouvoir créer des objectifs stratégiques. [!DNL Workfront Goals] sont disponibles uniquement avec une licence supplémentaire.</p> 
     <p>Pour plus d’informations, voir Vue d’ensemble des <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals]</a>. </p> 
     <p>Vous pouvez afficher les objectifs stratégiques dans un rapport d’objectif ou de projet et y accéder via l’API. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Goal Hierarchy]</td> 
   <td> <p>Dans les rapports d’[!UICONTROL Goal] et de [!UICONTROL Project], il s’agit d’un champ de collection qui affiche les objectifs dans la hiérarchie à laquelle un objectif stratégique appartient lorsqu’il s’aligne sur d’autres objectifs. Les objectifs sont séparés par un délimiteur ▸. </p> <p>Seuls les parents de l’objectif et l’objectif s’affichent dans ce champ. Les objectifs enfants ne s’affichent pas. </p> <p>Pour plus d’informations sur l’alignement des objectifs dans [!DNL Workfront Goals], voir <a href="../../../workfront-goals/goal-alignment/goal-alignment-overview.md">Vue d’ensemble de l’alignement des objectifs dans les [!DNL Workfront Goals]</a>. </p> 
   <p>Ce champ n’est visible que si votre entreprise a acheté [!DNL Workfront Goals]. Pour plus d’informations sur la gestion des objectifs stratégiques à l’aide des [!DNL Workfront Goals], voir Vue d’ensemble des <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals]</a>. </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Goal Success Score]</td> 
   <td> Dans un rapport de [!UICONTROL Project], ce champ est utilisé pour faire référence aux objectifs au niveau du projet associés au [!UICONTROL Business Case]. Actuellement, il s’agit d’un champ obsolète qui n’est associé à aucune fonctionnalité.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Goals] </td> 
   <td> <p>Dans un rapport de [!UICONTROL Project], il s’agit d’un champ de collection qui affiche tous les objectifs stratégiques associés à un projet. Les objectifs sont séparés par des virgules.</p> <p>Ce champ n’est visible que si votre entreprise a acheté [!DNL Workfront Goals]. Pour plus d’informations sur la gestion des objectifs stratégiques à l’aide des [!DNL Workfront Goals], voir Vue d’ensemble des <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals]</a>. Pour plus d’informations sur les objectifs stratégiques et les objectifs de projet dans [!DNL Workfront], voir « [!UICONTROL Goal] » dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Global Interface Preferences]</td> 
   <td>Paramètres de l’interface qui affectent tous les utilisateurs et utilisatrices. Les [!UICONTROL Global Interface Preferences] peut être remplacées par les [!UICONTROL User Interface Preferences].</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Group]</td> 
   <td> <p>Collection d’utilisateurs et utilisatrices (provenant éventuellement du même service ou unité opérationnelle) ayant accès aux mêmes objets. Outre les utilisateurs et utilisatrices, les groupes peuvent être associés à des portfolios, des programmes, projets,<span> modèles de projet,</span> entreprises, équipes, plannings, modèles de mise en page et profils de feuille de temps.</p> <p>Vous pouvez également accorder des autorisations aux objets par groupe. Pour plus d’informations, voir <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Vue d’ensemble des groupes</a>.</p> <p>Dans une liste ou un rapport d’objets de l’un des types suivants, vous pouvez utiliser le champ [!UICONTROL Group] pour répertorier les objets de ce type associés à un groupe particulier : utilisateur ou utilisatrice, portfolio, programme, projet, <span>modèle de projet</span>, entreprise, équipe, planning, modèle de mise en page ou profil de feuille de temps.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Group Administrator]</td> 
   <td> <p>Personnes qui gèrent les objets, l’accès, et utilisateurs et utilisatrices de groupes désignés.</p> <p> Dans un rapport de [!UICONTROL Group], ce champ affiche les noms des utilisateurs et utilisatrices désignés comme [!UICONTROL Group Administrators] dans le groupe. Pour plus d’informations sur les administrateurs et administratrices de groupe, voir <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administrateurs et administratrices de groupe</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Group with Administration Access]</td> 
   <td> <p> Dans un [!UICONTROL Layout Template], un [!UICONTROL Timesheet Profile] ou un [!UICONTROL Schedule report], ce champ affiche les groupes auxquels les administrateurs et administratrices de groupe ont un accès en modification du modèle. Vous pouvez également filtrer ce rapport selon ce champ. </p> <p> Pour plus d’informations, voir <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Créer et gérer des modèles de mise en page</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Grouping]</td> 
   <td> <p>Élément de rapport utilisé pour classer les informations d’une liste selon un critère commun.</p> <p>Pour plus d’informations, voir la section « [!UICONTROL Groupings] » de l’article <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">Éléments de création de rapports : filtres, vues et regroupements</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Handoff Date]</td> 
   <td> <p>Date à laquelle une tâche devient disponible pour le travail. La [!UICONTROL Handoff Date] est un calcul qui ne peut pas être défini manuellement. <br>Pour plus d’informations sur la [!UICONTROL Handoff Date], voir l’article <a href="../../../manage-work/tasks/task-information/handoff-task-date.md" class="MCXref xref">Vue d’ensemble de la [!UICONTROL Task Handoff Date]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Help Desk]</td> 
   <td>Autre nom pour décrire la zone [!UICONTROL Requests] de [!DNL Workfront]. Vous pouvez utiliser la zone [!UICONTROL Requests] pour traiter les tickets d’assistance clientèle, les demandes de projet, les tickets du centre d’assistance, etc.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Owner]</td> 
   <td>Dans un rapport d’[!UICONTROL Hour], la personne [!UICONTROL Owner] est la personne à qui les heures sont attribuées. Différent de l’utilisateur ou de l’utilisatrice qui consigne réellement les heures. Ces deux entités peuvent parfois être deux personnes différentes. <br>Pour plus d’informations sur la consignation des heures d’un autre utilisateur ou d’une autre utilisatrice, voir l’article <a href="../../../timesheets/create-and-manage-timesheets/log-time.md" class="MCXref xref">Enregistrer des heures</a>.</td> 
  </tr>

<tr> 
   <td>Statut d'heure</td> 
   <td> <p>Attribut défini par Workfront pour les heures effectives que les utilisateurs et utilisatrices consignent pour les tâches, les problèmes ou les projets. </p>

Dans Workfront, les entrées d’heures peuvent avoir l’un des statuts suivants :
<ul>
   <li><b>Envoyées</b> : les heures ont été consignées sur un projet, une tâche ou un problème. Elles font partie d’un enregistrement de facturation ou ne sont pas encore ajoutées à un enregistrement de facturation.</li>
   <li><b>Approuvées</b> : les heures ont été enregistrées et elles ont été approuvées par la personne propriétaire du projet. Elles font partie d’un enregistrement de facturation ou ne sont pas encore ajoutées à un enregistrement de facturation.</li> 
   <li><b>Non approuvées</b> : les heures ont été enregistrées et rejetées par la personne propriétaire du projet. Elles font partie d’un enregistrement de facturation ou ne sont pas encore ajoutées à un enregistrement de facturation.</li>
   <li><b>Facturées</b> : les heures ont été consignées, ajoutées à un enregistrement de facturation et le statut de l’enregistrement de facturation a été marqué comme Facturé. Elles n’avaient pas besoin d’être approuvées par la personne propriétaire du projet.</li>
   <li><b>Facturées et approuvées</b> : les heures ont été consignées, approuvées par la personne propriétaire du projet et le statut de l’enregistrement de facturation a été marqué comme Facturé.</li>
   </ul>

<p>Lorsque les heures font partie d’un enregistrement de facturation, le statut des heures indique si elles ont été approuvées ou si l’enregistrement de facturation auquel elles appartiennent a été facturé. Le statut d’une entrée d’heure n’est visible que dans une liste ou un rapport d’heures. </p>

<p>Pour plus d’informations sur l’ajout d’heures à des enregistrements de facturation, voir la section « Ajouter des heures à des enregistrements de facturation » dans l’article <a href="../../../manage-work/projects/project-finances/create-billing-records.md" >Créer des enregistrements de facturation</a>.</p>

<p>Pour plus d’informations sur l’approbation des heures passées sur les projets, voir <a href="../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md" >Solliciter l’approbation d’heures pour un projet</a>.</p>

<p><b>CONSEIL</b></p>

<p>Les heures générales qui ne sont pas consignées directement sur des éléments de travail n’affichent pas le statut d’heure. </p> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Hour Type]</td> 
   <td> <p>Attribut pouvant être défini pour les heures effectives que les utilisateurs et utilisatrices consignent pour les tâches, problèmes ou projets. Il s’agit également d’un attribut pour les heures consignées qui ne sont pas directement liées au travail, telles que [!UICONTROL Vacation] et [!UICONTROL Time Off].</p> <p>Pour plus d’informations, voir <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md" class="MCXref xref">Gérer les types d’heures</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td> <p>L’identifiant est un indicateur alphanumérique associé à chaque objet dans [!DNL Workfront]. Il identifie de manière unique chaque objet dans la base de données [!DNL Workfront]. Vous pouvez voir l’identifiant de n’importe quel objet présent dans un rapport ou une liste. </p> <p><b>CONSEIL</b></p>   <p>Vous pouvez également voir l’identifiant dans l’URL de la page de l’objet. Par exemple, l’identifiant d’un projet peut ressembler au nombre surligné dans l’URL suivante, lorsque vous accédez à la page [!UICONTROL Project Details] :</p> <p><code>https://&lt;your domain>.my.workfront.com/project/<b>5e29c8010027d8eb334762d4fff3ffca</b>/overview</code> </p> </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL IMS]</td> 
   <td>Système Identity Management. Adobe IMS exige que vous vous connectiez à Workfront via Adobe plutôt que d’utiliser votre nom d’utilisateur et votre mot de passe Workfront.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Individual Goals]</td> 
   <td>Objectifs individuels qui contribuent aux mesures des objectifs de l’équipe, sans rapport avec le développement personnel ou professionnel.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Inherited Access]</td> 
   <td>Fonction de partage qui accorde l’accès permettant de propager un objet à un autre. Par exemple, l’accès hérité de l’utilisateur ou de l’utilisatrice du projet défini dans les enregistrements de programme et de portfolio.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Initiative]</td> 
   <td> <p>Dans le [!DNL Workfront Scenario Planner], vous pouvez diviser un plan en plusieurs initiatives pour faciliter la gestion du plan. <span>Vous pouvez créer un rapport d’[!UICONTROL Initiative] et accéder aux informations d’[!UICONTROL Initiative] dans un rapport de [!UICONTROL Project].</span></p> <p>Le [!DNL Scenario Planner] nécessite une licence supplémentaire. Pour plus d’informations sur le [!DNL Workfront Scenario Planner], voir <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">Vue d’ensemble du [!DNL Scenario Planner]</a>. </p> <p>Le rapport d’[!DNL Initiative] n’est pas visible dans votre instance [!DNL Workfront] à moins que votre entreprise n’ait acheté une licence [!DNL Workfront Scenario Planner]. Vous ne pouvez pas accéder aux [!UICONTROL Initiatives] par le biais de l’API.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Initiative Job Role]</span> </td> 
   <td> <p><span>Le type de rapport [!UICONTROL Initiative Job Role] affiche des informations sur les fonctions associées à une initiative de plan dans le [!DNL Workfront Scenario Planner].</span> </p> <p>Le [!DNL Scenario Planner] nécessite une licence supplémentaire. Pour plus d’informations sur le [!DNL Workfront Scenario Planner], voir <a href="../../../scenario-planner/scenario-planner-overview.md">Vue d’ensemble du [!DNL Scenario Planner]</a>. </p> <p><span>Ce type de rapport n’est pas visible dans votre instance [!DNL Workfront] à moins que votre société n’ait acheté une licence [!DNL Workfront Scenario Planner].</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Initiative Job Role Hours]</span> </td> 
   <td> <p><span> Dans un rapport [!UICONTROL Initiative Job Role], ce champ indique le nombre d’heures associées à une fonction dans une initiative.</span> </p> <p>Le [!DNL Scenario Planner] nécessite une licence supplémentaire. Pour plus d’informations sur le [!DNL Workfront Scenario Planner], voir <a href="../../../scenario-planner/scenario-planner-overview.md">Vue d’ensemble du [!DNL Scenario Planner]</a>. </p> <p>Ce champ et le type de rapport [!UICONTROL Initiative Job Role] ne sont pas visibles dans votre instance [!DNL Workfront] à moins que votre société n’ait acheté une licence [!DNL Workfront Scenario Planner].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Initiative Job Role Count]</td> 
   <td> <p>Dans un rapport [!UICONTROL Initiative Job Role], ce champ indique le nombre de fonctions spécifiques associées à une initiative.</p> <p>Le [!DNL Scenario Planner] nécessite une licence supplémentaire. Pour plus d’informations sur le [!DNL Workfront Scenario Planner], voir <a href="../../../scenario-planner/scenario-planner-overview.md">Vue d’ensemble du [!DNL Scenario Planner]</a>. </p> <p>Ce champ et le type de rapport [!UICONTROL Initiative Job Role] ne sont pas visibles dans votre instance [!DNL Workfront] à moins que votre société n’ait acheté une licence [!DNL Workfront Scenario Planner].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Initiative Last Published Date]</td> 
   <td> <p>Champ dans un rapport [!UICONTROL Initiative], [!UICONTROL Initiative Job Role] et [!UICONTROL Project] qui affiche la date de la dernière publication d’une initiative de plan dans un projet. Vous pouvez publier des initiatives pour créer des projets ou mettre à jour des projets liés aux initiatives.</p> <p>Le [!DNL Scenario Planner] nécessite une licence supplémentaire. Pour plus d’informations sur le [!DNL Workfront Scenario Planner], voir <a href="../../../scenario-planner/scenario-planner-overview.md">Vue d’ensemble du [!DNL Scenario Planner]</a>. </p> <p><span>Pour plus d’informations sur la publication d’initiatives, voir</span><a href="../../../scenario-planner/publish-scenarios-update-projects.md">Publication de scénarios pour créer et mettre à jour des projets dans le [!DNL Workfront Scenario Planner]</a>. Ce champ n’est pas visible dans votre instance [!DNL Workfront] à moins que votre société n’ait acheté une licence [!DNL Workfront Scenario Planner].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Inline Search]</td> 
   <td>Recherche effectuée lors du processus de remplissage d’un formulaire, pour rechercher les entrées possibles pour un champ spécifique.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Interface Setup]</td> 
   <td>Zone de l’application qui permet de définir des vues personnalisées, des filtres, des regroupements, des contrôles de liste, etc.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL Is Company Goal]</p></td> 
   <td> <p>Dans [!DNL goal reports], ce champ affiche une valeur « [!UICONTROL True]/ [!UICONTROL False] » pour chaque objectif stratégique afin d’indiquer si votre organisation est affectée à l’objectif en tant que propriétaire. </p> 
   <p>Ce champ n’est visible que si votre entreprise a acheté [!DNL Workfront Goals]. Pour plus d’informations sur la gestion des objectifs stratégiques à l’aide de [!DNL Workfront Goals], voir Vue d’ensemble de <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals]</a>.</p>
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Issue]</td> 
   <td> <p>Un élément de travail non planifié indiquant généralement qu’un problème empêche la réalisation d’une tâche ou d’un projet. Il est classé et évalué pour déterminer si un effort de travail supplémentaire doit être envisagé.</p> <p>Un [!UICONTROL Issue] peut également être une requête auprès du [!UICONTROL Help Desk]. Les [!UICONTROL Change Orders], [!UICONTROL Requests] et les [!UICONTROL Bugs] sont également des [!UICONTROL Issues].</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Issue Management]</td> 
   <td> <p>Processus et règles régissant la définition des types de problèmes et le processus de routage, de triage ou de trafic associé à chaque type.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Issue Owner]</td> 
   <td>L’équipe ou les utilisateurs et les utilisatrices responsables du triage et de la résolution d’un problème.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Iteration]</td> 
   <td>Période pendant laquelle une équipe produit un ensemble prédéfini de livrables.</td> 
  </tr> 
 </tbody> 
</table>

## J - L

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nom de l'objet</th> 
   <th>Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Job Role]</td> 
   <td> <p>Utilisé pour identifier les fonctions et responsabilités quotidiennes d’un utilisateur ou d’une utilisatrice. Les fonctions peuvent être affectées à des éléments de travail afin d’identifier la compétence requise pour terminer un processus de travail sans l’affecter à un utilisateur ou à une utilisatrice spécifique. </p> <p>Un utilisateur ou une utilisatrice peut avoir plusieurs rôles. Par exemple, graphiste ou consultant/consultante.</p> <p>Pour plus d’informations, consultez la section <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Créer et gérer des fonctions</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL Journal Entry]</p> </td> 
   <td> <p>Un objet pouvant faire l’objet d’un rapport qui vous donne des informations sur les mises à jour du système pour les champs suivis qui apparaissent dans la zone des [!UICONTROL Updates] des projets, des tâches, des problèmes et d’autres objets.</p> <p>Pour en savoir plus, voir <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md" class="MCXref xref">Rapport sur la zone Mises à jour avec un rapport Entrée du journal</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Kanban Flag]</td> 
   <td> <p>Dans un rapport sur les [!UICONTROL Task] ou sur les [!UICONTROL Issue], le champ [!UICONTROL Kanban Flag] affiche le statut de l’indicateur défini sur l’histoire dans le [!UICONTROL Kanban board]. Les valeurs possibles sont [!UICONTROL On Track], [!UICONTROL Ready to Pull] et [!UICONTROL Is Blocked].</p> <p>Pour plus d’informations sur la définition du statut de l’indicateur sur les histoires du [!UICONTROL Kanban story board], consultez l’article <a href="../../../agile/use-kanban-in-an-agile-team/use-flags-on-stories.md" class="MCXref xref">Utiliser des indicateurs sur les histoires du [!UICONTROL Kanban board].</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>KPI</td> 
   <td>Une valeur mesurable qui démontre l’efficacité avec laquelle une entreprise atteint ses principaux objectifs commerciaux.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Lag]</td> 
   <td>Temps qui doit s’écouler après la [!UICONTROL Planned Completion Date] de la tâche antérieure avant que la tâche dépendante ne puisse commencer.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Lag Types]</td> 
   <td> <p>Méthode de calcul du [!UICONTROL Lag]. Il peut s’agir des éléments suivants :</p> 
    <ul> 
     <li>[!UICONTROL Days] (jours ouvrés)</li> 
     <li>[!UICONTROL Calendar Days] (ignorer les jours fériés)</li> 
     <li>[!UICONTROL Percent]</li> 
     <li>[!UICONTROL Day of Week]</li> 
    </ul> <p>Pour en savoir plus, consultez la section <a href="../../../manage-work/tasks/use-prdcssrs/lag-types.md" class="MCXref xref">Vue d’ensemble des types de décalage</a>.</p> </td>
  </tr> 
  <tr> 
   <td>[!UICONTROL Large Thumbnail]</td> 
   <td> <p> Dans une liste ou un rapport de [!UICONTROL Document], une prévisualisation du document s’affiche dans une miniature. </p> <p>Sélectionnez la <strong>[!UICONTROL Large Thumbnail]</strong> pour afficher une miniature de 400 pixels de large dans le rapport.</p> <p>La taille de la miniature s’ajuste lorsque vous modifiez la largeur de la colonne dans une liste ou un rapport.</p> <p>Consultez aussi « [!UICONTROL Thumbnail] » dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Last 10 Viewers]</td> 
   <td> <p>Dans une liste de rapports, ce champ affiche les noms des 10 utilisateurs et utilisatrices maximum qui ont consulté le rapport le plus récemment.<br>Pour en savoir plus sur les informations d’utilisation dans les listes de rapports, consultez l’article <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Afficher l’utilisation du rapport</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Last Condition Note]</td> 
   <td> <p>Ce champ affiche la dernière mise à jour saisie sur un objet par la personne propriétaire de l’objet. Il s’agit de son activité ou de son interaction la plus récente sur un objet.</p> <p>La colonne [!DNL Last Condition Note] est vide si le texte de la dernière note d’un objet a été supprimé. Lorsqu’une nouvelle note est saisie sur l’objet, elle devient la dernière note et s’affiche à nouveau dans la colonne.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Last Finance Update Date]</td> 
   <td>Dans un rapport [!UICONTROL project], ce champ capture la date et l’heure auxquelles les finances du projet ont été calculées et mises à jour pour la dernière fois. Pour plus d’informations sur les finances de projet, consultez <a href="../../../manage-work/projects/project-finances/project-finances-overview-1.md" class="MCXref xref">Vue d’ensemble des finances du projet</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Last Note]</td> 
   <td> <p>Ce champ affiche la dernière mise à jour saisie sur un objet par un utilisateur ou une utilisatrice. Il s’agit de l’activité ou de l’interaction la plus récente sur un objet.</p> <p>La colonne [!UICONTROL Last Note] est vide si le texte de la dernière note d’un objet a été supprimé. Lorsqu’une nouvelle note est saisie sur l’objet, elle devient la dernière note et s’affiche à nouveau dans la colonne.</p>
   <p>Lorsque ce champ est ajouté à un rapport [!UICONTROL Task], les mises à jour restantes sur les objets enfants, tels que les événements, les sous-tâches ou les documents, de la tâche ne s'affichent pas dans cette colonne.</p> 
   <p><b>NOTE</p>
   <p>La dernière note ajoutée à un objet à l’aide de l’API ne s’affiche pas dans un rapport dans Workfront. Le champ [!DNL Last Note] est vide si la dernière mise à jour d’un objet a été ajoutée à l’aide de l’API. </p>

</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Last Viewed By]</td> 
   <td> <p>Dans une liste de rapports, ce champ affiche des informations sur l’utilisateur ou l’utilisatrice qui a consulté le rapport en dernier.<br>Pour plus d’informations sur l’utilisation des listes de rapports, consultez l’article <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Afficher l’utilisation du rapport</a>.<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Last Viewed Date]</td> 
   <td> <p>Dans une liste de rapports, ce champ affiche la date à laquelle le rapport a été affiché en dernier.<br>Pour plus d’informations sur l’utilisation des listes de rapports, consultez l’article <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Afficher l’utilisation du rapport</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Layout Template]</td> 
   <td>Défini par l’administrateur ou l’administratrice système, ou par l’administrateur ou l’administratrice de groupes pour identifier les onglets et les rapports qui s’affichent dans l’espace de travail d’un utilisateur ou d’une utilisatrice spécifique.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Layout Type]</td> 
   <td>En association avec [!UICONTROL Custom Views], le [!UICONTROL Layout Type] spécifie le type de [!UICONTROL Custom View]. Actuellement, seul le type Liste est disponible. [!UICONTROL Detail] (la vue [!UICONTROL Detail] d’un objet) sera prochainement disponible.</td> 
  </tr> 
  <!--<tr data-mc-conditions=""> 
   <td>Legacy Budgeted Cost</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p> <p>The field is still visible in some reports and lists, but the information displayed cannot be updated. </p> <p>See <i>Budgeted Cost</i>. </p> </td> 
  </tr>
  --> 
  <!--<tr data-mc-conditions=""> 
   <td>Legacy Budgeted Hours</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p> <p>The field is still visible in some reports and lists, but the information displayed cannot be updated. </p> <p>See <i>Budgeted Hours</i>. </p> <p>
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        This field shows the number of hours budgeted for the project in the Legacy Resource Estimates area of the Business Case or in the Capacity Planner. 
       <br>If there  are multiple job roles, this is a summary of the budgeted hours for all job roles. The Legacy Budgeted Hours are calculated after you have used the "Set budget to schedule" feature, or after you have defined how many of the Planned Hours should be budgeted, in the Resource Estimates area of the Business Case of the project or in the Capacity Planner.   
     </p> </td> </tr> -->
  <!--<tr data-mc-conditions=""> 
   <td>Legacy Budgeted Labor Cost</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed. This field cannot be updated. </p> <p>The field is still visible in some reports and lists. </p> <p>See <i>Budgeted Labor Cost</i>. </p> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">In a project report, this field shows the labor cost associated with the project, taking into account the Cost per Hour rate of every job role and the amount of Legacy Budgeted Hours estimated in the Legacy Resource Estimates area of the Business Case that is needed for each role to complete the project.  </p>
    --> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Legacy Budgeted Labor Cost in a project report is calculated using the following formula:</p>
    --> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code style="font-style: normal;">Legacy Budgeted Labor Cost = SUM(Job Role Cost per Hour * Legacy Budgeted Hours per Job Role)</code> </p>
    --> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about calculating Legacy Budgeted Labor Cost, see the article <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Understand Budgeted Labor Cost and Budgeted Hours for projects</a>    </p>
    --> </td> 
  </tr> 
  <tr> 
   <!-- <td>Legacy Resource Pool</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed. This field cannot be updated. </p> 
   <p>Although not recommended, you may update the information in this report using the API.</p> 
   <p>See <i>Resource Pools</i> for updated fields. </p> 
   <p>The Legacy Resource Pool is a collection  of job roles associated with a project or a user. The functionality of the Legacy Resource Pools is displayed in the tools available in the Legacy Resource Planning tab of the People area. This is a deprecated field.</p>
    --> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL - Heures effectives héritées]</td> 
   <td> <p>Dans un rapport de projet, de tâche ou d'événement, les [!UICONTROL Legacy Actual Hours] représentent la somme de toutes les heures enregistrées dans le projet, la tâche ou l'événement, y compris avant mai 2021.</p>  
   <p>Les heures réelles héritées s'affichent sous la forme d'heures réelles dans une zone de détails de projet, de tâche ou d'événement. </p>
   <p>Voir aussi <strong>Heures réelles</strong>.
    <p>Pour plus d'informations, voir <a href="/help/quicksilver/manage-work/tasks/task-information/actual-hours.md">Afficher les heures réelles</a>.</p>
    </td> 
  </tr>  <tr> 
   <td>[!UICONTROL License Type]</td> 
   <td>Type de licence attribué à un [!UICONTROL Access Level]. Le type peut être [!UICONTROL Full User], [!UICONTROL Limited User] ou [!UICONTROL Requester].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL License Limit Plan]</td> 
   <td> <p>Dans un rapport ou une vue [!UICONTROL Group], ce champ indique le nombre maximal de licences [!UICONTROL Plan] pouvant être attribuées aux utilisateurs et aux utilisatrices dont le groupe respectif est désigné comme [!UICONTROL Home Group].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL License Limit Work]</td> 
   <td> <p>Dans un rapport ou une vue [!UICONTROL Group], ce champ indique le nombre maximal de licences [!UICONTROL Work] pouvant être attribuées aux utilisateurs et aux utilisatrices dont le groupe respectif est désigné comme [!UICONTROL Home Group].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limited User]</td> 
   <td>Un type de licence qui permet la création d’un [!DNL Access Level] qui contient des privilèges de lecture seule, avec la possibilité de soumettre des problèmes, de saisir des notes et de charger des documents.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL List Controls]</td> 
   <td> <p>Une partie de la [!UICONTROL Interface Setup] qui permet de lier des filtres, des vues et des regroupements personnalisés à des utilisateurs et utilisatrices individuellement ou globalement à tous les utilisateurs et utilisatrices.</p> </td> 
  </tr> 
<tr> 
   <td>[!UICONTROL Lookup fields]</td> 
   <td> <p>Dans Workfront Planning, après avoir établi la connexion entre deux types d'enregistrements et lié des enregistrements individuels entre eux, vous pouvez référencer les champs des enregistrements liés sur l'enregistrement à partir duquel vous vous connectez.</p>
   <p>Par exemple, si vous connectez un type d’enregistrement Campaign à un type d’objet Projet Workfront, vous pouvez afficher le champ Budget des projets connectés sur les enregistrements Campaign. Le champ Projet budgétaire est un champ de recherche parmi les projets d'une campagne.</p> <p>Les valeurs des champs de recherche sont automatiquement renseignées sur les enregistrements auxquels ils sont connectés.</p>
   <p>Pour plus d’informations, voir <a href="/help/quicksilver/planning/records/connected-records-overview.md">Présentation des enregistrements connectés</a>.</p>
   <p>Workfront Planning requiert une licence supplémentaire.</p>
    </td> 
  </tr> 
 </tbody> 
</table>

## M - O

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nom de l'objet</th> 
   <th>Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Manual Only]</td> 
   <td> <p>L’un des [!UICONTROL Update Types] du [!UICONTROL Project]. Ce paramètre permet de mettre à jour les chronologies [!UICONTROL Project Projected] et [!UICONTROL Planned] uniquement en cas de clic sur « [!UICONTROL Recalculated Timelines] ». Les projets configurés de cette manière seront ignorés lors du processus de recalcul nocturne et lorsque le projet ou les tâches du projet seront mis à jour.</p> <p>Pour plus d’informations, consultez <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Sélectionner le [!UICONTROL Update Type] du projet</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Me]</td> 
   <td> <p>Cela fait référence à la personne actuellement connectée. </p> <p>Il est recommandé d’utiliser ce champ dans un filtre afin de rendre les rapports plus génériques lors de leur partage avec d’autres utilisateurs et utilisatrices. Ainsi, vous pouvez créer un seul rapport qui affichera des informations différentes en fonction de la personne qui se connecte pour les afficher, car les informations sont toujours personnalisées pour l’utilisateur ou utilisatrice connecté. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Max Users]</td> 
   <td> <p>Ce champ est obsolète. Toute information que ce champ peut afficher est liée à une fonctionnalité supprimée par [!DNL Workfront] et le champ ne peut pas être mis à jour. </p> <p>Dans les versions précédentes de [!DNL Workfront], vous pouviez mettre à jour ce champ lors de la création ou de la modification d’une fonction. Il affichait, pour un rôle sur chaque projet, le nombre total d’affectations d’utilisateurs et d’utilisatrices. La valeur zéro est autorisée pour un nombre illimité d’affectations d’utilisateurs et d’utilisatrices à un projet. </p>Le champ est toujours visible dans certains rapports et listes, mais les informations affichées ne peuvent pas être mises à jour. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Milestone]</td> 
   <td> <p>Marqueur que vous pouvez associer à une tâche pour indiquer qu’un point clé du projet a été atteint une fois la tâche terminée. Vous pouvez généralement utiliser des jalons pour afficher un événement significatif, tel que la fin d’une phase du projet ou un ensemble d’activités critiques. Les [!UICONTROL Milestones] sont généralement associés à des tâches parent. Vous devez créer les jalons avant de pouvoir les associer aux tâches. Pour plus d’informations sur les jalons, consultez les sections <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md">Créer un chemin jalonné</a> et <a href="../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md">Associer des jalons à des tâches</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Milestone Path]</td> 
   <td>Collection de [!UICONTROL milestones]. Les [!UICONTROL Milestone Paths] sont utilisés sur les projets pour distinguer les projets avec certains types de [!UICONTROL Milestones] des projets avec un ensemble différent de [!UICONTROL Milestones].</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Milestone Task]</td> 
   <td>Tâche marquée pour indiquer un événement à mesurer.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Module]</td> 
   <td>Étape unique d’un scénario dans [!DNL Workfront Fusion] qui exécute une fonction d’après l’application associée.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL My Primary Role]</td> 
   <td> <p>Lorsqu’il est référencé dans les filtres, ce champ affiche soit les utilisateurs et les utilisatrices qui ont le même [!UICONTROL Primary Role] que les personnes connectées, soit les éléments de travail affectés au [!UICONTROL Primary Role] des personnes connectées qui l’utilisent.</p> <p>Il est recommandé d’utiliser ce champ dans un filtre afin de rendre les rapports plus génériques lors de leur partage avec d’autres utilisateurs et utilisatrices. Ainsi, vous pouvez créer un seul rapport qui affichera des informations différentes en fonction de la personne qui se connecte pour les afficher, car les informations sont toujours personnalisées pour l’utilisateur ou utilisatrice connecté. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL My Home Team]</td> 
   <td> <p>Lorsqu’il est référencé dans les filtres, ce champ affiche soit les utilisateurs et les utilisatrices qui ont la même [!UICONTROL Home Team] que les personnes connectées, soit les éléments de travail affectés à l’[!UICONTROL Home Team] des personnes connectées. </p> <p>Il est recommandé d’utiliser ce champ dans un filtre afin de rendre les rapports plus génériques lors de leur partage avec d’autres utilisateurs et utilisatrices. Ainsi, vous pouvez créer un seul rapport qui affichera des informations différentes en fonction de la personne qui se connecte pour les afficher, car les informations sont toujours personnalisées pour l’utilisateur ou utilisatrice connecté. </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Naming convention]</td> 
   <td>Ensemble de règles à l’échelle de l’organisation qui utilise des données pour créer des noms de projets, de tâches et d’éléments livrables.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Native Integration]</td> 
   <td>Intégration qui ne nécessite pas de codage manuel ni de configuration d’API. Également appelée intégration « prête à l’emploi ».</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Navigation Menu]</td> 
   <td>Panneau supérieur central de l’application qui contient les liens vers les principales zones de [!UICONTROL Workfront].</td> 
  </tr> 
 </tr> 
  <tr> 
   <td>[!UICONTROL New Number Value]</td> 
   <td>Dans un rapport [!UICONTROL Journal Entry], cette option affiche la valeur mise à jour d’un champ qui remplace l’[!UICONTROL Old Number Value].
   Pour plus d’informations, voir « [!UICONTROL Old Number Value] » dans cet article.</td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL Non-Billable Expense]</td> 
   <td> <p>Dépense non marquée comme facturable au client ou à la cliente. Il peut s’agir d’une dépense prévue ou d’une dépense effective.</p> <p>Les champs Coût prévu des dépenses non facturables et Coût réel des dépenses non facturables peuvent être ajoutés aux vues et aux rapports. Ils n’apparaissent pas sur les pages de détails du projet ou de la tâche.</p>
   <p>Vous trouverez ces champs dans les types de rapports suivants :</p>
   <ul>
   <li>Niveau de référence</li>
   <li>Modèle</li>
   <li>Projet (données financières)</li>
   </ul>
   <p>Pour plus d’informations sur le marquage d’une dépense comme facturable, voir <a href="/help/quicksilver/manage-work/projects/project-finances/manage-project-expenses.md">Gérer les dépenses du projet</a>.</p>
   </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Non Work Day]</td> 
   <td>Jour qui n’est pas consacré à la réalisation d’une affectation. Il s’agit généralement d’un jour de congé, d’un jour férié ou d’un week-end. Le terme s’affiche dans l’explorateur d’API. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Note]</td> 
   <td>Commentaire ou mise à jour effectué sur un objet [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Note Text]</td> 
   <td> <p>Cette option affiche le texte d’une mise à jour saisie par un utilisateur ou par une utilisatrice sur n’importe quel objet. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Number of Linked Goals]</td> 
   <td> <p>Dans un rapport de [!UICONTROL Project], il s’agit du nombre d’objectifs stratégiques associés au projet. Pour plus d’informations sur l’association de projets à des objectifs stratégiques, consultez la section <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md">Ajouter des projets aux objectifs dans [!DNL Adobe Workfront Goals]</a>.</p> 
   <p>Pour plus d’informations sur les objectifs stratégiques, consultez aussi dans cet article la section « [!UICONTROL Goal] ».</p> 
   <p>Ce champ n’est visible que si votre entreprise a acheté [!DNL Workfront Goals]. Pour plus d’informations sur la gestion des objectifs stratégiques à l’aide de [!DNL Workfront Goals], consultez la section <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md">Ajouter des projets aux objectifs dans [!UICONTROL Adobe Workfront Goals]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Object]</td> 
   <td> <p>Les informations affichées dans [!DNL Adobe Workfront] sont représentées par des objets stockés dans la base de données [!DNL Workfront]. Les objets sont les éléments qui alimentent l’information dans Workfront. Voici quelques exemples d’objets :</p> 
    <ul> 
     <li>[!UICONTROL Portfolios]</li> 
     <li>[!UICONTROL Programs]</li> 
     <li>[!UICONTROL Projects]</li> 
     <li>[!UICONTROL Tasks]</li> 
     <li>[!UICONTROL Issues]</li> 
     <li>[!UICONTROL Documents]</li> 
     <li>[!UICONTROL Dashboards]</li> 
     <li>[!UICONTROL Reports]</li> 
     <li>[!UICONTROL Groups]</li> 
     <li>[!UICONTROL Teams]</li> 
     <li>[!UICONTROL Users]</li> 
     <li>[!UICONTROL Companies]</li> 
     <li>[!UICONTROL Custom forms]</li>
     <li>[!UICONTROL Custom fields]</li>  
     <li>[!UICONTROL Hours]</li> 
     <li>[!UICONTROL Billing Rates]</li> 
     <li>[!UICONTROL Templates]</li> 
     <li>[!UICONTROL Template tasks]</li>

<p><b>NOTE</b></p>
  <p>Cette liste n’est pas exhaustive. </p>

</ul> <p>Pour plus d’informations, consultez la section <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Présentation des objets dans [!UICONTROL Adobe Workfront]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Object Types]</td> 
   <td>Vous pouvez utiliser ce champ comme vue ou filtre pour identifier les types d’objets associés à chaque formulaire si vous créez un rapport ou une liste contenant tous vos formulaires personnalisés. </td> 
  </tr> 
 <tr> 
   <td>[!UICONTROL Old Number Value]</td> 
   <td>Dans un rapport d’[!UICONTROL Journal Entry], la valeur d’origine d’un champ s’affiche avant d’être mise à jour. Une fois la valeur d’un champ mise à jour, elle s’affiche sous la forme d’une [!UICONTROL New Number Value] dans un rapport d’[!UICONTROL Journal Entry]. Pour plus d’informations, consultez également la section « [!UICONTROL New Number Value] ».</td> 
  </tr>
  <tr> 
   <td>[!UICONTROL On Change Only]</td> 
   <td> <p>Un des types [!UICONTROL Project Update]. Lorsque cette option est sélectionnée, les chronologies de [!UICONTROL Project Projected] et [!UICONTROL Planned] ne sont mises à jour que lorsqu’une mise à jour ou une modification est apportée au projet ou à une tâche du projet. Le projet n’est pas mis à jour tous les soirs.</p> <p>Pour plus d’informations, consultez la section <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Sélectionner le type de mise à jour du projet</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Op Task]</td> 
   <td> <p>Nom du [!UICONTROL Issue] dans la base de données [!DNL Workfront], utilisé dans les rapports en mode texte ou les données personnalisées calculées.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Open]</td> 
   <td>Un problème ou une tâche qui n’est pas terminé(e), mais sur lequel ou laquelle un travail est en cours.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Org Chart]</td> 
   <td>Abréviation d’Organizational Chart (Organigramme). Il s’agit d’un graphique montrant les liens hiérarchiques au sein d’une organisation. Il s’agit également de l’onglet de l’écran de détail d’[UICONTROL User] qui affiche et permet de définir les relations de l’[UICONTROL Company] et du [UICONTROL Reporting] de l’[UICONTROL User].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Organizational Setup]</td> 
   <td>Ce champ définit les [!UICONTROL Companies], [!UICONTROL Groups], et [!UICONTROL Security Profiles] pour votre organisation.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Other Groups]</td> 
   <td> <p>Dans un rapport ou une vue qui répertorie les utilisateurs et les utilisatrices, ce champ affiche tous les groupes dont chaque utilisateur ou chaque utilisatrice est membre. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Override Currency]</span> </td> 
   <td> 
    <div> 
     <p>Dans un rapport de [!UICONTROL Job Role], il s’agit de la devise associée à une fonction. Il s’agit du remplacement de la [!UICONTROL Base Currency] telle qu’elle est définie dans la zone de [!UICONTROL Setup] par l’équipe d’administration de [!DNL Workfront]. </p> 
     <p>Pour plus d’informations, consultez la section <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Créer et gérer des fonctions</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Override Currency Billing/ Hour]</span> </td> 
   <td> 
    <div> 
     <p>Dans un rapport sur les [!UICONTROL Job Role], il s’agit du taux de facturation par heure de la fonction à l’aide de la [!UICONTROL Override Currency] sélectionnée pour la fonction.</p> 
     <p> Pour plus d’informations, consultez la section <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Créer et gérer des fonctions</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Override Currency Cost/ Hour]</span> </td> 
   <td> 
    <div> 
     <p>Dans un rapport sur les [!UICONTROL Job Role], il s’agit du coût par heure de la fonction utilisant la [!UICONTROL Override Currency] sélectionnée pour la fonction. </p> 
     <p>Pour plus d’informations, consultez la section <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Créer et gérer des fonctions</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Owner]</td> 
   <td>L’utilisateur ou l’utilisatrice responsable de l’achèvement de l’objet désigné.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Owner Type]</span> </td> 
   <td> 
    <div> 
     <p>Dans un rapport d’[!UICONTROL Goal], ce champ affiche le type de propriétaire affecté à un objectif stratégique. Voici les types de propriétaire d’objectif :</p> 
     <ul> 
      <li> <p>[!UICONTROL User]</p> </li> 
      <li> <p>[!UICONTROL Team] </p> </li> 
      <li> <p>[!UICONTROL Group]</p> </li> 
     </ul> 
     <p>Aucune valeur ne s’affiche dans ce champ si votre organisation détient l’objectif. </p> 
     <p>Cela nécessite une licence supplémentaire. Pour plus d’informations sur les [!DNL Workfront Goals], consultez la section « Vue d’ensemble des <a href="../../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">[!DNL Adobe Workfront Goals] »</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

## P - R

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nom de l'objet</th> 
   <th>Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Parameter]</td> 
   <td> <p>Un [!UICONTROL parameter] est un champ personnalisé. Vous pouvez générer un rapport pour tous les paramètres ou champs personnalisés de votre système. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Parent]</td> 
   <td>Dans un rapport, ce champ affiche des informations sur le parent de l’objet. Dans un rapport sur les [!UICONTROL issue], par exemple, il peut afficher des informations sur la tâche ou le projet sous lequel le problème est connecté ; dans un rapport sur les tâches, il peut afficher des informations sur la tâche parent directe ou sur le projet. Pour plus d’informations sur les objets dont les parents peuvent se trouver dans [!DNL Workfront], consultez la section « Interdépendance et hiérarchie des objets » dans l’article <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Présentation des objets dans [!DNL Adobe Workfront]</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Parent Lag]</td> 
   <td>Le temps qui doit s’écouler entre le démarrage de la [!UICONTROL Parent Task] et celui de la [!UICONTROL Subtask].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Parent Task]</td> 
   <td>Connue également sous le nom de [!UICONTROL Summary Task]. Il s’agit d’une tâche qui comporte des sous-tâches (également appelées [!UICONTROL Children Tasks]). Les [!UICONTROL Duration], [!UICONTROL Work Required], et [!UICONTROL Percent Complete] de la tâche parent sont calculés à partir des sous-tâches.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Part-Time Resources]</td> 
   <td>Un utilisateur ou une utilisatrice sous licence ayant une capacité inférieure au planning par défaut défini dans le système.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Percent Complete]</td> 
   <td> <p>Un champ de projet, de tâche ou de problème qui indique le pourcentage de travail associé à la tâche, au projet ou au problème qui est terminé.</p> <p>Vous pouvez mettre à jour ce champ manuellement pour les problèmes et les tâches de travail. </p> <p>Pour les projets et les tâches parents, ce champ est un cumul de toutes les tâches opérationnelles et il ne peut être mis à jour manuellement. </p> <p>Pour plus d’informations, consultez la section <a href="../../../manage-work/tasks/task-information/project-percent-complete.md" class="MCXref xref">Vue d’ensemble du [!UICONTROL Percent Complete] du projet</a>.</p> </td> 
  </tr> 
<tr> 
   <td>[!UICONTROL Performance Index Method (PIM)]</td> 
   <td> <p>La méthode [!UICONTROL Performance Index Method (PIM)] pour le projet contrôle la méthode utilisée par Adobe Workfront pour calculer les mesures de performances du projet, telles que l’indice de performance des coûts (ICP), l’indice de performance des prévisions de coûts (CSI), l’indice de performance des prévisions (SPI) et l’estimation à l’achèvement (EAC).</p> 
   <p>Workfront calcule ces valeurs à l’aide des heures ou du coût.</p>
   <p>Pour plus d'informations, voir <a href="/help/quicksilver/manage-work/projects/project-finances/set-pim.md">Définir la méthode d'indice de performance (PIM)</a>.</p>
   </td> 
  </tr>
 <tr> 
   <td>[!UICONTROL Permission]</td> 
   <td> <p>Droits accordés à un utilisateur ou à une utilisatrice sur un objet, généralement donnés pour lui permettre de terminer le travail sur l’élément ou de l’afficher. Vous pouvez octroyer des autorisations aux :</p> 
    <ul> 
     <li>[!UICONTROL Projects]</li> 
     <li>[!UICONTROL Tasks]</li> 
     <li>[!UICONTROL Issues]</li> 
     <li>[!UICONTROL Portfolios]</li> 
     <li>[!UICONTROL Programs]</li> 
     <li>[!UICONTROL Reports]</li> 
     <li>[!UICONTROL Dashboards]</li> 
     <li>[!UICONTROL Documents]</li> 
     <li>[!UICONTROL Custom Forms]</li> 
     <li>[!UICONTROL Views]</li> 
     <li>[!UICONTROL Filters]</li> 
     <li>[!UICONTROL Groupings]</li> 
    </ul> <p>Pour plus d’informations, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Vue d’ensemble des autorisations de partage sur les objets</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Plan]</td> 
   <td> <p>Il s’agit d’un type de licence complet dans le système [!DNL Workfront]. Les utilisateurs et utilisatrices doivent disposer de ce plan pour accéder à toutes les fonctionnalités de [!DNL Workfront].</p> <p>Pour plus d’informations, voir Vue d’ensemble des licences <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Plan] (dans le [!DNL Scenario Planner])</td> 
   <td> <p>Un plan est l’objet principal lors de l’utilisation du planificateur de scénarios [!DNL Workfront]. Vous pouvez définir la stratégie à court et à long terme de votre entreprise, identifier chaque résultat de haut niveau et l’ajouter en tant que plan au planificateur de scénarios [!DNL Workfront]. </p> <p>Vous ne pouvez pas afficher les plans [!DNL Scenario Planner] dans un rapport et vous ne pouvez pas y accéder via l’API [!DNL Workfront]. </p> <p>Le [!DNL Scenario Planner] nécessite une licence supplémentaire. Pour plus d’informations sur le [!DNL Workfront Scenario Planner], voir <a href="../../../scenario-planner/scenario-planner-overview.md">Vue d’ensemble du [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned]</td> 
   <td> <p>Période pendant laquelle un événement est planifié. Lorsque vous créez des projets, des tâches ou des problèmes dans [!DNL Workfront], vous définissez les dates de début et de fin prévues, ainsi que la période prévue pendant laquelle elles ont lieu. Ces valeurs représentent votre intention initiale ou votre estimation du temps nécessaire à l’exécution d’un élément. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Benefit]</td> 
   <td>Entrée manuelle permettant à la personne gestionnaire de projet d’estimer si la réalisation d’un projet apporterait un avantage financier à l’organisation. La spécification de cette valeur peut se faire dans le cadre de l’élaboration d’un [!UICONTROL Business Case] pour le projet. Pour mettre à jour cette valeur, vous devez disposer des autorisations de [!UICONTROL Manage] pour le projet.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Planned Budgeted Hours]</td> 
   <td> <p>Dans un rapport [!UICONTROL Budgeted Hour], cela indique le nombre d’heures budgétées pour les projets ou les [!UICONTROL Job Roles] dans le [!UICONTROL Resource Planner]. </p> <p>Pour plus d’informations sur la budgétisation des projets ou des rôles dans le [!UICONTROL Resource Planner], voir l’article <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Budgéter des ressources dans le [!UICONTROL Resource Planner] à l’aide des vues [!UICONTROL Project] et [!UICONTROL Role]</a>. Pour plus d’informations sur le rapport des [!UICONTROL Budgeted Hours], voir l’article <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref">Rapport : heures budgétées</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Completion Date]</td> 
   <td> <p>Vous pouvez définir manuellement la [!UICONTROL Planned Completion Date] d’une tâche, d’un projet ou d’un événement à une date de votre choix. Si vous ne définissez pas la [!UICONTROL Planned Completion Date], [!DNL Workfront] la définit automatiquement. Lorsqu’elle est définie automatiquement, la [!UICONTROL Planned Completion Date] est : [!UICONTROL Planned Start Date] + [!UICONTROL Duration].</p> <p>Pour plus d’informations, consultez les articles suivants :</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Vue d’ensemble de la [!UICONTROL Planned Completion Date] de la tâche</a> </p> </li> 
     <li> <p><a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">Définir la [!UICONTROL Planned Completion Date] du projet</a> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Cost]</td> 
   <td> <p>Total du [!UICONTROL Planned Labor Cost] et du [!UICONTROL Planned Expense Cost] du projet. Cela n’inclut pas le [!UICONTROL Planned Risk Cost] du projet. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Date Alignment]</td> 
   <td> <p>Il s’agit d’un indicateur automatique que Workfront affecte des projets, des tâches et des événements pour indiquer quand un élément sera terminé par rapport à sa date d’achèvement prévue. </p>
   <p>Les valeurs suivantes sont des valeurs possibles pour l’indicateur Alignement de date prévu : </p>
<ul>
<li>Sera terminé à la date d'achèvement prévisionnelle</li>
<li>Sera terminé avant la date d'achèvement prévisionnelle</li>
<li>Sera terminé après la date d'achèvement prévisionnelle</li></ul>
<p>L’alignement des dates prévues est visible dans les listes et les rapports des projets, des tâches et des événements. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Duration]</td> 
   <td> <p>La [!UICONTROL Planned Duration] d’une tâche est généralement identique à sa [!UICONTROL Duration]. Elle représente la différence en jours entre le [!UICONTROL Planned Start] et les [!UICONTROL Planned Completion Dates] de la tâche. </p> <p>Lorsque la tâche possède un type de [!UICONTROL Duration] [!UICONTROL Effort Driven], la [!UICONTROL Planned Duration] peut différer de la [!UICONTROL Duration] de la tâche, en fonction du nombre de ressources que vous affectez à la tâche. </p> <p>Par exemple, si une tâche avec un type de [!UICONTROL Duration] [!UICONTROL Effort Driven] a une [!UICONTROL Duration] de 3 jours et que vous attribuez une ressource avec un planning à temps plein à la tâche, la [!UICONTROL Planned Duration] est également de 3 jours. Si vous affectez trois ressources à temps plein à la même tâche, la [!UICONTROL Duration] reste de 3 jours, mais la [!UICONTROL Planned Duration] passe à 1 jour. La [!UICONTROL Planned Duration] modifie également les dates de [!UICONTROL Planned Start] et de [!UICONTROL Planned Completion] de la tâche, afin de refléter la nouvelle [!UICONTROL Planned Duration]. Par conséquent, la chronologie du projet est également affectée. </p> <p>Pour plus d’informations sur la différence entre la [!UICONTROL Duration] et la [!UICONTROL Planned Duration] pour les tâches, consultez l’article <a href="../../../manage-work/tasks/task-information/planned-duration-vs-duration-for-tasks.md" class="MCXref xref">Différence entre [!UICONTROL Planned Duration] et [!UICONTROL Duration] pour les tâches</a>.</p> <p>Les projets et problèmes n’ont pas de [!UICONTROL Planned Duration]. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Duration Minutes]</td> 
   <td> <p>La [!UICONTROL Planned Duration Minutes] d’un projet ou d’un problème représente la [!UICONTROL Duration] du projet ou du problème en minutes. </p> <p>Les tâches n’ont pas de champ de [!UICONTROL Planned Duration Minutes]. </p> <p>Les [!UICONTROL Template Tasks] disposent d’un champ de [!UICONTROL Planned Duration Minutes] qui affiche la [!UICONTROL Planned Duration] de la tâche en minutes. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Expense Cost]</td> 
   <td> <p>Somme des [!UICONTROL Planned Amounts] pour toutes les dépenses enregistrées pour un projet ou une tâche.</p> <p><b>EXEMPLE</b></p>
   <p>Si vous créez une dépense pour la tâche 1 et que vous saisissez 600,00 $ dans le champ du [!UICONTROL Planned Amount], le [!UICONTROL Planned Expense Cost] pour cette tâche est de 600,00 $. </p> 
   <p>Pour un projet, [!DNL Workfront] utilise la formule suivante pour calculer le [!UICONTROL Planned Expense Cost] :</p> <p><code>Project [!UICONTROL Planned Expense Cost] = SUM (All Project [!UICONTROL Planned Expense Costs]) + SUM (All Tasks [!UICONTROL Planned Expense Costs])</code> </p> 
   <!--
     <p>Important: If the value in the Actual Amount field for an expense is negative, Workfront will ignore that expense record. For example, if the value in the Planned Amount field is $200.00 but the value in the Actual Amount field is -$300.00, the system will ignore this entire expense record which means you would not include the $200.00 planned value or the -$300.00 actual value in any calculations for Planned Expense Cost or Actual Expense Cost. (Drafting this because not sure if this is correct anymore)</p>
    --> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Hours]</td> 
   <td> <p>Ce champ apparaît dans les zones [!UICONTROL projects], [!UICONTROL tasks] et problèmes, les rapports sur les projets, les tâches ou les problèmes, et les outils de gestion des ressources tels que le [!UICONTROL Resource Planner], l’[!UICONTROL Workload Balancer] et le rapport d’[!UICONTROL Utilization]. </p> <p>Il indique le nombre d’heures que la personne propriétaire du projet estime nécessaire à l’exécution de chaque tâche ou problème. Pour les projets, il s’agit généralement d’un cumul des [!UICONTROL Planned Hours] des tâches du projet. </p> <p>Selon l’endroit d’où vous l’affichez, le champ [!UICONTROL Planned Hours] peut présenter différentes informations. Pour plus d’informations sur le nombre d’heures prévues, consultez la section <a href="../../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref">Vue d’ensemble du nombre d’heures prévues</a>.</p> <p>Le nombre d’heures prévues est stocké en minutes dans la base de données [!DNL Workfront]. Lorsque vous effectuez des calculs à l’aide de ce champ, tenez compte du fait que les heures s’affichent en minutes.<br></p> <p>Le nombre d’heures prévues est réparti uniformément sur tous les jours de la durée d’un élément de travail par défaut, ainsi que sur toutes les ressources affectées à la tâche. Les utilisateurs et les utilisatrices peuvent mettre à jour le nombre quotidien d’heures prévues pour un élément de travail ou le nombre d’heures prévues individuelles pour chaque personne cessionnaire.</p> <p>La mise à jour de ce champ diffère pour les projets, les tâches et les problèmes : </p> 
    <ul> 
     <li> <p>Pour les problèmes, vous pouvez mettre à jour ce champ manuellement.Le nombre d’heures prévues du problème n’est pas ajouté à celui du projet. </p> <p><b>CONSEIL</b></p> <p>Dans un rapport sur un problème, l’un des champs [!UICONTROL Planned Hours] est remplacé par le champ [!UICONTROL Work].Le champ affiche le nombre d’heures prévues sur le problème. Pour plus d’informations, consultez les champs « travail » ou « [!UICONTROL Work] » de ce tableau. </p> </li> 
    </ul> 
    <ul> 
     <li> <p>Pour les tâches, vous pouvez mettre à jour manuellement ce champ lorsque le [!UICONTROL Duration Type] de la tâche est [!UICONTROL Calculated Assignment] ou [!UICONTROL Simple]. Ce champ est calculé par [!DNL Workfront] lorsque le [!UICONTROL Duration Type] de la tâche est [!UICONTROL Calculated Work] ou [!UICONTROL Effort Driven].<br>Pour plus d’informations sur la [!UICONTROL Task Duration], consultez l’article <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Vue d’ensemble de la [!UICONTROL Duration] et du [!UICONTROL Duration Type]</a>.</p> </li> 
    </ul> 
    <ul> 
     <li> <p>Pour les projets, [!DNL Workfront] calcule le nombre d’heures prévues en ajoutant toutes les heures prévues de toutes les tâches du projet. </p> </li> 
    </ul> <p><b>CONSEIL</b></p> <p>Vous pouvez afficher le [!UICONTROL Planned Hours] dans les rapports sur les [!UICONTROL project], [!UICONTROL task] ou [!UICONTROL issues] en utilisant également le mode texte et en référençant des champs supplémentaires. Pour plus d’informations, consultez les champs « <code>work</code> », « [!UICONTROL Work] » et « <code>workRequiredExpression</code> » dans ce tableau. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Labor Cost]</td> 
   <td> 
    <p>Il s’agit, pour une tâche, du taux horaire de l’utilisateur ou de l’utilisatrice ou du rôle multiplié par le nombre d’heures affecté à l’utilisateur ou à l’utilisatrice ou au rôle.</p> <p>Pour un projet, il s’agit du total des [!UICONTROL Planned Labor Costs] de toutes les tâches.</p> <p>Le taux d’utilisation de l’utilisateur ou de l’utilisatrice ou du rôle dépend du type de coût sélectionné pour la tâche donnée. </p> <p>Pour plus d’informations, consultez la section <a href="../../../manage-work/projects/project-finances/track-costs.md">Suivre les coûts</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Revenue]</td> 
   <td> <p>Les tâches et les projets peuvent afficher une valeur pour [!UICONTROL Planned Revenue] dans [!DNL Workfront]. Les [!UICONTROL Planned Revenue] représentent l’argent associé au [!UICONTROL Planned Hours] des tâches du projet. Pour les projets, ils peuvent également inclure les [!UICONTROL Fixed Revenue] du projet. </p> <p>Pour les tâches, il s’agit des revenus associés au [!UICONTROL Planned Hours] des tâches. Le nombre d’heures prévues de toutes les tâches se cumule au nombre d’heures prévues du projet afin de contribuer au calcul du [!UICONTROL Planned Hours] du projet. </p> 
   <p>[!DNL Workfront] calcule les [!UICONTROL Planned Revenue] pour les tâches et les projets à l’aide des formules suivantes :</p> 
   <p><code>Task [!UICONTROL Planned Revenue] = [!UICONTROL Planned Hours] * Billing hourly rate</code> </p> <p><code>Project [!UICONTROL Planned Revenue] = SUM (All tasks [!UICONTROL Planned Revenue]) + [!UICONTROL Fixed Revenue]</code> </p> 
   <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(the note below is duplicated in this article: /Content/Resource Mgmt/Resource utilization/view-utilization-information.htm and in the glossary)</p>
    --> 
    <p>Les [!UICONTROL Planned Revenue] du projet qui s’affichent dans la zone [!UICONTROL Project Details] et dans les rapports du projet diffèrent des revenus prévus qui s’affichent dans le rapport [!UICONTROL Utilization]. </p> <p>Les [!UICONTROL Planned Revenue] dans la zone [!UICONTROL Project Details] reflètent les revenus de la tâche ainsi que les revenus fixes du projet. Les [!UICONTROL Planned Revenue] du [!UICONTROL Utilization Report] affiche les [!UICONTROL Planned Revenue] associés uniquement aux tâches du projet. </p> 
     <p><b>EXEMPLE</b></p>  
      <p>Si le projet comporte une tâche de 10 heures, affectée à un consultant avec un taux horaire de 20 $ et que le projet a des [!UICONTROL Fixed Revenue] de 100 $, le rapport d’[!UICONTROL Utilization] affiche 200 $ pour les [!UICONTROL Planned Revenue] (les [!UICONTROL Planned Revenue] associés aux heures passées sur la tâche). La section [!UICONTROL Project Details] affiche 300 $ (les [!UICONTROL Planned Revenue] de la tâche et les revenus fixes du projet.) </p> 
    <p>Pour plus d’informations sur le suivi des revenus dans [!DNL Workfront], voir <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md">Vue d’ensemble de la facturation et des revenus</a>. </p> 
    <p>Pour plus d’informations sur les calculs des [!UICONTROL Planned Revenue] dans le [!UICONTROL Utilization report], voir <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md">Afficher des informations sur l’utilisation des ressources</a>. </p> 
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Risk Cost]</td> 
   <td> <p>Total du [!UICONTROL Potential Cost] de tous les risques sur le projet en tenant compte de leur probabilité de réalisation. Ce montant n’est pas inclus dans le [!UICONTROL Planned Cost] du projet.</p> <p>Le [!UICONTROL Planned Risk Cost] d’un projet est calculé selon la formule suivante :</p> <p><code>Planned Risk Cost = SUM(Potential Risk Cost * Probability / 100)</code> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Portal Profile]</td> 
   <td>Collection d’onglets et de sections définie par l’administrateur qui s’affiche dans [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Portal Section]</td> 
   <td>Composant d’un onglet sur un tableau de bord ou une page de portail. Généralement un seul rapport, graphique, calendrier ou une seule liste d’informations clés.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Portal Tab]</td> 
   <td>Onglet d’un portail ou d’un tableau de bord qui contient jusqu’à trois sections de portail.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Portfolio]</td> 
   <td> <p>Collection de projets présentant des caractéristiques communes. Ces projets sont généralement en concurrence pour les mêmes ressources, le même budget ou le même créneau horaire. Vous pouvez diviser les portfolios en programmes et associer les projets aux programmes avant de les ajouter à un portfolio.</p> <p>Pour plus d’informations sur les portefeuilles, voir <a href="../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md">Comprendre la méthodologie du portefeuille</a>.</p> 
   </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Portfolio Management]</td> 
   <td>Zone de pratique axée sur la gestion d’une collection ou de programmes connexes et les efforts du projet.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Portfolio Optimizer]</td> 
   <td>Outil [!DNL Workfront] permettant d’évaluer et de hiérarchiser les projets au sein d’un portfolio.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Portfolio Owner]</td> 
   <td>Parties prenantes responsables de la définition des priorités et du budget d’un portfolio.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Potential Risk Cost]</td> 
   <td>Il s’agit d’un champ de projet que vous pouvez trouver dans les listes et les rapports. Il indique le coût potentiel des risques associés au projet, s’ils se produisent. Pour plus d’informations, voir <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">Calculer le coût potentiel des risques</a>. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Predecessor]</td> 
   <td> <p>Tâche qui doit être terminée avant la fin d’une tâche dépendante. Tâche marquée comme [!UICONTROL Dependency] d’une autre tâche. Les tâches antérieures permettent au planificateur de définir une logique de dépendance de séquence, par exemple pour démarrer une tâche une fois qu’une autre tâche est terminée.</p> <p>Pour plus d’informations, voir <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">Vue d’ensemble des tâches antérieures</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Primary Company]</td> 
   <td>Entreprise à laquelle appartient l’utilisateur ou utilisatrice comme indiqué dans ses paramètres utilisateur. Les entreprises peuvent également être associées à des projets.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Primary Contact]</td> 
   <td><p>Le [!UICONTROL Primary Contact] est le créateur ou la créatrice d’un problème et il est automatiquement désigné par [!DNL Workfront] lorsqu’une personne crée le problème. Vous pouvez mettre ce champ à jour manuellement si vous avez des autorisations de [!DNL Manage] pour le problème. Un problème ne peut avoir qu’un créateur ou qu’une créatrice.</p> 
   <p>Si vous modifiez le créateur ou la créatrice, la personne désignée à l’origine comme créateur ou créatrice a toujours l’accès en [!UICONTROL Manage].</p>
   <p>Lors de la conversion d’un problème en une tâche ou un projet, l’utilisateur ou l’utilisatrice représentant le [!UICONTROL Primary Contact] du problème devient le [!UICONTROL Converted Issue Originator] du projet ou de la tâche. Si le [!UICONTROL Primary Contact] du problème est mis à jour après la conversion du problème, le [!UICONTROL Converted Issue Originator] sera conservé en tant que [!UICONTROL Primary Contact] du problème au moment de la conversion. Consultez aussi dans cet article la section « [!UICONTROL Converted Issue Originator] ».</p> 
   </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Priority]</td> 
   <td>Une valeur pouvant être affectée à une tâche, à un problème ou à un projet pour désigner l’importance de cette tâche. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Private]</td> 
   <td>Dans une [!UICONTROL Note] ou un [!UICONTROL Document], cette option masque cet objet à la plupart des personnes pouvant le voir. Dans le cas d’une file d’attente de requêtes d’aide privée, seuls les utilisateurs ou les utilisatrices de l’équipe de projet peuvent soumettre des problèmes à cette file d’attente (ou projet) par le biais de la zone des [!UICONTROL Requests].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Profile]</td> 
   <td>Toutes les informations sur un compte d’utilisateur ou d’utilisatrice.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Program]</td> 
   <td> <p>Un sous-ensemble au sein d’un portfolio, où des projets similaires peuvent être regroupés afin d’obtenir un avantage bien défini.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Program Management]</td> 
   <td>Gestion des dépendances, des risques, des problèmes, des exigences et des solutions entre les projets afin de préserver la qualité du programme et d’atteindre les objectifs définis.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Program Owner]</td> 
   <td>Les parties prenantes responsables de la supervision et de l’organisation des activités pour s’assurer que les objectifs du projet sont alignés sur ceux de l’entreprise.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Progress]</span> </td> 
   <td> <p>Dans un rapport d’[!UICONTROL Goal], ce champ affiche le pourcentage de réalisation d’un objectif stratégique. Le pourcentage de progression s’affiche sous la forme d’un nombre. Pour plus d’informations sur les objectifs stratégiques, consultez aussi dans ce tableau « [!UICONTROL Goal] ».</p> <p>Ce champ n’est visible que si votre entreprise a acheté les Objectifs [!DNL Workfront]. Pour plus d’informations sur la gestion des objectifs stratégiques à l’aide de [!DNL Workfront Goals], consultez la section <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md">Ajouter des projets aux objectifs dans [!DNL Adobe Workfront Goals] </a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Progress Status]</td> 
   <td> <p>Dans un rapport sur les projets, tâches et objectifs, ce champ affiche le statut de progression des projets, des tâches ou des objectifs stratégiques. Pour plus d’informations, consultez les articles suivants :</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/projects/planning-a-project/project-progress-status.md" class="MCXref xref">Vue d’ensemble de statut de progression du projet</a> </p> </li> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">Vue d’ensemble du statut de progression de la tâche</a> </p> </li> 
     <li> <p><a href="../../../workfront-goals/goal-management/calculate-goal-progress.md">Vue d’ensemble de la progression et de la condition des objectifs dans [!DNL Adobe Workfront Goals]</a> </p>
     <p>Les rapports sur les [!UICONTROL Goal] et les [!UICONTROL Progress Status] pour le champ [!DNL goals] ne sont visibles que si votre organisation a acheté [!DNL Workfront Goals]. Pour plus d’informations sur les objectifs stratégiques dans [!DNL Workfront Goals], consultez la section « Vue d’ensemble des <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] »</a>. </p> </li>
    </ul> </td> 
  </tr> 
  <td>[!UICONTROL Project]</td> 
   <td> <p>Une grande quantité de travail qui doit être réalisée dans un délai spécifique et qui doit utiliser un budget et un nombre de ressources spécifiques. Divisez le projet en une série de tâches pour le rendre gérable. La réalisation de toutes les tâches entraîne la fin du projet. Pour plus d’informations sur la planification d’un projet, consultez la section <a href="../../../manage-work/projects/planning-a-project/plan-project.md">Vue d’ensemble de la planification d’un projet</a>.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Assignment Planned Hours]</td> 
   <td> <p>Dans un rapport sur les [!UICONTROL Initiative Job Role], ce champ indique le nombre d’[!UICONTROL Planned Hours] associé à une fonction affectée à des tâches ou à des problèmes dans le projet. Ce champ et le type de rapport sur les [!UICONTROL Initiative Job Role] ne s’affichent pas dans votre instance [!DNL Workfront] à moins que votre société n’ait acheté une licence [!DNL Workfront Scenario Planner]. Pour plus d’informations sur le [!DNL Workfront Scenario Planner], consultez <a href="../../../scenario-planner/scenario-planner-overview.md">La vue d’ensemble du [!DNL Workfront Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Details]</td> 
   <td>Détails du statut actuel d’un projet.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Budgeted Cost]</td> 
   <td> <p> Il s’agit du [!UICONTROL Budgeted Cost] d’un projet tel qu’il s’affiche dans les listes et les rapports.</p><p>Consultez aussi dans cet article « [!UICONTROL Budgeted Cost] ».</p></td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Project Management]</td> 
   <td>Un ensemble de stratégies qui déterminent les seuils de création, de classification et d’affectation de noms des projets.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Project Overhead]</td> 
   <td>Dans un rapport [!UICONTROL Hour], ce champ est réservé aux informations financières liées aux heures consignées avec le type d’heure de [!UICONTROL Project Time]. Les projets peuvent avoir leurs propres taux de facturation. Si une heure est consignée directement sur un projet, ces taux seront utilisés dans les calculs. En fonction des paramètres du projet, les projets peuvent également comporter des devises différentes et une conversion de devise peut être effectuée pour ces heures. L’objet [!UICONTROL Project Overhead] permet à [!DNL Workfront] d’obtenir cette information.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Owner]</td> 
   <td>L’utilisateur ou l’utilisatrice responsable de la gestion de la portée, de la chronologie et des affectations d’un projet. L’approbateur ou l’approbatrice par défaut pour les ordres de modification, les modifications financières et les éléments livrables.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Planning]</td> 
   <td>Processus d’élaboration et de gestion du planning du projet.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Sponsor]</td> 
   <td>Un profil de partie prenante désigné auquel chacun de vos utilisateurs et utilisatrices doit se rattacher. Dans [!DNL Workfront], les éléments de la sorte sont désignés comme des [!UICONTROL Access Levels].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Teams]</td> 
   <td> <p>L’ensemble des utilisateurs et utilisatrices ou des rôles affectés à un projet</p> <p>Pour plus d’informations, voir <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md">Vue d’ensemble de l’équipe de projet</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project tracking]</td> 
   <td>Les données utilisées pour mesurer l’intégrité et la portée d’un projet</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Projected]</td> 
   <td> <p>Une estimation de la date et de l’heure d’achèvement du travail en fonction du nombre d’heures prévues et du pourcentage terminé d’une tâche, d’un problème ou d’un projet.</p> <p>Cet élément fait référence aux dates ou à la [!UICONTROL Duration] des tâches, des problèmes ou des projets. En règle générale, il désigne les dates et les durées les plus proches de la durée de vie des éléments de travail, une fois que certains travaux sont terminés ou qu’un certain temps s’est écoulé. </p> <p>Par exemple, la [!UICONTROL Projected Completion Date] d’une tâche est la date à laquelle [!DNL Workfront] estime qu’elle se terminera, en fonction du travail accompli jusqu’à présent, du nombre de personnes qui y sont affectées et du temps écoulé depuis la date de début.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof Deadline]</td> 
   <td> <p>Dans les rapports contenant l’objet [!UICONTROL Document Version] (tels que des rapports de [!UICONTROL Document Version] ou de [!UICONTROL Proof Approval]), ce champ affiche le jour de la semaine, la date, l’heure et l’année d’échéance de la relecture.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof Decision]</td> 
   <td> <p>Dans les rapports contenant l’objet [!UICONTROL Document Version] (tels que des rapports de [!UICONTROL Document Version] ou de [!UICONTROL Proof Approval]), ce champ affiche le statut de décision de l’épreuve (en attente, modifications requises, ou approuvé).</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof Name]</td> 
   <td> <p>Dans les rapports contenant l’objet [!UICONTROL Document Version] (tels que des rapports de [!UICONTROL Document Version] ou de [!UICONTROL Proof Approval]), ce champ affiche le nom de l’épreuve.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof Pages]</td> 
   <td> <p>Dans les rapports contenant l’objet [!UICONTROL Document Version] (tels que des rapports de [!UICONTROL Document Version] ou de [!UICONTROL Proof Approval]), ce champ affiche le nombre de pages incluses dans l’épreuve.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof Progress]</td> 
   <td> <p>Dans les rapports contenant l’objet [!UICONTROL Document Version] (tels que des rapports de [!UICONTROL Document Version] ou de [!UICONTROL Proof Approval]), affiche le statut de la progression de l’épreuve ([!UICONTROL Sent], [!UICONTROL Opened], [!UICONTROL Commented], [!UICONTROL Decision Made]).</p> <p>Pour plus d’informations, voir <a href="../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md#understanding-progress-and-status" class="MCXref xref">Vue d’ensemble de la progression de la relecture</a> dans <a href="../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md" class="MCXref xref">Vue d’ensemble des statuts et de la progression de la relecture</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proofing]</td> 
   <td>Processus de relecture au cours duquel un ou plusieurs utilisateurs et utilisatrices partagent des commentaires sur le contenu qui doit être modifié dans une image, un document texte, une vidéo ou du contenu web interactif.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Public]</td> 
   <td>Dans une [!UICONTROL Note] ou un [!UICONTROL Document], cette option rend cet objet accessible à d’autres utilisateurs et utilisatrices, voire à des personnes extérieures à [!DNL Workfront]. Pour une [!UICONTROL Help Request Queue], [!UICONTROL Public] signifie que tous les utilisateurs et utilisatrices qui peuvent soumettre des problèmes à un projet peuvent le faire via la zone [!UICONTROL Requests].</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Quality]</td> 
   <td>Perception de la qualité du travail au sein de l’entreprise.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Queue]</td> 
   <td>Également appelée File d’attente du centre d’assistance ou [!UICONTROL Help Request Queue]. Il s’agit d’un projet qui a été publié dans la zone [!UICONTROL Requests] pour permettre aux utilisateurs et utilisatrices de lui soumettre des problèmes. En règle générale, des files d’attente sont créées pour des rubriques particulières, telles que [!UICONTROL Bugs], [!UICONTROL Project Requests], etc.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Queue Properties]</td> 
   <td>Ces paramètres définissent les règles de soumission des problèmes pour un projet publié dans la zone [!UICONTROL Requests].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Queue Topic]</td> 
   <td> <p>Propriété sur une [!UICONTROL Help Request Queue] qui permet aux utilisateurs et utilisatrices qui soumettent un problème de sélectionner une rubrique. Les rubriques peuvent :</p> 
    <ul> 
     <li>être associées à un formulaire de données personnalisées ;</li> 
     <li>affecter automatiquement le problème à un utilisateur ou une utilisatrice, à un rôle ou à une équipe par le biais du jeu de règles de transmission sur la rubrique sélectionnée ;</li> 
     <li>déplacer le problème vers un autre projet ou une autre file d’attente par le biais du jeu de règles de transmission sur la rubrique sélectionnée.</li> 
    </ul> <p>Pour plus d’informations, voir <a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">Créer des rubriques de file d’attente</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Rank]</td> 
   <td> <p>Dans un rapport [!UICONTROL Access Level], vous pouvez indiquer manuellement un [!UICONTROL Rank] du [!UICONTROL Access Level]. Cela vous aide, en tant qu’administrateur ou administratrice [!DNL Workfront], à identifier visuellement le niveau de complexité associé à chaque niveau d’accès. Vous pouvez par exemple attribuer des nombres plus faibles pour les niveaux d’accès plus complexes (niveau [!UICONTROL Plan]) et des nombres plus élevés pour les niveaux d’accès moins complexes (niveau [!UICONTROL Requester]). Vous ne pouvez pas classer les niveaux d’accès standard.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ready]</td> 
   <td> <p>Ce champ d’un rapport de tâche indique si une tâche [!UICONTROL Agile] a été marquée comme [!UICONTROL Ready] sur la liste d’attente. Cet indicateur s’applique uniquement aux tâches [!UICONTROL Agile], qui sont des tâches affectées à une équipe [!UICONTROL Agile]. </p> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Record]</td> 
   <td> <p>Dans Workfront Planning, un enregistrement est une instance unique d'un type d'enregistrement.</p>
<p>Une fois qu’un type d’enregistrement a été ajouté à un espace de travail, vous pouvez commencer à ajouter des enregistrements de ce type sur la page du type d’enregistrement.</p>
<p>Par exemple, « Campagne » peut être un type d’enregistrement et « Campagne d’été pour la zone EMEA » est un enregistrement du type d’enregistrement Campagne .</p>
<p>Pour plus d’informations sur la création d’enregistrements, voir <a href="/help/quicksilver/planning/records/create-records.md">Créer des enregistrements</a>. </p> <p>Workfront Planning requiert une licence supplémentaire. </p></td> 
  </tr>


<tr> 
   <td>[!UICONTROL Record type]</td> 
   <td> <p>Type d'objet de Workfront Planning.</p>
<p>Contrairement à Workfront, où les types d'objet sont prédéfinis, dans Workfront Planning, vous pouvez créer vos propres types d'objet. Les types d'objet Workfront Planning sont appelés types d'enregistrement.</p>
<p>Par exemple, dans Workfront, les types d’objets Programme, Portfolio, Projet, Tâche ou Problème sont déjà créés.</p>
<p>Dans Workfront Planning, vous pouvez créer tous les types d’enregistrements qui correspondent aux workflows de votre organisation. Vous pouvez ensuite définir la manière dont les types d’enregistrements sont associés les uns aux autres ou aux dépendances des formulaires.</p> Pour plus d’informations sur la création de types d’enregistrements, voir <a href="/help/quicksilver/planning/architecture/create-record-types.md">Créer des types d’enregistrements</a>. </p> <p>Workfront Planning requiert une licence supplémentaire. </p></td> 
  </tr>

<tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Recurrence Frequency]</td> 
   <td> <p>Champ qui s’affiche dans la zone [!UICONTROL Task Details] ou [!UICONTROL Edit Task] d’un parent de tâches récurrentes. Il s’agit de la fréquence à laquelle les tâches de la périodicité se produisent. Pour plus d’informations sur la création de tâches récurrentes, voir <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Créer des tâches récurrentes</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Reference Number]</td> 
   <td> <p>Les projets, tâches et problèmes sont automatiquement associés à un numéro de référence unique au fur et à mesure qu’ils sont créés. Vous pouvez afficher le [!UICONTROL Reference Number] sur la page [!UICONTROL Details] des projets, tâches ou problèmes, ou dans une liste ou un rapport. </p> <p><b>CONSEIL</b><p><br>Vous pouvez vous reporter aux numéros de référence lorsque deux éléments portent le même nom, car les numéros de référence sont toujours uniques. </p> <p>[!DNL Workfront] Des numéros de référence séquentiels au niveau du système sont générés automatiquement. Chaque projet, tâche ou problème obtient le numéro suivant disponible dans la séquence. <br></p> <p>Par exemple, si l’utilisateur ou l’utilisatrice A crée une tâche, [!DNL Workfront] peut affecter automatiquement à la tâche le numéro de référence 100. Si l’utilisateur ou l’utilisatrice B crée un problème juste après, [!DNL Workfront] affecte au problème le numéro de référence 101. Vous ne pouvez pas modifier manuellement les numéros de référence. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Rejection Issue]</td> 
   <td>Dans un projet ou un rapport de tâche, il s’agit du problème créé lorsque l’approbation du projet ou de la tâche est refusée. Pour plus d’informations sur les problèmes de refus, consultez l’article <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Créer un processus d’approbation pour les éléments de travail</a>. </td> 
  </tr>

<tr>
  <td>Types de relation</td>
  <td><p>Les objets Workfront sont toujours connectés les uns aux autres à l’aide de l’un des types de relations suivants :</p>

<ul><li> <b>Un à plusieurs</b> : dans cette relation, un objet peut être connecté à plusieurs autres objets de types différents. Par exemple, un projet peut comporter plusieurs tâches. La relation Projet-Tâches est une relation un-à-plusieurs. Vous ne pouvez pas afficher cette relation dans un rapport à l'aide de l'interface Standard. Vous devez utiliser le mode texte pour afficher les relations un à plusieurs.</li>
  <li><b>Un à un</b> : dans cette relation, un objet ne peut être connecté qu’à un autre objet d’un type différent. Par exemple, un projet ne peut avoir qu’un seul groupe. La relation Projet-Groupe est une relation un-à-un. Vous pouvez afficher des relations un-à-un entre des objets dans un rapport standard.</li>
  <li><b>Plusieurs à un</b> : dans cette relation, plusieurs objets ne peuvent être connectés qu’à un seul autre objet d’un type différent. Par exemple, plusieurs tâches peuvent être connectées au même projet. La relation Tâches-Projet est une relation multiple-à-un. Vous pouvez afficher des relations multiples-à-un entre des objets dans un rapport standard. </li>
  <li><b>Plusieurs à plusieurs</b> : dans cette relation, plusieurs objets du même type peuvent être connectés à plusieurs objets d’un type différent. Par exemple, plusieurs utilisateurs peuvent appartenir à plusieurs autres équipes, et les équipes peuvent appartenir à plusieurs utilisateurs. Vous ne pouvez pas afficher cette relation dans un rapport à l'aide de l'interface Standard. Vous devez utiliser le mode texte pour afficher les relations multiples à multiples. </li> </ul>
  </td></tr>
<tr> 
   <td>[!UICONTROL Remaining Risk Cost]</td> 
   <td> <p>Champ de projet qui indique la différence entre le [!UICONTROL Planned Risk Cost] d’un projet et le total de tous les [!UICONTROL Actual Costs] de tous les risques du projet. </p> <p>Le [!UICONTROL Remaining Risk Cost] d’un projet est calculé à l’aide de la formule suivante :</p> <p><code>[!UICONTROL Remaining Risk Cost] = Project [!UICONTROL Planned Risk Cost] - SUM([!UICONTROL Actual Cost] for all risks)</code> </p> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Replanning]</td> 
   <td>Modification des dates d’un projet pour résoudre ou surmonter les problèmes. Par exemple, un projet qui est en attente depuis plusieurs mois doit être replanifié pour refléter des dates précises. Il s’agit d’une opération manuelle d’ajustement des dates du projet ou des tâches. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Report]</td> 
   <td>Graphique ou tableau contenant des informations sur un objet [!DNL Workfront] donné et ses attributs associés.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Request]</td> 
   <td> <p>Type de problème qui est trié dans une file d’attente centralisée unique et qui n’a aucun rapport avec un effort de travail en cours.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Request Queue]</td> 
   <td>Liste d’attente des problèmes gérés par un processus de trafic et de triage.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Request velocity]</td> 
   <td>Durée totale du cycle de travail pour la prise en charge et la réalisation d’une demande.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Requester]</td> 
   <td>Généralement, un type de licence. Un utilisateur ou une utilisatrice disposant d’une licence de demande peut envoyer une nouvelle demande de travail dans le système.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Reserved Time]</td> 
   <td>Jours spécifiés de congés personnels d’un utilisateur ou d’une utilisatrice indiquant que cette personne ne sera pas disponible pour le travail. Voir « [!UICONTROL Non Work Days] ».</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resolve Issue]</td> 
   <td> <p>Dans un rapport de problème, utilisez ce champ dans les vues ou les filtres pour faire référence au problème qui résout le problème. </p> <p>Pour plus d’informations sur l’affichage des objets de résolution dans les rapports, voir <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">Afficher les information des objets résolvables et de résolution dans un rapport</a> dans <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Vue d’ensemble des objets de résolution et résolvables</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resolve Project]</td> 
   <td> <p>Dans un rapport de problème, utilisez ce champ dans les vues ou les filtres pour faire référence au projet qui résout le problème. </p> <p>Pour plus d’informations sur l’affichage des objets de résolution dans les rapports, voir <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">Afficher les information des objets résolvables et de résolution dans un rapport</a> dans <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Vue d’ensemble des objets de résolution et résolvables</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resolve Task]</td> 
   <td> <p>Dans un rapport de problème, utilisez ce champ dans les vues ou les filtres pour faire référence à la tâche qui résout le problème. </p> <p>Pour plus d’informations sur l’affichage des objets de résolution dans les rapports, voir <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">Afficher les information des objets résolvables et de résolution dans un rapport</a> dans <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Vue d’ensemble des objets de résolution et résolvables</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resource]</td> 
   <td>Utilisateurs et utilisatrices ou rôles existant dans [!DNL Workfront] et qui sont affectés aux équipes de projet, aux tâches et aux problèmes. Ils sont chargés de terminer le travail associé aux projets, tâches ou problèmes. </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Resource Estimates</td> 
    <td>This report captures information about an area in  Workfront that has been removed. The report might display legacy information but it does not update with current data. Although not recommended, you may update the information in this report using the API. For information about how you estimate resources for projects, see <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Resource Planner overview</a>. </td> 
   </tr>
   <td>Resource Grid</td> 
   <td>A visual table showing the allocation of resources.</td> 
  </tr> -->
  <tr> 
   <td>[!UICONTROL Resource Management]</td> 
   <td> <p>[!UICONTROL Resource Management] est un ensemble d’outils d’entreprise qui vous permet de prévoir avec précision l’utilisation de vos ressources en fonction de leur disponibilité, de sorte que le travail à effectuer soit achevé dans le respect des délais et du budget. </p> <p>Grâce aux outils de gestion des ressources, vous pouvez planifier des capacités à long terme et des besoins de planification à court terme pour vos ressources. </p> <p>Pour plus d’informations sur la gestion des ressources dans [!DNL Workfront], voir <a href="../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md">Commencer avec la gestion des ressources</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resource Manager IDs]</td> 
   <td><p>Dans un rapport de projet, vous pouvez utiliser cette option lors de la création d’un filtre pour trouver une personne gestionnaire de ressources spécifique. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resource Managers]</td> 
   <td> <p>Dans un rapport de projet ou en mode Liste, il s’agit d’un champ d’information qui affiche les utilisateurs et utilisatrices désignés pour exécuter des activités de gestion des ressources sur le projet.  Lorsque vous utilisez « [!UICONTROL Resource Managers] » dans un rapport, une liste de personnes gestionnaires de ressources s’affiche, chaque personne gestionnaire membre du projet étant séparée par une virgule. Vous pouvez désigner jusqu’à 30 personnes gestionnaires de ressources pour un projet donné.</p> <p>Pour plus d’informations, voir l’article <a href="../../../manage-work/projects/planning-a-project/designate-resource-managers-for-projects-and-templates.md">Désigner des personnes gestionnaires de ressources pour un projet ou un modèle</a>.</p> </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Resource Planner Budgeted Hours] </td> 
   <td>Heures budgétées pour le projet et ressources qui lui sont associées dans le [!UICONTROL Resource Planner]. Voir aussi « [!UICONTROL Budgeted Hours] » dans cet article. </td> 
  </tr>  
  <tr> 
   <td>[!UICONTROL Resource Planner] </td> 
   <td>Un outil [!DNL Workfront] avancé qui vous permet d’afficher et de gérer des ressources entre les projets, les fonctions ou les utilisateurs et utilisatrices. Pour plus d’informations, voir <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Vue d’ensemble du planificateur de ressources</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resource Planner Budgeted Labor Cost]</td> 
   <td> <p>Il s’agit du coût associé aux heures budgétées pour les fonctions de projet à l’aide du planificateur de ressources. </p> <p>Voir aussi « Coût budgété de la main-d’œuvre » dans cet article. </p> </td>

</tr> 
  <tr> 
   <td>[!UICONTROL Resource Pools]</td> 
   <td> <p>Les groupes de ressources sont des groupes d’utilisateurs et d’utilisatrices qui peuvent être associés à un projet. Les utilisateurs et utilisatrices du même groupe de ressources appartiennent généralement au même service, possèdent des compétences similaires ou complémentaires ou sont financés par le même budget. Vous pouvez associer plusieurs groupes de ressources à un projet ou à un utilisateur ou une utilisatrice. Un groupe de ressources peut être attribué exclusivement à un projet ou partagé par plusieurs projets.</p> 
   <p>Pour plus d’informations sur les groupes de ressources, voir <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref">Vue d’ensemble des groupes de ressources</a>.</p> 
   <p>Dans les rapports de projet, les groupes de ressources affichent tous les groupes associés à un projet. Cet objet ne peut pas être utilisé dans un regroupement.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resource Utilization]</td> 
   <td>Rapport affichant le nombre d’heures disponibles pendant une certaine période et le nombre d’heures prévues pour chaque utilisateur ou utilisatrice du rapport. Il est également calculé en [!UICONTROL Average Hours Per Day] et en pourcentage d’attribution.</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Result]</td> 
   <td>Dans [!DNL Workfront Goals], un résultat est un indicateur de progression pour un objectif. Il peut s’agir d’un nombre, d’une valeur de pourcentage ou d’un montant monétaire que vous mettez à jour manuellement. Vous ne pouvez pas afficher les résultats dans un rapport et vous ne pouvez pas y accéder via l’API [!DNL Workfront]. Pour plus d’informations sur les activités, voir <a href="../../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md" class="MCXref xref">Prise en main des résultats et des activités dans les Objectifs Adobe Workfront</a>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Revenue]</td> 
   <td>Montant facturable pour la tâche ou le projet. Le montant peut être horaire, fixe ou une combinaison des deux.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Revenue Type]</td> 
   <td>Le type de revenu détermine la manière dont la tâche va augmenter les revenus. Voici quelques exemples : [!UICONTROL Fixed Hourly], [!UICONTROL Role Hourly] et [!UICONTROL Role Hourly w/Cap]. Pour plus d’informations sur le suivi des revenus dans [!DNL Workfront], voir <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Vue d’ensemble de la facturation et des revenus</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Reviewer]</td> 
   <td>Généralement, un type de licence. Une personne disposant d’une licence [!UICONTROL Reviewer] peut passer en revue et approuver des éléments de travail dans le système.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Risk]</td> 
   <td> <p>Cela peut faire référence aux concepts suivants dans la section [!DNL Workfront] :</p> 
    <ul> 
     <li> <p>Champ d’un projet qui indique à quel point un projet peut être risqué. Vous pouvez hiérarchiser l’exécution de vos projets en fonction du niveau de risque. Les projets peuvent présenter les niveaux de risque suivants :</p> <p>- [!UICONTROL Very Low]</p> <p>- [!UICONTROL Low]</p> <p>- [!UICONTROL Medium]</p> <p>- [!UICONTROL High]</p> <p>- [!UICONTROL Very High]</p> <p>Les niveaux de risques que vous indiquez pour un projet ne peuvent pas être personnalisés. </p> <p> Pour plus d’informations sur la mise à jour du risque d’un projet, voir la section « Paramètres des projets » de l’article <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Modifier des projets</a>. Vous pouvez afficher le champ des risques d’un projet dans les rapports. </p> </li> 
     <li> <p>Événement qui peut se produire pendant la durée d’un projet et qui identifie un impact potentiel sur le coût, la portée ou le planning du projet. Vous définissez les risques potentiels pour un projet et associez une probabilité qu’ils se produisent ou un coût au moment de la création du business case du projet. Pour plus d’informations sur l’ajout de risques au business case du projet, voir « Créer et modifier des risques sur les projets ». </p> <p>Vous ne pouvez pas afficher les risques définis dans le [!UICONTROL Business Case] dans les rapports. Vous ne pouvez afficher que plusieurs types de coûts de risque dans les rapports et les listes. </p> </li> 
    </ul> </td>

</tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Risk Cost]</td> 
   <td> <p>Coût associé aux risques sur un projet. Vous trouverez ci-dessous les coûts de risque associés aux projets que vous pouvez afficher dans les rapports :</p> 
    <ul> 
     <li> <p>[!UICONTROL Actual Cost] : champ concernant un risque qui indique le coût réel du risque qui s’est produit. Outre les rapports et les listes, vous pouvez les localiser dans la zone [!UICONTROL Edit Risk] lors de la modification ou de la création d’un risque. </p> <p>Pour les coûts de projet, de tâche ou de problème, voir « [!UICONTROL Actual Cost] » dans cet article. </p> </li> 
     <li> <p>[!UICONTROL Planned Risk Cost] : champ d’un projet qui indique le total des [!UICONTROL Potential Risk Costs] pour le projet. Voir aussi « [!UICONTROL Planned Risk Cost] » dans cet article. </p> <p>Pour plus d’informations sur le coût potentiel des risques voir <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">Calculer le coût potentiel des risques</a>. </p> </li> 
     <li> <p>[!UICONTROL Remaining Risk Cost] : champ d’un projet qui affiche la différence entre le total des [!UICONTROL Actual Costs] de tous les risques et le [!UICONTROL Planned Risk Cost]. Voir aussi « Coût restant des risques » dans cet article. </p> </li>
    </ul> </td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL Risk Management]</td> 
   <td>Processus permettant d’identifier, d’atténuer et de surveiller les risques.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Role]</td> 
   <td>Voir « [!UICONTROL Job Role] » dans cet article.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Routing]</td> 
   <td>Affectation ou déplacement automatique d’un problème, généralement en raison d’une rubrique de file d’attente ou au moyen de l’option Itinéraire par défaut (règle de transmission) pour la file d’attente.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Routing Rule]</td> 
   <td>Paramètre sur les projets et les rubriques de la file d’attente qui attribue automatiquement un problème à une personne, un rôle ou une équipe, ou qui déplace le problème vers un autre projet ou une rubrique de file d’attente. Les règles de transmission sont généralement utilisées avec les files d’attente de demande d’aide pour affecter automatiquement les problèmes entrants.</td> 
  </tr> 
 </tbody> 
</table>

## S - U

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nom de l'objet</th> 
   <th>Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Saved Search]</td> 
   <td>Recherche pour laquelle les critères de recherche ont été enregistrés. Les recherches enregistrées permettent d’exécuter des recherches à nouveau sans saisir les critères de recherche à nouveau.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Scenario] (dans [!DNL Workfront Fusion]) </td> 
   <td> <p>Un scénario est une série d’étapes (modules) qui indiquent la façon dont les données doivent être transférées et transformées entre les applications/les services.</p> <p>Pour plus d’informations sur les scénarios dans [!DNL Workfront Fusion], consultez <a href="https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/scenario-overview">[!DNL Adobe Workfront Fusion]Vue d’ensemble du scénario</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Scenario] (dans le [!DNL Workfront Scenario Planner]) </td> 
   <td> <p>Dans le [!DNL Scenario Planner], un scénario est la copie d’un plan. </p> <p>Le [!DNL Scenario Planner] nécessite une licence supplémentaire. Pour plus d’informations sur le [!DNL Workfront Scenario Planner], consultez <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">Vue d’ensemble du [!DNL Scenario Planner]</a>. </p> <p>Pour plus d’informations sur la création de scénarios, consultez <a href="../../../scenario-planner/create-and-compare-scenarios-for-a-plan.md">Créer et comparer des scénarios de plan dans le [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Schedule]</td> 
   <td>Planning de travail hebdomadaire, y compris les horaires de travail, combiné avec les jours de congé (par exemple les jours fériés) et les jours exceptionnels (par exemple, un samedi travaillé). Vous pouvez associer des plannings à des projets et des utilisateurs et utilisatrices.</td> 
  </tr> 
<tr> 
   <td>[!UICONTROL Schedule Performance Index (SPI)]</td> 
   <td><p>L’[!UICONTROL Schedule Performance Index (SPI)] décrit la relation entre le planning prévu et le planning réel. Adobe Workfront calcule le SPI au niveau du projet et des tâches. Les responsables de projet examinent cette mesure pour déterminer si les tâches ou les projets sont actuellement en avance ou en retard sur le planning.</p>
  <p>Pour plus d'informations, voir <a href="/help/quicksilver/manage-work/projects/project-finances/calculate-spi.md">Calculer l'indice de performance horaire (IHP)</a>

</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Schedule Exemption]</td> 
   <td>Connu également sous le nom [!UICONTROL Modified Shift]. Jours planifiés par opposition aux heures de travail hebdomadaires régulières définies par le planning. Par exemple, un samedi de travail planifié, lorsque le planning prévoit uniquement les jours de travail du lundi au vendredi, serait une [!UICONTROL Schedule Exemption].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Scheduled Report]</td> 
   <td> <p>Lorsque vous créez un rapport de rapports, vous pouvez afficher des informations sur les plannings du rapport, si la diffusion du rapport est planifiée à l’aide du champ [!UICONTROL Scheduled Report]. Ce champ affiche plusieurs valeurs, une pour chaque planning de chaque rapport, dans une liste à puces. Pour plus d’informations sur les plannings de rapports, consultez l’article <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md" class="MCXref xref">Vue d’ensemble de la diffusion des rapports</a>.</p> <p>Comme ce champ affiche plusieurs valeurs, il ne peut pas être utilisé dans un regroupement. Vous pouvez y accéder uniquement dans un filtre ou une vue. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Scope Change]</td> 
   <td>Un [!UICONTROL Audit Trail] qui, s’il est actif, génère une note chaque fois que la portée d’un projet ou d’une tâche est modifiée, par exemple si une [!UICONTROL Task Duration] ou les [!UICONTROL Predecessors] sont modifiés.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Section]</td> 
   <td>Zone de l’écran, avec son propre en-tête, créée pour organiser les données personnalisées pour améliorer l’affichage.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Section Break]</td> 
   <td>Espace ou bordure entre les sections.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Security]</td> 
   <td>Paramètres permettant à un utilisateur ou une utilisatrice d’interagir avec certains objets du système et non avec d’autres. Consultez également « [!UICONTROL Access Levels] » dans cet article.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Setup]</td> 
   <td>Zone dans laquelle les administrateurs et les administratrices peuvent définir les configurations et les préférences du système.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Severity]</td> 
   <td> <p>[!UICONTROL Severity] indique la probabilité qu’un élément ait un impact sur l’achèvement du travail. Par exemple, un problème de [!UICONTROL Severity] élevée peut complètement bloquer l’achèvement d’une tâche, mais un problème de [!UICONTROL Severity] faible peut être purement esthétique.</p> <p>Pour plus d’informations, consultez <a href="../../../manage-work/issues/issue-information/update-issue-severity.md" class="MCXref xref">Mettre à jour la gravité d’un problème</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Severities]</td> 
   <td>Consultez « [!UICONTROL Severity] » dans cet article.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sharing]</td> 
   <td>Action permettant à d’autres utilisateurs et utilisatrices d’afficher ou de modifier un élément spécifique dans [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Slack Date]</td> 
   <td>Dans une vue de tâche ou un rapport, la [!UICONTROL Slack Date] affiche la date exacte à laquelle une tâche aura un impact sur la [!UICONTROL Completion Date] du projet. Pour plus d’informations sur la [!UICONTROL Slack Date] d’une tâche, consultez <a href="../../../manage-work/tasks/task-information/task-slack-date.md" class="MCXref xref">Vue d’ensemble de la date de marge de la tâche</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Smart Assignments]</td> 
   <td> <p>Lors de l’attribution de tâches ou de problèmes aux utilisateurs et aux utilisatrices, [!DNL Workfront] émet des recommandations ([!UICONTROL Smart Assignments]) aux utilisateurs et utilisatrices qui sont les mieux placés pour terminer le travail, en fonction du temps dont ils disposent pour le terminer et de leur relation avec le projet.</p> <p>Pour plus d’informations, consultez <a href="../../../manage-work/tasks/assign-tasks/smart-assignments.md" class="MCXref xref">Vue d’ensemble des affectations intelligentes</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source]</td> 
   <td> <p>Indique l’objet parent d’un autre objet. Par exemple, un document joint à une tâche porte le nom de la tâche dans le champ [!UICONTROL Source] d’un rapport ou d’une vue [!UICONTROL Document] ; un problème consigné sous un projet porte le nom du projet dans le champ [!UICONTROL Source] d’un rapport ou d’une vue Problème. </p> 
   <p>Les rapports suivants affichent une colonne Source dans laquelle vous pouvez afficher des informations sur l’objet parent :</p>
  <ul><li>Rapports sur les événements</li>
    <li>Rapports sur les heures</li>
    <li>Rapports sur les documents </li>
    </ul>
   <p>Si les personnes ne disposent pas d’autorisations sur l’objet parent d’un problème, d’une heure ou d’un document, la colonne Source du rapport s’affiche vide, même lorsque le rapport est configuré pour s’afficher ou pour être diffusé avec les droits d’accès d’une autre personne. </p>
   <p> Pour afficher des informations sur l’objet parent dans le rapport, il est recommandé d’ajouter une colonne pour l’objet parent dans laquelle vous pouvez afficher le nom du parent. </p>
    <p>Par exemple, vous pouvez ajouter l’un des éléments suivants à un rapport avec une colonne Source : </p>
    <ul><li>Les colonnes Nom du projet, Nom de la tâche ou Nom du problème dans un rapport sur les documents ou les heures.</li>
    <li>Colonnes Nom du projet ou Nom de la tâche pour un rapport sur les problèmes. </li> </ul>
    Pour plus d’informations, voir <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md">Exécuter et diffuser un rapport avec les droits d’accès d’une autre personne</a>.

</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Start Date]</td> 
   <td> <p>Date à laquelle le travail sur un élément est défini pour commencer. Il existe plusieurs dates de début dans [!DNL Workfront] : </p> 
    <ul> 
     <li>[!UICONTROL Planned]</li> 
     <li>[!UICONTROL Actual]</li> 
     <li>[!UICONTROL Projected] </li> 
    </ul> <p>Dans un [!UICONTROL Rate report], il s’agit de la date à laquelle commence un nouveau taux de facturation pour une fonction au niveau du projet. Les heures associées au projet qui se trouvent après cette date sont multipliées par ce taux de facturation pour calculer les revenus sur le projet. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Status]</td> 
   <td> <p>Indicateur utilisé pour signaler la position d’un workflow d’un élément de travail ou d’un objectif stratégique.</p> <p>Pour les projets, le [!UICONTROL Status] est un paramètre du projet qui indique si le projet est :</p> 
    <ul> 
     <li>[!UICONTROL Current]</li> 
     <li>[!UICONTROL On Hold] </li> 
     <li>[!UICONTROL Complete] </li> 
     <li>[!UICONTROL Dead]</li> 
    </ul> <p>Pour plus d’informations sur le statut d’un projet, voir <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md">Accéder à la liste des statuts des projets système</a>.</p>
    <p>Pour les tâches, le [!UICONTROL Status] est un paramètre de la tâche qui indique si la tâche est :</p> 
    <ul> 
     <li>[!UICONTROL New]</li> 
     <li>[!UICONTROL In Progress]</li> 
     <li>[!UICONTROL Complete]</li> 
    </ul> <p>Pour plus d’informations sur le statut de la tâche, voir <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md">Accéder à la liste des statuts des tâches système</a>.</p> <p>Pour les problèmes, le [!UICONTROL Status] est un paramètre qui indique si le problème est :</p> 
    <ul> 
     <li>[!UICONTROL New]</li> 
     <li>[!UICONTROL In Progress]</li> 
     <li>[!UICONTROL Awaiting Feedback]</li> 
     <li>[!UICONTROL On Hold]</li> 
     <li>[!UICONTROL Resolved]</li> 
     <li>[!UICONTROL Won't Resolve]</li> 
     <li>[!UICONTROL Cannot Duplicate]</li> 
     <li>[!UICONTROL Verified Complete]</li> 
     <li>[!UICONTROL Reopened]</li> 
    </ul> <p>Pour plus d’informations sur les statuts de problème, voir <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">Accéder à la liste des statuts des problèmes système</a>.</p> 
    <p>Pour les objectifs stratégiques, le [!UICONTROL Status] est un paramètre de l’objectif qui indique si l’objectif est :</p> 
     <ul> 
      <li>[!UICONTROL Active]</li> 
      <li>[!UICONTROL Draft]</li> 
      <li>[!UICONTROL Inactive]</li> 
      <li>[!UICONTROL Closed]</li> 
     </ul> 
     <p>Pour plus d’informations sur les objectifs stratégiques, voir aussi « [!UI[!UICONTROL Goal] » or « [!UICONTROL Goals] » dans cet article. </p> 
     <p>Pour les objectifs stratégiques, ce champ n’est visible que si votre entreprise a acheté [!DNL Workfront Goals]. Pour plus d’informations sur la gestion des objectifs stratégiques à l’aide de [!DNL Workfront Goals], voir Vue d’ensemble de <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals]</a>. </p>
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Status Change]</td> 
   <td>Un [!UICONTROL Audit Trail]. Une note est générée lorsqu’un utilisateur ou une utilisatrice modifie le statut du projet, de la tâche ou du problème.</td> 
  </tr> 
  <tr> 
   <td>Icônes de statut</td> 
   <td> <p>Vous pouvez ajouter le champ intégré [!UICONTROL Status Icons] en tant que colonne dans vos vues afin d’améliorer la visibilité sur les points clés de vos objets, tels que les suivants :</p> 
    <ul> 
     <li>Un objet est associé à des documents</li> 
     <li>Un objet est associé à un processus d’approbation</li> 
     <li>Un objet est associé à des notes supplémentaires</li> 
     <li>Une dépense est facturable ou remboursable.</li> 
     <li>Une tâche est sur un chemin critique</li> 
     <li>Un utilisateur ou une utilisatrice appartient à une entreprise, à une équipe ou se trouve dans un fuseau horaire différent.</li> 
    </ul> <p>Vous pouvez ajouter le champ [!UICONTROL Status Icons] dans les vues des objets suivants :</p> 
    <ul> 
     <li>[!UICONTROL Tasks]</li> 
     <li>[!UICONTROL Issues]</li> 
     <li>[!UICONTROL Projects]</li> 
     <li>[!UICONTROL Template Tasks]</li> 
     <li>[!UICONTROL Templates]</li> 
     <li>[!UICONTROL Expenses]</li> 
     <li>[!UICONTROL Documents]</li> 
     <li>[!UICONTROL Users]</li> 
    </ul> <p>Pour plus d’informations, voir <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">Icônes de statut intégrées dans les vues</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Status Update]</td> 
   <td> <p>Dans un rapport de projet, de tâche ou de problème, ce champ affiche la mise à jour du statut la plus récente fournie par les personnes propriétaires d’objets dans la zone « [!UICONTROL Updates] ».Pour les projets, cela se rapporte aux commentaires effectués par la personne propriétaire du projet ; pour les tâches et les problèmes, cela se rapporte aux commentaires effectués par les personnes cessionnaires.</p> 
   <p> Les commentaires effectués lors de la mise à jour du statut d’un objet ne s’affichent pas dans la colonne [!UICONTROL Status Update].</p> <p>Pour afficher les statuts « [!UICONTROL New] », « [!UICONTROL In Process] » et « [!UICONTROL Complete] », utilisez la colonne [!UICONTROL Status].</p> <p>Pour plus d’informations sur les statuts, voir l’article <a href="../../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref">Mettre à jour le statut des tâches</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Statuses]</td> 
   <td>Voir « [!UICONTROL Status] » dans cet article.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Storyboard]</td> 
   <td>Graphique qui représente le statut des histoires (tâches dans la méthodologie Agile) et leur progression vers leur achèvement.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Story Hours]</td> 
   <td>Mesure utilisée pour mesurer la difficulté ou la complexité d’une histoire. Les équipes Agile peuvent choisir d’utiliser les heures ou les points.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Story Points]</td> 
   <td>Mesure utilisée pour mesurer la difficulté ou la complexité d’une histoire. Les équipes Agile peuvent choisir d’utiliser les heures ou les points.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Strategic]</td> 
   <td>Travail à long terme qui modifie l’organisation ou le fonctionnement de l’organisation.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Strategic Alignment]</td> 
   <td>Mesure et alignement des objectifs de l’entreprise entre les portfolios et les programmes.</td> 
  </tr>

<tr> 
   <td><code>[!UICONTROL stretch]</code></td> 
   <td><p>Cet élément est utilisé dans les colonnes du rapport lors de l’utilisation de l’interface du mode Texte. </p>
   <p>L’élément <code>[!UICONTROL stretch]</code> est utilisé pour identifier les colonnes qui occupent un espace supplémentaire dont la vue n’a pas besoin. La largeur de l’interface utilisateur de l’espace de travail pour un utilisateur ou ue utilisatrice type est d’environ 850 pixels. Cela signifie que si vous avez une vue dotée de quatre colonnes (150 pixels chacune), votre vue occupe 600 des 850 pixels. Il y a 250 pixels supplémentaires dans l’interface utilisateur qui seront ajoutés aux colonnes pour lesquelles un pourcentage d’extension a été fourni. </p>
   <p>L’étirement d’une colonne est appliqué lorsque vous utilisez la ligne de code supplémentaire <code>[!UICONTROL usewidths=true]</code> pour au moins une des colonnes de la vue. 
   </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Subscribers]</td> 
   <td> <p>Les utilisateurs et utilisatrices qui s’abonnent à des projets, des tâches ou des problèmes.</p> <p>Lorsque vous utilisez ce champ dans un rapport, une liste de personnes abonnées s’affiche, chaque personne étant séparée par une virgule.</p> <p>Pour plus d’informations, consultez l’article <a href="../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md" class="MCXref xref">S’abonner à des éléments dans [!DNL Adobe Workfront]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Summary Task]</td> 
   <td>Consultez « [!UICONTROL Parent Task] » dans cet article.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Subtask]</td> 
   <td>Tâche enfant, située sous une tâche parent.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL System Governance]</td> 
   <td>Ensemble de politiques qui régit les modifications et la maintenance d’un système.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL System Integration]</td> 
   <td>Processus consistant à lier différents systèmes informatiques et applications logicielles, physiquement ou fonctionnellement, pour qu’ils fontionnent comme un ensemble coordonné.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Task]</td> 
   <td> <p>Activité qui s’inscrit dans un processus de plusieurs étapes vers un objectif final (achèvement du projet).</p>

<p>Les tâches sont des unités de travail plus petites qui terminent finalement un projet, ce qui représente une unité de travail plus grande.</p>
   <p>Les tâches ne peuvent jamais exister indépendamment. Ils font toujours partie d'un projet. </p>
   <p>Pour plus d’informations sur les tâches, voir <a href="../../../manage-work/tasks/task-information/tasks-overview.md" class="MCXref xref">Présentation des tâches</a>.</p> 
   <p>Pour plus d’informations sur la création de tâches, voir <a href="/help/quicksilver/manage-work/tasks/create-tasks/create-tasks-in-project.md">Créer des tâches dans un projet</a>
   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Task Attribute]</td> 
   <td>Autres champs ou objets associés à une tâche et indiquant certains détails sur la tâche. Voici quelques exemples : [!UICONTROL Planned Completion Date] et [!UICONTROL Status].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Task Constraint]</td> 
   <td>Voir « [!UICONTROL Constraint Type] » et « [!UICONTROL Constraint Date] ».</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Task Management]</td> 
   <td>Ensemble de politiques qui détermine les seuils pour la création, l’affectation, la fermeture et la visibilité des tâches.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Task Owner]</td> 
   <td>Équipe ou personne responsable de l’estimation de l’effort et de l’achèvement de la tâche.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Team]</td> 
   <td> <p>Ensemble d’utilisateurs et d’utilisatrices travaillant à des objectifs similaires, notamment des objectifs commerciaux. Ces utilisateurs et utilisatrices peuvent être affectés collectivement à un élément de travail en y affectant l’équipe.</p> <p>Pour plus d’informations sur les équipes, consultez <a href="../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md" class="MCXref xref">Vue d’ensemble des équipes</a>.</p> <p>Les projets peuvent avoir une [!UICONTROL Project Team], qui comprend tous les utilisateurs, utilisatrices ou rôles associés au travail sur le projet.</p> <p>Pour plus d’informations sur les équipes du projet, voir <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Vue d’ensemble de l’équipe du projet</a></p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode,SnippetConitions_MaturityModel.Ad hoc"> 
    <td>Team Goals</td> 
    <td>Team goals which contribute to the metrics of enterprise or department goals.</td> 
   </tr>
  --> 
  <tr> 
   <td>[!UICONTROL Template]</td> 
   <td> <p>Les modèles de projet sont des compositions génériques de vos projets les plus reproductibles. Pour gagner du temps lorsque vous créez un projet, vous pouvez définir des tâches, des rubriques de files d’attente et des formulaires personnalisés, mais aussi joindre des documents ou des approbations. </p> <p>Vous pouvez joindre des modèles à des projets existants ou les utiliser pour créer des projets. Toutes les informations spécifiées sur le modèle sont transférées vers les projets créés à l’aide de celui-ci. </p> <p>Pour plus d’informations sur les modèles, consultez <a href="../../../manage-work/projects/create-and-manage-templates/project-template-overview.md">Vue d’ensemble des modèles de projet</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Template Task]</td> 
   <td>Tâche qui fait partie d’un modèle. Les tâches du modèle deviennent des tâches dans le projet créé à l’aide du modèle.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Thread]</td> 
   <td>[!UICONTROL Note] et son ensemble de réponses liées à une rubrique particulière.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Thumbnail]</td> 
   <td> <p> Dans une liste ou un rapport de [!UICONTROL Document], une prévisualisation du document s’affiche dans une miniature. </p> <p> Sélectionnez <strong>[!UICONTROL Thumbnail]</strong> pour afficher une miniature de 33 à 66 pixels de large dans le rapport. </p> <p>La taille de la miniature s’ajuste lorsque vous modifiez la largeur de la colonne dans une liste ou un rapport.</p> <p>Consultez aussi « [!UICONTROL Large Thumbnail] » dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Time Off]</td> 
   <td>Vous pouvez créer un rapport de [!UICONTROL Time Off] afin d’afficher le moment où les utilisateurs et les utilisatrices ont indiqué des congés dans leur profil. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Timesheet]</td> 
   <td> <p>Fiche de temps qui permet aux utilisateurs et utilisatrices de consigner les heures effectives passées à travailler sur des projets, des tâches ou des problèmes, ou les heures consacrées à d’autres activités non liées au travail, telles que des réunions ou des formations. En plus de consigner les heures de travail, vous pouvez aussi spécifier si elles sont liées au travail ou si elles correspondent à des frais généraux en utilisant les types d’heures pour catégoriser vos entrées de temps. Pour plus d’informations sur les feuilles de temps, consultez la section <a href="../../../timesheets/timesheets/timesheets-overview.md">Vue d’ensemble des feuilles de temps</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Timesheet Profile]</td> 
   <td> <p>Un [!UICONTROL Timesheet Profile] est un modèle que [!DNL Workfront] utilise pour créer automatiquement des feuilles de temps pour les personnes qui y sont associées. </p> <p>Vous pouvez configurer plusieurs paramètres qui s’appliqueront à chaque feuille de temps lors de sa création. Parmi ces paramètres figurent : la fréquence de création de la feuille de temps (hebdomadaire, toutes les deux semaines, deux fois par mois ou mensuelle), le jour de début de la feuille de temps, les personnes chargées de l’approbation de la feuille de temps, ainsi que les [!UICONTROL Hour Types] disponibles que les utilisateurs et les utilisatrices peuvent associer aux heures enregistrées.</p> </td> 
  </tr> 
  <tr > 
   <td>[!UICONTROL Top Parent ID] </td> 
   <td> <p>Ce champ vous permet d’identifier et de filtrer les données d’un groupe de niveau supérieur et de ses sous-groupes dans une liste ou un rapport.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Top Parent Name] </td> 
   <td> <p>Ce champ vous permet d’identifier les données d’un groupe de niveau supérieur et de ses sous-groupes dans une [!UICONTROL View] pour une liste ou un rapport.</p> <p>Vous pouvez aussi le faire en utilisant le champ [!UICONTROL Top Parent ID].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Total Hours]</td> 
   <td> <p>Dans un [!UICONTROL project report], ce champ affiche la somme arrondie de toutes les heures du projet lors du dernier calcul du financement du projet. Les [!UICONTROL Actual Hours] reflètent les heures exactes consignées sur le projet. En règle générale, les [!UICONTROL Actual Hours] doivent correspondre au [!UICONTROL Total Hours]. Si le champ du [!UICONTROL Total Hours] présente une différence notable par rapport au champ des [!UICONTROL Actual Hours], il est nécessaire de recalculer les finances du projet.</p> <p>Pour plus d’informations sur la façon de recalculer les finances d’un projet, consultez l’article <a href="../../../manage-work/projects/project-finances/recalculate-project-finances.md" class="MCXref xref">Recalculer les finances d’un projet</a>.</p> <p>Dans une vue de feuille de temps [!UICONTROL Standard], ce champ fait référence au nombre total d’heures consignées pour les éléments aux dates affichées sur une feuille de temps. Le champ [!UICONTROL Total Hours] des feuilles de temps dans cette vue intégrée fait référence au champ « [!UICONTROL hoursDuration] » qui calcule dynamiquement la différence en heures entre les dates de début et de fin de la feuille de temps. Il est utilisé pour afficher en rouge la colonne du [!UICONTROL Total Hours] si l’utilisateur ou l’utilisatrice consigne plus d’heures que les heures disponibles dans la période de la feuille de temps. Pour plus d’informations, consultez la section <a href="../../../timesheets/create-and-manage-timesheets/view-total-hours-timesheets.md" class="MCXref xref">Afficher le nombre total d’heures sur la feuille de temps</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tracking Mode]</td> 
   <td> <p>Attribut d’une tâche. Ce champ détermine comment et à quel moment les chronologies prévisionnelles seront mises à jour pour une tâche. Par exemple :</p> 
    <ul> 
     <li>[!UICONTROL User Must Update] nécessite qu’une tâche soit mise à jour manuellement. Sinon, elle passera du statut [!UICONTROL Behind Schedule] au statut [!UICONTROL Late].</li> 
     <li>[!UICONTROL Auto Complete] termine automatiquement une tâche lorsque la date d’échéance, ou la [!UICONTROL Planned Completion Date], est passée.</li> 
    </ul> <p>Pour plus d’informations, consultez la section <a href="../../../manage-work/tasks/task-information/task-tracking-mode.md" class="MCXref xref">Vue d’ensemble du mode de suivi des tâches</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Trigger]</td> 
   <td>Événement qui démarre un scénario.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Trouble Task]</td> 
   <td>Tâche incomplète avec un statut [!UICONTROL Late], [!UICONTROL Behind Schedule], ou [!UICONTROL At Risk].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Unassigned Task]</td> 
   <td>Tâche qui n’est affectée à aucun rôle ni à aucune personne ou équipe.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Update Type]</td> 
   <td> <p>Paramètre d’un projet qui détermine le moment où sa chronologie prévisionnelle sera recalculée. Le [!UICONTROL Update Type] peut avoir les valeurs suivantes :</p> 
    <ul> 
     <li>[!UICONTROL Automatic and On Change]</li> 
     <li>[!UICONTROL Automatic Only]</li> 
     <li>[!UICONTROL Manual Only] </li> 
    </ul> <p>Pour plus d’informations, consultez la section <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Sélectionner le type de mise à jour du projet</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL User]</td> 
   <td>Compte créé dans [!DNL Workfront] pour permettre à une personne de se connecter et d’interagir avec le système.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL User Delegation]</p> </td> 
   <td> <p>Objet pouvant faire l’objet d’un rapport qui vous indique ce qui suit :</p> 
    <ul> 
     <li>Quelles personnes ont délégué la tâche, le problème et les approbations de projet.</li> 
     <li>Quelles personnes ont fait l’objet d’une délégation d’approbations de tâche, de problème et de projet.</li> 
     <li>Quand ces délégations commencent et se terminent.</li> 
    </ul> <p>Pour en savoir plus, voir <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-user-delegation-report.md" class="MCXref xref">Créer un rapport de délégation d’utilisateurs et d’utilisatrices</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL User Interface]</td> 
   <td>Tous les aspects visuels et interactifs de l’application [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL User Interface Preferences]</td> 
   <td>[!UICONTROL User Interface Setup]. Les équipes d’administration [!DNL Workfront] peuvent modifier ces paramètres pour personnaliser certains aspects de l’interface d’utilisation.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Utilization]</td> 
   <td>Disponibilité d’un utilisateur ou d’une utilisatrice ou d’un rôle en fonction du planning affecté, des congés payés et de la charge de travail actuelle.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL User Utilization]</td> 
   <td> <p>Recherche combinée à un rapport qui indique comment les personnes (ressources) sont affectées ou suraffectées. Voir « [!UICONTROL Resource Utilization] » dans cet article.</p> </td> 
  </tr> 
 </tbody> 
</table>

## V - Z

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nom de l'objet</th> 
   <th>Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Velocity]</td> 
   <td>Mesure du temps total du cycle de travail (le temps nécessaire pour terminer un travail) et de la fréquence à laquelle le travail est réalisé dans les délais de l’engagement initial (ratio travail/engagement).</td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL View]</td> 
   <td> <p>Les vues se rapportent à un élément de création de rapports qui permet de modifier les colonnes d’un rapport ou d’une liste d’objets.</p> 
   <p> La vue fait également référence au droit d’un utilisateur ou d’une utilisatrice à afficher uniquement les informations sur un objet, en fonction de son niveau d’accès ou à un niveau de partage d’autorisations sur cet objet.</p> 
   <p>Dans Workfront Planning, les enregistrements s'affichent sur la page Type d'enregistrement dans l'un des types de vue suivants :</p>
   <ul><li>Tableau</li>
   <li>Journal</li>
   <li>Calendrier</li></ul>
   <p>Dans Workfront Planning, les vues incluent les filtres, les regroupements, le tri et d'autres paramètres appliqués aux enregistrements de l'écran.</p> <p>Pour plus d’informations, consultez la section <a href="/help/quicksilver/planning/views/manage-record-views.md">Gérer les vues d’enregistrement</a>.</p>   
   <p>Workfront Planning requiert une licence supplémentaire.</p>
   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL View Icons]</td> 
   <td> <p> Il s’agit du même champ que Icônes de statut, mais il n’est disponible que pour les vues suivantes : </p> 
    <ul> 
     <li> [!UICONTROL Documents] </li> 
    </ul> <p> Pour plus d’informations, voir l’article <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">Icônes de statut intégrées dans les vues</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Views Last Month]</td> 
   <td> <p>Dans une liste de rapports, cela affiche le nombre de fois où le rapport a été consulté au cours du dernier mois.<br>Pour plus d’informations sur les informations d’utilisation dans les listes de rapports, voir l’article <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Afficher l’utilisation des rapports</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Views Last Quarter]</td> 
   <td>Dans une liste de rapports, cela affiche le nombre de fois où le rapport a été consulté au cours du dernier trimestre.<br>Pour plus d’informations sur les informations d’utilisation dans les listes de rapports, voir l’article <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" >Afficher l’utilisation des rapports</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Views Last Year]</td> 
   <td>Dans une liste de rapports, cela affiche le nombre de fois où le rapport a été consulté au cours de la dernière année.<br>Pour plus d’informations sur les informations d’utilisation dans les listes de rapports, voir l’article <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Afficher l’utilisation des rapports</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Views This Month]</td> 
   <td> <p>Dans une liste de rapports, cela affiche le nombre de fois où le rapport a été consulté au cours de ce mois.<br>Pour plus d’informations sur les informations d’utilisation dans les listes de rapports, voir l’article <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Afficher l’utilisation des rapports</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Views This Quarter]</td> 
   <td>Dans une liste de rapports, cela affiche le nombre de fois où le rapport a été consulté au cours de ce trimestre.<br>Pour plus d’informations sur les informations d’utilisation dans les listes de rapports, voir l’article <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Afficher l’utilisation des rapports</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Views This Year]</td> 
   <td>Dans une liste de rapports, cela affiche le nombre de fois où le rapport a été consulté au cours de cette année.<br>Pour plus d’informations sur les informations d’utilisation dans les listes de rapports, voir l’article <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md">Afficher l’utilisation des rapports</a>.</td> 
  </tr>

<tr>
  <td> <code>[!UICONTROL width]</code>
  </td>
<td> Dans un rapport, lors de l’utilisation de l’interface [!UICONTROL Text Mode], il s’agit de la ligne de code dans laquelle vous pouvez spécifier la largeur de chaque colonne en pixels. Workfront fournit une largeur suggérée pour chaque champ. Cependant, selon le type de champ et le format, vous pouvez effectuer des ajustements.
Vous devez utiliser la ligne de code <code>[!UICONTROL usewidths=true]</code> pour appliquer la largeur spécifiée pour la colonne. 
  </td>

</tr>

<tr> 
   <td><code>[!UICONTROL work]</code> </td> 
   <td> <p>Dans un rapport de projet, de tâche ou de problème, l’instruction suivante en mode texte affiche le nombre d’heures prévues du projet, de la tâche ou du problème :</p>
   <code><p>valuefield=work</p>
   <p>valueformat=HTML</p></code> 
   <p>Pour plus d’informations sur l’utilisation du mode texte, voir <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">Vue d’ensemble de la syntaxe du mode texte</a>. </p> 
   <p><b>CONSEIL</b> 
   <p>Dans un rapport de problème, l’ajout de l’un des champs [!UICONTROL Planned Hours] ajoute le champ <code>work </code> au rapport. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work]</td> 
   <td> <p>L’un des deux principaux types de licence. Toutes les personnes qui disposent d’un accès inférieur à celui de la licence [!UICONTROL Plan], mais qui peuvent créer et effectuer des mises à jour dans le système. Un utilisateur ou une utilisatrice disposant d’une licence de travail a plus de capacités qu’une personne détenant une licence [!UICONTROL External], [!UICONTROL Reviewer] ou [!UICONTROL Requester].</p> <p>Pour plus d’informations, consultez la section Vue d’ensemble des licences <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront]</a>.</p> <p>Le travail peut faire référence au [!UICONTROL Planned Hours] pour un projet, une tâche ou un problème.Pour plus d’informations, consultez dans ce tableau le champ « [!UICONTROL work] ». </p> <p><b>CONSEIL</b></p> <p> Dans un rapport sur les problèmes, ajouter l’un des champs de [!UICONTROL Planned Hours] ajoute au rapport le champ <code>work </code>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work Breakdown Structure]</td> 
   <td>Structure hiérarchique des tâches à exécuter par l’équipe de projet en fonction de la relation parent/enfant.</td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL Work Effort] </td> 
   <td> 
    <p>La personne chargée de la gestion du projet peut choisir d’utiliser ce champ à la place du [!UICONTROL Planned Hours] pour estimer l’effort nécessaire pour terminer la tâche. Ce champ n’est visible que lorsque les conditions suivantes sont remplies :</p> 
     <ul> 
      <li> <p>La tâche a un [!UICONTROL Simple Duration Type]. </p> <p><b>CONSEIL</b></p> <p> Lorsque vous mettez à jour la tâche en remplaçant le [!UICONTROL Duration Type] par un autre type, ce champ devient masqué. </p> </li> 
      <li>La personne chargée de la gestion du projet a activé l’option [!UICONTROL Use Work Effort] pour calculer automatiquement le champ [!UICONTROL Planned Hours] du projet. </li> 
     </ul> 
     <p>Pour plus d’informations sur l’utilisation de l’[!UICONTROL Work Effort] au lieu du [!UICONTROL Planned Hours] pour estimer l’effort pour réaliser la tâche, consultez la section <a href="../../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Vue d’ensemble de l’effort de travail</a>. </p> 
     <p>Vous pouvez afficher ce champ dans les listes et rapports de tâches.</p> 
    </td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL Work Item]</td> 
   <td> <p>Ce champ fait référence à des tâches ou à des problèmes dans [!DNL Workfront]. </p> <p>Le rapport [!UICONTROL Work Item] affiche des informations sur les tâches et les problèmes. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work management mix]</td> 
   <td>Un [!UICONTROL Work Performance Indicator] (WPI) mesure la proportion de travail affectée au fonctionnement de votre entreprise par rapport au changement de votre entreprise. L’indicateur WPI vous aide à comprendre, au niveau de l’organisation, si votre stratégie bénéficie d’une réelle répartition du travail.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work Management Resource]</td> 
   <td>Désignation d’une persona dans le système qui peut recevoir du travail ou suivre le temps.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work Management Role and Responsibilities]</td> 
   <td>Définir les personnes propriétaires et les parties prenantes pour gérer la portée, l’exécution et les approbations du problème, de la tâche, du projet, du programme ou du portfolio désigné.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work management SLA]</td> 
   <td>Mesure quantifiable acceptée par toutes les parties prenantes.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work Management Stakeholder]</td> 
   <td>Collection d’utilisateurs et d’utilisatrices ayant un intérêt particulier dans les résultats d’une requête de travail.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work management touchpoints]</td> 
   <td>Enregistrements numérisés de la communication entre les parties prenantes.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work Performance Indicators] </td> 
   <td> <p>Indicateurs de ratio, capacité, vitesse, qualité et engagement.</p> <p>WPI est un acronyme courant pour [!UICONTROL Work Performance Indicator].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work Process]</td> 
   <td> <p>Méthode selon laquelle le travail est reçu, classé par ordre de priorité et exécuté. La manière dont vous exécutez le travail est généralement appelée « workflow » ou « plan de projet » (une liste de tâches avec des dates, des relations antérieures, etc.). </p> <p>Un processus de travail peut être, par exemple, la production d’une seule ressource ou la diffusion d’une campagne multiressources. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Workflow template]</td> 
   <td>Dans le rapport [!UICONTROL Proof Approval], ce champ affiche tous les modèles de workflow associés à une épreuve. Si aucun modèle n’est joint, la colonne est vide.</td> 
  </tr>

<tr> 
   <td>[!UICONTROL Work Time]</td> 
   <td>

<p>Représente le pourcentage de l’équivalent temps complet ([!UICONTROL FTE]) dont dispose l’utilisateur ou l’utilisatrice pour le travail effectif, hors frais généraux. [!UICONTROL Work Time] doit être un nombre décimal inférieur ou égal à 1 et ne peut être égal à 0. Par exemple, une disponibilité de 20 % pour le travail effectif serait de 0,2.</p>
   </p>La valeur par défaut de ce champ est 1, ce qui indique qu’un utilisateur ou qu’une utilisatrice consacre la totalité de son [!UICONTROL FTE] au travail réel lié au projet.  </p>
   <p>Le système utilise ce nombre pour calculer la disponibilité de la personne quant au travail réel lié au projet. </p>
   <p> Les exceptions au planning et les congés peuvent également affecter la capacité de la personne. </p>
   <p>Pour plus d’informations sur la création de plannings dans Workfront, voir <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md">Création d’un planning</a>. </p>
    <p>Workfront calcule la disponibilité d’un utilisateur ou d’une utilisatrice en fonction des préférences de gestion des ressources dans la zone [!UICONTROL Setup]. Pour plus d’informations, voir <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md/">Configurer les préférences de gestion des ressources</a>. </p> 
   <p>Vous pouvez mettre à jour le [!UICONTROL Work Time] d’un utilisateur ou d’une utilisatrice lors de sa modification ou de sa création. Pour plus d’informations, voir <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md">Modifier le profil d’un utilisateur ou d’une utilisatrice</a></p> 
   <b>CONSEIL</b> 
   <p>Définissez la valeur [!UICONTROL Work Time] sur 1 pour indiquer que la personne est disponible pour un travail lié au projet et qu’elle dispose de son équivalent temps complet.</p> 
   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Working time]</td> 
   <td>Dans la documentation Workfront, ce terme est utilisé pour décrire le temps alloué au travail, selon un planning.</td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL workRequiredExpression]</code> </td> 
   <td> <p>Dans un rapport de projet, de tâche ou de problème, l’instruction suivante en mode texte affiche le nombre d’heures prévues du projet, de la tâche ou du problème, suivi du mot « Heures » :</p>
   <code>
   <p>valuefield=workRequiredExpression</p>
   <p>valueformat=HTML</p>
   </code>
    <p>Pour plus d’informations sur l’utilisation du mode texte, voir <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">Vue d’ensemble de la syntaxe du mode texte</a>. </p> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Workspace] </td> 
   <td> <p>Dans Workfront Planning, un espace de travail est un ensemble de types d’enregistrements qui définissent le cycle de vie opérationnel d’une certaine organisation. Un espace de travail est le cadre de travail d’une unité organisationnelle.</p>
   <p>Workfront Planning requiert une licence supplémentaire. </p>
   <p>Pour plus d’informations, voir <a href="/help/quicksilver/planning/architecture/create-workspaces.md">Créer des espaces de travail</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>


