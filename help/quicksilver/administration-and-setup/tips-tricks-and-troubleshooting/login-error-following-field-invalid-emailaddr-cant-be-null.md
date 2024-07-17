---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Erreur de connexion : les champs suivants ne sont pas valides : emailAddr ne peut pas être nul'
description: Lorsque j’essaie de me connecter à l’URL de mon domaine, je suis redirigé vers le portail de connexion SAML, puis redirigé vers  [!DNL Workfront]  avec une erreur indiquant que le champ emailAddr ne peut pas être nul. [!DNL Adobe Workfront]
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 15b702cf-61b8-41dc-8253-77cadc69bd80
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '147'
ht-degree: 4%

---

# Erreur de connexion : les champs suivants ne sont pas valides : emailAddr ne peut pas être nul

## Problème

Lorsque je tente de me connecter à [!DNL Adobe Workfront] avec mon URL (https://customerdomain.my.workfront.com), je suis redirigé vers le portail de connexion SAML, puis redirigé vers [!DNL Workfront] avec l’erreur suivante :

« Réessayons. Les champs suivants ne sont pas valides : emailAddr ne peut pas être nul.&quot;

## Cause

Cette erreur est provoquée par un élément incorrect dans la zone Mapper les attributs de l’utilisateur de la configuration SAML 2.0. Pour plus d’informations sur le mappage des attributs utilisateur pour SAML 2.0, voir [Configuration d’Adobe Workfront avec SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

## Solution

Mettez à jour le mappage des attributs pour l’adresse électronique, puis cliquez sur **[!UICONTROL Enregistrer]**.
