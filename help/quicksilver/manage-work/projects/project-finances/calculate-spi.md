---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calculer l’Indice Horaire Performances (SPI)
description: L’index de performance de planification (SPI) décrit la relation entre le planning planifié et le planning réel.
author: Alina
feature: Work Management
exl-id: 38259774-f22b-4b69-9e22-5b541118a7de
source-git-commit: a55041ad5a6cd41cd11ec3ade27bf5227ae0ac47
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 23%

---

# Calculer l’Indice Horaire Performances (SPI)

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.)</p>
-->

L’index de performance de planification (SPI) décrit la relation entre le planning planifié et le planning réel. Adobe Workfront calcule SPI au niveau du projet et des tâches. Les chefs de projet examinent cette mesure pour déterminer si les tâches ou les projets sont actuellement suivis en amont ou en aval du planning.

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
   <td> <p>Afficher l’accès aux projets et aux données financières</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Afficher les autorisations du projet ou des autorisations supérieures avec les autorisations de Afficher le financement</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Planification de l’index de performance (SPI) - Aperçu

* [Ce que la valeur SPI indique](#what-the-spi-value-shows)
* [Comment Workfront calcule SPI](#how-workfront-calculates-spi)

### Ce que la valeur SPI indique {#what-the-spi-value-shows}

Les chefs de projet comprennent qu’une valeur SPI de 1 signifie que le projet est planifié ou planifié.  Les valeurs supérieures à 1 indiquent qu’un projet est en avance sur le planning et les valeurs inférieures à 1 indiquent qu’un projet est en retard sur le planning.  Plus on s&#39;éloigne de 1, plus on s&#39;éloigne du plan.

| **Valeur SPI** | **Indication de &quot;On Schedule&quot;** |
|---|---|
| 1 | À l’heure prévue ou planifiée |
| > 1 (supérieur à 1) | Avant le planning |
| &lt; 1 (moins de 1) | En arrière-plan de la planification |

{style="table-layout:auto"}

### Comment Workfront calcule SPI  {#how-workfront-calculates-spi}

Workfront calcule SPI selon la formule suivante :

```
SPI = (Total Planned Hours x % Complete) / Planned Hours Scheduled to Date*
```

*&#42;Si les heures planifiées sont planifiées avec date = 0, SPI = 1*.

La planification des heures est calculée à la minute lorsque vous effectuez les calculs. Il indique le nombre d’heures planifiées planifiées à la date actuelle. Il peut être recalculé automatiquement lorsque vous modifiez les données financières pour qu&#39;elles soient exactes. Aucun champ dans Workfront n’indique cette valeur.

Par exemple, si vous avez un projet avec une tâche qui comporte 10 heures planifiées et une durée de 10 jours, la planification des heures planifiées à date du 5e jour est de 5. 

## Localisation de SPI dans un projet ou une tâche

1. Accédez au projet ou à la tâche où vous souhaitez afficher SPI.
1. Selon que vous souhaitez afficher SPI sur un projet ou une tâche, effectuez l’une des opérations suivantes :

   1. Cliquez sur **Détails du projet** dans le panneau de gauche, puis affichez la zone **Finance**.

   1. Cliquez sur **Détails de la tâche** dans le panneau de gauche, puis affichez la zone **Finance**.

      ![](assets/spi-on-project-nwe.png)

1. Recherchez le champ **CPI/ SPI/ CSI** .
