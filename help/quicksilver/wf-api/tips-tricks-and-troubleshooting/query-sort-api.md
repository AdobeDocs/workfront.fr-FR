---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Trier les résultats d’une requête dans l’API
description: Trier les résultats d’une requête dans l’API
author: Becky
feature: Workfront API
role: Developer
exl-id: f001adb8-6295-4646-b9f1-78244a8c44a6
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '60'
ht-degree: 58%

---


# Trier les résultats d’une requête dans l’API

Vous pouvez trier vos résultats selon n’importe quel champ si vous ajoutez les éléments suivants à votre appel API :

```
&entryDate_Sort=asc
```

Par exemple, si vous souhaitez trier par date de début planifiée de la tâche, supprimez `entryDate` et remplacez-le par `plannedCompletionDate`.

Cela fonctionne pour la plupart des champs dans Adobe Workfront.
