---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Trier les résultats d’une requête dans l’API
description: Trier les résultats d’une requête dans l’API
author: Becky
feature: Workfront API
role: Developer
exl-id: f001adb8-6295-4646-b9f1-78244a8c44a6
TQID: https://experienceleague.adobe.com/r7PCHEpU413ajyML7-uzWdmXN11gylNHRU2q60J35Go
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 60
ht-degree: 71%

---

# Trier les résultats d’une requête dans l’API

Vous pouvez trier vos résultats selon n’importe quel champ si vous ajoutez les éléments suivants à votre appel API :

```
&entryDate_Sort=asc
```

Par exemple, si vous souhaitez trier par date d’achèvement prévue de la tâche, supprimez `entryDate` et remplacez-la par `plannedCompletionDate`.

```
&plannedCompletionDate_Sort=asc
```

Cela fonctionne pour la plupart des champs dans Adobe Workfront.
