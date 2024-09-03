---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: Empêcher l’action Recalculer les finances d’affecter les heures historiques lorsque les taux changent
description: Vous devez mettre à jour le coût horaire d’une personne ou d’une fonction (en raison d’une augmentation ou d’une autre circonstance), mais vous ne souhaitez pas que cette modification affecte les heures qui ont été précédemment consignées sur des projets ou que cela affecte uniquement une partie des heures historiques.
author: Alina
feature: Timesheets
exl-id: 29d3124b-cf7a-4a47-95c4-cd5379489810
source-git-commit: 7786d899841cb82cc4d3832fb083c6e2bda2e197
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 100%

---

# Empêcher l’action Recalculer les finances d’affecter les heures historiques lorsque les taux changent

## Problème

Vous devez mettre à jour le coût horaire d’une personne ou d’une fonction (en raison d’une augmentation ou d’une autre circonstance), mais vous ne souhaitez pas que cette modification affecte les heures qui ont été précédemment consignées sur des projets ou que cela affecte uniquement une partie des heures historiques.

## Solution

Ajoutez les heures que vous ne souhaitez pas modifier dans un enregistrement de facturation sur le projet et définissez le statut de l’enregistrement de facturation sur Facturé.Cela se verrouille sur l’ancien taux et sera ignoré par l’action Recalculer les finances.Toutes les heures qui ne font pas partie d’un enregistrement de facturation Facturé sont calculées au nouveau taux. Pour plus d’informations, voir [Recalculer les finances d’un projet](../../manage-work/projects/project-finances/recalculate-project-finances.md).
