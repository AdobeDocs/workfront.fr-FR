---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Plusieurs onglets de navigateur entraînent la déconnexion de Workfront.
description: Lorsqu’une personne a plusieurs onglets de navigateur ouverts, Workfront peut se déconnecter automatiquement.
feature: Get Started with Workfront
source-git-commit: ef85b267b3417dddd0c9cc4a2b916b83dc416e14
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 8%

---

# Plusieurs onglets de navigateur entraînent la déconnexion de Workfront.

>[!IMPORTANT]
>
>Ce problème est présent uniquement pour les organisations qui ont été intégrées à Adobe IMS.

## Problème

Lorsqu’un utilisateur dispose de plusieurs onglets de navigateur ouverts et qu’il clique dans un onglet inactif depuis un certain temps, la session de l’onglet a expiré. L’utilisateur ne peut pas voir la page qu’il a ouverte, mais voit à la place le message suivant :

```
Tab session expired
This tab session has been halted due to inactivity. Refresh the tab to continue where you left off.
```

## Raison

Ce comportement est dû à l’authentification basée sur des stratégies (PBA), une mesure de sécurité configurée par votre organisation. Lorsqu’un onglet est inactif depuis plus que la limite de temps définie dans la configuration PBA de votre organisation, la session d’onglets expire.

## Solution

La solution dépend de si vous avez été actif dans un autre onglet connecté à Workfront.

* Si un onglet Workfront actif est ouvert, rechargez l’onglet expiré. Il revient à la page que vous avez ouverte avant qu’elle n’expire.

* Si aucun onglet Workfront actif n’est ouvert, connectez-vous à nouveau à Workfront.