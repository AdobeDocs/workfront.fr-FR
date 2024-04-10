---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Format de domaine pour les appels API Adobe Workfront
description: Localiser votre domaine à utiliser dans l’API Adobe Workfront
author: Becky
feature: Workfront API
role: Developer
exl-id: 8f5b78c9-b84f-4f56-b7cc-ba686fac2da1
source-git-commit: c2ce6776ceebe3c1d3915e3791fc84eb0245ba4d
workflow-type: tm+mt
source-wordcount: '147'
ht-degree: 0%

---

# Format de domaine pour les appels API Adobe Workfront

Lorsque vous effectuez un appel API à l’API Workfront, vous utilisez le domaine de votre organisation dans l’appel. Le format de cette URL de domaine diffère selon que votre organisation a été intégrée ou non au Unified Shell d’Adobe.

Pour savoir si votre organisation utilise le shell unifié d’Adobe, examinez l’URL qui s’affiche lorsque vous consultez une page Workfront.

| L’URL de Workfront commence par : | URL pour les appels API : |
|---|---|
| `<yourdomain>.my.workfront.com` | `<yourdomain>.my.workfront.com` |
| `experience.adobe.com` | `<yourdomain>.my.workfront.adobe.com` |

Pour localiser votre domaine :

1. Cliquez sur le lien **[!UICONTROL Menu principal]** icône ![Menu principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront ou (le cas échéant), cliquez sur le lien **[!UICONTROL Menu principal]** icône ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis cliquez sur **[!UICONTROL Configuration]** ![Icône Configurer](/help/_includes/assets/gear-icon-setup.png).
1. Sélectionner **Système**, puis sélectionnez **Informations sur le client**.

   Votre domaine est répertorié à droite de l’écran.

   ![Domaine](assets/domain.png)

