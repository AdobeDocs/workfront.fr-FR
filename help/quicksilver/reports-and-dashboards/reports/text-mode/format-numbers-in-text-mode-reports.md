---
product-area: reporting
navigation-topic: text-mode-reporting
title: Formatage des valeurs, des devises et des pourcentages dans les rapports en mode texte
description: Les valeurs numériques, y compris les devises, peuvent être configurées pour s’afficher dans divers formats dans des rapports et des listes dans Adobe Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: 965f5dcd-4844-4792-9fd0-a47814a325a4
source-git-commit: 8de9c79f6c62b74a652482ec10bf38fada8c5fc8
workflow-type: tm+mt
source-wordcount: '155'
ht-degree: 7%

---

# Formatage des valeurs, des devises et des pourcentages dans les rapports en mode texte

<!-- Audited: 2/2024 -->

Les valeurs numériques, y compris les devises, peuvent être configurées pour s’afficher dans divers formats dans des rapports et des listes dans Adobe Workfront.

Pour modifier le format d’une valeur numérique, vous devez modifier la variable **valueformat** de votre colonne.

Par exemple, si vous souhaitez afficher la colonne Budget à 1 000 $, la ligne de format de valeur se présente comme suit :

```
valueformat=currencyStringCurrencyRounded
valuefield=budget
```

Pour plus d’informations sur l’application d’une mise en forme conditionnelle dans les rapports Workfront et les listes en mode texte, voir [Utilisation de la mise en forme conditionnelle en mode Texte](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md).

Vous pouvez formater les nombres à l’aide des valeurs suivantes pour la variable `valueformat` ligne de votre colonne :

| Exemple | `valueformat=` |
|---|---|
| 1234 | <pre>doubleAsString</pre> <br>ou <br><pre>int</pre> |
| 1 234 | <pre>doubleAsInt</pre> |
| 1 234 $ | <pre>currencyStringCurrencyRounded</pre> |
| 1234,56 | <pre>doubleAsDouble</pre> |
| 1 234,56 $ | <pre>currencyStringCurrency</pre> |
| 12% | <pre>doubleAsPercentRounded</pre> |
| 12,34 % | <pre>doubleAsPercent</pre> |
| (1,234.56) | <pre>doubleAsFinancial</pre> |
| (1,234) | <pre>doubleAsFinancialRounded</pre> |

