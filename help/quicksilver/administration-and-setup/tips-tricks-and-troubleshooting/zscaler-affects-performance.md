---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Les paramètres ZScaler peuvent entraîner une baisse des performances
description: Après la création de l’utilisateur ou de l’utilisatrice, vous pouvez modifier l’utilisateur ou l’utilisatrice et activer l’option « Autoriser uniquement l’authentification SAML 2.0 » afin que son utilisateur ou utilisatrice et son mot de passe soient contrôlés par le système SAML. Lorsque cette option est activée, l’utilisateur est uniquement autorisé à se connecter via SAML.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 2752a9e2-44fe-49b5-a7ab-4021d91ed37b
TQID: https://experienceleague.adobe.com/-3-p8fzXIiV-gnjIjhRzBmLfspAEEVAuD2lpmcsVjLA
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 107
ht-degree: 70%

---

# Workfront : les paramètres ZScaler peuvent diminuer les performances.

>[!NOTE]
>
>Il s’agit d’un problème lié à ZScaler, qui ne sera pas résolu par Workfront.

Le service web de ZScaler utilise `http/1.1` par défaut, ce qui peut entraîner une diminution des performances dans Workfront.

Pour vérifier et résoudre ce problème, configurez votre logiciel ZScaler pour utiliser `http/2`. Cette configuration ne peut pas être effectuée dans Workfront.

Vous trouverez des informations sur `http/2` dans la documentation ZScaler.
