---
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: Le nom du document a été modifié après le téléchargement et contient un caractère non valide.
description: Certains documents ne peuvent pas être convertis en BAT.
author: Courtney
source-git-commit: a01c2e42dad1a7c00ac73fcaeb1202c56238a8bb
workflow-type: tm+mt
source-wordcount: '133'
ht-degree: 0%

---


# Le nom du document a été modifié après le téléchargement et contient un caractère non valide.

## Problème

Certains documents ne peuvent pas être convertis en BAT.

## Cause

Les fichiers chargés dans Workfront ne peuvent pas contenir certains caractères dans les noms de fichiers. Si un fichier contient l’un des caractères suivants, les caractères sont supprimés du nom du fichier lors du téléchargement du fichier : `! # % * \ | ' " / ? < > { } [ ]`.

Si un nom de document est mis à jour pour inclure un caractère non valide après le téléchargement initial, la génération du BAT échoue.

## Solution

Supprimez le caractère non valide du nom du document :

1. Sélectionnez le document, puis cliquez sur **Détails du document**.
1. Cliquez sur le nom du document, supprimez le caractère non valide, puis appuyez sur Entrée.

   Caractères non valides : `! # % * \ | ' " / ? < > { } [ ]`

   ![](assets/doc-name.png)

1. Actualisez la page et générez le BAT.