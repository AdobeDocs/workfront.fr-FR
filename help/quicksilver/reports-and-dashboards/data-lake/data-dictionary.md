---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Dictionnaire de données de Workfront Data Connect
description: Cette page contient des informations sur la structure et le contenu des données dans Workfront Data Connect.
author: Courtney
feature: Reports and Dashboards
exl-id: 57985404-554e-4289-b871-b02d3427aa5c
source-git-commit: 815bee06ce413005e362d2e38068d591696cad5b
workflow-type: tm+mt
source-wordcount: '8878'
ht-degree: 9%

---

# Dictionnaire de données de Workfront Data Connect

Cette page contient des informations sur la structure et le contenu des données dans Workfront Data Connect.

>[!NOTE]
>
>Les données de Data Connect sont actualisées toutes les 4 heures, de sorte que les modifications récentes peuvent ne pas être immédiatement répercutées.

## Types de vue

Il existe plusieurs types de vues que vous pouvez utiliser dans Data Connect pour afficher vos données Workfront de manière à fournir le plus d’insight.

* **Vue actuelle**

  La vue actuelle reflète les données de la même manière qu’elles existent dans Workfront, dans chaque objet et dans leur état actuel. Cependant, la latence de navigation est bien inférieure dans Workfront.

* **Vue Événement**

  L’affichage Événement suit chaque enregistrement de modification dans Workfront : en d’autres termes, chaque fois qu’un objet change d’état, un enregistrement est créé pour indiquer la date de la modification, l’auteur de la modification et ce qui a été modifié. Par conséquent, cette vue est utile pour les comparaisons ponctuelles. Cette vue inclut uniquement les enregistrements des trois dernières années.

* **Vue Historique quotidien**

  La vue Historique quotidien offre une version abrégée de la vue Événement, dans la mesure où elle affiche l&#39;état de chaque objet sur une base quotidienne plutôt que lorsque chaque événement individuel s&#39;est produit. Cette vue est donc utile pour l’analyse des tendances.

<!-- Custom view -->

## Diagramme de relation d’entité

Les objets dans Workfront (et, par conséquent, dans votre lac de données Data Connect) sont définis non seulement par leurs valeurs individuelles, mais également par leurs relations avec d’autres objets. Le diagramme de relation d’entité ci-dessous fournit un mappage de haut niveau des relations d’objet dans Data Connect. Le diagramme peut être visualisé et téléchargé à l’aide du lien suivant :

[Diagramme de relation de l’entité Data Connect](/help/quicksilver/reports-and-dashboards/data-lake/assets/Workfront-data-lake_entity-relationship-diagram.pdf)

