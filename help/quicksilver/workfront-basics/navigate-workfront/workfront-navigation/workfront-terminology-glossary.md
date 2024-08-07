---
content-type: reference
navigation-topic: workfront-navigation
title: Glossaire de la terminologie  [!DNL Adobe Workfront]
description: Le glossaire  [!DNL Adobe Workfront] répertorie les termes couramment utilisés dans l’interface  [!DNL Adobe Workfront]. You can use the glossary when you want to find the definition of concepts you see in the [!UICONTROL Workfront] des rapports, ou vous essayez de comprendre la signification de [!DNL Workfront] concepts définis dans la documentation  [!DNL Workfront] .
author: Alina
feature: Get Started with Workfront
exl-id: 758072b3-775e-4771-9ae9-da0b38580c93
source-git-commit: 6f1f669f7e2235637864a92a40aadbfb19b4310b
workflow-type: tm+mt
source-wordcount: '20384'
ht-degree: 1%

---


# Glossaire de la terminologie [!DNL Adobe Workfront]

<!--Audited: 12/2023-->

>[!IMPORTANT]
>
>Cet article doit être utilisé comme référence pour comprendre les termes que vous pouvez rencontrer dans l’application [!DNL Adobe Workfront], dans la documentation [!DNL Workfront] ou lorsque vous parlez généralement de planification et de gestion du travail. Nous mettons actuellement à jour ces informations et il se peut donc que ce tableau ne soit pas complet. Nous supprimerons cette clause lorsque cette information sera considérée comme exhaustive.

Le tableau suivant répertorie les termes fréquemment utilisés dans Adobe Workfront :

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
   <td>[!UICONTROL Niveau d’accès]</td> 
   <td>Profil utilisateur qui détermine comment un utilisateur peut interagir avec différents objets et outils dans Workfront.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tâche active]</td> 
   <td>Tâche incomplète dans un projet en cours qui n’est pas empêchée d’être travaillée par une tâche précédente et qui n’a pas de contrainte de tâche avec une date de début planifiée ultérieure. En d'autres termes, cela peut être fait aujourd'hui.</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Activity]</td> 
   <td>Dans [!DNL Workfront Goals], une activité est un indicateur de progression pour un objectif. Il peut s’agir d’une barre de progression que vous mettez à jour manuellement ou d’un projet associé à l’objectif. Vous ne pouvez pas afficher d’activités dans un rapport et vous ne pouvez pas y accéder via l’API [!DNL Workfront]. Pour plus d’informations sur les activités, voir <a href="../../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md" class="MCXref xref">Prise en main des résultats et des activités dans les objectifs Adobe Workfront</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Coût réel]</td> 
   <td> <p>Pour les tâches et les problèmes, il s’agit du coût associé aux heures réelles consignées par rapport au taux de coût par heure de la ressource affectée à la tâche ou au problème. Pour les projets, il s’agit du total des [!UICONTROL Coûts réels] provenant des tâches et des problèmes du projet. Pour plus d’informations, voir <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Tracker les coûts</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Coût des dépenses réelles]</td> 
   <td> <p>Somme des [!UICONTROL Montants réels] pour toutes les dépenses enregistrées pour un projet ou une tâche.</p> <b>EXEMPLE</b>
   <p>Si vous créez une dépense pour la tâche 1 et que vous saisissez 600,00 $ dans le champ [!UICONTROL Montant réel] , le [!UICONTROL Coût réel des dépenses] de cette tâche est de 600,00 $. </p> 
   <p>Pour un projet, [!DNL Workfront] utilise la formule suivante pour calculer le [!UICONTROL Coût réel des dépenses] :</p> <p><code>Project Actual Expense Cost = SUM (All Project Actual Expense Costs) + SUM (All Tasks Actual Expense Costs) + Project Fixed Cost</code> <br> </p> 
   <!--
     <p>Important: If the value in the Actual Amount field for an expense is negative, Workfront will ignore that expense record. For example, if the value in the Planned Amount field is $200.00 but the value in the Actual Amount field is -$300.00, the system will ignore this entire expense record which means you would not include the $200.00 planned value or the -$300.00 actual value in any calculations for Planned Expense Cost or Actual Expense Cost. (drafting this because not sure if this is still correct)</p>
    --> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Heures réelles]</td> 
   <td> <p>Dans un rapport de projet, de tâche ou d’émission, les [!UICONTROL Heures réelles] sont la somme de toutes les heures consignées sur le projet, la tâche ou le problème.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemple : </b></span></span> Si, dans l’onglet [!UICONTROL Mises à jour] de la tâche 1, vous cliquez sur "Temps journal" et saisissez 25 heures, les Heures réelles de la tâche 1 = 25 heures. </p> <p>[!DNL Workfront] calcule les [!UICONTROL Heures réelles] pour les tâches ou les projets parents à l’aide des formules suivantes :</p> 
    <ul> 
     <li> <p><code>For parent tasks = children [!UICONTROL Actual Hours] + [!UICONTROL Actual Hours] on the parent task. </code> </p> </li> 
     <li> <p><code>For projects = [!UICONTROL Actual Hours] logged on the project + [!UICONTROL Actual Hours] logged on standalone or children tasks in the project</code> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Coût réel du travail]</td> 
   <td> <p>Le [!UICONTROL Coût réel] associé à la main-d’oeuvre investie dans une tâche ou un projet. </p> <p>Pour une tâche, [!DNL Workfront] calcule le [!UICONTROL Coût réel de la main-d’oeuvre] à l’aide de la formule suivante :</p> <p><code>Task [!UICONTROL Actual Labor Cost] = Number of [!UICONTROL Actual Hours] on the task * User or Job Role [!UICONTROL Hourly Cost Rate]</code> </p> <p>Si la tâche possède un [!UICONTROL Cost Type] de [!UICONTROL User Hourly], [!DNL Workfront] utilise le taux d’utilisation. Si la tâche possède un [!UICONTROL Cost Type] de [!UICONTROL Role Hourly], [!DNL Workfront] utilise le taux de rôle de tâche pour calculer le coût réel de la main-d’oeuvre. </p> <p>Pour un projet, [!DNL Workfront] utilise la formule suivante pour calculer le [!UICONTROL Coût réel du travail] :</p> <p><code>Project [!UICONTROL Actual Labor Cost] = SUM(All Tasks [!UICONTROL Actual Labor Cost]) </code> </p> <p>Pour plus d’informations, voir <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Tracker les coûts</a>.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemple : </b></span></span>Par exemple, si un utilisateur consigne 5 heures pour une tâche avec un [!UICONTROL User Hourly] [!UICONTROL Cost Type] et que son taux horaire est de 100 $, le [!UICONTROL Real Labor Cost] est de 500 $.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Recettes réelles] </td> 
   <td> <p>Le [!UICONTROL Recettes réelles] d’un projet ou d’une tâche correspond au montant d’argent associé aux [!UICONTROL Heures réelles] du projet ou de la tâche. </p> <p>Pour plus d’informations sur le suivi des recettes dans [!DNL Workfront], voir <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Présentation de la facturation et des recettes</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Démarrage réel]</td> 
   <td>Horodatage lorsqu’un utilisateur modifie un objet en cours sur le travail qui lui est affecté.</td> 
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
   <td>Type de méthodologie basée sur l’évolution collaborative des besoins et des solutions avec des équipes interfonctionnelles. Il encourage la flexibilité et le changement selon un calendrier fixe.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Équipe agile]</td> 
   <td>Diffère d’une équipe traditionnelle, car ils prennent leurs travaux potentiels depuis un log et y travaillent dans un laps de temps défini appelé une [!UICONTROL Itération].</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Toutes Mes Équipes]</td> 
   <td> <p>Lorsqu’il est référencé dans les [!UICONTROL filtres], ce champ affiche soit les utilisateurs appartenant à l’une des équipes auxquelles appartient l’utilisateur connecté, soit les tâches affectées à l’une des équipes auxquelles appartient l’utilisateur connecté. </p> <p>Il est recommandé d'utiliser ce champ dans un filtre afin de rendre les rapports plus génériques lors de leur partage avec d'autres utilisateurs. Ainsi, vous ne pouvez créer qu’un seul rapport qui affichera des informations différentes en fonction de la personne qui se connecte pour les afficher, car les informations sont toujours personnalisées pour l’utilisateur connecté. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Date d’allocation]</td> 
   <td> <p>Vous trouverez ce champ dans les types de rapports suivants :</p> 
    <ul> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates</li>
     --> 
     <li>[!UICONTROL Project] (Données financières)</li> 
     <li>[!UICONTROL Heure budgétée]</li> 
    </ul> <p>Pour un rapport<!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        Resource Estimates or 
      </MadCap:conditionalText>
     -->[!UICONTROL Project (Financial Data)] : </p> 
    <ul> 
     <li>Créez ce rapport lorsque vous essayez de comprendre <!--
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
         how resources are budgeted for work, or 
       </MadCap:conditionalText>
      --> la quantité d’[!UICONTROL Heures planifiées] affectée à vos ressources.</li> 
     <li> <p>La [!UICONTROL Date d’attribution] est le premier jour (dimanche) d’une semaine au cours duquel l’attribution d’un [!UICONTROL Rôle de tâche] à une tâche commence. Une ressource ([!UICONTROL Job Role]) peut comporter autant de [!UICONTROL Attribution Dates] que de semaines au cours de la [!UICONTROL Duration] des tâches auxquelles elle est affectée. Si les tâches s’étendent sur plusieurs mois, le premier jour d’un mois peut également devenir une [!UICONTROL Date d’attribution], si elle tombe dans la [!UICONTROL Durée] de la tâche.</p> <p>Par exemple, un [!UICONTROL Rôle de tâche] peut être affecté à une tâche qui s’étend sur 3 semaines et qui comprend 90 [!UICONTROL Heures planifiées]. Ces heures sont réparties uniformément pendant la durée de la tâche, ce qui fait que chaque jour assigne 6 [!UICONTROL Heures planifiées] à votre rôle de tâche :</p> <p><em> [!UICONTROL Heures planifiées quotidiennes] = [!UICONTROL Total des heures planifiées]/ Nombre de [!UICONTROL Jours de travail] pendant la [!UICONTROL Durée] de la tâche </em> </p> <p>Par conséquent, il existe trois [!UICONTROL Dates d’affectation], une pour chaque dimanche de chaque semaine pendant la [!UICONTROL Durée] de la tâche, chacune associée à un certain nombre d’[!UICONTROL Heures planifiées].<br>Si la tâche commence au milieu de la dernière semaine d’un mois et se termine deux semaines après le début d’un nouveau mois, la tâche aura quatre [!UICONTROL Dates d’affectation] : une pour chaque dimanche de chaque semaine pendant la [!UICONTROL Durée] de la tâche et une pour le premier jour du nouveau mois.</p> <p>Pour tirer le meilleur parti de ces informations, nous vous recommandons de créer un rapport <!--
        <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          Resource Estimates or a 
        </MadCap:conditionalText>
       --> Projet (données financières) et d’ajouter une matrice de regroupement pour la [!UICONTROL Date d’attribution], puis de regrouper les résultats par semaine, mois, trimestre ou année pour obtenir les données les plus précises.<br> Pour plus d'informations sur la création d'un groupement de matrice, consultez l'article <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md" class="MCXref xref">Créer un rapport de matrice</a>.</p> </li> 
    </ul> <p>Les informations financières sont renseignées dans les rapports [!UICONTROL Project (Financial Data)] uniquement lorsque les données qui y sont associées ont moins de 5 ans. Par exemple, si un rôle de tâche a été attribué à une tâche en janvier 2015 et qu’aujourd’hui est septembre 2021, un champ financier comme la [!UICONTROL Date d’attribution] du rôle de tâche n’est pas renseigné dans le rapport [!UICONTROL Projet (données financières)]. </p> 
    <div> 
     <p>Pour un rapport [!UICONTROL Hour budgétée] :</p> 
     <ul> 
      <li>Générez ce rapport lorsque vous essayez de comprendre le nombre d’[!UICONTROL Heures budgétées] qui est alloué à vos ressources ou à vos projets dans le planificateur de ressources.</li> 
      <li> <p>La [!UICONTROL Date d’allocation] est le premier jour (un dimanche) de la semaine pour lequel vous avez budgété les heures dans le [!UICONTROL Resource Planner]. </p> <p><b>CONSEIL</b></p> <p>Si une semaine s’étend sur deux mois, elle génère deux lignes dans le rapport : l’une correspondant au premier jour de la semaine (le dimanche de la première semaine qui dure le premier mois), et la deuxième ligne affiche le premier jour du deuxième mois. </p> <p>Si, par exemple, vous allouez 8 heures à un utilisateur pour la semaine du 30 juin (dimanche) au 6 juillet (samedi), les deux lignes indiquent une [!UICONTROL Date d’attribution] du 30 juin et du 1er juillet. </p> </p> <p>Pour plus d’informations sur la budgétisation des ressources dans [!DNL Resource Planner], consultez l’article <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Ressources budgétaires dans l’ [!DNL Resource Planner] à l’aide des vues [!UICONTROL Project] et [!UICONTROL Role]</a>.</p> <p>Pour plus d’informations sur la création d’un rapport [!UICONTROL Hour budgétée], voir <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref">Rapport : Heure budgétée</a>. </p> </li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Annonces]</td> 
   <td> <p>Un moyen de communiquer avec les utilisateurs les informations du système. Ces informations proviennent souvent de [!DNL Workfront] vers l’administrateur ou de l’administrateur vers l’utilisateur. </p> <p>Pour plus d’informations, voir <a href="../../../administration-and-setup/get-started-wf-administration/view-send-announcements.md" class="MCXref xref">Envoi d’annonces</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Intégration de l’application]</td> 
   <td>Une application représente le plus souvent un connecteur vers une application logicielle, mais peut également représenter des fonctions spéciales qui manipulent les données.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Décision d’approbateur]</td> 
   <td> <p>Dans le rapport [!UICONTROL Approbation de BAT], ce champ affiche les décisions d’approbation de BAT pour les BAT qui ne sont plus actifs.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Étape approbateur]</td> 
   <td>Dans le [!UICONTROL Rapport d’approbation de BAT], ce champ affiche des informations sur l’étape actuelle des BAT.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Approval]</td> 
   <td> <p>Un élément de travail donné, tel qu’une tâche, un document ou une feuille de temps, peut exiger qu’un superviseur ou une superviseuse, ou un autre utilisateur ou une autre utilisatrice, valide l’élément de travail. Ce processus de désinscription est appelé approbation. </p> <p>Pour plus d’informations, voir <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">Présentation du processus d’approbation</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Date d’approbation]</td> 
   <td>Dans le rapport [!UICONTROL Approbation de BAT], ce champ affiche la date de validation d’un BAT.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Approbateur]</td> 
   <td>Un utilisateur ou un rôle de tâche qui doit approuver une tâche donnée, ou l’utilisateur qui approuve les entrées d’heure sur les feuilles de temps.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Affecté À]</td> 
   <td> <p>Dans un rapport [!UICONTROL Tâche ou problème], ce champ affiche le Propriétaire de la tâche ou du problème, ou le [!UICONTROL Principal cessionnaire]. Vous pouvez également filtrer ou regrouper en fonction de ce champ.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assignation]</td> 
   <td>Un utilisateur, un rôle de tâche ou une équipe affecté à un problème ou à une tâche. Les projets, portefeuilles ou programmes ne peuvent pas avoir d’affectations.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assignments]</td> 
   <td> <p>Dans un rapport [!UICONTROL Tâche] ou [!UICONTROL Problème] , ce champ affiche la liste de toutes les entités (utilisateurs, rôles de tâche, équipes) affectées à la tâche ou au problème. Vous pouvez filtrer selon ce champ à l’aide des champs [!UICONTROL Assignation des utilisateurs] et [!UICONTROL Rôles d’affectation]. Vous pouvez filtrer selon l’équipe affectée à la tâche ou au problème à l’aide du champ Equipe . Vous ne pouvez pas regrouper un rapport en fonction de ce champ.</p> <p>Les éléments de travail qui ont été placés dans la corbeille [!UICONTROL] continueront à s’afficher dans certains rapports qui font référence à l’objet [!UICONTROL Assignation] dans lequel un modificateur de filtre [!DNL OR] est utilisé.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Rôles d’affectation]</td> 
   <td>
   <p>Dans un rapport [!UICONTROL Tâche] ou [!UICONTROL Problème] , ce champ affiche des informations sur les rôles de tâche affectés aux tâches ou problèmes. Ce champ affiche les [!UICONTROL propriétaires de Principal], ainsi que d’autres rôles de tâche affectés à des tâches ou à des problèmes.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assignment Status]</td> 
   <td> <p>Dans un rapport d’affectation, de tâche ou de problème, le rapport [!UICONTROL État d’affectation] indique si les utilisateurs affectés à un élément de travail ont cliqué sur le bouton [!UICONTROL Travailler dessus] ou [!UICONTROL Terminé] pour accepter ou terminer le travail. Les [!UICONTROL Affectation États] suivants existent :</p> 
    <ul> 
     <li><b>[!UICONTROL Demandé]</b> : l’utilisateur a été affecté à la tâche ou au problème, mais il n’a pas cliqué sur le bouton [!UICONTROL Travailler dessus] pour commencer à travailler dessus.</li> 
     <li><b>[!UICONTROL En cours]</b> : l’utilisateur a cliqué sur le bouton [!UICONTROL Travailler dessus] et travaille actuellement sur l’élément. </li> 
     <li><b>[!UICONTROL Terminé]</b> : l’utilisateur a cliqué sur le bouton [!UICONTROL Terminé] et a terminé son travail sur l’élément. </li> 
    </ul> <p>Pour plus d’informations, voir <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/work-on-it-and-done-buttons-accept-complete-work.md" class="MCXref xref">[!UICONTROL Travailler dessus] et [!UICONTROL Terminé] présentation du bouton </a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Équipes d’affectation]</td> 
   <td>
   <p>Dans un rapport [!UICONTROL Tâche] ou [!UICONTROL Problème] , ce champ affiche des informations sur les équipes affectées aux tâches ou problèmes. Le champ affiche les [!UICONTROL propriétaires de Principal], ainsi que d’autres équipes affectées à des tâches ou des problèmes. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assignation d’utilisateurs]</td> 
   <td>
   <p>Dans un rapport [!UICONTROL Tâche] ou [!UICONTROL Problème] , ce champ affiche des informations sur les utilisateurs affectés aux tâches ou problèmes. Ce champ affiche les [!UICONTROL propriétaires de Principal], ainsi que d’autres utilisateurs affectés à des tâches ou des problèmes. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Attribute]</td> 
   <td>Un attribut est une caractéristique d’un objet [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Zone d’audit]</td> 
   <td> <p>Les audits sont des messages système qui enregistrent une action survenue dans Workfront. Les types d’audit suivants sont enregistrés :</p> 
    <ul> 
     <li>[!UICONTROL Modification de la portée]</li> 
     <li>[!UICONTROL Action de pièce jointe]</li> 
     <li>[!UICONTROL General Edit]</li> 
     <li>[!UICONTROL Changement d’état]</li> 
     <li>[!UICONTROL Remarque]</li> 
     <li>[!UICONTROL Entrée combinée]</li> 
     <li>[!UICONTROL Entrée d’erreur]</li> 
     <li>[!UICONTROL Changement d’état]</li> 
     <li>[!UICONTROL Changement d’abonnement]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Journal d’audit]</td> 
   <td>Collection de notes générée automatiquement par les événements qui font l’objet d’un suivi par le biais des modifications enregistrées ([!UICONTROL Zones d’audit]). Chaque note enregistre qui a fait l'action, ce qu'il a fait, et quand il l'a fait.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Automatique Et En Changement]</td> 
   <td> <p>Un des types [!UICONTROL Project Update]. Cela recalculera les calendriers Prévu et Prévu du projet lors de l’exécution du processus de recalcul de nuit et lors de toute mise à jour du projet ou des tâches dans le projet. </p> <p>Pour plus d’informations, voir <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Sélectionner le type de mise à jour de projet </a>.</p> </td> 
  </tr>

<tr> 
   <td><p>Disponibilité</p></td> 
   <td> <p>Ce terme est utilisé par rapport à la "disponibilité de l’utilisateur" ou à la "disponibilité de la ressource" et illustre le temps pendant lequel la ressource (utilisateur ou rôle de tâche) est disponible pour fonctionner. </p> 
   <p>Workfront calcule la disponibilité des utilisateurs à l’aide de plusieurs champs et selon les paramètres des préférences de gestion des ressources de votre système. Pour plus d’informations, voir <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configurer les préférences de gestion des ressources</a>. </p>
   <p>Pour plus d’informations sur la disponibilité des ressources, voir <a href="../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md">Prise en main de la gestion des ressources</a></p>
   Alternativement, "capacité" est également utilisé pour faire référence à la disponibilité des ressources. 
   </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Automatique Uniquement]</td> 
   <td> <p>Un des types [!UICONTROL Project Update]. Cela permet de recalculer les calendriers Prévu et Prévu lors de l’exécution du processus de recalcul de nuit.</p> <p>Pour plus d’informations, voir <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Sélectionner le type de mise à jour du projet</a>.</p> </td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL BAU]</td> 
   <td>Travail "Business as usual" qui contribue à l’exécution des objectifs principaux quotidiens de l’entreprise.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Backlog]</td> 
   <td>La zone dans un environnement agile où de nouveaux problèmes sont conservés jusqu’à ce qu’ils soient prêts à être résolus.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Baseline]</td> 
   <td>Source de données pour mesurer les itérations dans un environnement agile.</td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL Frais facturables]</td> 
   <td> <p>Une dépense marquée comme facturable au client. Il peut s’agir soit d’une dépense planifiée, soit d’une dépense réelle.</p> <p>Les champs Coût facturable planifié et Coût facturable réel peuvent être ajoutés aux vues et aux rapports. Elles n’apparaissent pas sur les pages de détails du projet ou de la tâche.</p>
   <p>Vous trouverez ces champs dans les types de rapports suivants :</p>
   <ul>
   <li>Niveau de référence</li>
   <li>Modèle</li>
   <li>Projet (données financières)</li>
   </ul>
   <p>Pour plus d’informations sur le marquage d’une dépense comme facturable, voir <a href="/help/quicksilver/manage-work/projects/project-finances/manage-project-expenses.md">Gérer les dépenses de projet</a>.</p>
   </td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL Enregistrement de facturation]</td> 
   <td> <p>Consigne les recettes, les heures ou les dépenses qui peuvent être facturées. Ces informations peuvent être utilisées pour créer des factures dans un système comptable externe.</p> <p>Pour plus d’informations, consultez <a href="../../../manage-work/projects/project-finances/create-billing-records.md">Créer des enregistrements de facturation</a>. </p> 
   </td> 
  </tr>

<tr> 
   <td>État de l’enregistrement de facturation</td> 
   <td> <p>Dans un rapport d’enregistrement de facturation ou d’heure, l’état d’un enregistrement de facturation indique si l’enregistrement de facturation a été facturé ou non. Vous ne pouvez pas supprimer un projet ni modifier l’heure associée à un enregistrement de facturation. Pour plus d’informations, consultez <a href="../../../manage-work/projects/project-finances/create-billing-records.md" >Créer des enregistrements de facturation</a>.</p>  
   </td> 
  </tr>


<tr> 
   <td>[!UICONTROL Marques]</td> 
   <td><p>Processus de personnalisation de [!DNL Workfront] pour donner à l’interface une apparence qui reflète votre entreprise en utilisant vos couleurs et logos.</p><p><strong>REMARQUE</strong><br>Si votre organisation a été intégrée à [!DNL Adobe Experience Cloud], la valorisation de marque n’est pas disponible.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Chemins de navigation]</td> 
   <td> <p>Zone située en haut de la page qui indique l’emplacement hiérarchique de l’utilisateur dans l’application.</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Pour plus d’informations, voir <a href="../../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md" class="MCXref xref">Présentation du chemin de navigation</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL État du budget]</td> 
   <td> <p>Il s’agit d’un champ obsolète. Toutes les informations que ce champ peut afficher sont liées à une fonctionnalité que [!DNL Workfront] a supprimée et le champ ne peut pas être mis à jour. </p> <p>Ce champ indique si le projet a été ajouté au [!UICONTROL Capacity Planner] et si le calcul du budget est terminé. Le [!UICONTROL Capacity Planner] a été supprimé de [!DNL Workfront]. </p> 
    <ul> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">If the project is&nbsp;not added to the capacity planner, its value is <i>Not Included</i>.&nbsp;</li>
     --> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">If the project is&nbsp;added to the Capacity Planner but is excluded from the budget calculation,&nbsp;the value is <i>Included but not Calculated</i>.&nbsp;</li>
     --> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> If the project is&nbsp;added to the Capacity Planner and included in the budget calculation, the value is <i>Included and Calculated</i>. </li>
     --> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Date d’achèvement du budget]</td> 
   <td> <p>Il s’agit d’un champ obsolète. Toutes les informations que ce champ peut afficher sont liées à une fonctionnalité que [!DNL Workfront] a supprimée. Ce champ ne peut pas être mis à jour. </p>
   <p> Ce champ est toujours visible dans les listes et les rapports [!UICONTROL Projet].</p>  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Coût budgété]</td>

