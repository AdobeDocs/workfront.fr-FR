---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Plusieurs onglets du navigateur entraînent la déconnexion de Workfront
description: Lorsqu’une personne a plusieurs onglets de navigateur ouverts, Workfront peut se déconnecter automatiquement.
feature: Get Started with Workfront
author: Becky
exl-id: 1cc8bf6c-0eda-41ef-8efd-bba3a5f33b08
TQID: https://experienceleague.adobe.com/Zof7zbTOm-w1vyBTchiXJv2QrNYbOxw9O4DYIjYQ6Ss
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 165
ht-degree: 42%

---

# Plusieurs onglets du navigateur entraînent la déconnexion de Workfront

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
