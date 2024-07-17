---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calculer l’estimation à l’achèvement (EAC)
description: En tant que mesure de performances, l’estimation à la fin (EAC) représente le coût total prévu de votre projet ou tâche une fois qu’elle s’est terminée.
author: Alina
feature: Work Management
exl-id: 9061fa56-cff3-4fe2-866e-1fdda9d43efc
source-git-commit: a55041ad5a6cd41cd11ec3ade27bf5227ae0ac47
workflow-type: tm+mt
source-wordcount: '878'
ht-degree: 11%

---

# Calculer l’estimation à l’achèvement (EAC)

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link!) </p>
-->

En tant que mesure de performances, l’estimation à la fin (EAC) représente le coût total prévu de votre projet ou tâche une fois qu’elle s’est terminée.

Il vous permet de définir la manière dont la valeur du contrôle d’accès doit être calculée. 

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
   <td> <p>Afficher l’accès aux projets et aux données financières</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Afficher les autorisations du projet ou des autorisations supérieures avec les autorisations de Afficher le financement</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Définition de la méthode de calcul du contrôle d’accès

Dans le cadre des préférences du système de projet, l’administrateur Adobe Workfront peut définir la manière de calculer le contrôle d’accès. Le calcul du taux d&#39;effet élévateur cumulé peut se faire de l&#39;une des deux façons suivantes :

