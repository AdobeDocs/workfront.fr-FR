---
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: Le nom du document a changé après le chargement et contient un caractère non valide
description: Certains documents ne peuvent pas être convertis en épreuves.
author: Courtney
exl-id: 7771deb5-cf9f-4a32-a444-b701bec1619e
TQID: https://experienceleague.adobe.com/bE5iUIG7rFpIIa3zXt-5pO0sgfbEO-3QDVFVLwkayIo
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 135
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

   ![ Nom du document ](assets/doc-name.png)

1. Actualisez la page et générez l’épreuve.
