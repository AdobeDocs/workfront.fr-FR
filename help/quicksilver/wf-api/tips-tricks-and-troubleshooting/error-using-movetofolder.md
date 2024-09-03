---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: L’action moveToFolder du document ne fonctionne pas.
description: Lors de l’utilisation de l’action Document moveToFolder, une erreur 422 est renvoyée.
author: Becky
feature: Workfront API
role: Developer
exl-id: 811efabc-e101-4de5-a800-a1447654dc3e
source-git-commit: 53edc378e000e5b36fe0ce5750b8917fb13cfde1
workflow-type: tm+mt
source-wordcount: '121'
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
