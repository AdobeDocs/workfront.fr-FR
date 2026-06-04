---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: L’action moveToFolder du document ne fonctionne pas.
description: Lors de l’utilisation de l’action Document moveToFolder, une erreur 422 est renvoyée.
author: Becky
feature: Workfront API
role: Developer
exl-id: 811efabc-e101-4de5-a800-a1447654dc3e
TQID: https://experienceleague.adobe.com/UV4VnQEs-jGJau1UqXTLnp7Ak-cmKRpjuJqxgNTF5z8
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 121
ht-degree: 100%

---

# L’action moveToFolder du document ne fonctionne pas.

## Problème

Lors de l’utilisation de l’action `moveToFolder` de l’objet Document, une erreur 422 est renvoyée.

Ou

Si vous utilisez cette action via le module Adobe Authenticator dans Workfront Fusion, le document n’est pas déplacé, mais aucune indication de l’erreur n’est affichée. L’erreur est la même, mais le module Adobe Authenticator ne l’affiche pas.

## Solution

L’une des causes possibles d’une erreur 422 pour cette action est la tentative de déplacement d’un document dans un dossier lié vers un autre dossier lié.

Vérifiez que le document que vous souhaitez déplacer ne se trouve pas déjà dans un dossier lié.
