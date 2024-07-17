---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Informations d’identification de l’utilisateur Adobe Workfront par rapport aux informations d’identification de l’utilisateur  [!DNL SAML]
description: Après la création de l’utilisateur, vous pouvez modifier l’utilisateur et activer l’option "Autoriser uniquement l’authentification SAML 2.0" afin que son utilisateur et son mot de passe soient contrôlés par le système SAML. Lorsque cette option est activée, l’utilisateur n’est autorisé à se connecter que par SAML. Lorsqu’ils accèdent à l’URL  [!DNL Workfront] , ils sont automatiquement redirigés vers le système SAML et invités à saisir leur nom d’utilisateur et leur mot de passe SAML.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: faa55b09-10c3-48e6-8b39-33f9feb0a335
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 0%

---

# Informations d’identification de l’utilisateur Adobe Workfront et informations d’identification de l’utilisateur SAML

Cet article se concentre spécifiquement sur [!DNL Adobe Workfront] et SAML et ne couvre pas d’autres méthodes d’authentification SSO.

Dans une base de données, [!DNL Workfront] stocke l’adresse électronique de chaque utilisateur comme nom d’utilisateur [!DNL Workfront], ainsi que son mot de passe [!DNL Workfront]. Ces informations d’identification sont répliquées dans les sandbox Aperçu et Actualisation personnalisée.

Lors de la création de l’utilisateur, si [!DNL Workfront] détecte que SAML 2.0 est configuré, l’utilisateur dispose par défaut de l’option &quot;Autoriser uniquement l’authentification SAML 2.0&quot;. Si la case &quot;Envoyer un email d’invitation à cette personne&quot; est activée, [!DNL Workfront] désactive &quot;Uniquement autoriser l’authentification SAML 2.0&quot; et masque cette option. Une fois que l’option &quot;Envoyer un courrier électronique d’invitation à cette personne&quot; est activée, l’utilisateur devient un utilisateur [!DNL Workfront] non SAML.

Après la création de l’utilisateur, vous pouvez modifier l’utilisateur et activer l’authentification **[!UICONTROL Uniquement Autoriser l’authentification SAML 2.0]** afin que l’utilisateur et le mot de passe soient contrôlés par le système SAML.

Une fois cela fait, l’utilisateur peut se connecter uniquement via SAML. Lorsqu’ils accèdent à l’URL [!DNL Workfront], ils sont automatiquement redirigés vers le système SAML et invités à saisir leur nom d’utilisateur et leur mot de passe SAML.

Les informations d’identification SAML sont stockées dans un système SAML externe, tel que Microsoft des ADFS, et non dans Workfront.
