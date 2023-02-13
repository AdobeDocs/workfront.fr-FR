---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: '''Error: Les utilisateurs SSO ne peuvent pas se connecter à [!DNL Adobe Workfront] En raison de diverses erreurs'
description: Lorsque vous recevez une erreur de connexion concernant l’authentification unique fédérée, votre combinaison nom d’utilisateur/mot de passe ou votre accès à [!DNL Workfront], the problem might be that your [!DNL Workfront] utilise l’authentification unique et vous essayez de vous connecter à l’aide d’une URL incorrecte. Assurez-vous que vous vous connectez à l’aide de l’URL correcte sans rien après ".com".
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 92936761-cda3-41ab-88b1-ec1cac3900d4
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 13%

---

# Erreur : Les utilisateurs SSO ne peuvent pas se connecter à [!DNL Adobe Workfront] En raison de diverses erreurs

## Problème

Je ne parviens pas à me connecter à [!DNL Workfront] et a reçu l’une des erreurs suivantes :

* Désolé, vous ne pouvez pas accéder à [!DNL Workfront] via cet écran de connexion. [!DNL Workfront] est configuré pour l’authentification unique fédérée avec SAML 2.0. Veuillez contacter votre [!DNL Workfront] administrateur.
* Cette combinaison de nom d&#39;utilisateur/mot de passe n&#39;était pas correcte.  Vérifiez que la touche Verr Maj n&#39;est pas activée.
* Désolé, vous n&#39;avez pas accès à [!DNL Workfront]. Veuillez contacter votre [!DNL Workfront] pour obtenir un nom d’utilisateur et un mot de passe.

## Solution

Votre [!DNL Workfront] utilise l’authentification unique et vous essayez de vous connecter par le biais d’une URL incorrecte. Assurez-vous que vous vous connectez à l’aide de l’URL correcte sans autre chose après &quot;.com&quot;.

>[!TIP]
>
>Supprimez les signets existants qui contiennent des URL non valides.