<td> <p>Il s’agit du coût associé aux ressources de budget pour un projet. </p>
   <p>Le champ s’affiche dans les zones suivantes de [!DNL Workfront] sous les noms suivants :</p>
   <ul>
   <li><strong>[!UICONTROL Coût budgété]</strong> : dans le panneau [!UICONTROL Résumé des dossiers]</li>
   <li><strong>[!UICONTROL Cost]</strong> : dans les zones [!UICONTROL Utilization] lors de l’affichage des informations par [!UICONTROL Cost]</li>
   <li><strong>[!UICONTROL Coût budgétaire du projet]</strong> : dans les listes et les rapports</li>
   </ul>   
    <p>Le coût [!UICONTROL budgété] du projet est calculé à l’aide de la formule suivante :</p> 
    <p><code>[!UICONTROL Project Budgeted Cost] (or [!UICONTROL Budgeted Cost]) = [!UICONTROL Budgeted Expense Cost] + [!UICONTROL Budgeted Labor Cost] + [!UICONTROL Fixed Cost] of the project</code> </p> 
    <p>Pour plus d’informations sur le calcul de l’[!UICONTROL Coût budgété] et pour comprendre les différents noms de ce concept dans [!DNL Workfront], voir <a href="../../../manage-work/projects/project-finances/budgeted-cost.md" class="MCXref xref">Calcul du coût budgété du projet</a>. </p>
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Hours budgétés]</td> 
   <td> <p>Heures budgétées pour les ressources nécessaires au travail sur les projets. Ce champ fait référence aux heures budgétées dans la zone [!UICONTROL Resource Budgeting] de l’[!UICONTROL Business Case] (ou dans le [!UICONTROL Resource Planner]) pour le projet ou pour les ressources du projet.</p> <p>Pour plus d’informations, voir <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Comprendre [!UICONTROL Budget Labor Cost] et [!UICONTROL Budget Hours] pour les projets</a>. </p> 
    <!-- 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Hours that were formerly budgeted in the Legacy Resource Estimates area of a project (or in the Capacity Planner)</p>
    <p>Important: This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p>
  -->
    <p> Pour plus d’informations sur la budgétisation des utilisateurs dans [!DNL Resource Planner], consultez l’article <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Ressources de budget dans [!DNL Resource Planner] à l’aide des vues [!UICONTROL Project] et [!UICONTROL Role]</a>. </p> 
    <p>Les heures budgétées dans la zone [!UICONTROL Resource Budget] de l’[!UICONTROL Business Case] ou du [!UICONTROL Resource Planner] s’affichent dans les zones suivantes de [!DNL Workfront] et sous les noms suivants :</p> 
     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td><strong>Nom d’affichage [!UICONTROL Hours budgétaires]</strong></td> 
        <td><strong>Zones [!DNL Workfront]</strong></td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Hours]</td> 
        <td>Zone [!UICONTROL Resource Budget] de l’[!UICONTROL Business Case]</td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL BDG]</td> 
        <td>[!UICONTROL Resource Planner] visualisé par [!UICONTROL Hours]</td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Hours budgétés]</td> 
        <td> <p>Vue Rapport d’utilisation [!UICONTROL Hours]</p> <p>Pour plus d’informations sur le rapport [!UICONTROL Utilisation], consultez l’article <a href="../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md" class="MCXref xref">Présentation du rapport [!UICONTROL Utilisation des ressources]</a>.</p> </td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Bud. Hours]</td> 
        <td> <p>Rapport [!UICONTROL Heure budgétée]</p><p>L’objet [!UICONTROL Hour budgétée] du rapport Heure budgétée fait référence à des informations relatives à un outil de gestion des ressources obsolète. Seul le "[!UICONTROL Bud". Le champ "Hours" de ce rapport fait référence aux heures budgétées dans le [!UICONTROL Resource Planner] ou la zone [!UICONTROL Resource Budget] de l’[!UICONTROL Business Case] du projet. </p> <p>Pour plus d’informations sur la création d’un rapport, consultez l’article <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Créer un rapport personnalisé</a>.</p> </td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Resource Planner Budget Hours] </td> 
        <td> <p>Les rapports suivants sont disponibles :</p>
        <ul>
        <li>Rapport [!UICONTROL Project]
        <li>Rapport [!UICONTROL Projet (données financières)]
        <li>Rapport [!UICONTROL Tâche]
        <li>Rapport [!UICONTROL Problème]
        <li>Rapport [!UICONTROL Heure budgétée]</li>
        </ul>
         <p>Pour plus d’informations sur la création d’un rapport, consultez l’article <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Créer un rapport personnalisé</a>.</p> </td> 
       </tr> 
      </tbody> 
     </table> 
    <p>Toute autre mention des [!UICONTROL Hours budgétés] dans [!DNL Adobe Workfront] fait référence aux heures budgétisées à l’aide de fonctionnalités obsolètes qui ont été supprimées de Workfront . Il s’agit de champs en lecture seule qui ne sont pas mis à jour avec les informations actuelles lorsque vous utilisez les outils de budget des ressources actuelles. </p>
    <!--<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate the Budgeted Hours from theResource Planner in the areas and reports listed below. </p>
     <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Planner Hours view (in the BDG column)</li>
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Utilization report Hours view</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Budgeting area of the Business Case (in the Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report (the Bud. Hours field refers to hours budgeted for users; the Pln. Bud. Hours field refers to hours budgeted for roles or projects)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report (in the Project: Budgeted Hours field) </li>
        </ul>
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The fields listed below display in the reports listed and are hours formerly budgeted in the&nbsp;Capacity Planner or the Legacy Resource Estimates area of the Business Case.</p>
         <p>Important: The Capacity Planner and Legacy&nbsp;Resource Estimates have been removed from Workfront. You cannot update any information that might display in these fields.</p>
        <ul>
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Capacity Planner</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Legacy&nbsp;Resource Estimates area of the Business Case (in the Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report (in the Bud. Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report (in the Budgeted Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project report (in the Budgeted Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project (Financial&nbsp;Data) report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Task&nbsp;report (in the Project: Budgeted Hours field)</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Issue report (in the Project: Budgeted Hours field)</li>
      </ul> --> 
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Coût de la main-d’oeuvre budgété]</td> 
   <td> <p>Il s’agit du coût associé aux heures que vous, en tant que responsable des ressources, consacrez à vos rôles de travail pour le travail qu’ils doivent effectuer sur les projets. </p> <p>Le [!UICONTROL Coût de la main-d’oeuvre budgété] d’un rapport de projet est calculé à l’aide de la formule suivante :</p> <p><code style="font-style: normal;">[!UICONTROL Budgeted Labor Cost] = SUM([!UICONTROL Job Role Cost] per [!UICONTROL Hour] * [!UICONTROL Budgeted Hours] per [!UICONTROL Job Role])</code> </p> <p>Ce champ peut faire référence aux éléments suivants :</p> 
    <ul> 
     <li> <p>Les coûts de main-d’oeuvre affichés dans la zone [!UICONTROL Resource Budgeting] de l’[!UICONTROL Business Case] ou dans le [!UICONTROL Resource Planner] qui sont associés au coût des rôles de travail sur un projet. Pour plus d’informations sur le calcul du [!UICONTROL Coût de la main-d’oeuvre budgété], consultez l’article <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">[!UICONTROL Comprendre le coût de la main-d’oeuvre budgété] et [!UICONTROL Hours budgétées] pour les projets</a></p> </li> 
     <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>Les coûts de main-d’oeuvre affichés dans la zone [!UICONTROL Resource Budget] de l’[!UICONTROL Business Case] qui reflètent les [!UICONTROL People Coûts] estimés dans une initiative liée au projet à partir de l’[!DNL Scenario Planner] lorsque vous utilisez le planificateur de scénario pour budgéter les ressources de votre projet. Pour plus d’informations sur les initiatives, consultez la <a href="../../../scenario-planner/initiatives-overview.md" class="MCXref xref">présentation des initiatives dans le planificateur de scénario</a>. </p> <p>[!DNL Scenario Planner] nécessite une licence supplémentaire. Pour plus d'informations sur [!DNL Workfront Scenario Planner], consultez la <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">présentation [!DNL Scenario Planner]</a>. </p> </li> 
     <p>Il s’affiche dans les zones suivantes de sous les noms suivants :</p>
   <ul>
   <li><strong>[!UICONTROL Coût de la main-d’oeuvre budgété]</strong> : dans la zone [!UICONTROL Budget des ressources] de l’[!UICONTROL Analyse de cas].
   <li><strong>[!UICONTROL Coût budgété]</strong> : dans la vue du rapport [!UICONTROL Utilisation]
   <p>Pour plus d’informations, voir <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">Affichage des informations sur l’utilisation des ressources </a>.</p>
   <li><strong>[!UICONTROL BDG]</strong> : dans les vues [!DNL Resource Planner] Projet ou [!DNL Role], lors de l’affichage par coût
   <li><strong>[!DNL Resource Planner Budgeted Labor Cost]</strong>: dans les rapports suivants : 
   <ul>
    <li>Rapport [!UICONTROL Project]</li>
    <li>Rapport [!UICONTROL Projet (données financières)]</li>
    <li>Rapport [!UICONTROL Tâche]</li>
    <li>Rapport [!UICONTROL Problème]</li>
    <li>Rapport [!UICONTROL Heure budgétée]</li> 
    </ul>
    <p>Pour plus d’informations sur la création d’un rapport, consultez l’article <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Créer un rapport personnalisé</a>.</p>
    <!--
          <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Labor costs for hours budgeted in the Legacy Resource Estimates area of a project (or in the Capacity Planner). This was available only in Adobe Workfront Classic. </p>
           <p>Important: This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p>
       </li> 
    </ul> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate the Budgeted Labor Cost field based on the hours budgeted in the Resource Planner in the following areas and reports in&nbsp;Workfront: </p>
        <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Planner Cost view (in the BDG column)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Utilization report Cost view (in the Budgeted Cost column)</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Budgeting area of the Business Case </li>
         </ul> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate the Budgeted Labor Cost associated with resources budgeted in the Resource Planner in the Resource Planner Resource Budgeted Cost field in the following reports: </p>
       <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report </li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Task&nbsp;report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Issue report</li>
         </ul> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate a Budgeted Labor Cost field that contains information from a tool that has been deprecated in the reports listed below. You can no longer update the fields displayed in these reports and budgeting your resources on the projects does not update them: </p>
        <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report </li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Task&nbsp;report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Issue report</li>
         </ul>      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about calculating the Budgeted Labor Cost, see the article <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Understand Budgeted Labor Cost and Budgeted Hours for projects</a>&nbsp;.&nbsp;</p>
    --> 
    </td> 
   </tr> 
   <tr> 
   <td>[!UICONTROL Date de début budgétée]</td> 
  <td> <p>Il s’agit d’un champ obsolète. Toutes les informations que ce champ peut afficher sont liées à une fonctionnalité que [!DNL Workfront] a supprimée. Ce champ ne peut pas être mis à jour.</p>
  <p>Ces zones ont été supprimées de [!DNL Workfront]. </p> 
  <p>Le champ est toujours visible dans les listes et les rapports [!UICONTROL Projet].</p>
   <!--
   <p>This field shows the date when the budgeting of resources starts, as defined in the Legacy Resource Estimates area of the Business Case of a project, or the Capacity Planner.</p>
   -->   
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Graphique de Burndown]</td> 
   <td>Un graphique en courbes qui fournit une représentation visuelle des tâches terminées et restantes.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Analyse de cas [!UICONTROL]</td> 
   <td> <p>Outil utilisé pour évaluer si un projet doit être transféré de l’état [!UICONTROL Idée] à l’état [!UICONTROL Planification]. En d’autres termes, un [!UICONTROL] permet à l’organisation de décider s’il est utile de lancer et de terminer le projet ou non, en particulier lors de la comparaison de projets avec d’autres membres d’un portfolio.</p> <p>Pour plus d’informations, voir <a href="../../../manage-work/projects/define-a-business-case/create-business-case.md" class="MCXref xref">Création d’un [!UICONTROL Business Case] pour un projet </a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Business Case Budget Hours]</td> 
   <td> <p>Il s’agit d’un champ obsolète. Toutes les informations que ce champ peut afficher sont liées à une fonctionnalité que [!DNL Workfront] a supprimée. Ce champ ne peut pas être mis à jour.</p> <p>Ce champ est toujours visible dans les listes et les rapports des projets et des [!UICONTROL Tâche]. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Attribution calculée]</td> 
   <td> <p>L’un des types de durée de la tâche [!UICONTROL] . Cela permet de calculer le pourcentage d’une journée de travail de 8 heures attribué à la tâche par l’utilisateur, en fonction de la [!UICONTROL Durée] de la tâche et du [!UICONTROL Travail requis].</p> <p>Pour plus d’informations, voir <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Présentation de la tâche [!UICONTROL Duration] et [!UICONTROL Duration Type]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Travail calculé]</td> 
   <td> <p>L’un des types de durée de la tâche [!UICONTROL]. Cela permet de calculer le [!UICONTROL Travail requis] sur une tâche, en fonction de la [!UICONTROL Durée] et des pourcentages de l’utilisateur [!UICONTROL Assignation] (qui sont basés sur un jour de travail de 8 heures).</p> <p>Pour plus d’informations, voir <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Présentation de la tâche [!UICONTROL Duration] et [!UICONTROL Duration Type]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendrier]</td> 
   <td> <p>Il existe deux types de calendriers dans [!DNL Workfront] : les rapports [!UICONTROL Home Calendar] et Calendrier.</p> <p>Le [!UICONTROL Home Calendar] est un calendrier personnel qui permet à un utilisateur de gérer sa charge de travail par rapport à ses heures disponibles dans [!DNL Workfront]. Les utilisateurs peuvent également intégrer leur [!UICONTROL Home Calendar] à [!DNL Outlook] ([!DNL Google] et [!DNL Microsoft] à venir). </p> <p>Pour plus d’informations sur le [!UICONTROL Home Calendar], voir <a href="../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md" class="MCXref xref">[!UICONTROL Home Calendar] view</a>.</p> <p>Un rapport Calendrier est un rapport dynamique dans lequel les utilisateurs peuvent afficher la date et d’autres détails importants d’un événement, y compris la date d’échéance, l’état du travail et l’utilisateur auquel l’événement est affecté.</p> <p> Pour plus d’informations sur les rapports de calendrier, consultez la <a href="../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md" class="MCXref xref">présentation des rapports de calendrier</a>.</p> </td> 
  </tr> 
   <tr> 
   <td>[!UICONTROL Peut Démarrer]</td> 
   <td> <p>Ce champ indique si une tâche est prête à démarrer. Si le début est prêt à être travaillé sur le champ [!UICONTROL Can Start] de la tâche, est défini sur [!UICONTROL True]. </p> <p>Pour plus d’informations, consultez la présentation de <a href="../../../manage-work/tasks/task-information/can-start-task-overview.md" class="MCXref xref">"[!UICONTROL Can Start]" pour les tâches </a>.</p> 
   <!--
     <p>(NOTE: everything below is drafted because I created a new article linked above with all this information - it was getting kind of too big for just a table cell)</p>
    --> <!--
     <p>Workfront checks for the following things before it marks a task as True for the Can Start field:<br></p>
    --> 
    <!--
     <ul> 
      <li> If the task has a parent, it checks to see if the value of Can Start for the parent it set to True. If the value for the parent is False, then all the subtasks have the value of Can Start set to False, as well.&nbsp;</li> 
      <li> It also checks to see if the predecessors of the task as well as the predecessors of their parents are complete. If they are complete, the Can Start value for the task is set to True. If any of the task predecessors or their parents' predecessors are not complete, or have a status of Complete-Pending Approval, then the Can Start value for the task is set to False.&nbsp;</li> 
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
   <td> <p>Le temps disponible d’une ressource lorsqu’elle peut être affectée au travail. Voir Disponibilité. </p></td> 
  </tr>

