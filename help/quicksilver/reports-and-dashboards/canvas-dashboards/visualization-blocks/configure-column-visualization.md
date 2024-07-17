---
title: Configurer une visualisation à colonnes dans la zone de travail de reporting
description: Configurer une visualisation à colonnes dans la zone de travail de reporting
hidefromtoc: true
hide: true
exl-id: 5a0cdcd4-b44b-4a63-964e-1c570cd9ff77
source-git-commit: 535e9c8481ce0781ee0d35636bb6d56de4d1e102
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 8%

---

# Configurer une visualisation à colonnes dans la zone de travail de reporting

Une visualisation en colonnes peut vous aider à raconter rapidement une histoire sur vos données en mettant en surbrillance des informations importantes à l’aide de colonnes verticales.

## Conditions préalables

Avant de commencer, vous devez vous inscrire à la version bêta du canevas de création de rapports. Pour plus d’informations, reportez-vous à la section [Présentation du canevas de rapports bêta : présentation](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## Configuration d’une visualisation en colonne

>[!TIP]
>
>Toutes vos modifications sont enregistrées automatiquement lorsque vous créez et modifiez les blocs de votre rapport.

1. Commencez par ajouter un bloc de visualisation avec le type de visualisation **Colonne** à un rapport, comme expliqué dans la section [Ajouter ou modifier un bloc de visualisation dans le canevas de rapports](../../../reports-and-dashboards/reporting-canvas/visualization-blocks/add-or-edit-report-visualization.md).

1. Cliquez sur l’icône Modifier la visualisation ![](assets/edit-icon.png) dans le coin supérieur droit de la visualisation, puis effectuez l’une des opérations suivantes.

   1. Sous l’onglet **Paramètres** :

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
           <li><p><b>Count</b> : nombre de valeurs</p></li>
           <li><p><b>Sum</b> : total de toutes les valeurs </p></li>
           <li><p><b>Moyenne</b> : moyenne de toutes les valeurs</p></li>
           <li><p><b>Minimum</b> : seule la valeur la plus basse</p></li>
           <li><p><b>Maximum</b> : seule la valeur la plus élevée</p></li>
          </ul></td>
        </tr>
       </tbody>
      </table>

   1. Sur l’onglet **Data** :

      | Source de données (menu déroulant) | Remplacez la source de données de la visualisation par un autre tableau du canevas de rapport. |
      |---|---|
      | Afficher le Source de données | Activez cette option pour afficher le tableau source de la visualisation sur la zone de travail du rapport ou désactivez l’option pour le masquer. |

      {style="table-layout:auto"}

      <!--   
      NOLAN-FLAG: convert table to html. 
      -->

1. Cliquez n’importe où en dehors du menu des paramètres de visualisation pour le fermer.
