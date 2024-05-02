---
title: Configurer une visualisation à barres dans la zone de travail de reporting
description: Configurer une visualisation à barres dans la zone de travail de reporting
hidefromtoc: true
hide: true
exl-id: 7dc4f156-d262-482f-aa82-c905f0d1b20f
source-git-commit: 535e9c8481ce0781ee0d35636bb6d56de4d1e102
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 8%

---

# Configurer une visualisation à barres dans la zone de travail de reporting

Une visualisation en barres peut vous aider à raconter rapidement une histoire sur vos données en mettant en évidence des informations importantes à l’aide de barres horizontales.

## Conditions préalables

Avant de commencer, vous devez vous inscrire à la version bêta du canevas de création de rapports. Pour plus d’informations, voir [Version bêta du canevas de création de rapports : présentation](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## Configuration d’une visualisation en barres

>[!NOTE]
>
>Toutes vos modifications sont enregistrées automatiquement lorsque vous créez et modifiez les blocs de votre rapport.

1. Ajoutez tout d’abord un bloc de visualisation avec le **Barre** type de visualisation d’un rapport, comme expliqué dans la section [Ajout ou modification d’un bloc de visualisation dans la zone de travail de création de rapports](../../../reports-and-dashboards/reporting-canvas/visualization-blocks/add-or-edit-report-visualization.md).

1. Cliquez sur l’icône Modifier la visualisation . ![](assets/edit-icon.png) dans le coin supérieur droit de la visualisation, effectuez l’une des opérations suivantes.

   1. Sur le **Paramètres** tab :

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">Type de visualisation</td>
         <td><p>Passez à un autre type de visualisation. Dans ce cas, les options suivantes du menu peuvent changer.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Axe vertical</td>
         <td><p>Sélectionnez les données que vous souhaitez représenter le long du bord vertical gauche ou de l’axe Y de la visualisation en barres. La visualisation compare les éléments sur cet axe en fonction de chaque élément de l’axe horizontal.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Axe horizontal</td>
         <td><p>Dans le menu déroulant de gauche, sélectionnez les données que vous souhaitez représenter le long de l’axe horizontal ou X. Les éléments de cet axe s’affichent sous forme de barres comparatives, en fonction de leurs valeurs.</p><p>Dans le menu déroulant de droite, sélectionnez la manière dont vous souhaitez que la visualisation calcule et affiche les valeurs le long de l’axe horizontal :</p>
          <ul>
           <li><p><b>Count</b>: nombre de valeurs</p></li>
           <li><p><b>Somme</b>: le total de toutes les valeurs </p></li>
           <li><p><b>Moyenne</b>: moyenne de toutes les valeurs</p></li>
           <li><p><b>Minimum</b>: seule la valeur la plus faible</p></li>
           <li><p><b>Maximum</b>: seule la valeur la plus élevée</p></li>
          </ul></td>
        </tr>
        <tr>
         <td role="rowheader">+ Ajouter une valeur</td>
         <td>Ajoutez un autre champ dont vous souhaitez effectuer le suivi le long de l’axe horizontal.</td>
        </tr>
       </tbody>
      </table>

   1. Sur le **Données** tab :

      | Source de données (menu déroulant) | Remplacez la source de données de la visualisation par un autre tableau du canevas de rapport. |
      |---|---|
      | Afficher la source de données | Activez cette option pour afficher le tableau source de la visualisation sur la zone de travail du rapport ou désactivez l’option pour le masquer. |

      {style="table-layout:auto"}

      <!--   
      NOLAN-FLAG: convert table to html. 
      -->

1. Cliquez n’importe où en dehors du menu des paramètres de visualisation pour le fermer.
