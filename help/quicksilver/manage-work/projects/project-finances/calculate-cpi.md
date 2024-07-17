---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calculer l’Indice Coûts Performances (IPC)
description: L’indice de performance des coûts (IPC) décrit la relation au niveau du projet ou de la tâche entre le coût prévu et le coût réel. Les chefs de projet examinent cette mesure pour identifier les tâches ou les projets qui effectuent actuellement le suivi sous ou sur-coût à un moment donné.
author: Alina
feature: Work Management
exl-id: 7f2efe26-7292-482d-986c-2d2077a7ca52
source-git-commit: a55041ad5a6cd41cd11ec3ade27bf5227ae0ac47
workflow-type: tm+mt
source-wordcount: '644'
ht-degree: 16%

---

# Calculer l’Indice Coûts Performances (IPC)

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.)</p>
-->

L’indice de performance des coûts (IPC) décrit la relation au niveau du projet ou de la tâche entre le coût prévu et le coût réel. Les chefs de projet examinent cette mesure pour identifier les tâches ou les projets qui effectuent actuellement le suivi sous ou sur-coût à un moment donné. Le coût peut être mesuré en heures ou en dollars, selon votre méthode d’index de performance (PIM). Pour plus d’informations sur la définition de la méthode d’index de performance, voir [Définition de la méthode d’index de performance (PIM)](../../../manage-work/projects/project-finances/set-pim.md).

Seules les organisations qui ont besoin d’une entrée dans le temps peuvent utiliser l’IPC. En outre, les valeurs PIM basées sur les coûts ne sont exactes que dans les organisations qui ont défini des taux de coût pour les personnes désignées pour des tâches (rôles de tâche ou utilisateurs).

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Révision ou supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Afficher l’accès aux projets et aux données financières</p> <p> Si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Afficher les autorisations du projet ou des autorisations supérieures avec les autorisations de Afficher le financement</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Présentation de l’indice de performance des coûts (IPC)

* [La valeur IPC](#the-cpi-value)
* [Méthode de calcul de l’IPC](#how-cpi-is-calculated)

### La valeur de l’indice des prix à la consommation {#the-cpi-value}

Les chefs de projet comprennent qu’une valeur IPC de 1 signifie que le projet est exactement conforme au budget. Les valeurs supérieures à 1 indiquent qu’un projet est sous-budget (moins d’heures ou de dépenses ont été enregistrées que prévu initialement) et les valeurs inférieures à 1 indiquent qu’un projet est surchargé de budget (plus d’heures ou de dépenses ont été enregistrées que prévu initialement). Plus on s&#39;éloigne de 1, plus on s&#39;éloigne du plan.

| **Valeur IPC** | **Indication sur le budget** |
|---|---|
| 1 | Sur plan ou budget |
| > 1 (supérieur à 1) | Sous budget |
| &lt; 1 (moins de 1) | Au-dessus du budget |


### Méthode de calcul de l’IPC {#how-cpi-is-calculated}

Dans Adobe Workfront, le calcul de l’IPC dépend de la méthode d’index de performance sélectionnée pour le projet. Pour plus d’informations sur la définition de la méthode d’index de performance, voir [Définition de la méthode d’index de performance (PIM)](../../../manage-work/projects/project-finances/set-pim.md).

* [Calculs de l’indice des prix à la consommation lors de l’utilisation d’un PIM basé sur l’heure](#cpi-calculations-when-using-hour-based-pim)
* [Calculs IPC lors de l’utilisation d’un PIM basé sur les coûts](#cpi-calculations-when-using-cost-based-pim)

#### Calculs des IPC lors de l’utilisation d’un PIM horaire {#cpi-calculations-when-using-hour-based-pim}

si

```
Actual Hours > 0 THEN CPI = Total Budgeted Cost Work Performed / Actual Hours
```

Sinon

```
CPI = 1
```

* **Pour une tâche non parent :**

  ```
  Total Budgeted Cost Work Performed = Planned Hours * (Percent Complete / 100)
  ```

* **Pour une tâche parente :**
Total des tâches de coût budgétisées exécutées = somme du champ Total des tâches de coût budgétisées exécutées pour toutes les tâches enfants directes.

* **Pour un projet :**
Coût total des tâches budgétaires exécutées = somme du champ Total des tâches budgétaires exécutées pour toutes les tâches de niveau supérieur (parents et tâches autonomes).

Pour plus d’informations sur le total des travaux de coûts budgétés réalisés (BCWP), voir [Calculate Budget Cost Work Performance (BCWP)](../../../manage-work/projects/project-finances/calculate-bcwp.md).

#### Calculs IPC lors de l’utilisation d’un PIM basé sur les coûts {#cpi-calculations-when-using-cost-based-pim}

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

Les champs de ce calcul sont décrits ci-dessous :

```
Total Actual Cost = Actual (logged) Hours * Hourly Rate of assignees
```

```
Incurred Actual Expense Cost = Actual Cost
```

Dépenses engagées désigne les dépenses pour lesquelles le coût réel est supérieur à 0

```
Planned Cost of Incurred Expenses = Total of Planned Cost of all incurred expenses
```



<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Old calculation - taken out by Lilit and replaced below: Planned Cost of Work Performed= (planned labor cost) * (percent complete) / 100 where planned labor cost is the planned hours allocated to assignees * their rates.)</p>
  -->

* Le coût planifié du travail effectué est calculé selon la formule suivante :

  ```
  Planned Cost of Work Performed = Planned cost * Percent Complete / 100
  ```

Le coût total du travail effectué est calculé comme suit :

* **Pour une tâche non parent :**

  ```
  Total Budgeted Cost Work Performed = Planned Labor Cost * Percent Complete / 100
  ```

* **Pour une tâche parente :**

  ```
  Total Budgeted Cost Work Performed = SUM(Total Budgeted Cost Work Performed field from all direct child tasks)
  ```

* **Pour un projet :**

  ```
  Total Budgeted Cost Work Performed = SUM(Total Budgeted Cost Work Performed field for all top level tasks)
  ```



## Localisation de l’IPC dans un projet ou une tâche

Vous pouvez afficher l’IPC d’un projet ou d’une tâche dans un projet, une liste de tâches ou un rapport. En outre, vous pouvez l’afficher au niveau du projet ou de la tâche.

1. Accédez au projet ou à la tâche où vous souhaitez afficher l’IPC.
1. Développez **Détails du projet** ou **Détails de la tâche** dans le panneau de gauche, selon que vous affichez l’IPC d’un projet ou d’une tâche.

1. Cliquez sur **Finance**.

   L’IPC s’affiche dans le champ **CPI/ SPI/ CSI**.

   ![](assets/cpi-on-project-nwe.png)