<tr> 
   <td> <p>[!UICONTROL Catégorie]</p> </td> 
   <td> <p>Une catégorie est un formulaire personnalisé. Vous pouvez créer des rapports pour cet objet et les afficher dans d’autres rapports d’objet. Tous les objets ne peuvent pas comporter de formulaire personnalisé ou de catégorie. Les objets suivants peuvent avoir un formulaire personnalisé : <br></p> 
    <ul> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Task]</li> 
     <li>[!UICONTROL Problème]</li> 
     <li>[!UICONTROL Portfolio]</li> 
     <li>[!UICONTROL Document]</li> 
     <li>[!UICONTROL Dépenses]</li> 
     <li>[!UICONTROL Program]</li> 
     <li>[!UICONTROL User]</li> 
     <li>[!UICONTROL Company]</li> 
     <li>[!UICONTROL Itération]</li></ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nom de catégorie]</td> 
   <td> <p>Lorsqu’elle est ajoutée en tant que colonne à la vue de l’un des objets suivants, elle affiche la liste de tous les formulaires personnalisés associés à ces objets :</p> 
    <ul> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Task]<br></li> 
     <li>[!UICONTROL Problème]<br></li> 
     <li>[!UICONTROL Portfolio]<br></li> 
     <li>[!UICONTROL Document]<br></li> 
     <li>[!UICONTROL Dépenses]<br></li> 
     <li>[!UICONTROL Program]<br></li> 
     <li>[!UICONTROL User]<br></li> 
     <li>[!UICONTROL Company]</li> 
     <li>[!UICONTROL Itération]</li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Gestion des modifications]</td> 
   <td>Un domaine de pratique axé sur la définition, la compréhension et l'adaptation des travaux planifiés aux changements de portée, de planification, de coûts et de ressources.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Modifier l’ordre]</td> 
   <td>Type de problème soulevé contre un projet qui décrit une modification requise de la portée convenue.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Modification Uniquement]</td> 
   <td>L’un des projets [!UICONTROL Update Types]. Il ne met à jour que les calendriers [!UICONTROL Projet projeté] et [!UICONTROL Planifié] lorsque des mises à jour sont apportées à des tâches ou que des modifications sont effectuées sur le projet ou les tâches.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Modifier l’ordre]</td> 
   <td> <p>L’un des types [!UICONTROL Problème], indiquant généralement qu’une quantité de travail non planifiée doit être effectuée avant que le projet puisse être terminé.</p> <p>Pour plus d’informations sur les types de problèmes [!UICONTROL Problèmes], voir la section "Types de problèmes par défaut" dans l’article <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md" class="MCXref xref">Personnaliser les types de problèmes par défaut</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Child Task]</td> 
   <td>Tâche qui est une [sous-tâche!UICONTROL] d’une [!UICONTROL Tâche parent] ([!UICONTROL Tâche de résumé]).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Children]</td> 
   <td>Collection de [!UICONTROL Sous-tâches] à une [!UICONTROL Tâche parent] ([!UICONTROL Tâche de résumé]).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Entraînement] et [!UICONTROL Formation]</td> 
   <td>Modules d’apprentissage, certifications, normes ou communauté de pratique.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Commit]</td> 
   <td>Outil de communication permettant aux utilisateurs de définir des attentes concernant les livrables de tâches.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Date de validation]</td> 
   <td>Outil de communication permettant à l’utilisateur de définir des attentes concernant les livrables de tâche.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Communication] et [!UICONTROL Reporting]</td> 
   <td>Normes pour examiner les exceptions et l’intégrité d’un projet, d’un programme ou d’un portfolio</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Company]</td> 
   <td> <p>Une [!UICONTROL Company] est une entité organisationnelle dans [!DNL Workfront]. </p> 
   <p> Vous pouvez associer un utilisateur ou un projet à une seule société. Pour plus d’informations, voir <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md">Création et modification d’entreprises</a>.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Date d’achèvement]</td> 
   <td> <p>Date à laquelle un projet, une tâche ou une publication doit être terminé. Il existe plusieurs types de [!UICONTROL Dates d’achèvement] dans [!DNL Workfront] :</p> 
    <ul> 
     <li>[!UICONTROL Date d’achèvement réelle]. Pour plus d’informations, voir <a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref">Présentation du projet [!UICONTROL Date d’achèvement réelle] </a>.</li> 
     <li>[!UICONTROL Date d’achèvement prévue]. Pour plus d’informations, voir <a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">Définition de la [!UICONTROL Date d’achèvement planifiée]</a> et <a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Présentation de la tâche [!UICONTROL Date d’achèvement planifiée]</a>.</li> 
     <li>[!UICONTROL Date d’achèvement prévue]. Pour plus d’informations, voir <a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">Présentation de la [!UICONTROL Date d’achèvement prévue] pour les projets, les tâches et les problèmes</a>.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Jour d’achèvement]</td> 
   <td>Le jour, par rapport au début du [!UICONTROL Modèle], où une [!UICONTROL Tâche de modèle] ou un [!UICONTROL Modèle] est censé être terminé.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Mode d’achèvement]</td> 
   <td> <p>Cela indique comment un projet sera marqué comme [!UICONTROL terminé]. Elle peut avoir deux valeurs :</p> 
    <ul> 
     <li>[!UICONTROL Manuel] : un utilisateur doit définir l’état du projet sur [!UICONTROL Terminé].</li> 
     <li>[!UICONTROL Automatique] : l’état du projet passe automatiquement à [!UICONTROL Terminé] lorsque toutes les tâches du projet sont entièrement terminées et que tous les problèmes sont résolus.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Condition]</td> 
   <td> <p>Il s’agit d’une représentation visuelle de la progression d’une tâche, d’un problème ou d’un projet.</p> <p>Pour les projets, la condition peut être définie manuellement par le propriétaire du projet ou automatiquement par [!DNL Workfront], en fonction de l’état d’avancement du projet. </p> <p>Les valeurs possibles pour la condition du projet sont les suivantes :</p> 
    <ul> 
     <li>[!UICONTROL Sur Target]</li> 
     <li>[!UICONTROL À Risque]</li> 
     <li>[!UICONTROL En Problème]</li> 
    </ul> <p>Pour plus d’informations sur les conditions du projet, consultez l’article <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">Présentation de [!UICONTROL Project Condition] et [!UICONTROL Condition Type]</a>.</p>
     <p>Vous pouvez associer des conditions de tâche et d’émission à un nombre qui peut s’afficher dans les rapports. Les listes ci-dessous affichent les noms et les nombres par défaut des conditions de tâche et de problème. Votre administrateur système peut mettre à jour les noms des conditions et ajouter de nouvelles conditions avec des nombres différents. Une fois qu’un nombre est associé à une condition, il ne peut pas être modifié.  </p> 
     <p>Pour les tâches, la condition est définie manuellement par le propriétaire de la tâche. Les valeurs possibles pour la condition de tâche sont les suivantes :</p> 
    <ul> 
     <li>[!UICONTROL Passage En douceur] (0)<br></li> 
     <li> [!UICONTROL Certaines Préoccupations] (1)<br></li> 
     <li>[!UICONTROL Blocs principaux] (2)</li> 
    </ul> <p>Pour plus d’informations sur les conditions de tâche, consultez l’article <a href="../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md" class="MCXref xref">Mise à jour de la [!UICONTROL Condition] pour les tâches et les problèmes</a>.</p> <p>Pour les problèmes, la condition est définie manuellement par le propriétaire du problème. Les valeurs possibles pour la condition de problème sont les suivantes :<br></p> 
    <ul> 
     <li>[!UICONTROL Passage En douceur] (0)<br></li> 
     <li>[!UICONTROL Certaines Préoccupations] (1)<br></li> 
     <li>[!UICONTROL Blocs principaux] (2)</li> 
    </ul> 
   <p><b>NOTE</b></p>
    <p>Lorsque le champ [!UICONTROL Condition] est suivi dans les rapports [!UICONTROL Entrée du journal], les valeurs [!UICONTROL Nouveau] et [!UICONTROL Anciennes valeurs numériques] affichent le numéro associé à la condition au lieu de son nom. Si une condition n’est pas définie à l’origine pour une tâche ou un problème et que vous la mettez à jour par la suite, l’entrée de journal qui capture la mise à jour affichera la [!UICONTROL Ancienne valeur numérique] du champ [!UICONTROL Condition] comme étant de -2 147 483 648. Voir aussi "[!UICONTROL Nouvelle valeur numérique]", "[!UICONTROL Ancienne valeur numérique]" et "[!UICONTROL Entrée du journal]" dans cet article. </p> 
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Mise À Jour De La Condition]</td> 
   <td> <p>Ce champ présente l’état actuel des tâches, des projets ou des problèmes. Cette option affiche les mises à jour les plus récentes fournies par les propriétaires des tâches, projets ou problèmes dans le champ [!UICONTROL Etat de mise à jour], ainsi que la nouvelle condition.</p> <p>Les commentaires effectués sur les mises à jour de condition ne s’affichent pas dans la colonne [!UICONTROL Mise à jour de condition] ; seule la mise à jour principale s’affiche.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Date de contrainte]</td> 
   <td> <p>Si vous utilisez une [!UICONTROL Contrainte de tâche] liée à une date spécifique, telle que [!UICONTROL Doit démarrer le], cette date spécifique devient la [!UICONTROL Date de contrainte] de la tâche.</p> <p>Les contraintes de tâche suivantes mettent à jour le champ [!UICONTROL Constraint Date] :</p> 
    <ul> 
     <li>[!UICONTROL Doit Commencer Le]</li> 
     <li>[!UICONTROL Doit Se Terminer Le]</li> 
     <li>[!UICONTROL Ne Démarre Pas Plus Tard Que]</li> 
     <li>[!UICONTROL Ne Commence Pas Avant]</li> 
    </ul> <p><b>CONSEIL</b></p>   
     <ul> 
      <li> <p>Une tâche avec une [!UICONTROL Contrainte] de [!UICONTROL Dates fixes] n’a pas de [!UICONTROL Date de contrainte]. </p> </li> 
      <li> <p> [!UICONTROL Date de contrainte] ne peut être affichée que dans un rapport ou une vue personnalisée.</p> </li> 
     </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Construit le jour]</td> 
   <td> <p>Si vous utilisez une contrainte de tâche dans une tâche de modèle liée à un jour spécifique, comme Doit démarrer le, ce jour spécifique devient le jour de contrainte de la tâche de modèle.</p> <p>Les contraintes de tâche suivantes mettent à jour le champ [!UICONTROL Constraint Day] :</p> 
    <ul> 
     <li>[!UICONTROL Doit Commencer Le]</li> 
     <li>[!UICONTROL Doit Se Terminer Le]</li> 
     <li>[!UICONTROL Ne Démarre Pas Plus Tard Que]</li> 
     <li>[!UICONTROL Ne Commence Pas Avant]</li> 
    </ul> <p><b>CONSEIL</b></p> <p>  [!UICONTROL Constraint Day] ne peut être affiché que dans un rapport ou une vue personnalisée. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Constraint Type]</td> 
   <td> <p>La tendance de planification d’une tâche. Par exemple, [!UICONTROL Dès que possible] planifiera le début d’une tâche dès que possible, et [!UICONTROL Terminer au plus tard] planifiera une tâche pour qu’elle se termine au plus tard à la [!UICONTROL Date de contrainte] et au plus tard.</p> <p>Pour plus d’informations, voir <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">[!UICONTROL Task Constraint] overview</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Menu contextuel]</td> 
   <td>Un menu, situé sur le côté gauche de l’écran, dans lequel les éléments changent pour établir une corrélation avec le contenu actif. Par exemple, lorsqu’un utilisateur consulte un projet, le [!UICONTROL Menu contextuel] affiche des liens vers des informations et des outils liés au projet.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converti de l’Émetteur de problème]</td> 
   <td>Champ d’un rapport de projet ou de tâche qui affiche des informations sur l’utilisateur qui est le [!UICONTROL Contact de Principal] d’un problème lorsque le problème est converti en projet ou en tâche. Le champ s’affiche également dans la section [!UICONTROL Détails du projet] où il indique le nom du [!UICONTROL Contact Principal] du problème converti. Voir aussi "[!UICONTROL Contact Principal]" dans cet article.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Coût [!UICONTROL]</td> 
   <td> <p>Montant monétaire que vous devez dépenser lors de la réalisation d’un projet, d’une tâche ou d’une émission. </p> <p>Vous pouvez suivre différents types de coûts pour la main-d'oeuvre, les dépenses, les risques liés au projet. Pour plus d'informations sur le suivi des coûts dans [!DNL Workfront], voir <a href="../../../manage-work/projects/project-finances/track-costs.md">Tracker les coûts</a>.</p> 
   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cost Type]</td> 
   <td>Pour une tâche, le [!UICONTROL Cost Type] détermine la manière dont la tâche va augmenter les coûts. Voici quelques exemples : [!UICONTROL Horaire fixe], [!UICONTROL Heure de l’utilisateur] et [!UICONTROL Heure de l’utilisateur plus Fixe]. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dépendances inter-projets]</td> 
   <td> <p>Une tâche d’un projet dépend d’une tâche d’un autre projet.</p> <p>Pour plus d’informations, voir <a href="../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md" class="MCXref xref">Création de prédécesseurs multi-projets</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Données personnalisées]</td> 
   <td> <p>Données propres à une organisation. Les organisations peuvent personnaliser l’application [!DNL Workfront] en créant des formulaires personnalisés et des champs personnalisés. Ces informations personnalisées peuvent générer des rapports pour les indicateurs de performance clés, le contrôle et la combinaison de demandes. </p> <p>[!UICONTROL Données personnalisées] peut être lié à :</p> 
    <ul> 
     <li>[!UICONTROL Projects]</li> 
     <li>[!UICONTROL Tasks]</li> 
     <li>[!UICONTROL Users]</li> 
     <li>[!UICONTROL Entreprises]</li> 
     <li>[!UICONTROL Issues]</li> 
     <li>[!UICONTROL Documents]</li> 
     <li>[!UICONTROL Dépenses]</li> 
     <li>[!UICONTROL Portfolio]</li> 
     <li>[!UICONTROL Programmes]</li> 
     <li>[!UICONTROL Itérations]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custom Data Type]</td> 
   <td>L’option permettant de spécifier si un champ [!UICONTROL Données personnalisées] est stocké dans la base de données sous la forme Texte, Date, Nombre ou Devise.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custom Display Type]</td> 
   <td>Le type d’affichage d’un champ personnalisé. Par exemple, [!UICONTROL Liste déroulante], [!UICONTROL Champ de texte], [!UICONTROL Zone de texte], [!UICONTROL Boutons radio [!UICONTROL], etc.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Champ personnalisé]</td> 
   <td>Pour les données personnalisées qui permettent à l’utilisateur de sélectionner parmi plusieurs options, il s’agit des valeurs à partir desquelles l’utilisateur peut sélectionner. Les options personnalisées ne sont valides que sur les [!UICONTROL Liste déroulante], [!UICONTROL Liste déroulante à sélection multiple], [!UICONTROL Boutons radio] et [!UICONTROL Cases à cocher].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Étiquette de formulaire personnalisée]</td> 
   <td>Lorsque vous utilisez un type d’affichage personnalisé avec des options personnalisées, il s’agit du texte de l’interface utilisateur qui s’affiche dans le menu déroulant, les cases à cocher ou les boutons radio de cette option personnalisée.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Valeur personnalisée]</td> 
   <td>Lors de l’utilisation d’un champ personnalisé avec des options personnalisées, il s’agit de la valeur qui sera stockée dans la base de données pour une option particulière.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Vue personnalisée]</td> 
   <td>Une définition des champs de données ou des colonnes qui s’affichent pour chaque objet d’une liste.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Client]</td> 
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
   <td>[!UICONTROL Tableaux de bord]</td> 
   <td> <p> Vous pouvez ajouter ce champ dans un rapport ou dans une vue de l’objet de rapport afin d’afficher les tableaux de bord sur lesquels le rapport est répertorié dans une liste. </p> <p> Vous pouvez également utiliser ce champ pour filtrer les rapports répertoriés sur un tableau de bord spécifique. </p> <p> Pour plus d’informations sur l’inclusion d’informations de tableau de bord dans les rapports d’objets de rapport, voir la section "Comprendre les rapports répertoriés sur les tableaux de bord" dans l’article <a href="../../../reports-and-dashboards/reports/report-usage/access-organize-reports.md" class="MCXref xref">Accès aux rapports et organisation des rapports</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data Type]</td> 
   <td>Voir "[!UICONTROL Custom Data Type]".</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Jours en retard]</td> 
   <td> <p>Ce champ présente une différence de date entre [!UICONTROL Début planifié] et [!UICONTROL Aujourd’hui] si la [!UICONTROL Date d’achèvement réelle] est manquante.</p> <p>Affiche également une différence de date entre [!UICONTROL Achèvement réel] et [!UICONTROL Achèvement planifié], en présence d’une [!UICONTROL Date d’achèvement réelle].</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Planification par défaut]</td> 
   <td> <p>Heures de travail par défaut personnalisables à attribuer aux utilisateurs et aux projets au sein d’une organisation. </p> <p>Les plannings sont utilisés pour calculer les dates prévues, de début et d’achèvement des tâches qui sont affectées aux utilisateurs.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Deliverable]</td> 
   <td>Les biens ou services quantifiables qui doivent être fournis à la fin d’un projet.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Gestion de la demande]</td> 
   <td>Notation et hiérarchisation des processus d’ingestion.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Objectifs du service]</td> 
   <td>Objectifs propres à un département spécifique qui se concentre sur l’amélioration des mesures opérationnelles au sein du département.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dependency]</td> 
   <td>Le lien entre deux tâches qui nécessitent qu’une tâche change d’état avant l’autre tâche peut également changer d’état.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dependency Type]</td> 
   <td> <p>Type de relation de planification entre une tâche et ses prédécesseurs. Par exemple, [!UICONTROL Finish-Start], qui nécessite que la première tâche soit Terminée avant que la seconde tâche ne puisse démarrer.</p> <p>Pour plus d’informations, voir <a href="../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md" class="MCXref xref">Présentation des types de dépendances de tâches</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Document]</td> 
   <td>Tout fichier joint à un objet dans [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Document Version]</td> 
   <td> <p>Chaque fois que le même document est téléchargé vers le même objet, un numéro de version lui est attribué. Les utilisateurs peuvent afficher et modifier plusieurs options pour une version précédente d’un document.</p> <p>Pour plus d’informations, voir <a href="../../../documents/managing-documents/manage-document-versions.md" class="MCXref xref">Gestion des versions de document</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Duration]</td> 
   <td> <p>La fenêtre de temps allouée à la fin d’une tâche ou d’un projet (déterminée par le nombre de jours entre le [!UICONTROL Début planifié] et la Fin planifiée).</p> 
    <ul> 
     <li>Pour les tâches, la Durée est un champ modifiable si le Type de durée de la tâche n’est pas Simple. Si le Type de durée de la tâche est simple ou si la Contrainte de tâche est définie sur Dates fixes, la Durée est un calcul effectué par Workfront.</li> 
     <li>Pour les problèmes, la durée est toujours un champ modifiable et doit représenter une estimation du nombre de jours pendant lesquels le problème doit être résolu.</li> 
     <li>Pour les projets, la Durée est un calcul effectué par [!DNL Workfront] et représente la différence en jours entre le Début planifié de la première tâche et la [!UICONTROL Fin planifiée] de la dernière tâche du projet.</li> 
    </ul> <p>Pour plus d’informations sur la différence entre la [!UICONTROL Durée] et la [!UICONTROL Durée planifiée] pour les tâches, consultez l’article <a href="../../../manage-work/tasks/task-information/planned-duration-vs-duration-for-tasks.md">Différence entre la [!UICONTROL Durée planifiée] et la [!UICONTROL Durée] pour les tâches </a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Durée en minutes]</td> 
   <td>Ce champ affiche les mêmes informations que le champ [!UICONTROL Durée] en minutes plutôt qu’en jours. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc,QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Durée par occurrence]</td> 
   <td> <p>Cela s’affiche dans les zones [!UICONTROL Détails de la tâche] et [!UICONTROL Modifier la tâche] d’un parent de tâches récurrentes. Il affiche la durée de chaque tâche récurrente. Pour plus d’informations sur la création de tâches récurrentes, voir <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Créer des tâches récurrentes</a>. </p> <p> <span>Les durées modifiées dans des tâches récurrentes individuelles n'affichent pas la valeur indiquée dans ce champ.</span> </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Duration Type]</td> 
   <td> <p>Un champ de tâche qui indique comment le travail requis pour terminer la tâche est affecté aux personnes désignées tout au long de la durée de la tâche. Il représente la relation entre la [!UICONTROL Durée] de la tâche, le [!UICONTROL Travail requis] et le temps, ou [!UICONTROL Affectation], que les ressources affectées doivent consacrer à la tâche pour la terminer. </p> <p>Ce champ apparaît dans l’onglet [!UICONTROL Détails] d’une tâche. </p> <p>Les options pour le type de durée d’une tâche sont les suivantes :</p> 
    <ul> 
     <li>[!UICONTROL Affectation calculée]</li> 
     <li>[!UICONTROL Travail calculé]</li> 
     <li>[!UICONTROL Effort piloté]</li> 
     <li>[!UICONTROL Simple]</li> 
    </ul> <p>Pour plus d’informations, voir <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Présentation de la tâche [!UICONTROL Duration] et [!UICONTROL Duration Type]</a>.</p> 
    --&gt; </td> 
   </tr> 
   <tr> 
   <td>[!UICONTROL Unité de durée]</td> 
   <td>Unité utilisée pour mesurer le temps dans une recherche d’énergie.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Effort piloté]</td> 
   <td>Relation entre le nombre d’utilisateurs et le temps nécessaire à l’exécution de la tâche. À mesure que vous ajoutez d’autres utilisateurs, la durée totale planifiée pour terminer la tâche diminue, mais la durée de la tâche reste la même. Par exemple, si une tâche consiste à bombarder un tonneau de cacahuètes, l’ajout de personnes supplémentaires diminuera le temps planifié, mais la durée en jours-personnes restera la même.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Temps écoulé]</td> 
   <td> <p>[!UICONTROL Délai écoulé] est une unité de temps pour la [!UICONTROL Durée] d’une tâche. Il s’agit de l’heure entre la [!UICONTROL Date de début planifiée] et la [!UICONTROL Date d’achèvement planifiée] d’une tâche qui comprend les jours fériés, les week-ends et les congés. En d’autres termes, le temps écoulé est le passage des jours calendaires. </p> <p>[!DNL Workfront] prend en charge les unités de temps écoulées suivantes pour la durée de la tâche :</p> 
    <ul> 
     <li> <p>[!UICONTROL Minutes Écoulées]</p> </li> 
     <li> <p>[!UICONTROL Heures écoulées]</p> </li> 
     <li> <p>[!UICONTROL Jours écoulés]</p> </li> 
     <li> <p>[!UICONTROL Semaines écoulées]</p> </li> 
     <li> <p>[!UICONTROL Mois écoulés]</p> </li> 
    </ul> <p>Pour plus d’informations sur la durée de la tâche, y compris le temps écoulé, voir <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Présentation de la [!UICONTROL Durée de la tâche] et [!UICONTROL Type de durée]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Date de fin]</td> 
   <td> <p> Dans un rapport [!UICONTROL Rate], il s’agit de la date à laquelle se termine un nouveau taux de facturation pour un rôle de tâche au niveau du projet. Les heures associées au projet qui se trouvent avant cette date sont multipliées par ce taux de facturation pour calculer les recettes sur le projet. </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Engagement]</td> 
   <td>L’[!UICONTROL Indicateur de performance professionnelle] (WPI) qui indique quand l’engagement et la confiance envers la tâche, le projet, l’équipe ou l’organisation sont en déclin. Cela indique que vous devez agir pour raviver cette croyance et cet engagement. WPI serait mesuré en posant les questions simples : "Avez-vous compris ce que vous attendiez de vous ? Le travail qui vous a été confié a-t-il fait une différence dans l'organisation ? Avez-vous fait du bon travail ?"</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Enterprise Goals]</td> 
   <td>Objectifs interfonctionnels qui contribuent aux mesures des objectifs de l’entreprise.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Event]</td> 
   <td>Toute modification dans un projet ou une tâche.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Event Handler]</td> 
   <td>Tâches automatisées survenant lorsque des événements se produisent. Un exemple courant est une notification électronique automatisée.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Notification d’événement]</td> 
   <td>Courrier électronique généré à partir d’un gestionnaire d’événements.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Dépenses]</td> 
   <td>Coût des tâches ou des projets non liés à la main d’oeuvre.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL External]</td> 
   <td> <p>En règle générale, il s’agit d’un type de licence, ou d’un utilisateur disposant d’une telle licence. Un utilisateur disposant d’un tel type de licence peut uniquement consulter les informations du système. Ils ne peuvent pas participer activement au travail.</p> <p>Pour plus d’informations, voir <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] - Présentation des licences</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Système externe]</td> 
   <td>Tout service ou logiciel stocké et géré en dehors du système d’enregistrement désigné.</td> 
  </tr>

<tr> 
   <td>[!UICONTROL Field]</td> 
   <td><p>Tout objet Workfront ou les informations qui lui sont associées, telles qu’elles apparaissent dans la base de données. </p>
   <p>Par exemple, "projet", "utilisateur", "heure" sont à la fois des objets Workfront et des champs. "Nom", "statut", "propriétaire", "date de début" sont des champs Workfront associés aux objets ci-dessus. </p>

<p>En ce qui concerne les objets, les termes "objets" et "champs" peuvent être interchangeables.</p>
   <p>Dans le cadre de la création de rapports, les "champs" se rapportent aux objets ou aux informations sur l’objet que vous souhaitez capturer dans le rapport.</p>

<p><b>NOTE</b></p>

<p>Dans les rapports de type texte, les champs font référence aux objets ou à leurs informations tels qu’ils apparaissent dans la base de données.</p>
   <p>Il arrive que le nom affiché dans l’interface utilisateur soit différent du nom du champ de la base de données. Par exemple, "issue" est le nom de l’objet dans l’interface de Workfront, mais "opTask" est le nom de l’objet (ou du champ) dans la base de données Workfront. </p> 
   <p> Il est important d'utiliser le champ tel qu'il apparaît dans la base de données lors de l'écriture d'un rapport en mode texte, de l'affichage, du filtrage, du regroupement ou lors de la création d'un champ calculé.</p>

<p>Pour plus d’informations, voir <a href="../../../wf-api/general/api-explorer.md">API Explorer</a> et <a href="../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md">Présentation du mode texte</a>.</p>

<p>Par défaut, Workfront est fourni avec un ensemble de champs qui définissent les objets et leurs informations. Vous pouvez également créer des champs personnalisés pour définir des objets, mais vous ne pouvez pas créer d’objets personnalisés.</p> 
   </td> 
  </tr>

<tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Filter]</td> 
   <td> <p>Un des principaux blocs de création d’un rapport ou d’un élément de liste qui définit les informations affichées à l’écran. Pour plus d’informations sur les éléments de création de rapports, voir <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">Eléments de création de rapports : filtres, vues et regroupements</a>.</p> <p>Le filtre détermine les résultats qui s’affichent dans un rapport ou dans une liste de panneaux [!DNL Workfront], tels que les projets, les tâches ou les problèmes.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Financial Work Management]</td> 
   <td>Processus de gestion des données sur les coûts, les dépenses et les recettes du travail dans [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Coût fixe]</td> 
   <td>Vous pouvez définir un montant fixe de coût pour un projet. Il fait partie du [!UICONTROL Coût planifié] du projet, qui représente le montant d’argent dont vous avez besoin pour terminer le projet. Pour plus d’informations sur les coûts, voir <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Tracker les coûts</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Recettes fixes]</td> 
   <td>Vous pouvez définir un montant fixe de recettes pour un projet. Il fait partie des [!UICONTROL Recettes prévues] du projet, qui représente le montant d’argent que vous pourriez obtenir si vous terminez le projet. Pour plus d’informations sur les recettes, voir <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Présentation de la facturation et des recettes</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Indicateurs]</td> 
   <td> <p> Il s’agit du même champ que les [!UICONTROL Icônes d’état], mais il n’est disponible que pour les vues suivantes : </p> 
    <ul> 
     <li> [!UICONTROL Modèles] </li> 
     <li> [!UICONTROL Dépenses] </li> 
    </ul> <p> Pour plus d’informations, voir l’article <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">Icônes d’état intégrées dans les vues</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder]</td> 
   <td>Les dossiers permettent d’organiser les documents ou les rapports associés à un objet.</td> </tr>
  <tr>
  <td>[!UICONTROL FTE] (équivalent temps plein)</td> 
   <td>Il s’agit de l’équivalent temps plein qui indique la durée pendant laquelle une ressource est disponible pour le travail. 
   Le champ [!UICONTROL FTE] s’affiche dans les zones suivantes : 
  <ul>
   <li> Profil de l’utilisateur, lors de la modification ou de la création de l’utilisateur </li>
   <li> [!UICONTROL Resource Planner] </li>
   <li> [!UICONTROL planificateur de scénarios] (nécessite une licence supplémentaire pour le planificateur de scénarios Workfront) </li>
   <li> Listes et rapports utilisateur </li> </ul>

<p>L’[!UICONTROL FTE] doit être un nombre décimal maximum de 1 et ne peut pas être égal à 0. </p>
   <p> Un [!UICONTROL FTE] de 1 (qui est la valeur par défaut du champ [!UICONTROL FTE] d’un utilisateur, tel que défini dans son profil) signifie qu’une ressource (utilisateur ou rôle) travaille toute la durée en fonction du planning qui calcule leur disponibilité. </p>
   <p>Votre administrateur Workfront décide du planning à utiliser pour déterminer la disponibilité de l’utilisateur.  </p>
   <ul>
   <li> Lorsque le [!UICONTROL Default Schedule] est utilisé, Workfront utilise l’[!UICONTROL FTE] de l’utilisateur figurant dans son profil pour calculer la disponibilité. </li>
   <li> Lors de l’utilisation de la planification de l’utilisateur, Workfront utilise le temps de congé de l’utilisateur, la valeur [!UICONTROL Work Time] et les heures de [!UICONTROL Default Schedule] pour calculer l’heure [!UICONTROL FTE] de l’utilisateur. </li> </ul>

<p>Pour plus d’informations, voir <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configurer les préférences de gestion des ressources</a>.  </p>
   <p>Pour plus d’informations sur la création de plannings dans [!DNL Workfront], consultez la section <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md">Créer un planning</a>. </p>

