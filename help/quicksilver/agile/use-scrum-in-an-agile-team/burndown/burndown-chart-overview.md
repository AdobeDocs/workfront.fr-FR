---
content-type: overview
product-area: agile-and-teams
navigation-topic: burndown
title: Présentation du graphique en décharge agile
description: Le graphique de condensation fournit une représentation visuelle de l’avancement des articles dans l’itération ou le projet . Le taux de charge réel est mesuré par rapport au taux de charge idéal pour l’itération ou la chronologie du projet.
author: Lisa
feature: Agile
exl-id: 414e3315-35ed-4aa4-a2d8-be42ec585f29
source-git-commit: ddff70b61a2c3b3479e278bb3bb8628ac83f5c97
workflow-type: tm+mt
source-wordcount: '936'
ht-degree: 0%

---

# Présentation du graphique en décharge agile

Le graphique en courbes de charge fournit une représentation visuelle de l’évolution des histoires à travers l’itération. Le taux de charge réel est mesuré par rapport au taux de charge idéal pour la chronologie d’itération.

Le graphique de ventilation s’ajuste en fonction du jour sélectionné. Le jour en cours est la valeur par défaut. Lorsqu’un jour précédent est sélectionné, toutes les données du graphique de ventilation et toutes les valeurs de la variable [!UICONTROL état d’achèvement] Les sections situées au-dessus du graphique de ventilation sont recalculées afin de représenter les données telles qu’elles se trouvaient à la fin du jour sélectionné. (Vous pouvez sélectionner les derniers jours ou le jour en cours ; vous ne pouvez pas sélectionner de jours à l’avenir.)

![](assets/agile-iteration-burndown-350x88.png)

## Indicateurs visuels

Le graphique de ventilation contient les indicateurs visuels suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-dottedblue.png" alt=""> </td> 
   <td> <p>Taux de charge idéal en fonction du moment où l’itération a commencé.</p> <p>Cette ligne ne s’affiche pas si la portée de l’itération ne change jamais (les heures ou les points ne sont jamais ajoutés ou supprimés).</p> <p>Cette ligne s’affiche comme plate lorsque le travail est effectué un jour de congé. Pour plus d’informations, voir <a title="Utilisation du diagramme de Burndown ageur" href="#how-days-off-affect-the-burndown-chart" class="MCXref xref">Effet des jours de congé sur le graphique de ventilation</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-solidblue.png" alt=""> </td> 
   <td> <p>Taux de charge idéal en fonction des articles ou des tâches en cours.</p> <p>Le taux de charge idéal actuel (ligne bleue pleine) diffère du taux de charge idéal d’origine (ligne bleue pointillée) lorsque des heures ou des points sont ajoutés ou supprimés de l’itération une fois l’itération commencée.</p> <p>Cette ligne s’affiche comme plate lorsque le travail est effectué un jour de congé.</p> <p>Pour plus d’informations, voir <a title="Utilisation du diagramme de Burndown ageur" href="#how-days-off-affect-the-burndown-chart" class="MCXref xref">Effet des jours de congé sur le graphique de ventilation</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-red.png" alt=""> </td> 
   <td> <p>Le taux de charge réel s’affiche en rouge lorsque le taux de charge est inférieur à l’idéal (plus de points ou d’heures par jour que le calcul idéal).</p> <p>La formule suivante est utilisée pour calculer le taux de charge réel :</p> <p>[SUM(valeur ponctuelle ou horaire du travail en cours * pourcentage terminé) + valeur ponctuelle ou horaire du travail terminé]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-green.png" alt=""> </td> 
   <td> <p>Le taux de charge réel s’affiche en vert lorsque le taux de charge est égal ou supérieur à l’idéal (égal ou inférieur au nombre de points restant par jour par rapport au calcul idéal).</p> <p>La formule suivante est utilisée pour calculer le taux de charge réel :</p> <p>[SUM(valeur ponctuelle ou horaire du travail en cours * pourcentage terminé) + valeur ponctuelle ou horaire du travail terminé]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-scope.png" alt=""> </td> 
   <td> <p>Modification de la portée (les heures ou les points sont ajoutés ou supprimés de l’itération).</p> <p>Les changements de portée sont toujours affichés sous la forme d’une ligne verticale au milieu de la journée. En outre, un point bleu s’affiche au milieu de toute journée où un changement de portée s’est produit.</p> <p>L’axe vertical du graphique de condensation affiche les points ou heures de l’histoire.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-scope.png" alt=""> </td> 
   <td> <p>Modification de la période (la durée d’itération est augmentée ou réduite).</p> <p>Un point bleu s’affiche au milieu d’une journée où la durée d’itération a été modifiée.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-scope.png" alt=""> </td> 
   <td> <p>Un point vert ou rouge est affiché sur le taux de charge réel chaque fois que le travail est réduit en cendres. (Lorsque le taux de charge réel sur cette journée est rouge, le point est rouge ; lorsque le taux de charge réel sur cette journée est vert, le point est vert.)</p> <p>Le travail est réduit en cendres lorsque l’une des situations suivantes se produit :</p> 
    <ul> 
     <li> Le [!UICONTROL Pourcentage terminé] est augmenté dans l’histoire.<br>[!UICONTROL Pourcentage terminé] augmente lorsque : 
      <ul> 
       <li> <p>Modifié manuellement</p> </li> 
       <li> <p>Le nombre de points ou d’heures est mis à jour sur l’article.</p> </li> 
      </ul></li>  
     <li>L’état de l’article passe à [!UICONTROL Complete]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Effet des jours de congé sur le graphique de ventilation {#how-days-off-affect-the-burndown-chart}

La planification par défaut définie dans [!DNL Workfront] affecte le graphique de la charge en excluant les jours de congé (week-ends et jours fériés) de la charge. Le graphique de ventilation utilise la planification par défaut pour définir les jours de travail (comme décrit dans la section  [Création d’un planning](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)).

Les équipes agiles peuvent incorporer des jours non ouvrés spécifiques à l’équipe en définissant un autre planning (comme décrit dans l’article). [Utilisation d’un autre planning d’équipe pour les graphiques de ventilation](../../../agile/use-scrum-in-an-agile-team/burndown/use-alt-team-schedule-burndown-charts.md)). Ce planning alternatif est ensuite repris dans le graphique de répartition de toute itération affectée à l&#39;équipe. La planification alternative affecte uniquement le graphique de ventilation.

