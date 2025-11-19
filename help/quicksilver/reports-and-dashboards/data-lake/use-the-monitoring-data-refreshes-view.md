---
product-area: reports and dashboards
navigation-topic: data-connect
title: Utilisation de la vue Surveillance des actualisations des données dans Data Connect
description: Avec Data Connect, les administrateurs de Workfront peuvent accéder aux enregistrements détaillés des mises à jour récentes qui ont été apportées à la date du lac de données lors de la dernière actualisation.
author: Jenny
feature: Reports and Dashboards
source-git-commit: 1bcb64fbcdf2cb8b40cb50e5a7d4f5768f3a712f
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 2%

---

# Utilisation de la vue Surveillance des actualisations des données dans Data Connect

La vue Surveillance des actualisations des données affiche les mises à jour récentes apportées à la date du lac de données lors de la dernière actualisation. Les données de cette vue sont mises à jour après chaque fin réussie d’un chargement de données.

En raison du volume élevé de données et de la complexité des agrégations, la vue Surveillance de l’actualisation des données n’affiche que les vues d’objets qui ont été mises à jour au cours des 2 dernières semaines. Si un type d’enregistrement spécifique est absent de cette vue, cela est probablement dû à un manque d’activité au cours de cette période.

>[!NOTE]
>
>Cette vue affiche une collection détaillée des données fournies par l’application et les activités d’actualisation, par opposition à une vue d’historique quotidien ou d’événement qui affiche l’historique des activités d’actualisation. Pour obtenir les détails de l’activité d’actualisation historique, vous pouvez utiliser la variable <code>DL_LOAD_TIMESTAMP</code> objet date.

## Colonnes de la vue Surveillance de l’actualisation des données

Les colonnes de la vue Surveillance de l&#39;actualisation des données contiennent les informations suivantes :

<table>
    <tr>
        <td><b>Nom de la colonne</b></td>
        <td><b>Type</b></td>
        <td><b>Description</b></td>
    </tr>
    <tr>
        <td>OBJ_TYPE</td>
        <td>Varchar
        </td>
        <td> 
      Type d’objet associé aux enregistrements Workfront envoyés au lac de données. 
        </ul></td>
    </tr>
    <tr>
        <td>CALENDAR_DATE </td>
        <td>Date</td>
        <td>
   Date de la dernière actualisation réussie des données pour le type d'objet affiché dans la colonne OBJ_TYPE. </td>
    </tr>
        <tr>
        <td>RECORD_LOAD_TIMESTAMP </td>
        <td>Timestamp_NTZ</td>
        <td>
 Date et heure de la dernière actualisation des données pour le type d'objet affiché dans la colonne OBJ_TYPE.  </td>
    </tr>
        <tr>
        <td>PREVIOUS_RECORD_LOAD_TIMESTAMP </td>
        <td>Timestamp_NTZ </td>
        <td>
       Date et heure de la deuxième actualisation la plus récente des données pour le type d'objet affiché dans la colonne OBJ_TYPE. </td>
    </tr>
        <tr>
        <td>MINUTES_SINCE_PREVIOUS_LOAD </td>
        <td>Nombre</td>
        <td>
     Durée (en minutes) écoulée depuis la dernière actualisation des données pour le type d’objet. </td>
    </tr>
            <tr>
        <td>CRÉÉ </td>
        <td>Nombre </td>
        <td>Nombre d’événements d’enregistrement CREATE capturés entre les actualisations de données précédentes et les dernières pour le type d’objet.  </td>
    </tr>
                <tr>
        <td>MIS À JOUR</td>
        <td>Nombre </td>
        <td>Nombre d’événements d’enregistrement UPDATE capturés entre les actualisations de données précédentes et les dernières pour le type d’objet.</td>
    </tr>
                <tr>
        <td>SUPPRIMÉ</td>
        <td>Nombre </td>
        <td>Nombre d’événements d’enregistrement DELETE capturés entre les actualisations de données précédentes et les dernières pour le type d’objet. </td>
    </tr>
                <tr>
        <td>TOTAL</td>
        <td>Nombre </td>
        <td>Nombre total d’événements entre les actualisations de données précédentes et les dernières pour le type d’objet. 
        <br> 
        <br><b>Remarque </b> : il ne s’agit pas du même nombre total d’enregistrements affectés par des événements CREATE, UPDATE ou DELETE, car un même enregistrement peut être CRÉÉ et MIS À JOUR plusieurs fois entre les actualisations.  </td>
    </tr>
   </table>

