---
product-area: reporting
navigation-topic: text-mode-reporting
title: Mettre en forme des dates dans les rapports en mode texte
description: Les dates peuvent être configurées pour s’afficher dans divers formats dans les rapports et les listes d’Adobe Workfront. Pour établir un format de date, vous devez modifier la ligne de valeur du code du mode Texte dans la colonne.
author: Nolan
feature: Reports and Dashboards
exl-id: ff0686aa-b306-4954-8f9b-3e98bf8cff22
source-git-commit: 9caac488522d2a12d3bdf4bf23ba7e44c6dbf7d2
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 94%

---

# Mettre en forme des dates dans les rapports en mode texte

<!-- Audited: 1/2025 -->

Les dates peuvent être configurées pour s’afficher dans divers formats dans les rapports et les listes d’Adobe Workfront. Pour définir un format de date, vous devez modifier la ligne `valueformat` du code du mode Texte dans la colonne.

`valueformat= [new date format]` Par exemple, si vous souhaitez que la date de fin projetée s’affiche sous la forme JJ/MM/AA, le code se présente comme suit :

```
valueformat=atDate
valuefield=projectedCompletionDate
```

Si vous souhaitez afficher la date d’achèvement prévue sous la forme *JJ, Mois, Année*, le code ressemblerait à ceci :

```
valueformat=mediumAtdate
valuefield=plannedCompletionDate
```

Pour plus d’informations sur l’application d’une mise en forme conditionnelle dans les rapports Workfront et les listes en mode Texte, voir [Utiliser la mise en forme conditionnelle en mode Texte](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md).

Vous pouvez formater des dates à l’aide des valeurs de mode de texte `valueformat` suivantes :

| **Format** | Exemple | ***valueformat=*** |
|---|---|---|
| JJ/MM/AA | 11/10/18 | `atDate` |
| JJ/MM/AA Heure | 11/10/18 12 h | `longAtDate` |
| JJ/MM/AA | 11/10/18 | `shortAtDate` |
| JJ, Mois, An | 11 octobre 2018 | `mediumAtDate` |
| JS, Jour, Mois, An | Lun, 11 octobre 2018 | `partialAtDate` |
| JS, Jour, Mois, An Heure | Lun, 11 octobre 2018 12 h | `fullAtDate` |
