---
content-type: faq
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: Données de colonnes partagées non affichées dans les rapports du tableau de bord
description: Les données des colonnes partagées ne s’affichent pas lorsque le rapport est placé dans un tableau de bord à plusieurs colonnes, mais elles s’affichent dans une disposition à colonne unique. Les sauts de ligne sont également remplacés.
author: Courtney
feature: Reports and Dashboards
exl-id: b8307182-3ec1-4f16-8427-48ef7a65f969
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/OEFlwkdPf98g4-rC1tzaTmmEwb5-BXHx-j8XGrRR8sE
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 162
ht-degree: 83%

---

# Données de colonnes partagées non affichées dans les rapports du tableau de bord

## Problème

Les données des colonnes partagées ne s’affichent pas lorsque le rapport est placé dans un tableau de bord à plusieurs colonnes, mais elles s’affichent dans une disposition à colonne unique. Les sauts de ligne sont également remplacés.

## Cause

Seules les colonnes marquées comme

```
shortview=true
```

sont incluses dans la vue tableau de bord du rapport lorsque la disposition du tableau de bord comporte un partage gauche/droite ou un partage gauche/milieu/droite.

## Solution

Accédez à la vue utilisée dans le rapport et ouvrez le mode texte. (Pour plus d’informations, voir [Modifier une vue en mode texte](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md).) Étiqueter toutes les colonnes du rapport, y compris les colonnes utilisées dans une colonne partagée/fusionnée, avec

```
shortview=true
```

. Les colonnes du rapport s’afficheront alors correctement dans le tableau de bord.
