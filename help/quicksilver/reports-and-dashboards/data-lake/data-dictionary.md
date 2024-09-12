---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Dictionnaire de données Workfront Data Connect
description: Cette page contient des informations sur la structure et le contenu des données dans Workfront Data Connect.
author: Nolan
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: 57985404-554e-4289-b871-b02d3427aa5c
source-git-commit: c3e18716aa74ed91e21e542437a017586a58d0b3
workflow-type: tm+mt
source-wordcount: '4294'
ht-degree: 4%

---

# Dictionnaire de données Workfront Data Connect

Cette page contient des informations sur la structure et le contenu des données dans Workfront Data Connect.

>[!NOTE]
>
>Les données de Data Connect sont actualisées toutes les quatre heures, de sorte que les modifications récentes peuvent ne pas être immédiatement répercutées.

## Types de tableau

Il existe plusieurs types de tableau que vous pouvez utiliser dans Data Connect pour afficher vos données Workfront d’une manière optimale.

* **Table actuelle**

  Le tableau actuel reflète les données de la même manière qu’il existe dans Workfront, chaque objet et son état actuel. Il est toutefois possible de naviguer avec une latence beaucoup plus faible que dans Workfront.

* **Table d’événements**

  Le tableau Événement effectue le suivi de chaque enregistrement de modification dans Workfront : c’est-à-dire, chaque fois qu’un objet change d’état, un enregistrement est créé qui indique le moment où la modification a eu lieu, qui a apporté la modification et ce qui a été modifié. Par conséquent, ce tableau est utile pour les comparaisons de temps en temps. Ce tableau ne contient que les données des trois dernières années.

* **Table d&#39;historique quotidienne**

  Le tableau Historique quotidien offre une version abrégée du tableau Événement, dans la mesure où il indique l’état de chaque objet sur une base quotidienne plutôt que lors de chaque événement. Ce tableau est donc utile pour l’analyse des tendances.

<!-- Custom table -->

## Diagramme de relation d’entité

Les objets dans Workfront (et, par conséquent, dans votre lac de données Data Connect) sont définis non seulement par leurs valeurs individuelles, mais aussi par leurs relations avec d’autres objets. Le diagramme des relations d’entité ci-dessous fournit un mappage de haut niveau des relations d’objet dans Data Connect. Le diagramme peut être visualisé et téléchargé à l’aide du lien suivant :

[Diagramme de relation d’entité Data Connect](/help/quicksilver/reports-and-dashboards/data-lake/assets/Workfront-data-lake_entity-relationship-diagram.pdf)

>[!IMPORTANT]
>
>Le diagramme des relations d’entité est un travail en cours : il est donc destiné uniquement à des fins de référence et peut faire l’objet de modifications.

## Types de date

Un certain nombre d’objets date fournissent des informations sur le moment où des événements spécifiques se produisent.

* `DL_LOAD_TIMESTAMP` : Cette date est utilisée à des fins de référence interne et reflète le moment où les données ont été chargées dans la table Actuel, Événement ou Historique quotidien. Cette date ne doit pas être utilisée pour l’analyse des données et doit être supprimée pendant la phase bêta du lac de données Workfront.
* `CALENDAR_DATE` : cette date n’est présente que dans la table Historique quotidien. Ce tableau fournit un enregistrement de l’apparence des données à 11:59 UTC pour chaque date spécifiée dans `CALENDAR_DATE`.
* `BEGIN_EFFECTIVE_TIMESTAMP` : cette date est présente dans les tables Event (Événement) et Daily History (Historique quotidien) et enregistre exactement lorsqu’un enregistrement a changé _en_ la valeur qu’il possède dans la ligne actuelle.
* `END_EFFECTIVE_TIMESTAMP` : cette date est présente dans les tables Historique quotidien et Événement et enregistre exactement lorsqu’un enregistrement a changé _de_ la valeur de la ligne en cours à une valeur d’une autre ligne. Pour permettre entre les requêtes sur `BEGIN_EFFECTIVE_TIMESTAMP` et `END_EFFECTIVE_TIMESTAMP`, cette valeur n’est jamais nulle, même s’il n’y a pas de nouvelle valeur. Dans le cas où un enregistrement est toujours valide (c’est-à-dire que la valeur n’a pas changé), `END_EFFECTIVE_TIMESTAMP` aura une valeur de 2300-01-01.

## Table de terminologie

Le tableau suivant met en corrélation les noms d’objet dans Workfront (ainsi que leurs noms dans l’interface et l’API) avec leurs noms équivalents dans Data Connect.

