---
content-type: faq
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: Données de colonnes partagées non affichées dans les rapports du tableau de bord
description: Les données des colonnes partagées ne s’affichent pas lorsque le rapport est placé dans un tableau de bord à plusieurs colonnes, mais elles s’affichent dans une disposition à colonne unique. Les sauts de ligne sont également remplacés.
author: Courtney
feature: Reports and Dashboards
exl-id: b8307182-3ec1-4f16-8427-48ef7a65f969
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '162'
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
