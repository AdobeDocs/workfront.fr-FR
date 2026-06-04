---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Informations d’identification de l’utilisateur Adobe Workfront et informations d’identification de l’utilisateur SAML
description: Après la création de l’utilisateur ou de l’utilisatrice, vous pouvez modifier l’utilisateur ou l’utilisatrice et activer l’option « Autoriser uniquement l’authentification SAML 2.0 » afin que son utilisateur ou utilisatrice et son mot de passe soient contrôlés par le système SAML. Lorsque cette option est activée, l’utilisateur est uniquement autorisé à se connecter via SAML.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: faa55b09-10c3-48e6-8b39-33f9feb0a335
TQID: https://experienceleague.adobe.com/8paS2GIumamOltxTC8Gw2mBZ4bKB6TOgbly7IBPKhDw
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 235
ht-degree: 90%

---

# Informations d’identification de l’utilisateur ou utilisatrice Adobe Workfront et informations d’identification de l’utilisateur ou utilisatrice SAML

Cet article porte spécifiquement sur [!DNL Adobe Workfront] et SAML et ne couvre pas d’autres méthodes d’authentification SSO.

Dans une base de données, [!DNL Workfront] stocke l’adresse e-mail des utilisateurs et utilisatrices comme leur nom d’utilisateur ou d’utilisatrice [!DNL Workfront], ainsi que leur mot de passe [!DNL Workfront]. Ces informations d’identification sont répliquées dans les sandbox de prévisualisation et d’actualisation personnalisée.

Lors de la création de l’utilisateur ou utilisatrice, si [!DNL Workfront] détecte que SAML 2.0 est configuré, il définit par défaut « Autoriser uniquement l’authentification SAML 2.0 » pour l’utilisateur ou l’utilisatrice. Si la case « Envoyer un e-mail d’invitation à cette personne » est cochée, [!DNL Workfront] désactive l’option « Autoriser uniquement l’authentification SAML 2.0 » et masque cette option. Une fois que l’option « Envoyer un e-mail d’invitation à cette personne » est activée, l’utilisateur ou l’utilisatrice devient un utilisateur ou une utilisatrice [!DNL Workfront] non SAML.

Après la création de l’utilisateur ou utilisatrice, vous pouvez le ou la modifier et activer **[!UICONTROL Autoriser uniquement l’authentification SAML 2.0]** afin que son utilisateur ou utilisatrice et son mot de passe soient contrôlés par le système SAML.

Une fois cela fait, l’utilisateur ou utilisatrice peut se connecter uniquement via SAML. Lorsque la personne accède à l’URL [!DNL Workfront], elle est automatiquement redirigée vers le système SAML et est invitée à saisir son nom d’utilisateur ou d’utilisatrice et son mot de passe SAML.

Les informations d’identification SAML sont stockées dans un système SAML externe, tel que l’ADFS de Microsoft, et non dans Workfront.
