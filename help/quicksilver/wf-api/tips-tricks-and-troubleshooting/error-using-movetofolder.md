---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: L’action déplacement de document vers le dossier ne fonctionne pas.
description: Lors de l’utilisation de l’action Document moveToFolder, une erreur 422 est renvoyée.
author: Becky
feature: Workfront API
role: Developer
source-git-commit: 86c0517443537ec5af640036c290b3a495825fdc
workflow-type: tm+mt
source-wordcount: '121'
ht-degree: 0%

---


# L’action déplacement de document vers le dossier ne fonctionne pas.

## Problème

Lors de l’utilisation de la propriété `moveToFolder` , une erreur 422 est renvoyée.

Ou

Si vous utilisez cette action via le module Adobe Authenticator dans Workfront Fusion, le document n’est pas déplacé, mais aucune indication de l’erreur n’est affichée. L&#39;erreur est la même, mais le module Adobe Authenticator ne l&#39;affiche pas.

## Solution

L’une des causes possibles d’une erreur 422 pour cette action est la tentative de déplacement d’un document dans un dossier lié vers un autre dossier lié.

Vérifiez que le document que vous souhaitez déplacer ne se trouve pas déjà dans un dossier lié.
