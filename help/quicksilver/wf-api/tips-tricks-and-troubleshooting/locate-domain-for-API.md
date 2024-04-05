---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Format de domaine pour les appels API Adobe Workfront
description: Localisez votre domaine à utiliser dans l’API Adobe Workfront.
author: Becky
feature: Workfront API
role: Developer
source-git-commit: 8487f8d4b1651df268720806cfe07fa271a7b87d
workflow-type: tm+mt
source-wordcount: '147'
ht-degree: 0%

---


# Format de domaine pour les appels API Adobe Workfront

Lorsque vous effectuez un appel API vers l’API Workfront, vous utilisez le domaine de votre organisation dans l’appel . Le format de cette URL de domaine varie selon que votre organisation a été intégrée à l’Adobe Unified Shell.

Pour savoir si votre organisation se trouve sur l’Adobe de Shell unifié, examinez l’URL qui s’affiche lorsque vous affichez une page Workfront.

| L’URL Workfront commence par : | URL des appels API : |
|---|---|
| `<yourdomain>.my.workfront.com` | `<yourdomain>.my.workfront.com` |
| `experience.adobe.com` | `<yourdomain>.my.workfront.adobe.com` |

Pour localiser votre domaine :

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![Menu Principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (le cas échéant), cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![Menu Principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis cliquez sur **[!UICONTROL Configuration]** ![Icône Configuration](/help/_includes/assets/gear-icon-setup.png).
1. Sélectionner **Système**, puis sélectionnez **Informations sur le client**.

   Votre domaine est répertorié à droite de l’écran.

   ![Domaine](assets/domain.png)