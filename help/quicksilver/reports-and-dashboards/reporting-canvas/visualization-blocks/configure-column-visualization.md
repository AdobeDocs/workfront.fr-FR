---
title: Configuration d’une visualisation en colonne dans le canevas de création de rapports
description: Configuration d’une visualisation en colonne dans le canevas de création de rapports
hidefromtoc: true
hide: true
source-git-commit: 350d64577bac677bb0cc9bcb804c32b0301bc5d4
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 1%

---


# Configuration d’une visualisation en colonne dans le canevas de création de rapports

Une visualisation en colonnes peut vous aider à raconter rapidement une histoire sur vos données en mettant en surbrillance des informations importantes à l’aide de colonnes verticales.

## Conditions préalables

Avant de commencer, vous devez vous inscrire à la version bêta du canevas de création de rapports. Pour plus d’informations, voir [Version bêta du canevas de création de rapports : présentation](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## Configuration d’une visualisation en colonne

>[!TIP]
>
>Toutes vos modifications sont enregistrées automatiquement lorsque vous créez et modifiez les blocs de votre rapport.

1. Ajoutez tout d’abord un bloc de visualisation avec le **Colonne** type de visualisation d’un rapport, comme expliqué dans la section [Ajout ou modification d’un bloc de visualisation dans la zone de travail de création de rapports](../../../reports-and-dashboards/reporting-canvas/visualization-blocks/add-or-edit-report-visualization.md).

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
         <td role="rowheader">Axe horizontal</td>
         <td><p>Sélectionnez les données que vous souhaitez représenter le long de l’axe horizontal ou X de la visualisation en colonne. La visualisation compare les éléments sur cet axe en fonction de chaque élément de l’axe vertical.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Axe vertical</td>
         <td><p>Dans le menu déroulant de gauche, sélectionnez les données que vous souhaitez représenter le long de l’axe horizontal ou Y. La visualisation affiche les éléments sur cet axe sous forme de colonnes comparatives, en fonction de leurs valeurs.</p><p>Dans le menu déroulant de droite, sélectionnez le mode de calcul de ces valeurs dans l’affichage :</p>
          <ul>
           <li><p><b>Count</b>: nombre de valeurs</p></li>
           <li><p><b>Somme</b>: le total de toutes les valeurs </p></li>
           <li><p><b>Moyenne</b>: moyenne de toutes les valeurs</p></li>
           <li><p><b>Minimum</b>: seule la valeur la plus faible</p></li>
           <li><p><b>Maximum</b>: seule la valeur la plus élevée</p></li>
          </ul></td>
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
