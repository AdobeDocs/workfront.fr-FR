---
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: Le nom du document a changé après le chargement et contient un caractère non valide
description: Certains documents ne peuvent pas être convertis en BAT.
author: Courtney
exl-id: 7771deb5-cf9f-4a32-a444-b701bec1619e
source-git-commit: 3e16f69f5b3c2b37093b00841945e6529394fa94
workflow-type: tm+mt
source-wordcount: '133'
ht-degree: 46%

---

# Le nom du document a changé après le chargement et contient un caractère non valide

## Problème

Certains documents ne peuvent pas être convertis en BAT.

## Cause

Certains caractères ne peuvent pas figurer dans le nom des fichiers téléchargés vers Workfront. Si le nom d’un fichier contient l’un des caractères suivants, ces caractères sont supprimés du nom du fichier lorsque celui-ci est téléchargé : `! # % * \ | ' " / ? < > { } [ ]`.

Si un nom de document est mis à jour pour inclure un caractère non valide après le téléchargement initial, la génération du BAT échoue.

## Solution

Supprimez le caractère non valide du nom du document :

1. Sélectionnez le document, puis cliquez sur **Document Details**.
1. Cliquez sur le nom du document, supprimez le caractère non valide, puis appuyez sur Entrée.

   Caractères non valides : `! # % * \ | ' " / ? < > { } [ ]`

   ![](assets/doc-name.png)

1. Actualisez la page et générez le BAT.
