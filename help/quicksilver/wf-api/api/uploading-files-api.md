---
content-type: api
navigation-topic: api-navigation-topic
title: Charger des fichiers via l’API
description: Charger des fichiers via l’API
author: Becky
feature: Workfront API
role: Developer
exl-id: 4e0b73b6-0d6d-4971-a87a-dfec85fb031a
TQID: https://experienceleague.adobe.com/Yd7byYJ1pYDXwdKvINXh4fKy-pWoEiNMj345jr1HHNs
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 176
ht-degree: 93%

---

# Charger des fichiers via l’API

Vous pouvez charger des fichiers en utilisant les API Workfront avec des outils d’API, tels que Postman, ou avec de simples commandes cURL.

Pour charger des documents, voir les instructions pour **Charger des documents** dans [Comportement de la requête POST](/help/quicksilver/wf-api/general/api-basics.md#post-behavior) dans Workfront. Vous pouvez également utiliser ces mêmes instructions pour les requêtes cURL.

**Lorsque vous utilisez les outils d’API pour charger des fichiers, suivez les instructions suivantes :**

* Utilisez l’option de votre outil d’API pour charger votre fichier. L’écran de la requête contient souvent un bouton **Choisir un fichier**.

* Utilisez la méthode HTTP POST pour demander le chargement du fichier.

* Votre requête doit donner lieu à une réponse qui contient une valeur pour son pseudo.

* Utilisez la valeur du pseudo, le type d’objet et la valeur du GUID pour l’objID dans un payload JSON pour effectuer un appel ultérieur. Il s’agit de créer l’objet pour votre fichier, comme dans l’exemple suivant :

```
{
"name": "TestPDF",
"handle": "7af257e64aba4a22c33ccdfc40bbb87",
"docObjCode": "PROJ",
"objID": "0398450f8345980843445534354",
"currentVersion": {"version": "1", "fileName" : "TestPDF"},
}
```

Vous devriez recevoir un ID pour l’objet dans la réponse.

Pour plus d’informations, reportez-vous à l’aide de l’outil d’API spécifique que vous utilisez.
