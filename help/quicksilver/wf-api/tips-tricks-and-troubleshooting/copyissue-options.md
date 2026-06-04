---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Configuration des options pour OPTASK copyIssue
description: Explication des valeurs entières attendues par le point d’entrée copyIssue.
author: Becky
feature: Workfront API
role: Developer
exl-id: a2b8ef01-1c14-47a5-8b0a-550b17b526ff
TQID: https://experienceleague.adobe.com/9cDJFoKl6zqpaAvqzpGqzflcbGZNrAWvEnUAFuqD-Rc
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 122
ht-degree: 100%

---

# Configuration des options pour OPTASK copyIssue


L’une des propriétés d’un appel API copyIssue est un champ appelé `options`. Ce champ exige un entier.

Pour inclure l’une des options suivantes, saisissez l’entier correspondant. Pour inclure plusieurs options, saisissez la somme des entiers correspondants.

| Option | Valeur* |
|---|---|
| Effacer les affectations | 2 |
| Effacer la progression | 4 |
| Effacer les documents | 128 |
| Effacer les mises à jour | 65536 |
| Autorisations de suppression | 524288 |
| Effacer les données personnalisées | 1048576 |

* Toutes les valeurs sont des puissances de 2.

Exemples :

* Pour effacer la progression lorsque vous copiez le problème, saisissez une valeur `options` de `4`.

* Pour effacer la progression et les documents, saisissez une valeur `options` de `132`.

  Effacer la progression = 4

  Effacer les documents = 128

  4 + 128 = 132
