---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Erreur de connexion : les champs suivants ne sont pas valides : emailAddr ne peut pas être nul.'
description: Lorsque j’essaie de me connecter [!DNL Adobe Workfront] l’URL de mon domaine, on me redirige vers le portail de connexion SAML, puis on me redirige vers [!DNL Workfront] avec une erreur indiquant que le champ emailAddr ne peut pas être nul.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 15b702cf-61b8-41dc-8253-77cadc69bd80
TQID: 'https://experienceleague.adobe.com/MfWVOYcQAVjlbxwiqVaPwipyq5ulv0toajH-2tX7c9k'
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
source-wordcount: '148'
ht-degree: 76%
---
# Erreur de connexion : les champs suivants ne sont pas valides : emailAddr ne peut pas être nul.

## Problème

Lorsque je tente de me connecter à [!DNL Adobe Workfront] avec mon URL (https://customerdomain.my.workfront.com), je fais l’objet d’une redirection vers le portail de connexion SAML, puis vers [!DNL Workfront] avec l’erreur suivante :

« Réessayons. Les champs suivants ne sont pas valides : emailAddr ne peut pas être nul. »

## Cause

Cette erreur est due à un élément incorrect dans la zone Mapper les attributs de l’utilisateur ou de l’utilisatrice de la configuration SAML 2.0. Pour plus d’informations sur le mappage des attributs de l’utilisateur ou de l’utilisatrice pour SAML 2.0, voir [Configurer Adobe Workfront avec SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

## Solution

Mettez à jour le mappage d’attributs pour l’adresse e-mail, puis cliquez sur **[!UICONTROL Enregistrer]**.
