---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Dictionnaire de données de Workfront Data Connect
description: Cette page contient des informations sur la structure et le contenu des données dans Workfront Data Connect.
author: Nolan
feature: Reports and Dashboards
exl-id: 57985404-554e-4289-b871-b02d3427aa5c
source-git-commit: eccc878f4b6fdeeffbcd5635b80ac3e26f7fb8c6
workflow-type: tm+mt
source-wordcount: '4719'
ht-degree: 4%

---

# Dictionnaire de données de Workfront Data Connect

Cette page contient des informations sur la structure et le contenu des données dans Workfront Data Connect.

>[!NOTE]
>
>Les données de Data Connect sont actualisées toutes les quatre heures, de sorte que les modifications récentes peuvent ne pas être immédiatement répercutées.

## Types de table

Il existe plusieurs types de tableau que vous pouvez utiliser dans Data Connect pour afficher vos données Workfront de manière à fournir le plus d’informations possible.

* **Table actuelle**

  Le tableau actuel reflète les données de la même manière qu’il existe dans Workfront, chaque objet et son état actuel. Cependant, la latence de navigation est bien inférieure dans Workfront.

* **Tableau des événements**

  Le tableau Événement suit chaque enregistrement de modification dans Workfront : en d’autres termes, chaque fois qu’un objet change d’état, un enregistrement est créé pour indiquer la date de la modification, l’auteur de la modification et ce qui a été modifié. Par conséquent, ce tableau est utile pour les comparaisons ponctuelles. Ce tableau ne comprend que les enregistrements des trois dernières années.

* **Tableau Historique quotidien**

  Le tableau Historique quotidien offre une version abrégée du tableau Événement , dans la mesure où il indique l’état de chaque objet sur une base quotidienne plutôt que la date à laquelle chaque événement individuel s’est produit. Par conséquent, ce tableau est utile pour l’analyse des tendances.

<!-- Custom table -->

## Diagramme de relation d’entité

Les objets dans Workfront (et, par conséquent, dans votre lac de données Data Connect) sont définis non seulement par leurs valeurs individuelles, mais également par leurs relations avec d’autres objets. Le diagramme de relation d’entité ci-dessous fournit un mappage de haut niveau des relations d’objet dans Data Connect. Le diagramme peut être visualisé et téléchargé à l’aide du lien suivant :

[Diagramme de relation de l’entité Data Connect](/help/quicksilver/reports-and-dashboards/data-lake/assets/Workfront-data-lake_entity-relationship-diagram.pdf)

>[!IMPORTANT]
>
>Le diagramme de relation d’entité est un travail en cours. Il est fourni à titre de référence uniquement et peut faire l’objet de modifications.

## Types de date

Plusieurs objets de date fournissent des informations sur le moment où des événements spécifiques se produisent.

* `DL_LOAD_TIMESTAMP` : cette date sert de référence interne et indique le moment où les données ont été chargées dans la table En cours, Événement ou Historique quotidien. Cette date ne doit pas être utilisée pour l’analyse des données et doit être supprimée pendant la phase bêta du lac de données Workfront.
* `CALENDAR_DATE` : cette date est uniquement présente dans le tableau Historique quotidien. Ce tableau fournit un enregistrement de l’aspect des données à 11 h 59 UTC pour chaque date spécifiée dans `CALENDAR_DATE`.
* `BEGIN_EFFECTIVE_TIMESTAMP` : cette date est présente dans les tableaux Événement et Historique quotidien et enregistre exactement quand un enregistrement est modifié _en_ la valeur qu&#39;il a dans la ligne active.
* `END_EFFECTIVE_TIMESTAMP` : Cette date est présente dans les tables Historique des événements et Historique quotidien et enregistre exactement le moment où un enregistrement est passé _de_ la valeur de la ligne active à une valeur d&#39;une autre ligne. Pour permettre la comparaison entre les requêtes sur `BEGIN_EFFECTIVE_TIMESTAMP` et `END_EFFECTIVE_TIMESTAMP`, cette valeur n’est jamais nulle, même s’il n’existe aucune nouvelle valeur. Dans le cas où un enregistrement est toujours valide (c’est-à-dire, que la valeur n’a pas changé), `END_EFFECTIVE_TIMESTAMP` aura une valeur de 2300-01-01.

## Table de terminologie

Le tableau suivant met en corrélation les noms d’objet dans Workfront (ainsi que leurs noms dans l’interface et l’API) avec leurs noms équivalents dans Data Connect.