<p><b>NOTE</b></p>
   <p>Pour tous les calculs dans le [!UICONTROL Scenario Planner], Workfront utilise la valeur suivante : 1 [!UICONTROL FTE] = 8 heures.</p>
   <p>Pour plus d’informations, voir <a href="../../../scenario-planner/get-started-with-scenario-planning.md">Prise en main du [!UICONTROL Gestionnaire de scénarios]</a>. </p>
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
   <td>[!UICONTROL Graphique de Gantt]</td> 
   <td> <p>Chronologie visuelle des dates du projet dans une vue Calendrier basée sur les dates planifiées ou prévues au fur et à mesure que les tâches du projet sont planifiées.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Goal]</td> 
   <td><p>Il existe deux concepts d’objectifs dans [!DNL Workfront] : </p> 
    <ul> 
     <li> <p><b>Objectifs du projet</b> : ensemble d’objectifs commerciaux convenus par les parties prenantes d’un projet. Les objectifs du projet font partie de l’analyse de cas d’un projet. </p> <p>Vous ne pouvez pas afficher les objectifs du projet dans des listes ou des rapports, mais vous pouvez y accéder via l’API. </p> <p>Pour plus d’informations sur les objectifs d’un projet de Business Case, voir <a href="../../../manage-work/projects/define-a-business-case/create-business-case-goals.md">Créer des objectifs de Business Case </a>. </p> </li> 
     <li> <p><b>Objectifs stratégiques</b> : un objectif stratégique est un objectif que vous créez pour planifier votre stratégie de travail pour une période donnée. Vous pouvez créer ces types d’objectifs à l’aide de [!DNL Workfront Goals]. Votre entreprise doit acheter une licence supplémentaire et vous devez avoir accès à cette fonctionnalité pour pouvoir créer des objectifs stratégiques. [!DNL Workfront Goals] est disponible uniquement avec une licence supplémentaire.</p> 
     <p>Pour plus d’informations, voir <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] - Aperçu </a>. </p> 
     <p>Vous pouvez afficher les objectifs stratégiques dans un rapport d’objectif ou de projet et y accéder via l’API. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Hiérarchie des objectifs]</td> 
   <td> <p>Dans les rapports [!UICONTROL Objectif] et [!UICONTROL Projet] , il s’agit d’un champ de collection qui affiche les objectifs dans la hiérarchie auxquels un objectif stratégique appartient lorsqu’il s’aligne sur d’autres objectifs. Les objectifs sont séparés par un délimiteur ▸. </p> <p>Seuls les parents de l’objectif et de l’objectif s’affichent dans ce champ. Les objectifs pour les enfants ne s’affichent pas. </p> <p>Pour plus d’informations sur l’alignement des objectifs dans [!DNL Workfront Goals], consultez la <a href="../../../workfront-goals/goal-alignment/goal-alignment-overview.md">présentation de l’alignement des objectifs dans [!DNL Workfront Goals]</a>. </p> 
   <p>Ce champ n’est visible que si votre organisation a acheté [!DNL Workfront Goals]. Pour plus d'informations sur la gestion des objectifs stratégiques à l'aide de [!DNL Workfront Goals], consultez la <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] présentation </a>. </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Score de réussite de l’objectif]</td> 
   <td> Dans un rapport [!UICONTROL Projet] , ce champ est utilisé pour faire référence aux objectifs au niveau du projet associés à l’[!UICONTROL Business Case]. Actuellement, il s’agit d’un champ obsolète qui n’est associé à aucune fonctionnalité.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Goals] </td> 
   <td> <p>Dans un rapport [!UICONTROL Projet], il s’agit d’un champ de collection qui affiche tous les objectifs stratégiques associés à un projet. Les objectifs sont séparés par des virgules.</p> <p>Ce champ n’est visible que si votre organisation a acheté [!DNL Workfront Goals]. Pour plus d'informations sur la gestion des objectifs stratégiques à l'aide de [!DNL Workfront Goals], voir <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] - Aperçu</a>. Pour plus d’informations sur les objectifs stratégiques et les objectifs de projet dans [!DNL Workfront], voir "[!UICONTROL Objectif]" dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Global Interface Preferences]</td> 
   <td>Paramètres de l’interface qui affectent tous les utilisateurs. [!UICONTROL Global Interface Preferences] peut être remplacée par les [!UICONTROL User Interface Preferences].</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Group]</td> 
   <td> <p>Collection d’utilisateurs (provenant éventuellement du même service ou unité opérationnelle) ayant accès aux mêmes objets. Outre les utilisateurs, les groupes peuvent être associés à des portefeuilles, des programmes, des projets, des modèles de projet <span>, des entreprises, des équipes, des plannings, des modèles de mise en page et des profils de feuille de temps.</span></p> <p>Vous pouvez également octroyer des autorisations aux objets par groupe. Pour plus d’informations, voir <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Présentation des groupes</a>.</p> <p>Dans une liste ou un rapport d’objets de l’un des types suivants, vous pouvez utiliser le champ [!UICONTROL Groupe] pour répertorier les objets de ce type associés à un groupe particulier : utilisateur, portfolio, programme, projet, <span>modèle de projet</span>, société, équipe, planning, modèle de mise en page ou profil de feuille de temps.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Administrateur de groupe]</td> 
   <td> <p>Utilisateurs qui gèrent les objets, y accèdent et les utilisateurs de groupes d’utilisateurs désignés.</p> <p> Dans un rapport [!UICONTROL Groupe], ce champ affiche les noms des utilisateurs désignés comme [!UICONTROL Administrateurs de groupe] dans le groupe. Pour plus d’informations sur les administrateurs de groupe, voir <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administrateurs de groupe</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Groupe [!UICONTROL avec accès à l’administration]</td> 
   <td> <p> Dans un [!UICONTROL Modèle de mise en page], un [!UICONTROL Profil de feuille de calcul] ou un [!UICONTROL Rapport de planification], ce champ affiche les groupes dont les administrateurs de groupe ont accès pour modifier le modèle. Vous pouvez également filtrer ce rapport selon ce champ. </p> <p> Pour plus d’informations, voir <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Créer et gérer des modèles de mise en page</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Groupement]</td> 
   <td> <p>Élément de rapport utilisé pour classer les informations d’une liste selon un critère commun.</p> <p>Pour plus d’informations, reportez-vous à la section "[!UICONTROL Groupements]" de l’article <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref"> Éléments de reporting : filtres, vues et regroupements</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Date de remise]</td> 
   <td> <p>Date à laquelle une tâche devient disponible pour le travail. La [!UICONTROL Date de remise] est un calcul qui ne peut pas être défini manuellement. <br>Pour plus d’informations sur la [!UICONTROL Date de passation], consultez l’article <a href="../../../manage-work/tasks/task-information/handoff-task-date.md" class="MCXref xref">[!UICONTROL Date de remise des tâches] </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Help Desk]</td> 
   <td>Un autre nom pour décrire la zone [!UICONTROL Demandes] de [!DNL Workfront]. Vous pouvez utiliser la zone [!UICONTROL Demandes] pour traiter les tickets d’assistance clientèle, les demandes de projet, les tickets d’assistance, etc.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Propriétaire]</td> 
   <td>Dans un rapport [!UICONTROL Heure], le [!UICONTROL Propriétaire] est l’utilisateur auquel les heures sont attribuées. Différent de l’utilisateur qui consigne réellement l’heure. Ces deux entités peuvent parfois être deux utilisateurs différents. <br>Pour plus d’informations sur l’heure de connexion d’un autre utilisateur, reportez-vous à l’article <a href="../../../timesheets/create-and-manage-timesheets/log-time.md" class="MCXref xref">Temps du journal</a>.</td> 
  </tr>

<tr> 
   <td>Statut d'heure</td> 
   <td> <p>Attribut défini par Workfront pour les heures réelles que les utilisateurs consignent pour les tâches, les problèmes ou les projets. </p>

Les entrées d’heure peuvent avoir l’un des états suivants dans Workfront :
<ul>
   <li><b>Envoyé</b> : les heures ont été enregistrées sur un projet, une tâche ou un problème. Ils font partie d’un enregistrement de facturation ou ne sont pas encore ajoutés à un enregistrement de facturation.</li>
   <li><b>Approuvé</b> : les heures ont été enregistrées et elles ont été approuvées par le propriétaire du projet. Ils font partie d’un enregistrement de facturation ou ne sont pas encore ajoutés à un enregistrement de facturation.</li> 
   <li><b>Non approuvé</b> : les heures ont été enregistrées et rejetées par le propriétaire du projet. Ils font partie d’un enregistrement de facturation ou ne sont pas encore ajoutés à un enregistrement de facturation.</li>
   <li><b>Facturé</b> : les heures ont été enregistrées, ajoutées à un enregistrement de facturation et l’état de l’enregistrement de facturation a été marqué comme Facturé. Ils n’avaient pas besoin d’être approuvés par le propriétaire du projet.</li>
   <li><b>Facturé et approuvé</b> : les heures ont été enregistrées, approuvées par le propriétaire du projet et l’état de l’enregistrement de facturation a été marqué comme Facturé.</li>
   </ul>


<p>Lorsque les heures font partie d’un enregistrement de facturation, l’état de l’heure indique si les heures ont été approuvées ou si l’enregistrement de facturation auquel elles appartiennent a été facturé. L’état de l’heure d’une entrée d’heure n’est visible que dans une liste d’heures ou un rapport. </p>

<p>Pour plus d’informations sur l’ajout d’heures aux enregistrements de facturation, reportez-vous à la section "Ajout d’heures aux enregistrements de facturation" dans l’article <a href="../../../manage-work/projects/project-finances/create-billing-records.md" >Créer des enregistrements de facturation</a>.</p>

<p>Pour plus d'informations sur l'approbation du temps passé sur les projets, voir <a href="../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md" >Exiger du temps pour l'approbation d'un projet</a>.</p>

<p><b>CONSEIL</b></p>

<p>Les heures générales qui ne sont pas connectées directement aux tâches n’affichent pas le statut de l’heure. </p> </td> 
  </tr>



<tr> 
   <td>[!UICONTROL Hour Type]</td> 
   <td> <p>Attribut pouvant être défini pour Heures réelles que les utilisateurs enregistrent pour les tâches, problèmes ou projets. Il s’agit également d’un attribut pour les heures consignées qui ne sont pas directement liées au travail, telles que [!UICONTROL Vacance] et [!UICONTROL Heure de désactivation].</p> <p>Pour plus d’informations, voir <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md" class="MCXref xref">Gestion des types d’heures</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td> <p>L’ID est un indicateur alphanumérique associé à chaque objet de [!DNL Workfront]. Elle identifie de manière unique chaque objet de la base de données [!DNL Workfront]. Vous pouvez afficher l’identifiant de n’importe quel objet d’un rapport ou d’une liste pour chaque objet. </p> <p><b>CONSEIL</b></p>   <p>Vous pouvez également afficher l’identifiant dans l’URL de la page de l’objet. Par exemple, l’ID d’un projet peut ressembler au nombre indiqué dans l’URL suivante, lorsque vous accédez à la page [!UICONTROL Détails du projet] :</p> <p><code>https://&lt;your domain>.my.workfront.com/project/<b>5e29c8010027d8eb334762d4fff3ffca</b>/overview</code> </p> </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Individual Goals]</td> 
   <td>Objectifs individuels qui contribuent aux mesures des objectifs de l’équipe, mais sans rapport avec le développement personnel ou professionnel.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Accès hérité]</td> 
   <td>Fonction de partage permettant d’accéder à la propagation d’un objet à un autre. Par exemple, l’accès de l’utilisateur du projet hérite défini dans les enregistrements de programme et de portefeuille.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Initiative]</td> 
   <td> <p>Dans le [!DNL Workfront Scenario Planner], vous pouvez diviser un plan en plusieurs initiatives pour faciliter la gestion du plan. <span>Vous pouvez créer un rapport [!UICONTROL Initiative] et accéder aux informations [!UICONTROL Initiative] dans un rapport [!UICONTROL Projet].</span></p> <p>[!DNL Scenario Planner] nécessite une licence supplémentaire. Pour plus d'informations sur [!DNL Workfront Scenario Planner], consultez la <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">présentation [!DNL Scenario Planner]</a>. </p> <p>Le rapport [!DNL Initiative] n’est pas visible dans votre instance [!DNL Workfront], sauf si votre entreprise a acheté une licence [!DNL Workfront Scenario Planner]. Vous ne pouvez pas accéder aux [!UICONTROL Initiatives] par le biais de l’API.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Rôle de tâche de l’initiative]</span> </td> 
   <td> <p><span>Le type de rapport [!UICONTROL Initiative Job Role] affiche des informations sur les rôles de tâche associés à une initiative de plan dans [!DNL Workfront Scenario Planner].</span> </p> <p>[!DNL Scenario Planner] nécessite une licence supplémentaire. Pour plus d'informations sur [!DNL Workfront Scenario Planner], consultez la <a href="../../../scenario-planner/scenario-planner-overview.md">présentation [!DNL Scenario Planner]</a>. </p> <p><span>Ce type de rapport n’est pas visible dans votre instance [!DNL Workfront], sauf si votre société a acheté une licence [!DNL Workfront Scenario Planner].</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Initiative Heures de rôle de tâche]</span> </td> 
   <td> <p><span> Dans un rapport [!UICONTROL Rôle de tâche de l’initiative], il affiche le nombre d’heures associées à un rôle de tâche dans une initiative.</span> </p> <p>[!DNL Scenario Planner] nécessite une licence supplémentaire. Pour plus d'informations sur [!DNL Workfront Scenario Planner], consultez la <a href="../../../scenario-planner/scenario-planner-overview.md">présentation [!DNL Scenario Planner]</a>. </p> <p>Ce champ et le type de rapport [!UICONTROL Initiative Job Role] ne sont pas visibles dans votre instance [!DNL Workfront], sauf si votre entreprise a acheté une licence [!DNL Workfront Scenario Planner].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Décompte du rôle de l’initiative]</td> 
   <td> <p>Dans un rapport [!UICONTROL Rôle dans la tâche de l’initiative], il indique le nombre de rôles de tâche spécifiques associés à une initiative.</p> <p>[!DNL Scenario Planner] nécessite une licence supplémentaire. Pour plus d'informations sur [!DNL Workfront Scenario Planner], consultez la <a href="../../../scenario-planner/scenario-planner-overview.md">présentation [!DNL Scenario Planner]</a>. </p> <p>Ce champ et le type de rapport [!UICONTROL Initiative Job Role] ne sont pas visibles dans votre instance [!DNL Workfront], sauf si votre entreprise a acheté une licence [!DNL Workfront Scenario Planner].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Initiative Date de dernière publication]</td> 
   <td> <p>Champ dans un rapport [!UICONTROL Initiative], [!UICONTROL Rôle de tâche de l’initiative] et [!UICONTROL Projet] qui affiche la date de la dernière publication d’une initiative de plan dans un projet. Vous pouvez publier des initiatives pour créer des projets ou mettre à jour des projets liés aux initiatives.</p> <p>[!DNL Scenario Planner] nécessite une licence supplémentaire. Pour plus d'informations sur [!DNL Workfront Scenario Planner], consultez la <a href="../../../scenario-planner/scenario-planner-overview.md">présentation [!DNL Scenario Planner]</a>. </p> <p><span>Pour plus d’informations sur les initiatives de publication, voir</span><a href="../../../scenario-planner/publish-scenarios-update-projects.md">Scénarios Publish pour créer et mettre à jour des projets dans [!DNL Workfront Scenario Planner]</a>. Ce champ n’est pas visible dans votre instance [!DNL Workfront], sauf si votre entreprise a acheté une licence [!DNL Workfront Scenario Planner].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Recherche en ligne]</td> 
   <td>Recherche effectuée, lors du processus de remplissage d’un formulaire, pour trouver les entrées possibles pour un champ spécifique.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Configuration de l’interface]</td> 
   <td>Zone de l’application qui permet de définir des vues personnalisées, des filtres, des groupes, des contrôles de liste, etc.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL Est L’Objectif De La Société]</p></td> 
   <td> <p>Dans [!DNL goal reports], une valeur "[!UICONTROL True]/ [!UICONTROL False] s’affiche pour chaque objectif stratégique afin d’indiquer si votre organisation est affectée à l’objectif en tant que propriétaire. </p> 
   <p>Ce champ n’est visible que si votre organisation a acheté [!DNL Workfront Goals]. Pour plus d'informations sur la gestion des objectifs stratégiques à l'aide de [!DNL Workfront Goals], consultez la <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] présentation </a>.</p>
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Problème]</td> 
   <td> <p>Élément de travail non planifié qui indique généralement qu’un problème empêche la réalisation d’une tâche ou d’un projet. Il est mis à l'essai et évalué en vue d'un examen plus approfondi de l'effort de travail.</p> <p>Un [!UICONTROL Problème] peut également être une requête [!UICONTROL Help Desk] . [!UICONTROL Modifier les commandes], les [!UICONTROL requêtes] et les [!UICONTROL bogues] sont également des [!UICONTROL problèmes].</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Gestion des problèmes]</td> 
   <td> <p>Processus et règles régissant la définition des types de problèmes et le processus de routage, de triage ou de trafic associé à chaque type.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Propriétaire du problème]</td> 
   <td>L’équipe ou les utilisateurs responsables du triage et de la résolution d’un problème.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Itération]</td> 
   <td>Période pendant laquelle une équipe produit un ensemble prédéfini de livrables.</td> 
  </tr> 
 </tbody> 
</table>

## J - L

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
   <td> <p>Utilisé pour identifier les fonctions et responsabilités quotidiennes d’un utilisateur. Les rôles de tâche peuvent être attribués à des tâches afin d’identifier la compétence requise pour terminer un processus de travail sans l’affecter à un utilisateur spécifique. </p> <p>Un utilisateur peut avoir plusieurs rôles. Par exemple, Designer graphique ou consultant.</p> <p>Pour plus d’informations, voir <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Création et gestion des rôles de tâche</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL Entrée du journal]</p> </td> 
   <td> <p>Objet à générer des rapports qui fournit des informations sur les mises à jour du système pour les champs suivis qui apparaissent dans la zone [!UICONTROL Mises à jour] des projets, tâches, problèmes et autres objets.</p> <p>Pour en savoir plus, consultez la section <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md" class="MCXref xref">Rapport sur les [!UICONTROL Mises à jour]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Indicateur Kanban]</td> 
   <td> <p>Dans un rapport [!UICONTROL Tâche] ou [!UICONTROL Problème] , le champ [!UICONTROL Indicateur Kanban] affiche l’état de l’indicateur défini sur l’article sur le [!UICONTROL Panorama Kanban]. Les valeurs possibles sont [!UICONTROL Sur la piste], [!UICONTROL Prêt pour l’extraction] et [!UICONTROL Bloqué].</p> <p>Pour plus d’informations sur la définition de l’état de l’indicateur sur les articles du [!UICONTROL Kanban story board], voir  L’article <a href="../../../agile/use-kanban-in-an-agile-team/use-flags-on-stories.md" class="MCXref xref">Utiliser des indicateurs sur les articles sur l’[!UICONTROL Panne Kanban]</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>IPC</td> 
   <td>Une valeur mesurable qui démontre l’efficacité avec laquelle une entreprise atteint ses principaux objectifs commerciaux.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Lag]</td> 
   <td>Délai qui doit s’écouler une fois que la [!UICONTROL Date d’achèvement planifiée] de la tâche précédente est passée jusqu’à ce que la tâche dépendante puisse commencer.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Types de journalisation]</td> 
   <td> <p>Méthode de calcul de la balise [!UICONTROL]. Il peut s’agir :</p> 
    <ul> 
     <li>[!UICONTROL Jours] (jours ouvrés)</li> 
     <li>[!UICONTROL Jours du calendrier] (ignorer les jours fériés)</li> 
     <li>[!UICONTROL Pourcentage]</li> 
     <li>[!UICONTROL Jour de la semaine]</li> 
    </ul> <p>Pour plus d’informations, voir <a href="../../../manage-work/tasks/use-prdcssrs/lag-types.md" class="MCXref xref">Présentation des types de balises</a>.</p> </td>
  </tr> 
  <tr> 
   <td>[!UICONTROL Grande miniature]</td> 
   <td> <p> Dans une liste ou un rapport [!UICONTROL Document], un aperçu du document s’affiche dans une miniature. </p> <p>Sélectionnez <strong>[!UICONTROL Grande miniature]</strong> pour afficher une miniature de 400 pixels de large dans le rapport.</p> <p>La taille de la miniature s’ajuste lorsque vous modifiez la largeur de la colonne dans une liste ou un rapport.</p> <p>Voir aussi "[!UICONTROL Miniature]" dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 10 dernières visionneuses]</td> 
   <td> <p>Dans une liste de rapports, ce champ affiche le nom des 10 utilisateurs au maximum qui ont consulté le rapport le plus récemment.<br>Pour plus d’informations sur l’utilisation dans les listes de rapports, reportez-vous à l’article <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Afficher l’utilisation des rapports</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Last Condition Note]</td> 
   <td> <p>Ce champ affiche la dernière mise à jour saisie sur un objet par le propriétaire de l’objet. Il s’agit de l’activité ou de l’interaction la plus récente du propriétaire sur un objet.</p> <p>La colonne [!DNL Last Condition Note] est vide si le texte de la dernière note d’un objet a été supprimé. Lorsqu’une nouvelle note est saisie sur l’objet, elle devient la dernière note et s’affiche à nouveau dans la colonne. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Date de dernière mise à jour financière]</td> 
   <td>Dans un rapport [!UICONTROL project] , ce champ capture la date et l’heure auxquelles les finances du projet ont été calculées et mises à jour pour la dernière fois. Pour plus d’informations sur les finances de projet, voir <a href="../../../manage-work/projects/project-finances/project-finances-overview-1.md" class="MCXref xref">Présentation des finances du projet</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dernière remarque]</td> 
   <td> <p>Ce champ affiche la dernière mise à jour saisie sur un objet par un utilisateur. Il s’agit de l’activité ou de l’interaction la plus récente sur un objet.</p> <p>La colonne [!UICONTROL Dernière remarque] est vide si le texte de la dernière note d’un objet a été supprimé. Lorsqu’une nouvelle note est saisie sur l’objet, elle devient la dernière note et s’affiche à nouveau dans la colonne.</p>
   <p>Lorsque ce champ est ajouté à un rapport [!UICONTROL Tâche], toutes les mises à jour qui restent sur les objets enfants, telles que les problèmes, les sous-tâches, les documents, etc. — de la tâche ne s’affiche pas dans cette colonne.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dernière consultation par]</td> 
   <td> <p>Dans une liste de rapports, ce champ affiche des informations sur l’utilisateur qui a consulté le rapport en dernier.<br>Pour plus d’informations sur l’utilisation dans les listes de rapports, reportez-vous à l’article <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Afficher l’utilisation des rapports</a>.<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Date de dernière consultation]</td> 
   <td> <p>Dans une liste de rapports, ce champ affiche la date à laquelle le rapport a été affiché en dernier.<br>Pour plus d’informations sur l’utilisation dans les listes de rapports, reportez-vous à l’article <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Afficher l’utilisation des rapports</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Modèle de mise en page]</td> 
   <td>Défini par l’administrateur système ou l’administrateur de groupe pour identifier les onglets et les rapports qui s’affichent dans l’espace de travail d’un utilisateur donné.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Type de mise en page]</td> 
   <td>En association avec [!UICONTROL Custom Views], le [!UICONTROL Layout Type] spécifie le type de [!UICONTROL Custom View]. Actuellement, seule la liste est disponible. À l’avenir, la vue [!UICONTROL Détails] (la vue [!UICONTROL Détails] d’un objet) pourra être disponible.</td> 
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
       <br>If there&nbsp;are multiple job roles, this is a summary of the budgeted hours for all job roles. The Legacy Budgeted Hours are calculated after you have used the "Set budget to schedule" feature, or after you have defined how many of the Planned Hours should be budgeted, in the Resource Estimates area of the Business Case of the project or in the Capacity Planner.&nbsp; 
     </p> </td> </tr> -->
  <!--<tr data-mc-conditions=""> 
   <td>Legacy Budgeted Labor Cost</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed. This field cannot be updated. </p> <p>The field is still visible in some reports and lists. </p> <p>See <i>Budgeted Labor Cost</i>. </p> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">In a project report, this field shows the labor cost associated with the project, taking into account the Cost per Hour rate of every job role and the amount of Legacy Budgeted Hours estimated in the Legacy Resource Estimates area of the Business Case that is needed for each role to complete the project.&nbsp;</p>
    --> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Legacy Budgeted Labor Cost in a project report is calculated using the following formula:</p>
    --> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code style="font-style: normal;">Legacy Budgeted Labor Cost = SUM(Job Role Cost per Hour * Legacy Budgeted Hours per Job Role)</code> </p>
    --> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about calculating Legacy Budgeted Labor Cost, see the article <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Understand Budgeted Labor Cost and Budgeted Hours for projects</a>&nbsp;&nbsp;</p>
    --> </td> 
  </tr> 
  <tr> 
   <!-- <td>Legacy Resource Pool</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed. This field cannot be updated. </p> 
   <p>Although not recommended, you may update the information in this report using the API.</p> 
   <p>See <i>Resource Pools</i> for updated fields. </p> 
   <p>The Legacy Resource Pool is a collection&nbsp;of job roles associated with a project or a user. The functionality of the Legacy Resource Pools is displayed in the tools available in the Legacy Resource Planning tab of the People area. This is a deprecated field.</p>
    --> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tâche de bibliothèque]</td> 
   <td>Un modèle pour une seule tâche qui permet d’attribuer un nom cohérent aux [!UICONTROL Tâches] et aux [!UICONTROL Tâches du modèle] dans l’application.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL License Type]</td> 
   <td>Type de licence attribué à un niveau d’accès [!UICONTROL]. Il s’agit de [!UICONTROL Utilisateur complet], [!UICONTROL Utilisateur limité] ou [!UICONTROL Demandeur].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL License Limite Plan]</td> 
   <td> <p>Dans un rapport ou une vue [!UICONTROL Groupe], ce champ indique le nombre maximal de licences [!UICONTROL Plan] pouvant être attribuées aux utilisateurs dont le groupe respectif est désigné comme groupe d’accueil [!UICONTROL].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Licence Limite Work]</td> 
   <td> <p>Dans un rapport ou une vue [!UICONTROL Group], ce champ indique le nombre maximal de licences [!UICONTROL Work] pouvant être attribuées aux utilisateurs dont le groupe respectif est désigné comme leur groupe d’accueil [!UICONTROL].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limited User]</td> 
   <td>Un type de licence qui permet la création d’un [!DNL Access Level] qui contient des privilèges d’affichage uniquement, avec la possibilité d’envoyer des problèmes, de saisir des notes et de charger des documents.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Contrôles de liste]</td> 
   <td> <p>Partie de la [!UICONTROL Configuration de l’interface] qui permet de lier des filtres, des vues et des groupes personnalisés à des utilisateurs individuels ou globalement à tous les utilisateurs.</p> </td> 
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
   <td>[!UICONTROL Manuel Uniquement]</td> 
   <td> <p>L’un des [!UICONTROL Project] d’[!UICONTROL Update Types]. Ce paramètre permet de mettre à jour les chronologies [!UICONTROL Projet projeté] et [!UICONTROL Planifié] uniquement en cas de clic sur "[!UICONTROL Recalculated Timelines]". Les projets configurés de cette manière seront ignorés lors du processus de recalcul de nuit et lorsque le projet ou les tâches du projet seront mis à jour.</p> <p>Pour plus d’informations, voir <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Sélection du projet [!UICONTROL Update Type] </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Me]</td> 
   <td> <p>Cela fait référence à l’utilisateur actuellement connecté. </p> <p>Il est recommandé d'utiliser ce champ dans un filtre afin de rendre les rapports plus génériques lors de leur partage avec d'autres utilisateurs. Ainsi, vous ne pouvez créer qu’un seul rapport qui affichera des informations différentes en fonction de la personne qui se connecte pour les afficher, car les informations sont toujours personnalisées pour l’utilisateur connecté. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nombre max. d’utilisateurs]</td> 
   <td> <p>Il s’agit d’un champ obsolète. Toutes les informations que ce champ peut afficher sont liées à une fonctionnalité que [!DNL Workfront] a supprimée et le champ ne peut pas être mis à jour. </p> <p>Dans les versions précédentes de [!DNL Workfront], vous pouviez mettre à jour ce champ lors de la création ou de la modification d’un rôle de tâche. Il affichait le nombre total d’utilisateurs pouvant être associés à un rôle sur chaque projet. La valeur zéro est autorisée pour un nombre illimité d’utilisateurs pouvant être affectés à un projet. </p>Le champ est toujours visible dans certains rapports et listes, mais les informations affichées ne peuvent pas être mises à jour. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Milestone]</td> 
   <td> <p>Un marqueur que vous pouvez associer à une tâche pour indiquer qu’un point clé du projet a été atteint une fois la tâche terminée. Vous pouvez généralement utiliser des jalons pour afficher un événement significatif, tel que la fin d’une phase du projet ou un ensemble d’activités critiques. [!UICONTROL Jalons] sont généralement associés à des tâches parentes. Vous devez créer les jalons avant de pouvoir les joindre aux tâches. Pour plus d’informations sur les jalons, voir <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md">Création d’un chemin de jalon</a> et <a href="../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md">Association de jalons à des tâches</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Milestone Path]</td> 
   <td>Ensemble de [!UICONTROL milestones]. Les [!UICONTROL Milestone Paths] sont utilisés sur les projets pour distinguer les projets avec certains types de [!UICONTROL Milestones] des projets avec un ensemble différent de [!UICONTROL Milestones].</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Tâche Milestone]</td> 
   <td>Tâche marquée pour indiquer un événement à mesurer.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Module]</td> 
   <td>Une seule étape dans un scénario de [!DNL Workfront Fusion] qui exécute une fonction en fonction de l’application associée.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Mon rôle de Principal]</td> 
   <td> <p>Lorsqu’il est référencé dans les filtres, cela affiche soit les utilisateurs qui ont le même [!UICONTROL Rôle de Principal] que l’utilisateur connecté, soit les tâches affectées au [!UICONTROL Rôle de Principal] de l’utilisateur connecté.</p> <p>Il est recommandé d'utiliser ce champ dans un filtre afin de rendre les rapports plus génériques lors de leur partage avec d'autres utilisateurs. Ainsi, vous ne pouvez créer qu’un seul rapport qui affichera des informations différentes en fonction de la personne qui se connecte pour les afficher, car les informations sont toujours personnalisées pour l’utilisateur connecté. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Mon équipe d’accueil]</td> 
   <td> <p>Lorsqu’il est référencé dans les filtres, ce champ affiche soit les utilisateurs appartenant à l’[!UICONTROL Home Team] de l’utilisateur connecté, soit les tâches affectées à l’[!UICONTROL Home Team] de l’utilisateur connecté. </p> <p>Il est recommandé d'utiliser ce champ dans un filtre afin de rendre les rapports plus génériques lors de leur partage avec d'autres utilisateurs. Ainsi, vous ne pouvez créer qu’un seul rapport qui affichera des informations différentes en fonction de la personne qui se connecte pour les afficher, car les informations sont toujours personnalisées pour l’utilisateur connecté. </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Convention d’affectation de nom]</td> 
   <td>Ensemble de règles à l’échelle de l’organisation qui utilise les données pour créer des noms de projets, de tâches et de livrables.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Native Integration]</td> 
   <td>Une intégration qui ne nécessite pas de codage manuel ni de configuration d’API. Également appelé intégration "d’usine".</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Menu de navigation]</td> 
   <td>Panneau supérieur central de l’application qui contient des liens vers les principales zones de [!UICONTROL Workfront].</td> 
  </tr> 
 </tr> 
  <tr> 
   <td>[!UICONTROL Nouvelle valeur numérique]</td> 
   <td>Dans un rapport [!UICONTROL Entrée du journal], cette option affiche la valeur mise à jour d’un champ qui remplace la [!UICONTROL Ancienne valeur numérique].
   Pour plus d’informations, voir "[!UICONTROL Ancienne valeur numérique]" dans cet article.</td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL Frais non facturables]</td> 
   <td> <p>Une dépense qui n’est pas marquée comme facturable au client. Il peut s’agir soit d’une dépense planifiée, soit d’une dépense réelle.</p> <p>Les champs Coût des dépenses non facturables planifié et Coût des dépenses non facturables réel peuvent être ajoutés aux vues et aux rapports. Elles n’apparaissent pas sur les pages de détails du projet ou de la tâche.</p>
   <p>Vous trouverez ces champs dans les types de rapports suivants :</p>
   <ul>
   <li>Niveau de référence</li>
   <li>Modèle</li>
   <li>Projet (données financières)</li>
   </ul>
   <p>Pour plus d’informations sur le marquage d’une dépense comme facturable, voir <a href="/help/quicksilver/manage-work/projects/project-finances/manage-project-expenses.md">Gérer les dépenses de projet</a>.</p>
   </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Jour sans travail]</td> 
   <td>Un jour qui n’est attribué à aucune affectation. Il s’agit généralement d’un jour de vacances, de vacances ou de week-end. Le terme s’affiche dans l’explorateur d’API. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Remarque]</td> 
   <td>Commentaire ou mise à jour effectué sur un objet [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Texte de la remarque]</td> 
   <td> <p>Cette option affiche le texte d’une mise à jour saisie par un utilisateur sur n’importe quel objet. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Nombre d’objectifs liés]</td> 
   <td> <p>Dans un rapport [!UICONTROL Projet], il s’agit du nombre d’objectifs stratégiques associés au projet. Pour plus d’informations sur l’association de projets à des objectifs stratégiques, voir <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md">Ajout de projets à des objectifs dans [!DNL Adobe Workfront Goals]</a>.</p> 
   <p>Pour plus d’informations sur les objectifs stratégiques, voir aussi "[!UICONTROL Objectif]" dans cet article.</p> 
   <p>Ce champ n’est visible que si votre organisation a acheté [!DNL Workfront Goals]. Pour plus d’informations sur la gestion des objectifs stratégiques à l’aide de [!DNL Workfront Goals], voir <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md">Ajout de projets aux objectifs dans [!UICONTROL Adobe Workfront Goals]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Object]</td> 
   <td> <p>Les informations que vous affichez dans [!DNL Adobe Workfront] sont représentées par des objets stockés dans la base de données [!DNL Workfront]. Les objets sont ce qui motive les informations dans Workfront. Voici quelques exemples d’objets :</p> 
    <ul> 
     <li>[!UICONTROL Portfolio]</li> 
     <li>[!UICONTROL Programmes]</li> 
     <li>[!UICONTROL Projects]</li> 
     <li>[!UICONTROL Tasks]</li> 
     <li>[!UICONTROL Issues]</li> 
     <li>[!UICONTROL Documents]</li> 
     <li>[!UICONTROL Tableaux de bord]</li> 
     <li>[!UICONTROL Rapports]</li> 
     <li>[!UICONTROL Groups]</li> 
     <li>[!UICONTROL Équipes]</li> 
     <li>[!UICONTROL Users]</li> 
     <li>[!UICONTROL Entreprises]</li> 
     <li>[!UICONTROL Custom forms]</li>
     <li>[!UICONTROL Custom fields]</li>  
     <li>[!UICONTROL Hours]</li> 
     <li>[!UICONTROL Taux de facturation]</li> 
     <li>[!UICONTROL Modèles]</li> 
     <li>[!UICONTROL Tâches de modèle]</li>

