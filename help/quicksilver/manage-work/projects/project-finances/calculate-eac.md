---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calculer l’estimation à l’achèvement (CRE)
description: L’estimation à l’achèvement en tant que mesure de performance, représente le coût total projeté de votre projet ou tâche lorsqu’il est terminé.
author: Alina
feature: Work Management
exl-id: 9061fa56-cff3-4fe2-866e-1fdda9d43efc
source-git-commit: a55041ad5a6cd41cd11ec3ade27bf5227ae0ac47
workflow-type: tm+mt
source-wordcount: '878'
ht-degree: 100%

---

# Calculer l’estimation à l’achèvement (CRE)

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link!) </p>
-->

L’estimation à l’achèvement en tant que mesure de performance, représente le coût total projeté de votre projet ou tâche lorsqu’il est terminé.

Ce paramètre vous permet de définir la manière dont l’estimation à l’achèvement doit être calculée. 

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Révision ou supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Afficher l’accès aux projets et aux données financières</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si votre niveau d’accès est soumis à des restrictions supplémentaires. Pour plus d’informations sur la façon dont l’administration Workfront peut modifier votre niveau d’accès, consultez la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations Afficher ou supérieures pour le projet avec les autorisations Afficher Finance</p> <p>Pour plus d’informations sur les demandes d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès à des objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Définir la méthode de calcul de l’estimation à l’achèvement

Dans le cadre des préférences du système de projet, l’équipe d’administration Adobe Workfront peut définir la méthode de calcul de l’estimation à l’achèvement. Le calcul de l’estimation à l’achèvement peut se faire de l’une des deux façons suivantes :

