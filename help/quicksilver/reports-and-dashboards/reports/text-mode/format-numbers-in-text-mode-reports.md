---
product-area: reporting
navigation-topic: text-mode-reporting
title: Mettre en forme des nombres, des devises et des pourcentages dans les rapports en mode texte
description: Les valeurs numériques, y compris les devises, peuvent être configurées pour s’afficher dans divers formats dans des rapports et des listes dans Adobe Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: 965f5dcd-4844-4792-9fd0-a47814a325a4
source-git-commit: 9caac488522d2a12d3bdf4bf23ba7e44c6dbf7d2
workflow-type: tm+mt
source-wordcount: '145'
ht-degree: 99%

---

# Mettre en forme des nombres, des devises et des pourcentages dans les rapports en mode texte

<!-- Audited: 1/2025 -->

Les valeurs numériques, y compris les devises, peuvent être configurées pour s’afficher dans divers formats dans des rapports et des listes dans Adobe Workfront.

Pour modifier le format d’une valeur numérique, vous devez modifier la ligne **valueformat** de votre colonne.

Par exemple, si vous souhaitez afficher la colonne Budget comme 1 000 $, la ligne de format de valeur se présente comme suit :

```
valueformat=currencyStringCurrencyRounded
valuefield=budget
```

Pour plus d’informations sur l’application d’une mise en forme conditionnelle dans les rapports Workfront et les listes en mode texte, voir [Utiliser la mise en forme conditionnelle en mode texte](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md).

Vous pouvez formater les nombres à l’aide des valeurs suivantes pour la ligne `valueformat` de votre colonne :

| Exemple | `valueformat=` |
|---|---|
| 1234 | `doubleAsString`<br> ou <br>`int` |
| 1 234 | `doubleAsInt` |
| 1 234 $ | `currencyStringCurrencyRounded` |
| 1234,56 | `doubleAsDouble` |
| 1 234,56 $ | `currencyStringCurrency` |
| 12% | `doubleAsPercentRounded` |
| 12,34 % | `doubleAsPercent` |
| (1,234.56) | `doubleAsFinancial` |
| (1,234) | `doubleAsFinancialRounded` |