<p><b>NOTE</b></p>
  <p>Ce n'est pas une liste exhaustive. </p>

</ul> <p>Pour plus d’informations, voir <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Comprendre les objets dans [!UICONTROL Adobe Workfront]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Types d’objet]</td> 
   <td>Si vous créez un rapport ou une liste contenant tous vos formulaires personnalisés, vous pouvez utiliser ce champ comme vue ou filtre pour identifier les types d’objets associés à chaque formulaire. </td> 
  </tr> 
 <tr> 
   <td>[!UICONTROL Ancienne valeur numérique]</td> 
   <td>Dans un rapport [!UICONTROL Entrée du journal], la valeur d’origine d’un champ s’affiche avant d’être mise à jour. Une fois la valeur d’un champ mise à jour, elle s’affiche sous la forme de la valeur [!UICONTROL New Number Value] dans un rapport [!UICONTROL Journal Entry] . Pour plus d’informations, voir également "[!UICONTROL Nouvelle valeur numérique]".</td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Sur Modification Uniquement]</td> 
   <td> <p>L’un des types [!UICONTROL Project Update]. Lorsque cette option est sélectionnée, les chronologies [!UICONTROL Projet projeté] et [!UICONTROL Planifié] ne sont mises à jour que lorsqu’une mise à jour ou une modification est apportée au projet ou à une tâche du projet. Il ne met pas à jour le projet tous les soirs.</p> <p>Pour plus d’informations, voir <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Sélectionner le type de mise à jour de projet </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Op Task]</td> 
   <td> <p>Nom du [!UICONTROL Problème] dans la base de données [!DNL Workfront], utilisé dans les rapports en mode texte ou dans les données personnalisées calculées.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ouvrir]</td> 
   <td>Un problème ou une tâche qui n’est pas terminé, mais sur lequel on travaille.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Graphique d’organisation]</td> 
   <td>Courte pour l’organigramme. Il s’agit d’un graphique qui montre la hiérarchie d’une organisation. Il se trouve également dans l’onglet de l’écran de détail [!UICONTROL User] qui affiche et permet de définir les relations [!UICONTROL User] de [!UICONTROL Company] et [!UICONTROL Reporting].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Configuration organisationnelle]</td> 
   <td>Cela définit les [!UICONTROL Sociétés], les [!UICONTROL Groupes] et les [!UICONTROL Profils de sécurité] pour votre organisation.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Autres groupes]</td> 
   <td> <p>Dans un rapport ou une vue qui répertorie les utilisateurs, ce champ affiche tous les groupes dont chaque utilisateur est membre. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Remplacer la devise]</span> </td> 
   <td> 
    <div> 
     <p>Dans un rapport [!UICONTROL Rôle de tâche], il s’agit de la devise associée à un rôle de tâche. Il s’agit d’un remplacement de la [!UICONTROL Devise de base] tel qu’il a été défini dans la zone [!UICONTROL Configuration] par l’administrateur [!DNL Workfront]. </p> 
     <p>Pour plus d’informations, voir <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Création et gestion des rôles de tâche</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Remplacer la facturation/heure de la devise]</span> </td> 
   <td> 
    <div> 
     <p>Dans un rapport [!UICONTROL Rôle de la tâche], il s’agit du taux de facturation par heure du rôle de la tâche à l’aide de la [!UICONTROL Devise de remplacement] sélectionnée du rôle de tâche.</p> 
     <p> Pour plus d’informations, voir <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Création et gestion des rôles de tâche</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Remplacer le coût/heure de la devise]</span> </td> 
   <td> 
    <div> 
     <p>Dans un rapport [!UICONTROL Rôle de la tâche], il s’agit du taux de coût par heure du rôle de tâche à l’aide de la [!UICONTROL Devise de remplacement] sélectionnée pour le rôle de tâche. </p> 
     <p>Pour plus d’informations, voir <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Création et gestion des rôles de tâche</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Propriétaire]</td> 
   <td>L’utilisateur responsable de la fin de l’objet désigné.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Type de propriétaire]</span> </td> 
   <td> 
    <div> 
     <p>Dans un rapport [!UICONTROL Objectif], celui-ci affiche le type de propriétaire affecté à un objectif stratégique. Voici les types de propriétaire d’objectif :</p> 
     <ul> 
      <li> <p>[!UICONTROL User]</p> </li> 
      <li> <p>[!UICONTROL Team] </p> </li> 
      <li> <p>[!UICONTROL Group]</p> </li> 
     </ul> 
     <p>Aucune valeur ne s’affiche dans ce champ lorsque le propriétaire de l’objectif est votre organisation. </p> 
     <p>Cela nécessite une licence supplémentaire. Pour plus d’informations sur [!DNL Workfront Goals], voir <a href="../../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">[!DNL Adobe Workfront Goals] - Aperçu</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

## P - R

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
   <td>Paramètre [!UICONTROL]</td> 
   <td> <p>Un paramètre [!UICONTROL] est un champ personnalisé. Vous pouvez créer un rapport pour tous les paramètres ou des champs personnalisés de votre système. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Parent]</td> 
   <td>Dans un rapport, ce champ affiche des informations sur le parent de l’objet. Par exemple, dans un rapport [!UICONTROL Problème], il peut afficher des informations sur la tâche ou le projet sous lequel le problème est connecté ; dans un rapport de tâche, il peut afficher des informations sur la tâche parent directe ou sur le projet. Pour plus d’informations sur les objets susceptibles d’avoir des parents dans [!DNL Workfront], voir la section "Interdépendance et hiérarchie des objets" dans l’article <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Comprendre les objets dans [!DNL Adobe Workfront]</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Journal parent]</td> 
   <td>Le temps qui doit s’écouler entre le démarrage de la [!UICONTROL Tâche parent] et le démarrage de la [!UICONTROL Subtask].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tâche Parente]</td> 
   <td>Connue également sous le nom de [!UICONTROL Tâche de résumé]. Il s’agit d’une tâche qui comporte des sous-tâches (également appelées [!UICONTROL Children Tasks]). La [!UICONTROL Durée], le [!UICONTROL Travail requis] et le [!UICONTROL Pourcentage terminé] de la tâche parente sont calculés à partir des sous-tâches.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Ressources à temps partiel]</td> 
   <td>Un utilisateur disposant d’une licence ayant une capacité inférieure à la planification par défaut définie dans le système.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pourcentage terminé]</td> 
   <td> <p>Champ de projet, de tâche ou de problème qui indique le pourcentage de travail associé à la tâche, au projet ou au problème qui est terminé.</p> <p>Vous pouvez mettre à jour ce champ manuellement pour les problèmes et les tâches de travail. </p> <p>Pour les projets et les tâches parentes, ce champ est un cumul de toutes les tâches opérationnelles et vous ne pouvez pas le mettre à jour manuellement. </p> <p>Pour plus d’informations, consultez la <a href="../../../manage-work/tasks/task-information/project-percent-complete.md" class="MCXref xref">présentation du projet [!UICONTROL Pourcentage terminé]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Permission]</td> 
   <td> <p>Droits accordés à un utilisateur sur un objet, généralement donnés pour lui permettre de terminer le travail sur l’élément ou d’afficher l’élément. Vous pouvez accorder des autorisations pour :</p> 
    <ul> 
     <li>[!UICONTROL Projects]</li> 
     <li>[!UICONTROL Tasks]</li> 
     <li>[!UICONTROL Issues]</li> 
     <li>[!UICONTROL Portfolio]</li> 
     <li>[!UICONTROL Programmes]</li> 
     <li>[!UICONTROL Rapports]</li> 
     <li>[!UICONTROL Tableaux de bord]</li> 
     <li>[!UICONTROL Documents]</li> 
     <li>[!UICONTROL Custom Forms]</li> 
     <li>[!UICONTROL Views]</li> 
     <li>[!UICONTROL Filtres]</li> 
     <li>[!UICONTROL Groupements]</li> 
    </ul> <p>Pour plus d’informations, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Vue d’ensemble du partage des autorisations sur les objets</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Plan]</td> 
   <td> <p>Il s’agit d’un type de licence complet dans le système [!DNL Workfront]. Les utilisateurs doivent disposer de cet accès pour accéder à toutes les fonctionnalités de [!DNL Workfront].</p> <p>Pour plus d’informations, voir <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] - Présentation des licences</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Plan] (dans le [!DNL Scenario Planner])</td> 
   <td> <p>Un plan est l’objet principal lors de l’utilisation du planificateur de scénario [!DNL Workfront]. Vous pouvez définir la stratégie à court et à long terme de votre entreprise, identifier chaque résultat de haut niveau et l’ajouter en tant que plan au planificateur de scénario [!DNL Workfront]. </p> <p>Vous ne pouvez pas afficher [!DNL Scenario Planner] plans dans un rapport et vous ne pouvez pas y accéder via l’API [!DNL Workfront]. </p> <p>[!DNL Scenario Planner] nécessite une licence supplémentaire. Pour plus d'informations sur [!DNL Workfront Scenario Planner], consultez la <a href="../../../scenario-planner/scenario-planner-overview.md">présentation [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planifié]</td> 
   <td> <p>Période pendant laquelle un événement est programmé. Lorsque vous créez des projets, des tâches ou des problèmes dans [!DNL Workfront], vous définissez les dates de début et de fin prévues, ainsi que la période prévue pendant laquelle elles se produisent. Ces valeurs représentent votre intention initiale ou votre estimation du temps nécessaire à l’exécution d’un élément. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Bénéfice prévu]</td> 
   <td>Il s’agit d’une entrée manuelle permettant au gestionnaire de projet d’estimer si la réalisation d’un projet apporterait un avantage financier à l’organisation. La spécification de cette valeur peut faire partie de l’assemblage d’un [!UICONTROL Business Case] pour le projet. Pour mettre à jour cette valeur, vous devez disposer des autorisations [!UICONTROL Gérer] pour le projet.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Heures planifiées budgétisées]</td> 
   <td> <p>Dans un rapport [!UICONTROL Heure planifiée], il indique le nombre d’heures budgétisées pour les projets ou les [!UICONTROL Rôles de tâche] dans le [!UICONTROL Resource Planner]. </p> <p>Pour plus d’informations sur la planification des projets ou des rôles dans le [!UICONTROL Resource Planner], consultez l’article <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Ressources de budget dans le [!UICONTROL Resource Planner] à l’aide des vues [!UICONTROL Project] et [!UICONTROL Role]</a>. Pour plus d’informations sur le rapport [!UICONTROL Hours budgétés], voir l’article <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref">Rapport : Heure budgétée</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Date d’achèvement prévue]</td> 
   <td> <p>Vous pouvez définir manuellement la [!UICONTROL Date d’achèvement planifiée] d’une tâche, d’un projet ou d’une émission à une date de votre choix. Si vous ne définissez pas la [!UICONTROL Date d’achèvement planifiée], [!DNL Workfront] la définit automatiquement. Lorsqu’elle est définie automatiquement, la [!UICONTROL Date d’achèvement planifiée] est : [!UICONTROL Date de début planifiée] + [!UICONTROL Durée]</p> <p>Pour plus d’informations, consultez les articles suivants :</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Présentation de la tâche [!UICONTROL Date d’achèvement planifiée]</a> </p> </li> 
     <li> <p><a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">Définition de la date d’achèvement prévue du projet [!UICONTROL]</a> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Coût planifié]</td> 
   <td> <p>Total du [!UICONTROL Coût planifié de la main-d’oeuvre] et du [!UICONTROL Coût planifié des dépenses] du projet. Cela n’inclut pas le coût du risque planifié [!UICONTROL] sur le projet.  </p> </td> 
  </tr>



<tr> 
   <td>[!UICONTROL Alignement des dates planifiées]</td> 
   <td> <p>Il s’agit d’un indicateur automatique selon lequel Workfront attribue des projets, des tâches et des problèmes à afficher lorsqu’un élément sera terminé par rapport à sa date d’achèvement planifiée. </p>
   <p>Voici les valeurs possibles pour l’indicateur d’alignement de la date planifiée : </p>
