---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: Exemple de calcul - Calcul d’un EAC en tant que cumul à partir de tâches
description: PIM = Basé sur l’heure
author: Alina
feature: Work Management
exl-id: 68b582c9-f72a-4000-9d28-f7dafa23541f
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '873'
ht-degree: 8%

---

# Exemple de calcul - Calcul d’un EAC en tant que cumul à partir de tâches

## Méthode EAC : cumul à partir de tâches ou de sous-tâches

* [PIM = Basé sur l’heure](#pim-hour-based)
* [PIM = Basé sur les coûts](#pim-cost-based)

### PIM = Basé sur l’heure {#pim-hour-based}

* [Exemple simple : projet n’a aucune tâche enfant](#simple-example-project-has-no-children-tasks)
* [Exemple complexe : projet comporte des tâches enfants](#complicated-example-project-has-children-tasks)

#### Exemple simple : projet n’a aucune tâche enfant {#simple-example-project-has-no-children-tasks}

PIM = Basé sur l’heure

Méthode EAC = Cumul à partir de tâches/sous-tâches

1. Créez le projet A avec trois tâches (aucune tâche enfant) affectées à l’utilisateur 1 dont le coût/heure est de 100,00 $.
1. Ajoutez les heures prévues/réelles à chaque tâche et % Terminé selon le tableau ci-dessous :

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
   <td> <p>5 heures</p> </td> 
   <td> <p>25 heures</p> </td> 
   <td> <p>20%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 2</p> </td> 
   <td> <p>10 heures</p> </td> 
   <td> <p>25 heures</p> </td> 
   <td> <p>30%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 3</p> </td> 
   <td> <p>15 heures</p> </td> 
   <td> <p>25 heures</p> </td> 
   <td> <p>40%</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Recalculer finances
1. **IPC pour la tâche 1** = .04 calculé comme suit :\
   **IPC pour la tâche 1** = *IF* Heures réelles > 0 *ALORS* IPC = TotalBudgetCostWorkPerformed/Heures réelles\
       *ELSE* IPC = 1\
   **IPC pour la tâche 1** = 1 / 25\
   **IPC pour la tâche 1** = 0,04

1. **CAE pour la tâche 1** = 125 heures calculées comme suit :\
   **CAE pour la tâche 1** = *IF* IPC &lt;> 0 *ALORS* CAE = Heures prévues/IPC\
       *ELSE*

   ```
   EAC = Planned  Hours + Actual  Hours
   ```

   **CAE pour la tâche 1** = 5 / 0,04\
   **CAE pour la tâche 1** = 125 heures

1. IPC/CAE pour les tâches 2 et 3 :\
   Tâche 2 = 0,12 / 83,33 heures\
   Tâche 3 = 0,24 / 62,5 heures

1. **IPC du projet** = .13 calculé comme suit :\
   **IPC du projet** = *IF* Heures réelles > 0 *ALORS*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* IPC = 1\
   **IPC du projet** = 10 / 75\
   **IPC du projet** = 0,13

1. **CAE pour le projet** = 270,83 heures calculées comme suit\
   **CAE pour le projet** = Tâche EAC 1 + Tâche EAC 2 + Tâche EAC 3\
   **CAE pour le projet** = 125 + 83,33 + 62,5\
   **CAE pour le projet** = 270,83 heures

#### Exemple complexe : projet comporte des tâches enfants {#complicated-example-project-has-children-tasks}

PIM = Basé sur l’heure

Méthode EAC = Cumul à partir de tâches/sous-tâches

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

1. Ajoutez 50 heures directement au projet (Plus > Heures > Heures de journal) afin d’obtenir 5 000 $ de coût réel de la main-d’oeuvre directement dans le projet.
1. Exécuter Recalculer Finance
1. **IPC pour la tâche 2** = .1 calculé comme suit :\
   **IPC pour la tâche 2** = *IF* Heures réelles > 0 *ALORS*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* IPC = 1\
   **IPC pour la tâche 2** = 1 / 10\
   **IPC pour la tâche 2** = .1

1. **EAC pour la tâche 2** = 50 heures calculées comme suit :\
   **EAC pour la tâche 2** = *IF* IPC &lt;> 0 *ALORS*

   ```
   EAC = Planned Hours / CPI
   ```

       *ELSE* EAC = Heures planifiées + Heures réelles\
   **EAC pour la tâche 2** = 5 / .1\
   **EAC pour la tâche 2** = 50 heures

1. IPC/CAE pour la tâche 4, la tâche 5 et la tâche 6 :\
   Tâche 4 = 0,4 / 25 heures\
   Tâche 5 = 0,75 / 20 heures\
   Tâche 6 = 1,2 / 16,67 heures

1. **IPC pour la tâche 3** = 0,38\
   **IPC pour la tâche 3** = *IF* Heures réelles > 0 *ALORS*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* IPC = 1\
   **IPC pour la tâche 3** = 11,5 / 30\
   **IPC pour la tâche 3** = 0,38

1. **EAC pour la tâche 3** = Tâche EAC 4 + Tâche EAC 5\
   **EAC pour la tâche 3** = 25 + 20\
   **EAC pour la tâche 3** = 45 heures

1. **IPC pour la tâche 1** = 0,25 calculé comme suit :\
   **IPC pour la tâche 1** = *IF* Heures réelles > 0 *ALORS*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* IPC = 1\
   **IPC pour la tâche 1** = 12,5 / 50\
   **IPC pour la tâche 1** = 0,25

1. **CAE pour la tâche 1** = Tâche EAC 2 + Tâche EAC 3\
   **CAE pour la tâche 1** = 50 + 45\
   **CAE pour la tâche 1** = 95 heures

1. IPC du projet = 0,22 calculé comme suit :\
   **IPC du projet** = *IF* Heures réelles > 0 *ALORS*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* IPC = 1\
   **IPC du projet** = 24,5 / 110\
   **IPC du projet** = 0,22272\
   **IPC du projet** = 0,22

1. **AEE du projet** = Tâche EAC 1 + Tâche EAC 6\
   **AEE du projet** = 95 + 16,67\
   **AEE du projet** = 111,67 heures

### PIM = Basé sur les coûts {#pim-cost-based}

* [Exemple simple : projet n’a aucune tâche enfant](#simple-example-project-has-no-children-tasks)

#### Exemple simple : projet n’a aucune tâche enfant {#simple-example-project-has-no-children-tasks-1}

PIM = Basé sur les coûts

Méthode EAC = Cumul à partir de tâches/sous-tâches

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
   <td> <p>$2,700.00</p> </td> 
  </tr> 
 </tbody> 
</table>

1. À partir des actions du projet, exécutez Recalculer Finance
1. **IPC****pour la tâche 1** = .14 calculé comme suit :\
   **IPC****pour la tâche 1**  = *IF* Coût réel de la main-d’oeuvre + InferredRepenseCost &lt;> 0 *ALORS*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* IPC = IPC_Travail\
   **IPC****pour la tâche 1**  = (100+300) / (2 500+400)\
   **IPC****pour la tâche 1**  = 400 / 2 900\
   **IPC****pour la tâche 1**  = 0,14

1. **EAC**** pour la tâche 1** = 13 400,00 $\
   **Travail IPC**** pour la tâche 1** = SI Coût réel du travail &lt;> 0 ALORS

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **Travail IPC**** pour la tâche 1** = 100/2500\
   **Travail IPC**** pour la tâche 1** = 0,04

   **EAC Labor****pour la tâche 1** = *IF* CPI_Labor &lt;> 0 *ALORS*

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   *   ELSE* Main-d’oeuvre du CCE = Coût de main-d’oeuvre planifié + coût de main-d’oeuvre réel\
   **EAC Labor****pour la tâche 1** = 500,00/.04\
   **EAC Labor****pour la tâche 1** = 12 500,00 $

   **Dépenses EAC****pour la tâche 1** = InferredRepenseCost + NotInferredScheduleExpense\
   **Dépenses EAC****pour la tâche 1** = 400,00 $ + 500,00 $\
   **Dépenses EAC****pour la tâche 1** = 900,00 $

   **EAC**** pour la tâche 1** = Main-d’oeuvre du CCE + Dépenses du CCE\
   **EAC**** pour la tâche 1**  = 12 500,00 $ + 900,00 $\
   **EAC**** pour la tâche 1**  = 13 400,00 $

1. Voici les valeurs IPC/CAE pour la tâche 2 et la tâche 3 :\
   Tâche 2 = 0,19 / 8 433,33 $\
   Tâche 3 = 0,44 / 6 950,00****

1. IPC du projet = 0,32\
   **IPC****pour le projet** = *IF* Coût réel de la main-d’oeuvre + InferredRepenseCost &lt;> 0 *ALORS*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* IPC = IPC_Travail\
   **IPC****pour le projet** = (1 000 + 2 300) / (7 500 + 2 700)\
   **IPC****pour le projet** = 3300 / 10200\
   **IPC****pour le projet** = 0,32

1. Le coût du projet s&#39;élève à 28 783,33 $.\
   ****** EACpour le projet** = Tâche EAC 1 + Tâche EAC 2 + Tâche EAC 3\
   ****** EACpour le projet** = 13 400,00 $ + 8 433,33 $ + 6 950,00 $\
   ****** EACpour le projet** = 28 783,33 $
