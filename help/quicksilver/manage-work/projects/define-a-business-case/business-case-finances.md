---
content-type: overview
navigation-topic: business-case-and-scorecards
title: Vue d’ensemble des champs financiers de l’analyse de rentabilité
description: Le sous-onglet Analyse de cas comprend des champs financiers pour le projet. Pour que certains champs financiers aient des valeurs, les domaines correspondants de l'Analyse de cas doivent être renseignés.
author: Alina
feature: Work Management
exl-id: d420fc3e-e98d-47a0-a456-b2df17d72f34
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '745'
ht-degree: 3%

---

# Vue d’ensemble des champs financiers de l’analyse de rentabilité

Le sous-onglet Analyse de cas comprend des champs financiers pour le projet. Pour que certains champs financiers aient des valeurs, les domaines correspondants de l&#39;Analyse de cas doivent être renseignés.  

Les champs financiers du projet suivants s’affichent dans l’Analyse de cas :

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th scope="col">Nom du champ</th> 
   <th scope="col">Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Aligné </td> 
   <td> <p>Affiche l’alignement du projet selon sa fiche d’évaluation. Un pourcentage élevé indique que le projet est bien aligné sur l’objectif et les objectifs de l’organisation. <br>Pour plus d’informations sur l’utilisation des Fiches d’évaluation, voir <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md" class="MCXref xref">Création d’une Fiche d’évaluation</a>.</p> <p>Ce champ s’affiche dans la zone Résumé de l’analyse de cas. </p> </td> 
  </tr> 
  <tr> 
   <td>Coût budgété</td> 
   <td> <p>Coût total estimé à associer au projet au lancement du projet.</p> <p>Le Coût budgété du projet est calculé selon la formule suivante :<br></p> <p><code>Budgeted Cost =&nbsp;Budgeted Expense Cost + Budgeted Labor Cost </code> <br> </p> <p>Adobe Workfront utilise les Heures budgétisées du planificateur de ressources pour calculer le coût de la main-d’oeuvre budgétisée.<br>Pour plus d’informations sur le calcul du coût budgété, voir <a href="../../../manage-work/projects/project-finances/budgeted-cost.md" class="MCXref xref">Calculer le coût budgété</a>. </p> <p>Ce champ s’affiche dans la zone Résumé de l’analyse de cas.</p> </td> 
  </tr> 
  <tr> 
   <td>Dépense inscrite au budget</td> 
   <td> <p>Le coût budgété de toutes les dépenses du projet. </p> <p>Elle est calculée par la formule suivante :</p> <p><code>Budgeted Expense Cost = SUM(Planned Amount of Expenses on the project) </code></p> <p>Pour plus d'informations sur le calcul des dépenses, voir <a href="../../../manage-work/projects/project-finances/manage-project-expenses.md" class="MCXref xref">Gérer les dépenses de projet </a>.</p> <p>Ce champ s'affiche dans la zone Dépenses .</p> </td> 
  </tr> 
  <tr> 
   <td>Coût budgété de la main-d'œuvre</td> 
   <td> <p>Le coût associé aux ressources affectées pour terminer le travail sur le projet.</p> <p>Le Coût de la main-d'oeuvre budgétisée du projet est calculé selon la formule suivante :<br></p> <p><code>Budgeted Labor Cost = SUM(Estimated/ Budgeted hours for each job role on the project * Cost per Hour rate of each job role on the project) </code><br></p> <p>Workfront utilise les Heures budgétisées du planificateur de ressources pour calculer le coût de la main-d’oeuvre budgétisée.<br>Pour plus d’informations sur le calcul du coût de la main-d’oeuvre budgété, voir <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Comprendre le coût de la main-d’oeuvre budgété et les heures budgétées pour les projets</a>.</p> <p>Ce champ s’affiche dans la zone Budget des ressources de l’Analyse de cas. </p> </td> 
  </tr> 
  <tr> 
   <td>Dépenses Coût planifié</td> 
   <td> <p>Il s’agit de la même chose que le coût des dépenses budgétisées. </p> <p>Remarque : le coût planifié des dépenses est différent du coût planifié du projet. Le coût planifié des dépenses est calculé à partir du montant prévu des dépenses du projet, tandis que le coût planifié est calculé à partir des Heures planifiées du projet. </p> <p>Ce champ s'affiche dans la zone Dépenses, pour chaque dépense.</p> </td> 
  </tr> 
  <tr> 
   <td>Valeur nette</td> 
   <td> <p>Il s’agit de la valeur totale attendue du projet après avoir calculé ses prestations et supprimé les coûts.</p> <p>La valeur nette du projet est calculée selon la formule suivante :<br></p> <p><code>Net Value = Planned Benefit - Budgeted Cost - Potential Risk</code>. <br></p> <p>Pour plus d’informations sur le calcul de la valeur nette, voir <a href="../../../manage-work/projects/project-finances/calculate-net-value.md" class="MCXref xref">Calculate Net Value</a>.<br></p> <p>Ce champ s’affiche dans la zone Résumé de l’analyse de cas.</p> </td> 
  </tr> 
  <tr> 
   <td>Bénéfice prévu</td> 
   <td>Une estimation manuelle de l’avantage financier pour votre organisation une fois ce projet terminé. Il peut s’agir de n’importe quelle devise et il est spécifique à vous et à chaque projet que vous gérez. La valeur de l’avantage prévu ne peut pas être négative. Ce champ s’affiche dans la zone Résumé de l’analyse de cas et peut être modifié dans la zone Informations sur le projet de l’analyse de cas. </td> 
  </tr> 
  <tr> 
   <td>Coût potentiel des risques</td> 
   <td> <p>C'est le coût potentiel de tous les risques sur le projet. </p> <p>Elle est calculée à l'aide de la formule suivante :</p> <p><code>Potential Risk = SUM(Potential Cost * Probability of Risk) </code></p> <p>Pour plus d’informations sur les risques du projet, voir <a href="../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md" class="MCXref xref">Création et modification des risques sur les projets</a>.</p> <p>Ce champ s’affiche dans la zone Résumé de l’analyse de cas.</p> </td> 
  </tr> 
  <tr> 
   <td>Risque potentiel</td> 
   <td> <p>Dans le résumé de l’analyse de cas, il s’agit du coût de tous les risques s’ils doivent se produire, en fonction de leur probabilité. Par exemple, si un risque a un coût potentiel de 100 $ et une probabilité de 10 %, le risque potentiel est de 10 $. Le risque potentiel dans le résumé de l'analyse de cas est calculé à l'aide de la formule suivante :</p> <p><code>Potential&nbsp;Risk = SUM(Risk Potential Cost x Probability)</code> pour tous les risques. </p> </td> 
  </tr> 
  <tr> 
   <td>Coût de réduction des risques</td> 
   <td> <p>Le coût du plan d’atténuation pour les risques que vous estimez peut survenir sur le projet.<br>Pour plus d’informations sur les risques du projet, voir <a href="../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md" class="MCXref xref">Créer et modifier des risques sur les projets</a>.</p> <p>Ce champ s’affiche dans la zone Risques pour chaque risque spécifié dans le projet.</p> </td> 
  </tr> 
  <tr> 
   <td>Coût potentiel d'un risque</td> 
   <td> <p>Le coût financier estimé lorsque les risques définis sur le projet se produiraient réellement, quelle que soit leur probabilité. </p> <p>Il s’agit d’un champ mis à jour manuellement qui s’affiche sur chaque risque dans la zone Risques de l’analyse de cas. </p> </td> 
  </tr> 
  <tr> 
   <td>Risques Coût potentiel total</td> 
   <td> <p>Il s’agit du coût financier total estimé de tous les risques définis sur le projet lorsqu’ils se sont réellement produits. </p> <p>Elle est calculée par la formule suivante :</p> <p><code>Risks Total Potential Cost = SUM(Potential Cost of all risks on the project) </code></p> <p>Il s’affiche sous la forme d’un numéro de devise en regard du titre de la zone Risques de l’Analyse de cas.</p> </td> 
  </tr> 
 </tbody> 
</table>