* [Calculer au niveau du projet](#calculate-at-the-project-level)
* [Regrouper depuis les tâches/sous-tâches](#roll-up-from-tasks-and-subtasks)

Pour plus d’informations sur la configuration des préférences de projet dans Workfront, y compris sur la manière de calculer l’estimation à l’achèvement, consultez la section [Configurer des préférences de projet à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

En tant que gestionnaire de projet, vous pouvez également modifier cette préférence au niveau du projet, dans le sous-onglet « Finances » du projet. Pour plus d’informations sur la modification du sous-onglet « Finances » d’un projet, consultez la section [Gérer les informations dans la zone « Finances » du projet](../../../manage-work/projects/project-finances/manage-project-finance-area.md).

### Calculer au niveau du projet {#calculate-at-the-project-level}

Les estimations à l’achèvement pour la tâche et le projet parent sont déterminées en entrant les heures effectives/coûts réels de main-d’œuvre dans les formules de calcul des estimations à l’achèvement. Ce calcul inclut les heures effectives/les coûts et les dépenses ajoutés directement à la tâche parent ou au projet.

### Regrouper depuis les tâches/sous-tâches {#roll-up-from-tasks-and-subtasks}

Les estimations à l’achèvement de la tâche parent et du projet sont déterminées en additionnant les estimations à l’achèvement de chaque tâche enfant. Ce calcul inclut les heures effectives/les coûts et les dépenses ajoutés directement à la tâche ou au projet parent.

## Comment calculer l’estimation à l’achèvement en fonction de la méthode d’indice de performances (PIM)

Dans Workfront, le calcul de l’estimation à l’achèvement dépend de la méthode d’indice de performances (PIM) sélectionnée du projet. Pour plus d’informations sur la définition de l’estimation à l’achèvement pour votre système ou votre projet, consultez la section [Définir la méthode d’indice de performances (PIM)](../../../manage-work/projects/project-finances/set-pim.md).

* [Calculer l’estimation à l’achèvement à l’aide d’un PIM basé sur les heures](#calculate-eac-using-hour-based-pim)
* [Calculer l’estimation à l’achèvement à l’aide d’un PIM basé sur les coûts](#calculate-eac-using-cost-based-pim)

### Calculer l’estimation à l’achèvement à l’aide d’un PIM basé sur les heures {#calculate-eac-using-hour-based-pim}

```
EAC = Total Planned Hours / CPI*
```

&#42;Si l’indice Coûts Performances [Calculer l’indice Coûts Performances (ICP)](../../../manage-work/projects/project-finances/calculate-cpi.md) = 0, Estimation à l’achèvement = Total des heures planifiées + heures effectives. Cela se produit lorsque des heures ont été enregistrées, mais que le projet/la tâche est terminé à 0 %.

Pour plus d’informations sur le calcul de l’ICP, consultez la section [Calculer l’indice Coûts Performances (IPC)](../../../manage-work/projects/project-finances/calculate-cpi.md).

### Calculer l’estimation à l’achèvement à l’aide d’un PIM basé sur les coûts {#calculate-eac-using-cost-based-pim}

L’estimation à l’achèvement d’un projet est calculée à l’aide de la formule suivante :

```
EAC = EAC Labor + EAC Expense 
```

<pre>Coût de main-d’œuvre de l’estimation à l’achèvement = <em>IF</em> ICP du coût de main-d’œuvre &lt;&gt; 0 THEN Coût de main-d’œuvre Estimation à l’achèvement = Coût prévu de main-d’œuvre/ICP de la main-d’œuvre</pre><pre><em>ELSE</em> Coût de main-d’œuvre Estimation à l’achèvement = Coût prévu de main-d’œuvre + Coût réel de main-d’œuvre</pre><pre>ICP de la main-d’œuvre = IF Coût réel de main-d’oeuvre &lt;&gt; 0 THEN ICP de la main-d’œuvre = TotalBudgetCostWorkPerformance/Coût réel de main-d’oeuvre</pre><pre>ELSE ICP de la main-d’œuvre = 1 </pre>Les champs suivants sont pris en compte dans le calcul de l’estimation à l’achèvement :

* Coût total budgété du travail effectué (BCWP) = résultat de la multiplication du coût budgété du travail prévu (coût budgété) et du pourcentage de la tâche qui a été effectué jusqu’à présent.

  Pour plus d’informations sur le coût total budgété du travail effectué (BCWP), voir [Calculer le coût budgété du travail effectué (BCWP)](../../../manage-work/projects/project-finances/calculate-bcwp.md).

   * **Pour une tâche non parent :**

     ```
     Total Budgeted Cost Work Performed = Planned Hours * (Percent Complete/100)
     ```

   * **Pour une tâche parent :**
Coût total budgété du travail effectué (BCWP) = somme du champ Coût total budgété du travail effectué pour toutes les tâches enfant directes.

   * **Pour un projet :**
Coût total budgété du travail effectué = somme du champ Coût total budgété du travail effectué pour toutes les tâches de niveau supérieur (parent et tâches autonomes).

* Dépenses Estimation à l’achèvement = résultat de l’ajout du Coût réel des dépenses engagées au Montant des dépenses prévues non engagées. Elles sont calculées selon la formule suivante :

  ```
  EAC Expense = Incurred Actual Expense Cost + Not Incurred Planned Expense
  ```

   * Coût réel des dépenses engagées = somme du champ Montant prévu pour toutes les dépenses pour lesquelles le champ Montant réel est > 0. Par exemple, si vous créez une dépense pour la Tâche 1 et que vous saisissez 500 $ dans le champ Montant prévu et un montant > 0 dans le champ Montant réel (par ex. 600 $), le Montant des dépenses prévues engagées pour cette tâche est de 500 $.
   * Dépenses prévues non engagées = somme du champ Montant prévu pour toutes les dépenses pour lesquelles le champ Montant réel = 0. Par exemple, si vous créez deux dépenses pour la Tâche 1 où, pour la première dépense, la valeur du champ Montant prévu est de 500 $ et la valeur du Montant réel est de 600 $ et, pour la seconde dépense, la valeur du champ Montant prévu est de 300 $ et la valeur du champ Montant réel est de 0 $, la valeur des Dépenses prévues non engagées pour cette tâche est de 300 $. 

## Localiser l’estimation à l’achèvement dans un projet ou une tâche

1. Accédez au projet ou à la tâche pour lequel vous souhaitez afficher l’estimation à l’achèvement.
1. Développez **Détails du projet** ou **Détails des tâches** dans le panneau de gauche du projet ou de la tâche, selon l’emplacement d’affichage de l’estimation à l’achèvement.

1. Cliquez sur **Finances**.

   La valeur de l’estimation à l’achèvement s’affiche dans le champ **Estimation à l’achèvement**.

   ![](assets/eac-highlighted-on-project-350x112.png)