<ul>
<li>Sera terminé à la date d'achèvement prévisionnelle</li>
<li>Sera terminé avant la date d'achèvement prévisionnelle</li>
<li>Sera terminé après la date d'achèvement prévisionnelle</li></ul>
<p>L’alignement des dates prévues est visible dans les listes et rapports des projets, des tâches et des problèmes. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Durée planifiée]</td> 
   <td> <p>La [!UICONTROL Durée planifiée] d’une tâche est généralement identique à la [!UICONTROL Durée de la tâche]. Il représente la différence en jours entre le [!UICONTROL Début planifié] et les [!UICONTROL Dates d’achèvement planifiées] de la tâche. </p> <p>Lorsque la tâche possède un type [!UICONTROL Durée] d’[!UICONTROL Effort piloté], la [!UICONTROL Durée planifiée] peut différer de la [!UICONTROL Durée] de la tâche, en fonction du nombre de ressources affecté à la tâche. </p> <p>Par exemple, si une tâche avec une [!UICONTROL Durée] de type [!UICONTROL Effort piloté] a une [!UICONTROL Durée] de 3 jours et que vous attribuez une ressource avec un planning à temps plein à la tâche, la [!UICONTROL Durée planifiée] est également de 3 jours. Si vous attribuez trois ressources avec un planning à temps plein à la même tâche, la [!UICONTROL Durée] reste de 3 jours, mais la [!UICONTROL Durée planifiée] devient de 1 jour. La [!UICONTROL Durée planifiée] modifie également les dates [!UICONTROL Début planifié] et [!UICONTROL Fin planifiée] de la tâche, afin de refléter la nouvelle [!UICONTROL Durée planifiée]. Par conséquent, la chronologie du projet est également affectée. </p> <p>Pour plus d’informations sur la différence entre la [!UICONTROL Durée] et la [!UICONTROL Durée planifiée] pour les tâches, consultez l’article <a href="../../../manage-work/tasks/task-information/planned-duration-vs-duration-for-tasks.md" class="MCXref xref">Différence entre la [!UICONTROL Durée planifiée] et la [!UICONTROL Durée] pour les tâches </a>.</p> <p>Les projets et problèmes n’ont pas de [!UICONTROL Durée planifiée]. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Minutes de durée planifiée]</td> 
   <td> <p>Le [!UICONTROL Durée planifiée minutes] d’un projet ou d’un problème correspond à la [!UICONTROL Durée] du projet ou du problème en minutes. </p> <p>Les tâches n’ont pas de champ [!UICONTROL Durée planifiée Minutes] . </p> <p>Les [!UICONTROL Tâches du modèle] comportent un champ [!UICONTROL Durée planifiée minutes] qui affiche la [!UICONTROL Durée planifiée] de la tâche en minutes. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Coût des dépenses prévues]</td> 
   <td> <p>Somme des [!UICONTROL Montants prévus] pour toutes les dépenses enregistrées pour un projet ou une tâche.</p> <p><b>EXEMPLE</b></p>
   <p>Si vous créez une dépense pour la tâche 1 et que vous saisissez 600,00 $ dans le champ [!UICONTROL Montant planifié] , le [!UICONTROL Coût des dépenses planifiées] de cette tâche est de 600,00 $. </p> 
   <p>Pour un projet, [!DNL Workfront] utilise la formule suivante pour calculer le [!UICONTROL Coût des dépenses planifiées] :</p> <p><code>Project [!UICONTROL Planned Expense Cost] = SUM (All Project [!UICONTROL Planned Expense Costs]) + SUM (All Tasks [!UICONTROL Planned Expense Costs])</code> </p> 
   <!--
     <p>Important: If the value in the Actual Amount field for an expense is negative, Workfront will ignore that expense record. For example, if the value in the Planned Amount field is $200.00 but the value in the Actual Amount field is -$300.00, the system will ignore this entire expense record which means you would not include the $200.00 planned value or the -$300.00 actual value in any calculations for Planned Expense Cost or Actual Expense Cost. (Drafting this because not sure if this is correct anymore)</p>
    --> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Heures planifiées]</td> 
   <td> <p>Ce champ s’affiche dans les sections [!UICONTROL Projets], [!UICONTROL Tâches], Problèmes, Rapports relatifs aux projets, aux tâches ou aux problèmes, ainsi que dans les outils de gestion des ressources tels que [!UICONTROL Resource Planner], [!UICONTROL Workload Balancer] et le rapport [!UICONTROL Utilitation]. </p> <p>Il indique le nombre d’heures que le propriétaire du projet estime nécessaire à l’exécution de chaque tâche ou problème. Pour les projets, il s’agit généralement d’un cumul des [!UICONTROL Heures planifiées] des tâches du projet. </p> <p>Le champ [!UICONTROL Heures planifiées] peut afficher différentes informations selon l’endroit d’où vous l’affichez. Pour plus d’informations sur le nombre d’heures prévues, voir <a href="../../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref">Vue d’ensemble du nombre d’heures prévues</a>.</p> <p>Les heures planifiées sont stockées en minutes dans la base de données [!DNL Workfront]. Lorsque vous rédigez des calculs à l’aide de ce champ, veillez à tenir compte du fait que les heures s’affichent en minutes.<br></p> <p>Par défaut, les Heures planifiées sont réparties uniformément sur tous les jours pendant la durée d’un élément de travail et également sur toutes les ressources affectées à la tâche. Les utilisateurs peuvent mettre à jour le nombre quotidien d’heures planifiées pour un élément de travail ou le nombre d’heures planifiées individuelles pour chaque personne désignée.</p> <p>La mise à jour de ce champ diffère pour les projets, les tâches et les problèmes : </p> 
    <ul> 
     <li> <p>Pour les problèmes, vous pouvez mettre à jour ce champ manuellement. Problème : les heures planifiées ne sont pas ajoutées aux heures planifiées du projet. </p> <p><b>CONSEIL</b></p> <p>Dans un rapport de problème, l’un des champs [!UICONTROL Heures planifiées] est remplacé par le champ [!UICONTROL Travail] . Le champ affiche le nombre d’heures planifiées sur le problème. Pour plus d’informations, voir les champs "work" ou "[!UICONTROL Work]" de ce tableau. </p> </li> 
    </ul> 
    <ul> 
     <li> <p>Pour les tâches, vous pouvez mettre à jour manuellement ce champ lorsque le [!UICONTROL Type de durée] de la tâche est [!UICONTROL Affectation calculée] ou [!UICONTROL Simple]. Ce champ est calculé par [!DNL Workfront] lorsque le [!UICONTROL Duration Type] de la tâche est [!UICONTROL Calculated Work] ou [!UICONTROL Effort Driven].<br>Pour plus d’informations sur [!UICONTROL Durée de la tâche], consultez l’article <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Présentation de la durée de la tâche [!UICONTROL] et [!UICONTROL Type de durée]</a>.</p> </li> 
    </ul> 
    <ul> 
     <li> <p>Pour les projets, [!DNL Workfront] calcule les heures planifiées en ajoutant toutes les heures planifiées de toutes les tâches du projet. </p> </li> 
    </ul> <p><b>CONSEIL</b></p> <p>Vous pouvez afficher les [!UICONTROL Heures planifiées] dans les rapports [!UICONTROL Projet], [!UICONTROL Tâche] ou [!UICONTROL Problèmes] en utilisant également le mode texte et en référençant des champs supplémentaires. Pour plus d’informations, voir les champs "<code>work</code>", "[!UICONTROL Work]" et "<code>workRequiredExpression</code>" de cette table. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Coût du travail planifié]</td> 
   <td> 
    <p>Pour une tâche, le taux horaire de l’utilisateur ou du rôle multiplié par le nombre d’heures attribué à l’utilisateur ou au rôle.</p> <p>Pour un projet, il s’agit du total des [!UICONTROL Coûts du travail planifiés] de toutes les tâches.</p> <p>Le taux d’utilisation de l’utilisateur ou du rôle dépend du type de coût sélectionné pour la tâche donnée. </p> <p>Pour plus d’informations, voir <a href="../../../manage-work/projects/project-finances/track-costs.md">Tracker les coûts</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Recettes prévues]</td> 
   <td> <p>Les tâches et les projets peuvent afficher une valeur pour [!UICONTROL Recettes prévues] dans [!DNL Workfront]. [!UICONTROL Recettes prévues] représente le montant d’argent associé aux [!UICONTROL Heures planifiées] des tâches du projet. Pour les projets, il peut également inclure les [!UICONTROL Recettes fixes] du projet. </p> <p>Pour les tâches, il s’agit des recettes associées aux [!UICONTROL Heures planifiées] des tâches. Les Heures planifiées de toutes les tâches s’étendent jusqu’aux Heures planifiées du projet afin de contribuer au calcul du projet [!UICONTROL Heures planifiées]. </p> 
   <p>[!DNL Workfront] calcule les [!UICONTROL Recettes prévues] pour les tâches et les projets à l’aide des formules suivantes :</p> 
   <p><code>Task [!UICONTROL Planned Revenue] = [!UICONTROL Planned Hours] * Billing hourly rate</code> </p> <p><code>Project [!UICONTROL Planned Revenue] = SUM (All tasks [!UICONTROL Planned Revenue]) + [!UICONTROL Fixed Revenue]</code> </p> 
   <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(the note below is duplicated in this article: /Content/Resource Mgmt/Resource utilization/view-utilization-information.htm and in the glossary)</p>
    --> 
    <p>Le projet [!UICONTROL Recettes prévues] qui s’affiche dans la zone [!UICONTROL Détails du projet] et dans les rapports du projet diffère des recettes prévues qui s’affichent dans le rapport [!UICONTROL Utilisation]. </p> <p>La zone [!UICONTROL Recettes planifiées] dans la zone [!UICONTROL Détails du projet] reflète les recettes de la tâche ainsi que les recettes fixes du projet. Le rapport [!UICONTROL Recettes prévues] du rapport [!UICONTROL Utilisation] affiche les [!UICONTROL Recettes prévues] associées uniquement aux tâches du projet. </p> 
     <p><b>EXEMPLE</b></p>  
      <p>Si le projet comporte une tâche de 10 heures, affectée à un consultant avec un taux horaire de 20 $ et que le projet a un revenu fixe de 100 $, le rapport [!UICONTROL Utilisation] affiche 200 $ pour [!UICONTROL Recettes prévues] (le rapport [!UICONTROL Recettes prévues] associé aux heures de la tâche). La section [!UICONTROL Détails du projet] affiche 300 $ (les [!UICONTROL Recettes prévues] de la tâche et les recettes fixes du projet.) </p> 
    <p>Pour plus d’informations sur le suivi des recettes dans [!DNL Workfront], voir <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md">Présentation de la facturation et des recettes</a>. </p> 
    <p>Pour plus d’informations sur les calculs [!UICONTROL Recettes prévues] dans le [!UICONTROL Rapport d’utilisation], voir <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md">Affichage des informations sur l’utilisation des ressources </a>. </p> 
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Coût des risques prévus]</td> 
   <td> <p>Total du [!UICONTROL Coût potentiel] de tous les risques sur le projet en tenant compte de leur probabilité de réalisation. Ce montant n’est pas inclus dans le coût planifié du projet.</p> <p>Le [!UICONTROL Coût des risques planifiés] d’un projet est calculé selon la formule suivante :</p> <p><code>Planned Risk Cost = SUM(Potential Risk Cost * Probability / 100)</code> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Portal Profile]</td> 
   <td>Collection définie par l’administrateur d’onglets et de sections du portail qui s’affiche sur l’[!UICONTROL Accueil] de l’application [!DNL Workfront] et d’autres tableaux de bord.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Portal Section]</td> 
   <td>Un composant d’un onglet sur un tableau de bord ou une page de portail. Généralement un seul rapport, graphique, calendrier ou liste d’informations clés.</td> 
  </tr> 
  <tr> 
   <td>Onglet [!UICONTROL Portal]</td> 
   <td>Un onglet d’un portail ou d’un tableau de bord qui contient jusqu’à trois sections du portail.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Portfolio]</td> 
   <td> <p>Ensemble de projets présentant des caractéristiques d’unification. Ces projets sont généralement en concurrence pour les mêmes ressources, le même budget ou la même tranche horaire. Vous pouvez diviser les Portfolios en programmes et associer les projets aux programmes avant de les ajouter à un Portfolio.</p> <p>Pour plus d’informations sur les portefeuilles, consultez la <a href="../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md">présentation des Portfolios dans [!DNL Adobe Workfront]</a>.</p> 
   </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Portfolio Management]</td> 
   <td>Un domaine de pratique axé sur la gestion d’une collection ou de programmes connexes et les efforts du projet.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Portfolio Optimizer]</td> 
   <td>Un outil [!DNL Workfront] pour aider à évaluer et à hiérarchiser les projets au sein d’un portefeuille.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Propriétaire du Portfolio]</td> 
   <td>Les parties prenantes responsables de la définition des priorités et du budget d’un portefeuille.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Coût des risques potentiels]</td> 
   <td>Il s’agit d’un champ de projet que vous pouvez trouver dans les listes et les rapports. Il indique le coût potentiel des risques associés au projet, s’ils se produisent. Pour plus d’informations, voir <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">Calculer le coût du risque potentiel </a>. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Predecessor]</td> 
   <td> <p>Tâche qui doit être complétée avant la fin d’une tâche dépendante. Une tâche également marquée comme [!UICONTROL Dependency] pour une autre tâche. Les prédécesseurs permettent au planificateur de définir une logique de dépendance de séquence, par exemple pour démarrer une tâche une fois qu’une autre tâche est terminée.</p> <p>Pour plus d’informations, voir <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">Présentation des prédécesseurs de tâches</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Principal Company]</td> 
   <td>Société à laquelle appartient l’utilisateur comme indiqué dans ses paramètres utilisateur. Les entreprises peuvent également être associées à des projets.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Contact de Principal]</td> 
   <td><p>Le [!UICONTROL Contact de Principal] est le créateur d’un problème et il est automatiquement désigné par [!DNL Workfront] lorsque la personne crée le problème. Vous pouvez mettre à jour manuellement ce champ si vous disposez de [!DNL Manage] autorisations sur le problème. Un problème ne peut avoir qu’un contact de Principal.</p> 
   <p>Si vous modifiez le contact de Principal, l’utilisateur désigné à l’origine comme contact principal a toujours accès à [!UICONTROL Gérer].</p>
   <p>Lors de la conversion d’un problème en une tâche ou un projet, l’utilisateur désigné comme le [!UICONTROL Contact de Principal] du problème devient l’[!UICONTROL Converted Issue Originator] du projet ou de la tâche. Si le [!UICONTROL Contact de Principal] du problème est mis à jour après la conversion du problème, le [!UICONTROL Converted Issue Originator] sera conservé en tant que [!UICONTROL Principal Contact] du problème au moment de la conversion. Voir aussi "[!UICONTROL Converted Issue Originator]" dans cet article.</p> 
   </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Priority]</td> 
   <td>Valeur pouvant être affectée à une tâche, à un problème ou à un projet pour désigner l’importance de cette tâche. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Private]</td> 
   <td>Dans une [!UICONTROL Remarque] ou un [!UICONTROL Document], cette option masque cet objet à la plupart des visionneuses. Pour une file d’attente de demandes d’aide privée, seuls les utilisateurs de l’équipe de projet peuvent envoyer des problèmes à cette file d’attente (ou projet) par le biais de la zone [!UICONTROL Demandes] .</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Profile]</td> 
   <td>Toutes les informations sur un compte d’utilisateur.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Program]</td> 
   <td> <p>Un sous-ensemble au sein d’un portefeuille, où des projets similaires peuvent être regroupés afin d’obtenir un avantage bien défini.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Gestion de programme]</td> 
   <td>la gestion des dépendances, des risques, des problèmes, des exigences et des solutions croisées pour maintenir le programme en bonne santé et obtenir les avantages définis du programme.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Propriétaire du programme]</td> 
   <td>Les parties prenantes responsables de la supervision et de l’organisation des activités pour s’assurer que les objectifs du projet correspondent aux objectifs de l’entreprise.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Progression]</span> </td> 
   <td> <p>Dans un rapport [!UICONTROL Objectif], ce rapport indique le pourcentage de la distance entre un objectif stratégique et son exécution. Le pourcentage de progression s’affiche sous la forme d’un nombre. Pour plus d’informations sur les objectifs stratégiques, voir aussi "[!UICONTROL Objectif]" dans ce tableau.</p> <p>Ce champ n’est visible que si votre entreprise a acheté [!DNL Workfront] Objectifs. Pour plus d'informations sur la gestion des objectifs stratégiques à l'aide de [!DNL Workfront Goals], voir <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md"> Ajout de projets aux objectifs dans [!DNL Adobe Workfront Goals] </a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL État de progression]</td> 
   <td> <p>Dans un rapport Projet, Tâche et Objectif, ce champ affiche l’état d’avancement des projets, des tâches ou des objectifs stratégiques. Pour plus d’informations, consultez les articles suivants :</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/projects/planning-a-project/project-progress-status.md" class="MCXref xref">Présentation de l’état de progression du projet</a> </p> </li> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">Présentation de l’état de progression de la tâche</a> </p> </li> 
     <li> <p><a href="../../../workfront-goals/goal-management/calculate-goal-progress.md">Présentation de la progression et de la condition de l’objectif dans [!DNL Adobe Workfront Goals]</a> </p>
     <p>Le rapport [!UICONTROL Objectif] et le champ [!UICONTROL État d’avancement] pour [!DNL goals] ne sont visibles que si votre entreprise a acheté [!DNL Workfront Goals]. Pour plus d’informations sur les objectifs stratégiques dans [!DNL Workfront Goals], voir <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] - Aperçu</a>. </p> </li>
    </ul> </td> 
  </tr> 
  <td>[!UICONTROL Project]</td> 
   <td> <p>Une grande quantité de travail qui doit être effectuée dans un délai spécifique et qui doit utiliser un budget et un nombre spécifiques de ressources. Pour le rendre gérable, vous divisez le projet en une série de tâches. La réalisation de toutes les tâches entraîne la fin du projet. Pour plus d’informations sur la planification d’un projet, consultez la section <a href="../../../manage-work/projects/planning-a-project/plan-project.md">Planification d’un projet</a>.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Heures planifiées d’affectation de projet]</td> 
   <td> <p>Dans un rapport [!UICONTROL Rôle de tâche de l’initiative] , il indique le nombre d’[!UICONTROL Heures planifiées] associées à un rôle de tâche affecté à des tâches ou à des problèmes dans le projet. Ce champ et le type de rapport [!UICONTROL Initiative Job Role] ne s’affichent pas dans votre instance [!DNL Workfront], sauf si votre entreprise a acheté une licence [!DNL Workfront Scenario Planner]. Pour plus d'informations sur [!DNL Workfront Scenario Planner], consultez la <a href="../../../scenario-planner/scenario-planner-overview.md">présentation [!DNL Workfront Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Détails du projet]</td> 
   <td>Détails de l’état actuel d’un projet.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Coût budgété du projet]</td> 
   <td> <p> Il s’agit du [!UICONTROL Coût budgété] d’un projet tel qu’il s’affiche dans les listes et les rapports.</p><p>Voir aussi "[!UICONTROL Coût budgété]" dans cet article.</p></td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Gestion de projet]</td> 
   <td>Ensemble de stratégies qui détermine les seuils de création, de classification et d’attribution de noms des projets.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Project Overhead]</td> 
   <td>Dans un rapport [!UICONTROL Heure], ce champ est réservé aux informations financières liées aux heures consignées avec le type d’heure de [!UICONTROL Heure du projet]. Les projets peuvent avoir leurs propres taux de facturation. Si une heure est enregistrée directement sur un projet, ces taux seront utilisés dans les calculs. En fonction des paramètres du projet, les projets peuvent également présenter des devises différentes et une conversion de devise peut être effectuée pour ces heures. L’objet [!UICONTROL Project Overhead] permet à [!DNL Workfront] d’obtenir ces informations.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Propriétaire du projet]</td> 
   <td>Utilisateur responsable de la gestion de la portée, de la chronologie et des affectations d’un projet. Approbateur par défaut pour les commandes de modification, les modifications financières et les livrables.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planification du projet]</td> 
   <td>Processus d’élaboration et de gestion du calendrier du projet.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sponsor De Projet]</td> 
   <td>Profil de parties prenantes désigné auquel chaque utilisateur doit se référer. Dans [!DNL Workfront], ils sont désignés comme [!UICONTROL Niveaux d’accès]</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Équipes de projet]</td> 
   <td> <p>Collection d’utilisateurs ou de rôles affectée à un projet</p> <p>Pour plus d’informations, voir <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md">Présentation de l’équipe de projet</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Suivi de projet]</td> 
   <td>Données utilisées pour mesurer l’intégrité et la portée d’un projet</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Projeté]</td> 
   <td> <p>Estimation de l’horodatage du moment où le travail sera terminé en fonction des heures planifiées et du pourcentage d’achèvement d’une tâche, d’un problème ou d’un projet.</p> <p>Cela fait référence aux dates ou à la [!UICONTROL Durée] de tâches, de problèmes ou de projets. En règle générale, il désigne les dates et les durées plus fidèles à la vie des éléments de travail, une fois que certains travaux ont été terminés ou qu’un certain temps s’est écoulé. </p> <p>Par exemple, la [!UICONTROL Date d’achèvement prévue] d’une tâche correspond à la date à laquelle [!DNL Workfront] estime que la tâche se terminera, en fonction du volume de travail qui y a été effectué jusqu’à présent, du nombre de personnes qui y sont affectées et du temps écoulé depuis la date de début.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Date limite de vérification]</td> 
   <td> <p>Dans les rapports qui contiennent l’objet [!UICONTROL Document Version] (tels qu’un rapport [!UICONTROL Document Version] et un rapport [!UICONTROL Approbation de BAT]), ce champ affiche le jour de la semaine, la date, l’heure et l’année de l’échéance du BAT.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Test Decision]</td> 
   <td> <p>Dans les rapports qui contiennent l’objet [!UICONTROL Document Version] (par exemple, un rapport [!UICONTROL Document Version]  et le rapport [!UICONTROL Approbation de BAT], ce champ affiche l’état de décision du BAT (en attente, modifications requises ou approuvées).</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof Name]</td> 
   <td> <p>Dans les rapports qui contiennent l’objet [!UICONTROL Document Version] (comme un rapport [!UICONTROL Document Version] et un rapport [!UICONTROL Approbation de BAT]), ce champ affiche le nom du BAT.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof Pages]</td> 
   <td> <p>Dans les rapports qui contiennent l’objet [!UICONTROL Document Version] (tels qu’un rapport [!UICONTROL Document Version] et un rapport [!UICONTROL Approbation de BAT]), ce champ affiche le nombre de pages incluses dans le BAT.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Progrès De La Preuve]</td> 
   <td> <p>Dans les rapports contenant l’objet [!UICONTROL Document Version] (tels qu’un rapport [!UICONTROL Document Version] et un rapport [!UICONTROL Approbation de BAT]), affiche l’état d’avancement du BAT ([!UICONTROL Envoyé], [!UICONTROL Ouvert], [!UICONTROL Commenté], [!UICONTROL Décision prise]).</p> <p>Pour plus d’informations, consultez la <a href="../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md#understanding-progress-and-status" class="MCXref xref">présentation de la progression du BAT</a> dans <a href="../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md" class="MCXref xref">  Proof progress and status overview</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Vérification]</td> 
   <td>Processus de révision au cours duquel un ou plusieurs utilisateurs marquent et commentent du contenu qui doit être modifié dans une image, un document texte, une vidéo ou du contenu web interactif.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Public]</td> 
   <td>Sur une [!UICONTROL Remarque] ou un [!UICONTROL Document], cette option rend cet objet accessible à d’autres utilisateurs, voire à des personnes extérieures à [!DNL Workfront]. Pour une [!UICONTROL File d’attente de demandes d’aide], [!UICONTROL Public] signifie que tous les utilisateurs qui peuvent soumettre des problèmes à un projet peuvent soumettre des problèmes par le biais de la zone [!UICONTROL Demandes].</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Qualité]</td> 
   <td>La perception de la qualité du travail au sein de l’organisation.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File d’attente]</td> 
   <td>Également appelé File d’attente du service d’aide ou [!UICONTROL File d’attente des demandes d’aide]. Il s’agit d’un projet qui a été publié dans la zone [!UICONTROL Demandes] pour permettre aux utilisateurs de lui soumettre des problèmes. En règle générale, des files d’attente sont créées pour des rubriques particulières, telles que [!UICONTROL Bogues], [!UICONTROL Requêtes de projet], etc.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Propriétés de la file d’attente]</td> 
   <td>Ces paramètres définissent les règles d’envoi des problèmes pour un projet qui est publié dans la zone [!UICONTROL Demandes] .</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Rubrique de la file d’attente]</td> 
   <td> <p>Une propriété sur une [!UICONTROL File d’attente de demande d’aide] qui permet aux utilisateurs d’envoyer un problème pour sélectionner une rubrique. Les rubriques peuvent :</p> 
    <ul> 
     <li>Être associé à un formulaire de données personnalisé.</li> 
     <li>Attribuez automatiquement le problème à un utilisateur, à un rôle ou à une équipe par le biais du jeu de règles de routage sur la rubrique sélectionnée.</li> 
     <li>Déplacez le problème vers un autre projet ou file d’attente par le biais du jeu de règles de routage sur la rubrique sélectionnée.</li> 
    </ul> <p>Pour plus d’informations, voir <a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">Créer des rubriques de file d’attente</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Classement]</td> 
   <td> <p>Dans un rapport [!UICONTROL Niveau d’accès], vous pouvez indiquer manuellement un [!UICONTROL Classement] du [!UICONTROL Niveau d’accès]. Cela vous permet, en tant qu’administrateur [!DNL Workfront], d’identifier visuellement le niveau de complexité associé à chaque niveau d’accès. Par exemple, vous pouvez attribuer des nombres plus faibles pour les niveaux d’accès plus complexes ([!UICONTROL Plan]) et des nombres plus élevés pour les niveaux d’accès moins complexes ([!UICONTROL Requester]). Vous ne pouvez pas classer les niveaux d’accès standard. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ready]</td> 
   <td> <p>Ce champ d’un rapport de tâche indique si une tâche [!UICONTROL Agile] a été marquée comme [!UICONTROL Ready] (Prêt pour UICONTROL) sur le journal en souffrance. Cet indicateur s’applique uniquement aux tâches [!UICONTROL Agile], qui sont des tâches affectées à une équipe [!UICONTROL Agile]. </p> </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Fréquence de périodicité]</td> 
   <td> <p>Champ qui s’affiche dans la zone [!UICONTROL Détails de la tâche] ou [!UICONTROL Modifier la tâche] d’un parent de tâches récurrentes. Il s’agit de la fréquence à laquelle les tâches de la périodicité se produisent. Pour plus d’informations sur la création de tâches récurrentes, voir <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Créer des tâches récurrentes</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Reference Number]</td> 
   <td> <p>Les projets, tâches et problèmes sont automatiquement associés à un numéro de référence unique au fur et à mesure de leur création. Vous pouvez afficher le [!UICONTROL Numéro de référence] sur la page [!UICONTROL Détails] des projets, tâches ou problèmes, ou dans une liste ou un rapport. </p> <p><b>CONSEIL</b><p><br>Vous pouvez vous reporter aux numéros de référence lorsque deux éléments portent le même nom, car les numéros de référence sont toujours uniques. </p> <p>[!DNL Workfront] génère automatiquement des numéros de référence séquentiels au niveau du système. Chaque projet, tâche ou problème obtient le prochain numéro disponible dans la séquence. <br></p> <p>Par exemple, si l’utilisateur A crée une tâche, [!DNL Workfront] peut attribuer automatiquement la tâche au numéro de référence 100. Si l’utilisateur B crée un problème juste après, [!DNL Workfront] lui affecte le numéro de référence 101. Vous ne pouvez pas modifier manuellement les numéros de référence. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Problème De Rejet]</td> 
   <td>Dans un projet ou un rapport de tâche, il s’agit du problème créé lorsque l’approbation du projet ou de la tâche est rejetée. Pour plus d’informations sur les problèmes de rejet, voir l’article <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Créer un processus d’approbation pour les tâches</a>. </td> 
  </tr>

<tr>
  <td>Types de relation</td>
  <td><p>Les objets Workfront sont toujours connectés les uns aux autres à l’aide de l’un des types de relations suivants :</p>

