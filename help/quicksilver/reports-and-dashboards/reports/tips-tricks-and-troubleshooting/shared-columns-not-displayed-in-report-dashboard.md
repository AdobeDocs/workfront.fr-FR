---
content-type: faq
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: Données de colonnes partagées non affichées dans les rapports du tableau de bord
description: Les données des colonnes partagées ne s’affichent pas lorsque le rapport est placé dans un tableau de bord à plusieurs colonnes, mais elles s’affichent dans une seule colonne. Les sauts de ligne sont également remplacés.
author: Nolan
feature: Reports and Dashboards
exl-id: b8307182-3ec1-4f16-8427-48ef7a65f969
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '162'
ht-degree: 0%

---

# Données de colonnes partagées non affichées dans les rapports du tableau de bord

## Problème

Les données des colonnes partagées ne s’affichent pas lorsque le rapport est placé dans un tableau de bord à plusieurs colonnes, mais elles s’affichent dans une seule colonne. Les sauts de ligne sont également remplacés.

## Cause

Seules les colonnes marquées comme

```
shortview=true
```

sont inclus dans la vue tableau de bord du rapport lorsque la disposition du tableau de bord comporte le partage gauche/droite ou le partage gauche/milieu/droite.

## Solution

Accédez à la vue utilisée dans le rapport et ouvrez le mode texte. (Pour plus d’informations, voir [Modification d’une vue en mode texte](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md).) Étiqueter toutes les colonnes du rapport, y compris les colonnes utilisées dans une colonne partagée/fusionnée, avec

```
shortview=true
```

. Les colonnes du rapport s&#39;afficheront alors correctement dans le tableau de bord.
