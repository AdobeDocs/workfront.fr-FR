---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Plusieurs onglets de navigateur entraînent la déconnexion de Workfront
description: Lorsqu’une personne a plusieurs onglets de navigateur ouverts, Workfront peut se déconnecter automatiquement.
feature: Get Started with Workfront
exl-id: 1cc8bf6c-0eda-41ef-8efd-bba3a5f33b08
source-git-commit: 99113ac4f2ceca6bd50f078916e33cec7f577362
workflow-type: tm+mt
source-wordcount: '164'
ht-degree: 32%

---

# Plusieurs onglets de navigateur entraînent la déconnexion de Workfront

## Problème

Lorsque l’utilisateur ouvre plusieurs onglets du navigateur et clique sur un onglet inactif depuis un certain temps, la session de l’onglet a expiré. L’utilisateur ne peut pas voir la page qu’il a ouverte, et voit le message suivant :

```
Tab session expired
This tab session has been halted due to inactivity. Refresh the tab to continue where you left off.
```

## Raison

Ce comportement est dû à l’authentification basée sur une politique (PBA), une mesure de sécurité configurée par votre organisation. Lorsqu’un onglet est inactif depuis plus longtemps que la limite de temps définie dans la configuration PBA de votre organisation, la session d’onglets expire.

## Solution

La solution dépend de si vous avez été actif dans un autre onglet connecté à Workfront.

* Si un onglet Workfront actif est ouvert, rechargez l’onglet expiré. Il revient à la page que vous avez ouverte avant qu’elle n’expire.

* Si aucun onglet Workfront actif n’est ouvert, connectez-vous à nouveau à Workfront.
