---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Erreur de connexion : les champs suivants ne sont pas valides : emailAddr ne peut pas être nul"
description: Lorsque je tente de me connecter à  [!DNL Adobe Workfront]  avec l’URL de mon domaine, je fais l’objet d’une redirection vers le portail de connexion SAML, puis vers  [!DNL Workfront]  avec une erreur indiquant que le champ emailAddr ne peut pas être nul.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 15b702cf-61b8-41dc-8253-77cadc69bd80
source-git-commit: c389b4829f16bf82a5851a597f5dd358d9c96999
workflow-type: tm+mt
source-wordcount: '147'
ht-degree: 92%

---

# Erreur de connexion : les champs suivants ne sont pas valides : emailAddr ne peut pas être nul.

## Problème

Lorsque je tente de me connecter à [!DNL Adobe Workfront] avec mon URL (https://customerdomain.my.workfront.com), je fais l’objet d’une redirection vers le portail de connexion SAML, puis vers [!DNL Workfront] avec l’erreur suivante :

« Réessayons. Les champs suivants ne sont pas valides : emailAddr ne peut pas être nul. »

## Cause

Cette erreur est due à un élément incorrect dans la zone Mapper les attributs de l’utilisateur ou de l’utilisatrice de la configuration SAML 2.0. Pour plus d’informations sur le mappage des attributs de l’utilisateur ou de l’utilisatrice pour SAML 2.0, voir [Configurer Adobe Workfront avec SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

## Solution

Mettez à jour le mappage d’attributs pour l’adresse e-mail, puis cliquez sur **[!UICONTROL Enregistrer]**.
