---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calculer l’Indice Coûts Performances (ICP)
description: L’Indice Coûts Performances (ICP) décrit la relation au niveau du projet ou de la tâche entre le coût prévu et le coût réel. Les personnes responsables de projet examinent cette mesure pour identifier les tâches ou les projets qui effectuent actuellement le suivi de sous ou sur-coût à un moment donné.
author: Lisa
feature: Work Management
exl-id: 7f2efe26-7292-482d-986c-2d2077a7ca52
source-git-commit: 6afa65f921864403c10541d283ef717dce81aed7
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 100%

---

# Calculer l’Indice Coûts Performances (ICP)

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.)</p>
-->

L’Indice Coûts Performances (ICP) décrit la relation au niveau du projet ou de la tâche entre le coût prévu et le coût réel. Les personnes responsables de projet examinent cette mesure pour identifier les tâches ou les projets qui effectuent actuellement le suivi de sous ou sur-coût à un moment donné. Le coût peut être mesuré en heures ou en dollars, selon votre méthode d’indice de performances (PIM). Pour plus d’informations sur la définition de la méthode d’indice de performances, voir [Définition de la méthode d’indice de performances (PIM)](../../../manage-work/projects/project-finances/set-pim.md).

Seules les organisations qui ont besoin d’une saisie des heures peuvent utiliser l’ICP. En outre, les valeurs de la PIM basées sur les coûts ne sont exactes que dans les organisations qui ont défini des taux de coût pour les personnes cessionnaires de tâches (fonctions ou utilisateurs et utilisatrices).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>
   <p>Nouveau : Light ou supérieur</p>
   <p>ou</p>
   <p>Actuel : Révision ou supérieur</p></td>  
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td>Afficher l’accès aux projets et aux données financières</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td>Autorisations Afficher ou supérieures pour le projet avec les autorisations Afficher Finance</td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vue d’ensemble de l’Indice Coûts Performances (ICP)

* [Valeur de l’ICP](#the-cpi-value)
* [Méthode de calcul de l’ICP](#how-cpi-is-calculated)

### Valeur de l’ICP {#the-cpi-value}

Les personnes responsables de projet comprennent qu’une valeur de l’ICP d’1 signifie que le projet est parfaitement conforme au budget. Les valeurs supérieures à 1 indiquent qu’un projet se situe sous le budget (moins d’heures ou de dépenses ont été enregistrées que prévu initialement) et les valeurs inférieures à 1 indiquent qu’un projet se situe au-dessus du budget (plus d’heures ou de dépenses ont été enregistrées que prévu initialement). Plus on s’éloigne de la valeur 1, plus on s’éloigne du plan initial.

| **Valeur de l’ICP** | **Indication sur le budget** |
|---|---|
| 1 | Conforme au plan ou budget |
| > 1 (supérieur à 1) | En dessous du budget |
| &lt; 1 (inférieur à 1) | Au-dessus du budget |


### Méthode de calcul de l’ICP {#how-cpi-is-calculated}

Dans Adobe Workfront, le calcul de l’ICP dépend de la méthode d’indice de performances sélectionnée pour le projet. Pour plus d’informations sur la définition de la méthode d’indice de performances, voir [Définir la méthode d’indice de performances (PIM)](../../../manage-work/projects/project-finances/set-pim.md).

* [Calculs de l’ICP lors de l’utilisation d’une PIM horaire](#cpi-calculations-when-using-hour-based-pim)
* [Calculs de l’ICP en utilisant la PIM basée sur les coûts](#cpi-calculations-when-using-cost-based-pim)

#### Calculs de l’ICP lors de l’utilisation d’une PIM horaire {#cpi-calculations-when-using-hour-based-pim}

si

```
Actual Hours > 0 THEN CPI = Total Budgeted Cost Work Performed / Actual Hours
```

Sinon

```
CPI = 1
```

* **Pour une tâche non parent :**

  ```
  Total Budgeted Cost Work Performed = Planned Hours * (Percent Complete / 100)
  ```

* **Pour une tâche parent :**
Total du coût budgété du travail réalisé = somme du champ de coût budgété total du travail réalisé pour toutes les tâches enfant directes.

* **Pour un projet :**
Total du coût budgété du travail réalisé = somme du champ de coût budgété total du travail réalisé pour toutes les tâches de niveau supérieur (tâches parent et autonomes).

Pour plus d’informations sur le total du « Coût budgété du travail effectué » (Budgeted Cost Work Performed, BCWP), consultez la section [Calculer le coût budgété du travail effectué (BCWP)](../../../manage-work/projects/project-finances/calculate-bcwp.md).

#### Calculs de l’ICP en utilisant la PIM basée sur les coûts {#cpi-calculations-when-using-cost-based-pim}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>CPI = (Planned Cost of Work Performed + Planned Cost of Incurred Expenses) / (Total Actual Cost + Actual Cost of Incurred Expenses) </code> </p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>NOTE: this used to be here before - above - but Anna sent me the one below. I kept the other one, although she is still researching its validity - see this issue: https://hub.workfront.com/issue/5fc7b1cf00012aeebf9e822db8ea2513/overview)</code> </p>
-->

si

```
Actual Labor Cost + Incurred Actual Expense Cost <> 0 THEN CPI = (Total Budgeted Cost Work Performed + Incurred Planned Expense Cost) / (Actual Labor Cost + Incurred Actual Expense Cost)
```



Sinon

```
CPI = 1
```

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>(NOTE: above: this used to say: CPI = CPI Labor, but Anna had me fix it on July 21, 2021)</code> </p>
-->

Les champs de ce calcul sont décrits ci-dessous :

```
Total Actual Cost = Actual (logged) Hours * Hourly Rate of assignees
```

```
Incurred Actual Expense Cost = Actual Cost
```

Les dépenses engagées sont les dépenses pour lesquelles le coût réel est supérieur à 0.

```
Planned Cost of Incurred Expenses = Total of Planned Cost of all incurred expenses
```



<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Old calculation - taken out by Lilit and replaced below: Planned Cost of Work Performed= (planned labor cost) * (percent complete) / 100 where planned labor cost is the planned hours allocated to assignees * their rates.)</p>
  -->

* Le coût budgété du travail effectué est calculé selon la formule suivante :

  ```
  Planned Cost of Work Performed = Planned cost * Percent Complete / 100
  ```

Le coût total budgété du travail effectué est calculé selon la formule suivante :

* **Pour une tâche non parent :**

  ```
  Total Budgeted Cost Work Performed = Planned Labor Cost * Percent Complete / 100
  ```

* **Pour une tâche parent :**

  ```
  Total Budgeted Cost Work Performed = SUM(Total Budgeted Cost Work Performed field from all direct child tasks)
  ```

* **Pour un projet :**

  ```
  Total Budgeted Cost Work Performed = SUM(Total Budgeted Cost Work Performed field for all top level tasks)
  ```



## Localiser l’ICP dans un projet ou une tâche

Vous pouvez afficher l’ICP d’un projet ou d’une tâche dans une liste ou un rapport de projet ou de tâche. Vous pouvez aussi l’afficher au niveau du projet ou de la tâche.

1. Accédez au projet ou à la tâche dont vous souhaitez afficher l’ICP.
1. Développez **Détails du projet** ou **Détails de la tâche** dans le panneau de gauche, selon que vous affichez l’ICP d’un projet ou d’une tâche.

1. Cliquez sur **Finances**.

   L’ICP s’affiche dans le champ **ICP/SPI/CSI**.

   ![](assets/cpi-on-project-nwe.png)
