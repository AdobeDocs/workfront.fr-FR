---
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: Le nom du document a changé après le chargement et contient un caractère non valide
description: Certains documents ne peuvent pas être convertis en épreuves.
author: Courtney
exl-id: 7771deb5-cf9f-4a32-a444-b701bec1619e
source-git-commit: 1e67375c12bc473130127887e6cd4fa474c4fb02
workflow-type: tm+mt
source-wordcount: '135'
ht-degree: 45%

---

# Le nom du document a changé après le chargement et contient un caractère non valide

## Problème

Certains documents ne peuvent pas être convertis en épreuves.

## Cause

Certains caractères ne peuvent pas figurer dans le nom des fichiers téléchargés vers Workfront. Si le nom d’un fichier contient l’un des caractères suivants, ces caractères sont supprimés du nom du fichier lorsque celui-ci est téléchargé : `! # % * \ | ' " / ? < > { } [ ]`.

Si un nom de document est mis à jour pour inclure un caractère non valide après le chargement initial, la génération de l’épreuve échoue.

## Solution

Supprimez le caractère non valide du nom du document :

1. Sélectionnez le document, puis cliquez sur **Détails du document**.
1. Cliquez sur le nom du document et supprimez le caractère non valide, puis appuyez sur Entrée.

   Caractères non valides : `! # % * \ | ' " / ? < > { } [ ]`

   ![&#x200B; Nom du document &#x200B;](assets/doc-name.png)

1. Actualisez la page et générez l’épreuve.
