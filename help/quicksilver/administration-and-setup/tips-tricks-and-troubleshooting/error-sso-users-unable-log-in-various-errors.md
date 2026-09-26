---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Erreur : les utilisateurs et utilisatrices de la SSO ne peuvent pas se connecter à [!DNL Adobe Workfront] en raison de diverses erreurs'
description: Lorsque vous recevez une erreur de connexion à propos de l’authentification unique fédérée, de votre combinaison nom d’utilisateur/mot de passe ou de votre accès à [!DNL Workfront], le problème peut être que votre instance [!DNL Workfront] utilise l’authentification unique et que vous essayez de vous connecter à l’aide d’une URL incorrecte.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 92936761-cda3-41ab-88b1-ec1cac3900d4
TQID: 'https://experienceleague.adobe.com/8L78zoOjC2KgtVKTorhvWDd8MvaficRL2pZKOfrlGSs'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '174'
ht-degree: 68%
---
# Erreur : les utilisateurs et utilisatrices de la SSO ne peuvent pas se connecter à [!DNL Adobe Workfront] en raison de diverses erreurs

## Problème

Je ne parviens pas à me connecter à [!DNL Workfront] et j’ai reçu l’une des erreurs suivantes :

* Désolé, vous ne pouvez pas accéder à [!DNL Workfront] à partir de cet écran de connexion. [!DNL Workfront] est configuré pour l&#39;authentification FSSO avec SAML 2.0. Contactez votre administrateur [!DNL Workfront].
* Cette combinaison de nom d’utilisateur ou d’utilisatrice/mot de passe était incorrecte. Vérifiez que le verrouillage des majuscules n’est pas activé et réessayez.
* Désolé, vous n’avez pas accès à [!DNL Workfront]. Veuillez contacter votre équipe d’administration [!DNL Workfront] pour obtenir un nom d’utilisateur ou d’utilisatrice et un mot de passe.

## Solution

Votre instance [!DNL Workfront] utilise la SSO et vous essayez de vous connecter via une URL incorrecte. Vérifiez que vous vous connectez en utilisant la bonne URL sans rien après « .com ».

>[!TIP]
>
>Supprimez tous les signets existants dont l’URL n’est pas valide.
