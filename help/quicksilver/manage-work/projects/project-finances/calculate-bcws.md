---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calculer le coût budgété du travail prévu (BCWS)
description: Également appelé Valeur prévue, le coût budgété du travail prévu (BCWS) est une mesure de performances du projet qui représente le montant de la tâche qui devrait avoir été achevée au moment où cette mesure est calculée.
author: Lisa
feature: Work Management
exl-id: b9a36333-9430-42bd-99dd-3ad82803b633
source-git-commit: 6afa65f921864403c10541d283ef717dce81aed7
workflow-type: tm+mt
source-wordcount: '615'
ht-degree: 100%

---

# Calculer le coût budgété du travail prévu (BCWS)

## Vue d’ensemble du coût budgété du travail prévu (BCWS)

Également appelé Valeur prévue, le coût budgété du travail prévu (BCWS) est une mesure de performances du projet qui représente le montant de la tâche qui devrait avoir été achevée au moment où cette mesure est calculée.

Adobe Workfront calcule le coût budgété du travail prévu (BCWS) pour les projets et les tâches.

Tenez compte des éléments suivants lorsque vous passez en revue les valeurs du coût budgété du travail prévu sur une tâche ou un projet :

* Workfront calcule le coût budgété du travail prévu d’une tâche en fonction de votre configuration de la méthode d’indice de performances (PIM) du projet.

  Vous pouvez configurer votre projet pour calculer la PIM en heures ou en coûts, et le coût budgété du travail prévu est également calculé à l’aide des mêmes valeurs.

  Pour plus d’informations sur la configuration du mode de calcul du BCWS, consultez la section [Configurer le calcul du BCWS](#configure-how-bcws-is-calculated) de cet article.

* Workfront calcule le BCWS d’un projet en ajoutant toutes les valeurs du BCWS de toutes les tâches parents et des tâches individuelles du projet.

  Les valeurs des tâches enfants ne sont pas ajoutées au BCWS du projet.

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
   <p>Nouveau : Standard</p>
   <p>ou</p>
   <p>Actuel : formule</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td>Accès en modification aux projets</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td>Autorisations de gestion pour le projet</td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez l’article [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurer le mode de calcul du BCWS {#configure-how-bcws-is-calculated}

Vous pouvez configurer le mode de calcul du BCWS en heures ou en coûts en configurant la méthode d’indice de performances (PIM) du projet.

1. Accédez à un projet et cliquez sur **Détails du projet** dans le panneau de gauche.
1. Dans la zone **Finances**, recherchez la **Méthode d’indice de performances** et double-cliquez dessus pour la modifier.

   ![](assets/pim-options-hour-cost-based-nwe.png)

1. Sélectionnez l’une des options suivantes :

   | Option | Exécution du calcul |
   |---|---|
   | Basé sur les heures | Workfront calcule le BCWS à l’aide du nombre d’heures prévues des tâches. |
   | Basé sur les coûts | Workfront calcule le BCWS à l’aide du coût prévu des tâches. |


1. Cliquez sur **Enregistrer les modifications**.

   Le BCWS des tâches sur le projet est calculé en heures ou en coûts.

## Calculer le BCWS

Workfront calcule le coût budgété du travail prévu (BCWS) pour les tâches ou les projets à l’aide des formules suivantes :

```
Task BCWS = Planned Percent Complete x Task Budget
```

```
Project BCWS = SUM(BCWS values of all parent and individual tasks)
```

Les valeurs utilisées dans ce calcul sont les suivantes :

| Valeur utilisée | Description de la valeur utilisée |
|---|---|
| Pourcentage terminé prévu | Il s’agit du pourcentage terminé prévu de la tâche en fonction du temps écoulé entre le début de la tâche et aujourd’hui. |
| Budget de la tâche | Il s’agit de la valeur du nombre d’heures prévues ou du coût prévu de la tâche. |

Par exemple, si nous sommes aujourd’hui le 12 février et qu’une tâche est programmée du 10 au 20 février, le pourcentage terminé de la tâche doit être de 20 % à la date d’aujourd’hui. Si le budget de la tâche (coût prévu) est de 10 000 €, le BCWS de la tâche est de :

```
Task BCWS = 20% x $10,000 = $2,000
```

## Localiser le BCWS pour un projet ou une tâche

Vous pouvez afficher la valeur du Coût budgété du travail prévu dans un rapport ou une liste, en ajoutant la colonne BCWS à votre vue.

1. Accédez à une liste de tâches ou de projets.
1. Développez le menu **Vue** et sélectionnez **Nouvelle vue** ou **Personnaliser la vue**.

1. Cliquez sur **Ajouter une colonne**.
1. Dans le champ **Afficher dans cette colonne :**, commencez à saisir **BCWS** et cliquez dessus pour le sélectionner lorsqu’il s’affiche dans la liste.

   ![](assets/bcws-in-project-view.png)

1. Cliquez sur **Enregistrer la vue**.
1. Le champ **BCWS** s’affiche dans la vue.
