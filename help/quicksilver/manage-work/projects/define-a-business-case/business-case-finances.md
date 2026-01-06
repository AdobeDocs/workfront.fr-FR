---
content-type: overview
navigation-topic: business-case-and-scorecards
title: Vue d’ensemble des champs financiers du business case
description: Le sous-onglet Business Case comprend des champs financiers pour le projet. Pour que certains champs financiers aient des valeurs, les zones correspondantes du business case doivent être complétées.
author: Becky
feature: Work Management
exl-id: d420fc3e-e98d-47a0-a456-b2df17d72f34
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '745'
ht-degree: 82%

---

# Vue d’ensemble des champs financiers du business case

Le sous-onglet Business Case comprend des champs financiers pour le projet. Pour que certains champs financiers aient des valeurs, les zones correspondantes du business case doivent être complétées.

Les champs financiers du projet suivant s’affichent dans le business case :

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
   <td>Aligné </td> 
   <td> <p>Affiche l’alignement du projet en fonction de sa carte de performance. Un pourcentage élevé indique que le projet est bien aligné sur la finalité et les objectifs de l’organisation. <br>Pour plus d’informations sur l’utilisation des cartes de performance, consultez <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md" class="MCXref xref">Créer une carte de performance</a>.</p> <p>Ce champ s’affiche dans la zone Résumé du business case. </p> </td> 
  </tr> 
  <tr> 
   <td>Coût budgété</td> 
   <td> <p>Le coût total estimé du projet au moment de son lancement.</p> <p>Le coût budgété du projet est calculé à l’aide de la formule suivante :<br></p> <p><code>Budgeted Cost = Budgeted Expense Cost + Budgeted Labor Cost </code> <br> </p> <p>Adobe Workfront utilise les heures budgétées du planificateur de ressources pour calculer le coût budgété de la main-d’œuvre.<br>Pour plus d'informations sur le calcul des coûts budgétés, voir <a href="../../../manage-work/projects/project-finances/budgeted-cost.md" class="MCXref xref">Calculer les coûts budgétés</a>. </p> <p>Ce champ s’affiche dans la zone Résumé du business case.</p> </td> 
  </tr> 
  <tr> 
   <td>Dépense inscrite au budget</td> 
   <td> <p>Coût budgété de toutes les dépenses du projet. </p> <p>Cela est calculé à l’aide de la formule suivante :</p> <p><code>Budgeted Expense Cost = SUM(Planned Amount of Expenses on the project) </code></p> <p>Pour plus d’informations sur le calcul des dépenses, consultez <a href="../../../manage-work/projects/project-finances/manage-project-expenses.md" class="MCXref xref">Gérer les dépenses du projet</a>.</p> <p>Ce champ s'affiche dans la zone Dépenses.</p> </td> 
  </tr> 
  <tr> 
   <td>Coût budgété de la main-d'œuvre</td> 
   <td> <p>Coût associé aux ressources affectées à la réalisation des travaux du projet.</p> <p>Le coût budgété de la main-d’œuvre pour le projet est calculé à l’aide de la formule suivante :<br></p> <p><code>Budgeted Labor Cost = SUM(Estimated/ Budgeted hours for each job role on the project * Cost per Hour rate of each job role on the project) </code><br></p> <p>Workfront utilise les heures budgétées du planificateur de ressources pour calculer le coût budgété de la main-d'œuvre.<br>Pour plus d’informations sur le calcul du coût budgété de la main-d’œuvre, consultez <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Présentation du coût budgété de la main-d’œuvre et des heures budgétées pour les projets</a>.</p> <p>Ce champ s’affiche dans la zone d’établissement du budget de ressources du business case. </p> </td> 
  </tr> 
  <tr> 
   <td>Coût prévu des dépenses</td> 
   <td> <p>C’est la même chose que le coût budgété des dépenses. </p> <p>Note : le coût prévu des dépenses est différent du coût prévu du projet. Le coût prévu des dépenses est calculé à partir du montant prévu des dépenses du projet, tandis que le coût prévu est calculé à partir du nombre d’heures prévues du projet. </p> <p>Ce champ s'affiche dans la zone Dépenses, pour chaque dépense.</p> </td> 
  </tr> 
  <tr> 
   <td>Valeur nette</td> 
   <td> <p>Il s’agit de la valeur totale attendue du projet après calcul de ses bénéfices et déduction des coûts.</p> <p>La valeur nette du projet est calculée à l’aide de la formule suivante :<br></p> <p><code>Net Value = Planned Benefit - Budgeted Cost - Potential Risk</code>. <br></p> <p>Pour plus d’informations sur le calcul de la valeur nette, consultez <a href="../../../manage-work/projects/project-finances/calculate-net-value.md" class="MCXref xref">Calculer la valeur nette</a>.<br></p> <p>Ce champ s’affiche dans la zone Résumé du business case.</p> </td> 
  </tr> 
  <tr> 
   <td>Bénéfice prévu</td> 
   <td>Estimation manuelle des bénéfices monétaires que votre organisation pourra retirer de la réalisation de ce projet. Il peut s’agir de n’importe quel montant. Ce dernier vous est propre et est spécifique à chaque projet que vous gérez. Le bénéfice prévu ne peut pas avoir une valeur négative. Ce champ s’affiche dans la zone Récapitulatif du business case et peut être modifié dans la zone Informations sur le projet du business case. </td> 
  </tr> 
  <tr> 
   <td>Coût potentiel des risques</td> 
   <td> <p>Il s’agit du coût potentiel de tous les risques associés au projet. </p> <p>Il est calculé à l’aide de la formule suivante :</p> <p><code>Potential Risk = SUM(Potential Cost * Probability of Risk) </code></p> <p>Pour plus d'informations sur les risques du projet, voir <a href="../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md" class="MCXref xref">Créer et modifier des risques sur les projets</a>.</p> <p>Ce champ s’affiche dans la zone Résumé du business case.</p> </td> 
  </tr> 
  <tr> 
   <td>Risque potentiel</td> 
   <td> <p>La zone Récapitulatif du business case comprend le montant du coût de tous les risques s’ils devaient se produire, sur la base de leur probabilité. Par exemple, si un risque a un coût potentiel de 100 $ et une probabilité de survenance de 10 %, le risque potentiel est de 10 $. Le risque potentiel indiqué dans le récapitulatif du business case est calculé à l’aide de la formule suivante :</p> <p><code>Potential Risk = SUM(Risk Potential Cost x Probability)</code> pour tous les risques. </p> </td> 
  </tr> 
  <tr> 
   <td>Coût de réduction des risques</td> 
   <td> <p>Le coût du plan d'atténuation pour les risques que vous estimez pourrait se produire sur le projet.<br>Pour plus d’informations sur les risques associés au projet, voir <a href="../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md" class="MCXref xref">Créer et modifier des risques sur des projets</a>.</p> <p>Ce champ s'affiche dans la zone Risques pour chaque risque spécifié dans le projet.</p> </td> 
  </tr> 
  <tr> 
   <td>Coût potentiel d’un risque</td> 
   <td> <p>Coût financier estimé lorsque les risques définis pour le projet se produisent, quelle que soit leur probabilité. </p> <p>Il s’agit d’un champ mis à jour manuellement qui s’affiche pour chaque risque dans la section Risques du Business case. </p> </td> 
  </tr> 
  <tr> 
   <td>Coût potentiel total des risques</td> 
   <td> <p>Coût financier total estimé de tous les risques définis pour le projet lorsqu’ils se sont produits. </p> <p>Cela est calculé à l’aide de la formule suivante :</p> <p><code>Risks Total Potential Cost = SUM(Potential Cost of all risks on the project) </code></p> <p>Cette donnée s’affiche sous une forme numérique en devise à côté du titre de la section Risques du Business case.</p> </td> 
  </tr> 
 </tbody> 
</table>