>[!IMPORTANT]
>
>Le diagramme de relation d’entité (ERD) fourni est délibérément incomplet, car un ERD complet deviendrait illisible en raison du nombre élevé de relations dans l’application.<br>
>Ce diagramme fournit un exemple de la manière dont les relations documentées dans le tableau Projet de la section [Tableau de terminologie](#terminology-table) ci-dessous peuvent être utilisées pour joindre des données de la vue de données Projet à des objets adjacents. Un ERD complet n’est pas nécessaire une fois que ce modèle est compris pour les relations d’objet du projet

## Types de date

Plusieurs objets de date fournissent des informations sur le moment où des événements spécifiques se produisent.

* `DL_LOAD_TIMESTAMP` : cette date est mise à jour une fois l’actualisation des données terminée avec succès et inclut l’horodatage du début de la tâche d’actualisation qui a fourni la dernière version d’un enregistrement.
* `CALENDAR_DATE` : cette date est uniquement présente dans la vue Historique quotidien. La vue Historique quotidien fournit un enregistrement de l’aspect des données à 11 :59 UTC pour chaque date spécifiée dans `CALENDAR_DATE`.
* `BEGIN_EFFECTIVE_TIMESTAMP` : cette date est présente dans les vues Événement et Historique quotidien et représente l&#39;heure à laquelle un enregistrement devient la valeur actuelle dans l&#39;application.
* `END_EFFECTIVE_TIMESTAMP` : Cette date est présente dans les vues Événement et Historique quotidien et enregistre exactement le moment où un enregistrement est passé _de_ la valeur de la ligne active à une valeur d&#39;une autre ligne. Pour permettre la comparaison entre les requêtes sur `BEGIN_EFFECTIVE_TIMESTAMP` et `END_EFFECTIVE_TIMESTAMP`, cette valeur n’est jamais nulle, même s’il n’existe aucune nouvelle valeur. Dans le cas où un enregistrement est toujours valide (c’est-à-dire, que la valeur n’a pas changé), `END_EFFECTIVE_TIMESTAMP` aura une valeur de 2300-01-01.

## Table de terminologie

Le tableau suivant met en corrélation les noms d’objet dans Workfront (ainsi que leurs noms dans l’interface et l’API) avec leurs noms équivalents dans Data Connect et inclut des champs de référence pour chaque objet avec d’autres objets Workfront.

>[!NOTE]
>
>De nouveaux champs peuvent être ajoutés aux vues d’objet sans préavis pour prendre en charge l’évolution des besoins en données de l’application Workfront. Nous vous déconseillons d’utiliser des requêtes « SELECT » lorsque le destinataire des données en aval n’est pas prêt à gérer des colonnes supplémentaires au fur et à mesure de leur ajout.<br>
>Si le changement de nom ou la suppression d’une colonne est nécessaire, nous vous avertirons à l’avance de ces modifications.

### Niveau d’accès

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Niveau d’accès</td>
            <td>Niveau d’accès</td>
            <td>ACSLVL</td>
            <td>Niveau d’accès</td>
            <td>ACCESSLEVELS_CURRENT<br>ACCESSLEVELS_DAILY_HISTORY<br>ACCESSLEVELS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ACCESSLEVELID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>APPGLOBALID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>ID D’ACCESSLEVEL HÉRITÉ</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variable, basée sur OBJCODE</td>
             <td>Clé primaire/ID de l’objet identifié dans le champ OBJCODE</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
    </tbody>
</table>

### Règle d&#39;accès

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Règle d'accès</td>
            <td>Partager</td>
            <td>ACSRUL</td>
            <td>Partager</td>
            <td>ACCESSRULES_CURRENT<br>ACCESSRULES_DAILY_HISTORY<br>ACCESSRULES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ACCESSORID</td>
             <td>FK</td>
             <td>Variable, basée sur ACCESSOROBJCODE</td>
             <td>Clé primaire/ID de l’objet identifié dans le champ ACCESSOROBJCODE</td>
        </tr>
        <tr>
             <td>ACCESSRULEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ANCESTORID</td>
             <td>PK</td>
             <td>Variable, basée sur ANCESTOROBJCODE</td>
             <td>Clé primaire/ID de l’objet identifié dans le champ ANCESTOROBJCODE</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SECURITYOBJID</td>
             <td>FK</td>
             <td>Variable, basée sur SECURITYOBJCODE</td>
             <td>Clé primaire/ID de l’objet identifié dans le champ SECURITYOBJCODE</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
    </tbody>
</table>

### Chemin d&#39;approbation

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Chemin d'approbation</td>
            <td>Chemin d'approbation</td>
            <td>ARVPTH</td>
            <td>Approbation</td>
            <td>APPROVALPATHS_CURRENT<br>APPROVALPATHS_DAILY_HISTORY<br>APPROVALPATHS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPROVALPATHID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>APPROVALPROCESSID</td>
             <td>FK</td>
             <td>APPROVALPROCESSES_CURRENT</td>
             <td>APPROVALPROCESSID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GLOBALPATHID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
    </tbody>
</table>

### Processus d’approbation

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Processus d’approbation</td>
            <td>Processus d’approbation</td>
            <td>ARVPRC</td>
            <td>Processus d’approbation</td>
            <td>APPROVALPROCESSES_CURRENT<br>APPROVALPROCESSES_DAILY_HISTORY<br>APPROVALPROCESSES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPROVALPROCESSID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
    </tbody>
</table>

### Étape d’approbation

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Étape d’approbation</td>
            <td>Étape d’approbation</td>
            <td>ARVSTP</td>
            <td>Étape d’approbation</td>
            <td>APPROVALSTEPS_CURRENT<br>APPROVALSTEPS_DAILY_HISTORY<br>APPROVALSTEPS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPROVALPATHID</td>
             <td>FK</td>
             <td>APPROVALPATHS_CURRENT</td>
             <td>APPROVALPATHID</td>
        </tr>
        <tr>
             <td>APPROVALSTEPID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
    </tbody>
</table>

### Statut de l&#39;approbateur

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Statut de l'approbateur</td>
            <td>Statut de l'approbateur</td>
            <td>ARVSTS</td>
            <td>ApproverStatus</td>
            <td>APPROVERSTATUSES_CURRENT<br>APPROVERSTATUSES_DAILY_HISTORY<br>APPROVERSTATUSES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPROVERSTATUSID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>APPROVABLEOBJID</td>
             <td>FK</td>
             <td>Variable, basée sur APPROVABLEOBJCODE</td>
             <td>Clé primaire/ID de l'objet identifié dans le champ APPROVABLEOBJCODE</td>
        </tr>
        <tr>
             <td>APPROVALSTEPID</td>
             <td>FK</td>
             <td>APPROVALSTEPS_CURRENT</td>
             <td>APPROVALSTEPID</td>
        </tr>
        <tr>
             <td>APPROVEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>DELEGATEUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>OVERRIDDENUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>STEPAPPROVERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSYSYID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>WILDCARDUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Affectation

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Affectation</td>
            <td>Affectation</td>
            <td>ASSGN</td>
            <td>Affectation</td>
            <td>ASSIGNMENTS_CURRENT<br>ASSIGNMENTS_DAILY_HISTORY<br>ASSIGNMENTS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ASSIGNEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>ASSIGNEDTOID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>ASSIGNMENTID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>CLASSIFIERID</td>
             <td>FK</td>
             <td>CLASSIFIER_CURRENT</td>
             <td>CLASSIFIERID</td>
        </tr>
      <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>PRIVATERATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>TEAMID</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>TEAMID</td>
        </tr>
    </tbody>
</table>

### Approbations en attente

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Approbations en attente</td>
            <td>Approbations en attente</td>
            <td>AWAPVL</td>
            <td>Approbations en attente</td>
            <td>AWAITINGAPPROVALS_CURRENT<br>AWAITINGAPPROVALS_DAILY_HISTORY<br>AWAITINGAPPROVALS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ACCESSREQUESTID</td>
             <td>-</td>
             <td colspan="2">Le tableau des demandes d'accès n'est pas pris en charge actuellement</td>
        </tr>
        <tr>
             <td>ID APPROUVABLE</td>
             <td>FK</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>APPROVERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>EN ATTENTE DE VALIDITÉ</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>DOCUMENTID</td>
             <td>FK</td>
             <td>DOCUMENTS_CURRENT</td>
             <td>DOCUMENTID</td>
        </tr>
        <tr>
             <td>DOCUMENTVERSIONID</td>
             <td>FK</td>
             <td>DOCUMENTVERSIONS_CURRENT</td>
             <td>DOCUMENTVERSIONID</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SUBMITTEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>TEAMID</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>TEAMID</td>
        </tr>
        <tr>
             <td>TIMESHEETID</td>
             <td>FK</td>
             <td>TIMESHEETS_CURRENT</td>
             <td>TIMESHEETID</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Niveau de référence

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Niveau de référence</td>
            <td>Niveau de référence</td>
            <td>AVEUGLE</td>
            <td>Niveau de référence</td>
            <td>BASELINES_CURRENT<br>BASELINES_DAILY_HISTORY<br>BASELINES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>BASELINEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
    </tbody>
</table>

### Tâche de ligne de base

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Tâche de ligne de base</td>
            <td>Tâche de ligne de base</td>
            <td>BSTSK</td>
            <td>Tâche de ligne de base</td>
            <td>BASELINETASKS_CURRENT<br>BASELINETASKS_DAILY_HISTORY<br>BASELINETASKS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>BASELINEID</td>
             <td>FK</td>
             <td>BASELINES_CURRENT</td>
             <td>BASELINEID</td>
        </tr>
        <tr>
             <td>BASELINETASKID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
    </tbody>
</table>

### Taux de facturation

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Taux de facturation</td>
            <td>Taux ou taux de remplacement</td>
            <td>TAUX</td>
            <td>Taux de facturation</td>
            <td>RATES_CURRENT<br>RATES_DAILY_HISTORY<br>RATES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ASSIGNMENTID</td>
             <td>FK</td>
             <td>ASSIGNMENTS_CURRENT</td>
             <td>ASSIGNMENTID</td>
        </tr>
        <tr>
             <td>CLASSIFIERID</td>
             <td>FK</td>
             <td>CLASSIFIER_CURRENT</td>
             <td>CLASSIFIERID</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>NLBRCATEGORYID</td>
             <td>FK</td>
             <td>NLBRCATEGORIES_CURRENT</td>
             <td>NLBRCATEGORYID</td>
        </tr>
        <tr>
             <td>NONLABORRESOURCEID</td>
             <td>FK</td>
             <td>NONLABORRESOURCES_CURRENT</td>
             <td>NONLABORRESOURCEID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variable, basée sur OBJCODE</td>
             <td>Clé primaire/ID de l’objet identifié dans le champ OBJCODE</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>RATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>RATEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SOURCERATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Enregistrement de facturation

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Enregistrement de facturation</td>
            <td>Enregistrement de facturation</td>
            <td>FACTURE</td>
            <td>Enregistrement de facturation</td>
            <td>BILLINGRECORDS_CURRENT<br>BILLINGRECORDS_DAILY_HISTORY<br>BILLINGRECORDS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>BILLINGRECORDID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>INVOICEID</td>
             <td>-</td>
             <td colspan="2">Table des factures non prise en charge actuellement</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
    </tbody>
</table>

### Réservation

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Réservation</td>
            <td>Réservation</td>
            <td>RÉSERVATION</td>
            <td>Réservation</td>
            <td>BOOKINGS_CURRENT<br>BOOKINGS_DAILY_HISTORY<br>BOOKINGS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>BOOKINGID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>NLBRCATEGORYID</td>
             <td>FK</td>
             <td>NLBRCATEGORIES_CURRENT</td>
             <td>NLBRCATEGORYID</td>
        </tr>
        <tr>
             <td>NONLABORRESOURCEID</td>
             <td>FK</td>
             <td>NONLABORRESOURCES_CURRENT</td>
             <td>NONLABORRESOURCEID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variable, basée sur OBJCODE</td>
             <td>Clé primaire/ID de l’objet identifié dans le champ OBJCODE</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
        <tr>
             <td>TEMPLATETASKID</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATETASKID</td>
        </tr>
        <tr>
             <td>TOPOBJID</td>
             <td>FK</td>
             <td>Variable, basée sur TOPOBJCODE</td>
             <td>Clé primaire/ID de l'objet identifié dans le champ TOPOBJCODE</td>
        </tr>
    </tbody>
</table>

### Profil professionnel

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Profil professionnel</td>
            <td>Profil professionnel</td>
            <td>BSNPRF</td>
            <td>BusinessProfile</td>
            <td>BUSINESSPROFILE_CURRENT<br>BUSINESSPROFILE_DAILY_HISTORY<br>BUSINESSPROFILE_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ACCESSLEVELID</td>
             <td>FK</td>
             <td>ACCESSLEVELS_CURRENT</td>
             <td>ACCESSLEVELID</td>
        </tr>
        <tr>
             <td>BUSINESSPROFILEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
    </tbody>
</table>

### Règles métier

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Règles métier</td>
            <td>Règles métier</td>
            <td>BNRUL</td>
            <td>Règles métier</td>
            <td>BUSINESSRULE_CURRENT<br>BUSINESSRULE_DAILY_HISTORY<br>BUSINESSRULE_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>BUSINESSRULEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
    </tbody>
</table>

### Catégorie

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Catégorie</td>
            <td>Formulaire personnalisé</td>
            <td>VINGT</td>
            <td>Catégorie</td>
            <td>CATEGORIES_CURRENT<br>CATEGORIES_DAILY_HISTORY<br>CATEGORIES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CATEGORYID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
    </tbody>
</table>

### Paramètre de catégorie

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Paramètre de catégorie</td>
            <td>Champs de formulaire personnalisés</td>
            <td>CTGYPA</td>
            <td>Paramètre de catégorie</td>
            <td>CATEGORIESPARAMETERS_CURRENT<br>CATEGORIESPARAMETERS_DAILY_HISTORY<br>CATEGORIESPARAMETERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CATEGORIESPARAMETERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>PARAMETERGROUPID</td>
             <td>FK</td>
             <td>PARAMETERGROUPS_CURRENT</td>
             <td>PARAMETERGROUPID</td>
        </tr>
        <tr>
             <td>PARAMETERID</td>
             <td>FK</td>
             <td>PARAMETERS_CURRENT</td>
             <td>PARAMETERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
    </tbody>
</table>

### Classificateur

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Classificateur</td>
            <td>Emplacement</td>
            <td>CLSF</td>
            <td>Emplacement</td>
            <td>CLASSIFIER_CURRENT<br>CLASSIFIER_DAILY_HISTORY<br>CLASSIFIER_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CLASSIFIERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PARENTID</td>
             <td>FK</td>
             <td>CLASSIFIER_CURRENT</td>
             <td>CLASSIFIERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
    </tbody>
</table>

### Entreprise

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Entreprise</td>
            <td>Entreprise</td>
            <td>CMPY</td>
            <td>Entreprise</td>
            <td>COMPANIES_CURRENT<br>COMPANIES_DAILY_HISTORY<br>COMPANIES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>COMPANYID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PRIVATERATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
    </tbody>
</table>

### Trimestre personnalisé

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Trimestre personnalisé</td>
            <td>Trimestre personnalisé</td>
            <td>DÉMARRER</td>
            <td>Trimestre personnalisé</td>
            <td>CUSTOMQUARTERS_CURRENT<br>CUSTOMQUARTERS_DAILY_HISTORY<br>CUSTOMQUARTERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CUSTOMQUARTERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
    </tbody>
</table>

### Énumération personnalisée

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>CustomEnum</td>
            <td>Statut, Priorité, Gravité, Statut</td>
            <td>SYSTÈME</td>
            <td>Énumération personnalisée</td>
            <td>CUSTOMENUMS_CURRENT<br>CUSTOMENUMS_DAILY_HISTORY<br>CUSTOMENUMS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CUSTOMENUMID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
    </tbody>
</table>

>[!NOTE]
>
>Le type d’enregistrement est identifié via la propriété `enumClass` . Voici les types attendus :<br>
><ul><li>CONDITION_OPTASK</li>
&gt;<li>CONDITION_PROJ</li>
&gt;<li>CONDITION_TASK</li>
&gt;<li>PRIORITY_OPTASK</li>
&gt;<li>PRIORITY_PROJ</li>
&gt;<li>PRIORITY_TASK</li>
&gt;<li>SEVERITY_OPTASK</li>
&gt;<li>STATUS_OPTASK</li>
&gt;<li>STATUS_PROJ</li>
&gt;<li>STATUS_TASK</li></ul>


### Document

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Document</td>
            <td>Document</td>
            <td>DOCU</td>
            <td>Document</td>
            <td>DOCUMENTS_CURRENT<br>DOCUMENTS_DAILY_HISTORY<br>DOCUMENTS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>CHECKEDOUTBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>DOCUMENTID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>DOCUMENTREQUESTID</td>
             <td>-</td>
             <td colspan="2">Le tableau de demande de document n’est actuellement pas pris en charge</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>ITÉRATIONID</td>
             <td>FK</td>
             <td>ITÉRATIONS_CURRENT</td>
             <td>ITÉRATIONID</td>
        </tr>
        <tr>
             <td>LASTNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>NOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variable, basée sur OBJCODE</td>
             <td>Clé primaire/ID de l’objet identifié dans le champ OBJCODE</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PORTFOLIOID</td>
             <td>FK</td>
             <td>PORTFOLIOS_CURRENT</td>
             <td>PORTFOLIOID</td>
        </tr>
        <tr>
             <td>PROGRAMID</td>
             <td>FK</td>
             <td>PROGRAMMES_ACTUELS</td>
             <td>PROGRAMID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>RELEASEVERSIONID</td>
             <td>-</td>
             <td colspan="2">Le tableau des versions de version n’est actuellement pas pris en charge</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
        <tr>
             <td>TEMPLATETASKID</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATETASKID</td>
        </tr>
        <tr>
             <td>TOPOBJID</td>
             <td>FK</td>
             <td>Variable, basée sur TOPOBJCODE</td>
             <td>Clé primaire/ID de l'objet identifié dans le champ TOPOBJCODE</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Approbation du document

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Approbation du document</td>
            <td>Approbation du document</td>
            <td>DOCAPL</td>
            <td>Approbation du document</td>
            <td>DOCAPPROVALS_CURRENT<br>DOCAPPROVALS_DAILY_HISTORY<br>DOCAPPROVALS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPROVERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>DOCAPPROVALID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>DOCUMENTID</td>
             <td>FK</td>
             <td>DOCUMENTS_CURRENT</td>
             <td>DOCUMENTID</td>
        </tr>
        <tr>
             <td>NOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>ID DU DEMANDEUR</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
    </tbody>
</table>

### Approbation du document (NOUVEAU)

Disponibilité limitée des clients

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Approbation du document</td>
            <td>Approbation</td>
            <td>S/O</td>
            <td>S/O</td>
            <td>APPROVAL_CURRENT<br>APPROVAL_DAILY_HISTORY<br>APPROVAL_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td class="key">APPROVALID</td>
             <td>PK</td>
             <td>-</td>
             <td>REMARQUE : il s'agit également de l'ID de l'objet DOCUMENTVERSION auquel l'approbation est associée.</td>
        </tr>
        <tr>
             <td class="key">ASSETID</td>
             <td>FK</td>
             <td>Variable, basée sur ASSETTYPE</td>
             <td>Clé primaire/ID de l’objet identifié dans le champ ASSETTYPE</td>
        </tr>
        <tr>
             <td class="key">CREATORID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td class="key">EAUTHTENANTID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td class="key">PRODUCTID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td class="key">REALCREATORID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Étape d&#39;approbation du document (NOUVEAU)

Disponibilité limitée des clients

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Étape d’approbation du document</td>
            <td>Étape d’approbation</td>
            <td>S/O</td>
            <td>S/O</td>
            <td>APPROVAL_STAGE_CURRENT<br>APPROVAL_STAGE_DAILY_HISTORY<br>APPROVAL_STAGE_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td class="key">APPROVALID</td>
             <td>FK</td>
             <td>APPROVAL_CURRENT</td>
             <td>APPROVALID</td>
        </tr>
        <tr>
             <td class="key">APPROVALSTAGEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td class="key">CREATORID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td class="key">OBJID</td>
             <td class="type">FK</td>
             <td class="relatedtable">Variable, basée sur OBJCODE</td>
             <td>Clé primaire/ID de l’objet identifié dans le champ OBJCODE</td>
        </tr>
    </tbody>
</table>

### Participants à l&#39;étape d&#39;approbation du document (NOUVEAU)

Disponibilité limitée des clients

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Personne participant à l’étape d’approbation du document</td>
            <td>Décisions d'approbation</td>
            <td>S/O</td>
            <td>S/O</td>
            <td>APPROVAL_STAGE_PARTICIPANT_CURRENT<br>APPROVAL_STAGE_PARTICIPANT_DAILY_HISTORY<br>APPROVAL_STAGE_PARTICIPANT_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td class="key">APPROVALID</td>
             <td>FK</td>
             <td>APPROVAL_CURRENT</td>
             <td>APPROVALID</td>
        </tr>
        <tr>
             <td class="key">APPROVALSTAGEPARTICIPANTID/td&gt;
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td class="key">ASSETID</td>
             <td>FK</td>
             <td>Variable, basée sur ASSETTYPE</td>
             <td>Clé primaire/ID de l’objet identifié dans le champ ASSETTYPE</td>
        </tr>
        <tr>
             <td class="key">DECISIONUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td class="key">OBJID</td>
             <td class="type">FK</td>
             <td class="relatedtable">Variable, basée sur OBJCODE</td>
             <td>Clé primaire/ID de l’objet identifié dans le champ OBJCODE</td>
        </tr>
        <tr>
             <td class="key">PARTICIPANTID</td>
             <td>FK</td>
             <td class="relatedtable">Variable, basée sur PARTICIPANTTYPE</td>
             <td>Clé primaire/ID de l’objet identifié dans le champ PARTICIPANTTYPE</td>
        </tr>
        <tr>
             <td class="key">REALREQUESTORID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td class="key">REALUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td class="key">ID DU DEMANDEUR</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td class="key">STAGEID</td>
             <td>FK</td>
             <td>APPROVAL_STAGE_CURRENT</td>
             <td>STAGEID</td>
        </tr>
    </tbody>
</table>

### Dossier de documents

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Dossier de documents</td>
            <td>Dossier de documents</td>
            <td>DOCFLD</td>
            <td>DocsFolders</td>
            <td>DOCFOLDERS_CURRENT<br>DOCFOLDERS_DAILY_HISTORY<br>DOCFOLDERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>DOCFOLDERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>ID DE PROBLÈME</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>ITÉRATIONID</td>
             <td>FK</td>
             <td>ITÉRATIONS_CURRENT</td>
             <td>ITÉRATIONID</td>
        </tr>
        <tr>
             <td>LINKEDFOLDERID</td>
             <td>FK</td>
             <td>LINKEDFOLDERS_CURRENT</td>
             <td>LINKEDFOLDERID</td>
        </tr>
        <tr>
             <td>PARENTID</td>
             <td>FK</td>
             <td>DOCFOLDERS_CURRENT</td>
             <td>DOCFOLDERID</td>
        </tr>
        <tr>
             <td>PORTFOLIOID</td>
             <td>FK</td>
             <td>PORTFOLIOS_CURRENT</td>
             <td>PORTFOLIOID</td>
        </tr>
        <tr>
             <td>PROGRAMID</td>
             <td>FK</td>
             <td>PROGRAMMES_ACTUELS</td>
             <td>PROGRAMID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
        <tr>
             <td>TEMPLATETASKID</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATETASKID</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Métadonnées du fournisseur de documents

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Métadonnées du fournisseur de documents</td>
            <td>Métadonnées du fournisseur de documents</td>
            <td>DOCUMENT</td>
            <td>DocumentProviderMetadata</td>
            <td>DOCPROVIDERMETA_CURRENT<br>DOCPROVIDERMETA_DAILY_HISTORY<br>DOCPROVIDERMETA_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>DOCPROVIDERMETAID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
    </tbody>
</table>

### Fournisseur de documents

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Fournisseur de documents</td>
            <td>Fournisseur de documents</td>
            <td>DOCPRO</td>
            <td>Fournisseur de documents</td>
            <td>DOCPROVIDERS_CURRENT<br>DOCPROVIDERS_DAILY_HISTORY<br>DOCPROVIDERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>DOCPROVIDERCONFIGID</td>
             <td>FK</td>
             <td>DOCPROVIDERCONFIG_CURRENT</td>
             <td>DOCPROVIDERCONFIGID</td>
        </tr>
        <tr>
             <td>DOCPROVIDERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
    </tbody>
</table>

### Configuration du fournisseur de documents

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Configuration du fournisseur de documents</td>
            <td>Configuration du fournisseur de documents</td>
            <td>DOCCFG</td>
            <td>DocumentProviderConfig</td>
            <td>DOCPROVIDERCONFIG_CURRENT<br>DOCPROVIDERCONFIG_DAILY_HISTORY<br>DOCPROVIDERCONFIG_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>DOCPROVIDERCONFIGID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
    </tbody>
</table>

### Version du document

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Version du document</td>
            <td>Version du document</td>
            <td>DOCV</td>
            <td>Version du document</td>
            <td>DOCUMENTVERSIONS_CURRENT<br>DOCUMENTVERSIONS_DAILY_HISTORY<br>DOCUMENTVERSIONS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>DOCUMENTID</td>
             <td>FK</td>
             <td>DOCUMENTS_CURRENT</td>
             <td>DOCUMENTID</td>
        </tr>
        <tr>
             <td>DOCUMENTPROVIDERID</td>
             <td>FK</td>
             <td>DOCPROVIDERS_CURRENT</td>
             <td>DOCUMENTPROVIDERID</td>
        </tr>
        <tr>
             <td>DOCUMENTVERSIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>EXTERNALSTORAGEID</td>
             <td>-</td>
             <td colspan="2">ID externe dans le système de stockage externe</td>
        </tr>
        <tr>
             <td>PROOFAPPROVALSTATUSID</td>
             <td>-</td>
             <td colspan="2">Le tableau Statut d'approbation de l'épreuve n'est pas pris en charge actuellement</td>
        </tr>
        <tr>
             <td>PROOFEDBYUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PROOFID</td>
             <td>-</td>
             <td colspan="2">La table d'épreuve n'est pas prise en charge actuellement</td>
        </tr>
        <tr>
             <td>PROOFOWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PROOFSTAGEID</td>
             <td>FK</td>
             <td>-</td>
             <td colspan="2">Le tableau Étape de l'épreuve n'est pas pris en charge actuellement</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
    </tbody>
</table>

### Taux de change

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Taux de change</td>
            <td>Taux de change</td>
            <td>EXRATE</td>
            <td>Taux de change</td>
            <td>EXCHANGERATES_CURRENT<br>EXCHANGERATES_DAILY_HISTORY<br>EXCHANGERATES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
    </tbody>
</table>

### Frais

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Frais</td>
            <td>Frais</td>
            <td>EXPNS</td>
            <td>Frais</td>
            <td>EXPENSES_CURRENT<br>EXPENSES_DAILY_HISTORY<br>EXPENSES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>BILLINGRECORDID</td>
             <td>FK</td>
             <td>BILLINGRECORDS_CURRENT</td>
             <td>BILLINGRECORDID</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>EXPENSEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>EXPENSETYPEID</td>
             <td>FK</td>
             <td>EXPENSETYPES_CURRENT</td>
             <td>EXPENSETYPEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variable, basée sur OBJCODE</td>
             <td>Clé primaire/ID de l’objet identifié dans le champ OBJCODE</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
        <tr>
             <td>TEMPLATETASKID</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATETASKID</td>
        </tr>
        <tr>
             <td>TOPOBJID</td>
             <td>FK</td>
             <td>Variable, basée sur TOPBJCODE</td>
             <td>Clé primaire/ID de l'objet identifié dans le champ TOPBJCODE</td>
        </tr>
    </tbody>
</table>

### Type de frais

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Type de frais</td>
            <td>Type de frais</td>
            <td>EXPTYP</td>
            <td>Type de frais</td>
            <td>EXPENSETYPES_CURRENT<br>EXPENSETYPES_DAILY_HISTORY<br>EXPENSETYPES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPGLOBALID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>EXPENSETYPEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variable, basée sur OBJCODE</td>
             <td>Clé primaire/ID de l’objet identifié dans le champ OBJCODE</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
    </tbody>
</table>

### Groupe

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Groupe</td>
            <td>Groupe</td>
            <td>GROUP</td>
            <td>Groupe</td>
            <td>GROUPS_CURRENT<br>GROUPS_DAILY_HISTORY<br>GROUPS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>BUSINESSLEADERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>LAYOUTTEMPLATEID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>PARENTID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>ROOTID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>UITEMPLATEID</td>
             <td>FK</td>
             <td>UITEMPLATES_CURRENT</td>
             <td>UITEMPLATEID</td>
        </tr>
    </tbody>
</table>

### Heure

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Heure</td>
            <td>Heure</td>
            <td>HOUR</td>
            <td>Heure</td>
            <td>HOURS_CURRENT<br>HOURS_DAILY_HISTORY<br>HOURS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPROVEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>BILLINGRECORDID</td>
             <td>FK</td>
             <td>BILLINGRECORDS_CURRENT</td>
             <td>BILLINGRECORDID</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>CLASSIFIERID</td>
             <td>FK</td>
             <td>CLASSIFIER_CURRENT</td>
             <td>CLASSIFIERID</td>
        </tr>
        <tr>
             <td>DUPID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>EXTERNALTIMESHEETID</td>
             <td>-</td>
             <td colspan="2">N’est pas une relation Workfront ; utilisé pour l’intégration à des systèmes externes.
Self</td>
        </tr>
        <tr>
             <td>HOURID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>HOURTYPEID</td>
             <td>FK</td>
             <td>HOURTYPES_CURRENT</td>
             <td>HOURTYPEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>PROJECTOVERHEADID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>TIMESHEETID</td>
             <td>FK</td>
             <td>TIMESHEETS_CURRENT</td>
             <td>TIMESHEETID</td>
        </tr>
    </tbody>
</table>

### Type d’heure

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Type d’heure</td>
            <td>Type d’heure</td>
            <td>HEURE</td>
            <td>Type d’heure</td>
            <td>HOURTYPES_CURRENT<br>HOURTYPES_DAILY_HISTORY<br>HOURTYPES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPGLOBALID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>HOURTYPEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variable, basée sur OBJCODE</td>
             <td>Clé primaire/ID de l’objet identifié dans le champ OBJCODE</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
    </tbody>
</table>

### Itération

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Itération</td>
            <td>Itération</td>
            <td>RETOUR</td>
            <td>Itération</td>
            <td>ITERATIONS_CURRENT<br>ITERATIONS_DAILY_HISTORY<br>ITERATIONS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>ITÉRATIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>TEAMID</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>TEAMID</td>
        </tr>
    </tbody>
</table>

### Entrée au journal

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Entrée au journal</td>
            <td>Entrée au journal</td>
            <td>JRNLE</td>
            <td>Entrée au journal</td>
            <td>JOURNALENTRIES_CURRENT<br>JOURNALENTRIES_DAILY_HISTORY<br>JOURNALENTRIES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPROVERSTATUSID</td>
             <td>FK</td>
             <td>APPROVERSTATUSES_CURRENT</td>
             <td>APPROVERSTATUSID</td>
        </tr>
        <tr>
             <td>ASSIGNMENTID</td>
             <td>FK</td>
             <td>ASSIGNMENTS_CURRENT</td>
             <td>ASSIGNMENTID</td>
        </tr>
        <tr>
             <td>AUDITRECORDID</td>
             <td>-</td>
             <td colspan="2">Table des enregistrements d’audit non prise en charge actuellement</td>
        </tr>
        <tr>
             <td>BASELINEID</td>
             <td>FK</td>
             <td>BASELINES_CURRENT</td>
             <td>BASELINEID</td>
        </tr>
        <tr>
             <td>BILLINGRECORDID</td>
             <td>FK</td>
             <td>BILLINGRECORDS_CURRENT</td>
             <td>BILLINGRECORDID</td>
        </tr>
        <tr>
             <td>COMPANYID</td>
             <td>FK</td>
             <td>COMPANIES_CURRENT</td>
             <td>COMPANYID</td>
        </tr>
        <tr>
             <td>DOCUMENTID</td>
             <td>FK</td>
             <td>DOCUMENTS_CURRENT</td>
             <td>DOCUMENTID</td>
        </tr>
        <tr>
             <td>DOCUMENTSHAREID</td>
             <td>-</td>
             <td colspan="2">Le tableau de partage de document n'est pas pris en charge actuellement</td>
        </tr>
        <tr>
             <td>EDITEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>EXPENSEID</td>
             <td>FK</td>
             <td>DEPENSES_CURRENT</td>
             <td>EXPENSEID</td>
        </tr>
        <tr>
             <td>HOURID</td>
             <td>FK</td>
             <td>HOURS_CURRENT</td>
             <td>HOURID</td>
        </tr>
        <tr>
             <td>INITIATIVEID</td>
             <td>-</td>
             <td colspan="2">Table d’initiative non prise en charge actuellement</td>
        </tr>
        <tr>
             <td>JOURNALENTRIESID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variable, basée sur OBJCODE</td>
             <td>Clé primaire/ID de l’objet identifié dans le champ OBJCODE</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>PORTFOLIOID</td>
             <td>FK</td>
             <td>PORTFOLIOS_CURRENT</td>
             <td>PORTFOLIOID</td>
        </tr>
        <tr>
             <td>PROGRAMID</td>
             <td>FK</td>
             <td>PROGRAMMES_ACTUELS</td>
             <td>PROGRAMID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>SUBOBJID</td>
             <td>FK</td>
             <td>Variable, basée sur SUBOBJCODE</td>
             <td>Clé primaire/ID de l’objet identifié dans le champ SUBOBJCODE</td>
        </tr>
        <tr>
             <td>SUBSCRIBEID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
        <tr>
             <td>TIMESHEETID</td>
             <td>FK</td>
             <td>TIMESHEETS_CURRENT</td>
             <td>TIMESHEETID</td>
        </tr>
        <tr>
             <td>TOPOBJID</td>
             <td>FK</td>
             <td>Variable, basée sur TOPOBJCODE</td>
             <td>Clé primaire/ID de l'objet identifié dans le champ TOPOBJCODE</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Dossier Lié

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Dossier Lié</td>
            <td>Dossier Lié</td>
            <td>LNKFDR</td>
            <td>LinkedFolder</td>
            <td>LINKEDFOLDERS_CURRENT<br>LINKEDFOLDERS_DAILY_HISTORY<br>LINKEDFOLDERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>DOCUMENTPROVIDERID</td>
             <td>FK</td>
             <td>DOCPROVIDERS_CURRENT</td>
             <td>DOCUMENTPROVIDERID</td>
        </tr>
        <tr>
             <td>EXTERNALSTORAGEID</td>
             <td>-</td>
             <td colspan="2">ID externe dans le système de stockage externe</td>
        </tr>
        <tr>
             <td>FOLDERID</td>
             <td>FK</td>
             <td>DOCFOLDERS_CURRENT</td>
             <td>FOLDERID</td>
        </tr>
        <tr>
             <td>LINKEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LINKEDFOLDERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
    </tbody>
</table>

### Jalon

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Jalon</td>
            <td>Jalon</td>
            <td>MILE</td>
            <td>Jalon</td>
            <td>MILESTONES_CURRENT<br>MILESTONES_DAILY_HISTORY<br>MILESTONES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>MILESTONEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>MILESTONEPATID</td>
             <td>FK</td>
             <td>MILESTONEPATHS_CURRENT</td>
             <td>MILESTONEPATID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
    </tbody>
</table>

### Chemin jalonné

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Chemin jalonné</td>
            <td>Chemin jalonné</td>
            <td>CHEMIN</td>
            <td>Chemin jalonné</td>
            <td>MILESTONEPATHS_CURRENT<br>MILESTONEPATHS_DAILY_HISTORY<br>MILESTONEPATHS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>MILESTONEPATID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
    </tbody>
</table>

### Ressource non liée à la main-d’œuvre

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Ressource non liée à la main-d’œuvre</td>
            <td>Ressource non liée à la main-d’œuvre</td>
            <td>NLBR</td>
            <td>Ressource non liée à la main-d’œuvre</td>
            <td>NONLABORRESOURCES_CURRENT<br>NONLABORRESOURCES_DAILY_HISTORY<br>NONLABORRESOURCES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>NONLABORRESOURCEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>HOMEGROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>NONLABORRESOURCECATEGORYID</td>
             <td>FK</td>
             <td>NLBRCATEGORIES_CURRENT</td>
             <td>NLBRCATEGORYID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
    </tbody>
</table>

### Catégorie de ressources non liée à la main-d’œuvre

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Catégorie de ressources non liée à la main-d’œuvre</td>
            <td>Catégorie de ressources non liée à la main-d’œuvre</td>
            <td>NLBRCY</td>
            <td>Catégorie de ressource non liée à la main d’œuvre</td>
            <td>NLBRCATEGORIES_CURRENT<br>NLBRCATEGORIES_DAILY_HISTORY<br>NLBRCATEGORIES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>NLBRCATEGORYID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>PRIVATERATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>SCHEDULEID</td>
             <td>FK</td>
             <td>SCHEDULES_CURRENT</td>
             <td>SCHEDULEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
    </tbody>
</table>

### Jour Non Ouvré

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Jour Non Ouvré</td>
            <td>Exception de planification</td>
            <td>NONWKD</td>
            <td>Jour non ouvrables</td>
            <td>NONWORKDAYS_CURRENT<br>NONWORKDAYS_DAILY_HISTORY<br>NONWORKDAYS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>NONWORKDAY ID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variable, basée sur OBJCODE</td>
             <td>Clé primaire/ID de l’objet identifié dans le champ OBJCODE</td>
        </tr>
        <tr>
             <td>SCHEDULEID</td>
             <td>FK</td>
             <td>SCHEDULES_CURRENT</td>
             <td>SCHEDULEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Note

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Note</td>
            <td>Note</td>
            <td>NOTE</td>
            <td>Note</td>
            <td>NOTES_CURRENT<br>NOTES_DAILY_HISTORY<br>NOTES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ATTACHDOCUMENTID</td>
             <td>FK</td>
             <td>DOCUMENTS_CURRENT</td>
             <td>DOCUMENTID</td>
        </tr>
        <tr>
             <td>ATTACHOBJID</td>
             <td>FK</td>
             <td>Variable, basée sur ATTACHOBJCODE</td>
             <td>Clé primaire/ID de l'objet identifié dans l'OBJCODE ATTACHOBJCODE</td>
        </tr>
        <tr>
             <td>ATTACHOPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>ATTACHWORKID</td>
             <td>FK</td>
             <td>WORKITEMS_CURRENT</td>
             <td>WORKITEMID</td>
        </tr>
        <tr>
             <td>ATTACHWORKUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>AUDITRECORDID</td>
             <td>-</td>
             <td colspan="2">Le tableau des enregistrements d’audit n’est pas pris en charge actuellement</td>
        </tr>
        <tr>
             <td>COMPANYID</td>
             <td>FK</td>
             <td>COMPANIES_CURRENT</td>
             <td>COMPANYID</td>
        </tr>
        <tr>
             <td>DOCUMENTID</td>
             <td>FK</td>
             <td>DOCUMENTS_CURRENT</td>
             <td>DOCUMENTID</td>
        </tr>
        <tr>
             <td>EXTERNALSERVICEID</td>
             <td>-</td>
             <td colspan="2">N’est pas une relation Workfront ; utilisé pour l’intégration à des systèmes externes.</td>
        </tr>
        <tr>
             <td>ITÉRATIONID</td>
             <td>FK</td>
             <td>ITÉRATIONS_CURRENT</td>
             <td>ITÉRATIONID</td>
        </tr>
        <tr>
             <td>NOTEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variable, basée sur NOTEOBJCODE</td>
             <td>Clé primaire/ID de l’objet identifié dans le champ NOTEOBJCODE</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PARENTENDORSEMENTID</td>
             <td>-</td>
             <td colspan="2">Table d’endossement non prise en charge actuellement</td>
        </tr>
        <tr>
             <td>PARENTJOURNALENTRYID</td>
             <td>FK</td>
             <td>JOURNALENTRIES_CURRENT</td>
             <td>JOURNALENTRYID</td>
        </tr>
        <tr>
             <td>PARENTNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>PORTFOLIOID</td>
             <td>FK</td>
             <td>PORTFOLIOS_CURRENT</td>
             <td>PORTFOLIOID</td>
        </tr>
        <tr>
             <td>PROGRAMID</td>
             <td>FK</td>
             <td>PROGRAMMES_ACTUELS</td>
             <td>PROGRAMID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>PROOFACTIONID</td>
             <td>-</td>
             <td colspan="2">Le tableau Action de l'épreuve n'est pas pris en charge actuellement</td>
        </tr>
        <tr>
             <td>PROOFID</td>
             <td>-</td>
             <td colspan="2">La table d'épreuve n'est pas prise en charge actuellement</td>
        </tr>
        <tr>
             <td>RICHTEXTNOTEID</td>
             <td>FK</td>
             <td>RESERVEDTEXTNOTES_CURRENT</td>
             <td>RICHTEXTNOTEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
        <tr>
             <td>TEMPLATETASKID</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATETASKID</td>
        </tr>
        <tr>
             <td>THREADID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>TIMESHEETID</td>
             <td>FK</td>
             <td>TIMESHEETS_CURRENT</td>
             <td>TIMESHEETID</td>
        </tr>
        <tr>
             <td>TOPOBJID</td>
             <td>FK</td>
             <td>Variable, basée sur TOPOBJCODE</td>
             <td>Clé primaire/ID de l'objet identifié dans le champ TOPOBJCODE</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>


</table>

### Intégration d’objet

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Intégration d’objet</td>
            <td>Intégration d’objet</td>
            <td>OBJINT</td>
            <td>ObjectIntegration</td>
            <td>OBJECTINTEGRATION_CURRENT<br>OBJECTINTEGRATION_DAILY_HISTORY<br>OBJECTINTEGRATION_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>LINKEDOBJECTID</td>
             <td>FK</td>
             <td>Variable, basée sur LINKEDOBJECTCODE</td>
             <td>Clé primaire/ID de l'objet identifié dans le champ LINKEDOBJECTCODE</td>
        </tr>
        <tr>
             <td>OBJECTINTEGRATIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variable, basée sur OBJCODE</td>
             <td>Clé primaire/ID de l’objet identifié dans le champ OBJCODE</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>

</table>

### Catégorie d&#39;objets

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Catégorie d'objets</td>
            <td>Catégories d’objets</td>
            <td>OBJET</td>
            <td>Catégorie d'objet</td>
            <td>OBJECTSCATEGORIES_CURRENT<br>OBJECTSCATEGORIES_DAILY_HISTORY<br>OBJECTSCATEGORIES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>OBJECTSCATEGORYID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variable, basée sur OBJCODE</td>
             <td>Clé primaire/ID de l’objet identifié dans le champ OBJCODE</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
    </tbody>
</table>

### Tâche/Événement d&#39;opération

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>TâcheOp</td>
            <td>Événement, demande</td>
            <td>OPTASK</td>
            <td>Problème</td>
            <td>OPTASKS_CURRENT<br>OPTASKS_DAILY_HISTORY<br>OPTASKS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPROVALPROCESSID</td>
             <td>FK</td>
             <td>APPROVALPROCESSES_CURRENT</td>
             <td>APPROVALPROCESSID</td>
        </tr>
        <tr>
             <td>ASSIGNEDTOID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>CURRENTAPPROVALSTEPID</td>
             <td>FK</td>
             <td>APPROVALSTEPS_CURRENT</td>
             <td>APPROVALSTEPID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>ITÉRATIONID</td>
             <td>FK</td>
             <td>ITÉRATIONS_CURRENT</td>
             <td>ITÉRATIONID</td>
        </tr>
        <tr>
             <td>KANBANBOARDID</td>
             <td>-</td>
             <td colspan="2">La table de tableau kanban n’est actuellement pas prise en charge</td>
        </tr>
        <tr>
             <td>LASTCONDITIONNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>QUEUEDEFID</td>
             <td>-</td>
             <td colspan="2">Le tableau de définition de file d'attente n'est pas pris en charge actuellement</td>
        </tr>
        <tr>
             <td>QUEUETOPICID</td>
             <td>-</td>
             <td colspan="2">Le tableau Rubrique de file d'attente n'est pas pris en charge actuellement</td>
        </tr>
        <tr>
             <td>RESOLVEOPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>RESOLVEPROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>RESOLVETASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>RESOLVINGOBJID</td>
             <td>FK</td>
             <td>Variable, basée sur RESOLVINGOBJCODE</td>
             <td>Clé primaire/ID de l’objet identifié dans le champ RESOLVINGOBJCODE</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SOURCEOBJID</td>
             <td>FK</td>
             <td>Variable, basée sur SOURCEOBJCODE</td>
             <td>Clé primaire/ID de l’objet identifié dans le champ SOURCEOBJCODE</td>
        </tr>
        <tr>
             <td>SOURCETASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>SUBMITTEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>TEAMID</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>TEAMID</td>
        </tr>
    </tbody>
</table>

### Paramètre

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Paramètre</td>
            <td>Champ personnalisé</td>
            <td>PARAMÈTRE</td>
            <td>Paramètre</td>
            <td>PARAMETERS_CURRENT<br>PARAMETERS_DAILY_HISTORY<br>PARAMETERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PARAMETERFILTERID</td>
             <td>-</td>
             <td colspan="2">Tableau de filtres de paramètres actuellement non pris en charge</td>
        </tr>
        <tr>
             <td>PARAMETERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
    </tbody>
</table>

### Groupe de paramètres

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Groupe de paramètres</td>
            <td>Section du formulaire</td>
            <td>PARAMÈTRE</td>
            <td>Groupe de paramètres</td>
            <td>PARAMETERGROUPS_CURRENT<br>PARAMETERGROUPS_DAILY_HISTORY<br>PARAMETERGROUPS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PARAMETERGROUPID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
    </tbody>
</table>

### Option de paramètre

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Option de paramètre</td>
            <td>Option de paramètre</td>
            <td>POPT</td>
            <td>Option de paramètre</td>
            <td>PARAMETEROPTIONS_CURRENT<br>PARAMETEROPTIONS_DAILY_HISTORY<br>PARAMETEROPTIONS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>PARAMETERID</td>
             <td>FK</td>
             <td>PARAMETERS_CURRENT</td>
             <td>PARAMETERID</td>
        </tr>
        <tr>
             <td>PARAMETEROPTIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
    </tbody>
</table>

### Section/Rapport du portail

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Section du portail</td>
            <td>Rapport</td>
            <td>PTLSEC</td>
            <td>Rapport</td>
            <td>PORTALSECTIONS_CURRENT<br>PORTALSECTIONS_DAILY_HISTORY<br>PORTALSECTIONS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPGLOBALID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>FILTERID</td>
             <td>FK</td>
             <td>UIFILTERS_CURRENT</td>
             <td>FILTERID</td>
        </tr>
        <tr>
             <td>GROUPBYID</td>
             <td>FK</td>
             <td>UIGROUPBYS_CURRENT</td>
             <td>GROUPBYID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTVIEWEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variable, basée sur OBJCODE</td>
             <td>Clé primaire/ID de l’objet identifié dans le champ OBJCODE</td>
        </tr>
        <tr>
             <td>PORTALSECTIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>PREFERENCEID</td>
             <td>FK</td>
             <td>PREFERENCES_CURRENT</td>
             <td>PREFERENCEID</td>
        </tr>
        <tr>
             <td>PUBLICRUNASUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>REPORTFOLDERID</td>
             <td>FK</td>
             <td>REPORTFOLDERS_CURRENT</td>
             <td>REPORTFOLDERID</td>
        </tr>
        <tr>
             <td>RUNASUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SCHEDULEDREPORTID</td>
             <td>-</td>
             <td colspan="2">Le tableau Rapport planifié n’est actuellement pas pris en charge</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>VIEWID</td>
             <td>FK</td>
             <td>UIVIEWS_CURRENT</td>
             <td>VIEWID</td>
        </tr>
    </tbody>
</table>

### Onglet de portail/tableau de bord

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Onglet Portail</td>
            <td>Tableau de bord</td>
            <td>PTLTAB</td>
            <td>Tableau de bord</td>
            <td>PORTALTABS_CURRENT<br>PORTALTABS_DAILY_HISTORY<br>PORTALTABS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>DOCID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PORTALPROFILEID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>PORTALTABID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Section d&#39;onglet de portail

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Section d'onglet de portail</td>
            <td>Section Tableau de bord</td>
            <td>PRTBSC</td>
            <td>Section d'onglet de portail</td>
            <td>PORTALTABSPORTALSECTIONS_CURRENT<br>PORTALTABSPORTALSECTIONS_DAILY_HISTORY<br>PORTALTABSPORTALSECTIONS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CALENDARPORTALSECTIONID</td>
             <td>-</td>
             <td colspan="2">Section de portail de calendrier non prise en charge actuellement</td>
        </tr>
        <tr>
             <td>EXTERNALSECTIONID</td>
             <td>-</td>
             <td colspan="2">Le tableau des sections externes n'est pas pris en charge actuellement</td>
        </tr>
        <tr>
             <td>INTERNALSECTIONID</td>
             <td>FK</td>
             <td>PORTALSECTIONS_CURRENT</td>
             <td>PORTALSECTIONID</td>
        </tr>
        <tr>
             <td>PORTALSECTIONOBJID</td>
             <td>FK</td>
             <td>Variable, basée sur PORTALSECTIONOBJCODE</td>
             <td>Clé primaire/ID de l'objet identifié dans le champ PORTALSECTIONOBJCODE</td>
        </tr>
        <tr>
             <td>PORTALTABID</td>
             <td>FK</td>
             <td>PORTALTABS_CURRENT</td>
             <td>PORTALTABID</td>
        </tr>
        <tr>
             <td>PORTALTABSECTIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
    </tbody>
</table>

### Dernière visionneuse de section de portail

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>PortalSectionLastViewer</td>
            <td>Signaler les dernières visionneuses</td>
            <td>PLSLSV</td>
            <td>PortalSectionLastViewer</td>
            <td>REPORTLASTVIEWERS_CURRENT<br>REPORTLASTVIEWERS_DAILY_HISTORY<br>REPORTLASTVIEWERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>REPORTID</td>
             <td>FK</td>
             <td>PORTALSECTIONS_CURRENT</td>
             <td>REPORTID</td>
        </tr>
        <tr>
             <td>REPORTLASTVIEWERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>VIEWERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Portfolio

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Portfolio</td>
            <td>Portfolio</td>
            <td>PORT</td>
            <td>Portfolio</td>
            <td>PORTFOLIOS_CURRENT<br>PORTFOLIOS_DAILY_HISTORY<br>PORTFOLIOS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ALIGNMENTSCORECARDID</td>
             <td>-</td>
             <td colspan="2">Le tableau des cartes de performance n’est actuellement pas pris en charge</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PORTFOLIOID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
    </tbody>
</table>

### Préférence

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Préférence</td>
            <td>Affichage, Filtrage, Regroupement, Définition De Rapport</td>
            <td>PROSET</td>
            <td>Préférence</td>
            <td>PREFERENCES_CURRENT<br>PREFERENCES_DAILY_HISTORY<br>PREFERENCES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPGLOBALID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>PREFERENCEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
    </tbody>
</table>

### Programme

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Programme</td>
            <td>Programme</td>
            <td>PRGM</td>
            <td>Programme</td>
            <td>PROGRAMS_CURRENT<br>PROGRAMS_DAILY_HISTORY<br>PROGRAMS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PORTFOLIOID</td>
             <td>FK</td>
             <td>PORTFOLIOS_CURRENT</td>
             <td>PORTFOLIOID</td>
        </tr>
        <tr>
             <td>PROGRAMID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
    </tbody>
</table>

### Projet

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Projet</td>
            <td>Projet</td>
            <td>PROJ</td>
            <td>Projet</td>
            <td>PROJECTS_CURRENT<br>PROJECTS_DAILY_HISTORY<br>PROJECTS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>AEMNATIVEFOLDERTREESREFID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>ALIGNMENTSCORECARDID</td>
             <td>-</td>
             <td colspan="2">Le tableau des cartes de performance n’est actuellement pas pris en charge</td>
        </tr>
        <tr>
             <td>APPROVALPROCESSID</td>
             <td>FK</td>
             <td>APPROVALPROCESSES_CURRENT</td>
             <td>APPROVALPROCESSID</td>
        </tr>
        <tr>
             <td>ATTACHEDRATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>COMPANYID</td>
             <td>FK</td>
             <td>COMPANIES_CURRENT</td>
             <td>COMPANYID</td>
        </tr>
        <tr>
             <td>CONVERTEDOPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>CONVERTEDOPTASKORIGINATORID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>CURRENTAPPROVALSTEPID</td>
             <td>FK</td>
             <td>APPROVALSTEPS_CURRENT</td>
             <td>APPROVALSTEPID</td>
        </tr>
        <tr>
             <td>DELIVERABLESCORECARDID</td>
             <td>-</td>
             <td colspan="2">Le tableau des cartes de performance n’est actuellement pas pris en charge</td>
        </tr>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTCONDITIONNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>MILESTONEPATID</td>
             <td>FK</td>
             <td>MILESTONEPATHS_CURRENT</td>
             <td>MILESTONEPATID</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>POPACCOUNTID</td>
             <td>-</td>
             <td colspan="2">La table des comptes POP n’est actuellement pas prise en charge</td>
        </tr>
        <tr>
             <td>PORTFOLIOID</td>
             <td>FK</td>
             <td>PORTFOLIOS_CURRENT</td>
             <td>PORTFOLIOID</td>
        </tr>
        <tr>
             <td>PRIVATERATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>PROGRAMID</td>
             <td>FK</td>
             <td>PROGRAMMES_ACTUELS</td>
             <td>PROGRAMID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>QUEUEDEFID</td>
             <td>-</td>
             <td colspan="2">Le tableau de définition de file d'attente n'est pas pris en charge actuellement</td>
        </tr>
        <tr>
             <td>REJECTIONISSUEID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>RESOURCEPOOLID</td>
             <td>FK</td>
             <td>RESOURCEPOOLS_CURRENT</td>
             <td>RESOURCEPOOLID</td>
        </tr>
        <tr>
             <td>SCHEDULEID</td>
             <td>FK</td>
             <td>SCHEDULES_CURRENT</td>
             <td>SCHEDULEID</td>
        </tr>
        <tr>
             <td>SPONSORID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SUBMITTEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>TEAMID</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>TEAMID</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
    </tbody>
</table>

### Utilisateur de l&#39;équipe du projet

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Utilisateur de l'équipe du projet</td>
            <td>Utilisateur de l'équipe du projet</td>
            <td>PRTU</td>
            <td>Utilisateur du projet</td>
            <td>PROJECTSUSERS_CURRENT<br>PROJECTSUSERS_DAILY_HISTORY<br>PROJECTSUSERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>PROJECTSUSERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>TMPUSERID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Rôle d&#39;utilisateur d&#39;équipe de projet

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Rôle d'utilisateur d'équipe de projet</td>
            <td>Rôle d'utilisateur d'équipe de projet</td>
            <td>PTEAM</td>
            <td>ProjectUserRole</td>
            <td>PROJECTSUSERSROLES_CURRENT<br>PROJECTSUSERSROLES_DAILY_HISTORY<br>PROJECTSUSERSROLES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>PROJECTSUSERSROLEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Carte tarifaire

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Carte tarifaire</td>
            <td>Carte tarifaire</td>
            <td>CRTD</td>
            <td>Carte tarifaire</td>
            <td>RATECARD_CURRENT<br>RATECARD_DAILY_HISTORY<br>RATECARD_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>RATECARDID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SECURITYROOTID</td>
             <td>FK</td>
             <td>Variable, basée sur SECURITYOBJCODE</td>
             <td>Clé primaire/ID de l’objet identifié dans le champ SECURITYOBJCODE</td>
        </tr>
        <tr>
             <td>SOURCEID</td>
             <td>FK</td>
             <td>Variable, basée sur SOURCEOBJCODE</td>
             <td>Clé primaire/ID de l’objet identifié dans le champ SOURCEOBJCODE</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>

</table>

### Dossier des rapports

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Dossier des rapports</td>
            <td>Dossier des rapports</td>
            <td>RPTFDR</td>
            <td>Dossier des rapports</td>
            <td>REPORTFOLDERS_CURRENT<br>REPORTFOLDERS_DAILY_HISTORY<br>REPORTFOLDERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>REPORTFOLDERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
    </tbody>
</table>

### Nombre de statistiques de vues de rapports

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Nombre de statistiques de vues de rapports</td>
            <td>Nombre de statistiques de vues de rapports</td>
            <td>PLSVST</td>
            <td>PortalSectionStatisticInfo</td>
            <td>REPORTVIEWSTATISTICCOUNTS_CURRENT<br>REPORTVIEWSTATISTICCOUNTS_DAILY_HISTORY<br>REPORTVIEWSTATISTICCOUNTS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>REPORTID</td>
             <td>FK</td>
             <td>PORTALSECTIONS_CURRENT</td>
             <td>PORTALSECTIONID</td>
        </tr>
        <tr>
             <td>REPORTVIEWSTATISTICCOUNTID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
    </tbody>
</table>

### Heures budgétées à déclarer

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Heures budgétées à déclarer</td>
            <td>Heures budgétées à déclarer</td>
            <td>RPBGHR</td>
            <td>Heure budgétée</td>
            <td>REPORTABLEBUDGETEDHOURS_CURRENT<br>REPORTABLEBUDGETEDHOURS_DAILY_HISTORY<br>REPORTABLEBUDGETEDHOURS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>REPORTABLEBUDGETEDHOURID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Temps réservé / PTO

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Temps réservé</td>
            <td>Congés (personnels)</td>
            <td>RESVT</td>
            <td>Congés</td>
            <td>RESERVEDTIMES_CURRENT<br>RESERVEDTIMES_DAILY_HISTORY<br>RESERVEDTIMES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>RESERVEDTIMEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Gestionnaire des ressources

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Gestionnaire des ressources</td>
            <td>Gestionnaire des ressources</td>
            <td>RESMGR</td>
            <td>Gestionnaire des ressources</td>
            <td>RESOURCEMANAGERS_CURRENT<br>RESOURCEMANAGERS_DAILY_HISTORY<br>RESOURCEMANAGERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>RESOURCEMANAGERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
    </tbody>
</table>

### Pool de ressources

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Pool de ressources</td>
            <td>Pool de ressources</td>
            <td>RSPL</td>
            <td>Pool de ressources</td>
            <td>RSRCPOOLS_CURRENT<br>RSRCPOOLS_DAILY_HISTORY<br>RSRCPOOLS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>RESOURCEPOOLID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
    </tbody>
</table>

### Remarque Rich Text

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Remarque Rich Text</td>
            <td>Remarque Rich Text</td>
            <td>RHNOTE</td>
            <td>Remarque Rich Text</td>
            <td>RESERVEDTEXTNOTES_CURRENT<br>RESERVEDTEXTNOTES_DAILY_HISTORY<br>RESERVEDTEXTNOTES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>RICHTEXTNOTEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
    </tbody>
</table>

### Valeur de paramètre Rich Text

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Valeur de paramètre Rich Text</td>
            <td>Valeur de paramètre Rich Text</td>
            <td>ARCHVAL</td>
            <td>RichTextParameterValue</td>
            <td>RICHTEXTPARAMETERVALUES_CURRENT<br>RICHTEXTPARAMETERVALUES_DAILY_HISTORY<br>RICHTEXTPARAMETERVALUES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>PARAMETERVALUEID</td>
             <td>-</td>
             <td colspan="2">Tableau de valeurs de paramètres non pris en charge actuellement</td>
        </tr>
        <tr>
             <td>RICHTEXTPARAMETERVALUEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
    </tbody>
</table>

### Risque

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Risque</td>
            <td>Risque</td>
            <td>RISQUE</td>
            <td>Risque</td>
            <td>RISKS_CURRENT<br>RISKS_DAILY_HISTORY<br>RISKS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>RISKID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>RISKTYPEID</td>
             <td>FK</td>
             <td>RISKTYPES_CURRENT</td>
             <td>RISKTYPEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
    </tbody>
</table>

### Type de risque

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Type de risque</td>
            <td>Type de risque</td>
            <td>RSKTYPE</td>
            <td>Type de risque</td>
            <td>RISKTYPES_CURRENT<br>RISKTYPES_DAILY_HISTORY<br>RISKTYPES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>RISKTYPEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
    </tbody>
</table>

### Rôle

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Rôle</td>
            <td>Fonction</td>
            <td>RÔLE</td>
            <td>Fonction</td>
            <td>ROLES_CURRENT<br>ROLES_DAILY_HISTORY<br>ROLES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LAYOUTTEMPLATEID</td>
             <td>-</td>
             <td colspan="2">Le tableau Modèle de mise en page ne sera pas pris en charge</td>
        </tr>
        <tr>
             <td>PRIVATERATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>UITEMPLATEID</td>
             <td>FK</td>
             <td>UITEMPLATES_CURRENT</td>
             <td>UITEMPLATEID</td>
        </tr>
    </tbody>
</table>

### Planning

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Planning</td>
            <td>Planning</td>
            <td>PLANIFIÉ</td>
            <td>Planning</td>
            <td>SCHEDULES_CURRENT<br>SCHEDULES_DAILY_HISTORY<br>SCHEDULES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>HOMEGROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>SCHEDULEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
    </tbody>
</table>

### Plan de recrutement

Disponibilité limitée des clients

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Plan de recrutement</td>
            <td>Plan de recrutement</td>
            <td>PERSONNEL</td>
            <td>Plan de recrutement</td>
            <td>STAFFING_PLAN_CURRENT<br>STAFFING_PLAN_DAILY_HISTORY<br>STAFFING_PLAN_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ATTACHEDRATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT </td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>COMPANYID</td>
             <td>FK</td>
             <td>COMPANIES_CURRENT</td>
             <td>COMPANYID</td>
        </tr>        
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>        
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>        
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>       
         <tr>
             <td>PRIVATERATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID
</td>
        </tr>        
        <tr>
             <td>SCHEDULEID</td>
             <td>FK</td>
             <td>SCHEDULES_CURRENT</td>
             <td>SCHEDULEID
</td>
        </tr>        
        <tr>
             <td>STAFFINGPLANID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### Ressource du plan de recrutement

Disponibilité limitée des clients

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Ressource du plan de recrutement</td>
            <td>Ressource du plan de recrutement</td>
            <td>PERSONNEL</td>
            <td>Ressource du plan de recrutement</td>
            <td>STAFFING_PLAN_RESOURCE_CURRENT<br>STAFFING_PLAN_RESOURCE_DAILY_HISTORY<br>STAFFING_PLAN_RESOURCE_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ASSIGNEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>ASSIGNEDTOID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>        
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>        
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>        
        <tr>
             <td>STAFFINGPLANID</td>
             <td>FK</td>
             <td>STAFFING_PLAN_CURRENT</td>
             <td>STAFFINGPLANID</td>
        </tr>       
         <tr>
             <td>STAFFINGPLANRESOURCEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>        
    </tbody>
</table>

### Personne approbatrice d’étape

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Personne approbatrice d’étape</td>
            <td>Personne approbatrice d’étape</td>
            <td>SPAPVR</td>
            <td>Approbateur d'étape</td>
            <td>STEPAPPROVERS_CURRENT<br>STEPAPPROVERS_DAILY_HISTORY<br>STEPAPPROVERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPROVALSTEPID</td>
             <td>FK</td>
             <td>APPROVALSTEPS_CURRENT</td>
             <td>APPROVALSTEPID</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>STEPAPPROVERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>TEAMID</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>TEAMID</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Tâche

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Tâche</td>
            <td>Tâche</td>
            <td>TASK</td>
            <td>Tâche</td>
            <td>TASKS_CURRENT<br>TASKS_DAILY_HISTORY<br>TASKS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPROVALPROCESSID</td>
             <td>FK</td>
             <td>APPROVALPROCESSES_CURRENT</td>
             <td>APPROVALPROCESSID</td>
        </tr>
        <tr>
             <td>ASSIGNEDTOID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>BILLINGRECORDID</td>
             <td>FK</td>
             <td>BILLINGRECORDS_CURRENT</td>
             <td>BILLINGRECORDID</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>CONVERTEDOPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>CONVERTEDOPTASKORIGINATORID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>CURRENTAPPROVALSTEPID</td>
             <td>FK</td>
             <td>APPROVALSTEPS_CURRENT</td>
             <td>APPROVALSTEPID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>ITÉRATIONID</td>
             <td>FK</td>
             <td>ITÉRATIONS_CURRENT</td>
             <td>ITÉRATIONID</td>
        </tr>
        <tr>
             <td>KANBANBOARDID</td>
             <td>-</td>
             <td colspan="2">La table de tableau kanban n’est actuellement pas prise en charge</td>
        </tr>
        <tr>
             <td>LASTCONDITIONNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>MILESTONEID</td>
             <td>FK</td>
             <td>MILESTONES_CURRENT</td>
             <td>MILESTONEID</td>
        </tr>
        <tr>
             <td>PARENTID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>RECURRENCERULEID</td>
             <td>-</td>
             <td colspan="2">Le tableau des règles de récurrence n'est pas pris en charge actuellement</td>
        </tr>
        <tr>
             <td>REJECTIONISSUEID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>RESERVEDTIMEID</td>
             <td>FK</td>
             <td>RESERVEDTIMES_CURRENT</td>
             <td>RESERVEDTIMEID</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SUBMITTEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>SUBMITTEDBYID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>TEAMID</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>TEAMID</td>
        </tr>
        <tr>
             <td>TEMPLATETASKID</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATETASKID</td>
        </tr>
    </tbody>
</table>

### Tâche antérieure

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Tâche antérieure</td>
            <td>Tâche antérieure</td>
            <td>PRED</td>
            <td>Tâche antérieure</td>
            <td>PREDECESSORS_CURRENT<br>PREDECESSORS_DAILY_HISTORY<br>PREDECESSORS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>PREDECESSORID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>SUCCESSORID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
    </tbody>
</table>

### Equipe

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Equipe</td>
            <td>Equipe</td>
            <td>TEAMOB</td>
            <td>Equipe</td>
            <td>TEAMS_CURRENT<br>TEAMS_DAILY_HISTORY<br>TEAMS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LAYOUTTEMPLATEID</td>
             <td>-</td>
             <td colspan="2">Le tableau Modèle de mise en page ne sera pas pris en charge</td>
        </tr>
        <tr>
             <td>MYWORKVIEWID</td>
             <td>FK</td>
             <td>UIVIEWS_CURRENT</td>
             <td>UIVIEWID</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>REQUESTSVIEWID</td>
             <td>FK</td>
             <td>UIVIEWS_CURRENT</td>
             <td>UIVIEWID</td>
        </tr>
        <tr>
             <td>SCHEDULEID</td>
             <td>FK</td>
             <td>SCHEDULES_CURRENT</td>
             <td>SCHEDULEID</td>
        </tr>
        <tr>
             <td>TEAMID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>UITEMPLATEID</td>
             <td>FK</td>
             <td>UITEMPLATES_CURRENT</td>
             <td>UITEMPLATEID</td>
        </tr>
    </tbody>
</table>

>[!NOTE]
>
>Trois types d&#39;équipe sont stockés dans les tables d&#39;objets d&#39;équipe : PROJECT, TEMPLATE et ADHOC. <br>
>Chacun de ces types d’équipes est représenté ensemble dans les vues du lac de données Data Connect. Pour isoler le type spécifique d&#39;équipe que vous souhaitez renvoyer, vous devez appliquer un filtre sur la colonne `teamtype`. Par exemple, si vous souhaitez uniquement les équipes traditionnelles qui font partie de vos structures organisationnelles, configurées dans la zone Équipes de l’application, vous pouvez avoir une requête qui ressemble à ceci : <code>select * from team_current where teamtype = &#39;ADHOC&#39;;</code>

### Membre d&#39;équipe

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Membre d'équipe</td>
            <td>Autres équipes, membre d'équipe</td>
            <td>TEAMMB</td>
            <td>Membre d'équipe</td>
            <td>TEAMMEMBERS_CURRENT<br>TEAMMEMBERS_DAILY_HISTORY<br>TEAMMEMBERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>TEAMID</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>TEAMID</td>
        </tr>
        <tr>
             <td>TEAMMEMBERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Rôle de membre d&#39;équipe

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Rôle de membre d'équipe</td>
            <td>Rôle de membre d'équipe</td>
            <td>TEAMMR</td>
            <td>Rôle de membre d'équipe</td>
            <td>TEAMMEMBERROLES_CURRENT<br>TEAMMEMBERROLES_DAILY_HISTORY<br>TEAMMEMBERROLES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>TEAMID</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>TEAMID</td>
        </tr>
        <tr>
             <td>TEAMMEMBERROLEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Modèle

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Modèle</td>
            <td>Modèle, Modèle de projet</td>
            <td>TMPL</td>
            <td>Modèle</td>
            <td>TEMPLATES_CURRENT<br>TEMPLATES_DAILY_HISTORY<br>TEMPLATES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPROVALPROCESSID</td>
             <td>FK</td>
             <td>APPROVALPROCESSES_CURRENT</td>
             <td>APPROVALPROCESSID</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>COMPANYID</td>
             <td>FK</td>
             <td>COMPANIES_CURRENT</td>
             <td>COMPANYID</td>
        </tr>
        <tr>
             <td>DELIVERABLESCORECARDID</td>
             <td>-</td>
             <td colspan="2">Le tableau Carte de résultats livrable n'est pas pris en charge actuellement</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>MILESTONEPATID</td>
             <td>FK</td>
             <td>MILESTONEPATHS_CURRENT</td>
             <td>MILESTONEPATID</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PRIVATERATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>PROGRAMID</td>
             <td>FK</td>
             <td>PROGRAMMES_ACTUELS</td>
             <td>PROGRAMID</td>
        </tr>
        <tr>
             <td>QUEUEDEFID</td>
             <td>-</td>
             <td colspan="2">Le tableau de définition de file d'attente n'est pas pris en charge actuellement</td>
        </tr>
        <tr>
             <td>SCHEDULEID</td>
             <td>FK</td>
             <td>SCHEDULES_CURRENT</td>
             <td>SCHEDULEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>TEAMID</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>TEAMID</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### Modèle d&#39;affectation de tâche

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Modèle d'affectation de tâche</td>
            <td>Modèle d'affectation</td>
            <td>AFFECTATION</td>
            <td>Modèle d'affectation</td>
            <td>TEMPLATEASSIGNMENTS_CURRENT<br>TEMPLATEASSIGNMENTS_DAILY_HISTORY<br>TEMPLATEASSIGNMENTS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ASSIGNEDTOID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variable, basée sur OBJCODE</td>
             <td>Clé primaire/ID de l’objet identifié dans le champ OBJCODE</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>TEAMID</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>TEAMID</td>
        </tr>
        <tr>
             <td>TEAMTIMELINEABLEID</td>
             <td>-</td>
             <td colspan="2">Tableau de chronologie d'équipe non pris en charge actuellement</td>
        </tr>
        <tr>
             <td>TEMPLATEASSIGNMENTID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>TEMPLATETASKID</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATETASKID</td>
        </tr>
    </tbody>
</table>

### Tâche de modèle

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Tâche de modèle</td>
            <td>Tâche de modèle</td>
            <td>TTSK</td>
            <td>Tâche de modèle</td>
            <td>TEMPLATETASKS_CURRENT<br>TEMPLATETASKS_DAILY_HISTORY<br>TEMPLATETASKS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPROVALPROCESSID</td>
             <td>FK</td>
             <td>APPROVALPROCESSES_CURRENT</td>
             <td>APPROVALPROCESSID</td>
        </tr>
        <tr>
             <td>ASSIGNEDTOID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>LASTNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>MILESTONEID</td>
             <td>FK</td>
             <td>MILESTONES_CURRENT</td>
             <td>MILESTONEID</td>
        </tr>
        <tr>
             <td>PARENTID</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATETASKID</td>
        </tr>
        <tr>
             <td>RECURRENCERULEID</td>
             <td>-</td>
             <td colspan="2">Le tableau des règles de récurrence n'est pas pris en charge actuellement</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>TEAMID</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>TEAMID</td>
        </tr>
        <tr>
             <td>TEAMTIMELINEABLEID</td>
             <td>-</td>
             <td colspan="2">Tableau de chronologie d'équipe non pris en charge actuellement</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
        <tr>
             <td>TEMPLATETASKID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### Tâche de modèle antérieure

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Tâche de modèle antérieure</td>
            <td>Prédécesseur du modèle</td>
            <td>TPRED</td>
            <td>Tâche antérieure</td>
            <td>TEMPLATEPREDECESSORS_CURRENT<br>TEMPLATEPREDECESSORS_DAILY_HISTORY<br>TEMPLATEPREDECESSORS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>PREDECESSORID</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATETASKID</td>
        </tr>
        <tr>
             <td>SUCCESSORID</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATETASKID</td>
        </tr>
        <tr>
             <td>TEMPLATEPREDECESSORID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
    </tbody>
</table>

### KPI par étapes combinés

Disponibilité limitée des clients

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>KPI par étapes combinés</td>
            <td>KPI chronologique</td>
            <td>TMPH</td>
            <td>TimePhasedKPI</td>
            <td>TIMEPHASED_COMBINED_CURRENT<br>TIMEPHASED_COMBINED_DAILY_HISTORY<br>TIMEPHASED_COMBINED_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ASSIGNMENTID</td>
             <td>FK</td>
             <td>ASSIGNMENTS_CURRENT</td>
             <td>ASSIGNMENTID</td>
        </tr>
                <tr>
             <td>EVENT_ID    </td>
             <td>PK</td>
             <td>Il s’agit d’une clé naturelle pour l’entrée d’indicateur de performance clé temporel</td>
             <td>-</td>
        </tr>
                        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
                        <tr>
             <td>LOCATIONID</td>
             <td>FK</td>
             <td>CLASSIFIER_CURRENT</td>
             <td>CLASSIFIERID</td>
        </tr>
                        <tr>
             <td>METADATAID</td>
             <td>FK</td>
             <td>Le tableau METADATA n’est pas fourni</td>
             <td>-</td>
        </tr>
                        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
                        <tr>
             <td>PORTFOLIOID</td>
             <td>FK</td>
             <td>PORTFOLIOS_CURRENT</td>
             <td>PORTFOLIOID</td>
        </tr>
                        <tr>
             <td>PROGRAMID</td>
             <td>FK</td>
             <td>PROGRAMMES_ACTUELS</td>
             <td>PROGRAMID</td>
        </tr>
                        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
                        <tr>
             <td>REFERENCEID</td>
             <td>FK</td>
             <td>Variable, basée sur OBJCODE</td>
             <td>Clé primaire/ID de l’objet identifié dans le champ OBJCODE
</td>
        </tr>
                        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
                        <tr>
             <td>SCHEMAID</td>
             <td>FK</td>
             <td>Le tableau SCHEMA n’est pas fourni ; la valeur de ce tableau est fournie dans la colonne SCHEMANAME . Le SCHEMANAME identifie l'indicateur de performance clé (par exemple, les heures prévues, les heures estimées et les heures réelles) auquel l'enregistrement est connecté.</td>
             <td>-</td>
        </tr>
                                <tr>
             <td>SOURCETASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
                                <tr>
             <td>STAFFINGPLANID</td>
             <td>FK</td>
             <td>STAFFING_PLAN_CURRENT</td>
             <td>STAFFINGPLANID</td>
        </tr>
                                <tr>
             <td>STAFFINGPLANRESOURCEID</td>
             <td>FK</td>
             <td>STAFFING_PLAN_RESOURCE_CURRENT</td>
             <td>STAFFINGPLANRESOURCEID</td>
        </tr>
                                <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
                                <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Devise des indicateurs de performance clés temporels

Disponibilité limitée des clients

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Devise des indicateurs de performance clés temporels</td>
            <td>KPI chronologique</td>
            <td>TMPH</td>
            <td>TimePhasedKPI</td>
            <td>TIMEPHASED_CURRENCY_CURRENT<br>TIMEPHASED_CURRENCY_DAILY_HISTORY<br>TIMEPHASED_CURRENCY_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ASSIGNMENTID</td>
             <td>FK</td>
             <td>ASSIGNMENTS_CURRENT</td>
             <td>ASSIGNMENTID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LOCATIONID</td>
             <td>FK</td>
             <td>CLASSIFIER_CURRENT</td>
             <td>CLASSIFIERID</td>
        </tr>
                <tr>
             <td>METADATAID</td>
             <td>FK</td>
             <td>Le tableau METADATA n’est pas fourni</td>
             <td>-</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>PORTFOLIOID</td>
             <td>FK</td>
             <td>PORTFOLIOS_CURRENT</td>
             <td>PORTFOLIOID</td>
        </tr>
        <tr>
             <td>PROGRAMID</td>
             <td>FK</td>
             <td>PROGRAMMES_ACTUELS</td>
             <td>PROGRAMID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>REFERENCEID</td>
             <td>FK</td>
             <td>Variable, basée sur OBJCODE</td>
             <td>Clé primaire/ID de l’objet identifié dans le champ OBJCODE</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SCHEMAID</td>
             <td>FK</td>
             <td>Le tableau SCHEMA n’est pas fourni ; la valeur de ce tableau est fournie dans la colonne SCHEMANAME . Le SCHEMANAME identifie l'indicateur de performance clé (par exemple, scheduledRevenueRate, scheduledCostRate, realRevenue, etc.) auquel l'enregistrement est connecté.</td>
             <td>SCHEMAID</td>
        </tr>
        <tr>
             <td>SOURCETASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
                <tr>
             <td>STAFFINGPLANID</td>
             <td>FK</td>
             <td>STAFFING_PLAN_CURRENT</td>
             <td>STAFFINGPLANID</td>
        </tr>
          <tr>
             <td>STAFFINGPLANRESOURCEID</td>
             <td>FK</td>
             <td>STAFFING_PLAN_RESOURCE_CURRENT</td>
             <td>STAFFINGPLANRESOURCEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>TIMEPHASEDCURRENCYID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Durée des KPI par étapes

Disponibilité limitée des clients

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Durée des KPI par étapes</td>
            <td>KPI chronologique</td>
            <td>TMPH</td>
            <td>TimePhasedKPI</td>
            <td>TIMEPHASED_DURATION_CURRENT<br>TIMEPHASED_DURATION_DAILY_HISTORY<br>TIMEPHASED_DURATION_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ASSIGNMENTID</td>
             <td>FK</td>
             <td>ASSIGNMENTS_CURRENT</td>
             <td>ASSIGNMENTID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LOCATIONID</td>
             <td>FK</td>
             <td>CLASSIFIER_CURRENT</td>
             <td>CLASSIFIERID</td>
        </tr>
                <tr>
             <td>METADATAID</td>
             <td>FK</td>
             <td>Le tableau METADATA n’est pas fourni</td>
             <td>-</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>PORTFOLIOID</td>
             <td>FK</td>
             <td>PORTFOLIOS_CURRENT</td>
             <td>PORTFOLIOID</td>
        </tr>
        <tr>
             <td>PROGRAMID</td>
             <td>FK</td>
             <td>PROGRAMMES_ACTUELS</td>
             <td>PROGRAMID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>REFERENCEID</td>
             <td>FK</td>
             <td>Variable, basée sur OBJCODE</td>
             <td>Clé primaire/ID de l’objet identifié dans le champ OBJCODE</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SCHEMAID</td>
             <td>FK</td>
             <td>Le tableau SCHEMA n’est pas fourni ; la valeur de ce tableau est fournie dans la colonne SCHEMANAME . Le SCHEMANAME identifie l'indicateur de performance clé (par exemple, les heures prévues, les heures estimées et les heures réelles) auquel l'enregistrement est connecté.</td>
             <td>SCHEMAID</td>
        </tr>
        <tr>
             <td>SOURCETASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
                <tr>
             <td>STAFFINGPLANID </td>
             <td>FK</td>
             <td>STAFFING_PLAN_CURRENT</td>
             <td>STAFFINGPLANID</td>
        </tr>
           <tr>
             <td>STAFFINGPLANRESOURCEID</td>
             <td>FK</td>
             <td>STAFFING_PLAN_RESOURCE_CURRENT</td>
             <td>STAFFINGPLANRESOURCEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>TIMEPHASEDDURATIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Numéros d’indicateurs de performance clés temporels

Disponibilité limitée des clients

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Numéros d’indicateurs de performance clés temporels</td>
            <td>KPI chronologique</td>
            <td>TMPH</td>
            <td>TimePhasedKPI</td>
            <td>TIMEPHASED_NUMBERS_CURRENT<br>TIMEPHASED_NUMBERS_DAILY_HISTORY<br>TIMEPHASED_NUMBERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ASSIGNMENTID</td>
             <td>FK</td>
             <td>ASSIGNMENTS_CURRENT</td>
             <td>ASSIGNMENTID</td>
        </tr>
        <tr>
             <td>EVENT_ID</td>
             <td>PK</td>
             <td>Il s’agit d’une clé naturelle pour l’entrée d’indicateur de performance clé temporel</td>
             <td>-</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LOCATIONID</td>
             <td>FK</td>
             <td>CLASSIFIER_CURRENT</td>
             <td>CLASSIFIERID</td>
        </tr>
        <tr>
             <td>METADATAID</td>
             <td>FK</td>
             <td>Le tableau METADATA n’est pas fourni</td>
             <td>-</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>PORTFOLIOID</td>
             <td>FK</td>
             <td>PORTFOLIOS_CURRENT</td>
             <td>PORTFOLIOID</td>
        </tr>
                <tr>
             <td>PROGRAMID</td>
             <td>FK</td>
             <td>PROGRAMMES_ACTUELS</td>
             <td>PROGRAMID</td>
        </tr>
                <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
                <tr>
             <td>REFERENCEID</td>
             <td>FK</td>
             <td>Variable, basée sur OBJCODE</td>
             <td>Clé primaire/ID de l’objet identifié dans le champ OBJCODE</td>
        </tr>
                <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
                <tr>
             <td>SCHEMAID</td>
             <td>FK</td>
             <td>Le tableau SCHEMA n’est pas fourni ; la valeur de ce tableau est fournie dans la colonne SCHEMANAME . Le SCHEMANAME identifie l'indicateur de performance clé (par exemple, les heures prévues, les heures estimées et les heures réelles) auquel l'enregistrement est connecté.</td>
             <td>-</td>
        </tr>
                <tr>
             <td>SOURCETASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
                <tr>
             <td>STAFFINGPLANID</td>
             <td>FK</td>
             <td>STAFFING_PLAN_CURRENT</td>
             <td>STAFFINGPLANID</td>
        </tr>
                <tr>
             <td>STAFFINGPLANRESOURCEID</td>
             <td>FK</td>
             <td>STAFFING_PLAN_RESOURCE_CURRENT</td>
             <td>STAFFINGPLANRESOURCEID</td>
        </tr>
                <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
                <tr>
             <td>TIMEPHASEDNUMBERSID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
                <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Feuille de temps

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Feuille de temps</td>
            <td>Feuille de temps</td>
            <td>TSHET</td>
            <td>Feuille de temps</td>
            <td>TIMESHEETS_CURRENT<br>TIMESHEETS_DAILY_HISTORY<br>TIMESHEETS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPROVERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>TIMESHEETID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>TIMESHEETPROFILEID</td>
             <td>FK</td>
             <td>TIMESHEETPROFILES_CURRENT</td>
             <td>TIMESHEETPROFILEID</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Profil de feuille de temps

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Profil de feuille de temps</td>
            <td>Profil de feuille de temps</td>
            <td>TSPRO</td>
            <td>Profil de feuille de temps</td>
            <td>TIMESHEETPROFILES_CURRENT<br>TIMESHEETPROFILES_DAILY_HISTORY<br>TIMESHEETPROFILES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPROVERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>TIMESHEETPROFILEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### Filtre d’interface utilisateur

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Filtre d’interface utilisateur</td>
            <td>Filtre</td>
            <td>SOULEVER</td>
            <td>Filtre</td>
            <td>UIFILTERS_CURRENT<br>UIFILTERS_DAILY_HISTORY<br>UIFILTERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPGLOBALID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variable, basée sur OBJCODE</td>
             <td>Clé primaire/ID de l’objet identifié dans le champ OBJCODE</td>
        </tr>
        <tr>
             <td>PREFERENCEID</td>
             <td>FK</td>
             <td>PREFERENCES_CURRENT</td>
             <td>PREFERENCEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>UIFILTERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### Regrouper les interfaces utilisateur par

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Regrouper les interfaces utilisateur par</td>
            <td>Regroupement </td>
            <td>UIGB</td>
            <td>Regroupement </td>
            <td>UIGROUPBYS_CURRENT<br>UIGROUPBYS_DAILY_HISTORY<br>UIGROUPBYS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPGLOBALID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variable, basée sur OBJCODE</td>
             <td>Clé primaire/ID de l’objet identifié dans le champ OBJCODE</td>
        </tr>
        <tr>
             <td>PREFERENCEID</td>
             <td>FK</td>
             <td>PREFERENCES_CURRENT</td>
             <td>PREFERENCEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>UIGROUPBYID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### Modèle d’interface utilisateur

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Modèle d’interface utilisateur</td>
            <td>Modèle de mise en page</td>
            <td>UITMPL</td>
            <td>Modèle de mise en page</td>
            <td>UITEMPLATES_CURRENT<br>UITEMPLATES_DAILY_HISTORY<br>UITEMPLATES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>UITEMPLATEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### Vue UI

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Vue UI</td>
            <td>Afficher</td>
            <td>UIVIEW</td>
            <td>Afficher</td>
            <td>UIVIEWS_CURRENT<br>UIVIEWS_DAILY_HISTORY<br>UIVIEWS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPGLOBALID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variable, basée sur OBJCODE</td>
             <td>Clé primaire/ID de l’objet identifié dans le champ OBJCODE</td>
        </tr>
        <tr>
             <td>PREFERENCEID</td>
             <td>FK</td>
             <td>PREFERENCES_CURRENT</td>
             <td>PREFERENCEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>UIVIEWID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### l’utilisateur ou de l’utilisatrice

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>l’utilisateur ou de l’utilisatrice</td>
            <td>l’utilisateur ou de l’utilisatrice</td>
            <td>USER</td>
            <td>l’utilisateur ou de l’utilisatrice</td>
            <td>USERS_CURRENT<br>USERS_DAILY_HISTORY<br>USERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ACCESSLEVELID</td>
             <td>FK</td>
             <td>ACCESSLEVELS_CURRENT</td>
             <td>ACCESSLEVELID</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>COMPANYID</td>
             <td>FK</td>
             <td>COMPANIES_CURRENT</td>
             <td>COMPANYID</td>
        </tr>
        <tr>
             <td>DEFAULTHOURTYPEID</td>
             <td>FK</td>
             <td>HOURTYPES_CURRENT</td>
             <td>HOURTYPEID</td>
        </tr>
        <tr>
             <td>DELEGATIONTOID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>EAUTHUSERID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>HOMEGROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>HOMETEAMID</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>TEAMID</td>
        </tr>
        <tr>
             <td>LASTENTEREDNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LATESTUPDATENOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LAYOUTTEMPLATEID</td>
             <td>-</td>
             <td colspan="2">Le tableau Modèle de mise en page ne sera pas pris en charge</td>
        </tr>
        <tr>
             <td>MANAGERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PORTALPROFILEID</td>
             <td>-</td>
             <td colspan="2">La table Profil de portail ne sera pas prise en charge</td>
        </tr>
        <tr>
             <td>PRÉFLUIDE</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>PRIVATERATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>RESOURCEPOOLID</td>
             <td>FK</td>
             <td>RESOURCEPOOLS_CURRENT</td>
             <td>RESOURCEPOOLID</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SCHEDULEID</td>
             <td>FK</td>
             <td>SCHEDULES_CURRENT</td>
             <td>SCHEDULEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>TIMESHEETPROFILEID</td>
             <td>FK</td>
             <td>TIMESHEETPROFILES_CURRENT</td>
             <td>TIMESHEETPROFILEID</td>
        </tr>
        <tr>
             <td>UITEMPLATEID</td>
             <td>FK</td>
             <td>UITEMPLATES_CURRENT</td>
             <td>UITEMPLATEID</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>UUMUSERID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
    </tbody>
</table>

### Délégation d&#39;utilisateur

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Délégation d'utilisateur</td>
            <td>Délégation d'utilisateur</td>
            <td>USERDEL</td>
            <td>Délégation d'utilisateur</td>
            <td>USERDELEGATIONS_CURRENT<br>USERDELEGATIONS_DAILY_HISTORY<br>USERDELEGATIONS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>FROMUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>TOUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>USERDELEGATIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### Groupe d&#39;utilisateurs

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Groupe d'utilisateurs</td>
            <td>Autres groupes</td>
            <td>USRGPS</td>
            <td>Groupe d'utilisateurs</td>
            <td>USERSGROUPS_CURRENT<br>USERSGROUPS_DAILY_HISTORY<br>USERSGROUPS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>USERSGROUPID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### Emplacement de l’utilisateur

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Emplacement de l’utilisateur</td>
            <td>Emplacement de l’utilisateur</td>
            <td>USRLOC</td>
            <td>UserLocation</td>
            <td>USERLOCATIONS_CURRENT<br>USERLOCATIONS_DAILY_HISTORY<br>USERLOCATIONS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CLASSIFIERID</td>
             <td>FK</td>
             <td>CLASSIFIER_CURRENT</td>
             <td>CLASSIFIERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>USERLOCATIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### Rôle d’utilisateur

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Rôle d’utilisateur</td>
            <td>Autres rôles</td>
            <td>USROL</td>
            <td>Rôle d’utilisateur</td>
            <td>USERSROLES_CURRENT<br>USERSROLES_DAILY_HISTORY<br>USERSROLES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>USERROLESETID</td>
             <td>FK</td>
             <td>USERROLESET_CURRENT</td>
             <td>USERROLESETID</td>
        </tr>
        <tr>
             <td>USERLOCATIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### Valeur de préférence utilisateur

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Valeur de préférence utilisateur</td>
            <td>Préférence utilisateur</td>
            <td>USERPF</td>
            <td>Préférence utilisateur</td>
            <td>USERPREFVALUES_CURRENT<br>USERPREFVALUES_DAILY_HISTORY<br>USERPREFVALUES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>USERPREFVALUEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### User Role Set

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>UserRoleSet</td>
            <td>User Role Set</td>
            <td>URSET</td>
            <td>UserRoleSet</td>
            <td>USERROLESET_CURRENT<br>USERROLESET_DAILY_HISTORY<br>USERROLESET_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>PRIMARYROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>USERROLESETID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### Décisions des utilisateurs et utilisatrices

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>UsersDecisions</td>
            <td>Décisions des utilisateurs et utilisatrices</td>
            <td>USRDEC</td>
            <td>Décisions des utilisateurs et utilisatrices</td>
            <td>USERSDECISIONS_CURRENT<br>USERSDECISIONS_DAILY_HISTORY<br>USERSDECISIONS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>USERDECISIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Élément de travail

<table>
    <thead>
        <tr>
            <th>Nom de l’entité Workfront</th>
            <th>Références d’interface</th>
            <th>Référence d’API</th>
            <th>Libellé de l’API</th>
            <th>Vues du lac de données</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>WorkItem</td>
            <td>Élément de travail</td>
            <td>WRKITM</td>
            <td>WorkItem</td>
            <td>WORKITEMS_CURRENT<br>WORKITEMS_DAILY_HISTORY<br>WORKITEMS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Principal/Clé étrangère</th>
            <th>Type</th>
            <th>Table connexe</th>
            <th>Champ associé</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ASSIGNMENTID</td>
             <td>FK</td>
             <td>ASSIGNMENTS_CURRENT</td>
             <td>ASSIGNMENTID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variable, basée sur OBJCODE</td>
             <td>Clé primaire/ID de l’objet identifié dans le champ OBJCODE</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Pas une relation ; utilisé à des fins d’application interne.</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>WORKITEMID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>
