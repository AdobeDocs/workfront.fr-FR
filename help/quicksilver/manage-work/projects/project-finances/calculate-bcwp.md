---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calculer le coût des travaux réalisés budgétisés (BCWP)
description: Connue également sous le nom de Valeur acquise, le coût budgété du travail effectué (BCWP) est une mesure de performances de projet qui représente le montant de la tâche qui a été réellement terminée au moment où cette mesure est calculée.
author: Alina
feature: Work Management
exl-id: 203709a7-e522-4875-b3eb-40b967a938ec
source-git-commit: 1d5de5ff0ebebd84482507c71730cfbd05c513a5
workflow-type: tm+mt
source-wordcount: '620'
ht-degree: 0%

---

# Calculer le coût des travaux réalisés budgétisés (BCWP)

## Présentation du coût du travail effectué (BCWP) budgété

Connue également sous le nom de Valeur acquise, le coût budgété du travail effectué (BCWP) est une mesure de performances de projet qui représente le montant de la tâche qui a été réellement terminée au moment où cette mesure est calculée.

Adobe Workfront calcule le coût du travail effectué (BCWP) budgété pour les projets et les tâches.

Tenez compte de ce qui suit lorsque vous passez en revue les valeurs du BCWP sur une tâche ou un projet :

* Workfront calcule le BCWP d’une tâche en fonction de votre configuration pour la méthode d’index de performance (PMI) du projet.

   Vous pouvez configurer votre projet pour calculer le PMI en heures ou en coûts, et le BCWP est également calculé à l’aide des mêmes valeurs.

   Pour plus d’informations sur la configuration du mode de calcul du BCWP, voir la section [Configurer le calcul du BCWP](#configure-how-bcwp-is-calculated) dans cet article.

* Workfront calcule le BCWP d’un projet en ajoutant toutes les valeurs du BCWP de toutes les tâches parentes et des tâches individuelles du projet.

   Les valeurs des tâches enfants ne sont pas ajoutées au BCWP du projet.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modifier l’accès aux projets</p> <p>Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gestion des autorisations pour le projet</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Configurer le calcul du BCWP {#configure-how-bcwp-is-calculated}

Vous pouvez configurer le calcul du BCWP en heures ou en coûts en configurant la méthode de calcul de l’index de performance (PIM) du projet.

1. Accédez à un projet et développez **Détails du projet** dans le panneau de gauche.
1. Dans le **Finance** , recherchez la **Méthode d’index de performance** et double-cliquez pour l’éditer.

   ![](assets/pim-options-hour-cost-based-nwe.png)

1. Sélectionnez l’une des options suivantes :

   | Option | Exécution du calcul |
   |---|---|
   | Basé sur les heures | Workfront calcule le BCWP à l’aide des Heures planifiées des tâches. |
   | Basé sur les coûts | Workfront calcule le BCWP en utilisant le coût planifié des tâches. |

1. Cliquez sur **Enregistrer les modifications**.

Le BCWP des tâches sur le projet est calculé en heures ou en coûts.

## Calculer BCWP

Workfront calcule le coût budgété du travail effectué (BCWP) pour une tâche ou un projet à l’aide des formules suivantes :

```
Task BCWP = Actual Percent Complete x Task Budget
```

```
Project BCWP = SUM(BCWP values of all parent and individual tasks)
```

Les valeurs suivantes sont utilisées dans ce calcul :

| Valeur utilisée | Description de la valeur utilisée |
|---|---|
| Pourcentage réel terminé | Il s’agit du pourcentage réel d’achèvement de la tâche tel qu’il apparaît dans Workfront. |
| Budget des tâches | Il s’agit de la valeur de Heures planifiées ou Coût planifié de la tâche. |

Par exemple, si le pourcentage réel terminé de la tâche est de 25 % et que le budget de la tâche ou le coût planifié est de 10 000 $, le BCWP de la tâche est :

```
BCWP = 25% x $10,000 = $2,500
```

## Localisation du BCWP d’un projet ou d’une tâche

Vous pouvez afficher la valeur du Coût du travail budgété effectué dans un rapport ou une liste, en ajoutant la colonne BCWP à votre vue.

1. Accédez à une liste de tâches ou de projets.
1. Développez l’objet **Affichage** et sélectionnez **Nouvelle vue** ou **Vue Personnaliser**.

1. Cliquez sur **Ajouter une colonne**.
1. Dans le **Afficher dans cette colonne :** saisie de champ **BCWP** et cliquez pour la sélectionner lorsqu’elle s’affiche dans la liste.

   ![](assets/bcwp-project-view.png)

1. Cliquez sur **Enregistrer la vue**.
1. Le champ BCWP s’affiche dans la vue.
