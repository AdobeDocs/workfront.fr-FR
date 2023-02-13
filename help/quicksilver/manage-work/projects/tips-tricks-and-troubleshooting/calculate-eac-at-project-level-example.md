---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: Exemple de calcul - calculer le taux d’effet élévateur au niveau du projet
description: PIM = Basé sur l’heure
author: Alina
feature: Work Management
exl-id: ff88b7e3-2a5b-464f-bed1-6848067840b8
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '1768'
ht-degree: 9%

---

# Exemple de calcul - calculer le taux d’effet élévateur au niveau du projet

## Méthode EAC : Calculer au niveau du projet

* [PIM = Basé sur l’heure](#pim-hour-based)
* [PIM = Basé sur les coûts](#pim-cost-based)

### PIM = Basé sur l’heure {#pim-hour-based}

* [Exemple simple : projet n’a aucune tâche enfant](#simple-example-project-has-no-children-tasks)
* [Exemple complexe : projet comporte des tâches enfants](#complicated-example-project-has-children-tasks)

#### Exemple simple : projet n’a aucune tâche enfant {#simple-example-project-has-no-children-tasks}

PIM = Basé sur l’heure

Méthode EAC = Calcul au niveau du projet ****

1. Créez le projet A avec trois tâches (aucune tâche enfant) affectées à l’utilisateur 1 dont le coût/heure est de 100,00 $.
1. Ajoutez les heures planifiées et réelles à chaque tâche et % Terminé selon le tableau ci-dessous :

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
      <td><p>Tâche 1</p></td>
      <td><p>5 heures</p></td>
      <td><p>25 heures</p></td>
      <td><p>20%</p></td>
     </tr>
     <tr>
      <td><p>Tâche 2</p></td>
      <td><p>10 heures</p></td>
      <td><p>25 heures</p></td>
      <td><p>30%</p></td>
     </tr>
     <tr>
      <td><p>Tâche 3</p></td>
      <td><p>15 heures</p></td>
      <td><p>25 heures</p></td>
      <td><p>40%</p></td>
     </tr>
    </tbody>
   </table>

1. Recalculer la finance sur le projet.
1. **IPC pour la tâche 1** = .04 calculé comme suit :\
   **IPC pour la tâche 1** = *IF* Heures réelles > 0 *ALORS* IPC = TotalBudgetCostWorkPerformed/Heures réelles\
      *ELSE* IPC = 1\
   **IPC pour la tâche 1** = 1 / 25\
   **IPC pour la tâche 1** = 0,04

1. **CAE pour la tâche 1** = 125 heures calculées comme suit :\
   **CAE pour la tâche 1** = *IF* IPC &lt;> 0 *ALORS* CAE = Heures planifiées/IPC\
       *ELSE* EAC = Heures planifiées + Heures réelles\
   **CAE pour la tâche 1** = 5 / 0,04\
   **CAE pour la tâche 1** = 125 heures****

1. IPC/CAE pour les tâches 2 et 3 :\
   Tâche 2 = 0,12 / 83,33 heures\
   Tâche 3 = 0,24 / 62,5 heures

1. **IPC du projet** = .13 calculé comme suit :\
   **IPC du projet** = *IF* Heures réelles > 0 *ALORS* IPC = TotalBudgetCostWorkPerformed/Heures réelles\
       *ELSE* IPC = 1\
   **IPC du projet** = 10 / 75\
   **IPC du projet** = 0,13

1. **CAE pour le projet** = 225 heures calculées comme suit :\
   **CAE pour le projet** = *IF* IPC &lt;> 0 *ALORS* CAE = Heures planifiées/IPC\
       *ELSE* EAC = Heures planifiées + Heures réelles\
   **CAE pour le projet** = 30 / .13333\
   **CAE pour le projet** = 225 heures

#### Exemple complexe : projet comporte des tâches enfants {#complicated-example-project-has-children-tasks}

PIM = Basé sur l’heure

Méthode EAC = Calcul au niveau du projet

1. Créez le projet A avec six tâches pour lesquelles la tâche 3 est le parent des tâches 4 et 5 et la tâche 1 est le parent des tâches 2 et 3, comme illustré ci-dessous :\
   Tâche 1\
      Tâche 2\
      Tâche 3\
         Tâche 4\
         Tâche 5\
   Tâche 6

1. Affectez les tâches 2, 4, 5 et 6 à l’utilisateur 1 dont le coût/heure est de 100,00 $.
1. Ajoutez les heures planifiées/réelles pour chaque tâche et % Terminé selon le tableau ci-dessous.

   >[!NOTE]
   >
   >Pour les tâches 1 et 3, vous n’ajoutez que des heures réelles.

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
   <th> <p><strong>% Terminé</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Tâche 1</p> </td> 
   <td> </td> 
   <td> <p>10 heures</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 2</p> </td> 
   <td> <p>5 heures</p> </td> 
   <td> <p>10 heures</p> </td> 
   <td> <p>20%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 3</p> </td> 
   <td> </td> 
   <td> <p>10 heures</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 4</p> </td> 
   <td> <p>10 heures</p> </td> 
   <td> <p>10 heures</p> </td> 
   <td> <p>40%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 5</p> </td> 
   <td> <p>15 heures</p> </td> 
   <td> <p>10 heures</p> </td> 
   <td> <p>50%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 6</p> </td> 
   <td> <p>20 heures</p> </td> 
   <td> <p>10 heures</p> </td> 
   <td> <p>60%</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Ajoutez 50 heures directement au projet (Plus>Heures>Heures de journal).
1. **IPC pour la tâche 2** = .1 calculé comme suit :\
   **IPC pour la tâche 2** = *IF* Heures réelles > 0 *ALORS* IPC = TotalBudgetCostWorkPerformed/Heures réelles\
       *ELSE* IPC = 1\
   **IPC pour la tâche 2** = 1 / 10\
   **IPC pour la tâche 2** = .1

1. **EAC pour la tâche 2** = 50 heures calculées comme suit :\
   **EAC pour la tâche 2** = *IF* IPC &lt;> 0 *ALORS* CAE = Heures planifiées/IPC\
       *ELSE* EAC = Heures planifiées + Heures réelles\
   **EAC pour la tâche 2** = 5 / .1\
   **EAC pour la tâche 2** = 50 heures

1. L’IPC/le CAE pour les tâches 4, 5 et 6 sont les suivants :\
   Tâche 4 : .4 / 25 heures\
   Tâche 5 : .75 / 20 heures\
   Tâche 6 : 1.2 / 16.67 heures

1. **IPC pour la tâche 3** = .38 calculé comme suit :\
   **IPC pour la tâche 3** = *IF* Heures réelles > 0 *ALORS* IPC = TotalBudgetCostWorkPerformed/Heures réelles\
       *ELSE* IPC = 1\
   **IPC pour la tâche 3** = 11,5 / 30\
   **IPC pour la tâche 3** = 0,38

1. **EAC pour la tâche 3** = 65,22 heures calculées comme suit :\
   **EAC pour la tâche 3** = *IF* IPC &lt;> 0 *ALORS* CAE = Heures planifiées/IPC\
       *ELSE* EAC = Heures planifiées + Heures réelles\
   **EAC pour la tâche 3** = 25 / .383333\
   **EAC pour la tâche 3** = 65,22 heures

1. **IPC pour la tâche 1** = 0,25 calculé comme suit :\
   **IPC pour la tâche 1** = *IF* Heures réelles > 0 *ALORS* IPC = TotalBudgetCostWorkPerformed/Heures réelles\
       *ELSE* IPC = 1\
   **IPC pour la tâche 1** = 12,5 / 50\
   **IPC pour la tâche 1** = 0,25

1. **CAE pour la tâche 1** = 120 heures calculées comme suit :\
   **CAE pour la tâche 1** = *IF* IPC &lt;> 0 *ALORS* CAE = Heures planifiées / IPC\
       *ELSE* EAC = Heures planifiées + Heures réelles\
   **CAE pour la tâche 1** = 30/ .25\
   **CAE pour la tâche 1** = 120 heures

1. **IPC du projet** = 0,22 calculé comme suit :\
   **IPC du projet** = *IF* Heures réelles > 0 *ALORS* IPC = TotalBudgetCostWorkPerformed/Heures réelles\
       *ELSE* IPC = 1\
   **IPC du projet** = 24,5 / 110\
   **IPC du projet** = 0,22272\
   **IPC du projet** = 0,22

1. **CAE pour le projet** = 224,49 heures calculées comme suit :\
   **CAE pour le projet** = *IF* IPC &lt;> 0 *ALORS* CAE = Heures planifiées/IPC\
       *ELSE* EAC = Heures planifiées + Heures réelles\
   **CAE pour le projet** = 50 / .22272\
   **CAE pour le projet** = 224,49 heures

### PIM = Basé sur les coûts {#pim-cost-based}

* [Exemple simple : projet n’a aucune tâche enfant](#simple-example-project-has-no-children-tasks)
* [Exemple complexe : projet comporte des tâches enfants](#complicated-example-project-has-children-tasks)

#### Exemple simple : projet n’a aucune tâche enfant {#simple-example-project-has-no-children-tasks-1}

PIM = Basé sur les coûts

Méthode EAC = Calcul au niveau du projet

1. Créez le projet A avec trois tâches (aucune tâche enfant) affectées à l’utilisateur 1 dont le coût/heure est de 100,00 $.
1. Ajoutez les heures prévues/réelles à chaque tâche et % Terminé selon le tableau ci-dessous :

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
   <th> <br> <p><strong>Coût Lbr de plan</strong> </p> </th> 
   <th> <br> <p><strong>Hrs eff</strong> </p> </th> 
   <th> <br> <p><strong>Coût réel des actes</strong> </p> </th> 
   <th> <p><strong>% Terminé</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Tâche 1</p> </td> 
   <td> <p>5 heures</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>25 heures</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p>20%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 2</p> </td> 
   <td> <p>10 heures</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>25 heures</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p>30%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 3</p> </td> 
   <td> <p>15 heures</p> </td> 
   <td> <p>$1,500.00</p> </td> 
   <td> <p>25 heures</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p>40%</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Ajoutez des dépenses à chaque tâche en fonction du tableau ci-dessous :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Tâche</strong> </p> </th> 
   <th> <p><strong>Frais</strong> </p> </th> 
   <th> <p><strong>Montant prévu</strong> </p> </th> 
   <th> <p><strong>Montant réel</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Tâche 1</p> </td> 
   <td> <p>Tâche 1 Exp 1</p> </td> 
   <td> <p>$300.00</p> </td> 
   <td> <p>$400.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 1</p> </td> 
   <td> <p>Tâche 1 Exp 2</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>$0.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 2</p> </td> 
   <td> <p>Task 2 Exp</p> </td> 
   <td> <p>$200.00</p> </td> 
   <td> <p>$100.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 3</p> </td> 
   <td> <p>Task 3 Exp</p> </td> 
   <td> <p>$800.00</p> </td> 
   <td> <p>$700.00</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Ajoutez deux dépenses au projet (c’est-à-dire non liées à une tâche) comme suit :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Frais</strong> </p> </th> 
   <th> <p><strong>Montant prévu</strong> </p> </th> 
   <th> <p><strong>Montant réel</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Project Exp 1</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>$1,500.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 1 Exp 2</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p>$0.00</p> </td> 
  </tr> 
 </tbody> 
</table>

1. En fonction des valeurs ci-dessus, les coûts engendrés/non générés sont déterminés comme suit :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Tâche</strong> </p> </th> 
   <th> <p><strong>Dépenses prévues non engagées</strong> </p> </th> 
   <th> <p><strong>Dépenses prévues encourues</strong> </p> </th> 
   <th> <p><strong>Dépenses réelles encourues</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Tâche 1</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>$300.00</p> </td> 
   <td> <p>$400.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 2</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$200.00</p> </td> 
   <td> <p>$100.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 3</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$800.00</p> </td> 
   <td> <p>$700.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projet</p> </td> 
   <td> <p>$3,000.00</p> </td> 
   <td> <p>$2,300.00</p> </td> 
   <td> <p> $2,700.00 <strong></strong></p> </td> 
  </tr> 
 </tbody> 
</table>

1. À partir des actions du projet, exécutez Recalculer Finance
1. **IPC pour la tâche 1** = 0,14
1. **IPC****pour la tâche 1** = .14 calculé comme suit :\
   **IPC**  **pour la tâche 1** = *IF* Coût réel de la main-d’oeuvre + InferredRepenseCost &lt;> 0 *ALORS*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   *    ELSE* IPC = IPC_Travail\
   **IPC****pour la tâche 1** = (100+300) / (2 500+400)\
   **IPC**  **pour la tâche 1** = 400 / 2 900\
   **IPC**  **pour la tâche 1**  = 0,14****

1. **EAC**** pour la tâche 1** = 13 400,00 $\
   **Travail CPI**  **pour la tâche 1** = SI Coût réel du travail &lt;> 0 ALORS

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed/Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **Travail CPI**  **pour la tâche 1** = 100/2500\
   **Travail CPI**  **pour la tâche 1** = 0,04 ****** EAC Labor ****pour la tâche 1 **=*IF *CPI_Labor &lt;> 0*ALORS *Main-d’oeuvre du CCE = Coût du travail prévu/IPC_Travail\
   *    ELSE* Main-d’oeuvre du CCE = Coût de main-d’oeuvre planifié + coût de main-d’oeuvre réel\
   **Travail EAC ****pour la tâche 1** = 500.00/.04\
   **EAC Labor****pour la tâche 1** = 12 500,00 $\
   **Dépenses EAC****pour la tâche 1** = InferredRepenseCost + NotInferredScheduleExpense\
   **Dépenses EAC****pour la tâche 1** = 400,00 $ + 500,00 $\
   **Dépenses EAC****pour la tâche 1** = 900,00 $\
   **EAC**** pour la tâche 1** = Main-d’oeuvre du CCE + Dépenses du CCE\
   **EAC**** pour la tâche 1**  = 12 500,00 $ + 900,00 $\
   **EAC**** pour la tâche 1**  = 13 400,00 $

1. Voici les valeurs IPC/CAE pour la tâche 2 et la tâche 3 :\
   Tâche 2 = 0,19 / 8 433,33 $\
   Tâche 3 = 0,44 / 6 950,00 $

1. **IPC du projet** = .32 calculé comme suit :\
   **IPC****pour le projet** = *IF* Coût réel de la main-d’oeuvre + InferredRepenseCost &lt;> 0 *ALORS*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* IPC = IPC_Travail\
   **IPC****pour le projet** = (1 000 + 2 300) / (7 500 + 2 700)\
   **IPC****pour le projet** = 3300 / 10200\
   **IPC****pour le projet** = 0,32

1. **CAE pour le projet** = 28 200,00 $ calculé comme suit :\
   **Travail IPC****pour le projet** = SI Coût réel du travail &lt;> 0 ALORS

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed/Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **Travail IPC****pour le projet** = 1 000 / 7 500\
   **Travail IPC****pour le projet** = 0,13333\
   **Travail IPC****pour le projet** = 0,13

   **EAC Labor****pour le projet** = *IF* CPI_Labor &lt;> 0 *ALORS*

   ```
   EAC Labor = Planned Labor Cost/CPI_Labor
   ```

   *   ELSE* Main-d’oeuvre du CCE = Coût de main-d’oeuvre planifié + coût de main-d’oeuvre réel\
   **EAC Labor****pour le projet** = 3 000/ .13 333\
   **EAC Labor****pour le projet** = 22 500,00 $

   **EAC Expense****Project** =

   ```
   IncurredActualExpenseCost + NotIncurredPlannedExpense
   ```

   **EAC Expense****Project** = 3 000,00 $ + 2 700,00 $\
   **EAC Expense****Project** = 5 700,00 $

   **EAC****Project** = Main-d’oeuvre du CCE + Dépenses du CCE\
   **EAC****Project**  = 22 500,00 $ + 5 700,00 $\
   **EAC****Project**  = 28 200,00 $

#### Exemple complexe : projet comporte des tâches enfants {#complicated-example-project-has-children-tasks-1}

PIM = Basé sur les coûts

Méthode EAC = Calcul au niveau du projet

1. Créez le projet A avec six tâches pour lesquelles la tâche 3 est le parent des tâches 4 et 5 et la tâche 1 est le parent des tâches 2 et 3, comme illustré ci-dessous :\
   Tâche 1\
      Tâche 2\
      Tâche 3\
         Tâche 4\
         Tâche 5\
   Tâche 6

1. Affectez les tâches 2, 4, 5 et 6 à l’utilisateur 1 dont le coût/heure est de 100,00 $.
1. Ajoutez les heures planifiées/réelles pour chaque tâche et % Terminé selon le tableau ci-dessous.

   >[!NOTE]
   >
   >Pour les tâches 1 et 3, vous n’ajoutez que des heures réelles.

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
   <th> <br> <p><strong>Coût Lbr de plan</strong> </p> </th> 
   <th> <br> <p><strong>Hrs eff</strong> </p> </th> 
   <th> <br> <p><strong>Coût réel des actes</strong> </p> </th> 
   <th> <p><strong>% Terminé</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Tâche 1</p> </td> 
   <td> </td> 
   <td> </td> 
   <td> <p>10 heures</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 2</p> </td> 
   <td> <p>5 heures</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>10 heures</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>20%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 3</p> </td> 
   <td> </td> 
   <td> </td> 
   <td> <p>10 heures</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 4</p> </td> 
   <td> <p>10 heures</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>10 heures</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>40%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 5</p> </td> 
   <td> <p>15 heures</p> </td> 
   <td> <p>$1,500.00</p> </td> 
   <td> <p>10 heures</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>50%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 6</p> </td> 
   <td> <p>20 heures</p> </td> 
   <td> <p>$2,000.00</p> </td> 
   <td> <p>10 heures</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>60%</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Ajoutez 50 heures directement au projet (Plus > Heures > Heures de journal) afin d’obtenir 5 000 $ de coût réel de la main-d’oeuvre directement dans le projet. ****
1. Ajoutez des dépenses à chaque tâche en fonction du tableau ci-dessous (j’ai ajouté une ligne vide entre chaque tâche pour faciliter la lecture) :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Tâche</strong> </p> </th> 
   <th> <p><strong>Frais</strong> </p> </th> 
   <th> <p><strong>Montant prévu</strong> </p> </th> 
   <th> <p><strong>Montant réel</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Tâche 1</p> </td> 
   <td> <p>Tâche 1 Exp 1</p> </td> 
   <td> <p>$300.00</p> </td> 
   <td> <p>-$400.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 1</p> </td> 
   <td> <p>Tâche 1 Exp 2</p> </td> 
   <td> <p>-$500.00</p> </td> 
   <td> <p>$800.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 1</p> </td> 
   <td> <p>Tâche 1 Exp 3</p> </td> 
   <td> <p>$400.00</p> </td> 
   <td> <p>$0.00</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 2</p> </td> 
   <td> <p>Tâche 2 Exp 1</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>$700.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 2</p> </td> 
   <td> <p>Tâche 2 Exp 2</p> </td> 
   <td> <p>-$400.00</p> </td> 
   <td> <p>$0.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 2</p> </td> 
   <td> <p>Tâche 2 Exp 3</p> </td> 
   <td> <p>-$200.00</p> </td> 
   <td> <p>$600.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 2</p> </td> 
   <td> <p>Tâche 2 Exp 4</p> </td> 
   <td> <p>$700.00</p> </td> 
   <td> <p>-$200.00</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 3</p> </td> 
   <td> <p>Task 3 Exp</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$1,000.00</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 4</p> </td> 
   <td> <p>Tâche 4 Exp 1</p> </td> 
   <td> <p>$800.00</p> </td> 
   <td> <p>$0.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 4</p> </td> 
   <td> <p>Tâche 4 Exp 2</p> </td> 
   <td> <p>-$100.00</p> </td> 
   <td> <p>$300.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 4 </p> </td> 
   <td> <p>Tâche 4 Exp 3</p> </td> 
   <td> <p>-200.00</p> </td> 
   <td> <p>$0.00</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 5</p> </td> 
   <td> <p>Tâche 5 Exp 1</p> </td> 
   <td> <p>$700.00</p> </td> 
   <td> <p>$800.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 5</p> </td> 
   <td> <p>Tâche 5 Exp 2</p> </td> 
   <td> <p>-$100.00</p> </td> 
   <td> <p>$300.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 5</p> </td> 
   <td> <p>Tâche 5 Exp. 3</p> </td> 
   <td> <p>-$400.00</p> </td> 
   <td> <p>-$200.00</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 6</p> </td> 
   <td> <p>Tâche 6 Exp 1</p> </td> 
   <td> <p>$600.00</p> </td> 
   <td> <p>$700.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 6</p> </td> 
   <td> <p>Tâche 6 Exp 2</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>-$300.0</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Ajoutez deux dépenses au projet (c’est-à-dire non liées à une tâche) comme suit :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Frais</strong> </p> </th> 
   <th> <p><strong>Montant prévu</strong> </p> </th> 
   <th> <p><strong>Montant réel</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Project Exp 1</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>$1,500.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 1 Exp 2</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p> $0.00 <strong></strong></p> </td> 
  </tr> 
 </tbody> 
</table>

1. En fonction des valeurs ci-dessus, les coûts engendrés/non générés sont déterminés comme suit :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Tâche</strong> </p> </th> 
   <th> <p><strong>Dépenses prévues non engagées</strong> </p> </th> 
   <th> <p><strong>Dépenses prévues encourues</strong> </p> </th> 
   <th> <p><strong>Dépenses réelles encourues</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Tâche 1</p> </td> 
   <td> <p>$400.00</p> </td> 
   <td> <p>-$500.00</p> </td> 
   <td> <p>$800.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 2</p> </td> 
   <td> <p>-$400.00</p> </td> 
   <td> <p>$300.00</p> </td> 
   <td> <p>$1,300.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 3</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$1,000.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 4</p> </td> 
   <td> <p>$600.00</p> </td> 
   <td> <p>-$100.00</p> </td> 
   <td> <p>$300.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 5</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$600.00</p> </td> 
   <td> <p>$1,100.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 6</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$600.00</p> </td> 
   <td> <p>$700.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projet</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p>$1000.00</p> </td> 
   <td> <p>$1,500.00</p> </td> 
  </tr> 
 </tbody> 
</table>

1. À partir des actions du projet, exécutez Recalculer Finance
1. **IPC** pour la tâche 2 = 0,17 calculé comme suit :\
   **Tâche IPC 2** = *IF* Coût réel de la main-d’oeuvre + InferredRepenseCost &lt;> 0 *ALORS* IPC = (TotalBudgetedCostWorkPerformed + InferredScheduleExpenseCost) / (CoûtTravailRéel + CoûtRéelDépensesCoût)\
   *   ELSE* IPC = IPC_Travail\
   **IPC****Task 2** = (100+300) / (1000+1300)\
   **IPC****Task 2**  = 400 / 2 300\
   **IPC****Task 2**  = 0,17

1. **EAC** pour la tâche 2 = 5 900,00 $\
   **Tâche d’utilisation du IPC****Tâche 2** = SI Coût réel de la main-d’oeuvre &lt;> 0 ALORS IPC_Travail = TotalBudgetCostWorkPerformed / Coût réel de la main-d’oeuvre\
      ELSE CPI_Labor = 1\
   **Tâche d’utilisation du IPC****Tâche 2** = 100/1000\
   **Tâche d’utilisation du IPC****Tâche 2** = .1

   **EAC Labor****Task 2** = *IF* CPI_Labor &lt;> 0 *ALORS*

   ```
   EAC Labor = Planned Labor Cost/CPI_Labor
   ```

   *   ELSE* Main-d’oeuvre du CCE = Coût de main-d’oeuvre planifié + coût de main-d’oeuvre réel\
   **EAC Labor****Task 2** = 500,00/.1\
   **EAC Labor****Task 2** = 5 000,00 $****** Dépenses EAC ****Tâche 2 **= InferredRepenseCost + NotInferredScheduleExpense\
   **Frais de contrôle d’accès ****Tâche 2** = 1 300 $ + - 400 $\
   **EAC Expense****Task 2** = 900,00 $

   **EAC****Task 2** = Main-d’oeuvre du CCE + Dépenses du CCE\
   **EAC****Task 2**  = 5 000,00 $ + 900,00 $\
   **EAC****Task 2**  = 5 900,00 $

1. L’IPC/le CAE pour les tâches 4, 5 et 6 sont déterminés de la même manière. Je vais donc simplement fournir les valeurs ci-dessous :\
   Tâche 4 : .23 / 3 400,00 $\
   Tâche 5 : .64 / 3 100,00 $\
   Tâche 6 : 1,06 / 2 366,67 $

1. IPC pour la tâche 3 = 0,31 calculé comme suit :\
   **IPC****Task 3** = *IF* Coût réel de la main-d’oeuvre + InferredRepenseCost &lt;> 0 *ALORS*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* IPC = IPC_Travail\
   **IPC****Task 3**  = (1 150 + 500) / (3 000 + 2 400)\
   **IPC****Task 3**  = 1 650 / 5 400\
   **IPC****Task 3**  = 0,31 ****** EAC pour la tâche 3 **= 9 521,74 $ calculé comme suit :\
   **Travail CPI ****Tâche 3** = SI Coût réel du travail &lt;> 0 ALORS

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **Tâche d’utilisation du IPC****Tâche 3** = 1150/3000\
   **Tâche d’utilisation du IPC****Tâche 3** = .383333\
   **Tâche d’utilisation du IPC****Tâche 3** = 0,38

   **EAC Labor****Task 3** = *IF* CPI_Labor &lt;> 0 *ALORS*

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   *   ELSE* Main-d’oeuvre du CCE = Coût de main-d’oeuvre planifié + coût de main-d’oeuvre réel\
   **EAC Labor****Task 3** = 2 500,00 $ / .383333\
   **EAC Labor****Task 3** = 6 521,74 $

   **EAC Expense****Task 3** = InferredRepenseCost + NotInferredScheduleExpense\
   **EAC Expense****Task 3** = 2 400,00 $ + 600,00 $\
   **EAC Expense****Task 3** = 3 000,00 $

   **EAC****Task 3** = Main-d’oeuvre du CCE + Dépenses du CCE\
   **EAC****Task 3**  = 6 521,74 $ + 3 000 $\
   **EAC****Task 3**  = 9 521,74 $

1. IPC pour la tâche 1 = 0,16 calculé comme suit :\
   **IPC****Task 1** = *IF* Coût réel de la main-d’oeuvre + InferredRepenseCost &lt;> 0 *ALORS*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* IPC = IPC_Travail\
   **IPC****Task 1**  = (1 250 + 300) / (5 000 + 4 500)\
   **IPC****Task 1**  = 1550 / 9500=\
   **IPC****Task 1**  = 0,16

1. Le CAE pour la tâche 1 est de 17 100 $, calculé comme suit :\
   **Tâche du IPC****Tâche 1** = SI Coût réel du travail &lt;> 0 ALORS

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **Tâche du IPC****Tâche 1** = 1 250 / 5 000\
   **Tâche du IPC****Tâche 1** = 0,25

   **EAC Labor****Task 1** = *IF* CPI_Labor &lt;> 0 *ALORS* Main-d’oeuvre du CCE = Coût du travail planifié / IPC_Travail\
   *   ELSE* Main-d’oeuvre du CCE = Coût de main-d’oeuvre planifié + coût de main-d’oeuvre réel\
   **EAC Labor****Task 1** = 3 000,00 $ / 0,25\
   **EAC Labor****Task 1** = 12 000,00 $

   **Frais EAC****Tâche 1** = InferredRepenseCost + NotInferredScheduleExpense\
   **Frais EAC****Tâche 1** = 4 500 $ + 600 $\
   **Frais EAC****Tâche 1** = 5 100,00 $

   **EAC****Task 1** = Main-d’oeuvre du CCE + Dépenses du CCE\
   **EAC****Task 1**  = 12 000,00 $ + 5 100,00 $\
   **EAC****Task 1**  = 17 100,00 $

1. Le IPC du projet est de 0,25\
   **IPC****pour le projet** = *IF* Coût réel de la main-d’oeuvre + InferredRepenseCost &lt;> 0 *ALORS*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* IPC = IPC_Travail

   **IPC****pour le projet** = (2450 + 1900) / (11 000 + 6700)\
   **IPC****pour le projet** = 4350 / 17700\
   **IPC****pour le projet** = 0,25

1. **CAE pour le projet** = 32 248,98 $ calculé comme suit :\
   **Travail IPC****pour le projet** = SI Coût réel du travail &lt;> 0 ALORS

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **Travail IPC****pour le projet** = 2 450 / 1 1 000\
   **Travail IPC****pour le projet** = 0,22272\
   **Travail IPC****pour le projet** = 0,22

   **EAC Labor****pour le projet** = *IF* CPI_Labor &lt;> 0 *ALORS*

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   *   ELSE* Main-d’oeuvre du CCE = Coût de main-d’oeuvre planifié + coût de main-d’oeuvre réel\
   **EAC Labor****pour le projet** = 5 000,00 $ / .22272\
   **EAC Labor****pour le projet** = 22 448,97959 $\
   **EAC Labor****pour le projet** = 22 448,98 $

   **EAC Expense****Project** = InferredRepenseCost + NotInferredScheduleExpense\
   **EAC Expense****Project** = 3 100,00 $ + 6 700,00 $\
   **EAC Expense****Project** = 9 800,00 $

   **EAC****Project** = Main-d’oeuvre du CCE + Dépenses du CCE\
   **EAC****Project**  = 22 448,98 $ + 9 800,00 $\
   **EAC****Project**  = 32 248,98 $
