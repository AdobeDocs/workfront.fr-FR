---
content-type: overview
product-area: agile-and-teams
navigation-topic: burndown
title: Aperçu du graphique de Burndown mobile
description: Le graphique d’avancement fournit une représentation visuelle de l’avancement des histoires dans l’itération ou le projet. Le taux d’avancement réel est mesuré par rapport au taux d’avancement idéal pour la chronologie de l’itération ou du projet.
author: Lisa
feature: Agile
exl-id: 414e3315-35ed-4aa4-a2d8-be42ec585f29
source-git-commit: d660707dd69fab78095eed1414092a7c909ba174
workflow-type: tm+mt
source-wordcount: '936'
ht-degree: 99%

---

# Vue d’ensemble du graphique d’avancement Agile

Le graphique d’avancement fournit une représentation visuelle de l’évolution des histoires à travers l’itération. Le taux d’avancement réel est mesuré par rapport au taux d’avancement idéal pour la chronologie d’itération.

Le graphique d’avancement s’ajuste en fonction du jour sélectionné. Le jour en cours est la valeur par défaut. Lorsqu’un jour précédent est sélectionné, toutes les données du graphique d’avancement et toutes les valeurs de la section [!UICONTROL statut d’achèvement] au-dessus du graphique d’avancement sont recalculées afin de représenter les données telles qu’elles se trouvaient à la fin du jour sélectionné. (Vous pouvez sélectionner les jours précédents ou le jour en cours ; vous ne pouvez pas sélectionner de jours futurs.)

![](assets/agile-iteration-burndown-350x88.png)

## Indicateurs visuels

