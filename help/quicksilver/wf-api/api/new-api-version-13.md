---
content-type: api
navigation-topic: api-navigation-topic
title: Nouveautés de l’API version 13
description: Adobe Workfront a publié l’API version 13 le 22 avril 2021. L’API version 13 comprend les modifications suivantes à partir de la version 12.
author: Becky
feature: Workfront API
exl-id: afbc986e-8b5c-40bc-9120-e8d34e0f7004
source-git-commit: 1ea7e1a0435e9d199c3d828723d11ce530a80540
workflow-type: tm+mt
source-wordcount: '1064'
ht-degree: 2%

---

# Nouveautés de l’API version 13

Adobe Workfront a publié l’API version 13 le 22 avril 2021. L’API version 13 comprend les modifications suivantes à partir de la version 12.

## Ressources ajoutées

Aucune ressource n’a été ajoutée pour l’API version 13.

## Ressources supprimées

Aucune ressource n’a été supprimée pour l’API version 13.

## Ressources modifiées

Les ressources suivantes ont été modifiées pour l’API version 13.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li> <p><a href="#accesslevel" class="MCXref xref">AccessLevel</a> </p> </li> 
     <li> <p><a href="#breadcrumb" class="MCXref xref">BreadCrumb</a> </p> </li> 
     <li> <p><a href="#burndownevent" class="MCXref xref">BurndownEvent</a> </p> </li> 
     <li> <p><a href="#customerpreferences" class="MCXref xref">CustomerPreferences</a> </p> </li> 
     <li> <p><a href="#documentversion" class="MCXref xref">DocumentVersion</a> </p> </li> 
     <li> <p><a href="#group" class="MCXref xref">Groupe </a> </p> </li> 
     <li> <p><a href="#journalentry" class="MCXref xref">JournalEntry</a> </p> </li> 
     <li> <p><a href="#layouttemplate" class="MCXref xref">LayoutTemplate</a> </p> </li> 
     <li> <p><a href="#linkedfolder" class="MCXref xref">LinkedFolder</a> </p> </li> 
     <li> <p><a href="#optask" class="MCXref xref">TâcheOp</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="#project" class="MCXref xref">Projet</a> </p> </li> 
     <li> <p><a href="#proofapproval" class="MCXref xref">ProofApproval</a> </p> </li> 
     <li> <p><a href="#queuedef" class="MCXref xref">QueueDef</a> </p> </li> 
     <li> <p><a href="#task" class="MCXref xref">Tâche</a> </p> </li> 
     <li> <p><a href="#team" class="MCXref xref">Équipe</a> </p> </li> 
     <li> <p><a href="#timesheet" class="MCXref xref">Feuille de temps</a> </p> </li> 
     <li> <p><a href="#timesheetprofile" class="MCXref xref">TimesheetProfile</a> </p> </li> 
     <li> <p><a href="#uitemplate" class="MCXref xref">UITemplate</a> </p> </li> 
     <li> <p><a href="#userdelegation" class="MCXref xref">UserDelegation</a> </p> </li> 
     <li> <p><a href="#work" class="MCXref xref">Travail </a> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AccessLevel {#accesslevel}

Un objet AccessLevel est associé aux utilisateurs et décrit le jeu d’autorisations AccessLevel qui déterminent ce à quoi l’utilisateur peut accéder.

Pour plus d’informations sur les niveaux d’accès, voir [Fonctionnement des niveaux d’accès](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Champs directs</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>Description</b> </p> <p>Ajout du programme de validation MAX_LENGTH, qui spécifie que la longueur de la description ne dépasse pas 4 000 caractères.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### BreadCrumb {#breadcrumb}

Un objet BreadCrumb représente un élément dans la hiérarchie parent/enfant d’un élément de travail Workfront. Les chemins de navigation indiquent comment un élément de travail s’intègre à la plus grande structure de Portfolios, de projets, de projets et de tâches.

Pour plus d’informations sur les chemins de navigation, voir [Présentation du chemin de navigation dans la nouvelle expérience Adobe Workfront](../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md)

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Champs directs</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>objCode</b> </p> <p>Les codes d’objet se trouvent dans la variable <a href="../../wf-api/general/api-explorer.md" class="MCXref xref">Explorateur d’API</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### BurndownEvent {#burndownevent}

Un objet BurndownEvent représente un objet qui modifie le lot d’une itération.

Pour plus d’informations sur la ventilation, voir [Burndown](../../agile/use-scrum-in-an-agile-team/burndown/burndown.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Champs directs</p> </td> 
   <td> <p>Les champs suivants ont supprimé l’indicateur NOT_GROUPABLE </p> 
    <ul> 
     <li> <p>applyDate</p> </li> 
     <li> <p>entryDate</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### CustomerPreferences {#customerpreferences}

Un objet CustomerPreferences représente l’ensemble des préférences définies par un client pour son instance de Workfront.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Champs directs</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>name</p> <p style="font-weight: normal;">Ajout des valeurs possibles :</p> 
      <ul> 
       <li style="font-weight: normal;">password:aemAPIKey (config.general.aem.apikey)</li> 
       <li style="font-weight: normal;"> password:aemAADomain (config.general.aem.adomain) </li> 
       <li style="font-weight: normal;">password:aemIntegrationEnabled (config.general.aem.enabled)</li> 
       <li style="font-weight: normal;">password:aemHost (config.general.aem.host)</li> 
       <li style="font-weight: normal;">timesheet:default.timesheet.restricted.timesheet.edit.owner.admins (config.timesheet.restricted.timesheet.edit.owner.admins)</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Actions</td> 
   <td> <p>Les actions suivantes ont été ajoutées à la ressource CustomerPreferences .</p> 
    <ul> 
     <li> <p><b>getTimesheetPreferences</b> </p> </li> 
     <li> <p><b>setTimesheetPreferences</b> </p> <p>Prend l’argument :</p> 
      <ul> 
       <li> <p>preferences (map)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### DocumentVersion {#documentversion}

Un objet DocumentVersion représente une version spécifique d’un fichier (comme du matériel écrit, des images ou d’autres formes d’informations).

Pour plus d’informations sur les versions de document, voir [Télécharger une nouvelle version d’un document](../../documents/managing-documents/upload-new-document-version.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Champs directs</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>externalIntegrationType</b> </p> <p>Ajout de la valeur possible :</p> 
      <ul> 
       <li> <p>AEM (Adobe Experience Manager)</p> </li> 
      </ul> </li> 
    </ul> 
    <ul> 
     <li> <p><b>proofID</b> </p> <p>Ajout de l’indicateur NOT_FILTERABLE</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Groupe  {#group}

Un objet Group représente un ensemble d’utilisateurs et d’équipes. Les groupes représentent souvent la structure du Ministère.

Pour plus d’informations sur les groupes, voir [Groupes par rapport aux équipes dans Adobe Workfront](../../people-teams-and-groups/work-with-groups-and-teams/understanding-differences-and-similarities-between-groups-and-teams.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Actions</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>getParents</b> </p> <p>Cette action renvoie un tableau des groupes parents du groupe (groupes dont le groupe donné est un sous-groupe).</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### JournalEntry {#journalentry}

L’objet JournalEntry peut être configuré pour consigner des informations sur des champs d’objet spécifiques chaque fois que ces champs sont modifiés. Lorsqu’un champ est configuré pour être consigné dans le cadre de l’objet d’entrée de journal, une entrée de journal correspondante est créée chaque fois que ce champ est modifié.

La ressource JournalEntry a ajouté l’indicateur REPORTABLE.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Champs directs</p> </td> 
   <td> <p>Les champs suivants ont supprimé l’indicateur NOT_GROUPABLE :</p> 
    <ul> 
     <li> <p><b>changeType</b> </p> </li> 
     <li> <p><b>entryDate</b> </p> </li> 
     <li> <p><b>fieldName</b> </p> </li> 
     <li> <p><b>objObjCode</b> </p> </li> 
    </ul> <p>Les champs suivants ont ajouté l’indicateur NOT_FILTERABLE :</p> 
    <ul> 
     <li> <p><b>subObjCode</b> </p> </li> 
     <li> <p><b>subObjID</b> </p> </li> 
     <li> <p><b>topObjCode</b> </p> </li> 
     <li> <p><b>topObjID</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### LayoutTemplate {#layouttemplate}

Les administrateurs d’Adobe Workfront ou les administrateurs de groupe peuvent créer des modèles pour personnaliser les éléments de mise en page dans Adobe Workfront. L’objet LayoutTemplate est spécifique à Adobe Workfront Classic.

Pour l’objet qui représente les modèles de mise en page dans la nouvelle expérience Adobe Workfront, voir [UITemplate](#uitemplate)

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Champs directs</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>Description</b> </p> <p>Ajout du programme de validation MAX_LENGTH, qui spécifie que la longueur de la description ne dépasse pas 4 000 caractères.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### LinkedFolder {#linkedfolder}

Un objet LinkedFolder représente un dossier lié à un fournisseur de documents externe, tel que Google Drive ou Dropbox.

Pour plus d’informations sur les dossiers liés, voir [Liaison de documents à partir d’applications externes](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Champs directs</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>externalIntegrationType</b> </p> <p>Ajout de la valeur possible :</p> 
      <ul> 
       <li> <p>AEM (Adobe Experience Manager)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### TâcheOp {#optask}

Un objet OpTask est généralement appelé Problème. Un problème est un élément de travail qui indique généralement qu’un problème empêche la réalisation d’une tâche ou d’un projet. Il peut également s’agir d’une demande de service d’assistance. Modifier les commandes, les requêtes et les bogues sont également des problèmes.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Champs de recherche</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>favoritedByUsersMM</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Projet {#project}

Les projets sont des éléments de travail dans Workfront et sont une composante essentielle de la façon dont Workfront aide les personnes à travailler. Un objet Projet représente un groupe de tâches avec un objectif commun et spécifique.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Champs directs</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>convertiOpTaskOriginatorID</b> </p> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Removed flag NOT&nbsp;FILTERABLE</p>
      --> </li> 
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
   <td> <p>Champs directs</p> </td> 
   <td> <p>Les champs suivants ont été ajoutés à la ressource ProofApproval .</p> 
    <ul> 
     <li> <p><b>approverStage</b> </p> </li> 
     <li> <p><b>DecisionDate</b> </p> </li> 
     <li> <p><b>workflowTemplate</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### QueueDef {#queuedef}

Un objet QueueDef représente une file d’attente, qui est un projet qui a été publié dans la zone Aide Desk pour permettre aux utilisateurs de lui envoyer des problèmes.

Pour plus d’informations sur les files d’attente de requête, voir [Création d’une file d’attente de requête](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Champs directs</td> 
   <td> 
    <ul> 
     <li> <p><b>documentPosition</b> </p> <p>Ajout de . Les valeurs possibles sont les suivantes :</p> 
      <ul> 
       <li> <p>0 (après les formulaires personnalisés)</p> </li> 
       <li> <p>1 (Avant les formulaires personnalisés)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Tâche {#task}

Un objet Task représente un élément de travail qui doit être exécuté comme une étape vers l’atteinte d’un objectif final (achèvement d’un projet).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Champs de recherche</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>favoritedByUsersMM</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Équipe {#team}

Un objet Équipe est un ensemble d’utilisateurs pouvant être affectés à un élément de travail.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Champs directs</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Ce champ a été ajouté. Il s’agit d’un paramètre booléen dont la valeur est true si un objet est principal et false dans le cas contraire. Les objets définis sur Principal apparaissent dans les menus déroulants et les champs de type avant et peuvent être associés à d’autres objets. Les objets qui ne sont pas définis sur Principal ne sont pas visibles dans les menus déroulants et les champs de type devant à associer à d’autres objets.  </p> </li> 
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

### Feuille de temps {#timesheet}

Un objet de feuille de temps représente une feuille de temps virtuelle qui permet aux utilisateurs de saisir les heures réelles travaillées pour les tâches, les projets et les types d’heures de surcharge.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Champs directs</td> 
   <td> 
    <ul> 
     <li> <p><b>isOvertimeDisabled</b> </p> <p>Ajouté(e)(s)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Champs principaux</td> 
   <td> 
    <ul> 
     <li> <p><b>objCode</b> </p> <p>Supprimé</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### TimesheetProfile {#timesheetprofile}

Un objet de feuille de temps représente une feuille de temps virtuelle qui permet aux utilisateurs de saisir les heures réelles travaillées pour les tâches, les projets et les types d’heures de surcharge.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Champs directs</td> 
   <td> 
    <ul> 
     <li> <p><b>isOvertimeDisabled</b> </p> <p>Ajouté(e)(s)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Champs par défaut</td> 
   <td> 
    <ul> 
     <li> <p><b>isOvertimeDisabled</b> </p> <p>Ajouté(e)(s)</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### UITemplate {#uitemplate}

Les administrateurs d’Adobe Workfront ou les administrateurs de groupe peuvent créer des modèles pour personnaliser les éléments de mise en page dans Adobe Workfront. L’objet UITemplate est spécifique à la nouvelle expérience Adobe Workfront.

Pour l’objet qui représente les modèles de mise en page dans Adobe Workfront Classic, voir [LayoutTemplate](#layouttemplate).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Actions</td> 
   <td> <p>Les actions suivantes ont été ajoutées à la ressource UEMemplate.</p> 
    <ul> 
     <li> <p><b>migrateCustomersAllLayoutTemplates</b> </p> <p>Prend l’argument :</p> 
      <ul> 
       <li> <p>overrideIfExists (boolean)</p> </li> 
      </ul> </li> 
     <li> <p><b>migrateLayoutTemplates</b> </p> <p>Prend les arguments :</p> 
      <ul> 
       <li> <p>layoutTemplateIDs (string[])</p> </li> 
       <li> <p>overrideIfExists (boolean)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### UserDelegation {#userdelegation}

Un objet UserDelegation représente le fait de déléguer le travail d’un utilisateur à un autre pendant une période donnée.

L’objet UserDelegation a ajouté l’indicateur REPORTABLE.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Champs directs</td> 
   <td> <p>Les champs suivants ont supprimé l’indicateur NOT_GROUPABLE</p> 
    <ul> 
     <li> <p><b>endDate</b> </p> </li> 
     <li> <p><b>startDate</b> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Champs par défaut</td> 
   <td> <p>Les champs suivants ont été ajoutés :</p> 
    <ul> 
     <li> <p><b>endDate</b> </p> </li> 
     <li> <p><b>startDate</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Travail  {#work}

Un objet de travail est une interface commune dont Task et OpTask héritent tous deux et partagent le code commun entre les deux.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Champs de recherche</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>favoritedByUsersMM</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
