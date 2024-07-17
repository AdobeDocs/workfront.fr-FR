---
content-type: api
navigation-topic: api-navigation-topic
title: Charger des fichiers via l’API
description: Charger des fichiers via l’API
author: Becky
feature: Workfront API
role: Developer
exl-id: 4e0b73b6-0d6d-4971-a87a-dfec85fb031a
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 8%

---

# Charger des fichiers via l’API

Vous pouvez charger des fichiers à l’aide des API Workfront à l’aide d’outils d’API, tels que Postman, ou à l’aide de commandes cURL simples.

Pour télécharger des documents, reportez-vous aux instructions de la section **Téléchargement de documents** dans Workfront [Comportement Post](/help/quicksilver/wf-api/general/api-basics.md#post-behavior). Vous pouvez également utiliser ces mêmes instructions pour les demandes cURL.

**Lorsque vous utilisez des outils d’API pour charger des fichiers, suivez ces instructions :**

* Utilisez l’option de votre outil d’API pour télécharger votre fichier. Il s’agit souvent d’un bouton **Choisir le fichier** sur l’écran de demande.

* Utilisez la méthode HTTP du POST pour effectuer la requête de téléchargement du fichier.

* Votre requête doit générer une réponse qui inclut une valeur pour son gestionnaire.

* Utilisez la valeur handle, le type d’objet et la valeur GUID pour objID dans un payload JSON pour effectuer un appel ultérieur. Il s’agit de la création de l’objet pour votre fichier, comme dans l’exemple suivant :

```
}
"name": "TestPDF",
"handle": "7af257e64aba4a22c33ccdfc40bbb87",
"docObjCode": "PROJ",
"objID": "0398450f8345980843445534354",
"currentVersion": {"version": "v1.0", "fileName" : "TestPDF"},
}
```

Vous devriez recevoir un identifiant pour l’objet dans la réponse.

Pour plus d’informations, reportez-vous à l’aide de l’outil d’API spécifique que vous utilisez.
