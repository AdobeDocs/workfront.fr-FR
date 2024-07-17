---
title: Configurer une visualisation à secteurs dans la zone de travail de reporting
description: Configurer une visualisation à secteurs dans la zone de travail de reporting
hidefromtoc: true
hide: true
exl-id: 0497edb5-9322-406a-b53b-ec498afdd96e
source-git-commit: 535e9c8481ce0781ee0d35636bb6d56de4d1e102
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 7%

---

# Configurer une visualisation à secteurs dans la zone de travail de reporting

Une visualisation circulaire peut vous aider à raconter rapidement une histoire sur vos données en mettant en évidence des informations importantes dans un graphique circulaire avec des contours qui illustrent leurs proportions relatives.

## Conditions préalables

Avant de commencer, vous devez vous inscrire à la version bêta du canevas de création de rapports. Pour plus d’informations, reportez-vous à la section [Présentation du canevas de rapports bêta : présentation](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## Configuration d’une visualisation circulaire

>[!TIP]
>
>Toutes vos modifications sont enregistrées automatiquement lorsque vous créez et modifiez les blocs de votre rapport.

1. Commencez par ajouter un bloc de visualisation avec le type de visualisation **Circulaire** dans un rapport, comme expliqué dans la section [Ajouter ou modifier un bloc de visualisation dans le Canevas de création de rapports](../../../reports-and-dashboards/reporting-canvas/visualization-blocks/add-or-edit-report-visualization.md).

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
         <td role="rowheader">Tranches</td>
         <td>Sélectionnez les données que vous souhaitez que les contours représentent.</td>
        </tr>
        <tr>
         <td role="rowheader">Valeur</td>
         <td><p>Dans le menu déroulant de gauche, sélectionnez les valeurs à afficher sur chaque coin.</p><p>Dans le menu déroulant de droite, sélectionnez le mode de calcul de ces valeurs dans l’affichage :</p>
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