Les jours de congé ne sont pris en compte dans le graphique de ventilation que si :

* Le travail était auparavant connecté lors d’un jour de congé. (Le jour où le travail a été consigné s’affiche.)

  Lorsque le travail est connecté un jour de congé :

   * Les tâches consignées ne sont pas incluses lors du calcul de la charge maximale, car l’équipe n’est pas planifiée pour effectuer une tâche.
   * Les lignes de ventilation idéales (la ligne bleue pleine et la ligne bleue en pointillés) s’affichent sous forme de lignes plates dans le graphique de ventilation pour n’importe quel jour où le travail a été effectué ou le jour où vous affichez le graphique de ventilation (si vous affichez un jour de congé).
   * Le travail consigné est inclus lors du calcul d’autres statistiques de charge, telles que l’achèvement estimé et la moyenne des points ou heures par jour.

* Vous affichez le graphique de charge un jour de congé. (Le jour que vous affichez s’affiche sur le graphique de ventilation.)
* Vous effectuez le reste du travail pour l’itération un jour de congé.

  Lorsqu’un utilisateur termine la totalité du travail restant pour l’itération un jour de congé, la variable [!UICONTROL Achèvement estimé] affiche la date à laquelle l’itération a été effectuée.

  Lors de la planification de l’itération, si vous définissez la date de fin de l’itération pour un jour non fonctionnel et que le suivi de l’itération se termine à temps, la variable [!UICONTROL Achèvement estimé] est définie pour le dernier jour de travail précédant la date de fin de l’itération que vous définissez (car le travail n’est pas planifié pour être réduit en cendres les jours non ouvrés).

  La date de fin de l’itération est spécifiée lors de la planification de l’itération, comme décrit dans l’article. [Créer une itération](../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md).
