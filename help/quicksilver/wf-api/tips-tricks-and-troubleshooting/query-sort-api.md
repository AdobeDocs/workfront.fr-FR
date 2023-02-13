---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Tri des résultats des requêtes dans l’API
description: Tri des résultats des requêtes dans l’API
author: John
feature: Workfront API
exl-id: f001adb8-6295-4646-b9f1-78244a8c44a6
source-git-commit: a939e14cbd6936bdd0c46c1ed641acdda497b8fc
workflow-type: tm+mt
source-wordcount: '60'
ht-degree: 0%

---


# Tri des résultats des requêtes dans l’API

Vous pouvez trier vos résultats selon n’importe quel champ si vous ajoutez les éléments suivants à votre appel API :

```
&entryDate_Sort=asc
```

Par exemple, si vous souhaitez trier par date de début planifiée de la tâche, supprimez `entryDate` et remplacez-le par `plannedCompletionDate`.

Cela fonctionne pour la plupart des champs dans Adobe Workfront.
