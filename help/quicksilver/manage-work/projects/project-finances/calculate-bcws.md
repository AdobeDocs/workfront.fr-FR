---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calculer le coût budgété du travail prévu (BCWS)
description: Également appelé Valeur planifiée, le coût budgété du travail planifié (BCWS) est une mesure de performances du projet qui représente le montant de la tâche qui doit être terminée au moment où cette mesure est calculée.
author: Alina
feature: Work Management
exl-id: b9a36333-9430-42bd-99dd-3ad82803b633
source-git-commit: 1d5de5ff0ebebd84482507c71730cfbd05c513a5
workflow-type: tm+mt
source-wordcount: '649'
ht-degree: 20%

---

# Calculer le coût budgété du travail prévu (BCWS)

## Présentation du coût des travaux planifiés (BCWS)

Également appelé Valeur planifiée, le coût budgété du travail planifié (BCWS) est une mesure de performances du projet qui représente le montant de la tâche qui doit être terminée au moment où cette mesure est calculée.

Adobe Workfront calcule le coût du travail planifié (BCWS) budgété pour les projets et les tâches.

Tenez compte de ce qui suit lorsque vous passez en revue les valeurs du BCWS sur une tâche ou un projet :

* Workfront calcule le BCWS d’une tâche en fonction de votre configuration pour la méthode d’index de performance (PIM) du projet.

  Vous pouvez configurer votre projet pour calculer le PIM en heures ou en coûts, et le BCWS est également calculé à l’aide des mêmes valeurs.

  Pour plus d’informations sur la configuration du mode de calcul du BCWS, consultez la section [Configuration du mode de calcul du BCWS](#configure-how-bcws-is-calculated) de cet article.

* Workfront calcule le BCWS d’un projet en ajoutant toutes les valeurs du BCWS de toutes les tâches parentes et des tâches individuelles du projet.

  Les valeurs des tâches enfants ne sont pas ajoutées au BCWS du projet.

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux projets</p> <p>Si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations de gestion pour le projet</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Configuration du calcul du BCWS {#configure-how-bcws-is-calculated}

Vous pouvez configurer le calcul du BCWS en heures ou en coûts en configurant la méthode de calcul de l’index de performance (PIM) du projet.

1. Accédez à un projet et cliquez sur **Détails du projet** dans le panneau de gauche.
1. Dans la zone **Finance**, recherchez le champ **Méthode d’index de performance** et double-cliquez dessus pour le modifier.

   ![](assets/pim-options-hour-cost-based-nwe.png)

1. Sélectionnez l’une des options suivantes :

   | Option | Exécution du calcul |
   |---|---|
   | Basé sur les heures | Workfront calcule le BCWS à l’aide des Heures planifiées des tâches. |
   | Basé sur les coûts | Workfront calcule le CWS à l’aide du coût planifié des tâches. |


1. Cliquez sur **Enregistrer les modifications**.

   Le BCWS des tâches sur le projet est calculé en heures ou en coûts.

## Calculer BCWS

Workfront calcule le coût du travail planifié (BCWS) budgété pour les tâches ou les projets à l’aide des formules suivantes :

```
Task BCWS = Planned Percent Complete x Task Budget
```

```
Project BCWS = SUM(BCWS values of all parent and individual tasks)
```

Les valeurs utilisées dans ce calcul sont les suivantes :

| Valeur utilisée | Description de la valeur utilisée |
|---|---|
| Pourcentage prévu terminé | C&#39;est ce que devrait être le pourcentage de réalisation de la tâche en regardant le temps écoulé entre le début de la tâche et aujourd&#39;hui. |
| Budget des tâches | Il s’agit de la valeur de Heures planifiées ou Coût planifié de la tâche. |

Par exemple, si nous sommes le 12 février aujourd’hui et qu’une tâche est planifiée pour durer du 10 au 20 février, la tâche doit être terminée à 20 % aujourd’hui. Si le budget de la tâche (coût planifié) est de 10 000 $, le CWS de la tâche est :

```
Task BCWS = 20% x $10,000 = $2,000
```

## Localisation du BCWS pour un projet ou une tâche

Vous pouvez afficher la valeur du Coût budgétaire des travaux planifiés dans un rapport ou une liste, en ajoutant la colonne BCWS à votre vue.

1. Accédez à une liste de tâches ou de projets.
1. Développez le menu **Affichage** et sélectionnez **Nouvelle vue** ou **Personnaliser la vue**.

1. Cliquez sur **Ajouter une colonne**.
1. Dans le champ **Afficher dans cette colonne :**, commencez à saisir **BCWS** et cliquez pour le sélectionner lorsqu’il s’affiche dans la liste.

   ![](assets/bcws-in-project-view.png)

1. Cliquez sur **Enregistrer la vue**.
1. Le champ **BCWS** s’affiche dans la vue.
