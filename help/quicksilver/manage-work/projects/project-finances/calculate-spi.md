---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calculer l’indice de performances de planification (SPI)
description: L’indice de performance du planning (SPI) décrit la relation entre le planning prévu et le planning réel.
author: Lisa
feature: Work Management
exl-id: 38259774-f22b-4b69-9e22-5b541118a7de
source-git-commit: 23a4d055871c9138818e70fa1cd936581dbd7552
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 97%

---

# Calculer l’indice de performances de planification (SPI)

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.)</p>
-->

L’indice de performance du planning (SPI) décrit la relation entre le planning prévu et le planning réel. Adobe Workfront calcule le SPI au niveau du projet et des tâches. Les responsables de projet examinent cette mesure pour déterminer si les tâches ou les projets sont actuellement en avance ou en retard sur le planning.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Package Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td>Licence Adobe Workfront</td> 
   <td>
   <p>Léger ou supérieur</p>
   <p>Révision ou supérieur</p></td>  
  </tr> 
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td>Afficher l’accès aux projets et aux données financières</td> 
  </tr> 
  <tr> 
   <td>Autorisations d’objet</td> 
   <td>Autorisations Afficher ou supérieures pour le projet avec les autorisations Afficher Finance</td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vue d’ensemble de l’indice de performance du planning (SPI)

* [Ce que la valeur du SPI indique](#what-the-spi-value-shows)
* [Calcul du SPI par Workfront](#how-workfront-calculates-spi)

### Signification de la valeur du SPI {#what-the-spi-value-shows}

Les responsables de projet comprennent qu’une valeur de SPI de 1 signifie que le projet est prévu ou planifié. Les valeurs supérieures à 1 indiquent qu’un projet est en avance sur le planning et les valeurs inférieures à 1 indiquent qu’un projet est en retard sur le planning. Plus on s’éloigne de 1, plus on s’éloigne du plan.

| **Valeur de SPI** | **Indication de « Dans les temps »** |
|---|---|
| 1 | À l’heure prévue ou planifiée |
| > 1 (supérieur à 1) | En avance sur le planning |
| &lt; 1 (inférieur à 1) | En retard sur le planning |

{style="table-layout:auto"}

### Calcul du SPI par Workfront  {#how-workfront-calculates-spi}

Workfront calcule le SPI selon la formule suivante :

```
SPI = (Total Planned Hours x % Complete) / Planned Hours Scheduled to Date*
```

*&#42;Si le nombre d’heures prévues planifiées pour la date = 0, SPI = 1*.

Le nombre d’heures prévues planifiées pour la date est calculé à la minute lorsque vous effectuez les calculs. Il indique le nombre d’heures prévues planifiées pour la date actuelle.Il peut être recalculé automatiquement lorsque vous modifiez les données financières pour qu’elles soient exactes. Aucun champ dans Workfront n’indique cette valeur.

Par exemple, si vous avez un projet avec une tâche qui comporte 10 heures prévues et une durée de 10 jours, le nombre d’heures prévues planifiées pour le 5ème jour est de 5. 

## Localiser le SPI dans un projet ou une tâche

1. Accédez au projet ou à la tâche où vous souhaitez afficher le SPI.
1. Selon que vous souhaitez afficher le SPI sur un projet ou une tâche, effectuez l’une des opérations suivantes :

   1. Cliquez sur **Détails du projet** dans le panneau de gauche, puis affichez la zone **Finances**.

   1. Cliquez sur **Détails de la tâche** dans le panneau de gauche, puis affichez la zone **Finances**.

      ![IHP sur le projet](assets/spi-on-project-nwe.png)

1. Recherchez le champ **IPC/SPI/CSI**.