<ul><li> <b>Un à plusieurs</b> : dans cette relation, un objet peut être connecté à plusieurs autres objets de différents types. Par exemple, un projet peut comporter plusieurs tâches. La relation Projet-Tâches est une relation unique à plusieurs. Vous ne pouvez pas afficher cette relation dans un rapport à l’aide de l’interface Standard. Vous devez utiliser la création de rapports en mode texte pour afficher une ou plusieurs relations.</li>
  <li><b>Un à un</b> : dans cette relation, un objet ne peut être connecté qu’à un autre objet d’un type différent. Par exemple, un projet ne peut comporter qu’un seul groupe. La relation Projet-Groupe est une relation de type "un à un". Vous pouvez afficher une relation unique entre les objets d’un rapport standard.</li>
  <li><b>Plusieurs à un</b> : dans cette relation, plusieurs objets peuvent être connectés à un seul autre objet d’un type différent. Par exemple, plusieurs tâches peuvent être connectées au même projet. La relation Tâches-Projet est une relation multiple-à-un. Vous pouvez afficher plusieurs relations d’un objet à l’autre dans un rapport standard. </li>
  <li><b>Plusieurs à plusieurs</b> : dans cette relation, plusieurs objets du même type peuvent être connectés à plusieurs objets d’un type différent. Par exemple, plusieurs utilisateurs peuvent appartenir à plusieurs autres équipes et les équipes peuvent appartenir à plusieurs utilisateurs. Vous ne pouvez pas afficher cette relation dans un rapport à l’aide de l’interface Standard. Vous devez utiliser la création de rapports en mode texte pour afficher de nombreuses relations. </li> </ul>
  </td></tr>
<tr> 
   <td>[!UICONTROL Coût des risques restant]</td> 
   <td> <p>Champ de projet qui indique la différence entre le coût des risques planifiés d’un projet et le total de tous les risques [!UICONTROL Coûts réels] de tous les risques du projet. </p> <p>Le coût du risque restant d’un projet est calculé à l’aide de la formule suivante :</p> <p><code>[!UICONTROL Remaining Risk Cost] = Project [!UICONTROL Planned Risk Cost] - SUM([!UICONTROL Actual Cost] for all risks)</code> </p> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Replanning]</td> 
   <td>Modifier les dates d’un projet pour résoudre ou surmonter les problèmes. Par exemple, un projet qui est en attente depuis plusieurs mois doit être replanifié pour refléter des dates précises. Il s’agit d’une opération manuelle d’ajustement des dates du projet ou des tâches. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Report]</td> 
   <td>Un graphique ou un tableau contenant des informations sur un objet [!DNL Workfront] donné et ses attributs associés.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Request]</td> 
   <td> <p>Type de problème qui est trié dans une file d’attente centralisée unique et qui n’a aucun rapport avec un travail en cours.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL File d’attente des demandes]</td> 
   <td>Le journal des problèmes gérés par un processus de trafic et de triage.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Vitesse de la requête]</td> 
   <td>Durée totale du cycle de travail pour la prise en charge et la réalisation d’une demande.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Requester]</td> 
   <td>Généralement, un type de licence. Un utilisateur disposant d’une licence Requester peut soumettre des demandes de nouveau travail dans le système.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Durée réservée]</td> 
   <td>Jours spécifiés lors de l’heure personnelle d’un utilisateur, indiquant que l’utilisateur ne sera pas disponible pour le travail. Voir "[!UICONTROL Jours sans travail]".</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Résoudre un problème]</td> 
   <td> <p>Dans un rapport de problème, utilisez ce champ dans les vues ou les filtres pour faire référence au problème qui résout le problème. </p> <p>Pour plus d’informations sur l’affichage des objets de résolution dans les rapports, voir <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">Affichage des informations sur les objets résolvables et résolvables dans un rapport</a> dans <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Présentation de la résolution et de la résolution des objets résolvables </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Résoudre un projet]</td> 
   <td> <p>Dans un rapport de problème, utilisez ce champ dans les vues ou les filtres pour faire référence au projet qui résout le problème. </p> <p>Pour plus d’informations sur l’affichage des objets de résolution dans les rapports, voir <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">Affichage des informations sur les objets résolvables et résolvables dans un rapport</a> dans <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Présentation de la résolution et de la résolution des objets résolvables </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resolve Task]</td> 
   <td> <p>Dans un rapport de problème, utilisez ce champ dans les vues ou les filtres pour faire référence à la tâche qui résout le problème. </p> <p>Pour plus d’informations sur l’affichage des objets de résolution dans les rapports, voir <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">Affichage des informations sur les objets résolvables et résolvables dans un rapport</a> dans <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Présentation de la résolution et de la résolution des objets résolvables </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resource]</td> 
   <td>Utilisateurs ou rôles existant dans [!DNL Workfront] et affectés aux équipes de projet, aux tâches et aux problèmes. Il est chargé de terminer le travail associé aux projets, tâches ou problèmes. </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Resource Estimates</td> 
    <td>This report captures information about an area in&nbsp;Workfront that has been removed. The report might display legacy information but it does not update with current data. Although not recommended, you may update the information in this report using the API. For information about how you estimate resources for projects, see <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Resource Planner overview</a>. </td> 
   </tr>
   <td>Resource Grid</td> 
   <td>A visual table showing the allocation of resources.</td> 
  </tr> -->
  <tr> 
   <td>[!UICONTROL Resource Management]</td> 
   <td> <p>[!UICONTROL Resource Management] est un ensemble d’outils d’entreprise qui vous permet de prévoir précisément l’utilisation de vos ressources en fonction de leur disponibilité, de sorte que le travail à effectuer soit terminé à temps et selon le budget. </p> <p>Grâce aux outils de gestion des ressources, vous pouvez planifier des capacités à long terme et des besoins de planification à court terme pour vos ressources. </p> <p>Pour plus d’informations sur la gestion des ressources dans [!DNL Workfront], voir <a href="../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md">Prise en main de la gestion des ressources</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resource Manager IDs]</td> 
   <td><p>Dans un rapport de projet, vous pouvez utiliser cette option lors de la création d’un filtre pour trouver un gestionnaire de ressources spécifique. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Gestionnaire de ressources]</td> 
   <td> <p>En mode Liste ou rapport d’un projet, il s’agit d’un champ d’information qui affiche les utilisateurs désignés pour exécuter des activités de gestion des ressources sur le projet.  Lorsque vous utilisez "[!UICONTROL Gestionnaire de ressources]" dans un rapport, une liste de gestionnaires de ressources s’affiche, chaque gestionnaire de ressources figurant dans le projet étant séparé par une virgule. Vous pouvez désigner jusqu’à 30 gestionnaires de ressources pour un projet donné.</p> <p>Pour plus d’informations, reportez-vous à l’article <a href="../../../manage-work/projects/planning-a-project/designate-resource-managers-for-projects-and-templates.md">Désigner les gestionnaires de ressources pour un projet ou un modèle </a>.</p> </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Resource Planner Budget Hours] </td> 
   <td>Heures budgétées pour le projet et ressources qui lui sont associées dans le [!UICONTROL Resource Planner]. Voir aussi "[!UICONTROL Hours budgétés]" dans cet article. </td> 
  </tr>  
  <tr> 
   <td>[!UICONTROL Resource Planner] </td> 
   <td>Un outil [!DNL Workfront] avancé qui vous permet d’afficher et de gérer des ressources entre les projets, les rôles de tâche ou les utilisateurs. Pour plus d’informations, voir <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Présentation de Resource Planner</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resource Planner Budget Labor Cost]</td> 
   <td> <p>Il s’agit du coût associé aux heures budgétisées pour les rôles de tâche de projet à l’aide du planificateur de ressources. </p> <p>Voir aussi "Coût du travail budgété" dans cet article. </p> </td>

</tr> 
  <tr> 
   <td>[!UICONTROL Pools de ressources]</td> 
   <td> <p>Les groupes de ressources sont des groupes d’utilisateurs qui peuvent être associés à un projet. Les utilisateurs du même pool de ressources appartiennent généralement au même département, possèdent des compétences similaires ou complémentaires, ou sont financés par le même budget. Vous pouvez associer plusieurs groupes de ressources à un projet ou à un utilisateur. Un pool de ressources peut être attribué exclusivement à un projet ou partagé par plusieurs projets.</p> 
   <p>Pour plus d’informations sur les pools de ressources, voir <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref">Vue d’ensemble des pools de ressources</a>.</p> 
   <p>Dans les rapports de projet, les pools de ressources affichent tous les pools associés à un projet. Cet objet ne peut pas être utilisé dans un regroupement.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resource Utilization]</td> 
   <td>Rapport affichant le nombre d’heures disponibles pendant une certaine période et le nombre d’heures planifiées pour chaque utilisateur du rapport. Il est également calculé en [!UICONTROL Moyenne des heures par jour] et en pourcentage d’allocation.</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Result]</td> 
   <td>Dans [!DNL Workfront Goals], un résultat est un indicateur de progression pour un objectif. Il peut s’agir d’un nombre, d’une valeur de pourcentage ou d’un montant monétaire que vous mettez à jour manuellement. Vous ne pouvez pas afficher les résultats dans un rapport et vous ne pouvez pas y accéder via l’API [!DNL Workfront]. Pour plus d’informations sur les activités, voir <a href="../../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md" class="MCXref xref">Prise en main des résultats et des activités dans les objectifs Adobe Workfront</a>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Recettes]</td> 
   <td>Montant facturable pour la tâche ou le projet. Le montant peut être horaire, fixe ou une combinaison des deux.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Revenue Type]</td> 
   <td>Le type de recette détermine la manière dont la tâche va augmenter les recettes. Voici quelques exemples : [!UICONTROL Horaire fixe], [!UICONTROL Horaire du rôle et [!UICONTROL Horaire du rôle]. Pour plus d’informations sur le suivi des recettes dans [!DNL Workfront], voir <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Présentation de la facturation et des recettes</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Reviewer]</td> 
   <td>Généralement, un type de licence. Un utilisateur disposant d’une licence [!UICONTROL Reviewer] peut passer en revue et approuver des tâches dans le système.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Risque]</td> 
   <td> <p>Cela peut faire référence aux concepts suivants dans [!DNL Workfront] :</p> 
    <ul> 
     <li> <p>Champ d’un projet qui indique à quel point un projet peut être risqué. Vous pouvez hiérarchiser l’exécution de vos projets en fonction du niveau de risque. Les projets peuvent présenter les niveaux de risque suivants :</p> <p>- [!UICONTROL Très faible]</p> <p>- [!UICONTROL Low]</p> <p>- [!UICONTROL Medium]</p> <p>- [!UICONTROL Haut]</p> <p>- [!UICONTROL Très élevé]</p> <p>Les niveaux de risques que vous indiquez pour un projet ne peuvent pas être personnalisés. </p> <p> Pour plus d’informations sur la mise à jour du risque d’un projet, consultez la section "Paramètres du projet" de l’article <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Modifier les projets</a>. Vous pouvez afficher le champ des risques d’un projet dans les rapports. </p> </li> 
     <li> <p>Événement qui peut se produire pendant la durée d’un projet et qui identifie un impact potentiel sur le coût, la portée ou la planification du projet. Vous définissez les risques potentiels pour un projet et associez une probabilité qu’ils se produisent ou un coût au moment de la création de l’analyse de cas du projet. Pour plus d’informations sur l’ajout de risques à l’analyse de cas du projet, voir "Créer et modifier des risques sur les projets". </p> <p>Vous ne pouvez pas afficher les risques définis dans l’[!UICONTROL Business Case] dans les rapports. Vous ne pouvez afficher que plusieurs types de coûts de risque dans les rapports et les listes. </p> </li> 
    </ul> </td>

</tr> 
  <tr data-mc-conditions=""> 
   <td>Coût des risques [!UICONTROL]</td> 
   <td> <p>Le coût associé aux risques sur un projet. Vous trouverez ci-dessous les coûts de risque associés aux projets que vous pouvez afficher dans les rapports :</p> 
    <ul> 
     <li> <p>[!UICONTROL Coût réel] : champ sur un risque qui indique le coût réel du risque qui s’est produit. Outre les rapports et les listes, vous pouvez les localiser dans la zone [!UICONTROL Modifier le risque] lors de la modification ou de la création d’un risque. </p> <p>Pour les coûts de projet, de tâche ou d’émission, voir "[!UICONTROL Coût réel]" dans cet article. </p> </li> 
     <li> <p>[!UICONTROL Coût des risques planifiés] : champ du projet qui indique le total des [!UICONTROL Coûts des risques potentiels] pour le projet. Voir aussi "[!UICONTROL Coût des risques planifiés]" dans cet article. </p> <p>Pour plus d’informations sur le coût potentiel de risque, voir <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">Calculer le coût potentiel de risque </a>. </p> </li> 
     <li> <p>[!UICONTROL Coût du risque restant] : champ du projet qui affiche la différence entre le total des [!UICONTROL Coûts réels] de tous les risques et le coût du risque planifié [!UICONTROL]. Voir aussi "Coût du risque restant" dans cet article. </p> </li>
    </ul> </td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL Gestion des risques]</td> 
   <td>Processus permettant d’identifier, d’atténuer et de surveiller les risques.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Role]</td> 
   <td>Voir "[!UICONTROL Job Role]" dans cet article.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Routage]</td> 
   <td>Affectation ou déplacement automatique d’un problème, généralement en raison d’une rubrique de file d’attente ou au moyen de l’option Itinéraire par défaut (règle de routage) pour la file d’attente.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Routage Rule]</td> 
   <td>Paramètre sur les projets et les rubriques de la file d’attente qui attribue automatiquement un problème à un utilisateur, un rôle ou une équipe, ou qui déplace le problème vers un autre projet ou une rubrique de file d’attente. Les règles de routage sont généralement utilisées avec les files d’attente de demande d’aide pour affecter automatiquement les problèmes entrants.</td> 
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
   <td>[!UICONTROL Recherche enregistrée]</td> 
   <td>Recherche pour laquelle les critères de recherche ont été enregistrés. Les recherches enregistrées facilitent l’exécution des mêmes sans devoir à nouveau entrer les critères de recherche.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Scénario] (dans [!DNL Workfront Fusion]) </td> 
   <td> <p>Un scénario se compose d’une série d’étapes (modules) qui indiquent comment les données doivent être transférées et transformées entre les applications/services.</p> <p>Pour plus d’informations sur les scénarios dans [!DNL Workfront Fusion], voir <a href="../../../workfront-fusion/scenarios/scenario-overview.md" class="MCXref xref">[!DNL Adobe Workfront Fusion] présentation des scénarios</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Scénario] (dans [!DNL Workfront Scenario Planner]) </td> 
   <td> <p>Dans le [!DNL Scenario Planner], un scénario est une copie d’un plan. </p> <p>[!DNL Scenario Planner] nécessite une licence supplémentaire. Pour plus d'informations sur [!DNL Workfront Scenario Planner], consultez la <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">présentation [!DNL Scenario Planner]</a>. </p> <p>Pour plus d’informations sur la création de scénarios, voir <a href="../../../scenario-planner/create-and-compare-scenarios-for-a-plan.md">Création et comparaison de scénarios de plan dans [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planning]</td> 
   <td>Le planning de travail hebdomadaire, y compris les horaires de travail, combiné avec les jours de congé (par exemple les jours fériés) et les jours d’exception (par exemple, un jour de travail du samedi). Vous pouvez associer des planifications à des projets et des utilisateurs.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Exception de planification]</td> 
   <td>Connu également sous le nom de Maj modifiée . Jours planifiés par opposition aux heures de travail hebdomadaires régulières définies par le planning. Par exemple, un samedi programmé pour fonctionner, lorsque la planification est configurée pour travailler uniquement du lundi au vendredi, serait une [!UICONTROL exemption de planification].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Rapport planifié]</td> 
   <td> <p>Lorsque vous créez un rapport de rapports, vous pouvez afficher des informations sur les plannings du rapport, si la remise du rapport est planifiée à l’aide du champ [!UICONTROL Rapport planifié] . Ce champ affiche plusieurs valeurs, une pour chaque planning de chaque rapport, dans une liste à puces. Pour plus d’informations sur la planification des rapports, consultez l’article <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md" class="MCXref xref">Présentation de la remise de rapports</a>.</p> <p>Comme ce champ affiche plusieurs valeurs, il ne peut pas être utilisé dans un groupement. Vous ne pouvez y accéder que dans un filtre ou une vue. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Modification de la portée]</td> 
   <td>Un [!UICONTROL Journal d’audit] qui, s’il est actif, génère une note chaque fois qu’une modification est apportée à la portée d’un projet ou d’une tâche, par exemple si une [!UICONTROL Durée de la tâche] ou les [!UICONTROL Prédécesseurs] sont modifiés.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Section]</td> 
   <td>Zone de l’écran, avec son propre en-tête, créée pour organiser les données personnalisées à des fins d’affichage.</td> 
  </tr> 
  <tr> 
   <td>Saut de section [!UICONTROL]</td> 
   <td>Un espace ou une bordure entre les sections.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Security]</td> 
   <td>Paramètres permettant à un utilisateur d’interagir avec certains objets du système et non avec d’autres. Voir aussi "[!UICONTROL Niveaux d’accès]" dans cet article.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Configuration]</td> 
   <td>Zone dans laquelle les administrateurs peuvent configurer les configurations et les préférences du système.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Severity]</td> 
   <td> <p>[!UICONTROL Severity] indique la probabilité qu’un élément ait un impact sur l’achèvement du travail. Par exemple, un problème de [!UICONTROL Gravité] élevée peut complètement bloquer l’achèvement d’une tâche, mais un problème de [!UICONTROL Gravité] faible peut être purement cosmétique.</p> <p>Pour plus d’informations, voir <a href="../../../manage-work/issues/issue-information/update-issue-severity.md" class="MCXref xref"> Mise à jour de la gravité des problèmes </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Severties]</td> 
   <td>Voir "[!UICONTROL Severity]" dans cet article.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sharing]</td> 
   <td>Action permettant à d’autres utilisateurs d’afficher ou de modifier un élément spécifique dans [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Date du Slack]</td> 
   <td>Dans une vue de tâche ou un rapport, la [!UICONTROL Date du Slack] affiche la date exacte à laquelle une tâche peut avoir un impact certain sur la [!UICONTROL Date d’achèvement] du projet. Pour plus d’informations sur la [!UICONTROL Date du Slack] d’une tâche, voir <a href="../../../manage-work/tasks/task-information/task-slack-date.md" class="MCXref xref">Présentation de la date du Slack de tâches</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Affectations intelligentes]</td> 
   <td> <p>Lors de l’affectation de tâches ou de problèmes aux utilisateurs, [!DNL Workfront] émet des recommandations ([!UICONTROL Smart Assignments]) sur les utilisateurs qui sont les mieux placés pour terminer le travail, en fonction du temps dont ils disposent pour le terminer et de leur relation avec le projet.</p> <p>Pour plus d’informations, voir <a href="../../../manage-work/tasks/assign-tasks/smart-assignments.md" class="MCXref xref">Présentation des affectations dynamiques</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source]</td> 
   <td> <p>Indique l’objet parent d’un autre objet. Par exemple, un document joint à une tâche porte le nom de la tâche dans le champ [!UICONTROL Source] d’un rapport ou d’une vue [!UICONTROL Document] ; un problème consigné sous un projet porte le nom du projet dans le champ [!UICONTROL Source] d’un rapport ou d’une vue Problème. </p> 
   <p>Les rapports suivants affichent une colonne Source dans laquelle vous pouvez afficher des informations sur l’objet parent :</p>
  <ul><li>Rapports sur les problèmes</li>
    <li>Rapports d’heure</li>
    <li>Rapports sur les documents </li>
    </ul>
   <p>Si les utilisateurs ne disposent pas d’autorisations sur l’objet parent d’un problème, d’une heure ou d’un document, la colonne Source du rapport s’affiche vide, même lorsque le rapport est configuré pour s’afficher ou pour être diffusé avec les droits d’accès d’un autre utilisateur. </p>
   <p> Pour afficher des informations sur l’objet parent dans le rapport, il est recommandé d’ajouter une colonne pour l’objet parent dans laquelle vous pouvez afficher le nom du parent. </p>
    <p>Par exemple, vous pouvez ajouter l’un des éléments suivants à un rapport avec une colonne Source : </p>
    <ul><li>Les colonnes Nom du projet, Nom de la tâche ou Nom de la publication dans un document ou un rapport d’heure.</li>
    <li>Colonnes Nom du projet ou Nom de la tâche pour un rapport de problème. </li> </ul>
    Pour plus d'informations, voir <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md">Exécution et diffusion d'un rapport avec les droits d'accès d'un autre utilisateur</a>

</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Date de début]</td> 
   <td> <p>Date à laquelle le travail sur un élément est défini pour commencer. Il existe plusieurs dates de début dans [!DNL Workfront] : </p> 
    <ul> 
     <li>[!UICONTROL Planifié]</li> 
     <li>[!UICONTROL Réel]</li> 
     <li>[!UICONTROL Projeté] </li> 
    </ul> <p>Dans un rapport [!UICONTROL Rate], il s’agit de la date à laquelle commence un nouveau taux de facturation pour un rôle de tâche au niveau du projet. Les heures associées au projet qui se trouvent après cette date sont multipliées par ce taux de facturation pour calculer les recettes sur le projet. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Status]</td> 
   <td> <p>Indicateur utilisé pour signaler la position d’un workflow d’une tâche ou d’un objectif stratégique.</p> <p>Pour les projets, le paramètre [!UICONTROL Status] est un paramètre du projet qui indique si le projet est :</p> 
    <ul> 
     <li>[!UICONTROL Actuel]</li> 
     <li>[!UICONTROL En attente] </li> 
     <li>[!UICONTROL Terminé] </li> 
     <li>[!UICONTROL Morts]</li> 
    </ul> <p>Pour plus d’informations sur l’état d’un projet, voir <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md">Accès à la liste des états du projet système</a>.</p>
    <p>Pour les tâches, le [!UICONTROL Status] est un paramètre de la tâche qui indique si la tâche est :</p> 
    <ul> 
     <li>[!UICONTROL Nouveau]</li> 
     <li>[!UICONTROL En Cours]</li> 
     <li>[!UICONTROL Terminé]</li> 
    </ul> <p>Pour plus d’informations sur l’état de la tâche, voir <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md">Accès à la liste des états des tâches système</a></p> <p>Pour les problèmes, le paramètre [!UICONTROL Status] est un paramètre qui indique si le problème est :</p> 
    <ul> 
     <li>[!UICONTROL Nouveau]</li> 
     <li>[!UICONTROL En Cours]</li> 
     <li>[!UICONTROL En attente de commentaires]</li> 
     <li>[!UICONTROL En attente]</li> 
     <li>[!UICONTROL Résolu]</li> 
     <li>[!UICONTROL ne résoudra pas]</li> 
     <li>[!UICONTROL Impossible De Dupliquer]</li> 
     <li>[!UICONTROL Vérifié terminé]</li> 
     <li>[!UICONTROL rouvert]</li> 
    </ul> <p>Pour plus d’informations sur les états de problème, voir <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">Accès à la liste des états de problème système</a>.</p> 
    <p>Pour les objectifs stratégiques, le [!UICONTROL Status] est un paramètre de l’objectif qui indique si l’objectif est :</p> 
     <ul> 
      <li>[!UICONTROL Active]</li> 
      <li>[!UICONTROL Draft]</li> 
      <li>[!UICONTROL Inactif]</li> 
      <li>[!UICONTROL Fermé]</li> 
     </ul> 
     <p>Pour plus d’informations sur les objectifs stratégiques, voir aussi "[!UICONTROL Objectif]" ou "[!UICONTROL Objectifs]" dans cet article. </p> 
     <p>Pour les objectifs stratégiques, ce champ n’est visible que si votre organisation a acheté [!DNL Workfront Goals]. Pour plus d'informations sur la gestion des objectifs stratégiques à l'aide de [!DNL Workfront Goals], voir <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] - Aperçu</a>. </p>
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Changement d’état]</td> 
   <td>Un [!UICONTROL Journal D’Audit]. Une note est générée lorsqu’un utilisateur modifie l’état du projet, de la tâche ou du problème.</td> 
  </tr> 
  <tr> 
   <td>Icônes de statut</td> 
   <td> <p>Vous pouvez ajouter le champ intégré [!UICONTROL Icônes d’état] en tant que colonne dans vos vues afin d’améliorer la visibilité sur les points clés de vos objets, tels que :</p> 
    <ul> 
     <li>Un objet est associé à des documents</li> 
     <li>Un objet est associé à un processus de validation</li> 
     <li>Un objet est associé à des remarques supplémentaires.</li> 
     <li>Une dépense est facturable ou remboursable </li> 
     <li>Une tâche est sur un chemin critique</li> 
     <li>Un utilisateur appartient à une entreprise, à une équipe ou se trouve dans un fuseau horaire différent. </li> 
    </ul> <p>Vous pouvez ajouter le champ [!UICONTROL Icônes d’état] dans les vues des objets suivants : </p> 
    <ul> 
     <li>[!UICONTROL Tasks]</li> 
     <li>[!UICONTROL Issues]</li> 
     <li>[!UICONTROL Projects]</li> 
     <li>[!UICONTROL Tâches Du Modèle]</li> 
     <li>[!UICONTROL Modèles]</li> 
     <li>[!UICONTROL Dépenses]</li> 
     <li>[!UICONTROL Documents]</li> 
     <li>[!UICONTROL Users]</li> 
    </ul> <p>Pour plus d’informations, voir <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">Icônes d’état intégrées dans les vues</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Status Update]</td> 
   <td> <p>Dans un rapport de projet, de tâche ou de problème, ce champ affiche la mise à jour d’état la plus récente fournie par les propriétaires d’objets dans la zone '[!UICONTROL Updates]'. Pour les projets, cela signifie que les commentaires effectués par le propriétaire du projet, ainsi que pour les tâches et les problèmes, cela signifie que les commentaires effectués par les personnes désignées.</p> 
   <p> Les commentaires effectués lors de la mise à jour de l’état d’un objet ne s’affichent pas dans la colonne [!UICONTROL Status Update] .</p> <p>Pour afficher les états '[!UICONTROL Nouveau], '[!UICONTROL En cours]' et '[!UICONTROL Terminé]', utilisez la colonne [!UICONTROL Statut].</p> <p>Pour plus d’informations sur les états, consultez l’article <a href="../../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref">Mise à jour de l’état de la tâche</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL États]</td> 
   <td>Voir "[!UICONTROL Status]" dans cet article.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Storyboard]</td> 
   <td>Un graphique qui représente l’état des histoires (tâches dans la méthodologie agile) et leur progression vers l’achèvement.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Heures d’article]</td> 
   <td>Mesure utilisée pour mesurer la difficulté ou la complexité d’un article. Les équipes agiles peuvent choisir d’utiliser les heures ou les points.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Story Points]</td> 
   <td>Mesure utilisée pour mesurer la difficulté ou la complexité d’un article. Les équipes agiles peuvent choisir d’utiliser les heures ou les points.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Strategic]</td> 
   <td>Travail à long terme qui modifie l’organisation ou le fonctionnement de l’organisation.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Alignement stratégique]</td> 
   <td>Mesure et alignement des objectifs de l’entreprise entre les portefeuilles et les programmes.</td> 
  </tr>

