---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: Exemple de calcul - Calcul du CRE au niveau du projet
description: Cet article donne un exemple de calcul de l’Estimation à l’achèvement (EAC) d’un projet au niveau du projet dans Adobe Workfront.
author: Lisa
feature: Work Management
exl-id: ff88b7e3-2a5b-464f-bed1-6848067840b8
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '2213'
ht-degree: 81%

---

# Exemple de calcul - Calculer l’estimation à l’achèvement à l’échelle du projet

## Méthode EAC : calcul au niveau du projet

* [PIM = basé sur les heures](#pim-hour-based)
* [PIM = basé sur les coûts](#pim-cost-based)

### PIM = basé sur les heures {#pim-hour-based}

* [Exemple simple : le projet n’a aucune tâche enfant](#simple-example-project-has-no-children-tasks).
* [Exemple complexe : le projet comporte des tâches enfant.](#complicated-example-project-has-children-tasks)

#### Exemple simple : le projet n’a aucune tâche enfant. {#simple-example-project-has-no-children-tasks}

PIM = basé sur les heures

Méthode EAC = calcul au niveau du projet ****

1. Créez le projet A avec trois tâches (aucune tâche enfant) affectées à la personne 1 dont le coût/heure est de 100,00 $.
1. Ajoutez les heures prévues et les heures effectives à chaque tâche et le Pourcentage terminé selon le tableau ci-dessous :

   <table style="table-layout:auto">
    <col>
    <col>
    <col>
    <col>
    <thead>
     <tr>
      <th><br><p><strong>Tâche</strong></p></th>
      <th><br><p><strong>Hrs Prév</strong></p></th>
      <th><br><p><strong>Hrs eff</strong></p></th>
      <th><p><strong>% effectué</strong></p></th>
     </tr>
    </thead>
    <tbody>
     <tr>
      <td><p>Tâche 1</p></td>
      <td><p>5 heures</p></td>
      <td><p>25 heures</p></td>
      <td><p>20 %</p></td>
     </tr>
     <tr>
      <td><p>Tâche 2</p></td>
      <td><p>10 heures</p></td>
      <td><p>25 heures</p></td>
      <td><p>30 %</p></td>
     </tr>
     <tr>
      <td><p>Tâche 3</p></td>
      <td><p>15 heures</p></td>
      <td><p>25 heures</p></td>
      <td><p>40 %</p></td>
     </tr>
    </tbody>
   </table>

1. Recalculer les finances sur le projet.
1. **ICP pour la Tâche 1** = 0,04 calculé comme suit :\
   **ICP pour la tâche 1** = *IF* Heures effectives > 0 *THEN* ICP = Coût budgété du travail effectué/Heures effectives\
   *SINON* IPC = 1\
   **ICP pour la tâche 1** = 1 / 25\
   **ICP pour la tâche 1** = 0,04

1. **EAC pour la Tâche 1** = 125 heures calculées comme suit :\
   **EAC pour la Tâche 1** = *IF* ICP &lt;> 0 *THEN* EAC = Nombre d’heures prévues/ICP\
   *ELSE* CRE = heures prévues + heures réelles\
   **EAC pour la Tâche 1** = 5 / 0,04\
   **EAC pour la Tâche 1** = 125 heures****

1. ICP/EAC pour les Tâches 2 et 3 :\
   Tâche 2 = .12 / 83,33 heures\
   Tâche 3 = 0,24 / 62,5 heures

1. **ICP du projet** = 0,13 calculé comme suit :\
   **ICP du projet** = *IF* Heures effectives > 0 *THEN* IPC = Coût budgété du travail effectué/Heures effectives\
   *SINON* IPC = 1\
   **ICP du projet** = 10 / 75\
   **ICP du projet** = 0,13

1. **EAC pour le projet** = 225 heures calculées comme suit :\
   **EAC pour le projet** = *IF* ICP &lt;> 0 *THEN* EAC = Heures prévues/ICP\
   *ELSE* CRE = heures prévues + heures réelles\
   **EAC pour le projet** = 30 / 0,13333\
   **EAC pour le projet** = 225 heures

#### Exemple complexe : le projet comporte des tâches enfant. {#complicated-example-project-has-children-tasks}

PIM = basé sur les heures

Méthode EAC = Calcul au niveau du projet

1. Créez le projet A avec six tâches, la tâche 3 étant parent des tâches 4 et 5 et la tâche 1 étant parent des tâches 2 et 3, comme illustré ci-dessous :\
   Tâche 1\
   Tâche 2\
   Tâche 3\
   Tâche 4\
   Tâche 5\
   Tâche 6

1. Affectez les tâches 2, 4, 5 et 6 à la personne 1 dont le coût/heure est de 100,00 $.
1. Ajoutez les heures prévues/effectives pour chaque tâche et le pourcentage d’achèvement selon le tableau ci-dessous.

   >[!NOTE]
   >
   >Pour les tâches 1 et 3, vous ajoutez uniquement des heures effectives.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <br> <p><strong>Tâche</strong> </p> </th> 
   <th> <br> <p><strong>Hrs Prév</strong> </p> </th> 
   <th> <br> <p><strong>Hrs eff</strong> </p> </th> 
   <th> <p><strong>% terminé</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Tâche 1</p> </td> 
   <td> </td> 
   <td> <p>10 heures</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 2</p> </td> 
   <td> <p>5 heures</p> </td> 
   <td> <p>10 heures</p> </td> 
   <td> <p>20 %</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 3</p> </td> 
   <td> </td> 
   <td> <p>10 heures</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 4</p> </td> 
   <td> <p>10 heures</p> </td> 
   <td> <p>10 heures</p> </td> 
   <td> <p>40 %</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 5</p> </td> 
   <td> <p>15 heures</p> </td> 
   <td> <p>10 heures</p> </td> 
   <td> <p>50 %</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 6</p> </td> 
   <td> <p>20 heures</p> </td> 
   <td> <p>10 heures</p> </td> 
   <td> <p>60 %</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Ajoutez 50 heures directement au projet (Plus > Heure > Consigner les heures).
1. **ICP pour la tâche 2** = 0,1 calculé comme suit :\
   **ICP pour la tâche 2** = *IF* Heures effectives > 0 *THEN* ICP = Coût budgété du travail effecté/Heures effectives\
   *SINON* IPC = 1\
   **ICP pour la tâche 2** = 1 / 10\
   **ICP pour la tâche 2** = 0,1

1. **EAC pour la tâche 2** = 50 heures calculées comme suit :\
   **EAC pour la tâche 2** = *IF* ICP &lt;> 0 *THEN* EAC = Heures prévues/ICP\
   *ELSE* CRE = heures prévues + heures réelles\
   **EAC pour la tâche 2** = 5 / 0,1\
   **EAC pour la tâche 2** = 50 heures

1. L’ICP et l’EAC pour les tâches 4, 5 et 6 sont les suivants :\
   Tâche 4 : 0,4 / 25 heures\
   Tâche 5 : 0,75 / 20 heures\
   Tâche 6 : 1,2 / 16,67 heures

1. **IPC pour la tâche 3** = .38 calculé comme suit :\
   **ICP pour la tâche 3** = *IF* Heures effectives > 0 *THEN* ICP = Coût budgété du travail effectué/Heures effectives\
   *SINON* IPC = 1\
   **ICP pour la tâche 3** = 11,5 / 30\
   **ICP pour la tâche 3** = 0,38

1. **EAC pour la tâche 3** = 65,22 heures calculées comme suit :\
   **EAC pour la tâche 3** = *IF* ICP &lt;> 0 *THEN* EAC = Heures prévues/ICP\
   *ELSE* CRE = heures prévues + heures réelles\
   **CRE pour la tâche 3** = 25 / .383333\
   **EAC pour la tâche 3** = 65,22 heures

1. **ICP pour la tâche 1** = 0,25 calculé comme suit :\
   **ICP pour la tâche 1** = *IF* Heures effectives > 0 *THEN* ICP = Coût budgété du travail effectué/Heures effectives\
   *SINON* IPC = 1\
   **ICP pour la tâche 1** = 12,5 / 50\
   **ICP pour la tâche 1** = 0,25

1. **EAC pour la tâche 1** = 120 heures calculées comme suit :\
   **EAC pour la tâche 1** = *IF* ICP &lt;> 0 *THEN* EAC = Heures prévues / ICP\
   *ELSE* CRE = heures prévues + heures réelles\
   **CRE pour la tâche 1** = 30/.25\
   **EAC pour la tâche 1** = 120 heures

1. **ICP du projet** = 0,22 calculé comme suit :\
   **ICP du projet** = *IF* Heures effectives > 0 *THEN* ICP = Coût budgété du travail effectué/Heures effectives\
   *SINON* IPC = 1\
   **ICP du projet** = 24,5 / 110\
   **ICP du projet** = 0,22272\
   **ICP du projet** = 0,22

1. **CRE pour le projet** = 224,49 heures calculées comme suit :\
   **EAC pour le projet** = *IF* ICP &lt;> 0 *THEN* EAC = Heures prévues/ICP\
   *ELSE* CRE = heures prévues + heures réelles\
   **CRE pour le projet** = 50 / .22272\
   **EAC pour le projet** = 224,49 heures

### PIM = basé sur les coûts {#pim-cost-based}

* [Exemple simple : le projet n’a aucune tâche enfant](#simple-example-project-has-no-children-tasks).
* [Exemple complexe : le projet comporte des tâches enfant.](#complicated-example-project-has-children-tasks)

#### Exemple simple : le projet n’a aucune tâche enfant. {#simple-example-project-has-no-children-tasks-1}

PIM = Basé sur les coûts

Méthode EAC = Calcul au niveau du projet

1. Créez le projet A avec trois tâches (aucune tâche enfant) affectées à la personne 1 dont le coût/heure est de 100,00 $.
1. Ajoutez les heures prévues/effectives à chaque tâche et le pourcentage d’achèvement au tableau ci-dessous :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <br> <p><strong>Tâche</strong> </p> </th> 
   <th> <br> <p><strong>Hrs Prév</strong> </p> </th> 
   <th> <br> <p><strong>Ct M-o Pré</strong> </p> </th> 
   <th> <br> <p><strong>Hrs eff</strong> </p> </th> 
   <th> <br> <p><strong>Cts trv eff</strong> </p> </th> 
   <th> <p><strong>% effectué</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Tâche 1</p> </td> 
   <td> <p>5 heures</p> </td> 
   <td> <p>500,00 $</p> </td> 
   <td> <p>25 heures</p> </td> 
   <td> <p>2 500,00 $</p> </td> 
   <td> <p>20 %</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 2</p> </td> 
   <td> <p>10 heures</p> </td> 
   <td> <p>1 000,00 $</p> </td> 
   <td> <p>25 heures</p> </td> 
   <td> <p>2 500,00 $</p> </td> 
   <td> <p>30 %</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 3</p> </td> 
   <td> <p>15 heures</p> </td> 
   <td> <p>1 500,00 $</p> </td> 
   <td> <p>25 heures</p> </td> 
   <td> <p>2 500,00 $</p> </td> 
   <td> <p>40 %</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Ajoutez des dépenses à chaque tâche en fonction du tableau ci-dessous :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Tâche</strong> </p> </th> 
   <th> <p><strong>Dépense</strong> </p> </th> 
   <th> <p><strong>Montant prévu</strong> </p> </th> 
   <th> <p><strong>Montant réel</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Tâche 1</p> </td> 
   <td> <p>Dép 1 Tâche 1</p> </td> 
   <td> <p>300,00 $</p> </td> 
   <td> <p>400,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 1</p> </td> 
   <td> <p>Dép 2 Tâche 1</p> </td> 
   <td> <p>500,00 $</p> </td> 
   <td> <p>0,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 2</p> </td> 
   <td> <p>Dép Tâche 2</p> </td> 
   <td> <p>200,00 $</p> </td> 
   <td> <p>100,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 3</p> </td> 
   <td> <p>Dép Tâche 3</p> </td> 
   <td> <p>800,00 $</p> </td> 
   <td> <p>700,00 $</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Ajoutez deux dépenses au projet (c’est-à-dire non liées à une tâche) comme suit :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Dépense</strong> </p> </th> 
   <th> <p><strong>Montant prévu</strong> </p> </th> 
   <th> <p><strong>Montant réel</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Dép Projet 1</p> </td> 
   <td> <p>1 000,00 $</p> </td> 
   <td> <p>1 500,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Dép 2 Tâche 1</p> </td> 
   <td> <p>2 500,00 $</p> </td> 
   <td> <p>0,00 $</p> </td> 
  </tr> 
 </tbody> 
</table>

1. En fonction des valeurs ci-dessus, les coûts engagés/non engagés sont déterminés comme suit :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Tâche</strong> </p> </th> 
   <th> <p><strong>Dépenses prévues non engagées</strong> </p> </th> 
   <th> <p><strong>Dépenses prévues engagées</strong> </p> </th> 
   <th> <p><strong>Dépenses réelles engagées</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Tâche 1</p> </td> 
   <td> <p>500,00 $</p> </td> 
   <td> <p>300,00 $</p> </td> 
   <td> <p>400,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 2</p> </td> 
   <td> <p>0,00 $</p> </td> 
   <td> <p>200,00 $</p> </td> 
   <td> <p>100,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 3</p> </td> 
   <td> <p>0,00 $</p> </td> 
   <td> <p>800,00 $</p> </td> 
   <td> <p>700,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projet</p> </td> 
   <td> <p>3 000,00 $</p> </td> 
   <td> <p>2 300,00 $</p> </td> 
   <td> <p> 2 700,00 $ <strong></strong></p> </td> 
  </tr> 
 </tbody> 
</table>

1. À partir des actions du projet, exécuter Recalculer finances
1. **ICP pour la tâche 1** = 0,14
1. **ICP****pour la tâche 1** = 0,14 calculé comme suit :\
   **ICP** **pour la tâche 1** = *IF* Coût réel de la main-d&#39;œuvre + IncurredActualExpenseCost &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   * SINON* ICP = CPI_Labor\
     **ICP****pour la tâche 1** = (100+300) / (2 500+400)\
     **IPC** **pour la tâche 1** = 400/2900\
     **ICP** **pour la tâche 1** = .14****

1. **EAC**** de la tâche 1** = 13 400 $\
   **IPC Main-d&#39;œuvre** **pour la tâche 1** = SI Coût réel de la main-d&#39;œuvre &lt;> 0 ALORS

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed/Actual Labor Cost
   ```

   SINON CPI_Labor = 1\
   **IPC Travail** **pour la tâche 1** = 100/2500\
   **Main-d&#39;œuvre de l&#39;IPC** **pour la tâche 1** = .04******Main-d&#39;œuvre de l&#39;EAC ****pour la tâche 1**=* IF *CPI_Labor &lt;> 0* THEN *Main-d&#39;œuvre de l&#39;EAC = Coût de main-d&#39;œuvre prévu/CPI_Labor
   * SINON* CRE Main-d&#39;œuvre = Coût prévu de main-d&#39;œuvre + Coût réel de main-d&#39;œuvre\
     **EAC main d’œuvre****de la tâche 1** = 500/0,04\
     **EAC main d’œuvre****de la tâche 1** = 12 500,00 $\
     **EAC dépense****de la tâche 1** = Coût des dépenses réelles engagées + Coût des dépenses prévues non engagées\
     **EAC dépenses****de la tâche 1** = 400 $ + 500 $\
     **EAC dépenses****de la tâche 1** = 900 $\
     **EAC dépenses**** de la tâche 1** = EAC main d’œuvre + EAC dépenses\
     **CRE****pour la tâche 1** = 12 500 $ + 900 $\
     **CRE****pour la tâche 1** = 13 400 $

1. Voici les valeurs ICP/EAC pour la tâche 2 et la tâche 3 :\
   Tâche 2 = 0,19 / 8 433,33 $\
   Tâche 3 = 0,44 / 6 950,00 $

1. **ICP pour le projet** = .32 calculé comme suit :\
   **ICP****pour le projet** = *IF* Coût réel de la main-d’œuvre + IncurredActualExpenseCost &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/ActualLaborCost + IncurredActualExpenseCost)
   ```

   * SINON* ICP = CPI_Labor\
     **ICP****du projet** = (1 000 + 2 300)/(7 500 + 2 700)\
     **ICP****du projet** = 3 300/10 200\
     **ICP****pour le projet** = 0,32

1. **EAC pour le projet** = 28 200,00 $ calculé comme suit :\
   **ICP de la main d’œuvre****pour le projet** = IF Coût réel de main d’œuvre &lt;> 0 THEN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed/Actual Labor Cost
   ```

   SINON CPI_Labor = 1\
   **ICP de la main d’œuvre****pour le projet** = 1000 / 7500\
   **ICP de la main d’œuvre****pour le projet** = 0,13333\
   **ICP de la main d’œuvre****pour le projet** = 0,13

   **EAC de la main d’œuvre****pour le projet** = *IF* CPI_Labor &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost/CPI_Labor
   ```

   * SINON* CRE Main-d&#39;œuvre = Coût prévu de main-d&#39;œuvre + Coût réel de main-d&#39;œuvre\
     **EAC de la main d’œuvre** = 3000/ .13 33\
     **EAC de la main d’œuvre** = 22 500,00 $

   **EAC des dépenses****Projet** =

   ```
   IncurredActualExpenseCost + NotIncurredPlannedExpense
   ```

   **EAC des dépenses****Projet** = 3 000,00 $ + 2 700,00\
   **EAC des dépenses****Projet** = 5 700,00 $

   **EAC****Projet** = EAC de la main d’œuvre + EAC des dépenses\
   **CRE****Projet** = 22 500 $ + 5 700 $\
   **CRE****Projet** = 28 200 $

#### Exemple complexe : le projet comporte des tâches enfant. {#complicated-example-project-has-children-tasks-1}

PIM = Basé sur les coûts

Méthode EAC = Calcul au niveau du projet

1. Créez le projet A avec six tâches, la tâche 3 étant parent des tâches 4 et 5 et la tâche 1 étant parent des tâches 2 et 3, comme illustré ci-dessous :\
   Tâche 1\
   Tâche 2\
   Tâche 3\
   Tâche 4\
   Tâche 5\
   Tâche 6

1. Affectez les tâches 2, 4, 5 et 6 à la personne 1 dont le coût/heure est de 100,00 $.
1. Ajoutez les heures prévues/réelles pour chaque tâche et le % Terminé selon le tableau ci-dessous.

   >[!NOTE]
   >
   >Pour les tâches 1 et 3, vous ajoutez uniquement des heures effectives.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <br> <p><strong>Tâche</strong> </p> </th> 
   <th> <br> <p><strong>Hrs Prév</strong> </p> </th> 
   <th> <br> <p><strong>Ct M-o Pré</strong> </p> </th> 
   <th> <br> <p><strong>Hrs eff</strong> </p> </th> 
   <th> <br> <p><strong>Cts trv eff</strong> </p> </th> 
   <th> <p><strong>% effectué</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Tâche 1</p> </td> 
   <td> </td> 
   <td> </td> 
   <td> <p>10 heures</p> </td> 
   <td> <p>1 000,00 $</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 2</p> </td> 
   <td> <p>5 heures</p> </td> 
   <td> <p>500,00 $</p> </td> 
   <td> <p>10 heures</p> </td> 
   <td> <p>1 000,00 $</p> </td> 
   <td> <p>20 %</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 3</p> </td> 
   <td> </td> 
   <td> </td> 
   <td> <p>10 heures</p> </td> 
   <td> <p>1 000,00 $</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 4</p> </td> 
   <td> <p>10 heures</p> </td> 
   <td> <p>1 000,00 $</p> </td> 
   <td> <p>10 heures</p> </td> 
   <td> <p>1 000,00 $</p> </td> 
   <td> <p>40 %</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 5</p> </td> 
   <td> <p>15 heures</p> </td> 
   <td> <p>1 500,00 $</p> </td> 
   <td> <p>10 heures</p> </td> 
   <td> <p>1 000,00 $</p> </td> 
   <td> <p>50 %</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 6</p> </td> 
   <td> <p>20 heures</p> </td> 
   <td> <p>2 000,00 $</p> </td> 
   <td> <p>10 heures</p> </td> 
   <td> <p>1 000,00 $</p> </td> 
   <td> <p>60 %</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Ajoutez 50 heures directement au projet (Plus > Heures > Consigner les heures) afin d’enregistrer 5 000,00 $ de coût réel de main-d’œuvre directement dans le projet. ****
1. Ajoutez des dépenses à chaque tâche en fonction du tableau ci-dessous (j’ai ajouté une ligne vide entre chaque tâche pour faciliter la lecture) :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Tâche</strong> </p> </th> 
   <th> <p><strong>Dépense</strong> </p> </th> 
   <th> <p><strong>Montant prévu</strong> </p> </th> 
   <th> <p><strong>Montant réel</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Tâche 1</p> </td> 
   <td> <p>Dép 1 Tâche 1</p> </td> 
   <td> <p>300,00 $</p> </td> 
   <td> <p>- 400,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 1</p> </td> 
   <td> <p>Dép 2 Tâche 1</p> </td> 
   <td> <p>- 500,00 $</p> </td> 
   <td> <p>800,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 1</p> </td> 
   <td> <p>Dép 3 Tâche 1</p> </td> 
   <td> <p>400,00 $</p> </td> 
   <td> <p>0,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 2</p> </td> 
   <td> <p>Dép 1 Tâche 2</p> </td> 
   <td> <p>500,00 $</p> </td> 
   <td> <p>700,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 2</p> </td> 
   <td> <p>Dép 2 Tâche 2</p> </td> 
   <td> <p>- 400,00 $</p> </td> 
   <td> <p>0,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 2</p> </td> 
   <td> <p>Dép 3 Tâche 2</p> </td> 
   <td> <p>- 200,00 $</p> </td> 
   <td> <p>600,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 2</p> </td> 
   <td> <p>Dép 4 Tâche 2</p> </td> 
   <td> <p>700,00 $</p> </td> 
   <td> <p>- 200,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 3</p> </td> 
   <td> <p>Dép Tâche 3</p> </td> 
   <td> <p>0,00 $</p> </td> 
   <td> <p>1 000,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 4</p> </td> 
   <td> <p>Dép 1 Tâche 4</p> </td> 
   <td> <p>800,00 $</p> </td> 
   <td> <p>0,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 4</p> </td> 
   <td> <p>Dép 2 Tâche 4</p> </td> 
   <td> <p>- 100,00 $</p> </td> 
   <td> <p>300,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 4 </p> </td> 
   <td> <p>Dép 3 Tâche 4</p> </td> 
   <td> <p>-200,00</p> </td> 
   <td> <p>0,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 5</p> </td> 
   <td> <p>Dép 1 Tâche 5</p> </td> 
   <td> <p>700,00 $</p> </td> 
   <td> <p>800,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 5</p> </td> 
   <td> <p>Dép 2 Tâche 5</p> </td> 
   <td> <p>- 100,00 $</p> </td> 
   <td> <p>300,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 5</p> </td> 
   <td> <p>Dép 3 Tâche 5</p> </td> 
   <td> <p>- 400,00 $</p> </td> 
   <td> <p>- 200,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 6</p> </td> 
   <td> <p>Dép 1 Tâche 6</p> </td> 
   <td> <p>600,00 $</p> </td> 
   <td> <p>700,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 6</p> </td> 
   <td> <p>Dép 2 Tâche 6</p> </td> 
   <td> <p>500,00 $</p> </td> 
   <td> <p>- 300,0 $</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Ajoutez deux dépenses au projet (c’est-à-dire non liées à une tâche) comme suit :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Dépense</strong> </p> </th> 
   <th> <p><strong>Montant prévu</strong> </p> </th> 
   <th> <p><strong>Montant réel</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Dép Projet 1</p> </td> 
   <td> <p>1 000,00 $</p> </td> 
   <td> <p>1 500,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Dép 2 Tâche 1</p> </td> 
   <td> <p>2 500,00 $</p> </td> 
   <td> <p> 0,00 $ <strong></strong></p> </td> 
  </tr> 
 </tbody> 
</table>

1. En fonction des valeurs ci-dessus, les coûts engagés/non engagés sont déterminés comme suit :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Tâche</strong> </p> </th> 
   <th> <p><strong>Dépenses prévues non engagées</strong> </p> </th> 
   <th> <p><strong>Dépenses prévues engagées</strong> </p> </th> 
   <th> <p><strong>Dépenses réelles engagées</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Tâche 1</p> </td> 
   <td> <p>400,00 $</p> </td> 
   <td> <p>- 500,00 $</p> </td> 
   <td> <p>800,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 2</p> </td> 
   <td> <p>- 400,00 $</p> </td> 
   <td> <p>300,00 $</p> </td> 
   <td> <p>1 300,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 3</p> </td> 
   <td> <p>0,00 $</p> </td> 
   <td> <p>0,00 $</p> </td> 
   <td> <p>1 000,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 4</p> </td> 
   <td> <p>600,00 $</p> </td> 
   <td> <p>- 100,00 $</p> </td> 
   <td> <p>300,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 5</p> </td> 
   <td> <p>0,00 $</p> </td> 
   <td> <p>600,00 $</p> </td> 
   <td> <p>1 100,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 6</p> </td> 
   <td> <p>0,00 $</p> </td> 
   <td> <p>600,00 $</p> </td> 
   <td> <p>700,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projet</p> </td> 
   <td> <p>2 500,00 $</p> </td> 
   <td> <p>1 000,00 $</p> </td> 
   <td> <p>1 500,00 $</p> </td> 
  </tr> 
 </tbody> 
</table>

1. À partir des actions du projet, exécuter Recalculer finances
1. **ICP** pour la tâche 2 = 0,17 calculé comme suit :\
   **Tâche IPC 2** = *IF* Coût réel de la main-d&#39;œuvre + IncurredActualExpenseCost &lt;> 0 *THEN* IPC = (TotalBudgetedCostWorkPerforming + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCostCost)
   * SINON* ICP = CPI_Labor\
     **ICP****Tâche 2** = (100+300) / (1 000+1 300)\
     **ICP****Tâche 2** = 400/2300\
     **ICP****Tâche 2** = .17

1. **EAC** pour la tâche 2 = 5 900,00 $\
   **Main-d’oeuvre ICP****Tâche 2** = IF Coût réel de main-d’oeuvre &lt;> 0 THEN CPI_Labor = Coût budgété du travail effectué / Coût réel de main-d’oeuvre\
   SINON CPI_Labor = 1\
   **Main-d’oeuvre ICP****Tâche 2** = 100/1 000\
   **Main-d’oeuvre ICP****Tâche 2** = 0,1

   **Main-d’oeuvre EAC****Tâche 2** = *IF* CPI_Labor &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost/CPI_Labor
   ```

   * SINON* CRE Main-d&#39;œuvre = Coût prévu de main-d&#39;œuvre + Coût réel de main-d&#39;œuvre\
     **Main-d’oeuvre EAC****Tâche 2** = 500,00/0,1\
     **Main-d’oeuvre EAC****Tâche 2** = 5 000,00 $****** Dépenses EAC ****Tâche 2 **= Coût des dépenses réelles engagées + Coût des dépenses prévues non engagées\
     **Dépenses EAC ****Tâche 2** = 1 300,00 $ + - 400,00 $\
     **Dépenses EAC****Tâche 2** = 900,00 $

   **EAC****Tâche 2** = Main-d’oeuvre EAC + Dépenses EAC\
   **CRE****Tâche 2** = 5 000 $ + 900 $\
   **CRE****Tâche 2** = 5 900 $

1. L’ICP et l’EAC pour les tâches 4, 5 et 6 sont déterminés de la même manière. Je vais donc simplement fournir les valeurs ci-dessous :\
   Tâche 4 : 0,23 / 3 400,00 $\
   Tâche 5 : 0,64 / 3 100,00 $\
   Tâche 6 : 1,06 / 2 366,67 $

1. ICP pour la tâche 3 = 0,31 calculé comme suit :\
   **CPI****Tâche 3** = *IF* Coût réel de la main-d&#39;œuvre + IncurredActualExpenseCost &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   * SINON* ICP = CPI_Labor\
     **IPC****tâche 3** = (1 150 + 500) / (3 000 + 2 400)\
     **ICP****Tâche 3** = 1 650/5 400\
     **ICP****Tâche 3** = .31 ****** CRE pour la Tâche 3 **= 9 521,74 $ calculé comme suit :\
     **Main-d’œuvre ICP ****Tâche 3** = IF Coût réel de main-d’œuvre &lt;> 0 THEN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

   SINON CPI_Labor = 1\
   **Main-d’œuvre ICP****Tâche 3** = 1 150/3 000\
   **Main-d’œuvre ICP****Tâche 3** = 0,383333\
   **Main-d’œuvre ICP****Tâche 3** = 0,38

   **Main-d’œuvre EAC****Tâche 3** = *IF* CPI_Labor &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   * SINON* CRE Main-d&#39;œuvre = Coût prévu de main-d&#39;œuvre + Coût réel de main-d&#39;œuvre\
     **Main-d’œuvre EAC****Tâche 3** = 2 500,00 $ / 0,383333\
     **EAC de main d’oeuvre****Tâche 3** = 6 521,74 $

   **EAC des dépenses***Tâche 3** = Coût des dépenses réelles engagées + Coût des dépenses prévues non engagées\
   **EAC des dépenses****Tâche 3** = 2 400 $ + 600 $\
   **EAC des dépenses****Tâche 3** = 3 000 $

   **EAC des dépenses****Tâche 3** = EAC de main d’œuvre + EAC des dépenses\
   **CRE****Tâche 3** = 6 521,74 $ + 3 000,00 $\
   **CRE****tâche 3** = 9 521,74 $

1. ICP de la tâche 1 = 0,16 calculé comme suit :\
   **CPI****Tâche 1** = *IF* Coût réel de la main-d&#39;œuvre + IncurredActualExpenseCost &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   * SINON* ICP = CPI_Labor\
     **ICP****Tâche 1** = (1 250 + 300) / (5 000 + 4 500)\
     **ICP****Tâche 1** = 1 550 / 9 500=\
     **ICP****Tâche 1** = .16

1. L’EAC de la tâche 1 est de 17 100 $, calculé comme suit :\
   **ICP de main-d’œuvre****Tâche 1** = IF Coût réel de main-d’œuvre &lt;> 0 THEN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

   SINON CPI_Labor = 1\
   **ICP de main-d’œuvre****Tâche 1** = 1 250 / 5 000\
   **ICP de main-d’œuvre****Tâche 1** = 0,25

   **EAC de main-d’œuvre****Tâche 1** = *IF* CPI_Labor &lt;> 0 *THEN* EAC de main-d’œuvre = Coût prévu de main-d’œuvre / CPI_Labor
   * SINON* CRE Main-d&#39;œuvre = Coût prévu de main-d&#39;œuvre + Coût réel de main-d&#39;œuvre\
     **EAC de main-d’œuvre****Tâche 1** = 3 000,00 $ / 0,25\
     **EAC de main-d’œuvre****Tâche 1** = 12 000 $

   **EAC des dépenses****Tâche 1** = Coût des dépenses réelles engagées + Coût des dépenses prévues non engagées\
   **EAC des dépenses****Tâche 1** = 4 500 $ + 600 $\
   **EAC des dépenses****Tâche 1** = 5 100,00 $

   **EAC****Tâche 1** = EAC de main-d’oeuvre + EAC des dépenses\
   **CRE****Tâche 1** = 12 000 $ + 5 100 $\
   **CRE****Tâche 1** = 17 100 $

1. L’ICP du projet est de 0,25.\
   **ICP****pour le projet** = *IF* Coût réel de la main-d’œuvre + IncurredActualExpenseCost &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   * SINON* ICP = CPI_Labor

   **ICP****du projet** = (2 450 + 1 900) / (11 000 + 6 700)\
   **ICP****pour le projet** =   4350 / 17700\
   **ICP****du projet** = 0,25

1. **EAC du projet** = 32 248,98 $ calculé comme suit :\
   **ICP du coût de main-d’œuvre****pour le projet** = IF Coût réel de main-d’œuvre &lt;> 0 THEN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

   SINON CPI_Labor = 1\
   **ICP du coût de main-d’œuvre****pour le projet** = 2 450 / 11 000\
   **ICP du coût de main-d’œuvre****pour le projet** = 0,22272\
   **ICP du coût de main-d’œuvre****pour le projet** = 0,22

   **EAC de main-d’œuvre****pour le projet** = *IF* CPI_Labor &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   * SINON* CRE Main-d&#39;œuvre = Coût prévu de main-d&#39;œuvre + Coût réel de main-d&#39;œuvre\
     **EAC de main-d’œuvre****pour le projet** = 5 000,00 $ / 0,22272\
     **EAC de main-d’œuvre****pour le projet** = 22 448,97959 $\
     **EAC de main-d’œuvre****pour le projet** = 22 448,98 $

   **EAC des dépenses****pour le projet** = Coût des dépenses réelles engagées + Coût des dépenses prévues non engagées\
   **EAC des dépenses****pour le projet** = 3 100 $ + 6 700 $\
   **EAC des dépenses****pour le projet** = 9 800 $

   **EAC****pour le projet** = EAC de main-d’oeuvre + EAC des dépenses\
   **CRE****Projet** = 22 448,98 $ + 9 800,00 $\
   **CRE****Projet** = 32 248,98 $
