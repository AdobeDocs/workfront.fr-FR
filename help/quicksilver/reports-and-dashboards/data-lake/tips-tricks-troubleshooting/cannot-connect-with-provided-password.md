---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: L’outil Power BI ne peut pas se connecter avec le mot de passe fourni
description: Lorsque vous tentez de vous connecter à Data Connect à partir de votre outil Power BI, vous recevez un message d’erreur de connexion.
author: Courtney
feature: Reports and Dashboards
exl-id: c3f2b4a9-0831-48f0-871b-486d09ae5ea4
TQID: https://experienceleague.adobe.com/Z4RrMAPGd3CCti-cQFiJ7hlf-h8-suXeuoYfzk-9aKo
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 229
ht-degree: 6%

---

# L’outil Power BI ne peut pas se connecter avec le mot de passe fourni

## Problème

Lorsque vous tentez de vous connecter à Data Connect à partir de votre outil Power BI, le message d’erreur suivant s’affiche :

`Cannot connect from BI tool with provided password`

## Cause

Lors de la création de la connexion JDBC, Workfront fournit un mot de passe temporaire pour Data Connect.

Avant d’accéder à Data Connect via Power BI, vous devez d’abord vous connecter à l’aide des détails de connexion fournis, mettre à jour le mot de passe temporaire, puis procéder à votre connexion.


## Solution

Réinitialisez le mot de passe de connexion dans Workfront, puis créez un nouveau mot de passe avec le lien fourni dans la boîte de dialogue Modifier la connexion .

### Réinitialiser le mot de passe de connexion dans Workfront

1. Accédez à Workfront > Configuration > Système > Data Connect.
1. Recherchez et ouvrez la connexion à partir de la liste.
1. Sous **Réinitialiser le mot de passe de connexion**, cochez la case pour confirmer que vous souhaitez réinitialiser le mot de passe.
1. Cliquez sur **Réinitialiser le mot de passe de connexion**.
   ![réinitialiser le mot de passe de connexion](assets/reset-password.png)
1. Passez à la section ci-dessous.

### Créer un nouveau mot de passe pour la connexion

1. Copiez l’URL et collez-la dans un nouvel onglet du navigateur.
1. Dans Workfront, copiez et collez le Nom d’utilisateur de la connexion et le Mot de passe par défaut dans le nouvel onglet du navigateur.
   ![copier l’url et le mot de passe par défaut](assets/link-password.png)
1. Cliquez sur **Se connecter**.
1. Saisissez un nouveau mot de passe, puis cliquez sur **Envoyer**.
1. Accédez à l’outil Power BI et connectez-vous avec le nouveau mot de passe.