<table>
  <thead>
    <tr>
        <th>Nom d’entité Workfront</th>
        <th>Références de l’interface</th>
        <th>Référence d’API | Libellé</th>
        <th>Tableaux de lac de données</th>
        <th>Champ de relation</th>
        <th>Table et champ de relation</th>
    </tr>
  </thead>
  <tbody>
    <tr>
        <td>Niveau d’accès</td>
        <td>Niveau d’accès</td>
        <td>ACSLVL | Niveau d’accès</td>
        <td>ACCESSLEVELS_CURRENT<br>ACCESSLEVELS_DAILY_HISTORY<br>ACCESSLEVELS_EVENT</td>
        <td>ACCESSLEVELID (self)<br>APPGLOBALID<br>LASTUPDATEDBYID<br>LEGACYACCESSLEVELID<br>OBJID<br>SYSID</td>
        <td>Self<br>Aucune relation ; utilisée à des fins d’application interne<br>USER_CURRENT | USERID<br>Non-relation ; utilisé à des fins d’application interne<br>ID de l’objet identifié dans le champ OBJCODE<br>Non-relation ; utilisé à des fins d’application interne.</td>
    </tr>
    <tr>
        <td>Règle d'accès</td>
        <td>Partager</td>
        <td>ACTRUL | Partager</td>
        <td>ACCESSRULES_CURRENT<br>ACCESSRULES_DAILY_HISTORY<br>ACCESSRULES_EVENT</td>
        <td>ACCESSORID <br>ACCESSRULEID (self) <br>ANCESTORID <br>LASTUPDATEDBYID <br>SECURITYOBJID <br>SYSID</td>
        <td>ID de l’objet identifié dans le champ ACCESSOROBJCODE<br>Self<br>ID de l’objet identifié dans le champ ANCESTOROBJCODE<br>USERS_CURRENT | USERID<br>Identifiant de l’objet identifié dans le champ SECURITYOBJCODE<br>Non-relation ; utilisé à des fins d’application interne.</td>
    </tr>
    <tr>
        <td>Chemin d’approbation</td>
        <td>Chemin d’approbation</td>
        <td>ARVPTH | Validation</td>
        <td>APPROVALPATHS_CURRENT<br>APPROVALPATHS_DAILY_HISTORY<br>APPROVALPATHS_EVENT</td>
        <td>APPROVALPATHID (self) <br>APPROVALPROCESSID <br>ENTEREDBYID <br>GLOBALPATHID <br>LASTUPDATEDBYID <br>SYSID</td>
        <td>Self<br>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>USERS_CURRENT | USERID<br>Non-relation ; utilisé à des fins d’application interne<br>USERS_CURRENT | USERID<br>Non-relation ; utilisé à des fins d’application interne</td>
    </tr>
    <tr>
        <td>Processus d’approbation</td>
        <td>Processus d’approbation</td>
        <td>ARVPRC | Processus d’approbation</td>
        <td>APPROVALPROCESSES_CURRENT<br>APPROVALPROCESSES_DAILY_HISTORY<br>APPROVALPROCESSES_EVENT</td>
        <td>APPROVALPROCESSID (self) <br>ENTEREDBYID <br>LASTUPDATEDBYID<br>SYSID</td>
        <td>Self<br>USERS_CURRENT | USERID<br>USERS_CURRENT | USERID<br>Non-relation ; utilisé à des fins d’application interne</td>
    </tr>
    <tr>
        <td>Étape d’approbation</td>
        <td>Étape d’approbation</td>
        <td>ARVSTP | Évaluation</td>
        <td>APPROVALSTEPS_CURRENT<br>APPROVALSTEPS_DAILY_HISTORY<br>APPROVALSTEPS_EVENT</td>
        <td>APPROVALPATHID <br>APPROVALSTEPID (self) <br>SYSID</td>
        <td>APPROVALPATHS_CURRENT | APPROVALPATHID<br>Self<br>Aucune relation ; utilisé à des fins d’application interne</td>
    </tr>
    <tr>
        <td>ApproverStatus</td>
        <td>Statut de l'approbateur</td>
        <td>ARVSTS | ApproverStatus</td>
        <td>APPROVERSTATUSES_CURRENT<br>APPROVERSTATUSES_DAILY_HISTORY<br>APPROVERSTATUSES_EVENT</td>
        <td>APPROVERSTATUSID (self)<br>APPROVABLEOBJID<br>APPROVALSTEPID<br>APPROVEDBYID <br>DELEGATEUSERID<br>LASTUPDATEDBYID <br>OPTASKID<br>OVERRIDENUSERID<br>PROJECTID<br>STEPAPPROVERID<br> SYSID<br>TASKID<br>WILDCARDUSERID</td>
        <td>Self<br>ID de l’objet identifié dans le champ APPROVABLEOBJCODE<br>APPROVALSTEPS_CURRENT | APPROVALSTEPID<br>USERS_CURRENT | USERID <br>USERS_CURRENT | USERID<br>USERS_CURRENT | USERID <br>OPTASKS_CURRENT | OPTASKID<br>USERS_CURRENT | USERID<br>PROJECTS_CURRENT | PROJECTID<br>USERS_CURRENT | USERID<br>Non-relation ; utilisé à des fins d’application interne<br>TASKS_CURRENT | TASKID<br>USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Affectation</td>
        <td>Affectation</td>
        <td>ASSGN | Attribution</td>
        <td>ASSIGNMENTS_CURRENT<br>ASSIGNMENTS_DAILY_HISTORY<br>ASSIGNMENTS_EVENT</td>
        <td>ASSIGNEDBYID<br>ASSIGNEDTOID<br>ASSIGNMENTID (self)<br>CATEGORYID<br>CLASSIFIERID<br>OPTASKID<br>PRIVATERATECARDID<br>PROJECTID<br>ROLEID<br>TASKID<br>TEAMID</td>
        <td>USER_CURRENT | USERID<br>USER_CURRENT | USERID<br>Self<br>CATEGORIES_CURRENE | CATEGORYID<br>Table de classificateur non prise en charge actuellement<br>OPTASK_CURRENT | OPTASKID<br>RATECARD_CURRENT | RATECARDID<br>PROJECT_CURRENT | PROJECTID<br>ROLE_CURRENT | ROLEID<br>TASK_CURRENT | TASKID<br>TEAM_CURRENT | TEAMID</td>
    </tr>
    <tr>
        <td>En attente d’approbation</td>
        <td>En attente d’approbation</td>
        <td>AWAPVL | En attente d’approbation</td>
        <td>AWAITINGAPPROVALS_CURRENT<br>AWAITINGAPPROVALS_DAILY_HISTORY<br>AWAITINGAPPROVALS_EVENT</td>
        <td>ACCESSREQUESTID<br>APPROVABLEID <br>APPROVERID <br>AWAITINGAPPROVALID (self) <br>DOCUMENTID <br>DOCUMENTVERSIONID<br>OPTASKID <br>PROJECTID <br>ROLEID <br>SUBMITTEDBYID <br>SYSID<br>TASKID {1 1}TEAMID <br>TIMESHEETID<br>USERID<br></td>
        <td>La table des demandes d’accès n’est pas actuellement prise en charge<br>Aucune relation ; utilisée à des fins d’application interne<br>USERS_CURRENT | USERID<br>Self<br>DOCUMENTS_CURRENT | DOCUMENTID<br>DOCUMENTVERSIONS_CURRENT | DOCUMENTVERSIONID<br>OPTASKS_CURRENT | OPTASKID<br>PROJECTS_CURRENT | PROJECTID<br>ROLES_CURRENT | ROLEID<br>USERS_CURRENT | USERID<br>Non-relation ; utilisé à des fins d’application interne<br>TASKS_CURRENT | TASKID<br>TEAMS_CURRENT | TEAMID<br>TIMESHEETS_CURRENT | TIMESHEETID<br>USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Niveau de référence</td>
        <td>Niveau de référence</td>
        <td>BLIN | Ligne de base</td>
        <td>BASELINES_CURRENT<br>BASELINES_DAILY_HISTORY<br>BASELINES_EVENT</td>
        <td>BASELINEID (self)<br>EXCHANGERATEID <br>PROJECTID <br>SYSID</td>
        <td>Self<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>PROJECTS_CURRENT | PROJECTID<br>Non-relation ; utilisé à des fins d’application interne</td>
    </tr>
    <tr>
        <td>Tâche de ligne de base</td>
        <td>Tâche de ligne de base</td>
        <td>BSTSK | Tâche de ligne de base</td>
        <td>BASELINETASKS_CURRENT<br>BASELINETASKS_DAILY_HISTORY<br>BASELINETASKS_EVENT</td>
        <td>BASELINEID<br>BASELINETASKID (self) <br>EXCHANGERATEID <br>PROJECTID <br>SYSID<br>TASKID</td>
        <td>BASELINES_CURRENT | BASELINEID<br>Self<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>PROJECTS_CURRENT | PROJECTID<br>Non-relation ; utilisé à des fins d’application interne<br>TASKS_CURRENT | TASKID</td>
    </tr>
    <tr>
        <td>Taux de facturation</td>
        <td>Taux ou taux de remplacement</td>
        <td>TAUX | Taux de facturation</td>
        <td>RATES_CURRENT<br>RATES_DAILY_HISTORY<br>RATES_EVENT</td>
        <td>ASSIGNMENTID<br>CLASSIFIERID<br>EXCHANGERATEID<br>NLBRCATEGORYID<br>NONLABORRESOURCEID<br>OBJID<br>PROJECTID <br>RATECARDID<br>RATEID (self)<br>ROLEID <br>SOURCERATECARDID <br>SYSISIGNMENTID D <br>TEMPLATEID<br>USERID</td>
        <td>ASSIGNMENTS_CURRENT | ASSIGNMENTID<br>La table des classifications n'est actuellement pas prise en charge<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>Table Catégorie de ressource non professionnelle non prise en charge actuellement<br>NONLABORRESOURCES_CURRENT | NONLABORRESOURCEID<br>ID de l’objet identifié dans le champ OBJCODE<br>PROJECTS_CURRENT | PROJECTID <br>RATECARD_CURRENT | RATECARDID<br>Self<br>ROLES_CURREND | ROLEID <br>RATECARD_CURRENT | RATECARDID <br>Non-relation ; utilisé à des fins d’application interne <br>TEMPLATES_CURRNT | TEMPLATEID<br>USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Enregistrement de facturation</td>
        <td>Enregistrement de facturation</td>
        <td>BILL | Enregistrement de facturation</td>
        <td>BILLINGRECORDS_CURRENT<br>BILLINGRECORDS_DAILY_HISTORY<br>BILLINGRECORDS_EVENT</td>
        <td>BILLINGRECORDID (self)<br>CATEGORYID<br>EXCHANGERATEID <br>INVOICEID <br>LASTUPDATEDBYID <br>PROJECTID <br>SYSID</td>
        <td>Self<br>CATEGORIES_CURRENT | CATEGORYID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID <br>La table des factures n'est actuellement pas prise en charge <br>USERS_CURRENT | USERID <br>PROJECTS_CURRENT | PROJECTID   <br> N’est pas une relation, utilisée à des fins d’application interne</td>
    </tr>
    <tr>
        <td>Réservation</td>
        <td>Réservation</td>
        <td>BOOKING | Réservation</td>
        <td>BOOKINGS_CURRENT<br>BOOKINGS_DAILY_HISTORY<br>BOOKINGS_EVENT</td>
        <td>BOOKINGID (self)<br>ENTEREDBYID<br>LASTUPDATEDBYID<br>NLBRCATEGORYID<br>NONLABORRESOURCEID<br>OBJID<br>PROJECTID<br>SYSID<br>TASKID<br>TEMPLATEID<br>TEMPLATEID 10}TOPOBJID<br></td>
        <td>Self<br>USERS_CURRENT | USERID<br>USERS_CURRENT | USERID<br>Table Catégorie de ressource non ouvrière non prise en charge actuellement<br>NONLABORRESOURCES_CURRENT | NONLABORRESOURCEID<br>ID de l’objet identifié dans le champ OBJOBJCODE<br>PROJECTS_CURRENT | PROJECTID <br>Non-relation ; utilisé à des fins d’application interne<br>TASKS_CURRENT | TASKID     <br>TEMPLATES_CURRENT | TEMPLATEID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID<br>Identifiant de l’objet identifié dans le champ TOPOBJCODE.</td>
    </tr>
    <tr>
        <td>Catégorie</td>
        <td>Formulaire personnalisé</td>
        <td>CTGY | Catégorie</td>
        <td>CATEGORIES_CURRENT<br>CATEGORIES_DAILY_HISTORY<br>CATEGORIES_EVENT</td>
        <td>CATEGORYID (self)<br>ENTEREDBYID<br>GROUPID <br>LASTUPDATEDBYID <br>SYSID</td>
        <td>Self<br>USERS_CURRENT | USERID<br>GROUPS_CURRENT | GROUPID <br>USERS_CURRENT | USERID <br>Non-relation ; utilisé à des fins d’application interne</td>
    </tr>
    <tr>
        <td>Paramètre de catégorie</td>
        <td>Champs de formulaire personnalisés</td>
        <td>CTGYPA | Paramètre de catégorie</td>
        <td>CATEGORIESPARAMETERS_CURRENT<br>CATEGORIESPARAMETERS_DAILY_HISTORY<br>CATEGORIESPARAMETERS_EVENT</td>
        <td>CATEGORIESPARAMETERID (self)<br>CATEGORYID<br>PARAMETERGROUPID<br>PARAMETERID    <br>SYSID</td>
        <td>Self<br>CATEGORIES_CURRENT | CATEGORYID<br>La table Groupe de paramètres n’est actuellement pas prise en charge<br>PARAMETERS_CURRENT | PARAMETERID    <br> N’est pas une relation, utilisée à des fins d’application interne</td>
    </tr>
    <tr>
        <td>Entreprise</td>
        <td>Entreprise</td>
        <td>CMPY | Société</td>
        <td>COMPANIES_CURRENT<br>COMPANIES_DAILY_HISTORY<br>COMPANIES_EVENT</td>
        <td>CATEGORYID<br>COMPANYID (self)<br>ENTEREDBYID<br>GROUPID<br>LASTUPDATEDBYID<br>PRIVATERATECARDID<br>SYSID</td>
        <td>CATEGORIES_CURRENT | CATEGORYID<br>Self<br>USERS_CURRENT | USERID <br>GROUPS_CURRENT | GROUPID<br>USERS_CURRENT | USERID <br>RATECARD_CURRENT | RATECARDID<br>N’est pas une relation ; elle est utilisée à des fins d’application interne.</td>
    </tr>
    <tr>
        <td>Trimestre personnalisé</td>
        <td>Trimestre personnalisé</td>
        <td>CSTQRT | Trimestre personnalisé</td>
        <td>CUSTOMQUARTERS_CURRENT<br>CUSTOMQUARTERS_DAILY_HISTORY<br>CUSTOMQUARTERS_EVENT</td>
        <td>CUSTOMQUARTERID (self) <br>SYSID</td>
        <td>Self<br>Non une relation ; utilisé à des fins d’application interne</td>
    </tr>
    <tr>
        <td>CustomEnum</td>
        <td>Condition, priorité, gravité, état</td>
        <td>CSTEM | Énumération personnalisée</td>
        <td>CUSTOMENUMS_CURRENT<br>CUSTOMENUMS_DAILY_HISTORY<br>CUSTOMENUMS_EVENT<br>* Le type d’enregistrement est identifié par la propriété `enumClass`. Voici les types attendus :<br>CONDITION_OPTASK<br>CONDITION_PROJ<br>CONDITION_TASK<br>PRIORITY_OPTASK<br>PRIORITY_PROJ<br>PRIORITY_TASK<br>SEVERITY_OPTASK<br>STATUS_OPTASK<br>STATUS_PROJ<br>STATUS_TASK</td>
        <td>ENTEREDBYID<br>GROUPID</td>
        <td>USER_CURRENT | USERID<br>GROUP_CURRENT | GROUPID</td>
    </tr>
    <tr>
        <td>Document</td>
        <td>Document</td>
        <td>DOCU | Document</td>
        <td>DOCUMENTS_CURRENT<br>DOCUMENTS_DAILY_HISTORY<br>DOCUMENTS_EVENT<br>DOCUMENTS_CUSTOM_VALUE_CURRENT<br>DOCUMENTS_CUSTOM_VALUE_DAILY_HISTORY<br>DOCUMENTS_CUSTOM_VALUE_EVENT_EVENT</td>
        <td>CATEGORYID<br>CHECKEDOUTBYID<br>DOCUMENTID<br>DOCUMENTREQUESTID<br>EXCHANGERATEID<br>ITERATIONID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>NOTEID<br>OBJID<br>OPTASKID<br>OWNEWRID<br>PORTFOLIOID<br>PROGRAMID<br>PROJECTID<br>RELEASEVERSIONID<br>TASKID<br>TEMPLATEID<br>TEMPLATETASKID<br>TOPOBJID<br>USERID</td>
        <td>CATEGORIES_CURRENT | CATEGORYID<br>USER_CURRENT | USERID<br>Auto<br>Table de requête de document non prise en charge actuellement<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>ITERATIONS_CURRENT | ITERATIONID<br>REMARQUE_CURRENT | NOTEID<br>USER_CURRENT | USERID<br>REMARQUE_CURRENT | NOTEID<br>Variable selon la valeur DOCOBJCODE<br>OPTASK_CURRENT | OPTASKID<br>USER_CURRENT | USERID<br>PORTFOLIO_CURRENT | PORTFOLIOID<br>PROGRAM_CURRENT | PROGRAMID<br>PROJECT_CURRENT | PROJECTID<br>Table Version de publication non prise en charge actuellement<br>TASK_CURRENT | TASKID<br>TEMPLATES_CURRENT | TEMPLATEID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID<br>Variable selon la valeur TOPOBJCODE<br>USER_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Approbation du document</td>
        <td>Approbation du document</td>
        <td>DOCAPL | Approbation de document</td>
        <td>DOCAPPROVALS_CURRENT<br>DOCAPPROVALS_DAILY_HISTORY<br>DOCAPPROVALS_EVENT</td>
        <td>APPROVERID<br>DOCAPPROVALID (self)<br>DOCUMENTID<br>NOTEID<br>REQUESTORID<br>SYSID</td>
        <td>USERS_CURRENT | USERID <br>Self<br>DOCUMENTS_CURRENT | DOCUMENTID<br>NOTES_CURRENT | NOTEID<br>USERS_CURRENT | USERID <br>Non-relation ; utilisé à des fins d’application interne</td>
    </tr>
    <tr>
        <td>Dossier de documents</td>
        <td>Dossier de documents</td>
        <td>DOCFLD | DocsFolders</td>
        <td>DOCFOLDERS_CURRENT<br>DOCFOLDERS_DAILY_HISTORY<br>DOCFOLDERS_EVENT</td>
        <td>DOCFOLDERID (self)<br>ENTEREDBYID<br>ISSUEID<br>ITERATIONID    <br>LINKEDFOLDERID<br>PARENTID<br>PORTFOLIOID <br> PROGRAMID    <br>PROJECTID<br>SYSID<br>TASKID     <br>TEMPLATEID<br>TEMPLATETASKID<br>USERID</td>
        <td>Self<br>USERS_CURRENT | USERID<br>OPTASKS_CURRENT | OPTASKID<br>ITERATIONS_CURRENT | ITERATIONID<br>LINKEDFOLDERS_CURRENT | LINKEDFOLDERID<br>DOCFOLDERS_CURRENT | DOCFOLDERID<br>PORTFOLIO_CURRENT | PORTFOLIOID <br>PROGRAM_CURRENT | PROGRAMID    <br>PROJECTS_CURRENT | PROJECTID <br>Non-relation ; utilisé à des fins d’application interne<br>TASKS_CURRENT | TASKID     <br>TEMPLATES_CURRENT | TEMPLATEID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID<br>USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>DocumentDeliveryMetadata</td>
        <td>Métadonnées fournies par le document</td>
        <td>DOCMET | DocumentProviderMetadata</td>
        <td>DOCPROVIDERMETA_CURRENT<br>DOCPROVIDERMETA_DAILY_HISTORY<br>DOCPROVIDERMETA_EVENT</td>
        <td>DOCPROVIDERMETAID (self) <br>SYSID</td>
        <td>Self<br>Non une relation ; utilisé à des fins d’application interne</td>
    </tr>
    <tr>
        <td>DocumentProvider</td>
        <td>Fournisseur de documents</td>
        <td>DOCPRO | Fournisseur de documents</td>
        <td>DOCPROVIDERS_CURRENT<br>DOCPROVIDERS_DAILY_HISTORY<br>DOCPROVIDERS_EVENT</td>
        <td>DOCPROVIDERCONFIGID<br>DOCPROVIDERID (self)<br>OWNERID    <br>SYSID</td>
        <td>DOCPROVIDERCONFIG_CURRENT | DOCPROVIDERCONFIGID<br>Self<br>USERS_CURRENT | USERID    <br> N’est pas une relation ; elle est utilisée à des fins d’application interne.</td>
    </tr>
    <tr>
        <td>DocumentProviderConfig</td>
        <td>Configuration du fournisseur de documents</td>
        <td>DOCCFG | DocumentProviderConfig</td>
        <td>DOCPROVIDERCONFIG_CURRENT<br>DOCPROVIDERCONFIG_DAILY_HISTORY<br>DOCPROVIDERCONFIG_EVENT</td>
        <td>DOCPROVIDERCONFIGID (self)<br>SYSID</td>
        <td>Self<br>Non une relation ; utilisé à des fins d’application interne</td>
    </tr>
    <tr>
        <td>DocumentVersion</td>
        <td>Version du document</td>
        <td>DOCV | Document Version</td>
        <td>DOCUMENTVERSIONS_CURRENT<br>DOCUMENTVERSIONS_DAILY_HISTORY<br>DOCUMENTVERSIONS_EVENT</td>
        <td>DOCUMENTID<br>DOCUMENTPROVIDERID<br>DOCUMENTVERSIONID<br>ENTEREDBYID<br>EXTERNALSTORAGEID<br>PROOFAPPROVALSTATUSID<br>PROOFEDBYUSERID<br>PROOFID<br>PROOFOWNERID<br>PROOFSTAGEID</td>
        <td>DOCUMENT_CURRENT | DOCUMENTID<br>DOCPROVIDERS_CURRENT | DOCUMENTPROVIDERID<br>Self<br>USER_CURREND | USERID<br>ID externe<br>La table État d’approbation du BAT n’est actuellement pas prise en charge<br>USER_CURRENT | USERID<br>Table BAT non prise en charge actuellement<br>USER_CURRENT | USERID<br>Table d’évaluation du BAT non prise en charge actuellement</td>
    </tr>
    <tr>
        <td>Taux de change</td>
        <td>Taux de change</td>
        <td>EXRATE | Taux d’Exchange</td>
        <td>EXCHANGERATES_CURRENT<br>EXCHANGERATES_DAILY_HISTORY<br>EXCHANGERATES_EVENT</td>
        <td>EXCHANGERATEID (self)<br>PROJECTID<br>SYSID <br>TEMPLATEID  </td>
        <td>Self<br>PROJECTS_CURRENT | PROJECTID <br>Non-relation ; utilisé à des fins d’application interne <br>TEMPLATES_CURRENT | TEMPLATEID  </td>
    </tr>
    <tr>
        <td>Frais</td>
        <td>Frais</td>
        <td>EXPNS | Dépense</td>
        <td>EXPENSES_CURRENT<br>EXPENSES_DAILY_HISTORY<br>EXPENSES_EVENT</td>
        <td>BILLINGRECORDID<br>CATEGORYID<br>ENTEREDBYID<br>EXCHANGERATEID <br>EXPENSEID (self) <br>EXPENSETYPEID <br>LASTUPDATEDBYID <br>OBJID <br>PROJECTID<br>SYSID<br>TASKID<br>PLATEMTEMCORDID TEID<br>TEMPLATETASKID<br>TOPOBJID</td>
        <td>BILLINGRECORDS_CURRENT | BILLINGRECORDID<br>CATEGORIES_CURRENT | CATEGORYID<br>USERS_CURRENT | USERID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID <br>Self <br>EXPENSETYPES_CURRENT | EXPENSETYPEID <br>USERS_CURRENT | USERID <br>ID de l’objet identifié dans le champ OBJCODE <br>PROJECTS_CURRENT | PROJECTID <br>Non-relation ; utilisé à des fins d’application interne<br>TASKS_CURRENT | TASKID<br>TEMPLATES_CURRENT | TEMPLATEID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID<br>Identifiant de l’objet identifié dans le champ TOPOBJCODE.</td>
    </tr>
    <tr>
        <td>Type de frais</td>
        <td>Type de frais</td>
        <td>EXPTYP | Type de dépense</td>
        <td>EXPENSETYPES_CURRENT<br>EXPENSETYPES_DAILY_HISTORY<br>EXPENSETYPES_EVENT</td>
        <td>APPGLOBALID<br>EXPENSETYPEID (self)<br>OBJID <br>SYSID  </td>
        <td>Pas une relation ; utilisé à des fins d’application interne<br>Self<br>ID de l’objet identifié dans le champ OBJCODE <br>Non une relation ; utilisé à des fins d’application interne  </td>
    </tr>
    <tr>
        <td>Groupe</td>
        <td>Groupe</td>
        <td>GROUPE | Groupe</td>
        <td>GROUPS_CURRENT<br>GROUPS_DAILY_HISTORY<br>GROUPS_EVENT</td>
        <td>BUSINESSLEADERID<br>CATEGORYID<br>ENTEREDBYID<br>GROUPID<br>LAYOUTTEMPLATEID<br>PARENTID<br>ROOTID<br>UITEMPLATEID</td>
        <td>USER_CURRENT | USERID<br>CATEGORIES_CURRENT | CATEGORYID<br>USER_CURRENT | USERID<br>La table Modèle de mise en page self<br>ne sera pas prise en charge<br>GROUP_CURRENT | GROUPID<br>GROUP_CURRENT | GROUPID<br>UITEMPLATES_CURRENT | UITEMPLATEID</td>
    </tr>
    <tr>
        <td>Heure</td>
        <td>Heure</td>
        <td>HEURE | Heure</td>
        <td>HOURS_CURRENT<br>HOURS_DAILY_HISTORY<br>HOURS_EVENT</td>
        <td>APPROVEDBYID<br>BILLINGRECORDID<br>CATEGORYID<br>CLASSIFIERID<br>DUPID<br>EXCHANGERATEID<br>EXTERNALTIMESHEETID<br>HOURID<br>HOURTYPEID<br>LASTUPDATEDBYID<br>OPTASKID<br>OWNERID<br>PROJECTID<br>PROJECTOVERHEADID<br>ROLEID<br>TASKID<br>TIMESHEETID</td>
        <td>USER_CURRENT | USERID<br>BILLINGRECORDS_CURRENT | BILLINGRECORDID<br>CATEGORIES_CURRENT | CATEGORYID<br>La table de classificateur n’est actuellement pas prise en charge<br>Aucune relation ; utilisée à des fins d’application interne<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>Aucune relation Workfront ; utilisé pour l’intégration aux systèmes externes<br>Self<br>HOURTYPE_CURRENT | HOURTYPEID<br>USER_CURRENT | USERID<br>OPTASK_CURRENT | OPTASKID<br>USER_CURRENT | USERID<br>PROJECT_CURRENT | PROJECTID<br>Non-relation ; utilisé à des fins d’application interne<br>ROLE_CURRENT | ROLEID<br>TASK_CURRENT | TASKID<br>TIMESHEET_CURRENT | TIMESHEETID</td>
    </tr>
    <tr>
        <td>Type d’heure</td>
        <td>Type d’heure</td>
        <td>HOURT | Type d’heure</td>
        <td>HOURTYPES_CURRENT</td>
        <td>APPGLOBALID<br>HOURTYPEID<br>OBJID</td>
        <td>Pas une relation ; utilisé à des fins d’application interne <br>Self<br>Non une relation ; utilisé à des fins d’application interne</td>
    </tr>
    <tr>
        <td>Itération</td>
        <td>Itération</td>
        <td>ITRN | Itération</td>
        <td>ITERATIONS_CURRENT<br>ITERATIONS_DAILY_HISTORY<br>ITERATIONS_EVENT</td>
        <td>CATEGORYID<br>ENTEREDBYID<br>ITERATIONID (self)<br>LASTUPDATEDBYID<br>OWNERID<br>SYSID<br>TEAMID</td>
        <td>CATEGORIES_CURRENT | CATEGORYID<br>USERS_CURRENT | USERID <br>Self<br>USERS_CURRENT | USERID <br>USERS_CURRENT | USERID <br>Non-relation ; utilisé à des fins d’application interne<br>TEAMS_CURRENT | TEAMID</td>
    </tr>
    <tr>
        <td>Entrée au journal</td>
        <td>Entrée au journal</td>
        <td>JRNLE | Entrée du journal</td>
        <td>JOURNALENTRIES_CURRENT<br>JOURNALENTRIES_DAILY_HISTORY<br>JOURNALENTRIES_EVENT</td>
        <td>APPROVERSTATUSID<br>ASSIGNMENTID<br>AUDITRECORDID<br>BASELINEID <br>BILLINGRECORDID<br>COMPANYID <br>DOCUMENTID <br>DOCUMENTSHAREID <br>EDITEDBYID<br>EXPENSEID<br>HOURID<br>INITIATIATIID VEID<br>JOURNALENTRIEID (self)<br>OBJID<br>OPTASKID<br>PORTFOLIOID<br>PROGRAMID<br>PROJECTID<br>SUBOBJID<br>SUBSCRIBEID<br>SYSID<br>TASKID 1}TEMPLATEID<br>TIMESHEETID<br>TOPOBJID<br>USERID<br></td>
        <td>APPROVERSTATUSES_CURRENT | APPROVERSTATUSID<br>ASSIGNMENTS_CURRENT | ASSIGNMENTID<br>La table des enregistrements d’audit n’est actuellement pas prise en charge<br>BASELINES_CURRENT | BASELINEID <br>BILLINGRECORDS_CURRENT | BILLINGRECORDID<br>COMPANIES_CURRENT | COMPANYID <br>DOCUMENTS_CURRENT | DOCUMENTID <br>Table de partage de document non prise en charge actuellement <br>USERS_CURREND | USERID<br>EXPENSES_CURRENT | EXPENSEID<br>HOURS_CURRENT | HOURID<br>Table d'initiative non prise en charge actuellement<br>Self<br>ID de l'objet identifié dans le champ OBJCODE<br>OPTASKS_CURRENT | OPTASKID<br>PORTFOLIO_CURRENT | PORTFOLIOID<br>PROGRAM_CURRENT | PROGRAMID<br>PROJECTS_CURRENT | PROJECTID <br>ID de l’objet identifié dans le champ SOUS-CODE<br>Abonner la table non prise en charge actuellement<br>Aucune relation ; utilisé à des fins d’application interne<br>TASKS_CURRENT | TASKID<br>TEMPLATES_CURRENT | TEMPLATEID<br>TIMESHEETS_CURRENT | TIMESHEETID<br>ID de l’objet identifié dans le champ TOPOBJCODE<br>USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>LinkedFolder</td>
        <td>LinkedFolder</td>
        <td>LNKFDR | LinkedFolder</td>
        <td>LINKEDFOLDERS_CURRENT<br>LINKEDFOLDERS_DAILY_HISTORY<br>LINKEDFOLDERS_EVENT</td>
        <td>DOCUMENTPROVIDERID<br>EXTERNALSTORAGEID<br>FOLDERID<br>LINKEDBYID<br>LINKEDFOLDERID (self)<br>SYSID</td>
        <td>DOCPROVIDERS_CURRENT | DOCPROVIDERID<br>Identifiant externe<br>DOCFOLDERS_CURRENT | DOCFOLDERID<br>USERS_CURRENT | USERID <br>Self<br>Non une relation ; utilisée à des fins d’application interne  </td>
    </tr>
    <tr>
        <td>Jalon</td>
        <td>Jalon</td>
        <td>MILE | Milestone</td>
        <td>MILESTONES_CURRENT<br>MILESTONES_DAILY_HISTORY<br>MILESTONES_EVENT</td>
        <td>LASTUPDATEDBYID<br>MILESTONEID<br>MILESTONEPATHID</td>
        <td>USER_CURRENT | USERID<br>Self<br>MILESTONEPATH_CURRENT | MILESTONEID</td>
    </tr>
    <tr>
        <td>MilestonePath</td>
        <td>Chemin jalonné</td>
        <td>MPATH | Chemin Milestone</td>
        <td>MILESTONEPATHS_CURRENT<br>MILESTONEPATHS_DAILY_HISTORY<br>MILESTONEPATHS_EVENT</td>
        <td>ENTEREDBYID<br>LASTUPDATEDBYID<br>MILESTONEPATHID</td>
        <td>USER_CURRENT | USERID<br>USER_CURRENT | USERID<br>self</td>
    </tr>
    <tr>
        <td>NonLaborResource</td>
        <td>Ressource non liée à la main-d’œuvre</td>
        <td>NLBR | Ressource hors travail</td>
        <td>NONLABORRESOURCES_CURRENT<br>NONLABORRESOURCES_DAILY_HISTORY<br>NONLABORRESOURCES_EVENT</td>
        <td>CATEGORYID<br>NONLABORRESOURCEID (self)<br>ENTEREDBYID<br>HOMEGROUPID<br>LASTUPDATEDBYID<br>NONLABORRESOURCECATEGORYID <br>SYSID  </td>
        <td>CATEGORIES_CURRENT | CATEGORYID<br>Self<br>USERS_CURRENT | USERID <br>GROUPS_CURRENT | GROUPID<br>USERS_CURRENT | USERID <br>Table Catégorie de ressources autre que travail non prise en charge actuellement <br>Aucune relation ; utilisée à des fins d’application interne    </td>
    </tr>
    <tr>
        <td>Jour sans travail</td>
        <td>Exception de planification</td>
        <td>NONWKD | Jour sans travail</td>
        <td>NONWORKDAYS_CURRENT<br>NONWORKDAYS_DAILY_HISTORY<br>NONWORKDAYS_EVENT</td>
        <td>NONWORKDAYID (self)<br>OBJID <br>SCHEDULEID <br>SYSID <br>USERID  </td>
        <td>Self<br>ID de l’objet identifié dans le champ OBJCODE <br>SCHEDULES_CURRENT | SCHEDULEID <br>Non-relation ; utilisé à des fins d’application interne <br>USERS_CURRENT | USERID  </td>
    </tr>
    <tr>
        <td>Note</td>
        <td>Note</td>
        <td>REMARQUE | Remarque</td>
        <td>NOTES_CURRENT<br>NOTES_DAILY_HISTORY<br>NOTES_EVENT</td>
        <td>ATTACHDOCUMENTID<br>ATTACHOBJID<br>ATTACHOPTASKID<br>ATTACHWORKID<br>ATTACHWORKUSERID<br>AUDITRECORDID<br>COMPANYID<br>DOCUMENTID<br>EXTERNALSERVICEID<br>ITERATIONID<br>NOTEID<br>OBJID <br>OPTASKID<br>OWNERID<br>PARENTENDORSEMENTID<br>PARENTJOURNALENTRYID<br>PARENTNOTEID<br>PORTFOLIOID<br>PROGRAMID<br>PROJECTID<br>PROOFACTIONID{20 <br>RICHTEXTNOTEID<br>TASKID<br>TEMPLATEID<br>TEMPLATETASKID<br>THREADID<br>TIMESHEETID<br>TOPOBJID<br>USERID<br></td>
        <td>DOCUMENT_CURRENT | DOCUMENTID<br>Variable selon ATTACHOBJCODE<br>OPTASK_CURRENT | OPTASKID<br>WORKITEMS_CURRENT<br>USER_CURRENT | USERID<br>La table des enregistrements d’audit n’est actuellement pas prise en charge<br>COMPANIES_CURRENT | COMPANYID <br>DOCUMENT_CURRENT | DOCUMENTID<br>Il ne s’agit pas d’une relation Workfront ; elle est utilisée pour l’intégration à des systèmes externes<br>ITERATIONS_CURRENT | ITERATIONID<br>Self<br>Variable selon le NOTEOBJCODE<br>OPTASK_CURRENT | OPTASKID<br>USER_CURRENT | USERID<br>Table d'inscription non prise en charge actuellement<br>JOURNALENTRIES_CURRENT | JOURNALENTRYID<br>REMARQUE_CURRENT | NOTEID<br>PORTFOLIO_CURRENT | PORTFOLIOID<br>PROGRAM_CURRENT | PROGRAMID<br>PROJECT_CURRENT | PROJECTID<br>La table Action de BAT n’est actuellement pas prise en charge<br>La table BAT n’est actuellement pas prise en charge<br>RESERVEDTEXTNOTES_CURRENT | RICHTEXTNOTEID<br>TASK_CURRENT | TASKID<br>TEMPLATES_CURRENT | TEMPLATEID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID<br>REMARQUE_CURRENT | NOTEID<br>TIMESHEET_CURRENT | TIMESHEETID<br>Variable selon TOPOBJCODE<br>USER_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Intégration d’objets</td>
        <td>Intégration d’objets</td>
        <td>OBJINT | ObjectIntegration</td>
        <td>OBJECTINTEGRATION_CURRENT<br>OBJECTINTEGRATION_DAILY_HISTORY<br>OBJECTINTEGRATION_EVENT</td>
        <td>LINKEDOBJECTID<br>OBJECTINTEGRATIONID   (self)<br>OBJID <br>SYSID  </td>
        <td>ID de l’objet identifié dans le champ LINKEDOBJECTCODE <br>Self<br>ID de l’objet identifié dans le champ OBJCODE <br>Not a relation ; utilisé à des fins d’application interne.  </td>
    </tr>
    <tr>
        <td>Catégorie d’objets</td>
        <td>Catégories d’objets</td>
        <td>OBJCAT | Catégorie d’objet</td>
        <td>OBJECTSCATEGORIES_CURRENT<br>OBJECTSCATEGORIES_DAILY_HISTORY<br>OBJECTSCATEGORIES_EVENT</td>
        <td>CATEGORYID<br>OBJECTSCATEGORYID (self)<br>OBJID <br>SYSID  </td>
        <td>CATEGORIES_CURRENT | CATEGORYID<br>Self<br>Identifiant de l’objet identifié dans le champ OBJCODE <br>Non une relation ; utilisé à des fins d’application interne  </td>
    </tr>
    <tr>
        <td>TâcheOp</td>
        <td>Problème, requête</td>
        <td>OPTASK | Problème</td>
        <td>OPTASKS_CURRENT<br>OPTASKS_DAILY_HISTORY<br>OPTASKS_EVENT<br>OPTASKS_CUSTOM_VALUE_CURRENT<br>OPTASKS_CUSTOM_VALUE_DAILY_HISTORY<br>OPTASKS_CUSTOM_VALUE_EVENT_EVENT</td>
        <td>APPROVALPROCESSID<br>ASSIGNEDTOID<br>CATEGORYID<br>CURRENTAPPROVALSTEPID<br>ENTEREDBYID<br>EXCHANGERATEID<br>ITERATIONID<br>KANBANBOARDID<br>LASTCONDITIONNOTEID<br>LASTNOTEID<br>LASTUDAPTEDBYID<br>OPTASKID<br>OWNERID<br>PROJECTID<br>QUEUEDEFID<br>QUEUETOPICID<br>RESOLVEOPTASKID<br>RESOLVEPROJECTID<br>RESOLVETASKID<br>RE}RESOLYID VINGOBJID<br>ROLEID<br>SOURCEOBJID<br>SOURCETASKID<br>SUBMITTEDBYID<br>TEAMID</td>
        <td>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>USER_CURRENT | USERID<br>CATEGORIES_CURRENT | CATEGORYID<br>APPROVALSTEPS_CURRENT | APPROVALSTEPID<br>USER_CURRENT | USERID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>ITERATIONS_CURRENT | ITERATIONID<br>Table de panorama Kanban non prise en charge actuellement<br>REMARQUE_CURRENT | NOTEID<br>REMARQUE_CURRENT | NOTEID<br>USER_CURRENT | USERID<br>Self<br>USER_CURRENT | USERID<br>PROJECT_CURRENT | PROJECTID<br>Table de définition de file d’attente non prise en charge actuellement<br>Table de rubrique de file d’attente non prise en charge actuellement<br>OPTASK_CURRENT | OPTASKID<br>PROJECT_CURRENT | PROJECTID<br>TASK_CURRENT | TASKID<br>Variable selon RESOLVINGOBJCODE<br>ROLE_CURRENT | ROLEID<br>Variable selon SOURCEOBJCODE<br>TASK_CURRENT | TASKID<br>USER_CURRENT | USERID<br>TEAM_CURRENT | TEAMID</td>
    </tr>
    <tr>
        <td>Paramètre</td>
        <td>Champ personnalisé</td>
        <td>PARAM | Paramètre</td>
        <td>PARAMETERS_CURRENT<br>PARAMETERS_DAILY_HISTORY<br>PARAMETERS_EVENT</td>
        <td>LASTUPDATEDBYID<br>PARAMETERFILTERID<br>PARAMETERID (self)<br>SYSID  </td>
        <td>USERS_CURRENT | USERID<br>La table Filtre de paramètres n’est actuellement pas prise en charge<br>Auto<br>Aucune relation ; utilisée à des fins d’application interne  </td>
    </tr>
    <tr>
        <td>Option de paramètre</td>
        <td>Option de paramètre</td>
        <td>POPT | Option de paramètre</td>
        <td>PARAMETEROPTIONS_CURRENT<br>PARAMETEROPTIONS_DAILY_HISTORY<br>PARAMETEROPTIONS_EVENT</td>
        <td>PARAMETERID<br>PARAMETEROPTIONID (self) <br>SYSID  </td>
        <td>PARAMETERS_CURRENT | PARAMETERID <br>Self <br>Non une relation ; utilisé à des fins d’application interne  </td>
    </tr>
    <tr>
        <td>Section du portail</td>
        <td>Rapport</td>
        <td>PTLSEC | Rapport</td>
        <td>PORTALSECTIONS_CURRENT<br>PORTALSECTIONS_DAILY_HISTORY<br>PORTALSECTIONS_EVENT</td>
        <td>APPGLOBALID<br>ENTEREDBYID<br>FILTERID<br>GROUPBYID<br>LASTUPDATEDBYID<br>LASTVIEWEDBYID<br>OBJID<br>PORTALSECTIONID (self-self)<br>PREFERENCEID<br>PUBLICRUNASUSERID<br>}REPORTFOLFOLFOLLIID RID<br>RUNASUSERID<br>SCHEDULEDREPORTID<br>SYSID<br>VIEWID</td>
        <td>Pas une relation ; utilisé à des fins d’application interne <br>USERS_CURRENT | USERID <br>UIFILTERS_CURRENT | FILTERID<br>UIGROUPBYS_CURREND | GROUPBYID<br>USERS_CURRENT | USERID <br>USERS_CURRENT | USERID <br>ID de l’objet identifié dans le champ OBJOBJCODE<br>Self<br>PREFERENCES_CURRENT | PREFERENCEID<br>USERS_CURRENT | USERID <br>REPORTFOLDERS_CURRENT | REPORTFOLDERID<br>USERS_CURRENT | USERID <br>La table des rapports planifiés n’est actuellement pas prise en charge<br>Aucune relation ; utilisée à des fins d’application interne <br>UIVIEWS_CURRENT | VIEWID</td>
    </tr>
    <tr>
        <td>Onglet Portail</td>
        <td>Tableau de bord</td>
        <td>PTLTAB | Tableau de bord</td>
        <td>PORTALTABS_CURRENT<br>PORTALTABS_DAILY_HISTORY<br>PORTALTABS_EVENT</td>
        <td>DOCID<br>LASTUPDATEDBYID<br>PORTALPROFILEID<br>PORTALTABID (self)<br>SYSID<br>USERID</td>
        <td>Pas une relation ; utilisé à des fins d’application interne <br>USERS_CURRENT | USERID <br>La table Profil du portail ne sera pas prise en charge <br>Auto<br>Aucune relation ; utilisée à des fins d’application interne <br>USERS_CURRENT | USERID  </td>
    </tr>
    <tr>
        <td>Section d'onglet de portail</td>
        <td>Section du tableau de bord</td>
        <td>PRTBSC | Section d’onglet Portail</td>
        <td>PORTALTABSPORTALSECTIONS_CURRENT<br>PORTALTABSPORTALSECTIONS_DAILY_HISTORY<br>PORTALTABSPORTALSECTIONS_EVENT</td>
        <td>CALENDARPORTALSECTIONID<br>EXTERNALSECTIONID<br>INTERNALSECTIONID <br>PORTALSECTIONOBJID <br>PORTALTABID<br>PORTALTABSECTIONID (self)<br>SYSID</td>
        <td>La section Portail Calendrier n’est pas prise en charge actuellement<br>La table Sections externes n’est pas prise en charge actuellement<br>PORTALSECTIONS_CURRENT | PORTALSECTIONID <br>Identifiant de l’objet identifié dans le champ PORTALSECTIONOBJCODE<br>PORTALTABS_CURRENT | PORTALTABID<br>Self<br>Aucune relation ; utilisé à des fins d’application interne</td>
    </tr>
    <tr>
        <td>PortalSectionLastViewer</td>
        <td>Dernières visionneuses de rapports</td>
        <td>PLSLSV | PortalSectionLastViewer</td>
        <td>REPORTLASTVIEWERS_CURRENT<br>REPORTLASTVIEWERS_DAILY_HISTORY<br>REPORTLASTVIEWERS_EVENT</td>
        <td>REPORTID<br>REPORTLASTVIEWERID (self)<br>SYSID<br>VIEWERID</td>
        <td>PORTALSECTIONS_CURRENT | PORTALSECTIONID <br>REPORTLASTVIEWERID (self)<br>Aucune relation ; utilisé à des fins d’application interne<br>USERS_CURRENT | USERID  </td>
    </tr>
    <tr>
        <td>Portfolio</td>
        <td>Portfolio</td>
        <td>PORT | Portfolio</td>
        <td>PORTFOLIOS_CURRENT<br>PORTFOLIO_DAILY_HISTORY<br>PORTFOLIOS_EVENT<br>PORTFOLIO_CUSTOM_VALUE_CURRENT<br>PORTFOLIO_CUSTOM_VALUE_DAILY_HISTORY<br>PORTFOLIOS_CUSTOM_VALUE_EVENT_EVENT</td>
        <td>ALIGNMENTSCORECARDID<br>CATEGORYID<br>ENTEREDBYID<br>GROUPID<br>LASTUPDATEDBYID<br>OWNERID<br>PORTFOLIOID</td>
        <td>Table de Fiche d’évaluation non prise en charge actuellement<br>CATEGORIES_CURRENT | CATEGORYID<br>USER_CURRENT | USERID<br>GROUP_CURRENT | GROUPID<br>USER_CURRENT | USERID<br>USER_CURRENT | USERID<br>self</td>
    </tr>
    <tr>
        <td>Préférence</td>
        <td>Afficher, filtrer, regrouper, Définition de rapport</td>
        <td>PROSET | Préférence</td>
        <td>PREFERENCES_CURRENT<br>PREFERENCES_DAILY_HISTORY<br>PREFERENCES_EVENT</td>
        <td>APPGLOBALID<br>PREFERENCEID (self) <br>SYSID  </td>
        <td>Pas une relation ; utilisé à des fins d’application interne <br>Self <br>Non une relation ; utilisé à des fins d’application interne  </td>
    </tr>
    <tr>
        <td>Programme</td>
        <td>Programme</td>
        <td>PRGM | Programme</td>
        <td>PROGRAMS_CURRENT<br>PROGRAMS_DAILY_HISTORY<br>PROGRAMS_EVENT<br>PROGRAMS_CUSTOM_VALUE_CURRENT<br>PROGRAMS_CUSTOM_VALUE_DAILY_HISTORY<br>PROGRAMS_CUSTOM_VALUE_EVENT</td>
        <td>CATEGORYID<br>ENTEREDBYID<br>GROUPID<br>LASTUPDATEDBYID<br>OWNERID<br>PORTFOLIOID<br>PROGRAMID</td>
        <td>CATEGORIES_CURRENT | CATEGORYID<br>USER_CURRENT | USERID<br>GROUP_CURRENT | GROUPID<br>USER_CURRENT | USERID<br>USER_CURRENT | USERID<br>PORTFOLIO_CURRENT | PORTFOLIOID<br>self</td>
    </tr>
    <tr>
        <td>Projet</td>
        <td>Projet</td>
        <td>PROJ | Projet</td>
        <td>PROJECTS_CURRENT<br>PROJECTS_DAILY_HISTORY<br>PROJECTS_EVENT<br>PROJECTS_CUSTOM_VALUE_CURRENT<br>PROJECTS_CUSTOM_VALUE_DAILY_HISTORY<br>PROJECTS_CUSTOM_VALUE_EVENT_EVENT</td>
        <td>AEMNATIVEFOLDERTREESREFID<br>ALIGNMENTSCORECARDID<br>APPROVALPROCESSID<br>ATTACHEDRATECARDID<br>CATEGORYID<br>COMPANYID<br>CONVERTEDOPTASKID<br>CONVERTEPTAPTASKORIGINATORID<br>CURRENPPROPPROPPROPPROPPROPSTEPID<br>DELIVERABLESCORECARDID<br>ENTEREDBYID<br>GROUPID<br>LASTCONDITIONNOTEID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>MILESTONEPATHID<br>OWNERID<br>POPACCOUNTID<br>PORTFOLIOID<br>PRIVATERATECARDID<br>PROGRAMID<br>PROJECTID<br>QUEUEDEFID<br>REJECTIONISSUEID<br>RESOURCEPOOLID<br>SCHEDULEID<br>SPON}SPONRID<br>SUBMITTEDBYID<br>TEAMID<br>TEMPLATEID</td>
        <td>Aucune relation Workfront ; utilisée pour l’intégration aux systèmes externes<br>Table de Fiche d’évaluation non prise en charge actuellement<br>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>RATECARD_CURRENT | RATECARDID<br>CATEGORIES_CURRENT | CATEGORYID<br>COMPANIES_CURRENT | COMPANYID <br>OPTASK_CURRENT | OPTASKID<br>USER_CURRENT | USERID<br>APPROVALSTEPS_CURRENT | APPROVALSTEPID<br>Table de Fiche d’évaluation non prise en charge actuellement<br>USER_CURRENT | USERID<br>GROUP_CURRENT | GROUPID<br>REMARQUE_CURRENT | NOTEID<br>REMARQUE_CURRENT | NOTEID<br>USER_CURRENT | USERID<br>MILESTONEPATH_CURRENT | MILESTONEPATHID<br>USER_CURRENT | USERID<br>Table de compte pop non prise en charge actuellement<br>PORTFOLIO_CURRENT | PORTFOLIOID<br>RATECARD_CURRENT | RATECARDID<br>PROGRAM_CURRENT | PROGRAMID<br>Auto<br>Table de définition de file d’attente non prise en charge actuellement<br>OPTASK_CURRENT | OPTASKID<br>RESOURCEPOOLS_CURRENT | RESOURCEPOOLID<br>SCHEDULE_CURRENT | SCHEDULEID<br>USER_CURRENT | USERID<br>USER_CURRENT | USERID<br>TEAM_CURRENT | TEAMID<br>TEMPLATES_CURRENT | TEMPLATEID</td>
    </tr>
    <tr>
        <td>RateCard</td>
        <td>Carte tarifaire</td>
        <td>RTCRD |Rate Card</td>
        <td>RATECARD_CURRENT<br>RATECARD_DAILY_HISTORY<br>RATECARD_EVENT</td>
        <td>CATEGORYID<br>ENTEREDBYID<br>LASTUPDATEDBYID <br>RATECARDID (self-) <br>SECURITYROOTID <br>SOURCEID<br>SYSID</td>
        <td>CATEGORYID<br>USERS_CURRENT | USERID <br>USERS_CURRENT | USERID    <br>self<br>ID de l’objet identifié dans le champ SECURITYOBJCODE <br>ID de l’objet identifié dans le champ SOURCEOBJCODE<br>N’est pas une relation ; utilisé à des fins d’application interne.  </td>
    </tr>
    <tr>
        <td>Dossier des rapports</td>
        <td>Dossier des rapports</td>
        <td>RPTFDR | Dossier de rapports</td>
        <td>REPORTFOLDERS_CURRENT<br>REPORTFOLDERS_DAILY_HISTORY<br>REPORTFOLDERS_EVENT</td>
        <td>REPORTFOLDERID (self) <br>SYSID  </td>
        <td>Auto <br>Non-relation ; utilisé à des fins d’application interne  </td>
    </tr>
    <tr>
        <td>Durée réservée</td>
        <td>(Personnel) Heure de désactivation</td>
        <td>RESVT | Heure de désactivation</td>
        <td>RESERVEDTIMES_CURRENT<br>RESERVEDTIMES_DAILY_HISTORY<br>RESERVEDTIMES_EVENT</td>
        <td>RESERVEDTIMEID (self) <br>SYSID<br>TASKID<br>USERID  </td>
        <td>Self<br>N’est pas une relation ; elle est utilisée à des fins d’application interne<br>TASKS_CURRENT | TASKID<br>USERS_CURRENT | USERID  </td>
    </tr>
    <tr>
        <td>Pool de ressources</td>
        <td>Pool de ressources</td>
        <td>RSPL | Pool de ressources</td>
        <td>RSRCPOOLS_CURRENT<br>RSRCPOOLS_DAILY_HISTORY<br>RSRCPOOLS_EVENT</td>
        <td>ENTEREDBYID<br>LASTUPDATEDBYID <br>RESOURCEPOOLID (self)<br>SYSID  </td>
        <td>USERS_CURRENT | USERID <br>USERS_CURRENT | USERID <br>Self<br>Non une relation ; utilisée à des fins d’application interne  </td>
    </tr>
    <tr>
        <td>Remarque Rich Text</td>
        <td>Remarque Rich Text</td>
        <td>RHRENOTE | Remarque sur le texte enrichi</td>
        <td>RESERVEDTEXTNOTES_CURRENT<br>RESERVEDTEXTNOTES_DAILY_HISTORY<br>RESERVEDTEXTNOTES_EVENT</td>
        <td>RICHTEXTNOTEID (self) <br>SYSID  </td>
        <td>Auto <br>Non-relation ; utilisé à des fins d’application interne  </td>
    </tr>
    <tr>
        <td>Valeur de paramètre de texte enrichi</td>
        <td>Valeur de paramètre de texte enrichi</td>
        <td>RCHV | RichTextParameterValue</td>
        <td>RICHTEXTPARAMETERVALUES_CURRENT<br>RICHTEXTPARAMETERVALUES_DAILY_HISTORY<br>RICHTEXTPARAMETERVALUES_EVENT</td>
        <td>PARAMETERVALUEID<br>RICHTEXTPARAMETERVALUEID (self) <br>SYSID  </td>
        <td>La table Valeur de paramètre n'est actuellement pas prise en charge <br>Auto <br>Aucune relation ; utilisée à des fins d'application interne  </td>
    </tr>
    <tr>
        <td>Risque</td>
        <td>Risque</td>
        <td>RISQUE | Risque</td>
        <td>RISKS_CURRENT<br>RISKS_DAILY_HISTORY<br>RISKS_EVENT</td>
        <td>ENTEREDBYID<br>EXCHANGERATEID<br>LASTUPDATEDBYID <br>PROJECTID <br>RISKID (self)<br>RISKTYPEID<br>SYSID<br>TEMPLATEID</td>
        <td>USERS_CURRENT | USERID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>USERS_CURRENT | USERID <br>PROJECTS_CURRENT | PROJECTID   <br>Self<br>RISKTYPES_CURRENT | RISKTYPEID<br>Non-relation ; utilisé à des fins d’application interne<br>TEMPLATES_CURRENT | TEMPLATEID</td>
    </tr>
    <tr>
        <td>Type de risque</td>
        <td>Type de risque</td>
        <td>RSKTYP | Type de risque</td>
        <td>RISKTYPES_CURRENT<br>RISKTYPES_DAILY_HISTORY<br>RISKTYPES_EVENT</td>
        <td>RISKTYPEID<br>SYSID</td>
        <td>Self<br>Non une relation ; utilisé à des fins d’application interne</td>
    </tr>
    <tr>
        <td>Rôle</td>
        <td>Fonction</td>
        <td>RÔLE | Rôle de tâche</td>
        <td>ROLES_CURRENT<br>ROLES_DAILY_HISTORY<br>ROLES_EVENT</td>
        <td>ENTEREDBYID<br>LAYOUTTEMPLATEID<br>PRIVATERATECARDID<br>ROLEID<br>UITEMPLATEID</td>
        <td>USER_CURRENT | USERID<br>La table Modèle de mise en page ne sera pas prise en charge<br>RATECARD_CURRENT | RATECARDID<br>Self<br>UITEMPLATES_CURRENT |UITEMPLATEID</td>
    </tr>
    <tr>
        <td>Planning</td>
        <td>Planning</td>
        <td>SCHED | Planification</td>
        <td>SCHEDULES_CURRENT<br>SCHEDULES_DAILY_HISTORY<br>SCHEDULES_EVENT</td>
        <td>ENTEREDBYID<br>GROUPID<br>HOMEGROUPID<br>SCHEDULEID</td>
        <td>USER_CURRENT | USERID<br>GROUP_CURRENT | GROUPID<br>GROUP_CURRENT | GROUPID<br>Self</td>
    </tr>
    <tr>
        <td>Personne approbatrice d’étape</td>
        <td>Personne approbatrice d’étape</td>
        <td>SPAPVR | Approbateur d’étape</td>
        <td>STEPAPPROVERS_CURRENT<br>STEPAPPROVERS_DAILY_HISTORY<br>STEPAPPROVERS_EVENT</td>
        <td>APPROVALSTEPID<br>ROLEID<br>STEPAPPROVERID (self)<br>SYSID <br>TEAMID<br>USERID</td>
        <td>APPROVALSTEPS_CURRENT | APPROVALSTEPID<br>ROLES_CURRENT | ROLEID<br>Self<br>Aucune relation ; utilisé à des fins d’application interne <br>TEAMS_CURRENT | TEAMID<br>USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Tâche</td>
        <td>Tâche</td>
        <td>TÂCHE | Tâche</td>
        <td>TASKS_CURRENT<br>TASKS_DAILY_HISTORY<br>TASKS_EVENT<br>TASKS_CUSTOM_VALUE_CURRENT<br>TASKS_CUSTOM_VALUE_DAILY_HISTORY<br>TASKS_CUSTOM_VALUE_EVENT</td>
        <td>APPROVALPROCESSID<br>ASSIGNEDTOID<br>BILLINGRECORDID<br>CATEGORYID<br>CONVERTEDOPTASKID<br>CONVERTEDOPTASKORIGINATORID<br>CURRENTAPPROVALSTEPID<br>ENTEREDBYID<br>EXCHANGERATEID<br>GROUP8}ID<br>ITERATIONID<br>KANBANBOARDID<br>LASTCONDITIONNOTEID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>MILESTONEID<br>PARENTID<br>PROJECTID<br>RECURRENCERULEID <br>REJECTIONISSUEID<br>RESERVEDTIMEID<br>ROLEID<br>SUBMITTEDBYID<br>TASKID<br>TEAMID<br>TEMPLATETASKID</td>
        <td>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>USER_CURRENT | USERID<br>BILLINGRECORDS_CURRENT | BILLINGRECORDID<br>CATEGORIES_CURRENT | CATEGORYID<br>OPTASK_CURRENT | OPTASKID<br>USER_CURRENT | USERID<br>APPROVALSTEPS_CURRENT | APPROVALSTEPID<br>USER_CURRENT | USERID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>GROUP_CURRENT | GROUPID<br>ITERATIONS_CURRENT | ITERATIONID<br>Table de panorama Kanban non prise en charge actuellement<br>REMARQUE_CURRENT | NOTEID<br>REMARQUE_CURRENT | NOTEID<br>USER_CURRENT | USERID<br>MILESTONE_CURRENT | MILESTONEID<br>TASK_CURRENT | TASKID<br>PROJECT_CURRENT | PROJECTID<br>La table des règles de périodicité n’est actuellement pas prise en charge<br>OPTASK_CURRENT | OPTASKID<br>RESERVEDTIMES_CURRENT | RESERVEDTIMEID<br>ROLE_CURRENT | ROLEID<br>USER_CURRENT | USERID<br>Self<br>TEAM_CURRENT | TEAMID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID</td>
    </tr>
    <tr>
        <td>Prédécesseur de tâche</td>
        <td>Tâche antérieure</td>
        <td>PRED | Prédécesseur</td>
        <td>PREDECESSORS_CURRENT<br>PREDECESSORS_DAILY_HISTORY<br>PREDECESSORS_EVENT</td>
        <td>ID (self)<br>PREDECESSORID<br>SUCCESSORID <br>SYSID</td>
        <td>Self<br>TASKS_CURRENT | TASKID<br>TASKS_CURRENT | TASKID <br>Non-relation ; utilisé à des fins d’application interne</td>
    </tr>
    <tr>
        <td>Equipe</td>
        <td>Equipe</td>
        <td>TEAMOB | Équipe</td>
        <td>TEAMS_CURRENT<br>TEAMS_DAILY_HISTORY<br>TEAMS_EVENT</td>
        <td>ENTEREDBYID<br>GROUPID<br>LAYOUTTEMPLATEID<br>MYWORKVIEWID<br>OWNERID<br>REQUESTSVIEWID<br>SCHEDULEID<br>TEAMID<br>UITEMPLATEID</td>
        <td>USER_CURRENT | USERID<br>GROUP_CURRENT | GROUPID<br>La table Modèle de mise en page ne sera pas prise en charge<br>UIVIEWS_CURRENT | UIVIEWID<br>USER_CURRENT | USERID<br>UIVIEWS_CURRENT | UIVIEWID<br>SCHEDULE_CURRENT | SCHEDULEID<br>Self<br>UITEMPLATES_CURRENT |UITEMPLATEID</td>
    </tr>
    <tr>
        <td>Membre d'équipe</td>
        <td>Autres équipes, membre de l’équipe</td>
        <td>TEAMMB | Membre de l’équipe</td>
        <td>TEAMMEMBERS_CURRENT<br>TEAMMEMBERS_DAILY_HISTORY<br>TEAMMEMBERS_EVENT</td>
        <td>SYSID <br>TEAMID<br>TEAMMEMBERID (self)<br>USERID</td>
        <td>Pas une relation ; utilisé à des fins d’application interne <br>TEAMS_CURRENT | TEAMID<br>Self<br>USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>TeamMemberRole</td>
        <td>Rôle de membre d'équipe</td>
        <td>TEAMMR | Rôle du membre de l’équipe</td>
        <td>TEAMMEMBERROLES_CURRENT<br>TEAMMEMBERROLES_DAILY_HISTORY<br>TEAMMEMBERROLES_EVENT</td>
        <td>ROLEID <br>TEAMID<br>TEAMMEMBERROLEID (self)<br>USERID</td>
        <td>ROLES_CURRENT | ROLEID <br>TEAMS_CURRENT | TEAMID<br>Self<br>USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Modèle</td>
        <td>Modèle</td>
        <td>TMPL | Modèle</td>
        <td>TEMPLATES_CURRENT<br>TEMPLATES_DAILY_HISTORY<br>TEMPLATES_EVENT</td>
        <td>APPROVALPROCESSID<br>CATEGORYID<br>COMPANYID <br>DELIVERABLESCORECARDID <br>ENTEREDBYID<br>GROUPID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>MILESTONEPATHID <br>OWNERID <br>PRITERATÉRATÉRATECARDID<br>PROGRAMID<br>QUEUEDEFID<br>SCHEDULEID <br>SYSID <br>TEAMID<br>TEMPLATEID (self))</td>
        <td>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>CATEGORIES_CURREND | CATEGORYID<br>COMPANIES_CURRENT | COMPANYID   <br>DELIVERABLESCORECARDID <br>USERS_CURRENT | USERID<br>GROUPS_CURRENT | GROUPID<br>NOTES_CURRENT | NOTEID<br>USERS_CURRENT | USERID<br>MILESTONEPATH_CURRENT | MILESTONEPATHID <br>USERS_CURRENT | USERID <br>RATECARD_CURRENT | RATECARDID<br>PROGRAM_CURRENT | PROGRAMID<br>Table de définition de file d’attente non prise en charge actuellement<br>SCHEDULES_CURRENT | SCHEDULEID <br>N’est pas une relation ; utilisé à des fins d’application interne <br>TEAMS_CURRENT | TEAMID<br>Self</td>
    </tr>
    <tr>
        <td>Modèle d'affectation</td>
        <td>Modèle d'affectation</td>
        <td>TASSGN | Attribution de modèles</td>
        <td>TEMPLATEASSIGNMENTS_CURRENT<br>TEMPLATEASSIGNMENTS_DAILY_HISTORY<br>TEMPLATEASSIGNMENTS_EVENT</td>
        <td>ASSIGNEDTOID<br>CATEGORYID<br>LASTUPDATEDBYID<br>OBJID<br>ROLEID<br>SYSID<br>TEAMID<br>TEAMTIMELINEABLEID<br>TEMPLATEASSIGNMENTID (self)<br>TEMPLATETASKID</td>
        <td>USERS_CURRENT | USERID<br>CATEGORIES_CURRENT | CATEGORYID<br>USERS_CURRENT | USERID<br>Identifiant de l’objet identifié dans le champ OBJCODE<br>ROLES_CURRENT | ROLEID<br>Non-relation ; utilisé à des fins d’application interne<br>TEAMS_CURRENT | TEAMID<br>Table Timelineable de l’équipe non prise en charge actuellement<br>Self<br>TEMPLATETASKS_CURRENEN |TEMPLATETASKID</td>
    </tr>
    <tr>
        <td>Tâche de modèle</td>
        <td>Tâche de modèle</td>
        <td>TTSK | Tâche du modèle</td>
        <td>TEMPLATETASKS_CURRENT<br>TEMPLATETASKS_DAILY_HISTORY<br>TEMPLATETASKS_EVENT</td>
        <td>APPROVALPROCESSID<br>ASSIGNEDTOID<br>CATEGORYID<br>ENTEREDBYID<br>EXCHANGERATEID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>MILESTONEID<br>PARENTID<br>RECURRENULEID<br>ROLEID 10}SYSID<br>TEAMID<br>TEAMTIMELINEABLEID<br>TEMPLATEID<br>TEMPLATETASKID (self))<br></td>
        <td>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>USERS_CURRENT | USERID<br>CATEGORIES_CURRENT | CATEGORYID<br>USERS_CURRENT | USERID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>NOTES_CURRENT | NOTEID<br>USERS_CURRENT | USERID<br>MILESTONE_CURRENT | MILESTONEID<br>TEMPLATETASKS_CURRENT |TEMPLATETASKID<br>La table des règles de périodicité n’est actuellement pas prise en charge<br>ROLES_CURRENT | ROLEID<br>Non-relation ; utilisé à des fins d’application interne<br>TEAMS_CURRENT | TEAMID<br>Table Chronologique de l’équipe non prise en charge actuellement<br>TEMPLATES_CURRENT | TEMPLATEID<br>Self</td>
    </tr>
    <tr>
        <td>Prédécesseur de tâche de modèle</td>
        <td>Prédécesseur de modèle</td>
        <td>TPRED | Prédécesseur</td>
        <td>TEMPLATEPREDECESSORS_CURRENT<br>TEMPLATEPREDECESSORS_DAILY_HISTORY<br>TEMPLATEPREDECESSORS_EVENT</td>
        <td>PREDECESSORID<br>SUCCESSORID <br>TEMPLATEPREDECESSORID (self)<br>SYSID</td>
        <td>TEMPLATETASKS_CURRENT |TEMPLATETASKID<br>TEMPLATETASKS_CURRENT |TEMPLATETASKID <br>Self<br>Non-relation ; utilisé à des fins d’application interne</td>
    </tr>
    <tr>
        <td>Feuille de temps</td>
        <td>Feuille de temps</td>
        <td>TSHET | Feuille de calcul</td>
        <td>TIMESHEETS_CURRENT<br>TIMESHEETS_DAILY_HISTORY<br>TIMESHEETS_EVENT</td>
        <td>APPROVERID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>TIMESHEETID<br>TIMESHEETPROFILEID<br>USERID</td>
        <td>USER_CURRENT | USERID<br>REMARQUE_CURRENT | NOTEID<br>USER_CURRENT | USERID<br>Self<br>TIMESHEETPROFILES_CURRENT | TIMESHEETPROFILEID<br>USER_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Profil de feuille de temps</td>
        <td>Profil de feuille de temps</td>
        <td>TSPRO | Profil de feuille de calcul</td>
        <td>TIMESHEETPROFILES_CURRENT<br>TIMESHEETPROFILES_DAILY_HISTORY<br>TIMESHEETPROFILES_EVENT</td>
        <td>APPROVERID<br>ENTEREDBYID <br>GROUPID<br>SYSID<br>TIMESHEETPROFILEID (self)</td>
        <td>USERS_CURRENT | USERID<br>USERS_CURRENT | USERID <br>GROUPS_CURRENT | GROUPID<br>Non-relation ; utilisé à des fins d’application interne<br>Self</td>
    </tr>
    <tr>
        <td>Filtre d’interface utilisateur</td>
        <td>Filtre</td>
        <td>UIFT | Filtrer</td>
        <td>UIFILTERS_CURRENT<br>UIFILTERS_DAILY_HISTORY<br>UIFILTERS_EVENT</td>
        <td>APPGLOBALID<br>ENTEREDBYID <br>LASTUPDATEDBYID <br>OBJID<br>PREFERENCEID<br>SYSID <br>UIFILTERID (self)</td>
        <td>Pas une relation ; utilisé à des fins d’application interne<br>USERS_CURRENT | USERID <br>USERS_CURRENT | USERID <br>ID de l’objet identifié dans le champ OBJCODE<br>PREFERENCES_CURRENT | PREFERENCEID<br>Non-relation ; utilisé à des fins d’application interne <br>Self</td>
    </tr>
    <tr>
        <td>Groupe d’IU par</td>
        <td>Regroupement </td>
        <td>UIGB | Regroupement</td>
        <td>UIGROUPBYS_CURRENT<br>UIGROUPBYS_DAILY_HISTORY<br>UIGROUPBYS_EVENT</td>
        <td>ENTEREDBYID<br>GROUPID <br>LASTUPDATEDBYID <br>SYSID <br>UITEMPLATEID (self)</td>
        <td>USERS_CURRENT | USERID<br>GROUPS_CURRENT | GROUPID <br>USERS_CURRENT | USERID <br>Non-relation ; utilisé à des fins d’application interne <br>self</td>
    </tr>
    <tr>
        <td>Modèle d’IU</td>
        <td>Modèle de mise en page</td>
        <td>UITMPL | Modèle de mise en page</td>
        <td>UITEMPLATES_CURRENT<br>UITEMPLATES_DAILY_HISTORY<br>UITEMPLATES_EVENT</td>
        <td>APPGLOBALID<br>ENTEREDBYID <br>LASTUPDATEDBYID <br>OBJID<br>PREFERENCEID<br>SYSID <br>UIGROUPBYID (self)</td>
        <td>Pas une relation ; utilisé à des fins d’application interne<br>USERS_CURRENT | USERID <br>USERS_CURRENT | USERID <br>ID de l’objet identifié dans le champ OBJCODE<br>PREFERENCES_CURRENT | PREFERENCEID<br>Non-relation ; utilisé à des fins d’application interne <br>Self</td>
    </tr>
    <tr>
        <td>Vue de l’interface utilisateur</td>
        <td>Afficher</td>
        <td>UIVIEW | Affichage</td>
        <td>UIVIEWS_CURRENT<br>UIVIEWS_DAILY_HISTORY<br>UIVIEWS_EVENT</td>
        <td>APPGLOBALID<br>ENTEREDBYID <br>LASTUPDATEDBYID <br>OBJID<br>PREFERENCEID<br>SYSID <br>UIVIEWID (self)</td>
        <td>Pas une relation ; utilisé à des fins d’application interne<br>USERS_CURRENT | USERID <br>USERS_CURRENT | USERID <br>ID de l’objet identifié dans le champ OBJCODE<br>PREFERENCES_CURRENT | PREFERENCEID<br>Non-relation ; utilisé à des fins d’application interne <br>Self</td>
    </tr>
    <tr>
        <td>l’utilisateur ou de l’utilisatrice</td>
        <td>l’utilisateur ou de l’utilisatrice</td>
        <td>UTILISATEUR | Utilisateur</td>
        <td>USERS_CURRENT<br>USERS_DAILY_HISTORY<br>USERS_EVENT<br>USERS_CUSTOM_VALUE_CURRENT<br>USERS_CUSTOM_VALUE_DAILY_HISTORY<br>USERS_CUSTOM_VALUE_EVENT_EVENT</td>
        <td>ACCESSLEVELID<br>CATEGORYID<br>COMPANYID<br>DEFAULTHOURTYPEID<br>DELEGATIONTOID<br>EAUTHUSERID<br>ENTEREDBYID<br>HOMEGROUPID<br>HOMETEAMID<br>LASTENTEREDNOTEID<br>LASTUDAPID TEDBYID<br>LATESTUPDATENOTEID<br>LAYOUTTEMPLATEID<br>MANAGERID<br>PORTALPROFILEID<br>PREFUIID<br>PRIVATERATECARDID<br>RESOURCEPOOLID<br>ROLEID<br>SCHEDULEID<br>TIMESHEETPROFILEID<br>UITEMPLATEID<br>USERID<br>UMUSERID</td>
        <td>ACCESSLEVELS_CURRENT |ACCESSLEVELID<br>CATEGORIES_CURRENT | CATEGORYID<br>COMPANIES_CURRENT | COMPANYID <br>HOURTYPE_CURRENT | HOURTYPEID<br>USER_CURRENT | USERID<br>Non-relation ; utilisé à des fins d’application interne<br>USER_CURRENT | USERID<br>GROUP_CURRENT | GROUPID<br>TEAM_CURRENT | TEAMID<br>REMARQUE_CURRENT | NOTEID<br>USER_CURRENT | USERID<br>REMARQUE_CURRENT | NOTEID<br>La table Modèle de mise en page ne sera pas prise en charge<br>USER_CURRENT | USERID<br>La table Profil du portail ne sera pas prise en charge<br>Aucune relation ; utilisée à des fins d’application interne<br>RATECARD_CURRENT | RATECARDID<br>RESOURCEPOOLS_CURRENT | RESOURCEPOOLID<br>ROLE_CURRENT | ROLEID<br>SCHEDULE_CURRENT | SCHEDULEID<br>TIMESHEETPROFILES_CURRENT | TIMESHEETPROFILEID<br>UITEMPLATES_CURRENT |UITEMPLATEID<br>Self<br>Aucune relation ; utilisé à des fins d’application interne</td>
    </tr>
    <tr>
        <td>Délégation d'utilisateur</td>
        <td>Délégation d'utilisateur</td>
        <td>USRDEL | Délégation d’utilisateurs</td>
        <td>USERDELEGATIONS_CURRENT<br>USERDELEGATIONS_DAILY_HISTORY<br>USERDELEGATIONS_EVENT</td>
        <td>FROMUSERID<br>SYSID <br>TOUSERID <br>USERDELEGATIONID (self)</td>
        <td>USERS_CURRENT | USERID<br>Non-relation ; utilisé à des fins d’application interne <br>USERS_CURRENT | USERID <br> Self</td>
    </tr>
    <tr>
        <td>Groupe d'utilisateurs</td>
        <td>Autres groupes</td>
        <td>USRGPS | Groupe d’utilisateurs</td>
        <td>USERSGROUPS_CURRENT<br>USERSGROUPS_DAILY_HISTORY<br>USERSGROUPS_EVENT</td>
        <td>GROUPID <br>SYSID<br>USERID <br>USERSGROUPID (self)</td>
        <td>GROUPS_CURRENT | GROUPID <br>Non-relation ; utilisé à des fins d’application interne<br>USERS_CURRENT | USERID <br> Self</td>
    </tr>
    <tr>
        <td>Rôle utilisateur</td>
        <td>Autres rôles</td>
        <td>USRROL | Rôle d’utilisateur</td>
        <td>USERSROLES_CURRENT<br>USERSROLES_DAILY_HISTORY<br>USERSROLES_EVENT</td>
        <td>ROLEID <br>SYSID<br>USERID    <br>USERROLESETID<br>USERSROLEID (self)</td>
        <td>ROLES_CURRENT | ROLEID <br>Non-relation ; utilisé à des fins d’application interne<br>USERS_CURRENT | USERID    <br>USERROLESET_CURRENT | USERROLESETID<br>Self</td>
    </tr>
    <tr>
        <td>UserPrefValue</td>
        <td>UserPrefValue</td>
        <td>USERPF | Préférences utilisateur</td>
        <td>USERPREFVALUES_CURRENT<br>USERPREFVALUES_DAILY_HISTORY<br>USERPREFVALUES_EVENT</td>
        <td>SYSID    <br>USERID <br>USERPREFVALUEID (self)</td>
        <td>Pas une relation ; utilisé à des fins d’application interne<br>USERS_CURRENT | USERID    <br> self</td>
    </tr>
    <tr>
        <td>UserRoleSet</td>
        <td>UserRoleSet</td>
        <td>URSET | UserRoleSet</td>
        <td>USERROLESET_CURRENT<br>USERROLESET_DAILY_HISTORY<br>USERROLESET_EVENT</td>
        <td>PRIMARYROLEID <br>SYSID<br>USERID    <br>USERROLESETID (self)</td>
        <td>ROLES_CURRENT | ROLEID <br>Non-relation ; utilisé à des fins d’application interne<br>USERS_CURRENT | USERID <br> Self</td>
    </tr>
    <tr>
        <td>UsersDecisions</td>
        <td>Décisions des utilisateurs et utilisatrices</td>
        <td>USRDEC | Décisions des utilisateurs</td>
        <td>USERSDECISIONS_CURRENT<br>USERSDECISIONS_DAILY_HISTORY<br>USERSDECISIONS_EVENT</td>
        <td>USERDECISIONID (self)<br>SYSID <br>USERID  </td>
        <td>Self<br>Aucune relation ; utilisée à des fins d’application interne <br>USERS_CURRENT | USERID </td>
    </tr>
    <tr>
        <td>WorkItem</td>
        <td>Élément de travail</td>
        <td>WRKITM | WorkItem</td>
        <td>WORKITEMS_CURRENT<br>WORKITEMS_DAILY_HISTORY<br>WORKITEMS_EVENT</td>
        <td>ASSIGNMENTID <br>OBJID<br>OPTASKID    <br>PROJECTID <br>SYSID<br>TASKID    <br>USERID <br>WORKITEMID (self)</td>
        <td>ASSIGNMENTS_CURRENT | ASSIGNMENTID <br>ID de l’objet identifié dans le champ OBJOBJCODE<br>OPTASK_CURRENT | OPTASKID    <br>PROJECTS_CURRENT | PROJECTID <br>Non-relation ; utilisé à des fins d’application interne<br>TASKS_CURRENT | TASKID    <br>USERS_CURRENT | USERID    <br>self </td>
    </tr>
  </tbody>
</table>
