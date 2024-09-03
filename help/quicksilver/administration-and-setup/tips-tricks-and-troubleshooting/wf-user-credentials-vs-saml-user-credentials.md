---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Informations d’identification d’utilisateur Adobe Workfront et informations d’identification d’utilisateur SAML
description: Après la création de l’utilisateur ou de l’utilisatrice, vous pouvez modifier l’utilisateur ou l’utilisatrice et activer l’option « Autoriser uniquement l’authentification SAML 2.0 » afin que son utilisateur ou utilisatrice et son mot de passe soient contrôlés par le système SAML. Lorsque cette option est activée, l’utilisateur n’est autorisé à se connecter que par SAML.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: faa55b09-10c3-48e6-8b39-33f9feb0a335
source-git-commit: c389b4829f16bf82a5851a597f5dd358d9c96999
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 90%

---

# Informations d’identification de l’utilisateur ou utilisatrice Adobe Workfront et informations d’identification de l’utilisateur ou utilisatrice SAML

Cet article porte spécifiquement sur [!DNL Adobe Workfront] et SAML et ne couvre pas d’autres méthodes d’authentification SSO.

Dans une base de données, [!DNL Workfront] stocke l’adresse e-mail des utilisateurs et utilisatrices comme leur nom d’utilisateur ou d’utilisatrice [!DNL Workfront], ainsi que leur mot de passe [!DNL Workfront]. Ces informations d’identification sont répliquées dans les sandbox de prévisualisation et d’actualisation personnalisée.

Lors de la création de l’utilisateur ou utilisatrice, si [!DNL Workfront] détecte que SAML 2.0 est configuré, il définit par défaut « Autoriser uniquement l’authentification SAML 2.0 » pour l’utilisateur ou l’utilisatrice. Si la case « Envoyer un e-mail d’invitation à cette personne » est cochée, [!DNL Workfront] désactive l’option « Autoriser uniquement l’authentification SAML 2.0 » et masque cette option. Une fois que l’option « Envoyer un e-mail d’invitation à cette personne » est activée, l’utilisateur ou l’utilisatrice devient un utilisateur ou une utilisatrice [!DNL Workfront] non SAML.

Après la création de l’utilisateur ou utilisatrice, vous pouvez le ou la modifier et activer **[!UICONTROL Autoriser uniquement l’authentification SAML 2.0]** afin que son utilisateur ou utilisatrice et son mot de passe soient contrôlés par le système SAML.

Une fois cela fait, l’utilisateur ou utilisatrice peut se connecter uniquement via SAML. Lorsque la personne accède à l’URL [!DNL Workfront], elle est automatiquement redirigée vers le système SAML et est invitée à saisir son nom d’utilisateur ou d’utilisatrice et son mot de passe SAML.

Les informations d’identification SAML sont stockées dans un système SAML externe, tel que l’ADFS de Microsoft, et non dans Workfront.
