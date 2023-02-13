---
product-area: reporting
navigation-topic: text-mode-reporting
title: Mise en forme des dates dans les rapports en mode texte
description: Les dates peuvent être configurées pour s’afficher dans divers formats dans des rapports et des listes dans Adobe Workfront. Pour établir un format de date, vous devez modifier la ligne de valeur du code du mode texte dans la colonne.
author: Nolan
feature: Reports and Dashboards
exl-id: ff0686aa-b306-4954-8f9b-3e98bf8cff22
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '190'
ht-degree: 2%

---

# Mise en forme des dates dans les rapports en mode texte

Les dates peuvent être configurées pour s’afficher dans divers formats dans des rapports et des listes dans Adobe Workfront. Pour définir un format de date, vous devez modifier la variable `valueformat` ligne du code du mode texte dans la colonne .

`valueformat= [new date format]` Par exemple, si vous souhaitez que la date de fin prévue s’affiche sous la forme MM/JJ/AA, le code se présente comme suit :

```
valueformat=atDate
valuefield=projectedCompletionDate
```

Si vous souhaitez afficher la date de fin planifiée comme *Mth, DD, Year*, le code ressemblerait à ceci :

```
valueformat=mediumAtdate
valuefield=plannedCompletionDate
```

Pour plus d’informations sur l’application d’une mise en forme conditionnelle dans les rapports Workfront et les listes en mode texte, voir [Utilisation de la mise en forme conditionnelle en mode Texte](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md).

Vous pouvez formater des dates en utilisant les éléments suivants :

```
valueformat
```

 valeurs du mode texte :

| **Format** | Exemple  | ***valueformat=*** |
|---|---|---|
| MM/JJ/AA | 10/11/18 | `atDate` |
| MM/JJ/AA | 10/11/18 12h00 | `longAtDate` |
| MM/JJ/AA | 10/11/18 | `shortAtDate` |
| Mth, DD, YR | 11 octobre 2018 | `mediumAtDate` |
| DW, Mth, Day, YR | Lun, 11 octobre 2018 | `partialAtDate` |
| DW, Mth, Day, YR Time | Lun, 11 octobre 2018 12 h | `fullAtDate` |
