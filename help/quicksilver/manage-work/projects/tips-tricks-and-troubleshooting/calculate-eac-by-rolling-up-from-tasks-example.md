---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: Exemple de calcul - Calculer CRE comme un cumul à partir des tâches
description: Cet article donne un exemple de calcul de l’Estimation à l’achèvement (EAC) d’un projet comme cumul de toutes les tâches du projet dans Adobe Workfront.
author: Lisa
feature: Work Management
exl-id: 68b582c9-f72a-4000-9d28-f7dafa23541f
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '1134'
ht-degree: 88%

---

# Exemple de calcul - Calculer l’estimation à l’achèvement en tant que cumul à partir des tâches

## Méthode EAC : cumuler à partir des tâches ou des sous-tâches

* [PIM = Basé sur les heures](#pim-hour-based)
* [PIM = basé sur les coûts](#pim-cost-based)

### PIM = Basé sur les heures {#pim-hour-based}

* [Exemple simple : le projet n’a aucune tâche enfant](#simple-example-project-has-no-children-tasks).
* [Exemple complexe : le projet comporte des tâches enfant.](#complicated-example-project-has-children-tasks)

#### Exemple simple : le projet n’a aucune tâche enfant. {#simple-example-project-has-no-children-tasks}

PIM = basé sur les heures

Méthode EAC : cumuler à partir des tâches ou des sous-tâches

1. Créez le projet A avec trois tâches (aucune tâche enfant) affectées à la personne 1 dont le coût/heure est de 100,00 $.
1. Ajoutez les heures prévues/effectives à chaque tâche et le pourcentage d’achèvement au tableau ci-dessous :

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
   <td> <p>5 heures</p> </td> 
   <td> <p>25 heures</p> </td> 
   <td> <p>20 %</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 2</p> </td> 
   <td> <p>10 heures</p> </td> 
   <td> <p>25 heures</p> </td> 
   <td> <p>30 %</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tâche 3</p> </td> 
   <td> <p>15 heures</p> </td> 
   <td> <p>25 heures</p> </td> 
   <td> <p>40 %</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Recalculer finances
1. **ICP pour la tâche 1** = 0,04 calculé comme suit :\
   **ICP pour la tâche 1** = *IF* Heures effectives > 0 *THEN* ICP = Coût budgété du travail effectué/Heures effectives\
   *SINON* IPC = 1\
   **ICP pour la tâche 1** = 1 / 25\
   **ICP pour la tâche 1** = 0,04

1. **EAC pour la tâche 1** = 125 heures calculées comme suit :\
   **EAC pour la tâche 1** = *IF* ICP &lt;> 0 *THEN* EAC = Nombre d’heures prévues / ICP\
   *SINON*

   ```
   EAC = Planned  Hours + Actual  Hours
   ```

   **EAC pour la tâche 1** = 5 / 0,04\
   **EAC pour la tâche 1** = 125 heures

1. ICP/EAC pour les Tâches 2 et 3 :\
   Tâche 2 = .12 / 83,33 heures\
   Tâche 3 = 0,24 / 62,5 heures

1. **ICP du projet** = 0,13 calculé comme suit :\
   **ICP du projet** = *IF* Heures effectives > 0 *THEN*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *SINON* IPC = 1
   **ICP du projet** = 10 / 75\
   **ICP du projet** = 0,13

1. **EAC pour le projet** = 270,83 heures calculées comme suit\
   **EAC pour le projet** = EAC Tâche 1 + EAC Tâche 2 + EAC Tâche 3\
   **EAC pour le projet** = 125 + 83,33 + 62,5\
   **EAC pour le projet** = 270,83 heures

#### Exemple complexe : le projet comporte des tâches enfant. {#complicated-example-project-has-children-tasks}

PIM = basé sur les heures

Méthode EAC : cumuler à partir des tâches ou des sous-tâches

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

1. Ajoutez 50 heures directement au projet (Plus > Heures > Consigner les heures) afin d’enregistrer 5 000,00 $ de coût réel de main-d’œuvre directement dans le projet.

1. Exécuter Recalculer finances
1. **ICP pour la tâche 2** = 0,1 calculé comme suit :\
   **ICP pour la tâche 2** = *IF* Heures effectives > 0 *THEN*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *SINON* IPC = 1
   **ICP pour la tâche 2** = 1 / 10\
   **ICP pour la tâche 2** = 0,1

1. **EAC pour la tâche 2** = 50 heures calculées comme suit :\
   **EAC pour la tâche 2** = *IF* ICP &lt;> 0 *THEN*

   ```
   EAC = Planned Hours / CPI
   ```

       *ELSE* CRE = Heures prévues + Heures réelles
   **EAC pour la tâche 2** = 5 / 0,1\
   **EAC pour la tâche 2** = 50 heures

1. ICP/EAC pour la tâche 4, la tâche 5 et la tâche 6 :\
   Tâche 4 = 0,4 / 25 heures\
   Tâche 5 = 0,75 / 20 heures\
   Tâche 6 = 1,2 / 16,67 heures

1. **ICP pour la tâche 3** = 0,38\
   **ICP pour la tâche 3** = *IF* Heures effetives > 0 *THEN*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *SINON* IPC = 1
   **ICP pour la tâche 3** = 11,5 / 30\
   **ICP pour la tâche 3** = 0,38

1. **EAC pour la tâche 3** = EAC Tâche 4 + EAC Tâche 5\
   **EAC pour la tâche 3** = 25 + 20\
   **EAC pour la tâche 3** = 45 heures

1. **ICP pour la tâche 1** = 0,25 calculé comme suit :\
   **ICP pour la tâche 1** = *IF* Heures effectives > 0 *THEN*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *SINON* IPC = 1
   **ICP pour la tâche 1** = 12,5 / 50\
   **ICP pour la tâche 1** = 0,25

1. **EAC pour la tâche 1** = EAC Tâche 2 + EAC Tâche 3\
   **EAC pour la tâche 1** = 50 + 45\
   **EAC pour la tâche 1** = 95 heures

1. ICP du projet = 0,22 calculé comme suit :\
   **ICP du projet** = *IF* Heures effectives > 0 *THEN*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *SINON* IPC = 1
   **ICP du projet** = 24,5 / 110\
   **ICP du projet** = 0,22272\
   **ICP du projet** = 0,22

1. **EAC du projet** = EAC Tâche 1 + EAC Tâche 6\
   **EAC du projet** = 95 + 16,67\
   **EAC du projet** = 111,67 heures

### PIM = basé sur les coûts {#pim-cost-based}

* [Exemple simple : le projet n’a aucune tâche enfant.](#simple-example-project-has-no-children-tasks)

#### Exemple simple : le projet n’a aucune tâche enfant. {#simple-example-project-has-no-children-tasks-1}

PIM = Basé sur les coûts

Méthode EAC : cumuler à partir des tâches ou des sous-tâches

1. Créez le projet A avec trois tâches (aucune tâche enfant) toutes affectées à la personne 1 dont le coût/heure est de 100,00 $.
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
   <td> <p>2 700,00 $</p> </td> 
  </tr> 
 </tbody> 
</table>

1. À partir des actions du projet, exécuter Recalculer finances
1. **ICP**&#x200B;**de la tâche 1** = 0,14 calculé comme suit :\
   **IPC**&#x200B;**pour la tâche 1** = *IF* Coût réel de la main-d&#39;œuvre + IncurredActualExpenseCost &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   * SINON* ICP = CPI_Labor\
     **IPC**&#x200B;**pour la tâche 1** = (100 + 300) / (2 500 + 400)\
     **IPC**&#x200B;**pour la tâche 1** = 400/2900\
     **IPC**&#x200B;**pour la tâche 1** = .14

1. **EAC**&#x200B;**&#x200B; de la tâche 1** = 13 400 $\
   **ICP main d’œuvre**&#x200B;**&#x200B; de la tâche 1** = IF Coût réel de main d’œuvre &lt;> 0 THEN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

   SINON CPI_Labor = 1\
   **ICP main d’œuvre**&#x200B;**&#x200B; de la tâche 1** = 100/2500\
   **ICP main d’œuvre**&#x200B;**&#x200B; de la tâche 1** = 0,04

   **EAC main d’œuvre**&#x200B;**de la tâche 1** = *IF* CPI_Labor &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   * SINON* CRE Main-d&#39;œuvre = Coût prévu de main-d&#39;œuvre + Coût réel de main-d&#39;œuvre\
     **EAC main d’œuvre**&#x200B;**de la tâche 1** = 500/0,04\
     **EAC main d’œuvre**&#x200B;**de la tâche 1** = 12 500,00 $

   **EAC dépense**&#x200B;**de la tâche 1** = Coût des dépenses réelles engagées + Coût des dépenses prévues non engagées\
   **EAC dépenses**&#x200B;**de la tâche 1** = 400 $ + 500 $\
   **EAC dépenses**&#x200B;**de la tâche 1** = 900 $

   **EAC dépenses**&#x200B;**&#x200B; de la tâche 1** = EAC main d’œuvre + EAC dépenses\
   **CRE**&#x200B;**pour la tâche 1** = 12 500 $ + 900 $\
   **CRE**&#x200B;**pour la tâche 1** = 13 400 $

1. Voici les valeurs ICP/EAC pour la tâche 2 et la tâche 3 :\
   Tâche 2 = 0,19 / 8 433,33 $\
   Tâche 3 = 0,44/6 950 $**&#x200B;**

1. ICP du projet = 0,32\
   **ICP**&#x200B;**pour le projet** = *IF* Coût réel de la main-d’œuvre + IncurredActualExpenseCost &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   * SINON* ICP = CPI_Labor\
     **ICP**&#x200B;**du projet** = (1 000 + 2 300)/(7 500 + 2 700)\
     **ICP**&#x200B;**du projet** = 3 300/10 200\
     **ICP**&#x200B;**du projet** = 0,32

1. L’EAC du projet est de 28 783,33 $.\
   **EAC**&#x200B;**pour le projet** = EAC Tâche 1 + EAC Tâche 2 + EAC Tâche 3\
   **EAC**&#x200B;**pour le projet** = 13 400 $ + 8 433,33 $ + 6 950 $\
   **EAC**&#x200B;**pour le projet** = 28 783,33 $
