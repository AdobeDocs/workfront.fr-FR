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
ht-degree: 72%

---

# Erreur : les utilisateurs et utilisatrices de la SSO ne peuvent pas se connecter à [!DNL Adobe Workfront] en raison de diverses erreurs

## Problème

Je ne parviens pas à me connecter à [!DNL Workfront] et j’ai reçu l’une des erreurs suivantes :

* Désolé, vous ne pouvez pas accéder à [!DNL Workfront] à partir de cet écran de connexion. [!DNL Workfront] est configuré pour l’authentification unique fédérée avec SAML 2.0. Veuillez contacter votre équipe d’administration [!DNL Workfront].
* Cette combinaison de nom d’utilisateur ou d’utilisatrice/mot de passe était incorrecte. Vérifiez que le verrouillage des majuscules n’est pas activé et réessayez.
* Désolé, vous n’avez pas accès à [!DNL Workfront]. Veuillez contacter votre équipe d’administration [!DNL Workfront] pour obtenir un nom d’utilisateur ou d’utilisatrice et un mot de passe.

## Solution

Votre instance [!DNL Workfront] utilise la SSO et vous essayez de vous connecter via une URL incorrecte. Vérifiez que vous vous connectez en utilisant la bonne URL sans rien après « .com ».

>[!TIP]
>
>Supprimez tous les signets existants dont l’URL n’est pas valide.