* [Calculer au niveau du projet](#calculate-at-the-project-level)
* [Cumul à partir de tâches et de sous-tâches](#roll-up-from-tasks-and-subtasks)

Pour plus d’informations sur la configuration des préférences de projet dans Workfront, y compris sur la manière de calculer l’estimation à la fin, voir [Configuration des préférences de projet à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

En tant que chef de projet, vous pouvez également modifier cette préférence au niveau du projet, dans le sous-onglet Finance du projet. Pour plus d’informations sur la modification du sous-onglet Finance d’un projet, voir [Gestion des informations dans la zone Finance du projet](../../../manage-work/projects/project-finances/manage-project-finance-area.md).

### Calculer au niveau du projet {#calculate-at-the-project-level}

Le champ EAC de la tâche et du projet parents est déterminé en saisissant les heures réelles/le coût réel de la main-d’oeuvre dans les formules EAC. Ce calcul inclut les Heures/coûts réels et les dépenses ajoutées directement à la tâche ou au projet parent.

### Cumul à partir de tâches et de sous-tâches {#roll-up-from-tasks-and-subtasks}

Les champs de contrôle d’accès de la tâche parent et du projet sont déterminés en totalisant les champs de contrôle d’accès de chaque tâche enfant. Ce calcul exclut les Heures/coûts réels et les dépenses ajoutées directement à la tâche ou au projet parent.

## Comment calculer le CCE en fonction de la méthode d’index de performance (PIM)

Dans Workfront, le calcul du contrôle d’accès dépend de la méthode d’index de performance (PIM) sélectionnée du projet. Pour plus d’informations sur la définition du PIM pour votre système ou votre projet, voir [Définition de la méthode d’index de performance (PIM)](../../../manage-work/projects/project-finances/set-pim.md).

* [Calculer le CAE à l’aide de la PIM basée sur l’heure](#calculate-eac-using-hour-based-pim)
* [Calcul des EAC à l’aide d’un PIM basé sur les coûts](#calculate-eac-using-cost-based-pim)

### Calcul du contrôle d’accès à l’aide d’un PIM horaire {#calculate-eac-using-hour-based-pim}

```
EAC = Total Planned Hours / CPI*
```

&#42;Si l’indice de performance des coûts [Calculer l’indice de performance des coûts (IPC)](../../../manage-work/projects/project-finances/calculate-cpi.md) = 0, EAC = Total heures planifiées + heures réelles. Cela se produit lorsque des heures ont été capturées, mais que le projet/la tâche est terminé à 0 %.

Pour plus d’informations sur le calcul de l’IPC, voir [Calculate Cost Performance Index (CPI)](../../../manage-work/projects/project-finances/calculate-cpi.md).

### Calcul des EAC à l’aide d’un PIM basé sur les coûts {#calculate-eac-using-cost-based-pim}

Le taux d’intérêt d’un projet est calculé à l’aide de la formule suivante :

```
EAC = EAC Labor + EAC Expense 
```

<pre>EAC Labor =  <em>IF</em> Main-d’oeuvre CPI &lt;&gt; 0 ALORS MAIN-D’Oeuvre = Coût de main-d’oeuvre planifié/Oeuvre IPC</pre><pre><em>ELSE</em> EAC  Travail = Coût du travail planifié + coût réel du travail</pre><pre>IPC/Travail = IF Coût réel de la main-d’oeuvre &lt;&gt; 0 ALORS IPC/Main-d’oeuvre = TotalBudgetCostWorkPerformance / Coût réel de la main-d’oeuvre</pre><pre>ELSE CPI Labor = 1 </pre>Les champs suivants sont pris en compte dans le calcul de l'EAC :

* Coût total des travaux réalisés (BCWP) = résultat de la multiplication du coût budgété du travail planifié (coût budgété) et du pourcentage de la tâche qui a été effectuée jusqu&#39;à présent.

  Pour plus d’informations sur le total des travaux de coûts budgétés réalisés (BCWP), voir [Calculate Budget Cost Work Performance (BCWP)](../../../manage-work/projects/project-finances/calculate-bcwp.md).

   * **Pour une tâche non parent :**

     ```
     Total Budgeted Cost Work Performed = Planned Hours * (Percent Complete/100)
     ```

   * **Pour une tâche parente :**
Total des tâches de coût budgétisées exécutées = somme du champ Total des tâches de coût budgétisées exécutées pour toutes les tâches enfants directes.

   * **Pour un projet :**
Coût total des tâches budgétaires exécutées = somme du champ Total des tâches budgétaires exécutées pour toutes les tâches de niveau supérieur (parents et tâches autonomes). 

* Frais de CAE = résultat de l’ajout du coût des dépenses réelles encourues au coût des dépenses prévues non encourues. Elle est calculée selon la formule suivante :

  ```
  EAC Expense = Incurred Actual Expense Cost + Not Incurred Planned Expense
  ```

   * Coût des dépenses réelles engagées = somme du champ Montant planifié pour toutes les dépenses pour lesquelles le champ Montant réel est supérieur à 0. Par exemple, si vous créez une dépense pour la Tâche 1 et que vous saisissez 500,00 $ dans le champ Montant planifié et un montant > 0 dans le champ Montant réel (soit 600,00 $), le Coût des dépenses planifiées engagées pour cette tâche est de 500,00 $.
   * Dépenses prévues non exécutées = Somme du champ Montant planifié pour toutes les dépenses pour lesquelles le champ Montant réel = 0. Par exemple, si vous créez deux dépenses pour la tâche 1 où, pour la première dépense, la valeur du champ Montant planifié est de 500,00 $ et la valeur du montant réel est de 600,00 $ et, pour la seconde dépense, la valeur du champ Montant planifié est de 300,00 $ et la valeur du champ Montant réel est de 0,00 $, la valeur de Les frais pour cette tâche sont de 300 $. 

## Localisation de l’EAC dans un projet ou une tâche

1. Accédez au projet ou à la tâche où vous souhaitez afficher le contrôle d’accès.
1. Développez **Détails du projet** ou **Détails des tâches** dans le panneau de gauche du projet ou de la tâche, selon l’emplacement où vous affichez le contrôle EAC.

1. Cliquez sur **Finance**. 

   La valeur EAC s’affiche dans le champ **Estimation à l’achèvement** .

   ![](assets/eac-highlighted-on-project-350x112.png)
