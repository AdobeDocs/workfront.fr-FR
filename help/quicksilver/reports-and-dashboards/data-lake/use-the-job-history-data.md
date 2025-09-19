---
product-area: reports and dashboards
navigation-topic: data-connect
title: Utiliser la vue Historique des tâches dans Data Connect
description: Avec Data Connect, les administrateurs et administratrices de Workfront peuvent accéder à des enregistrements détaillés de chaque tâche d’actualisation des données dans la vue Historique des tâches .
author: Jenny
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
source-git-commit: 05cf34fe6659c50da76d2478c6e79352346dc9a5
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 0%

---

# Utiliser la vue Historique des tâches dans Data Connect

Dans la vue Historique des tâches, les administrateurs et administratrices de Workfront peuvent accéder à des enregistrements détaillés de chaque tâche d’actualisation des données. Ces enregistrements fournissent de précieuses informations insight sur les tâches qui maintiennent vos données à jour et vous aident à établir des délais idéaux pour exécuter les processus et actualiser vos visualisations d’entreprise.

![Vue Historique des tâches](assets/job-history-overview.png)

Les colonnes de la vue Historique des tâches contiennent les informations suivantes :

* **OBJECT_NAME** : affiche le nom de l’objet associé à la tâche.
* **SCHEDULED_TIME** : affiche l’heure de début de la tâche.
* **COMPLETED_TIME** : affiche l’heure d’achèvement de la tâche.
* **LATEST_FLAG** : indique si la tâche faisait partie de l’actualisation la plus récente.
* **STATE** : affiche le statut de la tâche. Pour plus d’informations, reportez-vous à la section suivante de cet article : [statuts des tâches disponibles](#available-job-statuses).
* **LAST_UPDATED** : date et heure de la dernière mise à jour de la tâche.

>[!NOTE]
>
>La vue Historique des tâches comprend des détails sur les 72 heures précédentes de tâches planifiées.


## Statuts de tâche disponibles

Chaque tâche Data Connect se voit attribuer un statut qui indique si elle a réussi, si elle a été ignorée ou si elle a échoué.

<table>
    <tr>
        <td><b>Statut du traitement</b></td>
        <td><b>Définition</b></td>
    </tr>
    <tr>
        <td>Succès</td>
        <td>La tâche a traité avec succès chaque mise à jour disponible et toutes les mises à jour pour ce type d’enregistrement sont désormais répercutées dans le lac de données.</td>
    </tr>
    <tr>
        <td>Ignoré</td>
        <td>Le traitement a été ignoré car aucune mise à jour n’était en file d’attente pour être traitée pour le type d’enregistrement.</td>
    </tr>
    <tr>
        <td>Échec</td>
        <td>Échec de l’exécution du traitement. Dans ces cas, il est probable qu’aucune donnée de la file d’attente n’ait été validée dans le lac de données. Les enregistrements qui restent dans la file d'attente seront traités dans la prochaine tâche planifiée pour ce type d'enregistrement. </td>
    </tr>
   </table>


## Considérations relatives à l’exécution des tâches et au comportement de journalisation

Snowflake utilise un outil d’optimisation du planificateur de tâches qui peut affecter la manière dont l’exécution des tâches est traitée et consignée dans la vue Historique des tâches. Ce comportement de journalisation peut varier selon qu’il existe ou non des données à traiter.

Par exemple, lorsqu’il n’y a pas de nouvelles lignes à traiter pour un objet donné, l’un des résultats suivants peut se produire :

* **La tâche s’exécute et est marquée comme Ignorée** : Snowflake détecte qu’il n’y a aucune ligne à traiter, exécute la tâche et l’enregistre avec un statut Ignorée dans le tableau.

* **La tâche ne s’exécute pas** : Snowflake détermine qu’il n’y a aucune ligne à traiter, n’exécute pas la tâche et l’enregistre avec un statut Ignorée dans le tableau.

  >[!NOTE]
  >
  >Dans le deuxième scénario où la tâche ne s’exécute pas, l’enregistrement le plus récent de cet objet peut refléter un horodatage qui ne correspond pas au planning attendu.

En d’autres termes, une tâche peut être considérée comme exécutée même si aucune ligne n’a été traitée, et elle peut être consignée ou non, selon le comportement du planificateur de tâches pour cette tâche spécifique.