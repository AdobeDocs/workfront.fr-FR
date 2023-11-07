---
content-type: api
navigation-topic: api-navigation-topic
title: Nouveautés de l’API version 12
description: 'Workfront a publié l’API version 12 le 12 novembre 2020. L’API version 12 comprend les modifications suivantes de la version 11 :'
author: Becky
feature: Workfront API
role: Developer
exl-id: 1ffba3b5-ab24-4ca2-a1ef-f7e5b77e776c
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '2516'
ht-degree: 2%

---

# Nouveautés de l’API version 12

Workfront a publié l’API version 12 le 12 novembre 2020. L’API version 12 comprend les modifications suivantes de la version 11 :

## Ajout de ressources

Les ressources suivantes sont nouvelles dans l’API Workfront version 12.

* [BreadCrumb](#breadcrumb)
* [RichTextParameterValue](#richtextparametervalue)

### BreadCrumb {#breadcrumb}

Un objet BreadCrumb représente un élément dans la hiérarchie parent/enfant d’un élément de travail Adobe Workfront. Les chemins de navigation indiquent comment un élément de travail s’intègre à la plus grande structure de Portfolios, de projets, de projets et de tâches.

Pour plus d’informations sur les chemins de navigation dans Workfront, voir [Présentation du chemin de navigation dans la nouvelle expérience Adobe Workfront](../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md)

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>Action</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">getObjectHierarchy</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### RichTextParameterValue {#richtextparametervalue}

Les champs de texte enrichi sont désormais disponibles pour d’autres objets. L’objet RichTextParameterValue a été ajouté à Workfront pour prendre en charge cette disponibilité.

Pour plus d’informations, voir [Champs de texte enrichi dans l’API Adobe Workfront](../../wf-api/general/rich-text-field-api.md).

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
     <li style="font-weight: bold;">ID</li> 
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

## Ressources supprimées

Aucune ressource n’a été supprimée pour l’API version 12.

## Ressources modifiées

Les ressources suivantes ont été modifiées pour l’API Workfront version 12.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> 
    <ul> 
     <li> <p><a href="#accesslevel" class="MCXref xref">AccessLevel</a> </p> </li> 
     <li> <p><a href="#accesslevelpermissions" class="MCXref xref">AccessLevelPermissions</a> </p> </li> 
     <li> <p><a href="#accessrequest" class="MCXref xref">AccessRequest</a> </p> </li> 
     <li> <p><a href="#accessrule" class="MCXref xref">AccessRule</a> </p> </li> 
     <li> <p><a href="#activitylog" class="MCXref xref">ActivityLog</a> </p> </li> 
     <li> <p><a href="#announcementattachment" class="MCXref xref">AnnonceAttachment</a> </p> </li> 
     <li> <p><a href="#approval" class="MCXref xref">Approbation</a> </p> </li> 
     <li> <p><a href="#calendarsection" class="MCXref xref">Section du calendrier</a> </p> </li> 
     <li> <p><a href="#company" class="MCXref xref">Entreprise</a> </p> </li> 
     <li> <p><a href="#customer" class="MCXref xref">Client</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="#customerpreferences" class="MCXref xref">CustomerPreferences</a> </p> </li> 
     <li> <p><a href="#document" class="MCXref xref">Document</a> </p> </li> 
     <li> <p><a href="#documentversion" class="MCXref xref">DocumentVersion</a> </p> </li> 
     <li> <p><a href="#group" class="MCXref xref">Groupe </a> </p> </li> 
     <li> <p><a href="#linkedfolder" class="MCXref xref">LinkedFolder</a> </p> </li> 
     <li> <p><a href="#optask" class="MCXref xref">TâcheOp</a> </p> </li> 
     <li> <p><a href="#parameter" class="MCXref xref">Paramètre</a> </p> </li> 
     <li> <p><a href="#portfolio" class="MCXref xref">Portfolio</a> </p> </li> 
     <li> <p><a href="#program" class="MCXref xref">Programme</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="#queuedef" class="MCXref xref">QueueDef</a> </p> </li> 
     <li> <p><a href="#scheduledreport" class="MCXref xref">ScheduledReport</a> </p> </li> 
     <li> <p><a href="#scorecardquestion" class="MCXref xref">ScoreCardQuestion</a> </p> </li> 
     <li> <p><a href="#task" class="MCXref xref">Tâche</a> </p> </li> 
     <li> <p><a href="#team" class="MCXref xref">Équipe</a> </p> </li> 
     <li> <p><a href="#templatetask" class="MCXref xref">TemplateTask</a> </p> </li> 
     <li> <p><a href="#timesheet" class="MCXref xref">Feuille de temps</a> </p> </li> 
     <li> <p><a href="#user" class="MCXref xref">l’utilisateur ou de l’utilisatrice</a> </p> </li> 
     <li> <p><a href="#work" class="MCXref xref">Travail </a> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

 

### AccessLevel {#accesslevel}

Un objet AccessLevel est associé à des utilisateurs et décrit le jeu d’autorisations AccessLevel qui déterminent ce à quoi l’utilisateur peut accéder.

Pour plus d’informations sur les niveaux d’accès, voir [Fonctionnement des niveaux d’accès](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels.md).

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> <!--
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Direct Fields</td>
   --> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">fieldAccessPrivileges</p>
      --> <!--
       <p style="font-weight: normal;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Added the possible value CPJ (Copy). This allows Users with Planner Access Level to copy Projects.</p>
      --> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AccessLevelPermissions {#accesslevelpermissions}

Un objet AccessLevelPermissions représente une autorisation spécifique d’accès, de création ou de modification d’un objet Workfront. Ces autorisations peuvent ensuite être associées à un niveau d’accès.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Champs directs</td> 
   <td> 
    <ul> 
     <li> <p><strong>coreAction</strong> </p> <p>Ajout des valeurs possibles suivantes :</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> <p>Un utilisateur disposant d’un niveau d’accès incluant cette autorisation peut mettre à jour les heures planifiées dans l’équilibreur de charge de travail.</p> <p>Pour plus d’informations, voir <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">Mettre à jour les heures planifiées de la tâche lors de la gestion des affectations utilisateur</a> in <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Gestion des affectations utilisateur dans l’équilibreur de charge de travail</a>.</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> <p>Un utilisateur disposant d’un niveau d’accès incluant cette autorisation peut ajouter des champs aux formulaires personnalisés.</p> <p>Pour plus d’informations, voir <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#add2" class="MCXref xref"></a> in <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Création ou modification d’un formulaire personnalisé</a>.</p> </li> 
       <li> <p>EDIT_SYSTEM_WIDE </p> <p>Un utilisateur disposant d’un niveau d’accès incluant cette autorisation peut partager un champ personnalisé à l’échelle du système avec l’accès Supprimer .</p> <p>Pour plus d’informations, voir <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">Configuration du partage pour les champs et widgets personnalisés</a>.</p> </li> 
      </ul> </li> 
     <li> <p><strong>forbiddenActions</strong> </p> <p>Ajout des valeurs possibles suivantes :</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> </li> 
       <li> <p>EDIT_SYSTEM_WIDE </p> </li> 
      </ul> </li> 
     <li> <p><strong>secondaryActions</strong> </p> <p>Ajout des valeurs possibles suivantes :</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> </li> 
       <li> <p>EDIT_SYSTEM_WIDE </p> </li> 
      </ul> </li> 
    </ul> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">OR</p>
    --> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The following fields added the possible value PLANNED_HOURS_CONTOURING, which allows a user to update planned hours in the Workload Balancer</p>
    --> 
    <ul> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">coreAction</p>
      --> </li> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">forbiddenActions</p>
      --> </li> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">secondaryActions</p>
      --> </li> 
    </ul> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The following fields added the possible value ADD_TO_CUSTOM_FORMS, which allows a user to add fields to custom forms.</p>
    --> 
    <ul> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">coreAction</p>
      --> </li> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">forbiddenActions</p>
      --> </li> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">secondaryActions</p>
      --> </li> 
    </ul> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The following fields added the possible value EDIT_SYSTEMWIDE, which allows a user to share a custom field system-wide with Delete access. </p>
    --> <!--
     <ul data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
      <li> <p>coreAction</p> </li> 
      <li> <p>forbiddenActions</p> </li> 
      <li> <p>secondaryActions</p> </li> 
     </ul>
    --> </td> 
  </tr> 
 </tbody> 
</table>

### AccessRequest {#accessrequest}

Si un utilisateur n’a pas accès à un objet Workfront dont il a besoin, il peut demander l’accès à cet objet. L’objet AccessRequest représente cette requête.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Champs directs</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">action</p> <p>Ajout des valeurs possibles suivantes :</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> <p>Un utilisateur disposant d’un niveau d’accès incluant cette autorisation peut mettre à jour les heures planifiées dans l’équilibreur de charge de travail.</p> <p>Pour plus d’informations, voir <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">Mettre à jour les heures planifiées de la tâche lors de la gestion des affectations utilisateur</a> in <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Gestion des affectations utilisateur dans l’équilibreur de charge de travail</a>.</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> <p>Un utilisateur disposant d’un niveau d’accès incluant cette autorisation peut ajouter des champs aux formulaires personnalisés.</p> <p>Pour plus d’informations, voir <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#add2" class="MCXref xref"></a> in <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Création ou modification d’un formulaire personnalisé</a>.</p> </li> 
       <li> <p>EDIT_SYSTEM_WIDE </p> <p>Un utilisateur disposant d’un niveau d’accès incluant cette autorisation peut partager un champ personnalisé à l’échelle du système avec l’accès Supprimer .</p> <p>Pour plus d’informations, voir <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">Configuration du partage pour les champs et widgets personnalisés</a>.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AccessRule {#accessrule}

Un objet AccessRule représente un jeu de règles dans les niveaux d’accès personnalisés qui détermine comment les utilisateurs peuvent partager les projets qu’ils créent.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Champs directs</td> 
   <td> 
    <ul> 
     <li><strong>coreAction</strong> <p>Ajout des valeurs possibles suivantes :</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> <p>Un utilisateur disposant d’un niveau d’accès incluant cette autorisation peut mettre à jour les heures planifiées dans l’équilibreur de charge de travail.</p> <p>Pour plus d’informations, voir <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">Mettre à jour les heures planifiées de la tâche lors de la gestion des affectations utilisateur</a> in <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Gestion des affectations utilisateur dans l’équilibreur de charge de travail</a>.</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> <p>Un utilisateur disposant d’un niveau d’accès incluant cette autorisation peut ajouter des champs aux formulaires personnalisés.</p> <p>Pour plus d’informations, voir <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#add2" class="MCXref xref"></a> in <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Création ou modification d’un formulaire personnalisé</a>.</p> </li> 
       <li> <p>EDIT_SYSTEM_WIDE </p> <p>Un utilisateur disposant d’un niveau d’accès incluant cette autorisation peut partager un champ personnalisé à l’échelle du système avec l’accès Supprimer .</p> <p>Pour plus d’informations, voir <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">Configuration du partage pour les champs et widgets personnalisés</a>.</p> </li> 
      </ul> </li> 
     <li> <p><strong>forbiddenActions</strong> </p> <p>Ajout des valeurs possibles suivantes :</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> </li> 
       <li> <p>EDIT_SYSTEM_WIDE </p> </li> 
      </ul> </li> 
     <li> <p><strong>secondaryActions</strong> </p> <p>Ajout des valeurs possibles suivantes :</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> </li> 
       <li> <p>EDIT_SYSTEM_WIDE </p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ActivityLog {#activitylog}

Un objet ActivityLog est une liste complète de toutes les activités qui ont eu lieu dans un compte de bon à tirer Workfront donné.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Opérations</p> </td> 
   <td> <p>L’opération suivante a été supprimée de l’objet ActivityLog :</p> 
    <ul> 
     <li> <p><strong>AJOUTER</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AnnonceAttachment {#announcementattachment}

Un objet AnnoncementAttachment représente un fichier joint à une annonce Workfront.

Pour plus d’informations sur les pièces jointes d’annonce, voir [Envoyer des annonces](../../administration-and-setup/get-started-wf-administration/view-send-announcements.md)

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Champs directs</p> </td> 
   <td> 
    <ul> 
     <li> <p><strong>fileExtension</strong> </p> <p>Ajout des valeurs possibles :</p> 
      <ul> 
       <li> <p>qdoc (enum.fileextension.qdoc)</p> </li> 
       <li> <p>qdiapas (enum.fileextension.qdiapas)</p> </li> 
       <li> <p>qsheet (enum.fileextension.qsheet)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Approbation {#approval}

Un élément de travail donné, tel qu’une tâche, un document ou une feuille de temps, peut exiger qu’un superviseur ou un autre utilisateur signe l’élément de travail. Un objet Approval représente l’action de déconnexion d’un élément de travail.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Champs directs</td> 
   <td> 
    <ul> 
     <li> <p><strong>backlogOrder</strong> </p> <p>Suppression des indicateurs suivants :</p> 
      <ul> 
       <li> <p>DYNAMIC,</p> </li> 
       <li> <p>LAZY_READ,</p> </li> 
       <li> <p>NOT_GROUPABLE</p> </li> 
      </ul> </li> 
     <li> <p><strong>groupID</strong> </p> <p>Ajout des indicateurs suivants</p> 
      <ul> 
       <li> <p>AUTO_LOAD,</p> </li> 
       <li> <p>DYNAMIC,</p> </li> 
       <li> <p>READ_ONLY</p> </li> 
      </ul> </li> 
     <li> <p><strong>workEffort</strong> </p> <p>Ce champ a été ajouté et indique si l’utilisateur doit faire un petit, moyen ou un gros effort quotidien pour terminer une tâche. Les valeurs possibles sont les suivantes :</p> 
      <ul> 
       <li> <p>1 (Petit)</p> </li> 
       <li> <p>2 (Moyen)</p> </li> 
       <li> <p>3 (Grand)</p> </li> 
      </ul> <p>Pour plus d’informations sur l’effort de travail dans Workfront, voir <a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Présentation de l’effort de travail</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Section du calendrier {#calendarsection}

Une section de calendrier est un rapport de calendrier.

Pour plus d’informations sur les rapports de calendrier, voir [Présentation des rapports sur les calendriers](../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Champs directs</td> 
   <td> <p style="font-weight: normal;">Les champs suivants ont été ajoutés à l’objet CalendarSection pour prendre en charge la nouvelle fonctionnalité d’utilisation de dates personnalisées dans les rapports de calendrier. </p> <p style="font-weight: normal;">Pour plus d’informations, voir <a href="../../reports-and-dashboards/reports/calendars/use-custom-dates.md" class="MCXref xref">Utilisation de champs de date personnalisés dans un rapport de calendrier</a>.</p> 
    <ul> 
     <li> <p style="font-weight: normal;">customDate</p> </li> 
     <li> <p style="font-weight: normal;">customEndDateParameterID</p> </li> 
     <li> <p style="font-weight: normal;">customStartDateParameterID</p> </li> 
     <li> <p style="font-weight: normal;">ignoreCurrentDates</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Entreprise {#company}

Un objet Société représente une organisation composée d’un ensemble de personnes.

Pour plus d’informations sur les entreprises, voir [Création et modification d’entreprises](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Champs directs</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">Identifiant du groupe auquel l’entreprise est associée.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Champs de référence</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupe</p> <p style="font-weight: normal;">Groupe auquel l’entreprise est associée. L’association d’une société à un groupe permet à l’administrateur du groupe d’étendre l’accès et les autorisations au groupe.</p> </li> 
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
  <tr> 
   <td>Actions</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: normal;"><strong>productEnabled</strong> </p> <p style="font-weight: normal;">Cette action prend un argument CustomerProductTypeEnum et renvoie une valeur booléenne qui indique si ce client possède un compte pour ce produit. </p> </li> 
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
       <li style="font-weight: normal;">password:zoomIntegrationEnabled (Activer l’intégration de zoom dans le flux de mises à jour)</li> 
       <li style="font-weight: normal;"> password:quipIntegrationEnabled (config.general.quip.enabled)  </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Document {#document}

Un objet Document représente un fichier (tel que du matériel écrit, des images ou d’autres formes d’informations).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Actions</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>createLinkedProofVersion</p> <p style="font-weight: normal;">Ajouté(e)(s)</p> </li> 
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
   <td>Champs directs</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>externalIntegrationType</p> <p style="font-weight: normal;">Suppression de la valeur possible :</p> 
      <ul> 
       <li style="font-weight: normal;">QUIP (Quip)</li> 
      </ul> </li> 
    </ul> 
    <ul> 
     <li> <p style="font-weight: normal;"><strong>proofDecision</strong> </p> <p>Ajouté(e)(s)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Actions</td> 
   <td> <p>Les actions suivantes ont été ajoutées à l’objet Document .</p> 
    <ul> 
     <li> <p style="font-weight: bold;">getDocumentReviewerDecision</p> <p style="font-weight: normal;">Cette action prend l’argument documentVersonID (chaîne) et renvoie un mappage qui indique la décision du réviseur.</p> </li> 
     <li style="font-weight: bold;"> <p>setDocumentReviewerDecision</p> <p style="font-weight: normal;">Cette action utilise les arguments suivants :</p> 
      <ul style="font-weight: normal;"> 
       <li> <p>documentVersionID (string)</p> </li> 
       <li> <p>reviewerDecision (string)</p> </li> 
       <li> <p>comment (string)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Groupe  {#group}

Un objet Group représente un ensemble d’utilisateurs et d’équipes. Les groupes représentent souvent la structure du Ministère.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Champs directs</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>businessLeaderID</p> <p style="font-weight: normal;">Identifiant du chef d’entreprise affecté au groupe.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Champs de référence</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>businessLeader</p> <p style="font-weight: normal;">Chef d’entreprise affecté au groupe. Un chef d’entreprise est quelqu’un qui prend des décisions commerciales pour le groupe.</p> <p style="font-weight: normal;">Pour plus d’informations sur les chefs d’entreprise, voir <a href="../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref">Présentation des chefs d’entreprise</a>.<br></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Actions</td> 
   <td> 
    <ul> 
     <li> <p><strong>assignMultiple</strong> </p> <p>Cette action utilise les arguments suivants :</p> 
      <ul> 
       <li> <p>userIDs (string[])</p> </li> 
       <li> <p>roleIDs (string[])</p> </li> 
       <li> <p>TeamID (string)</p> </li> 
      </ul> </li> 
     <li> <p><strong>getGroupMembers</strong> </p> </li> 
     <li> <p><strong>updateMembersList</strong> </p> <p>Cette action utilise les arguments suivants :</p> 
      <ul> 
       <li> <p>newMemberIDs (string[])</p> </li> 
       <li> <p>removeMemberDs (string[])</p> </li> 
      </ul> </li> 
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
     <li style="font-weight: bold;"> <p>externalIntegrationType</p> <p style="font-weight: normal;">Suppression de la valeur possible :</p> 
      <ul> 
       <li style="font-weight: normal;">QUIP (Quip)</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### TâcheOp {#optask}

Un objet OpTask est généralement appelé Problème. Un problème est un élément de travail qui indique généralement qu’un problème empêche la réalisation d’une tâche ou d’un projet. Il peut également s’agir d’une demande de service d’assistance. Modifier les commandes, les requêtes et les bogues sont également des problèmes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Champs directs</p> </td> 
   <td> 
    <ul> 
     <li> <p><strong>backlogOrder</strong> </p> <p>La commande indique la position d’une tâche ou d’une histoire sur le journal Agile.</p> <p>Ce champ a supprimé les indicateurs suivants :
       <ul>
        <li>DYNAMIC,</li>
        <li>LAZY_READ,</li>
        <li>NOT_GROUPABLE :</li>
       </ul></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Actions</td> 
   <td> <p>Ces actions ont ajouté l’état de l’argument pour prendre en charge la nouvelle fonctionnalité du bouton Démarrer , qui modifie l’état d’un élément de travail lorsqu’un utilisateur clique sur le bouton pour indiquer qu’il a commencé à travailler sur l’élément.</p> <p>Pour plus d’informations, voir <a href="../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Remplacez le bouton Travailler dessus par un bouton Démarrer</a>.</p> 
    <ul> 
     <li> <p><strong>acceptWork</strong> </p> </li> 
     <li> <p><strong>unacceptWork</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Paramètre {#parameter}

Un objet de paramètre est un champ personnalisé.

La ressource Paramètre a ajouté l’indicateur SHARABLE.

Pour plus d’informations sur les champs personnalisés, voir [Création ou modification d’un formulaire personnalisé](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#create) in [Création ou modification d’un formulaire personnalisé](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Champs directs</td> 
   <td> 
    <ul> 
     <li> <p><strong>dataType</strong> </p> <p>Ajout de la valeur possible :</p> 
      <ul> 
       <li> <p>RICH (texte enrichi)</p> <p>Pour plus d’informations, voir <a href="../../wf-api/general/rich-text-field-api.md" class="MCXref xref">Champs de texte enrichi dans l’API Adobe Workfront</a>.</p> </li> 
      </ul> </li> 
     <li> <p><strong>displayType</strong> </p> <p>Ajout de la valeur possible :</p> 
      <ul> 
       <li> <p>RICH (champ de texte avec mise en forme)</p> <p>Pour plus d’informations, voir <a href="../../wf-api/general/rich-text-field-api.md" class="MCXref xref">Champs de texte enrichi dans l’API Adobe Workfront</a>.</p> </li> 
      </ul> </li> 
     <li> <p><strong>label</strong> </p> <p>Ajouté(e)(s)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Champs de collection</td> 
   <td> 
    <ul> 
     <li> <p><strong>accessRules</strong> </p> <p>Ajouté(e)(s)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Champs par défaut</td> 
   <td> 
    <ul> 
     <li> <p class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"><strong>label</strong> </p> <p>Ajouté(e)(s)</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Portfolio {#portfolio}

Un objet de Portfolio est un ensemble de projets qui rivalisent pour les mêmes ressources, généralement de l’argent ou des personnes pour les compléter.

Pour plus d’informations sur les portefeuilles, voir [Présentation des Portfolios dans Adobe Workfront](../../manage-work/portfolios/portfolios-overview/portfolio-overview.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Champs directs</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">Identifiant du groupe auquel le portfolio est associé.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Champs de référence</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupe</p> <p style="font-weight: normal;">Groupe auquel le portfolio est associé. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Programme {#program}

Un objet de programme est un sous-ensemble de projets d’un portfolio, où des projets similaires peuvent être regroupés.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Champs directs</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">Identifiant du groupe auquel le programme est associé.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Champs de référence</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupe</p> <p style="font-weight: normal;">Groupe auquel le programme est associé. </p> </li> 
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
     <li><strong>requestorCoreAction</strong> <p>Ajout des valeurs possibles suivantes :</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> <p>Un utilisateur disposant d’un niveau d’accès incluant cette autorisation peut mettre à jour les heures planifiées dans l’équilibreur de charge de travail.</p> <p>Pour plus d’informations, voir <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">Mettre à jour les heures planifiées de la tâche lors de la gestion des affectations utilisateur</a> in <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Gestion des affectations utilisateur dans l’équilibreur de charge de travail</a>.</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> <p>Un utilisateur disposant d’un niveau d’accès incluant cette autorisation peut ajouter des champs aux formulaires personnalisés.</p> <p>Pour plus d’informations, voir <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#add2" class="MCXref xref"></a> in <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Création ou modification d’un formulaire personnalisé</a>.</p> </li> 
       <li> <p>EDIT_SYSTEM_WIDE </p> <p>Un utilisateur disposant d’un niveau d’accès incluant cette autorisation peut partager un champ personnalisé à l’échelle du système avec l’accès Supprimer .</p> <p>Pour plus d’informations, voir <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">Configuration du partage pour les champs et widgets personnalisés</a></p> </li> 
      </ul> <li> <p><strong>requestorForbiddenActions</strong> </p> <p>Ajout des valeurs possibles suivantes :</p> 
       <ul> 
        <li> <p>PLANNED_HOURS_CONTOURING </p> </li> 
        <li> <p>ADD_TO_CUSTOM_FORMS </p> </li> 
        <li> <p>EDIT_SYSTEM_WIDE </p> </li> 
       </ul> </li> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ScheduledReport {#scheduledreport}

Un objet ScheduledReport représente un rapport qui a été configuré pour être distribué.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Champs directs</td> 
   <td> 
    <ul> 
     <li> <p><strong>format</strong> </p> <p>Ajout des valeurs possibles :</p> 
      <ul> 
       <li> <p>qdoc (enum.fileextension.qdoc)</p> </li> 
       <li> <p>qdiapas (enum.fileextension.qdiapas)</p> </li> 
       <li> <p>qsheet (enum.fileextension.qsheet)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ScoreCardQuestion {#scorecardquestion}

Un objet ScoreCardQuestion représente une question qui a été ajoutée à une Fiche d’évaluation. Ces questions sont généralement définies par le responsable du Portfolio et leurs réponses permettent au responsable de comprendre dans quelle mesure un projet s’aligne sur les objectifs du portefeuille.

Pour plus d’informations sur les questions de la Fiche d’évaluation, voir [Création d’une Fiche d’évaluation](../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Champs directs</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>displayType</p> <p style="font-weight: normal;">Ajout de la valeur possible RICH (Champ de texte avec mise en forme). </p> <p style="font-weight: normal;">Pour plus d’informations, voir <a href="../../wf-api/general/rich-text-field-api.md" class="MCXref xref">Champs de texte enrichi dans l’API Adobe Workfront</a>.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Tâche {#task}

Un objet Task représente un élément de travail qui doit être exécuté comme une étape vers l’atteinte d’un objectif final (achèvement d’un projet).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Champs directs</td> 
   <td> 
    <ul> 
     <li> <p><strong>workEffort</strong> </p> <p>Ce champ a été ajouté et indique si l’utilisateur doit faire un petit, moyen ou un gros effort quotidien pour terminer une tâche. Les valeurs possibles sont les suivantes :</p> 
      <ul> 
       <li> <p>1 (Petit)</p> </li> 
       <li> <p>2 (Moyen)</p> </li> 
       <li> <p>3 (Grand)</p> </li> 
      </ul> <p>Pour plus d’informations sur l’effort de travail dans Workfront, voir <a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Présentation de l’effort de travail</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Actions</td> 
   <td> <p>Ces actions ont ajouté l’état de l’argument pour prendre en charge la nouvelle fonctionnalité du bouton Démarrer , qui modifie l’état d’un élément de travail lorsqu’un utilisateur clique sur le bouton pour indiquer qu’il a commencé à travailler sur l’élément.</p> <p>Pour plus d’informations, voir <a href="../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Remplacez le bouton Travailler dessus par un bouton Démarrer</a>.</p> 
    <ul> 
     <li> <p><strong>acceptWork</strong> </p> </li> 
     <li> <p><strong>unacceptWork</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Équipe {#team}

Un objet Équipe est un ensemble d’utilisateurs pouvant être affectés à un élément de travail.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Champs directs</td> 
   <td> <p>Les champs suivants ont été ajoutés à la ressource Equipe :</p> 
    <ul> 
     <li> <p><strong>completeDaysOnKanbanBoard</strong> </p> <p>Ce champ représente le nombre de jours pendant lesquels une carte terminée reste sur le panorama Kanban.</p> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information, see <a href="../../agile/get-started-with-agile-in-workfront/configure-kanban.md" class="MCXref xref">Configure Kanban</a>.</p>
      --> </li> 
     <li> <p><strong>groupID</strong> </p> <p>Ce champ associe une équipe à un groupe. Cela identifie l’équipe comme faisant partie du groupe et permet à l’administrateur du groupe de gérer les équipes.</p> </li> 
     <li> <p><strong>workOnItStatusChange</strong> </p> <p>Il s’agit d’un paramètre booléen qui indique si le bouton Travailler dessus de l’équipe a été configuré comme un bouton Démarrer . Lorsqu’un membre de l’équipe clique sur un bouton Démarrer pour commencer le travail sur un élément de travail, l’état de l’élément passe de Nouveau à un état configuré dans les paramètres de l’équipe.</p> </li> 
     <li> <p>Les champs suivants vous permettent de spécifier des états personnalisés pour le bouton Démarrer sur les tâches individuelles.</p> 
      <ul> 
       <li> <p><strong>workOnItOpTaskBugReportStatuses</strong> </p> </li> 
       <li> <p><strong>workOnItOpTaskChangeOrderStatuses</strong> </p> </li> 
       <li> <p><strong>workOnItOpTaskIssueStatuses</strong> </p> </li> 
       <li> <p><strong>workOnItOpTaskRequestStatuses</strong> </p> <p><strong>workOnItTaskStatuses</strong> </p> </li> 
      </ul> <p>Pour plus d’informations sur le bouton Démarrer , voir <a href="../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Remplacez le bouton Travailler dessus par un bouton Démarrer</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Champs de référence</td> 
   <td> <p>Le champ suivant a été ajouté à la ressource Équipe :</p> 
    <ul> 
     <li> <p><strong>groupe</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### TemplateTask {#templatetask}

Un objet TemplateTask représente une tâche qui fait partie d’un modèle. Les tâches du modèle deviennent des tâches dans le projet où le modèle est utilisé.

Pour plus d’informations sur les tâches de modèle, voir [Modifier une tâche de modèle](../../manage-work/projects/create-and-manage-templates/edit-template-task.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Champs directs</td> 
   <td> 
    <ul> 
     <li> <p><strong>workEffort</strong> </p> <p>Ce champ a été ajouté et indique si l’utilisateur doit faire un petit, moyen ou un gros effort quotidien pour terminer une tâche. Les valeurs possibles sont les suivantes :</p> 
      <ul> 
       <li> <p>1 (Petit)</p> </li> 
       <li> <p>2 (Moyen)</p> </li> 
       <li> <p>3 (Grand)</p> </li> 
      </ul> <p>Pour plus d’informations sur l’effort de travail dans Workfront, voir <a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Présentation de l’effort de travail</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Feuille de temps {#timesheet}

Un objet de feuille de temps représente une feuille de temps virtuelle qui permet aux utilisateurs de saisir les heures réelles travaillées pour les tâches, les projets et les types d’heures de surcharge.

Pour plus d’informations sur les feuilles de calcul, voir [Présentation des feuilles de calcul](../../timesheets/timesheets/timesheets-overview.md)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Champs principaux</td> 
   <td> <p>Le champ suivant a été supprimé de la ressource Feuille de calcul :</p> 
    <ul> 
     <li> <p><strong>objcode</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Mettre à jour

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Champs directs</td> 
   <td> 
    <ul> 
     <li> <p><strong>updateType</strong> </p> <p>Ajout des valeurs possibles suivantes :</p> 
      <ul> 
       <li> <p>initiativeAdd (enum.updatetypeenum.initiativeadd)</p> </li> 
       <li> <p>initiativeEdit (enum.updatetypeenum.initiativeedit)</p> </li> 
      </ul> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Pour plus d’informations sur les initiatives, voir <a href="../../scenario-planner/initiatives-overview.md" class="MCXref xref">Présentation des initiatives dans le planificateur de scénarios</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### l’utilisateur ou de l’utilisatrice {#user}

Un objet User représente une personne disposant d’un compte dans Workfront qui peut se connecter et interagir avec le système.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Champs directs</td> 
   <td> <p>Les champs suivants ont été ajoutés à la ressource Utilisateur :</p> 
    <ul> 
     <li> <p><strong>actualDeactivationDate</strong> </p> <p>Il s’agit de la date et de l’heure auxquelles un utilisateur a été désactivé.</p> <p>Pour plus d’informations sur les utilisateurs désactivés, voir <a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Désactivation ou réactivation d’un utilisateur</a>.</p> </li> 
     <li> <p><strong>alignAccessType</strong> </p> <p>Ce champ indique l’accès de l’utilisateur aux objectifs Workfront. Les valeurs possibles sont les suivantes :</p> 
      <ul> 
       <li> <p>Accès interdit</p> </li> 
       <li> <p>Afficher</p> </li> 
       <li> <p>Modifier</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Actions</td> 
   <td> <p>L’action suivante a été ajoutée à la ressource Utilisateur :</p> 
    <ul> 
     <li> <p><strong>getUserAccessPermissionsByCode</strong> </p> <p>Cette action utilise les arguments suivants :</p> 
      <ul> 
       <li> <p>ids (string)</p> </li> 
       <li> <p>objCode (string)</p> </li> 
      </ul> </li> 
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
   <td>Champs directs</td> 
   <td> 
    <ul> 
     <li> <p><strong>backlogOrder</strong> </p> <p>La commande indique la position d’une tâche ou d’une histoire sur le journal Agile.</p> <p>Ce champ a supprimé les indicateurs suivants :</p> 
      <ul> 
       <li> <p>DYNAMIC,</p> </li> 
       <li> <p>LAZY_READ,</p> </li> 
       <li> <p>NOT_GROUPABLE</p> </li> 
      </ul> </li> 
     <li> <p><strong>groupID</strong> </p> <p>Ce champ a ajouté les indicateurs suivants :</p> 
      <ul> 
       <li> <p>AUTO_LOAD,</p> </li> 
       <li> <p>DYNAMIC,</p> </li> 
       <li> <p>READ_ONLY</p> </li> 
      </ul> </li> 
     <li> <p><strong>workEffort</strong> </p> <p>Ce champ a été ajouté et indique si l’utilisateur doit faire un petit, moyen ou un gros effort quotidien pour terminer une tâche. Les valeurs possibles sont les suivantes :</p> 
      <ul> 
       <li> <p>1 (Petit)</p> </li> 
       <li> <p>2 (Moyen)</p> </li> 
       <li> <p>3 (Grand)</p> </li> 
      </ul> <p>Pour plus d’informations sur l’effort de travail dans Workfront, voir <a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Présentation de l’effort de travail</a>.</p> </li> 
    </ul> <p style="font-weight: normal;">  </p> </td> 
  </tr> 
 </tbody> 
</table>
