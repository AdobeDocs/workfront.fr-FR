---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Format de domaine pour les appels API Adobe Workfront
description: Localiser votre domaine à utiliser dans l’API Adobe Workfront
author: Becky
feature: Workfront API
role: Developer
exl-id: 8f5b78c9-b84f-4f56-b7cc-ba686fac2da1
source-git-commit: c2ce6776ceebe3c1d3915e3791fc84eb0245ba4d
workflow-type: ht
source-wordcount: '147'
ht-degree: 100%

---

# Format de domaine pour les appels API Adobe Workfront

Lorsque vous effectuez un appel API vers l’API Workfront, vous utilisez le domaine de votre entreprise dans l’appel. Le format de cette URL de domaine varie selon que votre entreprise a été intégrée ou non à Adobe Unified Shell.

Pour savoir si votre entreprise se trouve sur Adobe Unified Shell, examinez l’URL qui s’affiche lorsque vous consultez une page Workfront.

| L’URL Workfront commence par : | URL des appels API : |
|---|---|
| `<yourdomain>.my.workfront.com` | `<yourdomain>.my.workfront.com` |
| `experience.adobe.com` | `<yourdomain>.my.workfront.adobe.com` |

Pour localiser votre domaine :

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (si disponible), cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis sur **[!UICONTROL Configuration]** ![icône Configuration](/help/_includes/assets/gear-icon-setup.png).
1. Sélectionnez **Système**, puis **Infos client**.

   Votre domaine est répertorié à droite de l’écran.

   ![Domaine](assets/domain.png)

