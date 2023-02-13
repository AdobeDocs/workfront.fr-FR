---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Configuration des options pour OPTASK copyIssue
description: Une explication des valeurs entières attendues par le point de terminaison copyIssue .
author: Becky
feature: Workfront API
exl-id: a2b8ef01-1c14-47a5-8b0a-550b17b526ff
source-git-commit: 93a67b3dbd59f188dad6b060ec93c3f137c981b2
workflow-type: tm+mt
source-wordcount: '117'
ht-degree: 6%

---

# Configuration des options pour OPTASK copyIssue


L’une des propriétés d’un appel API copyIssue est un champ appelé `options`. Ce champ exige un entier.

Pour inclure l’une des options suivantes, saisissez l’entier correspondant. Pour inclure plusieurs options, saisissez la somme des entiers correspondants.

| option | value* |
|---|---|
| Effacer les affectations | 2 |
| Effacer la progression | 4 |
| Effacer les documents | 128 |
| Effacer les mises à jour | 65536 |
| Effacer les autorisations | 524288 |
| Effacer les données personnalisées | 1048576 |

*Toutes les valeurs sont des puissances de 2.

Exemples:

* Pour effacer la progression lorsque vous copiez le problème, saisissez une `options` valeur de `4`.

* Pour effacer la progression et les documents, saisissez une `options` valeur de `132`.

   Effacer la progression = 4

   Effacer des documents = 128

   4 + 128 = 132
