---
content-type: reference
product-area: reports and dashboards
navigation-topic: data lake
title: Dictionnaire de données du lac de données
description: Cette page contient des informations sur la structure et le contenu des données du lac de données Workfront.
author: Nolan
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: 57985404-554e-4289-b871-b02d3427aa5c
source-git-commit: 81f8477dd26b828c4255c678b36d98789cd81ff8
workflow-type: tm+mt
source-wordcount: '725'
ht-degree: 5%

---

# Dictionnaire de données de lac de données Workfront

Cette page contient des informations sur la structure et le contenu des données du lac de données Workfront.

>[!NOTE]
>
>Les données du lac de données Workfront sont actualisées toutes les quatre heures, de sorte que les modifications récentes peuvent ne pas être immédiatement répercutées.

## Types de tableau

Il existe plusieurs types de tableau que vous pouvez utiliser pour afficher vos données Workfront de manière à en tirer le meilleur parti.

* **Tableau actuel**

  Le tableau actuel reflète les données de la même manière qu’il existe dans Workfront, chaque objet et son état actuel. Il est toutefois possible de naviguer avec une latence beaucoup plus faible que dans Workfront.

* **Table d&#39;événements**

  Le tableau Événement effectue le suivi de chaque enregistrement de modification dans Workfront : c’est-à-dire, chaque fois qu’un objet change d’état, un enregistrement est créé qui indique le moment où la modification a eu lieu, qui a apporté la modification et ce qui a été modifié. Par conséquent, ce tableau est utile pour les comparaisons de temps en temps. Ce tableau ne contient que les données des trois dernières années.

* **Table d&#39;historique quotidien**

  Le tableau Historique quotidien offre une version abrégée du tableau Événement, dans la mesure où il indique l’état de chaque objet sur une base quotidienne plutôt que lors de chaque événement. Ce tableau est donc utile pour l’analyse des tendances.

<!-- Custom table -->

## Diagramme de relation d’entité

Les objets de Workfront (et, par conséquent, de votre lac de données) sont définis non seulement par leurs valeurs individuelles, mais aussi par leurs relations avec d’autres objets. Le diagramme des relations d’entité ci-dessous fournit un mappage de haut niveau des relations d’objet dans le lac de données Workfront. Le diagramme peut être visualisé et téléchargé à l’aide du lien suivant :

[Diagramme de relation d’entité de lac de données Workfront](/help/quicksilver/reports-and-dashboards/data-lake/assets/Workfront-data-lake_entity-relationship-diagram.pdf)

>[!IMPORTANT]
>
>Le diagramme des relations d’entité est un travail en cours : il est donc destiné uniquement à des fins de référence et peut faire l’objet de modifications.

## Types de date

Un certain nombre d’objets date fournissent des informations sur le moment où des événements spécifiques se produisent.

* `DL_LOAD_TIMESTAMP`: cette date est utilisée à des fins de référence interne et reflète le moment où les données ont été chargées dans la table Actuel, Événement ou Historique quotidien. Cette date ne doit pas être utilisée pour l’analyse des données et doit être supprimée pendant la phase bêta du lac de données Workfront.
* `CALENDAR_DATE`: cette date n’est présente que dans le tableau Historique quotidien . Ce tableau fournit un enregistrement de l’apparence des données à 11h59 UTC pour chaque date spécifiée dans `CALENDAR_DATE`.
* `BEGIN_EFFECTIVE_TIMESTAMP`: cette date est présente dans les tables Historique des événements et Historique quotidien, et enregistre exactement lorsqu’un enregistrement a été modifié. _to_ valeur de la ligne actuelle.
* `END_EFFECTIVE_TIMESTAMP`: cette date est présente dans les tables Historique des événements et Historique quotidien, et enregistre exactement lorsqu’un enregistrement a été modifié. _de_ valeur de la ligne actuelle par rapport à une valeur d’une autre ligne. Pour autoriser entre les requêtes sur `BEGIN_EFFECTIVE_TIMESTAMP` et `END_EFFECTIVE_TIMESTAMP` cette valeur n’est jamais nulle, même s’il n’y a pas de nouvelle valeur. Dans le cas où un enregistrement est toujours valide (c’est-à-dire que la valeur n’a pas changé), `END_EFFECTIVE_TIMESTAMP` a une valeur de 2300-01-01.

## Table de terminologie

Le tableau suivant établit la corrélation entre les noms d’objet dans Workfront (ainsi que leurs noms dans l’interface et l’API) et leurs noms équivalents dans le lac de données.

