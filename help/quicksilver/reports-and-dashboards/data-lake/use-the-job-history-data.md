---
product-area: reports and dashboards
navigation-topic: data-connect
title: Utilisation de la vue Historique des tâches dans Data Connect
description: Avec Data Connect, les administrateurs Workfront peuvent accéder aux enregistrements détaillés de chaque travail d’actualisation des données dans la vue Historique des travaux.
author: Courtney
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: d658c3df-5fa5-4756-ac42-71d9aed481df
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 0%

---

# Utilisation de la vue Historique des tâches dans Data Connect

Dans la vue Historique des tâches, les administrateurs et administratrices de Workfront peuvent accéder à des enregistrements détaillés de chaque tâche d’actualisation des données. Ces enregistrements fournissent de précieuses informations insight sur les tâches qui maintiennent vos données à jour et vous aident à établir des délais idéaux pour exécuter les processus et actualiser vos visualisations d’entreprise.

![Vue Historique des tâches](assets/job-history-overview.png)

Les colonnes de la vue Historique des tâches contiennent les informations suivantes :

* **OBJECT_NAME** : affiche le nom de l&#39;objet associé à la tâche.
* **SCHEDULED_TIME** : affiche l&#39;heure de début de la tâche.
* **COMPLETED_TIME** : affiche l&#39;heure d&#39;achèvement du travail.
* **LATEST_FLAG** : indique si la tâche faisait partie de la dernière actualisation.
* **ÉTAT** : affiche l&#39;état de la tâche. Pour plus d&#39;informations, consultez la section suivante de cet article : [Statuts des tâches disponibles](#available-job-statuses).
* **LAST_UPDATED** : horodatage de la dernière mise à jour de la tâche.

>[!NOTE]
>
>La vue Historique des tâches comprend les détails des 72 heures précédentes de tâches planifiées.


## Statuts de tâche disponibles

Chaque tâche Data Connect se voit attribuer un statut qui indique si elle a réussi, si elle a été ignorée ou si elle a échoué.

<table>
    <tr>
        <td><b>Statut du traitement</b></td>
        <td><b>Définition</b></td>
    </tr>
    <tr>
        <td>Réussite</td>
        <td>Le travail a traité avec succès chaque mise à jour disponible, et toutes les mises à jour pour ce type d'enregistrement sont maintenant reflétées dans le lac de données.</td>
    </tr>
    <tr>
        <td>Ignoré</td>
        <td>La tâche a été ignorée, car aucune mise à jour n'était en file d'attente pour être traitée pour le type d'enregistrement.</td>
    </tr>
    <tr>
        <td>Échec</td>
        <td>Échec de l'exécution de la tâche. Dans ces cas, il est probable qu’aucune donnée en file d’attente n’ait été validée dans le lac de données. Les enregistrements qui restent dans la file d'attente seront traités dans la prochaine tâche planifiée pour ce type d'enregistrement. </td>
    </tr>
   </table>


## Considérations relatives à l’exécution des tâches et au comportement de journalisation

Snowflake utilise un outil d’optimisation du planificateur de tâches qui peut affecter la manière dont l’exécution des tâches est traitée et consignée dans la vue Historique des tâches. Ce comportement d&#39;enregistrement peut varier selon qu&#39;il existe ou non des données à traiter.

Par exemple, lorsqu&#39;il n&#39;y a pas de nouvelles lignes à traiter pour un objet donné, l&#39;un des résultats suivants peut se produire :

* **La tâche s&#39;exécute et est marquée comme Ignorée** : Snowflake détecte qu&#39;il n&#39;y a aucune ligne à traiter, exécute la tâche et l&#39;enregistre avec un état Ignorée dans la table.

* **Le travail ne s&#39;exécute pas** : le Snowflake détermine qu&#39;il n&#39;y a aucune ligne à traiter, n&#39;exécute pas le travail et l&#39;enregistre avec un état Ignoré dans la table.

  >[!NOTE]
  >
  >Dans le deuxième scénario, où la tâche ne s’exécute pas, l’enregistrement le plus récent de cet objet peut refléter un horodatage qui ne correspond pas à la planification attendue.

En d&#39;autres termes, un travail peut être considéré comme exécuté même si aucune ligne n&#39;a été traitée, et il peut être enregistré ou non en fonction du comportement du planificateur de travaux pour ce travail particulier.
