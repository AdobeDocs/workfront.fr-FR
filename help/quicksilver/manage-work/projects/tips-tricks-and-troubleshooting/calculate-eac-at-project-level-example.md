---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: Exemple de calcul - Calculer l’estimation à l’achèvement au niveau du projet
description: PIM = Basé sur l’heure
author: Alina
feature: Work Management
exl-id: ff88b7e3-2a5b-464f-bed1-6848067840b8
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '2194'
ht-degree: 1%

---

# Exemple de calcul - Calculer l’estimation à l’achèvement au niveau du projet

## Méthode EAC : calculer au niveau du projet

* [PIM = Basé sur l’heure](#pim-hour-based)
* [PIM = Basé sur les coûts](#pim-cost-based)

### PIM = Basé sur l’heure {#pim-hour-based}

* [Exemple simple : le projet n’a aucune tâche enfant](#simple-example-project-has-no-children-tasks)
* [Exemple complexe : le projet comporte des tâches enfants](#complicated-example-project-has-children-tasks)

#### Exemple simple : le projet n’a aucune tâche enfant {#simple-example-project-has-no-children-tasks}

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
      <td><p>20 %</p></td>
     </tr>
     <tr>
      <td><p>Tâche 2</p></td>
      <td><p>10 heures</p></td>
      <td><p>25 heures</p></td>
      <td><p>30 %</p></td>
     </tr>
     <tr>
      <td><p>Tâche 3</p></td>
      <td><p>15 heures</p></td>
      <td><p>25 heures</p></td>
      <td><p>40 %</p></td>
     </tr>
    </tbody>
   </table>

1. Recalculer la finance sur le projet.
1. **CPI pour la tâche 1** = .04 calculé comme suit :\
   **CPI pour la tâche 1** = *IF* Heures réelles > 0 *THEN* CPI = TotalBudgetedCostWorkPerformed/Real Hours\
      *ELSE* CPI = 1\
   **IPC pour la tâche 1** = 1/25\
   **CPI pour la tâche 1** = 0,04

1. **EAC pour la tâche 1** = 125 heures calculées comme suit :\
   **EAC pour la tâche 1** = *IF* CPI &lt;> 0 *THEN* EAC = Heures/IPC planifiées\
       *ELSE* EAC = Planifié  Heures + Réelles  Heures\
   **EAC pour la tâche 1** = 5 / .04\
   **EAC pour la tâche 1** = 125 heures****

1. IPC/CAE pour les tâches 2 et 3 :\
   Tâche  2 = 0,12 / 83,33  hrs\
   Tâche 3 = 0,24 / 62,5 heures

1. **CPI pour le projet** = 0,13 calculé comme suit :\
   **CPI pour le projet** = *IF* Heures réelles > 0 *THEN* CPI = TotalBudgetCostWorkPerformed/Current Hours\
       *ELSE* CPI = 1\
   **CPI pour le projet** = 10 / 75\
   **CPI pour le projet** = 0,13

1. **EAC pour le projet** = 225 heures calculées comme suit :\
   **EAC pour le projet** = *IF* CPI &lt;> 0 *THEN* EAC = Heures/IPC planifiées\
       *ELSE* EAC = Planifié  Heures + Réelles  Heures\
   **EAC pour le projet** = 30 / .13333\
   **EAC pour le projet** = 225 heures

#### Exemple complexe : le projet comporte des tâches enfants {#complicated-example-project-has-children-tasks}

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
   >Pour les tâches 1 et 3, vous ajoutez uniquement des heures réelles.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <br> <p><strong>Tâche</strong> </p> </th> 
   <th> <br> <p><strong>Hrs Prév</strong> </p> </th> 
   <th> <br> <p><strong>Agir sur Hrs</strong> </p> </th> 
   <th> <p><strong>% Complète</strong> </p> </th> 
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
   <td> <p>20 %</p> </td> 
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
   <td> <p>40 %</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 5</p> </td> 
   <td> <p>15 heures</p> </td> 
   <td> <p>10 heures</p> </td> 
   <td> <p>50 %</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 6</p> </td> 
   <td> <p>20 heures</p> </td> 
   <td> <p>10 heures</p> </td> 
   <td> <p>60 %</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Ajoutez 50 heures directement au projet (Plus>Heures>Heures de journal).
1. **CPI pour la tâche 2** = .1 calculé comme suit :\
   **CPI pour la tâche 2** = *IF* Heures réelles > 0 *THEN* CPI = TotalBudgetedCostWorkPerformed/Real Hours\
       *ELSE* CPI = 1\
   **CPI pour la tâche 2** = 1/10\
   **CPI pour la tâche 2** = 0,1

1. **EAC pour la tâche 2** = 50 heures calculées comme suit :\
   **EAC pour la tâche 2** = *IF* CPI &lt;> 0 *THEN* EAC = Heures/IPC planifiées\
       *ELSE* EAC = Planifié  Heures + Réelles  Heures\
   **EAC pour la tâche 2** = 5 / .1\
   **EAC pour la tâche 2** = 50 heures

1. L’IPC/le CAE pour les tâches 4, 5 et 6 sont les suivants :\
   Tâche 4 : 0,4 / 25 heures\
   Tâche 5 : 0,75 / 20 heures\
   Tâche 6 : 1.2 / 16.67 heures

1. **CPI pour la tâche 3** = 0,38  calculé comme suit :\
   **CPI pour la tâche 3** = *IF* Heures réelles > 0 *THEN* CPI = TotalBudgetedCostWorkPerformed/Real Hours\
       *ELSE* CPI = 1\
   **IPC pour la tâche 3** = 11.5/30\
   **CPI pour la tâche 3** = 0,38

1. **EAC pour la tâche 3** = 65,22 heures calculées comme suit :\
   **EAC pour la tâche 3** = *IF* CPI &lt;> 0 *THEN* EAC = Heures/IPC planifiées\
       *ELSE* EAC = Planifié  Heures + Réelles  Heures\
   **EAC pour la tâche 3** =  25 / .383333\
   **EAC pour la tâche 3** = 65,22 heures

1. **IPC pour la tâche 1** = 0,25 calculé comme suit :\
   **CPI pour la tâche 1** = *IF* Heures réelles > 0 *THEN* CPI = TotalBudgetedCostWorkPerformed/Real Hours\
       *ELSE* CPI = 1\
   **IPC pour la tâche 1** = 12.5/50\
   **CPI pour la tâche 1** = 0,25

1. **EAC pour la tâche 1** = 120 heures calculées comme suit :\
   **EAC pour la tâche 1** = *IF* CPI &lt;> 0 *THEN* EAC = Heures planifiées / CPI\
       *ELSE* EAC = Planifié  Heures + Réelles  Heures\
   **EAC pour la tâche 1** =  30/ .25\
   **EAC pour la tâche 1** = 120 heures

1. **CPI pour le projet** = 0,22 calculé comme suit :\
   **CPI pour le projet** = *IF* Heures réelles > 0 *THEN* CPI = TotalBudgetCostWorkPerformed/Current Hours\
       *ELSE* CPI = 1\
   **CPI pour le projet** = 24.5/110\
   **CPI pour le projet** = 0,22272\
   **CPI pour le projet** = 0,22

1. **EAC pour le projet** = 224.49  hrs calculé comme suit :\
   **EAC pour le projet** = *IF* CPI &lt;> 0 *THEN* EAC = Heures/IPC planifiées\
       *ELSE* EAC = Planifié  Heures + Réelles  Heures\
   **EAC pour le projet** =  50 / .22272\
   **EAC pour le projet** = 224,49 heures

### PIM = Basé sur les coûts {#pim-cost-based}

* [Exemple simple : le projet n’a aucune tâche enfant](#simple-example-project-has-no-children-tasks)
* [Exemple complexe : le projet comporte des tâches enfants](#complicated-example-project-has-children-tasks)

#### Exemple simple : le projet n’a aucune tâche enfant {#simple-example-project-has-no-children-tasks-1}

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
   <th> <br> <p><strong>Pln Lbr Cost</strong> </p> </th> 
   <th> <br> <p><strong>Agir sur Hrs</strong> </p> </th> 
   <th> <br> <p><strong>Act Lbr Cost</strong> </p> </th> 
   <th> <p><strong>% Complète</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Tâche 1</p> </td> 
   <td> <p>5 heures</p> </td> 
   <td> <p>500,00 $</p> </td> 
   <td> <p>25 heures</p> </td> 
   <td> <p>2 500,00 $</p> </td> 
   <td> <p>20 %</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 2</p> </td> 
   <td> <p>10 heures</p> </td> 
   <td> <p>1 000,00 $</p> </td> 
   <td> <p>25 heures</p> </td> 
   <td> <p>2 500,00 $</p> </td> 
   <td> <p>30 %</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 3</p> </td> 
   <td> <p>15 heures</p> </td> 
   <td> <p>1 500 $</p> </td> 
   <td> <p>25 heures</p> </td> 
   <td> <p>2 500,00 $</p> </td> 
   <td> <p>40 %</p> </td> 
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
   <th> <p><strong>Montant planifié</strong> </p> </th> 
   <th> <p><strong>Montant réel</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Tâche 1</p> </td> 
   <td> <p>Tâche 1 Exp 1</p> </td> 
   <td> <p>300,00 $</p> </td> 
   <td> <p>400,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 1</p> </td> 
   <td> <p>Tâche 1 Exp 2</p> </td> 
   <td> <p>500,00 $</p> </td> 
   <td> <p>0,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 2</p> </td> 
   <td> <p>Task 2 Exp</p> </td> 
   <td> <p>200,00 $</p> </td> 
   <td> <p>100,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 3</p> </td> 
   <td> <p>Task 3 Exp</p> </td> 
   <td> <p>800,00 $</p> </td> 
   <td> <p>700,00 $</p> </td> 
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
   <th> <p><strong>Montant planifié</strong> </p> </th> 
   <th> <p><strong>Montant réel</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Project Exp 1</p> </td> 
   <td> <p>1 000,00 $</p> </td> 
   <td> <p>1 500 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 1 Exp 2</p> </td> 
   <td> <p>2 500,00 $</p> </td> 
   <td> <p>0,00 $</p> </td> 
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
   <th> <p><strong>Frais planifiés non engagés</strong> </p> </th> 
   <th> <p><strong>Dépenses Planifiées Accordées</strong> </p> </th> 
   <th> <p><strong>Dépenses réelles engagées</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Tâche 1</p> </td> 
   <td> <p>500,00 $</p> </td> 
   <td> <p>300,00 $</p> </td> 
   <td> <p>400,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 2</p> </td> 
   <td> <p>0,00 $</p> </td> 
   <td> <p>200,00 $</p> </td> 
   <td> <p>100,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 3</p> </td> 
   <td> <p>0,00 $</p> </td> 
   <td> <p>800,00 $</p> </td> 
   <td> <p>700,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projet</p> </td> 
   <td> <p>3 000 $</p> </td> 
   <td> <p>2 300,00 $</p> </td> 
   <td> <p> 2 700,00 $ <strong></strong></p> </td> 
  </tr> 
 </tbody> 
</table>

1. À partir des actions du projet, exécutez Recalculer Finance
1. **CPI pour la tâche 1** = 0,14
1. **CPI****pour la tâche 1** = .14 calculée comme suit :\
   **CPI**  **pour la tâche 1** = *IF* Coût réel du travail + InferredRepenseCost  &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   *    ELSE* CPI = IPC_Travail\
   **CPI****pour la tâche 1** = (100+300) / (2500+400)\
   **CPI**  **pour la tâche 1** = 400 / 2900\
   **CPI**  **pour la tâche 1**  = 0,14****

1. **EAC****pour la tâche 1** = 13 400,00 $\
   **Travail CPI**  **pour la tâche 1** = SI le coût réel du travail &lt;> 0 ALORS

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed/Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **Travail CPI**  **pour la tâche 1** = 100/2500\
   **Travail CPI**  **pour la tâche 1** = .04 ****** EAC Labor ****pour la tâche 1 **=*IF *CPI_Labor &lt;> 0*THEN *EAC Labor = Coût du travail planifié/CPI_Labor\
   *    ELSE* EAC  Travail = Coût du travail planifié + coût réel du travail\
   **Travail EAC ****pour la tâche 1** = 500.00/.04\
   **Main-d’oeuvre EAC****pour la tâche 1** = 12 500,00 $\
   **Frais EAC****pour la Tâche 1** = InferredExpenseCost + NotInferredScheduleExpense\
   **Frais de contrôle d’accès****pour la tâche 1** = 400,00 $ + 500,00 $\
   **Frais d’EAC****pour la tâche 1** = 900,00 $\
   **EAC****pour la tâche 1** = Main-d’oeuvre EAC + Dépenses EAC\
   **EAC****pour la tâche 1**  = 12 500 $ + 900 $\
   **EAC****pour la tâche 1**  = 13 400 $

1. Voici les valeurs IPC/CAE pour la tâche 2 et la tâche 3 :\
   Tâche 2 = 0,19 / 8 433,33 $\
   Tâche 3 = 0,44 / 6 950,00 $

1. **CPI pour le projet** = 0,32 calculé comme suit :\
   **CPI****pour le projet** = *IF* Coût réel de la main-d’oeuvre + InstartedRepenseCost  &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = IPC_Travail\
   **CPI****pour le projet** = (1 000 + 2 300) / (7 500 + 2 700)\
   **CPI****pour le projet** = 3300 / 10 200\
   **CPI****pour le projet** = 0,32

1. **EAC pour le projet** = 28 200,00 $ calculé comme suit :\
   **CPI Labor****for Project** = IF Réel Coût du travail &lt;> 0 ALORS

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed/Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **IPC/Travail****pour le projet** = 1 000 / 7 500\
   **Tâche à la baisse des prix****pour le projet** = 0,13333\
   **Travail IPC****pour le projet** = 0,13

   **EAC Labor****for Project** = *IF* CPI_Labor &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost/CPI_Labor
   ```

   *   ELSE* EAC  Travail = Coût du travail planifié + coût réel du travail\
   **Main-d’oeuvre EAC****pour le projet** = 3000/ .13333\
   **Main-d’oeuvre****EAC pour le projet** = 22 500,00 $

   **Frais EAC****Project** =

   ```
   IncurredActualExpenseCost + NotIncurredPlannedExpense
   ```

   ******Projet de dépenses EAC** = 3 000,00 $ + 2 700,00 $\
   ******Projet de dépenses EAC** = 5 700,00 $

   **EAC****Project** = Main-d’oeuvre EAC + Dépenses EAC\
   **EAC****Project**  = 22 500 $ + 5 700 $\
   **EAC****Project**  = 28 200,00 $

#### Exemple complexe : le projet comporte des tâches enfants {#complicated-example-project-has-children-tasks-1}

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
   >Pour les tâches 1 et 3, vous ajoutez uniquement des heures réelles.

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
   <th> <br> <p><strong>Pln Lbr Cost</strong> </p> </th> 
   <th> <br> <p><strong>Agir sur Hrs</strong> </p> </th> 
   <th> <br> <p><strong>Act Lbr Cost</strong> </p> </th> 
   <th> <p><strong>% Complète</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Tâche 1</p> </td> 
   <td> </td> 
   <td> </td> 
   <td> <p>10 heures</p> </td> 
   <td> <p>1 000,00 $</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 2</p> </td> 
   <td> <p>5 heures</p> </td> 
   <td> <p>500,00 $</p> </td> 
   <td> <p>10 heures</p> </td> 
   <td> <p>1 000,00 $</p> </td> 
   <td> <p>20 %</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 3</p> </td> 
   <td> </td> 
   <td> </td> 
   <td> <p>10 heures</p> </td> 
   <td> <p>1 000,00 $</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 4</p> </td> 
   <td> <p>10 heures</p> </td> 
   <td> <p>1 000,00 $</p> </td> 
   <td> <p>10 heures</p> </td> 
   <td> <p>1 000,00 $</p> </td> 
   <td> <p>40 %</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 5</p> </td> 
   <td> <p>15 heures</p> </td> 
   <td> <p>1 500 $</p> </td> 
   <td> <p>10 heures</p> </td> 
   <td> <p>1 000,00 $</p> </td> 
   <td> <p>50 %</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 6</p> </td> 
   <td> <p>20 heures</p> </td> 
   <td> <p>2 000 $</p> </td> 
   <td> <p>10 heures</p> </td> 
   <td> <p>1 000,00 $</p> </td> 
   <td> <p>60 %</p> </td> 
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
   <th> <p><strong>Montant planifié</strong> </p> </th> 
   <th> <p><strong>Montant réel</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Tâche 1</p> </td> 
   <td> <p>Tâche 1 Exp 1</p> </td> 
   <td> <p>300,00 $</p> </td> 
   <td> <p>- 400,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 1</p> </td> 
   <td> <p>Tâche 1 Exp 2</p> </td> 
   <td> <p>- 500,00 $</p> </td> 
   <td> <p>800,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 1</p> </td> 
   <td> <p>Tâche 1 Exp 3</p> </td> 
   <td> <p>400,00 $</p> </td> 
   <td> <p>0,00 $</p> </td> 
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
   <td> <p>500,00 $</p> </td> 
   <td> <p>700,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 2</p> </td> 
   <td> <p>Tâche 2 Exp 2</p> </td> 
   <td> <p>- 400,00 $</p> </td> 
   <td> <p>0,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 2</p> </td> 
   <td> <p>Tâche 2 Exp 3</p> </td> 
   <td> <p>- 200,00 $</p> </td> 
   <td> <p>600,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 2</p> </td> 
   <td> <p>Tâche 2 Exp 4</p> </td> 
   <td> <p>700,00 $</p> </td> 
   <td> <p>- 200,00 $</p> </td> 
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
   <td> <p>0,00 $</p> </td> 
   <td> <p>1 000,00 $</p> </td> 
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
   <td> <p>800,00 $</p> </td> 
   <td> <p>0,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 4</p> </td> 
   <td> <p>Tâche 4 Exp 2</p> </td> 
   <td> <p>- 100,00 $</p> </td> 
   <td> <p>300,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 4 </p> </td> 
   <td> <p>Tâche 4 Exp 3</p> </td> 
   <td> <p>-200,00</p> </td> 
   <td> <p>0,00 $</p> </td> 
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
   <td> <p>700,00 $</p> </td> 
   <td> <p>800,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 5</p> </td> 
   <td> <p>Tâche 5 Exp 2</p> </td> 
   <td> <p>- 100,00 $</p> </td> 
   <td> <p>300,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 5</p> </td> 
   <td> <p>Tâche 5 Exp. 3</p> </td> 
   <td> <p>- 400,00 $</p> </td> 
   <td> <p>- 200,00 $</p> </td> 
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
   <td> <p>600,00 $</p> </td> 
   <td> <p>700,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 6</p> </td> 
   <td> <p>Tâche 6 Exp 2</p> </td> 
   <td> <p>500,00 $</p> </td> 
   <td> <p>- 300,0 $</p> </td> 
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
   <th> <p><strong>Montant planifié</strong> </p> </th> 
   <th> <p><strong>Montant réel</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Project Exp 1</p> </td> 
   <td> <p>1 000,00 $</p> </td> 
   <td> <p>1 500 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 1 Exp 2</p> </td> 
   <td> <p>2 500,00 $</p> </td> 
   <td> <p> 0,00 $ <strong></strong></p> </td> 
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
   <th> <p><strong>Frais planifiés non engagés</strong> </p> </th> 
   <th> <p><strong>Dépenses Planifiées Accordées</strong> </p> </th> 
   <th> <p><strong>Dépenses réelles engagées</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Tâche 1</p> </td> 
   <td> <p>400,00 $</p> </td> 
   <td> <p>- 500,00 $</p> </td> 
   <td> <p>800,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 2</p> </td> 
   <td> <p>- 400,00 $</p> </td> 
   <td> <p>300,00 $</p> </td> 
   <td> <p>1 300 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 3</p> </td> 
   <td> <p>0,00 $</p> </td> 
   <td> <p>0,00 $</p> </td> 
   <td> <p>1 000,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 4</p> </td> 
   <td> <p>600,00 $</p> </td> 
   <td> <p>- 100,00 $</p> </td> 
   <td> <p>300,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 5</p> </td> 
   <td> <p>0,00 $</p> </td> 
   <td> <p>600,00 $</p> </td> 
   <td> <p>1 100,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 6</p> </td> 
   <td> <p>0,00 $</p> </td> 
   <td> <p>600,00 $</p> </td> 
   <td> <p>700,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projet</p> </td> 
   <td> <p>2 500,00 $</p> </td> 
   <td> <p>1 000,00 $</p> </td> 
   <td> <p>1 500 $</p> </td> 
  </tr> 
 </tbody> 
</table>

1. À partir des actions du projet, exécutez Recalculer Finance
1. **CPI** pour la tâche 2 = 0,17 calculé comme suit :\
   **Tâche IPC 2** = *IF* Coût réel de la main-d’oeuvre + InferredRepenseCost  &lt;> 0 *THEN* CPI = (TotalBudgetedCostWorkPerformed + InferredScheduleExpenseCost) / (RéelCoûtTravail + InferredRepenseCost)\
   *   ELSE* CPI = IPC_Travail\
   **CPI****Task 2** = (100+300) / (1000+1300)\
   **CPI****Task 2**  = 400 / 2 300\
   **CPI****Task 2**  = 0,17

1. **EAC** pour la tâche 2 = 5 900,00 $\
   **IPC/Travail****Tâche 2** = SI Coût réel de la main-d’oeuvre &lt;> 0 ALORS IPC_Travail = TotalBudgetCostWorkPerformed / Coût réel de la main-d’oeuvre\
      ELSE CPI_Labor = 1\
   **Tâche de travail CPI****Tâche 2** = 100/1000\
   **Tâche d’emploi IPC****Tâche 2** = 0,1

   **EAC Labor****Task 2** = *IF* CPI_Labor &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost/CPI_Labor
   ```

   *   ELSE* EAC  Travail = Coût du travail planifié + coût réel du travail\
   **Travail EAC****Tâche 2** = 500.00/.1\
   **Travail EAC****Tâche 2** = 5 000,00 $****** Frais EAC ****Tâche 2 **= InferredRepenseCost + NotInferredScheduleExpense\
   **Dépenses du CCE ****Tâche 2** = 1 300 $ + - 400 $\
   **Frais d’EAC****Tâche 2** = 900,00 $

   **EAC****Task 2** = Main-d’oeuvre de l’EAC + Dépenses de l’EAC\
   **EAC****Task 2**  = 5 000 $ + 900 $\
   **EAC****Task 2**  = 5 900,00 $

1. L’IPC/le CAE pour les tâches 4, 5 et 6 sont déterminés de la même manière. Je vais donc simplement fournir les valeurs ci-dessous :\
   Tâche 4 : 0,23 / 3 400,00 $\
   Tâche 5 : 0,64 / 3 100,00 $\
   Tâche 6 : 1,06 / 2 366,67 $

1. IPC pour la tâche 3 = 0,31 calculé comme suit :\
   **CPI****Task 3** = *IF* Coût réel de la main-d’oeuvre + coût réel de la dépense provenant d’une entreprise  &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = IPC_Travail\
   **CPI****Task 3**  = (1 150 + 500) / (3 000 + 2 400)\
   **CPI****Task 3**  =  1 650 / 5 400\
   **CPI****Task 3**  = .31 ****** EAC pour la tâche 3 **= 9 521,74 $ calculé comme suit :\
   **Tâche de l’IPC ****Tâche 3** = SI Coût réel de la main-d’oeuvre &lt;> 0 ALORS

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **Tâche d’utilisation des IPC****Tâche 3** = 1150/3000\
   **Tâche d’utilisation des IPC****Tâche 3** = .383333\
   **IPC Labor****Task 3** = 0,38

   **EAC Labor****Task 3** = *IF* CPI_Labor &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   *   ELSE* EAC  Travail = Coût du travail planifié + coût réel du travail\
   **Tâche****Travail EAC 3** = 2 500,00 $ / .383333\
   **EAC Labor****Task 3** = 6 521,74 $

   **EAC Expense****Task 3** = InferredRepenseCost + NotInptedExpense\
   ******TâcheEAC 3** = 2 400,00 $ + 600,00 $\
   **Frais d’EAC****Tâche 3** = 3 000,00 $

   **EAC****Task 3** = Main-d’oeuvre EAC + Dépenses EAC\
   **EAC****Task 3**  = 6 521,74 $ + 3 000 $\
   **EAC****Task 3**  = 9 521,74 $

1. IPC pour la tâche 1 = 0,16 calculé comme suit :\
   **CPI****Task 1** = *IF* Coût réel de la main-d’oeuvre + InferredRepenseCost  &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = IPC_Travail\
   **CPI****Task 1**  = (1 250 + 300) / (5 000 + 4 500)\
   **CPI****Task 1**  =  1550 / 9500=\
   **CPI****Task 1**  = 0,16

1. Le CAE pour la tâche 1 est de 17 100 $, calculé comme suit :\
   **CPI Labor****Tâche 1** = SI Coût réel du travail &lt;> 0 ALORS

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **IPC Labor****Task 1** = 1250 / 5000\
   **Tâche de l’IPC****Tâche 1** = 0,25

   **EAC Labor****Task 1** = *IF* CPI_Labor &lt;> 0 *THEN* EAC Labor = Coût du travail planifié / CPI_Labor\
   *   ELSE* EAC  Travail = Coût du travail planifié + coût réel du travail\
   **Tâche****Travail EAC 1** = 3 000,00 $ / 0,25\
   **Tâche****Travail EAC 1** = 12 000,00 $

   **EAC Expense****Task 1** = InferredRepenseCost + NotInptedExpense\
   **Frais d’EAC****Tâche 1** = 4 500 $ + 600\
   **Frais d’EAC****Tâche 1** = 5 100,00 $

   **EAC****Task 1** = Main-d’oeuvre EAC + Dépenses EAC\
   **EAC****Task 1**  = 12 000,00 $ + 5 100,00\
   **EAC****Task 1**  = 17 100,00 $

1. Le IPC du projet est de 0,25\
   **CPI****pour le projet** = *IF* Coût réel de la main-d’oeuvre + InstartedRepenseCost  &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = IPC_Travail

   **CPI****pour le projet** = (2 450 + 1 900) / (1 1 000 + 6 700)\
   **CPI****pour le projet** =   4350 / 17700\
   **CPI****pour le projet** = 0,25

1. **EAC pour le projet** = 32 248,98 $ calculé comme suit :\
   **CPI Labor****for Project** = IF Réel Coût du travail &lt;> 0 ALORS

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **IPC/Travail****pour le projet** = 2450/11000\
   **Travail IPC****pour le projet** = 0,2272\
   **Travail IPC****pour le projet** = 0,22

   **EAC Labor****for Project** = *IF* CPI_Labor &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   *   ELSE* EAC  Travail = Coût du travail planifié + coût réel du travail\
   **Travail du CCE****pour le projet** = 5 000,00 $ / .22272\
   **Travail****EAC pour le projet** = 22 448,97959 $\
   **Travail****EAC pour le projet** = 22 448,98 $

   **EAC Expense****Project** = InferredRepenseCost + NotInferredScheduleExpense\
   **Projet de dépenses du contrôle d’accès****** = 3 100,00 $ + 6 700,00 $\
   **EAC Expense****Project** = 9 800,00 $

   **EAC****Project** = Main-d’oeuvre EAC + Dépenses EAC\
   **EAC****Project**  = 22 448,98 $ + 9 800,00 $\
   **EAC****Project**  = 32 248,98 $
