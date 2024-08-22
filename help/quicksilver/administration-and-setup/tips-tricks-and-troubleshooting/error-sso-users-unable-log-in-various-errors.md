---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Erreur : les utilisateurs SSO ne peuvent pas se connecter à  [!DNL Adobe Workfront] en raison de diverses erreurs"
description: Lorsque vous recevez une erreur de connexion concernant l’authentification unique fédérée, votre combinaison nom d’utilisateur/mot de passe ou votre accès à l’instance  [!DNL Workfront], the problem might be that your [!DNL Workfront] utilise l’authentification unique et que vous essayez de vous connecter à l’aide d’une URL incorrecte.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 92936761-cda3-41ab-88b1-ec1cac3900d4
source-git-commit: c389b4829f16bf82a5851a597f5dd358d9c96999
workflow-type: tm+mt
source-wordcount: '166'
ht-degree: 1%

---

# Erreur : les utilisateurs SSO ne peuvent pas se connecter à [!DNL Adobe Workfront] en raison de diverses erreurs

## Problème

Je ne parviens pas à me connecter à [!DNL Workfront] et j&#39;ai reçu l&#39;une des erreurs suivantes :

* Désolé, vous ne pouvez pas accéder à [!DNL Workfront] via cet écran de connexion. [!DNL Workfront] est configuré pour l’authentification unique fédérée avec SAML 2.0. Veuillez contacter votre administrateur [!DNL Workfront].
* Cette combinaison nom d&#39;utilisateur/mot de passe n&#39;était pas tout à fait correcte. Assurez-vous que le cadenas n’est pas allumé et réessayez.
* Désolé, vous n&#39;avez pas accès à [!DNL Workfront]. Contactez votre administrateur [!DNL Workfront] pour obtenir un nom d’utilisateur et un mot de passe.

## Solution

Votre instance [!DNL Workfront] utilise la connexion unique et vous essayez de vous connecter par le biais d’une URL incorrecte. Assurez-vous que vous vous connectez à l’aide de l’URL correcte sans autre chose après &quot;.com&quot;.

>[!TIP]
>
>Supprimez les signets existants qui contiennent des URL non valides.