<table>
  <thead>
    <tr>
        <th>Nom de l’entité Workfront</th>
        <th>Références d’interface</th>
        <th>Référence d’API | Libellé</th>
        <th>Tableaux du lac de données</th>
        <th>Champ Relations</th>
        <th>Table et champ de relation</th>
    </tr>
  </thead>
  <tbody>
    <tr>
        <td>Niveau d’accès</td>
        <td>Niveau d’accès</td>
        <td>ACSLVL | Niveau d'accès</td>
        <td>ACCESSLEVELS_CURRENT<br>ACCESSLEVELS_DAILY_HISTORY<br>ACCESSLEVELS_EVENT</td>
        <td>ACCESSLEVELS (self)<br>APPGLOBALID<br>LASTUPDATEDBYID<br>LEGACYACCESSLEVELS<br>OBJID<br>SYSID</td>
        <td>Self<br>Not a relation ; utilisé à des fins d’application interne<br>USER_CURRENT | USERID<br>Pas de relation ; utilisé à des fins d’application interne<br>Identifiant de l’objet identifié dans le champ OBJCODE<br>Pas de relation ; utilisé à des fins d’application interne</td>
    </tr>
    <tr>
        <td>Règle d'accès</td>
        <td>Partager</td>
        <td>ACSRUL | Partager</td>
        <td>ACCESSRULES_CURRENT<br>ACCESSRULES_DAILY_HISTORY<br>ACCESSRULES_EVENT</td>
        <td>ACCESSORID <br>ACCESSRULEID (self) <br>ANCESTORID <br>LASTUPDATEDBYID <br>SECURITYOBJID <br>SYSID</td>
        <td>ID de l’objet identifié dans le champ ACCESSOROBJCODE <br>Self<br>ID de l’objet identifié dans le champ ANCESTOROBJCODE<br>USERS_CURRENT | USERID<br>ID de l’objet identifié dans le champ SECURITYOBJCODE<br>Pas de relation ; utilisé à des fins d’application interne.</td>
    </tr>
    <tr>
        <td>Chemin d'approbation</td>
        <td>Chemin d'approbation</td>
        <td>ARVPTH | Approbation</td>
        <td>APPROVALPATHS_CURRENT<br>APPROVALPATHS_DAILY_HISTORY<br>APPROVALPATHS_EVENT</td>
        <td>APPROVALPATHID (self) <br>APPROVALPROCESSID <br>ENTEREDBYID <br>GLOBALPATHID <br>LASTUPDATEDBYID <br>SYSID</td>
        <td>Self<br>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>USERS_CURRENT | USERID<br>Pas une relation ; utilisé à des fins d’application interne<br>USERS_CURRENT | USERID<br>pas une relation ; utilisé à des fins d’application interne.</td>
    </tr>
    <tr>
        <td>Processus d’approbation</td>
        <td>Processus d’approbation</td>
        <td>ARVPRC | Processus d'approbation</td>
        <td>APPROVALPROCESSES_CURRENT<br>APPROVALPROCESSES_DAILY_HISTORY<br>APPROVALPROCESSES_EVENT</td>
        <td>APPROVALPROCESSID (self) <br>ENTEREDBYID <br>LASTUPDATEDBYID<br>SYSID</td>
        <td>Self<br>USERS_CURRENT | USERID<br>USERS_CURRENT | USERID<br>pas une relation ; utilisé à des fins d’application interne.</td>
    </tr>
    <tr>
        <td>Étape d’approbation</td>
        <td>Étape d’approbation</td>
        <td>ARVSTP | Étape d'approbation</td>
        <td>APPROVALSTEPS_CURRENT<br>APPROVALSTEPS_DAILY_HISTORY<br>APPROVALSTEPS_EVENT</td>
        <td>APPROVALPATHID <br>APPROVALSTEPID (self) <br>SYSID</td>
        <td>APPROVALPATHS_CURRENT | APPROVALPATHID<br>Self<br>Not a Relationship ; utilisé pour les applications internes</td>
    </tr>
    <tr>
        <td>ApproverStatus</td>
        <td>Statut de l'approbateur</td>
        <td>ARVSTS | ApproverStatus</td>
        <td>APPROVERSTATUSES_CURRENT<br>APPROVERSTATUSES_DAILY_HISTORY<br>APPROVERSTATUSES_EVENT</td>
        <td>APPROVERSTATUSID (SELF)<br>APPROVABLEOBJID<br>APPROVALSTEPID<br>APPROVEDBYID <br>DELEGATEUSERID<br>LASTUPDATEDBYID <br>OPTASKID<br>OVERRIDDENUSERID<br>PROJECTID<br>STEPAPPROVERID<br>SYSID<br>TASKID<br>WILDCARDUSERID</td>
        <td>Self<br>ID de l’objet identifié dans le champ APPROVABLEOBJCODE<br>APPROVALSTEPS_CURRENT | APPROVALSTEPID<br>USERS_CURRENT | USERID <br>USERS_CURRENT | USERID<br>USERS_CURRENT | USERID <br>OPTASKS_CURRENT | OPTASKID<br>USERS_CURRENT | USERID<br>PROJECTS_CURRENT | PROJECTID<br>USERS_CURRENT | USERID<br>Pas une relation ; utilisé à des fins d’application interne<br>TASKS_CURRENT | TASKID<br>USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Affectation</td>
        <td>Affectation</td>
        <td>AFFECTER | Affectation</td>
        <td>ASSIGNMENTS_CURRENT<br>ASSIGNMENTS_DAILY_HISTORY<br>ASSIGNMENTS_EVENT</td>
        <td>ASSIGNEDBYID<br>ASSIGNEDTOID<br>ASSIGNMENTID (SELF)<br>CATEGORYID<br>CLASSIFIERID<br>OPTASKID<br>PRIVATERATECARDID<br>PROJECTID<br>ROLEID<br>TASKID<br>TEAMID</td>
        <td>USER_CURRENT | USERID<br>USER_CURRENT | USERID<br>Self<br>CATEGORIES_CURRENT | La table CATEGORYID<br>Classifier n'est pas prise en charge actuellement<br>OPTASK_CURRENT | OPTASKID<br>RATECARD_CURRENT | RATECARDID<br>PROJECT_CURRENT | PROJECTID<br>ROLE_CURRENT | ROLEID<br>TASK_CURRENT | TASKID<br>TEAM_CURRENT | TEAMID</td>
    </tr>
    <tr>
        <td>Approbations en attente</td>
        <td>Approbations en attente</td>
        <td>AWAPVL | Approbation en attente</td>
        <td>AWAITINGAPPROVALS_CURRENT<br>AWAITINGAPPROVALS_DAILY_HISTORY<br>AWAITINGAPPROVALS_EVENT</td>
        <td>ACCESSREQUESTID<br>APPROVABLEID <br>APPROVERID <br>AWAITINGAPPROVALID (SELF) <br>DOCUMENTID <br>DOCUMENTVERSIONID<br>OPTASKID <br>PROJECTID <br>ROLEID <br>SUBMITTEDBYID <br>SYSID<br>TASKID <br>TEAMID <br>TIMESHEETID<br>USERID</td>
        <td>Table des demandes d’accès non prise en charge actuellement<br>Il ne s’agit pas d’une relation ; utilisée à des fins d’application interne<br>USERS_CURRENT | USERID<br>Self<br>DOCUMENTS_CURRENT | DOCUMENTID<br>DOCUMENTVERSIONS_CURRENT | DOCUMENTVERSIONID<br>OPTASKS_CURRENT | OPTASKID<br>PROJECTS_CURRENT | PROJECTID<br>ROLES_CURRENT | ROLEID<br>USERS_CURRENT | USERID<br>Pas une relation ; utilisé à des fins d’application interne<br>TASKS_CURRENT | TASKID<br>TEAMS_CURRENT | TEAMID<br>TIMESHEETS_CURRENT | TIMESHEETID<br>USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Niveau de référence</td>
        <td>Niveau de référence</td>
        <td>AVEUGLE | Ligne de base</td>
        <td>BASELINES_CURRENT<br>BASELINES_DAILY_HISTORY<br>BASELINES_EVENT</td>
        <td>BASELINEID (self)<br>EXCHANGERATEID <br>PROJECTID <br>SYSID</td>
        <td>Self<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>PROJECTS_CURRENT | PROJECTID<br>pas une relation ; utilisé à des fins d’application interne</td>
    </tr>
    <tr>
        <td>Tâche de ligne de base</td>
        <td>Tâche de ligne de base</td>
        <td>BSTSK | Tâche de niveau de référence</td>
        <td>BASELINETASKS_CURRENT<br>BASELINETASKS_DAILY_HISTORY<br>BASELINETASKS_EVENT</td>
        <td>BASELINEID<br>BASELINETASKID (self) <br>EXCHANGERATEID <br>PROJECTID <br>SYSID<br>TASKID</td>
        <td>BASELINES_CURRENT | BASELINEID<br>Self<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>PROJECTS_CURRENT | PROJECTID<br>Pas une relation ; utilisé à des fins d’application interne<br>TASKS_CURRENT | TASKID</td>
    </tr>
    <tr>
        <td>Taux de facturation</td>
        <td>Taux ou taux de remplacement</td>
        <td>TAUX | Taux de facturation</td>
        <td>RATES_CURRENT<br>RATES_DAILY_HISTORY<br>RATES_EVENT</td>
        <td>ASSIGNMENTID<br>CLASSIFIERID<br>EXCHANGERATEID<br>NLBRCATEGORYID<br>NONLABORRESOURCEID<br>OBJID<br>PROJECTID <br>RATECARDID<br>RATEID (SELF)<br>ROLEID <br>SOURCERATECARDID <br>SYSID <br>TEMPLATEID<br>USERID</td>
        <td>ASSIGNMENTS_CURRENT | Table ASSIGNMENTID<br>Classifier non prise en charge actuellement<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>Table des catégories de ressources non liées à la main-d'œuvre non prise en charge actuellement<br>NONLABORRESOURCES_CURRENT | NONLABORRESOURCEID<br>ID de l’objet identifié dans le champ OBJCODE<br>PROJECTS_CURRENT | PROJECTID <br>RATECARD_CURRENT | RATECARDID<br>Self<br>ROLES_CURRENT | ROLEID <br>RATECARD_CURRENT | RATECARDID <br>relation inexistante ; utilisé pour les applications internes <br>TEMPLATES_CURRENT | TEMPLATEID<br>USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Enregistrement de facturation</td>
        <td>Enregistrement de facturation</td>
        <td>FACTURE | Enregistrement de facturation</td>
        <td>BILLINGRECORDS_CURRENT<br>BILLINGRECORDS_DAILY_HISTORY<br>BILLINGRECORDS_EVENT</td>
        <td>BILLINGRECORDID (SELF)<br>CATEGORYID<br>EXCHANGERATEID <br>INVOICEID <br>LASTUPDATEDBYID <br>PROJECTID <br>SYSID</td>
        <td>Self<br>CATEGORIES_CURRENT | CATEGORYID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID <br>Table des factures non prise en charge actuellement <br>USERS_CURRENT | USERID <br>PROJECTS_CURRENT | PROJECTID   <br>Pas une relation ; utilisé à des fins d’application interne.</td>
    </tr>
    <tr>
        <td>Réservation</td>
        <td>Réservation</td>
        <td>RÉSERVATION | Réservation</td>
        <td>BOOKINGS_CURRENT<br>BOOKINGS_DAILY_HISTORY<br>BOOKINGS_EVENT</td>
        <td>BOOKINGID (SELF)<br>ENTEREDBYID<br>LASTUPDATEDBYID<br>NLBRCATEGORYID<br>NONLABORRESOURCEID<br>OBJID<br>PROJECTID<br>SYSID<br>TASKID<br>TEMPLATEID<br>TEMPLATETASKID<br>TOPOBJID</td>
        <td>Self<br>USERS_CURRENT | USERID<br>USERS_CURRENT | USERID<br>Table des catégories de ressources hors main-d'œuvre non prise en charge actuellement<br>NONLABORRESOURCES_CURRENT | NONLABORRESOURCEID<br>ID de l’objet identifié dans le champ OBJOBJCODE<br>PROJECTS_CURRENT | PROJECTID <br>pas une relation ; utilisé à des fins d’application interne<br>TASKS_CURRENT | TASKID<br>TEMPLATES_CURRENT | TEMPLATEID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID <br> ID de l’objet identifié dans le champ TOPOBJCODE</td>
    </tr>
    <tr>
        <td>Profil professionnel</td>
        <td>Profil professionnel</td>
        <td>BSNPRF | BusinessProfile</td>
        <td>BUSINESSPROFILE_CURRENT<br>BUSINESSPROFILE_DAILY_HISTORY<br>BUSINESSPROFILE_EVENT</td>
        <td>ACCESSLEVELS<br>BUSINESSPROFILEID (self)<br>ENTEREDBYID<br>GROUPID<br>LASTUPDATEDBYID<br>SYSID</td>
        <td>ACCESSLEVELS_CURRENT | ACCESSLEVELS<br>Self<br>USERS_CURRENT | USERID<br>GROUPS_CURRENT | GROUPID<br>USERS_CURRENT | USERID<br>pas une relation ; utilisé à des fins d’application interne.</td>
    </tr>
    <tr>
        <td>Règles métier</td>
        <td>Règles métier</td>
        <td>BNRUL | Règle métier</td>
        <td>BUSINESSRULE_CURRENT<br>BUSINESSRULE_DAILY_HISTORY<br>BUSINESSRULE_EVENT</td>
        <td>BUSINESSRULEID (SELF)<br>ENTEREDBYID<br>LASTUPDATEDBYID<br>SYSID</td>
        <td>Self<br>USERS_CURRENT | USERID<br>USERS_CURRENT | USERID<br>pas une relation ; utilisé à des fins d’application interne.</td>
    </tr>
    <tr>
        <td>Catégorie</td>
        <td>Formulaire personnalisé</td>
        <td>VINGT | Catégorie</td>
        <td>CATEGORIES_CURRENT<br>CATEGORIES_DAILY_HISTORY<br>CATEGORIES_EVENT</td>
        <td>CATEGORYID (self)<br>ENTEREDBYID<br>GROUPID<br>LASTUPDATEDBYID<br>SYSID</td>
        <td>Self<br>USERS_CURRENT | USERID<br>GROUPS_CURRENT | GROUPID<br>USERS_CURRENT | USERID<br>pas une relation ; utilisé à des fins d’application interne.</td>
    </tr>
    <tr>
        <td>Paramètre de catégorie</td>
        <td>Champs de formulaire personnalisés</td>
        <td>CTGYPA | Paramètre de catégorie</td>
        <td>CATEGORIESPARAMETERS_CURRENT<br>CATEGORIESPARAMETERS_DAILY_HISTORY<br>CATEGORIESPARAMETERS_EVENT</td>
        <td>CATEGORIESPARAMETERID (SELF)<br>CATEGORYID<br>PARAMETERGROUPID<br>PARAMETERID<br>SYSID</td>
        <td>Self<br>CATEGORIES_CURRENT | CATEGORYID<br>Table de groupes de paramètres non prise en charge actuellement<br>PARAMETERS_CURRENT | PARAMETERID    <br>Pas une relation ; utilisé à des fins d’application interne.</td>
    </tr>
    <tr>
        <td>Classificateur</td>
        <td>Emplacement</td>
        <td>CLSF | Lieu</td>
        <td>CLASSIFIER_CURRENT<br>CLASSIFIER_DAILY_HISTORY<br>CLASSIFIER_EVENT</td>
        <td>CLASSIFIERID (SELF)<br>ENTEREDBYID<br>LASTUPDATEDBYID<br>PARENTID<br>SYSID</td>
        <td>Self<br>USERS_CURRENT | USERID<br>USERS_CURRENT | USERID<br>CLASSIFIER_CURRENT | CLASSIFIERID<br>pas une relation ; utilisé à des fins d’application interne</td>
    </tr>
    <tr>
        <td>Entreprise</td>
        <td>Entreprise</td>
        <td>COPY | Société</td>
        <td>COMPANIES_CURRENT<br>COMPANIES_DAILY_HISTORY<br>COMPANIES_EVENT</td>
        <td>CATEGORYID<br>COMPANYID (SELF)<br>ENTEREDBYID<br>GROUPID<br>LASTUPDATEDBYID<br>PRIVATERATECARDID<br>SYSID</td>
        <td>CATEGORIES_CURRENT | CATEGORYID<br>Self<br>USERS_CURRENT | USERID <br>GROUPS_CURRENT | GROUPID<br>USERS_CURRENT | USERID <br>RATECARD_CURRENT | RATECARDID<br>pas une relation ; utilisé pour les applications internes</td>
    </tr>
    <tr>
        <td>Trimestre personnalisé</td>
        <td>Trimestre personnalisé</td>
        <td>DÉMARRER | Trimestre personnalisé</td>
        <td>CUSTOMQUARTERS_CURRENT<br>CUSTOMQUARTERS_DAILY_HISTORY<br>CUSTOMQUARTERS_EVENT</td>
        <td>CUSTOMQUARTERID (self) <br>SYSID</td>
        <td>Self<br>Not a Relationship ; utilisé pour des applications internes</td>
    </tr>
    <tr>
        <td>CustomEnum</td>
        <td>Statut, Priorité, Gravité, Statut</td>
        <td>SYSTÈME | Énumération personnalisée</td>
        <td>CUSTOMENUMS_CURRENT<br>CUSTOMENUMS_DAILY_HISTORY<br>CUSTOMENUMS_EVENT<br>* Le type d’enregistrement est identifié via la propriété « enumClass ». Voici les types attendus :<br>CONDITION_OPTASK<br>CONDITION_PROJ<br>CONDITION_TASK<br>PRIORITY_OPTASK<br>PRIORITY_PROJ<br>PRIORITY_TASK<br>SEVERITY_OPTASK<br>STATUS_OPTASK<br>STATUS_PROJ<br>STATUS_TASK</td>
        <td>ENTEREDBYID<br>GROUPID</td>
        <td>USER_CURRENT | USERID<br>GROUP_CURRENT | GROUPID</td>
    </tr>
    <tr>
        <td>Document</td>
        <td>Document</td>
        <td>DOC | Document</td>
        <td>DOCUMENTS_CURRENT<br>DOCUMENTS_DAILY_HISTORY<br>DOCUMENTS_EVENT<br>DOCUMENTS_CUSTOM_VALUE_CURRENT<br>DOCUMENTS_CUSTOM_VALUE_DAILY_HISTORY<br>DOCUMENTS_CUSTOM_VALUE_EVENT</td>
        <td>CATEGORYID<br>CHECKEDOUTBYID<br>DOCUMENTID<br>DOCUMENTREQUESTID<br>EXCHANGERATEID<br>ITERATIONID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>NOTEID<br>OBJID<br>OPTASKID<br>OWNERID<br>PORTFOLIOID<br>PROGRAMID<br>PROJECTID<br>RELEASEVERSIONID<br>TASKID<br>TEMPLATEID<br>TEMPLATETASKID<br>TOPOBJID<br>USERID</td>
        <td>CATEGORIES_CURRENT | CATEGORYID<br>USER_CURRENT | La table de demandes USERID<br>Self<br>Document n'est pas prise en charge actuellement<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>ITERATIONS_CURRENT | ITERATIONID<br>NOTE_CURRENT | NOTEID<br>USER_CURRENT | USERID<br>NOTE_CURRENT | NOTEID<br>Variable en fonction de DOCOBJCODE value<br>OPTASK_CURRENT | OPTASKID<br>USER_CURRENT | USERID<br>PORTFOLIO_CURRENT | PORTFOLIOID<br>PROGRAM_CURRENT | PROGRAMID<br>PROJECT_CURRENT | PROJECTID<br>Release Table non prise en charge actuellement<br>TASK_CURRENT | TASKID<br>TEMPLATES_CURRENT | TEMPLATEID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID<br>Variable en fonction de la valeur TOPOBJCODE<br>USER_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Approbation du document</td>
        <td>Approbation du document</td>
        <td>DOCAPL | Approbation du document</td>
        <td>DOCAPPROVALS_CURRENT<br>DOCAPPROVALS_DAILY_HISTORY<br>DOCAPPROVALS_EVENT</td>
        <td>APPROVERID<br>DOCAPPROVALID (SELF)<br>DOCUMENTID<br>NOTEID<br>REQUESTORID<br>SYSID</td>
        <td>USERS_CURRENT | USERID <br>Self<br>DOCUMENTS_CURRENT | DOCUMENTID<br>NOTES_CURRENT | NOTEID<br>USERS_CURRENT | USERID <br>pas une relation ; utilisé à des fins d’application interne.</td>
    </tr>
    <tr>
        <td>Dossier de documents</td>
        <td>Dossier de documents</td>
        <td>DOCFLD | DocsFolders</td>
        <td>DOCFOLDERS_CURRENT<br>DOCFOLDERS_DAILY_HISTORY<br>DOCFOLDERS_EVENT</td>
        <td>DOCFOLDERID (self)<br>ENTEREDBYID<br>ISSUEID<br>ITERATIONID    <br>LINKEDFOLDERID<br>PARENTID<br>PORTFOLIOID <br>PROGRAMID    <br>PROJECTID<br>SYSID<br>TASKID     <br>TEMPLATEID<br>TEMPLATETASKID<br>USERID</td>
        <td>Self<br>USERS_CURRENT | USERID<br>OPTASKS_CURRENT | OPTASKID<br>ITERATIONS_CURRENT | ITERATIONID<br>LINKEDFOLDERS_CURRENT | LINKEDFOLDERID<br>DOCFOLDERS_CURRENT | DOCFOLDERID<br>PORTFOLIO_CURRENT | PORTFOLIOID <br>PROGRAM_CURRENT | PROGRAMID    <br>PROJECTS_CURRENT | PROJECTID <br>pas une relation ; utilisé à des fins d’application interne<br>TASKS_CURRENT | TASKID     <br>TEMPLATES_CURRENT | TEMPLATEID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID<br>USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>DocumentProvideMetadata</td>
        <td>Métadonnées fournies par le document</td>
        <td>DOCUMENT | DocumentProviderMetadata</td>
        <td>DOCPROVIDERMETA_CURRENT<br>DOCPROVIDERMETA_DAILY_HISTORY<br>DOCPROVIDERMETA_EVENT</td>
        <td>DOCPROVIDERMETAID (self) <br>SYSID</td>
        <td>Self<br>Not a Relationship ; utilisé pour des applications internes</td>
    </tr>
    <tr>
        <td>DocumentProvider</td>
        <td>Fournisseur de documents</td>
        <td>DOCPRO | Fournisseur de documents</td>
        <td>DOCPROVIDERS_CURRENT<br>DOCPROVIDERS_DAILY_HISTORY<br>DOCPROVIDERS_EVENT</td>
        <td>DOCPROVIDERCONFIGID<br>DOCPROVIDERID (self)<br>OWNERID    <br>SYSID</td>
        <td>DOCPROVIDERCONFIG_CURRENT | DOCPROVIDERCONFIGID<br>Self<br>USERS_CURRENT | USERID    <br>Pas une relation ; utilisé à des fins d’application interne.</td>
    </tr>
    <tr>
        <td>DocumentProviderConfig</td>
        <td>Configuration du fournisseur de documents</td>
        <td>DOCCFG | DocumentProviderConfig</td>
        <td>DOCPROVIDERCONFIG_CURRENT<br>DOCPROVIDERCONFIG_DAILY_HISTORY<br>DOCPROVIDERCONFIG_EVENT</td>
        <td>DOCPROVIDERCONFIGID (SELF)<br>SYSID</td>
        <td>Self<br>Not a Relationship ; utilisé pour des applications internes</td>
    </tr>
    <tr>
        <td>DocumentVersion</td>
        <td>Version du document</td>
        <td>DOCV | Version du document</td>
        <td>DOCUMENTVERSIONS_CURRENT<br>DOCUMENTVERSIONS_DAILY_HISTORY<br>DOCUMENTVERSIONS_EVENT</td>
        <td>DOCUMENTID<br>DOCUMENTPROVIDERID<br>DOCUMENTVERSIONID<br>ENTEREDBYID<br>EXTERNALSTORAGEID<br>PROOFAPPROVALSTATUSID<br>PROOFEDBYUSERID<br>PROOFID<br>PROOFOWNERID<br>PROOFSTAGEID</td>
        <td>DOCUMENT_CURRENT | DOCUMENTID<br>DOCPROVIDERS_CURRENT | DOCUMENTPROVIDERID<br>Self<br>USER_CURRENT | La table USERID<br>ID externe<br>Statut d'approbation de l'épreuve n'est pas prise en charge actuellement<br>USER_CURRENT | La table USERID<br>Proof n'est pas prise en charge actuellement<br>USER_CURRENT | La table d'étape USERID<br>Proof n'est pas prise en charge actuellement</td>
    </tr>
    <tr>
        <td>Taux de change</td>
        <td>Taux de change</td>
        <td>EXRATE | Taux de change</td>
        <td>EXCHANGERATES_CURRENT<br>EXCHANGERATES_DAILY_HISTORY<br>EXCHANGERATES_EVENT</td>
        <td>EXCHANGERATEID (self)<br>PROJECTID<br>SYSID <br>TEMPLATEID  </td>
        <td>Self<br>PROJECTS_CURRENT | PROJECTID <br>pas une relation ; utilisé à des fins d’application interne <br>TEMPLATES_CURRENT | TEMPLATEID  </td>
    </tr>
    <tr>
        <td>Frais</td>
        <td>Frais</td>
        <td>EXPNS | Dépense</td>
        <td>EXPENSES_CURRENT<br>EXPENSES_DAILY_HISTORY<br>EXPENSES_EVENT</td>
        <td>BILLINGRECORDID<br>CATEGORYID<br>ENTEREDBYID<br>EXCHANGERATEID <br>EXPENSEID (SELF) <br>EXPENSETYPEID <br>LASTUPDATEDBYID <br>OBJID <br>PROJECTID<br>SYSID<br>TASKID<br>TEMPLATEID<br>TEMPLATETASKID<br>TOPOBJID</td>
        <td>BILLINGRECORDS_CURRENT | BILLINGRECORDID<br>CATEGORIES_CURRENT | CATEGORYID<br>USERS_CURRENT | USERID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID <br>Self <br>EXPENSETYPES_CURRENT | EXPENSETYPEID <br>USERS_CURRENT | USERID <br>ID de l’objet identifié dans le champ OBJCODE <br>PROJECTS_CURRENT | PROJECTID <br>pas une relation ; utilisé à des fins d’application interne<br>TASKS_CURRENT | TASKID<br>TEMPLATES_CURRENT | TEMPLATEID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID <br> ID de l’objet identifié dans le champ TOPOBJCODE</td>
    </tr>
    <tr>
        <td>Type de frais</td>
        <td>Type de frais</td>
        <td>EXPTYP | Type de dépense</td>
        <td>EXPENSETYPES_CURRENT<br>EXPENSETYPES_DAILY_HISTORY<br>EXPENSETYPES_EVENT</td>
        <td>APPGLOBALID<br>EXPENSETYPEID (self)<br>OBJID <br>SYSID  </td>
        <td>Non une relation ; utilisé à des fins d’application interne<br>Self<br>Identifiant de l’objet identifié dans le champ OBJCODE <br>Non une relation ; utilisé à des fins d’application interne  </td>
    </tr>
    <tr>
        <td>Groupe</td>
        <td>Groupe</td>
        <td>GROUPE | Groupe</td>
        <td>GROUPS_CURRENT<br>GROUPS_DAILY_HISTORY<br>GROUPS_EVENT</td>
        <td>BUSINESSLEADERID<br>CATEGORYID<br>ENTEREDBYID<br>GROUPID<br>LAYOUTTEMPLATEID<br>PARENTID<br>ROOTID<br>UITEMPLATEID</td>
        <td>USER_CURRENT | USERID<br>CATEGORIES_CURRENT | CATEGORYID<br>USER_CURRENT | Le tableau USERID<br>Self<br>Layout Template ne sera pas pris en charge<br>GROUP_CURRENT | GROUPID<br>GROUP_CURRENT | GROUPID<br>UITEMPLATES_CURRENT | UITEMPLATEID</td>
    </tr>
    <tr>
        <td>Heure</td>
        <td>Heure</td>
        <td>HEURE | Heure</td>
        <td>HOURS_CURRENT<br>HOURS_DAILY_HISTORY<br>HOURS_EVENT</td>
        <td>APPROVEDBYID<br>BILLINGRECORDID<br>CATEGORYID<br>CLASSIFIERID<br>DUPID<br>EXCHANGERATEID<br>EXTERNALTIMESHEETID<br>HOURID<br>HOURTYPEID<br>LASTUPDATEDBYID<br>OPTASKID<br>OWNERID<br>PROJECTID<br>PROJECTOVERHEADID<br>ROLEID<br>TASKID<br>TIMESHEETID</td>
        <td>USER_CURRENT | USERID<br>BILLINGRECORDS_CURRENT | BILLINGRECORDID<br>CATEGORIES_CURRENT | La table CATEGORYID<br>Classifier n'est actuellement pas prise en charge<br>Il ne s'agit pas d'une relation ; utilisée à des fins d'application interne<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>relation non Workfront ; utilisé pour l’intégration à des systèmes externes<br>Self<br>HOURTYPE_CURRENT | HOURTYPEID<br>USER_CURRENT | USERID<br>OPTASK_CURRENT | OPTASKID<br>USER_CURRENT | USERID<br>PROJECT_CURRENT | PROJECTID<br>Pas de relation ; utilisé à des fins d’application interne<br>ROLE_CURRENT | ROLEID<br>TASK_CURRENT | TASKID<br>TIMESHEET_CURRENT | TIMESHEETID</td>
    </tr>
    <tr>
        <td>Type d’heure</td>
        <td>Type d’heure</td>
        <td>HEURE | Type d'heures</td>
        <td>HOURTYPES_CURRENT</td>
        <td>APPGLOBALID<br>HOURTYPEID<br>OBJID</td>
        <td>Pas une relation ; utilisé à des fins d’application interne<br>Self<br>Not a relation ; utilisé à des fins d’application interne</td>
    </tr>
    <tr>
        <td>Itération</td>
        <td>Itération</td>
        <td>RETOUR | Itération</td>
        <td>ITERATIONS_CURRENT<br>ITERATIONS_DAILY_HISTORY<br>ITERATIONS_EVENT</td>
        <td>CATEGORYID<br>ENTEREDBYID<br>ITERATIONID (SELF)<br>LASTUPDATEDBYID<br>OWNERID<br>SYSID<br>TEAMID</td>
        <td>CATEGORIES_CURRENT | CATEGORYID<br>USERS_CURRENT | USERID <br>Self<br>USERS_CURRENT | USERID <br>USERS_CURRENT | USERID <br>pas une relation ; utilisé à des fins d’application interne<br>TEAMS_CURRENT | TEAMID</td>
    </tr>
    <tr>
        <td>Entrée au journal</td>
        <td>Entrée au journal</td>
        <td>JRNLE | Entrée de journal</td>
        <td>JOURNALENTRIES_CURRENT<br>JOURNALENTRIES_DAILY_HISTORY<br>JOURNALENTRIES_EVENT</td>
        <td>APPROVERSTATUSID<br>ASSIGNMENTID<br>AUDITRECORDID<br>BASELINEID <br>BILLINGRECORDID<br>COMPANYID <br>DOCUMENTID <br>DOCUMENTSHAREID <br>EDITEDBYID<br>EXPENSEID<br>HOURID<br>INITIATIVEID<br>JOURNALENTRIEID (self)<br>OBJID<br>OPTASKID<br>PORTFOLIOID<br>PROGRAMID<br>SUBOBJID<br>SUBSCRIBEID<br>SYSID<br>TASKID<br>TEMPLATEID<br>TIMESHEETID<br>TOPOBJID<br><br> USERID</td>
        <td>APPROVERSTATUSES_CURRENT | APPROVERSTATUSID<br>ASSIGNMENTS_CURRENT | Table d'enregistrements d'audit <br>'ASSIGNMENTID non prise en charge actuellement<br>BASELINES_CURRENT | BASELINEID <br>BILLINGRECORDS_CURRENT | BILLINGRECORDID<br>COMPANIES_CURRENT | COMPANYID <br>DOCUMENTS_CURRENT | DOCUMENTID <br>Tableau de partage de documents non pris en charge actuellement <br>USERS_CURRENT | USERID<br>EXPENSES_CURRENT | EXPENSEID<br>HOURS_CURRENT | La table HOURID<br>Initiative n'est pas prise en charge actuellement<br>Self<br>ID de l'objet identifié dans le champ OBJCODE<br>OPTASKS_CURRENT | OPTASKID<br>PORTFOLIO_CURRENT | PORTFOLIOID<br>PROGRAM_CURRENT | PROGRAMID<br>PROJECTS_CURRENT | PROJECTID <br>ID de l'objet identifié dans le champ SUBOBJCODE<br>Table Subscribe non prise en charge actuellement<br>Pas de relation ; utilisé à des fins d'application interne<br>TASKS_CURRENT | TASKID<br>TEMPLATES_CURRENT | TEMPLATEID<br>TIMESHEETS_CURRENT | TIMESHEETID<br>ID de l’objet identifié dans le champ TOPOBJCODE<br>USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>LinkedFolder</td>
        <td>LinkedFolder</td>
        <td>LNKFDR | LinkedFolder</td>
        <td>LINKEDFOLDERS_CURRENT<br>LINKEDFOLDERS_DAILY_HISTORY<br>LINKEDFOLDERS_EVENT</td>
        <td>DOCUMENTPROVIDERID<br>EXTERNALSTORAGEID<br>FOLDERID<br>LINKEDBYID<br>LINKEDFOLDERID (SELF)<br>SYSID</td>
        <td>DOCPROVIDERS_CURRENT | DOCPROVIDERID<br>ID externe<br>DOCFOLDERS_CURRENT | DOCFOLDERID<br>USERS_CURRENT | USERID <br>Self<br>Not a Relationship ; utilisé pour les applications internes  </td>
    </tr>
    <tr>
        <td>Jalon</td>
        <td>Jalon</td>
        <td>MILE | Jalon</td>
        <td>MILESTONES_CURRENT<br>MILESTONES_DAILY_HISTORY<br>MILESTONES_EVENT</td>
        <td>LASTUPDATEDBYID<br>MILESTONEID<br>MILESTONEPATHID</td>
        <td>USER_CURRENT | USERID<br>Self<br>MILESTONEPATH_CURRENT | MILESTONEID</td>
    </tr>
    <tr>
        <td>MilestonePath</td>
        <td>Chemin jalonné</td>
        <td>CHEMIN | Chemin jalonné</td>
        <td>MILESTONEPATHS_CURRENT<br>MILESTONEPATHS_DAILY_HISTORY<br>MILESTONEPATHS_EVENT</td>
        <td>ENTEREDBYID<br>LASTUPDATEDBYID<br>MILESTONEPATHID</td>
        <td>USER_CURRENT | USERID<br>USER_CURRENT | USERID<br>Self</td>
    </tr>
    <tr>
        <td>Ressource non liée à la main-d’œuvre</td>
        <td>Ressource non liée à la main-d’œuvre</td>
        <td>NLBR | Ressource non liée à la main-d’œuvre</td>
        <td>NONLABORRESOURCES_CURRENT<br>NONLABORRESOURCES_DAILY_HISTORY<br>NONLABORRESOURCES_EVENT</td>
        <td>CATEGORYID<br>NONLABORRESOURCEID (SELF)<br>ENTEREDBYID<br>HOMEGROUPID<br>LASTUPDATEDBYID<br>NONLABORRESOURCECATEGORYID<br>SYSID  </td>
        <td>CATEGORIES_CURRENT | CATEGORYID<br>Self<br>USERS_CURRENT | USERID<br>GROUPS_CURRENT | GROUPID<br>USERS_CURRENT | USERID<br>Table des catégories de ressources hors main-d'œuvre non prise en charge actuellement<br>Pas de relation ; utilisé à des fins d'application interne</td>
    </tr>
    <tr>
        <td>Catégorie de ressources non liée à la main-d’œuvre</td>
        <td>Catégorie de ressources non liée à la main-d’œuvre</td>
        <td>NLBRCY | Catégorie de ressources non liées à la main-d’œuvre</td>
        <td>NLBRCATEGORIES_CURRENT<br>NLBRCATEGORIES_DAILY_HISTORY<br>NLBRCATEGORIES_EVENT</td>
        <td>CATEGORYID<br>ENTEREDBYID<br>LASTUPDATEDBYID<br>NLBRCATEGORYID (SELF)<br>PRIVATERATECARDID<br>SCHEDULEID<br>SYSID</td>
        <td>CATEGORIES_CURRENT | CATEGORYID<br>USERS_CURRENT | USERID<br>USERS_CURRENT | USERID<br>Self<br>RATECARD_CURRENT | RATECARDID<br>USERS_CURRENT | USERID<br>pas une relation ; utilisé à des fins d’application interne.</td>
    </tr>
    <tr>
        <td>Jour Non Ouvré</td>
        <td>Exception de planification</td>
        <td>NONWKD | Jour Non Ouvré</td>
        <td>NONWORKDAYS_CURRENT<br>NONWORKDAYS_DAILY_HISTORY<br>NONWORKDAYS_EVENT</td>
        <td>NONWORKDAYID (self)<br>OBJID <br>SCHEDULEID <br>SYSID <br>USERID  </td>
        <td>Self<br>ID de l’objet identifié dans le champ OBJCODE <br>SCHEDULES_CURRENT | SCHEDULEID <br>pas de relation ; utilisé à des fins d’application interne <br>USERS_CURRENT) | USERID  </td>
    </tr>
    <tr>
        <td>Note</td>
        <td>Note</td>
        <td>REMARQUE | Remarque</td>
        <td>NOTES_CURRENT<br>NOTES_DAILY_HISTORY<br>NOTES_EVENT</td>
        <td>ATTACHDOCUMENTID<br>ATTACHOBJID<br>ATTACHOPTASKID<br>ATTACHWORKID<br>ATTACHWORKUSERID<br>AUDITRECORDID<br>COMPANYID<br>DOCUMENTID<br>EXTERNALSERVICEID<br>ITERATIONID<br>NOTEID<br>OBJID<br>OPTASKID<br>OWNERID<br>PARENTENDORSEMENTID<br>PARENTJOURNALENTRYID<br>PARENTNOTEID<br>PORTFOLIOID<br>PROGRAMID<br>PROJECTID<br><br>PROOFACTIONIDPROOFID<br>RICHTEXTNOTEID<br>TASKID<br>TEMPLATEID<br>TEMPLATETASKID<br>THREADID<br>TIMESHEETID<br>TOPOBJID<br>USERID</td>
        <td>DOCUMENT_CURRENT | DOCUMENTID<br>Variable en fonction de ATTACHOBJCODE<br>OPTASK_CURRENT | OPTASKID<br>WORKITEMS_CURRENT<br>USER_CURRENT | USERID<br>Table des enregistrements d'audit non prise en charge actuellement<br>COMPANIES_CURRENT | COMPANYID <br>DOCUMENT_CURRENT | DOCUMENTID<br>Pas une relation Workfront ; utilisé pour l’intégration à des systèmes externes<br>ITERATIONS_CURRENT | ITERATIONID<br>Self<br>Variable en fonction de NOTEOBJCODE<br>OPTASK_CURRENT | OPTASKID<br>USER_CURRENT | USERID<br>Table d’endorsement non prise en charge actuellement<br>JOURNALENTRIES_CURRENT | JOURNALENTRYID<br>NOTE_CURRENT | NOTEID<br>PORTFOLIO_CURRENT | PORTFOLIOID<br>PROGRAM_CURRENT | PROGRAMID<br>PROJECT_CURRENT | PROJECTID<br>Proof Table d'actions non prise en charge actuellement<br>Table d'épreuves non prise en charge actuellement<br>RESERVEDTEXTNOTES_CURRENT | RICHTEXTNOTEID<br>TASK_CURRENT | TASKID<br>TEMPLATES_CURRENT | TEMPLATEID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID<br>NOTE_CURRENT | NOTEID<br>TIMESHEET_CURRENT | TIMESHEETID<br>Variable en fonction de TOPOBJCODE<br>USER_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Intégration d’objet</td>
        <td>Intégration d’objet</td>
        <td>OBJINT | ObjectIntegration</td>
        <td>OBJECTINTEGRATION_CURRENT<br>OBJECTINTEGRATION_DAILY_HISTORY<br>OBJECTINTEGRATION_EVENT</td>
        <td>LINKEDOBJECTID<br>OBJECTINTEGRATIONID   (self)<br>OBJID <br>SYSID  </td>
        <td>Identifiant de l’objet identifié dans le champ LINKEDOBJECTCODE <br>Self<br>Identifiant de l’objet identifié dans le champ OBJCODE <br>Pas de relation ; utilisé à des fins d’application interne  </td>
    </tr>
    <tr>
        <td>Catégorie d'objets</td>
        <td>Catégories d’objets</td>
        <td>OBJET | Catégorie d'objet</td>
        <td>OBJECTSCATEGORIES_CURRENT<br>OBJECTSCATEGORIES_DAILY_HISTORY<br>OBJECTSCATEGORIES_EVENT</td>
        <td>CATEGORYID<br>OBJECTSCATEGORYID (self)<br>OBJID <br>SYSID  </td>
        <td>CATEGORIES_CURRENT | CATEGORYID<br>Self<br>ID de l’objet identifié dans le champ OBJCODE <br>Pas de relation ; utilisé à des fins d’application interne.  </td>
    </tr>
    <tr>
        <td>TâcheOp</td>
        <td>Événement, demande</td>
        <td>OPTASK | Problème</td>
        <td>OPTASKS_CURRENT<br>OPTASKS_DAILY_HISTORY<br>OPTASKS_EVENT<br>OPTASKS_CUSTOM_VALUE_CURRENT<br>OPTASKS_CUSTOM_VALUE_DAILY_HISTORY<br>OPTASKS_CUSTOM_VALUE_EVENT</td>
        <td>APPROVALPROCESSID<br>ASSIGNEDTOID<br>CATEGORYID<br>CURRENTAPPROVALSTEPID<br>ENTEREDBYID<br>EXCHANGERATEID<br>ITERATIONID<br>KANBANBOARDID<br>LASTCONDITIONNOTEID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>OPTASKID<br>OWNERID<br><br>PROJECTID<br><br>QUEUEDEFID<br>QUEUETOPICID<br>RESOLVEOPTASKID<br><br>RESOLVEPROJECTID<br> VETASKID<br>RESOLVINGOBJID<br>ROLEID<br>SOURCETASKID SUBMITTEDBYID TEAMID</td>
        <td>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>USER_CURRENT | USERID<br>CATEGORIES_CURRENT | CATEGORYID<br>APPROVALSTEPS_CURRENT | APPROVALSTEPID<br>USER_CURRENT | USERID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>ITERATIONS_CURRENT | Table de tableau ITÉRATIONID<br>Kanban non prise en charge actuellement<br>NOTE_CURRENT | NOTEID<br>NOTE_CURRENT | NOTEID<br>USER_CURRENT | USERID<br>Self<br>USER_CURRENT | USERID<br>PROJECT_CURRENT | PROJECTID<br>Queue Definition table non prise en charge actuellement<br>Queue Topic table non prise en charge actuellement<br>OPTASK_CURRENT | OPTASKID<br>PROJECT_CURRENT | PROJECTID<br>TASK_CURRENT | TASKID<br>Variable en fonction de RESOLVINGOBJCODE<br>ROLE_CURRENT | ROLEID<br>Variable en fonction de SOURCEOBJCODE<br>TASK_CURRENT | TASKID<br>USER_CURRENT | USERID<br>TEAM_CURRENT | TEAMID</td>
    </tr>
    <tr>
        <td>Paramètre</td>
        <td>Champ personnalisé</td>
        <td>PARAMÈTRE | Paramètre</td>
        <td>PARAMETERS_CURRENT<br>PARAMETERS_DAILY_HISTORY<br>PARAMETERS_EVENT</td>
        <td>LASTUPDATEDBYID<br>PARAMETERFILTERID<br>PARAMETERID (self)<br>SYSID  </td>
        <td>USERS_CURRENT | USERID<br>Parameter Table de filtre non prise en charge actuellement<br>Self<br>Not a relation ; utilisée à des fins d’application interne  </td>
    </tr>
    <tr>
        <td>Option de paramètre</td>
        <td>Option de paramètre</td>
        <td>POPT | Option de paramètre</td>
        <td>PARAMETEROPTIONS_CURRENT<br>PARAMETEROPTIONS_DAILY_HISTORY<br>PARAMETEROPTIONS_EVENT</td>
        <td>PARAMETERID<br>PARAMETEROPTIONID (self) <br>SYSID  </td>
        <td>PARAMETERS_CURRENT | PARAMETERID <br>Self<br>Pas de relation ; utilisé pour des applications internes  </td>
    </tr>
    <tr>
        <td>Section du portail</td>
        <td>Rapport</td>
        <td>PTLSEC | Rapport</td>
        <td>PORTALSECTIONS_CURRENT<br>PORTALSECTIONS_DAILY_HISTORY<br>PORTALSECTIONS_EVENT</td>
        <td>APPGLOBALID<br>ENTEREDBYID<br>FILTERID<br>GROUPBYID<br>LASTUPDATEDBYID<br>LASTVIEWEDBYID<br>OBJID<br>PORTALSECTIONID (SELF)<br>PREFERENCEID<br>PUBLICRUNASUSERID<br>REPORTFOLDERID<br>RUNASUSERID<br>SCHEDULEDREPORTID<br>SYSID<br>VIEWID</td>
        <td>Pas une relation ; utilisé à des fins d’application interne <br>USERS_CURRENT | USERID <br>UIFILTERS_CURRENT | FILTERID<br>UIGROUPBYS_CURRENT | GROUPBYID<br>USERS_CURRENT | USERID <br>USERS_CURRENT | USERID <br>ID de l’objet identifié dans le champ OBJOBJCODE<br>Self<br>PREFERENCES_CURRENT | PREFERENCEID<br>USERS_CURRENT | USERID <br>REPORTFOLDERS_CURRENT | REPORTFOLDERID<br>USERS_CURRENT | USERID <br>Table de rapports planifiés non prise en charge actuellement<br>Il ne s’agit pas d’une relation ; utilisée à des fins d’application interne <br>UIVIEWS_CURRENT | VIEWID</td>
    </tr>
    <tr>
        <td>Onglet Portail</td>
        <td>Tableau de bord</td>
        <td>PTLTAB | Tableau de bord</td>
        <td>PORTALTABS_CURRENT<br>PORTALTABS_DAILY_HISTORY<br>PORTALTABS_EVENT</td>
        <td>DOCID<br>LASTUPDATEDBYID<br>PORTALPROFILEID<br>PORTALTABID (self)<br>SYSID<br>USERID</td>
        <td>Pas une relation ; utilisé à des fins d’application interne <br>USERS_CURRENT | USERID <br>La table Profil de portail ne sera pas prise en charge <br>Self<br>Not a relation ; utilisée à des fins d’application interne <br>USERS_CURRENT | USERID  </td>
    </tr>
    <tr>
        <td>Section d'onglet de portail</td>
        <td>Section Tableau de bord</td>
        <td>PRTBSC | Section d'onglet de portail</td>
        <td>PORTALTABSPORTALSECTIONS_CURRENT<br>PORTALTABSPORTALSECTIONS_DAILY_HISTORY<br>PORTALTABSPORTALSECTIONS_EVENT</td>
        <td>CALENDARPORTALSECTIONID<br>EXTERNALSECTIONID<br>INTERNALSECTIONID <br>PORTALSECTIONOBJID <br>PORTALTABID<br>PORTALTABSECTIONID (SELF)<br>SYSID</td>
        <td>Section de portail de calendrier non prise en charge actuellement<br>Table de sections externes non prise en charge actuellement<br>PORTALSECTIONS_CURRENT | PORTALSECTIONID <br>ID de l'objet identifié dans le champ PORTALSECTIONOBJCODE<br>PORTALTABS_CURRENT | PORTALTABID<br>Self<br>Not a Relationship ; utilisé pour les applications internes</td>
    </tr>
    <tr>
        <td>PortalSectionLastViewer</td>
        <td>Signaler les dernières visionneuses</td>
        <td>PLSLSV | PortalSectionLastViewer</td>
        <td>REPORTLASTVIEWERS_CURRENT<br>REPORTLASTVIEWERS_DAILY_HISTORY<br>REPORTLASTVIEWERS_EVENT</td>
        <td>REPORTID<br>REPORTLASTVIEWERID (SELF)<br>SYSID<br>VIEWERID</td>
        <td>PORTALSECTIONS_CURRENT | PORTALSECTIONID <br>REPORTLASTVIEWERID (self)<br>Pas de relation ; utilisé à des fins d’application interne<br>USERS_CURRENT | USERID  </td>
    </tr>
    <tr>
        <td>Portfolio</td>
        <td>Portfolio</td>
        <td>PORT | Portfolio</td>
        <td>PORTFOLIOS_CURRENT<br>PORTFOLIOS_DAILY_HISTORY<br>PORTFOLIOS_EVENT<br>PORTFOLIOS_CUSTOM_VALUE_CURRENT<br>PORTFOLIOS_CUSTOM_VALUE_DAILY_HISTORY<br>PORTFOLIOS_CUSTOM_VALUE_EVENT</td>
        <td>ALIGNMENTSCORECARDID<br>CATEGORYID<br>ENTEREDBYID<br>GROUPID<br>LASTUPDATEDBYID<br>OWNERID<br>PORTFOLIOID</td>
        <td>Le tableau des cartes de performance n’est pas pris en charge actuellement<br>CATEGORIES_CURRENT | CATEGORYID<br>USER_CURRENT | USERID<br>GROUP_CURRENT | GROUPID<br>USER_CURRENT | USERID<br>USER_CURRENT | USERID<br>Self</td>
    </tr>
    <tr>
        <td>Préférence</td>
        <td>Affichage, Filtrage, Regroupement, Définition De Rapport</td>
        <td>PROSET | Préférence</td>
        <td>PREFERENCES_CURRENT<br>PREFERENCES_DAILY_HISTORY<br>PREFERENCES_EVENT</td>
        <td>APPGLOBALID<br>PREFERENCEID (self) <br>SYSID  </td>
        <td>Pas une relation ; utilisé à des fins d’application interne<br>Self <br>Pas de relation ; utilisé à des fins d’application interne  </td>
    </tr>
    <tr>
        <td>Programme</td>
        <td>Programme</td>
        <td>PRGM | Programme</td>
        <td>PROGRAMMES_CURRENT<br>PROGRAMMES_DAILY_HISTORY<br>PROGRAMMES_EVENT<br>PROGRAMMES_CUSTOM_VALUE_CURRENT<br>PROGRAMMES_CUSTOM_VALUE_DAILY_HISTORY<br>PROGRAMMES_CUSTOM_VALUE_EVENT</td>
        <td>CATEGORYID<br>ENTEREDBYID<br>GROUPID<br>LASTUPDATEDBYID<br>OWNERID<br>PORTFOLIOID<br>PROGRAMID</td>
        <td>CATEGORIES_CURRENT | CATEGORYID<br>USER_CURRENT | USERID<br>GROUP_CURRENT | GROUPID<br>USER_CURRENT | USERID<br>USER_CURRENT | USERID<br>PORTFOLIO_CURRENT | PORTFOLIOID<br>Self</td>
    </tr>
    <tr>
        <td>Projet</td>
        <td>Projet</td>
        <td>PROJ | Projet</td>
        <td>PROJECTS_CURRENT<br>PROJECTS_DAILY_HISTORY<br>PROJECTS_EVENT<br>PROJECTS_CUSTOM_VALUE_CURRENT<br>PROJECTS_CUSTOM_VALUE_DAILY_HISTORY<br>PROJECTS_CUSTOM_VALUE_EVENT</td>
        <td>AEMNATIVEFOLDERTREESREFID<br>ALIGNMENTSCORECARDID<br>APPROVALPROCESSID<br>ATTACHEDRATECARDID<br>CATEGORYID<br>COMPANYID<br>CONVERTEDOPTASKID<br>CONVERTEDOPTASKORIGINATORID<br>CURRENTAPPROVALSTEPID<br>DELIVERABLESCORECARDID<br>ENTEREDBYID<br>GROUPID<br><br>LASTCONDITIONNOTEID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>MILESTONEPATHID OWNERID<br>POPACCOUNTID<br>PORTFOLIOID<br>PRIVATERATECARDID<br>PROGRAMID<br>PROJECTID<br>QUEUEDEFID<br>REJECTIONISSUEID<br>RESOURCEPOLID<br>SCHEDULEID<br>SPONSORID<br>SUBMITTEDBYID<br>TEAMID<br>TEMPLATEID</td>
        <td>N’est pas une relation Workfront ; utilisé pour l’intégration à des systèmes externes<br>le tableau de cartes de performance n’est actuellement pas pris en charge<br>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>RATECARD_CURRENT | RATECARDID<br>CATEGORIES_CURRENT | CATEGORYID<br>COMPANIES_CURRENT | COMPANYID <br>OPTASK_CURRENT | OPTASKID<br>USER_CURRENT | USERID<br>APPROVALSTEPS_CURRENT | La table APPROVALSTEPID<br>Scorecard n'est pas prise en charge actuellement<br>USER_CURRENT | USERID<br>GROUP_CURRENT | GROUPID<br>NOTE_CURRENT | NOTEID<br>NOTE_CURRENT | NOTEID<br>USER_CURRENT | USERID<br>MILESTONEPATH_CURRENT | MILESTONEPATHID<br>USER_CURRENT | La table des comptes USERID<br>Pop n’est actuellement pas prise en charge<br>PORTFOLIO_CURRENT | PORTFOLIOID<br>RATECARD_CURRENT | RATECARDID<br>PROGRAM_CURRENT | La table de définitions PROGRAMID<br>Self<br>Queue n'est pas prise en charge actuellement<br>OPTASK_CURRENT | OPTASKID<br>RESOURCEPOOLS_CURRENT | RESOURCEPOOLID<br>SCHEDULE_CURRENT | SCHEDULEID<br>USER_CURRENT | USERID<br>USER_CURRENT | USERID<br>TEAM_CURRENT | TEAMID<br>TEMPLATES_CURRENT | TEMPLATEID</td>
    </tr>
    <tr>
        <td>Utilisateur de l'équipe du projet</td>
        <td>Utilisateur de l'équipe du projet</td>
        <td>PRTU | Utilisateur du projet</td>
        <td>PROJECTSUSERS_CURRENT<br>PROJECTSUSERS_DAILY_HISTORY<br>PROJECTSUSERS_EVENT</td>
        <td>PROJECTID<br>PROJECTSUSERID (self)<br>SYSID<br>TMPUSERID<br>USERID</td>
        <td>PROJECTS_CURRENT | PROJECTID<br>Self<br>Pas de relation ; utilisé à des fins d’application interne<br>TEMPLATES_CURRENT | TEMPLATEID<br>USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Rôle d'utilisateur d'équipe de projet</td>
        <td>Rôle d'utilisateur d'équipe de projet</td>
        <td>PTEAM | ProjectUserRole</td>
        <td>PROJECTSUSERSROLES_CURRENT<br>PROJECTSUSERSROLES_DAILY_HISTORY<br>PROJECTSUSERSROLES_EVENT</td>
        <td>PROJECTID<br>PROJECTSUSERSROLEID (self)<br>ROLEID<br>SYSID<br>USERID</td>
        <td>PROJECTS_CURRENT | PROJECTID<br>Self<br>ROLES_CURRENT | ROLEID<br>Pas de relation ; utilisé à des fins d’application interne<br>USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Carte tarifaire</td>
        <td>Carte tarifaire</td>
        <td>CRTD |Carte tarifaire</td>
        <td>RATECARD_CURRENT<br>RATECARD_DAILY_HISTORY<br>RATECARD_EVENT</td>
        <td>CATEGORYID<br>ENTEREDBYID<br>LASTUPDATEDBYID <br>RATECARDID (SELF) <br>SECURITYROOTID <br>SOURCEID<br>SYSID</td>
        <td>CATEGORYID<br>USERS_CURRENT | USERID <br>USERS_CURRENT | USERID    <br>Self<br>ID de l’objet identifié dans le champ SECURITYOBJCODE <br>ID de l’objet identifié dans le champ SOURCEOBJCODE<br>Pas de relation ; utilisé à des fins d’application interne  </td>
    </tr>
    <tr>
        <td>Dossier des rapports</td>
        <td>Dossier des rapports</td>
        <td>RPTFDR | Dossier du rapport</td>
        <td>REPORTFOLDERS_CURRENT<br>REPORTFOLDERS_DAILY_HISTORY<br>REPORTFOLDERS_EVENT</td>
        <td>REPORTFOLDERID (self)<br>SYSID</td>
        <td>Self<br>Not a Relationship ; utilisé pour des applications internes</td>
    </tr>
    <tr>
        <td>Nombre de statistiques de vues de rapports</td>
        <td>Nombre de statistiques de vues de rapports</td>
        <td>PLSVST | PortalSectionStatisticInfo</td>
        <td>REPORTVIEWSTATISTICCOUNTS_CURRENT<br>REPORTVIEWSTATISTICCOUNTS_DAILY_HISTORY<br>REPORTVIEWSTATISTICCOUNTS_EVENT</td>
        <td>REPORTID<br>REPORTVIEWSTATISTICCOUNTID (SELF)<br>SYSID</td>
        <td>PORTALSECTIONS_CURRENT | PORTALSECTIONID<br>Self<br>Not a Relationship ; utilisé pour les applications internes</td>
    </tr>
    <tr>
        <td>Heures budgétées à déclarer</td>
        <td>Heures budgétées à déclarer</td>
        <td>RPBGHR | Heure budgétée</td>
        <td>REPORTABLEBUDGETEDHOURS_CURRENT<br>REPORTABLEBUDGETEDHOURS_DAILY_HISTORY<br>REPORTABLEBUDGETEDHOURS_EVENT</td>
        <td>PROJECTID<br>REPORTABLEBUDGETEDHOURID (SELF)<br>ROLEID<br>SYSID<br>USERID</td>
        <td>PROJECTS_CURRENT | PROJECTID<br>Self<br>ROLES_CURRENT | ROLEID<br>Pas de relation ; utilisé à des fins d’application interne<br>USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Temps réservé</td>
        <td>Congés (personnels)</td>
        <td>RESVT | Congés</td>
        <td>RESERVEDTIMES_CURRENT<br>RESERVEDTIMES_DAILY_HISTORY<br>RESERVEDTIMES_EVENT</td>
        <td>RESERVEDTIMEID (self)<br>SYSID<br>TASKID<br>USERID</td>
        <td>Self<br>Not a relation ; utilisé à des fins d’application interne<br>TASKS_CURRENT | TASKID<br>USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Gestionnaire des ressources</td>
        <td>Gestionnaire des ressources</td>
        <td>RESMGR | Gestionnaire des ressources</td>
        <td>RESOURCEMANAGERS_CURRENT<br>RESOURCEMANAGERS_DAILY_HISTORY<br>RESOURCEMANAGERS_EVENT</td>
        <td>ID (self)<br>PROJECTID<br>RESOURCEMANAGERID<br>SYSID<br>TEMPLATEID</td>
        <td>Self<br>PROJECTS_CURRENT | PROJECTID<br>USERS_CURRENT | USERID<br>Pas une relation ; utilisé à des fins d’application interne<br>TEMPLATES_CURRENT | TEMPLATEID</td>
    </tr>
    <tr>
        <td>Pool de ressources</td>
        <td>Pool de ressources</td>
        <td>RSPL | Pool de ressources</td>
        <td>RSRCPOOLS_CURRENT<br>RSRCPOOLS_DAILY_HISTORY<br>RSRCPOOLS_EVENT</td>
        <td>ENTEREDBYID<br>LASTUPDATEDBYID <br>RESOURCEPOOLID (self)<br>SYSID  </td>
        <td>USERS_CURRENT | USERID <br>USERS_CURRENT | USERID <br>Self<br>Not a Relationship ; utilisé pour les applications internes  </td>
    </tr>
    <tr>
        <td>Remarque Rich Text</td>
        <td>Remarque Rich Text</td>
        <td>RHNOTE | Note de texte enrichi</td>
        <td>RESERVEDTEXTNOTES_CURRENT<br>RESERVEDTEXTNOTES_DAILY_HISTORY<br>RESERVEDTEXTNOTES_EVENT</td>
        <td>RICHTEXTNOTEID (self)<br>SYSID</td>
        <td>Self<br>Not a Relationship ; utilisé pour des applications internes</td>
    </tr>
    <tr>
        <td>Valeur de paramètre Rich Text</td>
        <td>Valeur de paramètre Rich Text</td>
        <td>ARCHVAL | RichTextParameterValue</td>
        <td>RICHTEXTPARAMETERVALUES_CURRENT<br>RICHTEXTPARAMETERVALUES_DAILY_HISTORY<br>RICHTEXTPARAMETERVALUES_EVENT</td>
        <td>PARAMETERVALUEID<br>RICHTEXTPARAMETERVALUEID (self) <br>SYSID  </td>
        <td>Table de valeurs de paramètres non prise en charge actuellement<br>Self<br>Pas de relation ; utilisée à des fins d’application interne  </td>
    </tr>
    <tr>
        <td>Risque</td>
        <td>Risque</td>
        <td>RISQUE | Risque</td>
        <td>RISKS_CURRENT<br>RISKS_DAILY_HISTORY<br>RISKS_EVENT</td>
        <td>ENTEREDBYID<br>EXCHANGERATEID<br>LASTUPDATEDBYID <br>PROJECTID <br>RISKID (SELF)<br>RISKTYPEID<br>SYSID<br>TEMPLATEID</td>
        <td>USERS_CURRENT | USERID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>USERS_CURRENT | USERID <br>PROJECTS_CURRENT | PROJECTID   <br>Self<br>RISKTYPES_CURRENT | RISKTYPEID<br>Pas une relation ; utilisé à des fins d’application interne<br>TEMPLATES_CURRENT | TEMPLATEID</td>
    </tr>
    <tr>
        <td>Type de risque</td>
        <td>Type de risque</td>
        <td>RSKTYPE | Type de risque</td>
        <td>RISKTYPES_CURRENT<br>RISKTYPES_DAILY_HISTORY<br>RISKTYPES_EVENT</td>
        <td>RISKTYPEID<br>SYSID</td>
        <td>Self<br>Not a Relationship ; utilisé pour des applications internes</td>
    </tr>
    <tr>
        <td>Rôle</td>
        <td>Fonction</td>
        <td>RÔLE | Fonction</td>
        <td>ROLES_CURRENT<br>ROLES_DAILY_HISTORY<br>ROLES_EVENT</td>
        <td>ENTEREDBYID<br>LAYOUTTEMPLATEID<br>PRIVATERATECARDID<br>ROLEID<br>UITEMPLATEID</td>
        <td>USER_CURRENT | Le tableau USERID<br>Layout Template ne sera pas pris en charge<br>RATECARD_CURRENT | RATECARDID<br>Self<br>UITEMPLATES_CURRENT |UITEMPLATEID</td>
    </tr>
    <tr>
        <td>Planning</td>
        <td>Planning</td>
        <td>PLANIFIÉ | Planification</td>
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
        <td>APPROVALSTEPS_CURRENT | APPROVALSTEPID<br>ROLES_CURRENT | ROLEID<br>Self<br>Pas de relation ; utilisé pour les applications internes <br>TEAMS_CURRENT | TEAMID<br>USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Tâche</td>
        <td>Tâche</td>
        <td>TÂCHE | Tâche</td>
        <td>TASKS_CURRENT<br>TASKS_DAILY_HISTORY<br>TASKS_EVENT<br>TASKS_CUSTOM_VALUE_CURRENT<br>TASKS_CUSTOM_VALUE_DAILY_HISTORY<br>TASKS_CUSTOM_VALUE_EVENT</td>
        <td>APPROVALPROCESSID<br>ASSIGNEDTOID<br>BILLINGRECORDID<br>CATEGORYID<br>CONVERTEDOPTASKID<br>CONVERTEDOPTASKORIGINATORID<br>CURRENTAPPROVALSTEPID<br>ENTEREDBYID<br>EXCHANGERATEID<br>GROUPID<br>ITERATIONID<br>KANBANBOARDID<br>LASTCONDITIONNOTEID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>MILESTONEID<br><br>PARENTID<br><br>PROJD <br>RECURRENCERULEID<br>REJECTIONISSUEID<br>RESERVEDTIMEID<br>ROLEID<br>SUBMITTEDBYID<br>TASKID TEAMID TEMPLATETASKID</td>
        <td>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>USER_CURRENT | USERID<br>BILLINGRECORDS_CURRENT | BILLINGRECORDID<br>CATEGORIES_CURRENT | CATEGORYID<br>OPTASK_CURRENT | OPTASKID<br>USER_CURRENT | USERID<br>APPROVALSTEPS_CURRENT | APPROVALSTEPID<br>USER_CURRENT | USERID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>GROUP_CURRENT | GROUPID<br>ITERATIONS_CURRENT | Table de tableau ITÉRATIONID<br>Kanban non prise en charge actuellement<br>NOTE_CURRENT | NOTEID<br>NOTE_CURRENT | NOTEID<br>USER_CURRENT | USERID<br>MILESTONE_CURRENT | MILESTONEID<br>TASK_CURRENT | TASKID<br>PROJECT_CURRENT | La table de règles PROJECTID<br>Recurrence n'est pas prise en charge actuellement<br>OPTASK_CURRENT | OPTASKID<br>RESERVEDTIMES_CURRENT | RESERVEDTIMEID<br>ROLE_CURRENT | ROLEID<br>USER_CURRENT | USERID<br>Self<br>TEAM_CURRENT | TEAMID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID</td>
    </tr>
    <tr>
        <td>Tâche antérieure</td>
        <td>Tâche antérieure</td>
        <td>PRED | Prédécesseur</td>
        <td>PREDECESSORS_CURRENT<br>PREDECESSORS_DAILY_HISTORY<br>PREDECESSORS_EVENT</td>
        <td>ID (self)<br>PREDECESSORID<br>SUCCESSORID <br>SYSID</td>
        <td>SELF<br>TASKS_CURRENT | TASKID<br>TASKS_CURRENT | TASKID <br>pas une relation ; utilisé à des fins d’application interne</td>
    </tr>
    <tr>
        <td>Equipe</td>
        <td>Equipe</td>
        <td>TEAMOB | Équipe</td>
        <td>TEAMS_CURRENT<br>TEAMS_DAILY_HISTORY<br>TEAMS_EVENT</td>
        <td>ENTEREDBYID<br>GROUPID<br>LAYOUTTEMPLATEID<br>MYWORKVIEWID<br>OWNERID<br>REQUESTSVIEWID<br>SCHEDULEID<br>TEAMID<br>UITEMPLATEID</td>
        <td>USER_CURRENT | USERID<br>GROUP_CURRENT | Le tableau GROUPID<br>Layout Template ne sera pas pris en charge<br>UIVIEWS_CURRENT | UIVIEWID<br>USER_CURRENT | USERID<br>UIVIEWS_CURRENT | UIVIEWID<br>SCHEDULE_CURRENT | SCHEDULEID<br>Self<br>UITEMPLATES_CURRENT |UITEMPLATEID</td>
    </tr>
    <tr>
        <td>Membre d'équipe</td>
        <td>Autres équipes, membre d'équipe</td>
        <td>TEAMMB | Membre d'équipe</td>
        <td>TEAMMEMBERS_CURRENT<br>TEAMMEMBERS_DAILY_HISTORY<br>TEAMMEMBERS_EVENT</td>
        <td>SYSID <br>TEAMID<br>TEAMMEMBERID (self)<br>USERID</td>
        <td>Pas une relation ; utilisé à des fins d’application interne <br>TEAMS_CURRENT | TEAMID<br>Self<br>USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>TeamMemberRole</td>
        <td>Rôle de membre d'équipe</td>
        <td>TEAMMR | Rôle de membre d'équipe</td>
        <td>TEAMMEMBERROLES_CURRENT<br>TEAMMEMBERROLES_DAILY_HISTORY<br>TEAMMEMBERROLES_EVENT</td>
        <td>ROLEID <br>TEAMID<br>TEAMMEMBERROLEID (SELF)<br>USERID</td>
        <td>ROLES_CURRENT | ROLEID <br>TEAMS_CURRENT | TEAMID<br>Self<br>USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Modèle</td>
        <td>Modèle</td>
        <td>TMPL | Modèle</td>
        <td>TEMPLATES_CURRENT<br>TEMPLATES_DAILY_HISTORY<br>TEMPLATES_EVENT</td>
        <td>APPROVALPROCESSID<br>CATEGORYID<br>COMPANYID <br>DELIVERABLESCORECARDID <br>ENTEREDBYID<br>GROUPID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>MILESTONEPATHID <br>OWNERID <br>PRIVATERATECARDID<br>PROGRAMID<br>QUEUEDEFID<br>SCHEDULEID <br>SYSID <br>TEAMID<br>TEMPLATEID (SELF)</td>
        <td>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>CATEGORIES_CURRENT | CATEGORYID<br>COMPANIES_CURRENT | COMPANYID   <br>DELIVERABLESCORECARDID <br>USERS_CURRENT | USERID<br>GROUPS_CURRENT | GROUPID<br>NOTES_CURRENT | NOTEID<br>USERS_CURRENT | USERID<br>MILESTONEPATH_CURRENT | MILESTONEPATHID <br>USERS_CURRENT | USERID <br>RATECARD_CURRENT | RATECARDID<br>PROGRAM_CURRENT | La table de définition de la file d'attente PROGRAMID<br>Queue n'est pas prise en charge actuellement<br>SCHEDULES_CURRENT | SCHEDULEID <br>pas de relation ; utilisé à des fins d’application interne <br>TEAMS_CURRENT) | TEAMID<br>Self</td>
    </tr>
    <tr>
        <td>Modèle d'affectation</td>
        <td>Modèle d'affectation</td>
        <td>AFFECTATION | Modèle d'affectation</td>
        <td>TEMPLATEASSIGNMENTS_CURRENT<br>TEMPLATEASSIGNMENTS_DAILY_HISTORY<br>TEMPLATEASSIGNMENTS_EVENT</td>
        <td>ASSIGNEDTOID<br>CATEGORYID<br>LASTUPDATEDBYID<br>OBJID<br>ROLEID<br>SYSID<br>TEAMID<br>TEAMTIMELINEABLEID<br>TEMPLATEASSIGNMENTID (SELF)<br>TEMPLATETASKID</td>
        <td>USERS_CURRENT | USERID<br>CATEGORIES_CURRENT | CATEGORYID<br>USERS_CURRENT | USERID<br>ID de l’objet identifié dans le champ OBJCODE<br>ROLES_CURRENT | ROLEID<br>Pas de relation ; utilisé à des fins d’application interne<br>TEAMS_CURRENT | TEAMID<br>Team Table chronologique non prise en charge actuellement<br>Self<br>TEMPLATETASKS_CURRENT |TEMPLATETASKID</td>
    </tr>
    <tr>
        <td>Tâche de modèle</td>
        <td>Tâche de modèle</td>
        <td>TTSK | Tâche de modèle</td>
        <td>TEMPLATETASKS_CURRENT<br>TEMPLATETASKS_DAILY_HISTORY<br>TEMPLATETASKS_EVENT</td>
        <td>APPROVALPROCESSID<br>ASSIGNEDTOID<br>CATEGORYID<br>ENTEREDBYID<br>EXCHANGERATEID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>MILESTONEID<br>PARENTID<br>RECURRENCERULEID<br>ROLEID<br>SYSID<br>TEAMID<br>TEAMTIMELINEABLEID<br>TEMPLATEID<br>TEMPLATETASKID (SELF)</td>
        <td>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>USERS_CURRENT | USERID<br>CATEGORIES_CURRENT | CATEGORYID<br>USERS_CURRENT | USERID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>NOTES_CURRENT | NOTEID<br>USERS_CURRENT | USERID<br>MILESTONE_CURRENT | MILESTONEID<br>TEMPLATETASKS_CURRENT |TEMPLATETASKID<br>Table des règles de récurrence non prise en charge actuellement<br>ROLES_CURRENT | ROLEID<br>Pas de relation ; utilisé à des fins d’application interne<br>TEAMS_CURRENT | TEAMID<br>Team Table chronologique non prise en charge actuellement<br>TEMPLATES_CURRENT | TEMPLATEID<br>Self</td>
    </tr>
    <tr>
        <td>Tâche de modèle antérieure</td>
        <td>Prédécesseur du modèle</td>
        <td>TPRED | Prédécesseur</td>
        <td>TEMPLATEPREDECESSORS_CURRENT<br>TEMPLATEPREDECESSORS_DAILY_HISTORY<br>TEMPLATEPREDECESSORS_EVENT</td>
        <td>PREDECESSORID<br>SUCCESSORID <br>TEMPLATEPREDECESSORID (SELF)<br>SYSID</td>
        <td>TEMPLATETASKS_CURRENT |TEMPLATETASKID<br>TEMPLATETASKS_CURRENT |TEMPLATETASKID <br>Self<br>Not a Relationship ; utilisé pour les applications internes</td>
    </tr>
       <tr>
        <td>Devise des indicateurs de performance clés temporels (disponibilité limitée des clients)</td>
        <td>KPI chronologique</td>
        <td>TMPH | TimePhasedKPI</td>
        <td>TIMESHEETS_CURRENT<br>TIMESHEETS_DAILY_HISTORY<br>TIMESHEETS_EVENT</td>
        <td>APPROVERID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>TIMESHEETID<br>TIMESHEETPROFILEID<br>USERID</td>
        <td>USER_CURRENT | USERID<br>NOTE_CURRENT | NOTEID<br>USER_CURRENT | USERID<br>Self<br>TIMESHEETPROFILES_CURRENT | TIMESHEETPROFILEID<br>USER_CURRENT | USERID</td>
    </tr>
        <tr>
        <td>Durée des KPI par étapes (disponibilité limitée des clients)</td>
        <td>KPI chronologique</td>
        <td>TMPH | TimePhasedKPI</td>
        <td>TIMEPHASED_DURATION_CURRENT<br>TIMEPHASED_DURATION_DAILY_HISTORY<br>TIMEPHASED_DURATION_EVENT</td>
        <td>ASSIGNMENTID<br>GROUPID<br>LOCATIONID<br>OPTASKID<br>PORTFOLIOID<br>PROGRAMID<br>PROJECTID<br>REFERENCEID<br>ROLEID<br>SOURCETASKID<br>TASKID<br>TIMEPHASEDDURATIONID (SELF)<br>USERID</td>
        <td>ASSIGNMENTS_CURRENT | ASSIGNMENTID<br>GROUPS_CURRENT | GROUPID<br>CLASSIFIER_CURRENT | CLASSIFIERID<br>OPTASKS_CURRENT | OPTASKID<br>PORTFOLIOS_CURRENT | PORTFOLIOID<br>PROGRAMS_CURRENT | PROGRAMID<br>PROJECTS_CURRENT | PROJECTID<br>identifie l'objet de l'enregistrement d'indicateur de performance clé<br>ROLES_CURRENT | ROLEID<br>TASKS_CURRENT | TASKID<br>TASKS_CURRENT | TASKID<br>Self<br>USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Feuille de temps</td>
        <td>Feuille de temps</td>
        <td>TMPH | TimePhasedKPI</td>
        <td>TIMEPHASED_CURRENCY_CURRENT<br>TIMEPHASED_CURRENCY_DAILY_HISTORY<br>TIMEPHASED_CURRENCY_EVENT</td>
        <td>ASSIGNMENTID<br>GROUPID<br>LOCATIONID<br>OPTASKID<br>PORTFOLIOID<br>PROGRAMID<br>PROJECTID<br>REFERENCEID<br>ROLEID<br>SOURCETASKID<br>TASKID<br>TIMEPHASEDCURRENCYID (SELF)<br>USERID</td>
        <td>USER_CURRENT | USERID<br>NOTE_CURRENT | NOTEID<br>USER_CURRENT | USERID<br>Self<br>TIMESHEETPROFILES_CURRENT | TIMESHEETPROFILEID<br>USER_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Profil de feuille de temps</td>
        <td>Profil de feuille de temps</td>
        <td>TSPRO | Profil de feuille de temps</td>
        <td>TIMESHEETPROFILES_CURRENT<br>TIMESHEETPROFILES_DAILY_HISTORY<br>TIMESHEETPROFILES_EVENT</td>
        <td>APPROVERID<br>ENTEREDBYID <br>GROUPID<br>SYSID<br>TIMESHEETPROFILEID (SELF)</td>
        <td>ASSIGNMENTS_CURRENT | ASSIGNMENTID<br>GROUPS_CURRENT | GROUPID<br>CLASSIFIER_CURRENT | CLASSIFIERID<br>OPTASKS_CURRENT | OPTASKID<br>PORTFOLIOS_CURRENT | PORTFOLIOID<br>PROGRAMS_CURRENT | PROGRAMID<br>PROJECTS_CURRENT | PROJECTID<br>identifie l'objet de l'enregistrement d'indicateur de performance clé<br>ROLES_CURRENT | ROLEID<br>TASKS_CURRENT | TASKID<br>TASKS_CURRENT | TASKID<br>Self<br>USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Filtre d’interface utilisateur</td>
        <td>Filtre</td>
        <td>SOULEVER | Filtre</td>
        <td>UIFILTERS_CURRENT<br>UIFILTERS_DAILY_HISTORY<br>UIFILTERS_EVENT</td>
        <td>APPGLOBALID<br>ENTEREDBYID <br>LASTUPDATEDBYID <br>OBJID<br>PREFERENCEID<br>SYSID <br>UIFILTERID (self)</td>
        <td>Pas une relation ; utilisé à des fins d’application interne<br>USERS_CURRENT | USERID <br>USERS_CURRENT | USERID <br>ID de l’objet identifié dans le champ OBJCODE<br>PREFERENCES_CURRENT | PREFERENCEID<br>Pas une relation ; utilisé à des fins d’application interne <br>Self</td>
    </tr>
    <tr>
        <td>Regrouper les interfaces utilisateur par</td>
        <td>Regroupement </td>
        <td>UIGB | Regroupement</td>
        <td>UIGROUPBYS_CURRENT<br>UIGROUPBYS_DAILY_HISTORY<br>UIGROUPBYS_EVENT</td>
        <td>ENTEREDBYID<br>GROUPID <br>LASTUPDATEDBYID <br>SYSID <br>UITEMPLATEID (self)</td>
        <td>USERS_CURRENT | USERID<br>GROUPS_CURRENT | GROUPID <br>USERS_CURRENT | USERID <br>pas une relation ; utilisé à des fins d’application interne <br>Self)</td>
    </tr>
    <tr>
        <td>Modèle d’interface utilisateur</td>
        <td>Modèle de mise en page</td>
        <td>UITMPL | Modèle de mise en page</td>
        <td>UITEMPLATES_CURRENT<br>UITEMPLATES_DAILY_HISTORY<br>UITEMPLATES_EVENT</td>
        <td>APPGLOBALID<br>ENTEREDBYID <br>LASTUPDATEDBYID <br>OBJID<br>PREFERENCEID<br>SYSID <br>UIGROUPBYID (self)</td>
        <td>Pas une relation ; utilisé à des fins d’application interne<br>USERS_CURRENT | USERID <br>USERS_CURRENT | USERID <br>ID de l’objet identifié dans le champ OBJCODE<br>PREFERENCES_CURRENT | PREFERENCEID<br>Pas une relation ; utilisé à des fins d’application interne <br>Self</td>
    </tr>
    <tr>
        <td>Vue UI</td>
        <td>Afficher</td>
        <td>UIVIEW | Vue</td>
        <td>UIVIEWS_CURRENT<br>UIVIEWS_DAILY_HISTORY<br>UIVIEWS_EVENT</td>
        <td>APPGLOBALID<br>ENTEREDBYID <br>LASTUPDATEDBYID <br>OBJID<br>PREFERENCEID<br>SYSID <br>UIVIEWID (self)</td>
        <td>Pas une relation ; utilisé à des fins d’application interne<br>USERS_CURRENT | USERID <br>USERS_CURRENT | USERID <br>ID de l’objet identifié dans le champ OBJCODE<br>PREFERENCES_CURRENT | PREFERENCEID<br>Pas une relation ; utilisé à des fins d’application interne <br>Self</td>
    </tr>
    <tr>
        <td>l’utilisateur ou de l’utilisatrice</td>
        <td>l’utilisateur ou de l’utilisatrice</td>
        <td>UTILISATEUR | Utilisateur</td>
        <td>USERS_CURRENT<br>USERS_DAILY_HISTORY<br>USERS_EVENT<br>USERS_CUSTOM_VALUE_CURRENT<br>USERS_CUSTOM_VALUE_DAILY_HISTORY<br>USERS_CUSTOM_VALUE_EVENT</td>
        <td>ACCESSLEVELID<br>CATEGORYID<br>COMPANYID<br>DEFAULTHOURTYPEID<br>DELEGATIONTOID<br>EAUTHUSERID<br>ENTEREDBYID<br>HOMEGROUPID<br>HOMETEAMID<br>LASTENTEREDNOTEID<br>LASTUPDATEDBYID<br>LATESTUPDATENOTEID<br>LAYOUTTEMPLATEID<br>MANAGERID<br>PORTALPROFILEID<br>PREFUIID<br>PRIVATERATECARDID<br>RESOURCEPOOOD<br>ROLEID<br>SCHEDULEID<br>TIMESHEETPROFILEID<br>UITEMPLATEID<br>USERID<br>UUMUSERID</td>
        <td>ACCESSLEVELS_CURRENT |ACCESSLEVELS<br>CATEGORIES_CURRENT | CATEGORYID<br>COMPANIES_CURRENT | COMPANYID <br>HOURTYPE_CURRENT | HOURTYPEID<br>USER_CURRENT | USERID<br>Pas une relation ; utilisé à des fins d’application interne<br>USER_CURRENT | USERID<br>GROUP_CURRENT | GROUPID<br>TEAM_CURRENT | TEAMID<br>NOTE_CURRENT | NOTEID<br>USER_CURRENT | USERID<br>NOTE_CURRENT | NOTEID<br>Layout Template table ne sera pas pris en charge<br>USER_CURRENT | La table de profils USERID<br>Portal ne sera pas prise en charge<br>il ne s'agit pas d'une relation ; utilisée à des fins d'application interne<br>RATECARD_CURRENT | RATECARDID<br>RESOURCEPOOLS_CURRENT | RESOURCEPOOLID<br>ROLE_CURRENT | ROLEID<br>SCHEDULE_CURRENT | SCHEDULEID<br>TIMESHEETPROFILES_CURRENT | TIMESHEETPROFILEID<br>UITEMPLATES_CURRENT |UITEMPLATEID<br>Self<br>Not a Relationship ; utilisé pour les applications internes</td>
    </tr>
    <tr>
        <td>Délégation d'utilisateur</td>
        <td>Délégation d'utilisateur</td>
        <td>USERDEL | Délégation d’utilisateurs</td>
        <td>USERDELEGATIONS_CURRENT<br>USERDELEGATIONS_DAILY_HISTORY<br>USERDELEGATIONS_EVENT</td>
        <td>FROMUSERID<br>SYSID <br>TOUSERID <br>USERDELEGATIONID (self)</td>
        <td>USERS_CURRENT | USERID<br>pas une relation ; utilisé à des fins d’application interne <br>USERS_CURRENT | USERID <br>Self</td>
    </tr>
    <tr>
        <td>Groupe d'utilisateurs</td>
        <td>Autres groupes</td>
        <td>USRGPS | Groupe d’utilisateurs</td>
        <td>USERSGROUPS_CURRENT<br>USERSGROUPS_DAILY_HISTORY<br>USERSGROUPS_EVENT</td>
        <td>GROUPID <br>SYSID<br>USERID <br>USERSGROUPID (self)</td>
        <td>GROUPS_CURRENT | GROUPID <br>Pas de relation ; utilisé à des fins d’application interne<br>USERS_CURRENT | USERID <br>Self</td>
    </tr>
    <tr>
        <td>Emplacement de l’utilisateur</td>
        <td>Emplacement de l’utilisateur</td>
        <td>USRLOC | UserLocation</td>
        <td>USERLOCATIONS_CURRENT<br>USERLOCATIONS_DAILY_HISTORY<br>USERLOCATIONS_EVENT</td>
        <td>CLASSIFIERID<br>SYSID<br>USERID<br>USERLOCATIONID (self)</td>
        <td>CLASSIFIER_CURRENT | CLASSIFIERID<br>Pas de relation ; utilisé à des fins d’application interne<br>USERS_CURRENT | USERID<br>Self</td>
    </tr>
    <tr>
        <td>Rôle utilisateur</td>
        <td>Autres rôles</td>
        <td>USROL | Rôle de l'utilisateur</td>
        <td>USERSROLES_CURRENT<br>USERSROLES_DAILY_HISTORY<br>USERSROLES_EVENT</td>
        <td>ROLEID <br>SYSID<br>USERID    <br>USERROLESETID<br>USERSROLEID (self)</td>
        <td>ROLES_CURRENT | ROLEID <br>Pas de relation ; utilisé à des fins d’application interne<br>USERS_CURRENT | USERID    <br>USERROLESET_CURRENT | USERROLESETID<br>Self</td>
    </tr>
    <tr>
        <td>UserPrefValue</td>
        <td>UserPrefValue</td>
        <td>USERPF | Préférence utilisateur</td>
        <td>USERPREFVALUES_CURRENT<br>USERPREFVALUES_DAILY_HISTORY<br>USERPREFVALUES_EVENT</td>
        <td>SYSID    <br>USERID <br>USERPREFVALUEID (self)</td>
        <td>Pas une relation ; utilisé à des fins d’application interne<br>USERS_CURRENT | USERID    <br>Self</td>
    </tr>
    <tr>
        <td>UserRoleSet</td>
        <td>UserRoleSet</td>
        <td>URSET | UserRoleSet</td>
        <td>USERROLESET_CURRENT<br>USERROLESET_DAILY_HISTORY<br>USERROLESET_EVENT</td>
        <td>PRIMARYROLEID <br>SYSID<br>USERID    <br>USERROLESETID (self)</td>
        <td>ROLES_CURRENT | ROLEID <br>Pas de relation ; utilisé à des fins d’application interne<br>USERS_CURRENT | USERID <br>Self</td>
    </tr>
    <tr>
        <td>UsersDecisions</td>
        <td>Décisions des utilisateurs et utilisatrices</td>
        <td>USRDEC | Décisions des utilisateurs</td>
        <td>USERSDECISIONS_CURRENT<br>USERSDECISIONS_DAILY_HISTORY<br>USERSDECISIONS_EVENT</td>
        <td>USERDECISIONID (self)<br>SYSID <br>USERID  </td>
        <td>Self<br>Not a relation ; utilisé à des fins d’application interne <br>USERS_CURRENT | USERID </td>
    </tr>
    <tr>
        <td>WorkItem</td>
        <td>Élément de travail</td>
        <td>WRKITM | WorkItem</td>
        <td>WORKITEMS_CURRENT<br>WORKITEMS_DAILY_HISTORY<br>WORKITEMS_EVENT</td>
        <td>ASSIGNMENTID <br>OBJID<br>OPTASKID    <br>PROJECTID <br>SYSID<br>TASKID    <br>USERID <br>WORKITEMID (self)</td>
        <td>ASSIGNMENTS_CURRENT | ASSIGNMENTID <br>ID de l’objet identifié dans le champ OBJOBJCODE<br>OPTASK_CURRENT | OPTASKID    <br>PROJECTS_CURRENT | PROJECTID <br>pas une relation ; utilisé à des fins d’application interne<br>TASKS_CURRENT | TASKID    <br>USERS_CURRENT | USERID    <br>Self </td>
    </tr>
  </tbody>
</table>