<table>
<thead>
  <tr>
    <th>Nom d’entité Workfront</th>
    <th>Références de l’interface</th>
    <th>Référence d’API | Libellé</th>
    <th>Tableaux de lac de données</th>
    <th>Notes</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Affectation</td>
    <td>Affectation</td>
    <td>ASSGN | Attribution</td>
    <td>ASSIGNMENTS_CURRENT<br>ASSIGNMENTS_DAILY_HISTORY<br>ASSIGNMENTS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>CustomEnum</td>
    <td>Condition, priorité, gravité, état</td>
    <td>CSTEM | Énumération personnalisée</td>
    <td>CUSTOMENUMS_CURRENT<br>CUSTOMENUMS_DAILY_HISTORY<br>CUSTOMENUMS_EVENT</td>
    <td>Le type d’enregistrement est identifié par la propriété `enumClass`. Voici les types attendus :<br>CONDITION_OPTASK<br>CONDITION_PROJ<br>CONDITION_TASK<br>PRIORITY_OPTASK<br>PRIORITY_PROJ<br>PRIORITY_TASK<br>SEVERITY_OPTASK<br>STATUS_OPTASK<br>STATUS_PROJ<br>STATUS_TASK</td>
  </tr>
  <tr>
    <td>Document</td>
    <td>Document</td>
    <td>DOCU | Document</td>
    <td>DOCUMENTS_CURRENT<br>DOCUMENTS_DAILY_HISTORY<br>DOCUMENTS_EVENT<br><br>DOCUMENTS_CUSTOM_VALUE_CURRENT<br>DOCUMENTS_CUSTOM_VALUE_DAILY_HISTORY<br>DOCUMENTS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>DocumentVersion</td>
    <td>Version du document</td>
    <td>DOCV | Document Version</td>
    <td>DOCUMENTVERSIONS_CURRENT<br>DOCUMENTVERSIONS_DAILY_HISTORY<br>DOCUMENTVERSIONS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Groupe</td>
    <td>Groupe</td>
    <td>GROUPE | Groupe</td>
    <td>GROUPS_CURRENT<br>GROUPS_DAILY_HISTORY<br>GROUPS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Heure</td>
    <td>Heure</td>
    <td>HEURE | Heure</td>
    <td>HOURS_CURRENT<br>HOURS_DAILY_HISTORY<br>HOURS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Type d’heure</td>
    <td>Type d’heure</td>
    <td>HOURT | Type d’heure</td>
    <td>HOURTYPES_CURRENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Jalon</td>
    <td>Jalon</td>
    <td>MILE | Milestone</td>
    <td>MILESTONES_CURRENT<br>MILESTONES_DAILY_HISTORY<br>MILESTONES_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>MilestonePath</td>
    <td>Chemin jalonné</td>
    <td>MPATH | Chemin Milestone</td>
    <td>MILESTONEPATHS_CURRENT<br>MILESTONEPATHS_DAILY_HISTORY<br>MILESTONEPATHS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Note</td>
    <td>Note</td>
    <td>REMARQUE | Remarque</td>
    <td>NOTES_CURRENT<br>NOTES_DAILY_HISTORY<br>NOTES_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>TâcheOp</td>
    <td>Problème, requête</td>
    <td>OPTASK | Problème</td>
    <td>OPTASKS_CURRENT<br>OPTASKS_DAILY_HISTORY<br>OPTASKS_EVENT<br><br>OPTASKS_CUSTOM_VALUE_CURRENT<br>OPTASKS_CUSTOM_VALUE_DAILY_HISTORY<br>OPTASKS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Portfolio</td>
    <td>Portfolio</td>
    <td>PORT | Portfolio</td>
    <td>PORTFOLIOS_CURRENT<br>PORTFOLIOS_DAILY_HISTORY<br>PORTFOLIOS_EVENT<br><br>PORTFOLIOS_CUSTOM_VALUE_CURRENT<br>PORTFOLIOS_CUSTOM_VALUE_DAILY_HISTORY<br>PORTFOLIOS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Programme</td>
    <td>Programme</td>
    <td>PRGM | Programme</td>
    <td>PROGRAMS_CURRENT<br>PROGRAMS_DAILY_HISTORY<br>PROGRAMS_EVENT<br><br>PROGRAMS_CUSTOM_VALUE_CURRENT<br>PROGRAMS_CUSTOM_VALUE_DAILY_HISTORY<br>PROGRAMS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Projet</td>
    <td>Projet</td>
    <td>PROJ | Projet</td>
    <td>PROJECTS_CURRENT<br>PROJECTS_DAILY_HISTORY<br>PROJECTS_EVENT<br><br>PROJECTS_CUSTOM_VALUE_CURRENT<br>PROJECTS_CUSTOM_VALUE_DAILY_HISTORY<br>PROJECTS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Rôle</td>
    <td>Fonction</td>
    <td>RÔLE | Rôle de tâche</td>
    <td>ROLES_CURRENT<br>ROLES_DAILY_HISTORY<br>ROLES_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Planning</td>
    <td>Planning</td>
    <td>SCHED | Planification</td>
    <td>SCHEDULES_CURRENT<br>SCHEDULES_DAILY_HISTORY<br>SCHEDULES_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Tâche</td>
    <td>Tâche</td>
    <td>TÂCHE | Tâche</td>
    <td>TASKS_CURRENT<br>TASKS_DAILY_HISTORY<br>TASKS_EVENT<br><br>TASKS_CUSTOM_VALUE_CURRENT<br>TASKS_CUSTOM_VALUE_DAILY_HISTORY<br>TASKS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Equipe</td>
    <td>Equipe</td>
    <td>TEAMOB | Équipe</td>
    <td>TEAMS_CURRENT<br>TEAMS_DAILY_HISTORY<br>TEAMS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Feuille de temps</td>
    <td>Feuille de temps</td>
    <td>TSHET | Feuille de calcul</td>
    <td>TIMESHEETS_CURRENT<br>TIMESHEETS_DAILY_HISTORY<br>TIMESHEETS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>l’utilisateur ou de l’utilisatrice</td>
    <td>l’utilisateur ou de l’utilisatrice</td>
    <td>UTILISATEUR | Utilisateur</td>
    <td>USERS_CURRENT<br>USERS_DAILY_HISTORY<br>USERS_EVENT<br><br>USERS_CUSTOM_VALUE_CURRENT<br>USERS_CUSTOM_VALUE_DAILY_HISTORY<br>USERS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
</tbody>
</table>
