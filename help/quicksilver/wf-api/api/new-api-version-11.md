---
content-type: api
navigation-topic: api-navigation-topic
title: Nouveautés de la version 11 de l’API
description: ReportableBudgedHour a été ajouté à l’API Adobe Workfront en tant que ressource pour la création de rapports. Il comprend des champs de référence, des champs principaux et des champs par défaut absents de la fonction BudgetedHour.
author: Becky
feature: Workfront API
role: Developer
exl-id: b8826dc6-9791-49f6-923d-5a0c5392a8b0
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '3573'
ht-degree: 12%

---

# Nouveautés de la version 11 de l’API

* [Ressources ajoutées](#added-resources)
* [Ressources supprimées](#removed-resources)
* [Ressources modifiées](#modified-resources)

## Ajout de ressources {#added-resources}

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#loginasaccessrule" class="MCXref xref">LoginAsAccessRule</a> </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#loginasadditionalrule" class="MCXref xref">LoginAsAdditionalRule</a> </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#loginassettings" class="MCXref xref">LoginAsSettings</a> </li>
  -->

* [ReportableBudgetedHour](#reportablebudgetedhour)

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="loginasaccessrule">LoginAsAccessRule</h3>
-->

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>Champs directs</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">accessExpirationDate</li> 
     <li style="font-weight: bold;">accesseurID</li> 
     <li style="font-weight: bold;">customerID</li> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">userID</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Champs de référence</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">accesseur</li> 
     <li style="font-weight: bold;">client</li> 
     <li style="font-weight: bold;">user  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Champs principaux</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">objCode</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="loginasadditionalrule">LoginAsAdditionalRule</h3>
-->

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>Champs directs</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">customerID</li> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">loginAsSettingsID</li> 
     <li style="font-weight: bold;">objID</li> 
     <li style="font-weight: bold;">objObjCode  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Champs de référence</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">client  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Champs principaux</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">objCode</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="loginassettings">LoginAsSettings</h3>
-->

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>Champs directs</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">customerID</li> 
     <li style="font-weight: bold;">licenseTypes</li> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">restrictedLoginAs  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Champs de référence</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">client  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Champs de collection</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">additionalRules</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Champs principaux</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">objCode</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ReportableBudgetedHour {#reportablebudgetedhour}

ReportableBudgedHour a été ajouté à l’API Adobe Workfront en tant que ressource pour la création de rapports. Il comprend des champs de référence, des champs principaux et des champs par défaut absents de la fonction BudgetedHour.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Champs directs</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">allocationDate </p> <p>La date d’affectation est le premier jour (un dimanche) de la semaine pour lequel vous avez budgété les heures dans le planificateur de ressources.</p> </li> 
     <li> <p style="font-weight: bold;">recordsHours </p> <p>Les heures budgétisées sont les heures que le gestionnaire de ressources met à la disposition du travail que les ressources doivent effectuer sur les projets.</p> </li> 
     <li> <p style="font-weight: bold;">ID </p> <p>Identifiant Workfront unique attribué à un objet d’heure budgétaire à rapports spécifique.</p> </li> 
     <li style="font-weight: bold;">scheduledBudgetedHours </li> 
     <li> <p style="font-weight: bold;">projectID </p> <p>Identifiant Workfront unique attribué à un projet spécifique.</p> </li> 
     <li> <p style="font-weight: bold;">roleID</p> <p>Identifiant Workfront unique attribué à un rôle de tâche spécifique.</p> </li> 
     <li> <p style="font-weight: bold;">userID</p> <p>Identifiant Workfront unique attribué à un utilisateur spécifique.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Champs de référence</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">projet</p> <p>Projet auquel un ReportableBudgetedHour est associé.</p> </li> 
     <li> <p style="font-weight: bold;">Rôle</p> <p>Rôle de tâche auquel est associé un ReportableBudgetedHour.</p> </li> 
     <li> <p style="font-weight: bold;">utilisateur</p> <p>Utilisateur auquel est associé un ReportableBudgetedHour.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Champs principaux</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">name</li> 
     <li style="font-weight: bold;">objCode</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Champs par défaut</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">name</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Opérations</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">COUNT</li> 
     <li style="font-weight: bold;">GET</li> 
     <li style="font-weight: bold;">RAPPORT </li> 
     <li style="font-weight: bold;">SEARCH</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Ressources supprimées {#removed-resources}

Aucune ressource n’a été supprimée pour l’API v11.

## Ressources modifiées {#modified-resources}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li><a href="#accesslevelpermissions" class="MCXref xref">AccessLevelPermissions</a> </li> 
     <li><a href="#accessrequest" class="MCXref xref">AccessRequest</a> </li> 
     <li><a href="#accessrule" class="MCXref xref">AccessRule</a> </li> 
     <li><a href="#approval" class="MCXref xref">Approbation</a> </li> 
     <li><a href="#approvalpath" class="MCXref xref">ApprovalPath</a> </li> 
     <li><a href="#approvalprocess" class="MCXref xref">ApprovalProcess</a> </li> 
     <li><a href="#assignment" class="MCXref xref">Attribution</a> </li> 
     <li><a href="#baselinetask" class="MCXref xref">BaselineTask</a> </li> 
     <li><a href="#category" class="MCXref xref">Catégorie</a> </li> 
     <li><a href="#company" class="MCXref xref">Entreprise</a> </li> 
     <li><a href="#customenum" class="MCXref xref">CustomEnum</a> </li> 
     <li><a href="#customer" class="MCXref xref">Client</a> </li> 
     <li><a href="#customerpreferences" class="MCXref xref">CustomerPreferences</a> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li><a href="#docmetadatalinkgroup" class="MCXref xref">DocMetadataLinkGroup</a> </li> 
     <li><a href="#document" class="MCXref xref">Document</a> </li> 
     <li><a href="#iteration" class="MCXref xref">Itération</a> </li> 
     <li><a href="#layout-template" class="MCXref xref">Modèle de mise en page</a> </li> 
     <li><a href="#milestonepath" class="MCXref xref">MilestonePath</a> </li> 
     <li><a href="#note" class="MCXref xref">Remarque</a> </li> 
     <li><a href="#optask" class="MCXref xref">OpTask</a> </li> 
     <li><a href="#parameter" class="MCXref xref">Paramètre</a> </li> 
     <li><a href="#portfolio" class="MCXref xref">Portfolio</a> </li> 
     <li><a href="#program" class="MCXref xref">Programme</a> </li> 
     <li><a href="#project" class="MCXref xref">Projet</a> </li> 
     <li><a href="#proofapproval" class="MCXref xref">ProofApproval</a> </li> 
     <li><a href="#queuedef" class="MCXref xref">QueueDef</a> </li> 
     <li><a href="#reservedtime" class="MCXref xref">RéservéTime</a> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li><a href="#resourceplannerfilter" class="MCXref xref">ResourcePlannerFilter</a> </li> 
     <li><a href="#risk" class="MCXref xref">Risque</a> </li> 
     <li><a href="#scheduledreport" class="MCXref xref">ScheduledReport</a> </li> 
     <li><a href="#scorecardquestion" class="MCXref xref">ScoreCardQuestion</a> </li> 
     <li><a href="#task" class="MCXref xref">Tâche</a> </li> 
     <li><a href="#team" class="MCXref xref">Équipe</a> </li> 
     <li><a href="#template" class="MCXref xref">Modèle</a> </li> 
     <li><a href="#templateassignment" class="MCXref xref">TemplateAssignment</a> </li> 
     <li><a href="#templatetask" class="MCXref xref">TemplateTask</a> </li> 
     <li><a href="#timesheet" class="MCXref xref">Feuille de temps</a> </li> 
     <li><a href="#update" class="MCXref xref">Mise à jour</a> </li> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#user" class="MCXref xref">User</a> </li>
     --> 
     <li><a href="#usernote" class="MCXref xref">UserNote</a> </li> 
     <li><a href="#work" class="MCXref xref">Travail </a> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

 

### AccessLevelPermissions {#accesslevelpermissions}

Un objet AccessLevelPermissions représente un ensemble d’autorisations. Cet ensemble d’autorisations peut ensuite être associé à un niveau d’accès.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Champs directs</td> 
   <td> <p>Les champs suivants ont ajouté la valeur possible BUDGETING_INFORMATION. Cela permet aux utilisateurs autorisés de modifier les priorités et les heures budgétaires dans le planificateur.</p> 
    <ul> 
     <li style="font-weight: bold;">coreAction</li> 
     <li style="font-weight: bold;">forbiddenActions</li> 
     <li style="font-weight: bold;">secondaryActions  </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AccessRequest {#accessrequest}

Si un utilisateur ou une utilisatrice n’a pas accès à un objet Workfront dont il ou elle a besoin, il ou elle peut demander l’accès à cet objet. L’objet AccessRequest représente cette demande.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Champs directs</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">action</p> <p>Ajout de la valeur possible BUDGETING_INFORMATION. Cela permet aux utilisateurs autorisés de modifier les priorités et les heures budgétaires dans le planificateur.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AccessRule {#accessrule}

Un objet AccessRule représente un jeu de règles dans les niveaux d’accès personnalisés qui détermine comment les utilisateurs et les utilisatrices peuvent partager les projets qu’ils ou elles créent.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Champs directs</td> 
   <td> <p>Les champs suivants ont ajouté la valeur possible BUDGETING_INFORMATION. Cela permet aux utilisateurs autorisés de modifier les priorités et les heures budgétaires dans le planificateur.</p> 
    <ul> 
     <li style="font-weight: bold;">coreAction</li> 
     <li style="font-weight: bold;">forbiddenActions</li> 
     <li style="font-weight: bold;">secondaryActions  </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Approbation {#approval}

Un élément de travail donné, tel qu’une tâche, un document ou une feuille de temps, peut exiger qu’un superviseur ou une superviseuse, ou un autre utilisateur ou une autre utilisatrice, valide l’élément de travail. Un objet Approval représente l’action de validation d’un élément de travail.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">Champs directs<p style="font-weight: normal;">Les champs suivants ont ajouté les validateurs AT_DATE_BEFORE_YEAR et AT_DATE_AFTER_YEAR. Ces validateurs spécifient que les dates sur les objets associés ne peuvent pas être définies avant 1900 ou après 2200.</p>
    <ul>
     <li style="font-weight: bold;">currentCompletionDate</li>
     <li style="font-weight: bold;">currentStartDate</li>
     <li style="font-weight: bold;">constraintDate</li>
     <li style="font-weight: bold;">scheduleCompletionDate</li>
     <li style="font-weight: bold;">scheduledStartDate</li>
    </ul><p style="font-weight: normal;">Les champs suivants ont été ajoutés à l’API publique pour plus de transparence dans le calcul du taux d’effet élévateur (estimation à la fin).</p>
    <ul>
     <li><p style="font-weight: bold;">bcwp</p><p style="font-weight: normal;">Connue également sous le nom de Valeur acquise, le coût budgété du travail effectué (BCWP) est une mesure de performance du projet qui représente le coût budgété du montant de la tâche qui a été effectivement terminée au moment où cette mesure est calculée. Pour les tâches, BCWP = Pourcentage réel terminé x budget de la tâche. Pour les projets, BCWP = SUM (valeurs BCWP de toutes les tâches parents et individuelles).</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">Également appelé Valeur planifiée, le coût budgété du travail planifié (BCWS) est une mesure de performance du projet qui représente le coût budgété du montant de la tâche qui doit être terminée au moment où cette mesure est calculée. Pour les tâches, BCWS = Pourcentage planifié Complet x Budget de la tâche. Pour les projets, BCWS = SUM (valeurs BCWS de toutes les tâches parents et individuelles).</p></li>
    </ul><p style="font-weight: normal;">Les champs suivants ont ajouté la valeur possible ET. Cette valeur représente l’unité de temps des mois écoulés, qui fait référence aux mois sans tenir compte des week-ends ou des jours fériés.</p>
    <ul>
     <li style="font-weight: bold;">durationUnit</li>
     <li style="font-weight: bold;">workUnit</li>
    </ul><p style="font-weight: normal;">Les champs suivants ont ajouté l’indicateur DEVISE</p>
    <ul>
     <li style="font-weight: bold;">projectBudgetedCost</li>
     <li style="font-weight: bold;">projectNetValue</li>
    </ul><p style="font-weight: normal;">Les champs suivants ont été supprimés de l’objet Approval.</p>
    <ul>
     <li style="font-weight: bold;">reserveTimeID</li>
     <li style="font-weight: bold;">timelineExceptionInfo</li>
    </ul><p style="font-weight: normal;">Le champ suivant a été ajouté à l’objet Approval.</p>
    <ul>
     <li style="font-weight: bold;">storyPoints</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>Champs de référence</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>reserveTime</p> <p style="font-weight: normal;">Retiré de l’objet Approval  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Champs de collection</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">Ajout à l’objet Approval.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ApprovalPath {#approvalpath}

Un objet ApprovalPath est une branche dans un processus d’approbation. Les chemins d’approbation sont basés sur l’état de l’objet auquel le processus d’approbation est associé.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Champs directs</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>durationUnit </p> <p style="font-weight: normal;">Ajout de la valeur possible ET. Cette valeur représente l’unité de temps des mois écoulés, qui fait référence aux mois sans tenir compte des week-ends ou des jours fériés.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ApprovalProcess {#approvalprocess}

Un objet ApprovalProcess est une approbation en plusieurs étapes qui peut être associée à un projet, une tâche ou un problème.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Champs directs</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Ce champ a été ajouté. Il s’agit d’un paramètre booléen dont la valeur est true si un objet est actif et false dans le cas contraire. Les objets définis sur Actif s’affichent dans des menus déroulants et des champs de type avant et peuvent être associés à d’autres objets. Les objets qui ne sont pas définis sur Actif ne sont pas visibles dans les menus déroulants et les champs de type devant à joindre à d’autres objets.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Champs par défaut</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Ajouté(e)(s)</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Affectation {#assignment}

Un objet d’affectation représente la connexion entre un élément de travail et l’utilisateur, l’équipe ou le groupe affecté pour y travailler.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Champs directs</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>workUnit </p> <p style="font-weight: normal;">Ajout de la valeur possible ET. Cette valeur représente l’unité de temps des mois écoulés, qui fait référence aux mois sans tenir compte des week-ends ou des jours fériés.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### BaselineTask {#baselinetask}

Les références sont des instantanés de ce à quoi ressemblaient les performances d’un projet à un moment donné dans le temps. Elles stockent des informations clés sur le projet, telles que les dates clés, la progression, et les valeurs de coût et de revenu. Lorsque vous créez une référence, les informations de tâche sont également capturées sur les tâches de base de cette référence.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Champs directs</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>durationUnit </p> <p style="font-weight: normal;">Ajout de la valeur possible ET. Cette valeur représente l’unité de temps des mois écoulés, qui fait référence aux mois sans tenir compte des week-ends ou des jours fériés.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Catégorie {#category}

Un objet Category est un formulaire personnalisé. Vous pouvez créer des rapports pour cet objet et les afficher dans d’autres rapports d’objet.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Champs directs</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Ce champ a été ajouté. Il s’agit d’un paramètre booléen dont la valeur est true si un objet est actif et false dans le cas contraire. Les objets définis sur Actif s’affichent dans des menus déroulants et des champs de type avant et peuvent être associés à d’autres objets. Les objets qui ne sont pas définis sur Actif ne sont pas visibles dans les menus déroulants et les champs de type devant à joindre à d’autres objets.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Champs par défaut</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Ajouté(e)(s)</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Entreprise {#company}

Un objet Société représente une organisation composée d’un ensemble de personnes. Les entreprises sont associées à un utilisateur ou à un projet.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Champs directs</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Ce champ a été ajouté. Il s’agit d’un paramètre booléen dont la valeur est true si un objet est actif et false dans le cas contraire. Les objets définis sur Actif s’affichent dans des menus déroulants et des champs de type avant et peuvent être associés à d’autres objets. Les objets qui ne sont pas définis sur Actif ne sont pas visibles dans les menus déroulants et les champs de type devant à joindre à d’autres objets.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Champs par défaut</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Ajouté(e)(s)</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### CustomEnum {#customenum}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">A CustomEnum object is an enumeration that is created in Workfront to be used in objects and fields throughout Workfront.</p>
-->

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Actions</td> 
   <td> <p style="font-weight: normal;">Ajout des actions suivantes à l’objet CustomEnum</p> 
    <ul> 
     <li style="font-weight: bold;">getDefaultOpTaskConditionEnum</li> 
     <li style="font-weight: bold;">getDefaultProjectConditionEnum</li> 
     <li style="font-weight: bold;">getDefaultTaskConditionEnum</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Requêtes</td> 
   <td> <p>Les requêtes suivantes ont été ajoutées à l’objet CustomEnum .</p> 
    <ul> 
     <li style="font-weight: bold;">opTaskConditions</li> 
     <li style="font-weight: bold;">projectConditions</li> 
     <li style="font-weight: bold;">taskConditions</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Client {#customer}

Un objet client représente une organisation qui utilise une instance de Workfront.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td>Champs directs</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>customEnumTypes</p> <p style="font-weight: normal;">Ajout des valeurs possibles : </p> 
      <ul> 
       <li style="font-weight: normal;">CONDITION_PROJ (conditions du projet)</li> 
       <li style="font-weight: normal;">CONDITION_TASK (Conditions de tâche)</li> 
       <li style="font-weight: normal;">CONDITION_OPTASK (Conditions de problème)  </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Reference Fields</td> 
    <td> 
     <ul> 
      <li style="font-weight: bold;"> <p>loginAsSettings</p> <p style="font-weight: normal;">Added. &nbsp;</p> </li> 
     </ul> </td> 
   </tr>
  --> 
  <tr> 
   <td>Actions</td> 
   <td> <p style="font-weight: normal;">Les actions suivantes ont été ajoutées à l’objet client</p> 
    <ul> 
     <li style="font-weight: bold;">ObjectifEnabled</li> 
     <li style="font-weight: bold;">updateLoginAsSettings</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### CustomerPreferences {#customerpreferences}

Un objet CustomerPreferences représente l’ensemble des préférences définies par un client pour son instance de Workfront.

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>Champs directs</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>name</p> <p style="font-weight: normal;">Ajout des valeurs possibles :</p> 
      <ul> 
       <li style="font-weight: normal;">password:password.eauthPolicy (Exigences de complexité du mot de passe)</li> 
       <li style="font-weight: normal;"> password:password.minimumLength (Longueur minimum du mot de passe)</li> 
       <li style="font-weight: normal;">password:mobileSessionTimeout (délai d’expiration de la session mobile)</li> 
       <li style="font-weight: normal;"> project.mgmt:default.project.usertimeoff (heure de désactivation de l’utilisateur)</li> 
       <li style="font-weight: normal;">timesheet:default.timesheet.manualrole (rôle de contrôle manuel)</li> 
       <li style="font-weight: normal;">BAT:defaultNonRecipientRole (config.proofhq.defaultnonrecipientrole) </li> 
       <li style="font-weight: normal;">BAT:defaultNonRecipientGuestRole (config.proofhq.defaultnon-recipientguestrole)  </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### DocMetadataLinkGroup {#docmetadatalinkgroup}

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Actions</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>getMetadataDetailsForDocument</p> <p style="font-weight: normal;">Ajouté(e)(s)</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Document {#document}

Un objet Document représente un fichier (tel qu’un support écrit, des images ou d’autres formes d’informations).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Actions</td> 
   <td> <p>Les actions suivantes ont été ajoutées à l’objet Document .</p> 
    <ul> 
     <li style="font-weight: bold;">completeLargeDocument</li> 
     <li style="font-weight: bold;">createLargeDocument</li> 
     <li style="font-weight: bold;">createProofRest</li> 
     <li style="font-weight: bold;">getDocumentProofTemplate</li> 
     <li style="font-weight: bold;">getProofRecipients</li> 
     <li style="font-weight: bold;">getProofStages</li> 
     <li style="font-weight: bold;">getProofTemplate</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Itération {#iteration}

Un objet Itération représente une seule itération Agile. Les itérations sont des périodes discrètes utilisées pour planifier et compléter des histoires Agile.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Champs directs</td> 
   <td> <p>Les champs suivants ont été ajoutés à l’objet Itération .</p> 
    <ul> 
     <li style="font-weight: bold;">originalTotalPoints</li> 
     <li style="font-weight: bold;">points terminés</li> 
     <li style="font-weight: bold;">totalPoints  </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Modèles de mise en page {#layout-template}

Un objet Modèle de mise en page représente une disposition particulière des éléments de mise en page, tels que le menu principal, le panneau de navigation ou la zone d’accueil. Les modèles de mise en page peuvent être attribués à des utilisateurs, des équipes, des groupes ou des rôles de tâche.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Champs directs</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>showHomeTimestamps </p> <p style="font-weight: normal;">Ce champ a été ajouté. Il s’agit d’un paramètre booléen dont la valeur est true si un modèle de mise en page est défini pour afficher les horodatages des dates d’échéance dans la liste de travail et le calendrier, et false s’il est défini pour masquer les horodatages.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Champs par défaut</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>showHomeTimestamps</p> <p style="font-weight: normal;">Ajouté(e)(s)</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### MilestonePath {#milestonepath}

Un jalon est un marqueur d’une tâche qui indique qu’il s’agit d’un point clé du projet. Généralement utilisé pour désigner un événement important, tel que la fin d’une phase du projet ou un ensemble d’activités critiques. Un objet MilestonePath est un ensemble de jalons.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Champs directs</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Ce champ a été ajouté. Il s’agit d’un paramètre booléen dont la valeur est true si un objet est actif et false dans le cas contraire. Les objets définis sur Actif s’affichent dans des menus déroulants et des champs de type avant et peuvent être associés à d’autres objets. Les objets qui ne sont pas définis sur Actif ne sont pas visibles dans les menus déroulants et les champs de type devant à joindre à d’autres objets.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Champs par défaut</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Ajouté(e)(s)</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Note {#note}

Un objet Remarque est un commentaire ou une mise à jour effectué sur un objet Workfront.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Champs directs</td> 
   <td> <p>Les champs suivants ont été ajoutés à l’objet Remarque .</p> 
    <ul> 
     <li style="font-weight: bold;">proofID  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Champs de collection</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>likes</p> <p style="font-weight: normal;">Ajouté(e)(s)</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### TâcheOp {#optask}

Un objet OpTask est généralement appelé un Problème. Un problème est un élément de travail qui indique généralement qu’un problème empêche la réalisation d’une tâche ou d’un projet. Il peut également s’agir d’une demande de service d’assistance. Les ordres de modification, les demandes et les bogues sont également des problèmes.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">Champs directs<p style="font-weight: normal;">Les champs suivants ont ajouté les validateurs AT_DATE_BEFORE_YEAR et AT_DATE_AFTER_YEAR. Ces valeurs spécifient que les dates sur les objets associés ne peuvent pas être définies avant l’an 1900 ou après 2200.</p>
    <ul>
     <li style="font-weight: bold;">currentCompletionDate</li>
     <li style="font-weight: bold;">currentStartDate</li>
     <li style="font-weight: bold;">scheduleCompletionDate</li>
     <li style="font-weight: bold;">scheduledStartDate</li>
    </ul><p style="font-weight: normal;">Les champs suivants ont été ajoutés à OpTask.</p>
    <ul>
     <li style="font-weight: bold;"><p>kanbanBoardID </p><p style="font-weight: normal;">Identifiant Workfront unique d’un objet de panorama Kanban.</p></li>
     <li style="font-weight: bold;"><p>percentComplete</p><p style="font-weight: normal;">Pourcentage terminé est un paramètre qui renvoie le montant terminé d’une émission, sous forme de pourcentage.</p></li>
     <li style="font-weight: bold;">storyPoints</li>
     <li style="font-weight: bold;">work  </li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>Champs de collection</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">Ajouté(e)(s)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Champs de recherche</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>work</p> <p style="font-weight: normal;">Supprimé</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Champs par défaut</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>percentComplete</p> <p style="font-weight: normal;">Ajouté(e)(s)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Actions</td> 
   <td> <p>Les actions suivantes ont été ajoutées à l’objet OpTask</p> 
    <ul> 
     <li style="font-weight: bold;">bulkMove</li> 
     <li style="font-weight: bold;">copyIssue</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Paramètre {#parameter}

Un objet de paramètre est un champ personnalisé.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Champs directs</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>displayType</p> <p style="font-weight: normal;">Ajout de la valeur possible TYAH (Typeforward).</p> </li> 
     <li style="font-weight: bold;"> <p>refObjCode </p> <p style="font-weight: normal;">Ce champ a été ajouté et fait référence au code d’objet d’un objet référencé. Les codes d’objet pour tous les objets se trouvent dans l’ <a href="../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Portfolio {#portfolio}

Un objet de Portfolio est un ensemble de projets qui rivalisent pour les mêmes ressources, généralement de l’argent ou des personnes pour les compléter.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Champs directs</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>description</p> <p style="font-weight: normal;">Ajout du programme de validation MAX_LENGTH, qui spécifie que la longueur de la description ne dépasse pas 4 000 caractères.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Programme {#program}

Un objet de programme est un sous-ensemble d’un portfolio, où des projets similaires peuvent être regroupés.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Champs directs</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>description</p> <p style="font-weight: normal;">Ajout du programme de validation MAX_LENGTH, qui spécifie que la longueur de la description ne dépasse pas 4 000 caractères.</p> </li> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Ce champ a été ajouté. Il s’agit d’un paramètre booléen dont la valeur est true si un objet est actif et false dans le cas contraire. Les objets définis sur Actif s’affichent dans des menus déroulants et des champs de type avant et peuvent être associés à d’autres objets. Les objets qui ne sont pas définis sur Actif ne sont pas visibles dans les menus déroulants et les champs de type devant à joindre à d’autres objets.  </p> </li> 
     <li style="font-weight: bold;"> <p>name </p> <p style="font-weight: normal;">Ajout du programme de validation MAX_LENGTH, qui spécifie que la longueur du nom ne dépasse pas 255 caractères.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Champs par défaut</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Ajouté(e)(s)</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Projet {#project}

Les projets sont des éléments de travail dans Workfront et sont un bloc de création essentiel de la façon dont Workfront aide les personnes à travailler. Un objet Project représente un groupe de tâches avec un objectif commun et spécifique.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">Champs directs<p style="font-weight: normal;">Les champs suivants ont ajouté les validateurs AT_DATE_BEFORE_YEAR et AT_DATE_AFTER_YEAR. Ces valeurs spécifient que les dates sur les objets associés ne peuvent pas être définies avant l’an 1900 ou après 2200.</p>
    <ul>
     <li style="font-weight: bold;">currentCompletionDate</li>
     <li style="font-weight: bold;">currentStartDate</li>
     <li style="font-weight: bold;">scheduleCompletionDate</li>
     <li style="font-weight: bold;">scheduledStartDate</li>
    </ul><p style="font-weight: normal;">Les champs suivants ont été ajoutés à l’API publique pour plus de transparence dans le calcul du taux d’effet élévateur (estimation à la fin).</p>
    <ul>
     <li><p style="font-weight: bold;">bcwp</p><p style="font-weight: normal;">Connue également sous le nom de Valeur acquise, le coût budgété du travail effectué (BCWP) est une mesure de performance du projet qui représente le coût budgété du montant de la tâche qui a été effectivement terminée au moment où cette mesure est calculée. Pour les tâches, BCWP = Pourcentage réel terminé x budget de la tâche. Pour les projets, BCWP = SUM (valeurs BCWP de toutes les tâches parents et individuelles).</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">Également appelé Valeur planifiée, le coût budgété du travail planifié (BCWS) est une mesure de performance du projet qui représente le coût budgété du montant de la tâche qui doit être terminée au moment où cette mesure est calculée. Pour les tâches, BCWS = Pourcentage planifié Complet x Budget de la tâche. Pour les projets, BCWS = SUM (valeurs BCWS de toutes les tâches parents et individuelles).</p></li>
    </ul><p style="font-weight: normal;">Les champs suivants ont ajouté l’indicateur DEVISE</p>
    <ul>
     <li style="font-weight: bold;">projectBudgetedCost</li>
     <li style="font-weight: bold;">projectNetValue</li>
    </ul><p style="font-weight: normal;">Le champ suivant a été supprimé de l’objet de projet.</p>
    <ul>
     <li style="font-weight: bold;">timelineExceptionInfo</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>Champs de collection</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">Ajouté(e)(s)</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ProofApproval {#proofapproval}

Un objet ProofApproval représente une validation directement connectée à un BAT.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Champs directs</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isAwaitDecision</p> <p style="font-weight: normal;">Ce champ a été ajouté. Il s’agit d’un paramètre booléen dont la valeur est true si un BAT attend une décision et false dans le cas contraire.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### QueueDef {#queuedef}

Un objet QueueDef représente une file d’attente, qui est un projet qui a été publié dans la zone Aide Desk pour permettre aux utilisateurs de lui envoyer des problèmes.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Champs directs</td> 
   <td> <p>Les champs suivants ont ajouté la valeur possible BUDGETING_INFORMATION. Cela permet aux utilisateurs autorisés de modifier les priorités et les heures budgétaires dans le planificateur.</p> 
    <ul> 
     <li style="font-weight: bold;">requestorCoreAction</li> 
     <li style="font-weight: bold;">requestorForbiddenActions</li> 
    </ul>  </td> 
  </tr> 
 </tbody> 
</table>

### RéservéTime {#reservedtime}

Un objet ReserveTime représente les jours spécifiés dans l’heure personnelle d’un utilisateur, ce qui indique que l’utilisateur ne sera pas disponible pour le travail.

La ressource ReserveTime a ajouté l’indicateur REPORTABLE.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Champs directs</td> 
   <td> <p>Les champs suivants ont supprimé l’indicateur NOT_GROUPABLE.</p> 
    <ul> 
     <li style="font-weight: bold;">endDate</li> 
     <li style="font-weight: bold;">extRefID</li> 
     <li style="font-weight: bold;">startDate </li> 
    </ul> <p>Le champ suivant a été supprimé de l’objet ReserveTime .</p> 
    <ul> 
     <li style="font-weight: bold;">taskID</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Champs de référence</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>tâche</p> <p style="font-weight: normal;">Supprimé  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Opérations</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>MODIFIER</p> <p style="font-weight: normal;">Ajouté(e)(s)</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ResourcePlannerFilter {#resourceplannerfilter}

Un objet ResourcePlannerFilter est un ensemble de règles qui déterminent les éléments qui s’afficheront dans le planificateur de ressources.

La ressource ResourcePlannerFilter a ajouté l’indicateur SHARABLE. Il n’y a eu aucune autre modification de l’objet.

### Risque {#risk}

Un objet Risk représente un événement possible qui peut empêcher la fin d’un projet à temps ou dans les limites du budget. Lors de la phase de planification, des risques sont ajoutés aux projets pour identifier les obstacles potentiels avant l’approbation des travaux.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Champs directs</td> 
   <td> <p>Les champs suivants ont été ajoutés à l'objet Risk :</p> 
    <ul> 
     <li style="font-weight: bold;"> <p>entryByID</p> <p style="font-weight: normal;">L’identifiant de l’utilisateur qui a créé l’objet à l’origine.</p> </li> 
     <li> <p style="font-weight: bold;">entryDate</p> <p>Date à laquelle un utilisateur a envoyé un objet dans Workfront.</p> </li> 
     <li> <p style="font-weight: bold;">lastUpdateDate</p> <p>Le paramètre Date de dernière mise à jour renvoie la date à laquelle la dernière mise à jour a été effectuée sur un objet,</p> </li> 
     <li> <p style="font-weight: bold;">lastUpdatedByID </p> <p>Dernière mise à jour par identifiant est un paramètre qui renvoie l’identifiant utilisateur du dernier utilisateur qui a mis à jour l’objet.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Champs de référence</td> 
   <td> <p style="font-weight: normal;">Les champs de référence suivants ont été ajoutés à l’objet RIsk .</p> 
    <ul> 
     <li style="font-weight: bold;">entryBy</li> 
     <li style="font-weight: bold;">lastUpdatedBy  </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ScheduledReport {#scheduledreport}

Un objet ScheduledReport représente un rapport qui a été configuré pour être distribué.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Champs directs</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>pageSize</p> <p style="font-weight: normal;">Ajout des valeurs possibles suivantes :</p> 
      <ul> 
       <li style="font-weight: normal;">A2</li> 
       <li style="font-weight: normal;">A1</li> 
       <li style="font-weight: normal;">A0  </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ScoreCardQuestion {#scorecardquestion}

Un objet ScoreCardQuestion représente une question qui a été ajoutée à une Fiche d’évaluation. Ces questions sont généralement définies par le responsable du Portfolio et leurs réponses permettent au responsable de comprendre dans quelle mesure un projet s’aligne sur les objectifs du portefeuille.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Champs directs</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>displayType</p> <p style="font-weight: normal;">Ajout de la valeur possible TYAH (en caractères d’avance)  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Tâche {#task}

Un objet Task représente un élément de travail qui doit être exécuté en tant qu’étape vers la réalisation d’un objectif final (achèvement d’un projet).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">Champs directs<p style="font-weight: normal;">Les champs suivants ont ajouté les validateurs AT_DATE_BEFORE_YEAR et AT_DATE_AFTER_YEAR. Ces valeurs spécifient que les dates sur les objets associés ne peuvent pas être définies avant l’an 1900 ou après 2200.</p>
    <ul>
     <li style="font-weight: bold;">currentCompletionDate</li>
     <li style="font-weight: bold;">currentStartDate</li>
     <li style="font-weight: bold;">constraintDate</li>
     <li style="font-weight: bold;">scheduleCompletionDate</li>
     <li style="font-weight: bold;">scheduledStartDate</li>
    </ul><p style="font-weight: normal;">Les champs suivants ont été ajoutés à l’API publique pour plus de transparence dans le calcul du taux d’effet élévateur (estimation à la fin).</p>
    <ul>
     <li><p style="font-weight: bold;">bcwp</p><p style="font-weight: normal;">Connue également sous le nom de Valeur acquise, le coût budgété du travail effectué (BCWP) est une mesure de performance du projet qui représente le coût budgété du montant de la tâche qui a été effectivement terminée au moment où cette mesure est calculée. Pour les tâches, BCWP = Pourcentage réel terminé x budget de la tâche. Pour les projets, BCWP = SUM (valeurs BCWP de toutes les tâches parents et individuelles).</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">Également appelé Valeur planifiée, le coût budgété du travail planifié (BCWS) est une mesure de performance du projet qui représente le coût budgété du montant de la tâche qui doit être terminée au moment où cette mesure est calculée. Pour les tâches, BCWS = Pourcentage planifié Complet x Budget de la tâche. Pour les projets, BCWS = SUM (valeurs BCWS de toutes les tâches parents et individuelles).</p></li>
    </ul><p style="font-weight: normal;">Les champs suivants ont ajouté la valeur possible ET. Cette valeur représente l’unité de temps des mois écoulés, qui fait référence aux mois sans tenir compte des week-ends ou des jours fériés.</p>
    <ul>
     <li style="font-weight: bold;">durationUnit</li>
     <li style="font-weight: bold;">workUnit</li>
    </ul><p style="font-weight: normal;">Le champ suivant a été supprimé de l’objet Task.</p>
    <ul>
     <li style="font-weight: bold;">reserveTimeID</li>
    </ul><p style="font-weight: normal;">Le champ suivant a été ajouté à l’objet Task.</p>
    <ul>
     <li style="font-weight: bold;">storyPoints</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>Champs de référence</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>reserveTime</p> <p style="font-weight: normal;">Supprimé  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Champs de collection</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">Ajouté(e)(s)</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Equipe {#team}

Un objet Équipe est un ensemble d’utilisateurs pouvant être affectés à un élément de travail.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Champs directs</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>agileEstimateType </p> <p style="font-weight: normal;">Ce champ a été ajouté à l’objet Team . Le type d’estimation agile détermine la manière dont la charge de travail d’un article est estimée. S’il est estimé en heures, il s’agit du nombre d’heures planifiées ajoutées à l’article. Si vous l’estimez en points, chaque point ajoute un certain nombre d’heures planifiées à l’article en fonction de la définition des points (la valeur par défaut est de 8 heures). Les valeurs possibles pour le type d’estimation agile sont les suivantes :</p> 
      <ul> 
       <li style="font-weight: normal;"> STORY_POINTS (points d’article)</li> 
       <li style="font-weight: normal;">HEURES (Hours)</li> 
       <li style="font-weight: normal;">LEGACY_POINTS (Hours en tant que points)  </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Modèle {#template}

Un objet Template représente un modèle pour un projet. Les projets peuvent être créés à partir de modèles pour gagner du temps. Un modèle contient une équipe et des tâches qui seront copiées dans un projet lorsque le modèle sera utilisé.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Champs directs</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Ce champ a été ajouté. Il s’agit d’un paramètre booléen dont la valeur est true si un objet est actif et false dans le cas contraire. Les objets définis sur Actif s’affichent dans des menus déroulants et des champs de type avant et peuvent être associés à d’autres objets. Les objets qui ne sont pas définis sur Actif ne sont pas visibles dans les menus déroulants et les champs de type devant à joindre à d’autres objets.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Champs de collection</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allPriority</p> <p style="font-weight: normal;">Ajouté(e)(s)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Champs par défaut</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Ajouté(e)(s)</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### TemplateAssignment {#templateassignment}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">A TemplateAssignment object represents the connection between a Template and the User, Team, or Group it is assigned to.</p>
-->

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Champs directs</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>workUnit</p> <p style="font-weight: normal;">Ajout de la valeur possible ET. Cette valeur représente l’unité de temps des mois écoulés, qui fait référence aux mois sans tenir compte des week-ends ou des jours fériés.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### TemplateTask {#templatetask}

Un objet TemplateTask représente une tâche qui fait partie d’un modèle. Les tâches de modèle deviennent des tâches dans le projet où le modèle est utilisé.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Champs directs</td> 
   <td> <p style="font-weight: normal;">Les champs suivants ont ajouté la valeur possible ET. Cette valeur représente l’unité de temps des mois écoulés, qui fait référence aux mois sans tenir compte des week-ends ou des jours fériés.</p> 
    <ul> 
     <li style="font-weight: bold;">durationUnit</li> 
     <li style="font-weight: bold;">workUnit</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Champs de collection</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allPriority</p> <p style="font-weight: normal;">Ajouté(e)(s)</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Feuille de temps {#timesheet}

Un objet de feuille de temps représente une feuille de temps virtuelle qui permet aux utilisateurs de saisir les heures réelles travaillées pour les tâches, les projets et les types d’heures de surcharge.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Champs principaux</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>objCode</p> <p style="font-weight: normal;">Supprimé</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Mettre à jour {#update}

Les éléments de travail dans Workfront peuvent être mis à jour afin de tenir les utilisateurs et utilisatrices informés du statut actuel. Un objet Update représente l’une de ces mises à jour. Les mises à jour peuvent être saisies par les utilisateurs et utilisatrices ou créées par le système Workfront.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Champs directs</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>updateType</p> <p style="font-weight: normal;">Ajout de la valeur possible referenceObjectCustomData (enum.updatetypeenum.referenceobjectcustomdata)  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Requêtes</td> 
   <td> <p style="font-weight: normal;">Les requêtes suivantes ont été ajoutées à l’objet Update .</p> 
    <ul> 
     <li style="font-weight: bold;">objectUpdatesMobile</li> 
     <li style="font-weight: bold;">updateThreadMobile</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="user">User</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">A User object represents a person with an account in Workfront that can log in and interact with the system.</p>
-->

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>Champs de collection</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>loginAsAccessRules</p> <p style="font-weight: normal;">Ajouté(e)(s)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Actions</td> 
   <td> <p style="font-weight: normal;">Les actions suivantes ont été ajoutées à l’objet User .</p> 
    <ul> 
     <li style="font-weight: bold;">hasGrantLoginAsAccess</li> 
     <li style="font-weight: bold;">isUserAdmin</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Requêtes</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>userAdmins</p> <p style="font-weight: normal;">Ajouté(e)(s)</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### UserNote {#usernote}

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Actions</td> 
   <td> <p style="font-weight: normal;">Les actions suivantes ont été ajoutées à l’objet User .</p> 
    <ul> 
     <li style="font-weight: bold;">acceptMyNotifications</li> 
     <li style="font-weight: bold;">unknownAllObjectsTypeCount  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Requêtes</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>myAllObjectTypesUnreadNotifications</p> <p style="font-weight: normal;">Ajouté(e)(s)</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Travail  {#work}

Un objet Work est une interface commune dont Task et OpTask héritent tous deux, et partage le code commun entre les deux.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">Champs directs<p style="font-weight: normal;">Les champs suivants ont ajouté les validateurs AT_DATE_BEFORE_YEAR et AT_DATE_AFTER_YEAR. Ces valeurs spécifient que les dates sur les objets associés ne peuvent pas être définies avant l’an 1900 ou après 2200.</p>
    <ul>
     <li style="font-weight: bold;">currentCompletionDate</li>
     <li style="font-weight: bold;">currentStartDate</li>
     <li style="font-weight: bold;">constraintDate</li>
     <li style="font-weight: bold;">scheduleCompletionDate</li>
     <li style="font-weight: bold;">scheduledStartDate</li>
    </ul><p style="font-weight: normal;">Les champs suivants ont été ajoutés à l’API publique pour plus de transparence dans le calcul du taux d’effet élévateur (estimation à la fin).</p>
    <ul>
     <li><p style="font-weight: bold;">bcwp</p><p style="font-weight: normal;">Connue également sous le nom de Valeur acquise, le coût budgété du travail effectué (BCWP) est une mesure de performance du projet qui représente le coût budgété du montant de la tâche qui a été effectivement terminée au moment où cette mesure est calculée. Pour les tâches, BCWP = Pourcentage réel terminé x budget de la tâche. Pour les projets, BCWP = SUM (valeurs BCWP de toutes les tâches parents et individuelles).</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">Également appelé Valeur planifiée, le coût budgété du travail planifié (BCWS) est une mesure de performance du projet qui représente le coût budgété du montant de la tâche qui doit être terminée au moment où cette mesure est calculée. Pour les tâches, BCWS = Pourcentage planifié Complet x Budget de la tâche. Pour les projets, BCWS = SUM (valeurs BCWS de toutes les tâches parents et individuelles).</p></li>
    </ul><p style="font-weight: normal;">Les champs suivants ont ajouté la valeur possible ET. Cette valeur représente l’unité de temps des mois écoulés, qui fait référence aux mois sans tenir compte des week-ends ou des jours fériés.</p>
    <ul>
     <li style="font-weight: bold;">durationUnit</li>
     <li style="font-weight: bold;">workUnit</li>
    </ul><p style="font-weight: normal;">Le champ suivant a été supprimé de l’objet de travail.</p>
    <ul>
     <li style="font-weight: bold;">reserveTimeID</li>
    </ul><p style="font-weight: normal;">Le champ suivant a été ajouté à l’objet de travail.</p>
    <ul>
     <li style="font-weight: bold;">storyPoints</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>Champs de référence</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>reserveTime</p> <p style="font-weight: normal;">Supprimé  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Champs de collection</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">Ajouté(e)(s)</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