<tr> 
   <td><code>[!UICONTROL stretch]</code></td> 
   <td><p>Elle est utilisée dans les colonnes du rapport lors de l’utilisation de l’interface Mode texte. </p>
   <p>Le <code>[!UICONTROL stretch]</code> est utilisé pour identifier les colonnes qui occupent un espace supplémentaire non nécessaire à la vue. La largeur de l’interface utilisateur de l’espace de travail d’un utilisateur type est d’environ 850 pixels. Cela signifie que si vous disposez d’une vue avec quatre
   des colonnes (150 pixels chacune) que votre vue occupe 600 sur 850 pixels. L’interface utilisateur contient 250 pixels supplémentaires qui seront ajoutés aux colonnes pour lesquelles un pourcentage d’étirement est fourni. </p>
   <p>L'étirement d'une colonne est appliqué lorsque vous utilisez la ligne de code supplémentaire : <code>[!UICONTROL usewidths=true]</code> pour au moins une des colonnes de la vue. 
   </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Abonnés]</td> 
   <td> <p>Utilisateurs qui s’abonnent à des projets, des tâches ou des problèmes.</p> <p>Lorsque vous utilisez ce champ dans un rapport, une liste d'abonnés s'affiche, chaque abonné étant séparé par une virgule.</p> <p>Pour plus d’informations, voir l’article <a href="../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md" class="MCXref xref">Abonner aux éléments dans [!DNL Adobe Workfront]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tâche Résumé]</td> 
   <td>Voir "[!UICONTROL Tâche parente]" dans cet article.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Subtask]</td> 
   <td>Une tâche enfant, située sous une tâche parent.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Gouvernance du système]</td> 
   <td>Ensemble de stratégies qui régit les modifications et la maintenance d’un système.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Intégration du système]</td> 
   <td>Processus consistant à relier différents systèmes informatiques et applications logicielles, physiquement ou fonctionnellement, afin d’agir comme un tout coordonné.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Task]</td> 
   <td> <p>Une activité qui doit être effectuée comme une étape vers l’atteinte d’un objectif final (achèvement du projet).</p> <p>Pour plus d’informations, voir <a href="../../../manage-work/tasks/task-information/tasks-overview.md" class="MCXref xref">Présentation des tâches</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Task Attribute]</td> 
   <td>Autres champs ou objets associés à une tâche et indiquant certains détails sur la tâche. Voici quelques exemples : [!UICONTROL Date d’achèvement prévue] et [!UICONTROL État].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Contrainte de tâche]</td> 
   <td>Voir "[!UICONTROL Constraint Type]" et "[!UICONTROL Constraint Date]".</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Gestion des tâches]</td> 
   <td>Ensemble de stratégies qui détermine les seuils pour la création, l’affectation, la fermeture et la visibilité des tâches.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Propriétaire de la tâche]</td> 
   <td>L’équipe ou l’utilisateur responsable de l’estimation de l’effort et de l’achèvement de la tâche</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Team]</td> 
   <td> <p>Ensemble d’utilisateurs travaillant à des objectifs ou des objectifs commerciaux similaires. Ces utilisateurs peuvent être affectés collectivement à une tâche en affectant l’équipe à l’élément de travail.</p> <p>Pour plus d’informations sur les équipes, consultez la <a href="../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md" class="MCXref xref">présentation des équipes</a>.</p> <p>Les projets peuvent avoir une [!UICONTROL Équipe de projet], qui contient tous les utilisateurs ou rôles associés au travail sur le projet.</p> <p>Pour plus d’informations sur les équipes de projet, consultez la <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">présentation de l’équipe de projet</a></p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode,SnippetConitions_MaturityModel.Ad hoc"> 
    <td>Team Goals</td> 
    <td>Team goals which contribute to the metrics of enterprise or department goals.</td> 
   </tr>
  --> 
  <tr> 
   <td>[!UICONTROL Template]</td> 
   <td> <p>Les modèles de projet sont des compositions génériques de vos projets les plus répétables. Vous pouvez définir des tâches, des rubriques de file d’attente, des formulaires personnalisés, joindre des documents ou des validations lorsque vous créez un modèle de projet, ce qui vous permet de gagner du temps lorsque vous devez créer un nouveau projet. </p> <p>Vous pouvez joindre des modèles à des projets existants ou les utiliser pour créer des projets. Toutes les informations spécifiées sur le modèle sont transférées vers les projets créés à l’aide de celui-ci. </p> <p>Pour plus d’informations sur les modèles, consultez la <a href="../../../manage-work/projects/create-and-manage-templates/project-template-overview.md">présentation du modèle de projet</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tâche Modèle]</td> 
   <td>Tâche qui fait partie d’un modèle. Les tâches du modèle deviennent des tâches dans le projet créé à l’aide du modèle.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Thread]</td> 
   <td>Une [!UICONTROL Remarque] et son ensemble de réponses liées à un sujet particulier.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Miniature]</td> 
   <td> <p> Dans une liste ou un rapport [!UICONTROL Document], un aperçu du document s’affiche dans une miniature. </p> <p> Sélectionnez <strong>[!UICONTROL Miniature]</strong>  pour afficher une miniature de 33 à 66 pixels de large dans le rapport. </p> <p>La taille de la miniature s’ajuste lorsque vous modifiez la largeur de la colonne dans une liste ou un rapport.</p> <p>Voir aussi "[!UICONTROL Grande miniature]" dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Time Off]</td> 
   <td>Vous pouvez créer un rapport [!UICONTROL Heure de désactivation] afin d’afficher le moment où les utilisateurs ont indiqué une heure de désactivation dans leur profil. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Frise chronologique]</td> 
   <td> <p>Frise chronologique qui permet aux utilisateurs de saisir les heures réelles qu’ils ont passées à travailler sur des projets, des tâches ou des problèmes, ou les heures qu’ils ont passées pour d’autres activités non liées au travail, comme des réunions ou des formations. Outre le temps que vous avez passé à travailler, vous pouvez également indiquer si le temps est lié au travail ou s’il s’agit d’un temps de surcharge en utilisant les types d’heure pour définir vos entrées d’heure. Pour plus d’informations sur les feuilles de temps, consultez la <a href="../../../timesheets/timesheets/timesheets-overview.md">présentation des feuilles de temps</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Profil de la feuille de calcul]</td> 
   <td> <p>Un [!UICONTROL Timesheet Profile] est un modèle que [!DNL Workfront] utilise pour créer automatiquement des feuilles de temps pour les utilisateurs qui y sont associés. </p> <p>Vous pouvez configurer plusieurs paramètres qui s’appliqueront à chaque feuille de temps au fur et à mesure de sa création. Certains de ces paramètres sont les suivants : la fréquence de création de la feuille de temps (hebdomadaire, toutes les deux semaines, deux fois par mois ou mensuelle), le jour de début de la feuille de temps, les approbateurs de la feuille de temps, les [!UICONTROL Types d’heure] disponibles que les utilisateurs peuvent associer aux heures enregistrées.</p> </td> 
  </tr> 
  <tr > 
   <td>[!UICONTROL Top Parent ID] </td> 
   <td> <p>Ce champ vous permet d’identifier et de filtrer les données d’un groupe de niveau supérieur et de ses sous-groupes dans une liste ou un rapport.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Top Parent Name] </td> 
   <td> <p>Ce champ vous permet d’identifier les données relatives à un groupe de niveau supérieur et à ses sous-groupes dans une [!UICONTROL View] pour une liste ou un rapport.</p> <p>Vous pouvez également le faire à l’aide du champ [!UICONTROL Top Parent ID] .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Total des heures]</td> 
   <td> <p>Dans un [!UICONTROL rapport de projet], ce champ affiche la somme arrondie de toutes les heures du projet, la dernière fois que le financement du projet a été calculé. [!UICONTROL Heures réelles] reflètent les heures exactes connectées au projet. En règle générale, les [!UICONTROL Heures réelles] doivent correspondre au [!UICONTROL Total heures]. Si le champ [!UICONTROL Total heures] apparaît sensiblement différent du champ [!UICONTROL Heures réelles], vous devez recalculer les finances sur le projet.</p> <p>Pour plus d’informations sur le nouveau calcul des finances de projet, consultez l’article <a href="../../../manage-work/projects/project-finances/recalculate-project-finances.md" class="MCXref xref">Recalculer les finances de projet</a>.</p> <p>Dans une vue [!UICONTROL Standard] de feuille de temps, ce champ fait référence au nombre total d’heures consignées pour les éléments pour les dates affichées sur une feuille de temps. Le champ [!UICONTROL Total heures] pour les feuilles de temps dans cette vue intégrée fait référence au champ "[!UICONTROL hoursDuration]" qui calcule dynamiquement la différence en heures entre les dates de début et de fin de la feuille de temps. Elle est utilisée pour afficher la colonne [!UICONTROL Total heures] en rouge si l’utilisateur se connecte plus de temps que les heures disponibles dans la période de la feuille de temps. Pour plus d’informations, voir <a href="../../../timesheets/create-and-manage-timesheets/view-total-hours-timesheets.md" class="MCXref xref">Affichage du nombre total d’heures sur la feuille de temps</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Mode de suivi]</td> 
   <td> <p>Attribut d’une tâche. Cela détermine comment et à quel moment les chronologies projetées seront mises à jour pour une tâche. Par exemple :</p> 
    <ul> 
     <li>[!UICONTROL L L’utilisateur doit mettre à jour] nécessite qu’une tâche soit mise à jour manuellement. Sinon, il deviendra [!UICONTROL Derrière le calendrier], puis [!UICONTROL En retard].</li> 
     <li>[!UICONTROL Auto Complete] termine automatiquement une tâche lorsque la date d’échéance, ou [!UICONTROL Date d’achèvement planifiée], est dépassée.</li> 
    </ul> <p>Pour plus d’informations, voir <a href="../../../manage-work/tasks/task-information/task-tracking-mode.md" class="MCXref xref">Présentation du mode de suivi des tâches</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Trigger]</td> 
   <td>Événement qui démarre un scénario.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Trouble Task]</td> 
   <td>Une tâche incomplète avec une condition [!UICONTROL en retard], [!UICONTROL derrière le planning] ou [!UICONTROL en danger].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tâche non assignée]</td> 
   <td>Tâche qui n’est affectée à aucun utilisateur, rôle ou équipe.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Update Type]</td> 
   <td> <p>Paramètre d’un projet qui détermine le moment où la chronologie calculée du projet sera recalculée. Le [!UICONTROL Update Type] peut avoir les valeurs suivantes :</p> 
    <ul> 
     <li>[!UICONTROL Automatique et En modification]</li> 
     <li>[!UICONTROL Automatique Uniquement]</li> 
     <li>[!UICONTROL Manuel Uniquement] </li> 
    </ul> <p>Pour plus d’informations, voir <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Sélectionner le type de mise à jour de projet </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL User]</td> 
   <td>Un compte créé dans [!DNL Workfront] pour permettre à une personne de se connecter et d’interagir avec le système.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL Délégation D’Utilisateurs]</p> </td> 
   <td> <p>Un objet à déclarer qui vous indique :</p> 
    <ul> 
     <li>Les utilisateurs qui ont délégué la tâche, l’émission et les approbations de projet</li> 
     <li>Les utilisateurs auxquels ont été déléguées la tâche, l’émission et les approbations de projet</li> 
     <li>Lorsque ces délégations commencent et se terminent</li> 
    </ul> <p>Pour en savoir plus, voir <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-user-delegation-report.md" class="MCXref xref">Création d’un rapport de délégation d’utilisateur</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Interface Utilisateur]</td> 
   <td>Tous les aspects visuels et interactifs de l’application [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL User Interface Preferences]</td> 
   <td>[!UICONTROL Configuration de l’interface utilisateur]. Les administrateurs de [!DNL Workfront] peuvent modifier ces paramètres pour personnaliser certains aspects de l’interface utilisateur.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Utilisation]</td> 
   <td>Disponibilité d’un utilisateur ou d’un rôle en fonction du planning affecté, du PTO et de la charge de travail actuelle.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Utilisation des utilisateurs]</td> 
   <td> <p>Recherche combinée à un rapport qui indique comment les utilisateurs (ressources) sont affectés ou surattribués. Voir "[!UICONTROL Resource Utilization]" dans cet article.</p> </td> 
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
   <td>Mesure du temps total du cycle de travail (le temps nécessaire pour terminer un travail) et de la fréquence du travail dans le temps initialement engagé (ratio travail-validation).</td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL View]</td> 
   <td> <p>Les vues se rapportent à un élément de reporting qui permet de modifier les colonnes d'un rapport ou d'une liste d'objets.</p> 
   <p> La vue fait également référence au droit d’un utilisateur à afficher uniquement les informations sur un objet, en fonction de son niveau d’accès ou à un niveau de partage d’autorisations sur cet objet.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Icônes de vue]</td> 
   <td> <p> Il s’agit du même champ que les icônes d’état, mais il n’est disponible que pour les vues suivantes : </p> 
    <ul> 
     <li> [!UICONTROL Documents] </li> 
    </ul> <p> Pour plus d’informations, voir l’article <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">Icônes d’état intégrées dans les vues</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Vues le mois dernier]</td> 
   <td> <p>Dans une liste de rapports, il affiche le nombre de fois où le rapport a été affiché au cours du dernier mois.<br>Pour plus d’informations sur l’utilisation dans les listes de rapports, reportez-vous à l’article <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Afficher l’utilisation des rapports</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Vues au dernier trimestre]</td> 
   <td>Dans une liste de rapports, il affiche le nombre de fois où le rapport a été affiché au cours du dernier trimestre.<br>Pour plus d’informations sur l’utilisation dans les listes de rapports, reportez-vous à l’article <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" >Afficher l’utilisation des rapports</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Vues L’Année Dernière]</td> 
   <td>Dans une liste de rapports, il affiche le nombre de fois où le rapport a été consulté l’année dernière.<br>Pour plus d’informations sur l’utilisation dans les listes de rapports, reportez-vous à l’article <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Afficher l’utilisation des rapports</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Vues Ce Mois]</td> 
   <td> <p>Dans une liste de rapports, il affiche le nombre de fois où le rapport a été consulté au cours de ce mois.<br>Pour plus d’informations sur l’utilisation dans les listes de rapports, reportez-vous à l’article <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Afficher l’utilisation des rapports</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Affiche Ce Trimestre]</td> 
   <td>Dans une liste de rapports, il affiche le nombre de fois où le rapport a été affiché au cours de ce trimestre.<br>Pour plus d’informations sur l’utilisation dans les listes de rapports, reportez-vous à l’article <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Afficher l’utilisation des rapports</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Vues Cette Année]</td> 
   <td>Dans une liste de rapports, il affiche le nombre de fois où le rapport a été consulté au cours de cette année.<br>Pour plus d’informations sur l’utilisation dans les listes de rapports, reportez-vous à l’article <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md">Afficher l’utilisation des rapports</a>.</td> 
  </tr>

<tr>
  <td> <code>[!UICONTROL width]</code>
  </td>
<td> Dans un rapport, lors de l’utilisation de l’interface [!UICONTROL Mode Texte], ligne de code dans laquelle vous pouvez spécifier la largeur de chaque colonne en pixels. Workfront fournit une largeur suggérée pour chaque champ,
mais selon le type de champ et le format, vous pouvez effectuer des ajustements.
Vous devez utiliser la ligne de code <code>[!UICONTROL usewidths=true]</code> supplémentaire pour appliquer la largeur spécifiée pour la colonne. 
  </td>

</tr>

<tr> 
   <td><code>[!UICONTROL work]</code> </td> 
   <td> <p>Dans un rapport de projet, de tâche ou de problème, l’instruction suivante en mode texte affiche les heures planifiées du projet, de la tâche ou du problème :</p>
   <code><p>valuefield=work</p>
   <p>valueformat=HTML</p></code> 
   <p>Pour plus d’informations sur l’utilisation du mode texte, voir <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">Présentation de la syntaxe du mode texte</a>. </p> 
   <p><b>CONSEIL</b> 
   <p>Dans un rapport de problème, l’ajout de l’un des champs [!UICONTROL Heures planifiées] ajoute le champ <code>work </code> au rapport. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work]</td> 
   <td> <p>L’un des deux principaux types de licence. Celui-ci dispose d’un accès inférieur à [!UICONTROL Plan], mais il peut créer et mettre à jour le système. Un utilisateur disposant d’une licence de travail possède plus de fonctionnalités qu’un détenteur de licence [!UICONTROL externe], [!UICONTROL Reviewer] ou [!UICONTROL Requester].</p> <p>Pour plus d’informations, voir <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] - Présentation des licences</a>.</p> <p>Le travail peut faire référence au nombre d’[!UICONTROL Heures planifiées] pour un projet, une tâche ou un problème. Pour plus d’informations, voir le champ "[!UICONTROL work]" de ce tableau. </p> <p><b>CONSEIL</b></p> <p> Dans un rapport de problème, l’ajout de l’un des champs [!UICONTROL Heures planifiées] ajoute le champ <code>work </code> au rapport. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Structure de ventilation de travail]</td> 
   <td>Structure hiérarchique des tâches à exécuter par l’équipe de projet en fonction de la relation parent/enfant.</td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL Effort de travail] </td> 
   <td> 
    <p>Un chef de projet peut décider d’utiliser ce champ au lieu de [!UICONTROL Heures planifiées] pour estimer l’effort nécessaire pour terminer une tâche. Ce champ n’est visible que lorsque les conditions suivantes sont remplies :</p> 
     <ul> 
      <li> <p>La tâche a un [!UICONTROL Simple Duration Type]. </p> <p><b>CONSEIL</b></p> <p> Si vous mettez à jour la tâche [!UICONTROL Duration Type] vers un autre type, ce champ devient masqué. </p> </li> 
      <li>Le chef de projet a activé le champ [!UICONTROL Utiliser l’effort de travail] pour calculer automatiquement la tâche [!UICONTROL Heures planifiées] sur le projet. </li> 
     </ul> 
     <p>Pour plus d’informations sur l’utilisation de [!UICONTROL Effort de travail] au lieu de [!UICONTROL Heures planifiées] pour estimer l’effort de tâche, consultez la <a href="../../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">présentation de l’effort de travail</a>. </p> 
     <p>Vous pouvez afficher ce champ dans les listes et rapports de tâches.</p> 
    </td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL Élément de travail]</td> 
   <td> <p>Ce champ fait référence aux tâches ou aux problèmes de [!DNL Workfront]. </p> <p>Le rapport [!UICONTROL Élément de travail] affiche des informations sur les tâches et les problèmes. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Combinaison de gestion de travail]</td> 
   <td>Un [!UICONTROL Indicateur de performance professionnelle] (WPI) de la proportion de travail allouée à l’exécution de votre entreprise par rapport au changement de votre entreprise. L’interface utilisateur multisite vous aide à comprendre, au niveau de l’organisation, si une affectation réelle du travail est appliquée à votre stratégie.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work Management Resource]</td> 
   <td>Désignation d’une personne dans le système qui peut recevoir du travail ou suivre le temps.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Rôle et responsabilités de gestion du travail]</td> 
   <td>Définir les propriétaires et les parties prenantes pour gérer la portée, l’exécution et les approbations du problème, de la tâche, du projet, du programme ou du portefeuille désigné.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL SLA de gestion du travail]</td> 
   <td>Mesure quantifiable acceptée par toutes les parties prenantes.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Parties prenantes à la gestion du travail]</td> 
   <td>Collection d’utilisateurs ayant un intérêt particulier dans les résultats d’une demande de travail.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Points de contact de la gestion du travail]</td> 
   <td>Enregistrements numérisés de la communication entre les parties prenantes.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Indicateurs de performances de travail] </td> 
   <td> <p>Taux de mélange, capacité, vitesse, qualité et engagement.</p> <p>WPI est un acronyme courant pour [!UICONTROL Indicateur de performance professionnelle].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Workflow]</td> 
   <td> <p>Méthode de réception, de hiérarchisation et d’exécution des travaux. La manière dont vous exécutez le travail est généralement appelée "workflow" ou "plan de projet" (une liste de tâches avec des dates, des relations de prédécesseur, etc.). </p> <p>Par exemple, un processus de travail peut être la production d’une seule ressource ou la diffusion d’une campagne multiressource. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Modèle de workflow]</td> 
   <td>Dans le rapport [!UICONTROL Validation des BAT], ce champ affiche tous les modèles de workflow associés à un BAT. Si aucun modèle n’est joint, la colonne est vide.</td> 
  </tr>

<tr> 
   <td>[!UICONTROL Work Time]</td> 
   <td>

<p>Représente le pourcentage du temps équivalent à temps complet ([!UICONTROL FTE]) disponible pour le travail réel de l’utilisateur, sans compter les frais généraux. [!UICONTROL Work Time] doit être un nombre décimal maximum de 1 et ne peut pas être égal à 0. Par exemple, une disponibilité de 20 % pour le travail effectif serait de 0,2.</p>
   </p>La valeur par défaut du champ est 1, ce qui indique qu’un utilisateur passe l’intégralité de son [!UICONTROL FTE] au travail réel lié au projet.  </p>
   <p>Le système utilise ce nombre pour calculer la disponibilité de la personne quant au travail réel lié au projet. </p>
   <p> Les exceptions au planning et les congés peuvent également affecter la capacité de la personne. </p>
   <p>Pour plus d’informations sur la création de plannings dans Workfront, voir <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md">Créer un planning</a>. </p>
    <p>Workfront calcule la disponibilité d’un utilisateur en fonction des préférences de gestion des ressources dans la zone [!UICONTROL Configuration]. Pour plus d’informations, voir <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md/">Configurer les préférences de gestion des ressources</a>. </p> 
   <p>Vous pouvez mettre à jour le [!UICONTROL Work Time] d’un utilisateur lorsque vous modifiez ou créez l’utilisateur. Pour plus d’informations, voir <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md">Modification du profil d’un utilisateur</a></p> 
   <b>CONSEIL</b> 
   <p>Définissez la valeur [!UICONTROL Work Time] sur 1 pour indiquer que l’utilisateur est disponible pour les travaux liés au projet et qu’il dispose de son équivalent à temps plein.</p> 
   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Temps de travail]</td> 
   <td>Dans la documentation Workfront, ce terme est utilisé pour décrire le temps alloué au travail, selon un planning.</td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL workRequiredExpression]</code> </td> 
   <td> <p>Dans un rapport de projet, de tâche ou de problème, l’instruction suivante en mode texte affiche le nombre d’heures planifiées du projet, de la tâche ou du problème, suivies du mot "Heures" :</p>
   <code>
   <p>valuefield=workRequiredExpression</p>
   <p>valueformat=HTML</p>
   </code>
    <p>Pour plus d’informations sur l’utilisation du mode texte, voir <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">Présentation de la syntaxe du mode texte</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>
