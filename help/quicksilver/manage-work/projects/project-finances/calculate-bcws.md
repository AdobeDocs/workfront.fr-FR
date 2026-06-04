---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calculer le coût budgété du travail prévu (BCWS)
description: Également appelé Valeur prévue, le coût budgété du travail prévu (BCWS) est une mesure de performances du projet qui représente le montant de la tâche qui devrait avoir été achevée au moment où cette mesure est calculée.
author: Lisa
feature: Work Management
exl-id: b9a36333-9430-42bd-99dd-3ad82803b633
TQID: https://experienceleague.adobe.com/Nt0HZv7YfcMsAXZr3xRlkGXtCrQPJeJd4IQB0BuhbVM
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 600
ht-degree: 99%

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

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Package Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td>Licence Adobe Workfront</td> 
   <td>
   <p>Standard</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td>Accès en modification aux projets</td> 
  </tr> 
  <tr> 
   <td>Autorisations d’objet</td> 
   <td>Autorisations de gestion pour le projet</td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurer le mode de calcul du BCWS {#configure-how-bcws-is-calculated}

Vous pouvez configurer le mode de calcul du BCWS en heures ou en coûts en configurant la méthode d’indice de performances (PIM) du projet.

1. Accédez à un projet et cliquez sur **Détails du projet** dans le panneau de gauche.
1. Dans la zone **Finances**, recherchez la **Méthode d’indice de performances** et double-cliquez dessus pour la modifier.

   ![options PIM](assets/pim-options-hour-cost-based-nwe.png)

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

   ![CBTP dans la vue Projet](assets/bcws-in-project-view.png)

1. Cliquez sur **Enregistrer la vue**.
1. Le champ **BCWS** s’affiche dans la vue.