Le graphique d’avancement contient les indicateurs visuels suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-dottedblue.png" alt=""> </td> 
   <td> <p>Le taux d’avancement idéal en fonction du moment où l’itération a commencé.</p> <p>Cette ligne ne s’affiche pas si la portée de l’itération ne change jamais (les heures ou les points ne sont jamais ajoutés ou supprimés).</p> <p>Cette ligne est plate lorsque le travail est effectué un jour de congé. Pour plus d’informations, consultez <a title="Utiliser le graphique d’avancement Agile" href="#how-days-off-affect-the-burndown-chart" class="MCXref xref">Effet des jours de congé sur le graphique d’avancement</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-solidblue.png" alt=""> </td> 
   <td> <p>Le taux d’avancement idéal en fonction des histoires ou des tâches en cours.</p> <p>Le taux d’avancement idéal actuel (ligne bleue pleine) diffère du taux d’avancement idéal d’origine (ligne bleue pointillée) lorsque des heures ou des points sont ajoutés ou supprimés de l’itération une fois l’itération commencée.</p> <p>Cette ligne est plate lorsque le travail est effectué un jour de congé.</p> <p>Pour plus d’informations, consultez <a title="Utiliser le graphique d’avancement Agile" href="#how-days-off-affect-the-burndown-chart" class="MCXref xref">Effet des jours de congé sur le graphique d’avancement</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-red.png" alt=""> </td> 
   <td> <p>Le taux d’avancement réel s’affiche en rouge lorsque le taux d’avancement est inférieur au taux idéal (plus de points ou d’heures par jour que le calcul d’avancement idéal).</p> <p>La formule suivante est utilisée pour calculer le taux d’avancement réel :</p> <p>[SUM(valeur de point ou d’heure de travail en cours * pourcentage terminé) + valeur de point ou d’heure de travail terminé]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-green.png" alt=""> </td> 
   <td> <p>Le taux d’avancement réel s’affiche en vert lorsque le taux d’avancement est égal ou supérieur au taux idéal (égal ou inférieur au nombre de points restant par jour par rapport au calcul d’avancement idéal).</p> <p>La formule suivante est utilisée pour calculer le taux d’avancement réel :</p> <p>[SUM(valeur de point ou d’heure de travail en cours * pourcentage terminé) + valeur de point ou d’heure de travail terminé]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-scope.png" alt=""> </td> 
   <td> <p>Changements de portée (heures ou points ajoutés ou supprimés de l’itération).</p> <p>Les changements de portée sont toujours affichés sous la forme d’une ligne verticale au milieu de la journée. En outre, un point bleu s’affiche au milieu de toute journée où un changement de portée s’est produit.</p> <p>L’axe vertical du graphique d’avancement affiche les points ou heures de l’histoire.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-scope.png" alt=""> </td> 
   <td> <p>Changements de période (la durée d’itération est augmentée ou réduite).</p> <p>Un point bleu s’affiche au milieu d’une journée où la durée d’itération a été modifiée.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-scope.png" alt=""> </td> 
   <td> <p>Un point vert ou rouge est affiché sur le taux d’avancement réel chaque fois que le travail progresse. (Lorsque le taux d’avancement réel sur cette journée est rouge, le point est rouge ; lorsque le taux d’avancement réel sur cette journée est vert, le point est vert.)</p> <p>Le travail progresse lorsque l’une des situations suivantes se produit :</p> 
    <ul> 
     <li> La valeur [!UICONTROL Percent Complete] augmente dans l’histoire.<br>[!UICONTROL Percent Complete] augmente en cas de : 
      <ul> 
       <li> <p>modification manuelle ;</p> </li> 
       <li> <p>mise à jour du nombre de points ou d’heures dans l’histoire ;</p> </li> 
      </ul></li>  
     <li>modification du statut de l’histoire sur [!UICONTROL Complete].</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Effet des jours de congé sur le graphique d’avancement {#how-days-off-affect-the-burndown-chart}

Le planning par défaut défini dans [!DNL Workfront] affecte le graphique d’avancement en excluant les jours de congé (week-ends et jours fériés) de la progression. Le graphique d’avancement utilise le planning par défaut pour définir les jours de travail (comme décrit dans la section [Créer un planning](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)).

Les équipes Agile peuvent incorporer des jours non ouvrés spécifiques à l’équipe en définissant un autre planning (comme décrit dans l’article [Utiliser un autre planning d’équipe pour les graphiques d’avancement](../../../agile/use-scrum-in-an-agile-team/burndown/use-alt-team-schedule-burndown-charts.md)). Ce planning alternatif est ensuite repris dans le graphique d’avancement de toute itération affectée à l’équipe. Le planning alternatif affecte uniquement le graphique d’avancement.

Les jours de congé sont pris en compte dans le graphique d’avancement uniquement dans les cas suivants :

* Le travail a été consigné lors d’un jour de congé. (Le jour où le travail a été enregistré s’affiche.)

  Lorsque le travail est consigné un jour de congé :

   * Le travail consigné n’est pas inclus lors du calcul de l’avancement idéal, car l’équipe n’est pas planifiée pour effectuer du travail.
   * Les lignes d’avancement idéal (la ligne bleue pleine et la ligne bleue en pointillés) s’affichent sous forme de lignes plates dans le graphique d’avancement pour n’importe quel jour où le travail a été effectué ou le jour où vous affichez le graphique d’avancement (si vous affichez un jour de congé).
   * Le travail enregistré est inclus lors du calcul d’autres statistiques d’avancement, telles que l’achèvement estimé et la moyenne des points ou heures par jour.

* Vous affichez le graphique d’avancement un jour de congé. (Le jour que vous consultez s’affiche sur le graphique d’avancement.)
* Vous effectuez le travail restant pour l’itération un jour de congé.

  Lorsqu’un utilisateur ou une utilisatrice termine tout le travail restant pour l’itération un jour de congé, le champ [!UICONTROL Estimation d’achèvement] affiche la date à laquelle l’itération a été terminée.

  Lors de la planification de l’itération, si vous définissez la date de fin de l’itération sur un jour non ouvré et que l’itération est censée se terminer dans les temps, la date d’[!UICONTROL Estimation d’achèvement] est définie sur le dernier jour ouvrable précédant la date de fin de l’itération que vous avez définie (étant donné que le travail n’est pas planifié pour être effectué pendant les jours non ouvrés).

  La date de fin de l’itération est spécifiée lors de la planification de l’itération, comme décrit dans l’article [Créer une itération](../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md).
