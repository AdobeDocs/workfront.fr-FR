---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Format de domaine pour les appels API Adobe Workfront
description: Localiser votre domaine à utiliser dans l’API Adobe Workfront
author: Becky
feature: Workfront API
role: Developer
exl-id: 8f5b78c9-b84f-4f56-b7cc-ba686fac2da1
source-git-commit: e9a9e45720c8b9ad25e3fa9340c813a73989fb4a
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 95%

---

# Format de domaine pour les appels API Adobe Workfront

Lorsque vous effectuez un appel API vers l’API Workfront, vous utilisez le domaine de votre entreprise dans l’appel. Le format de cette URL de domaine varie selon que votre entreprise a été intégrée ou non à Adobe Unified Shell.

Pour savoir si votre entreprise se trouve sur Adobe Unified Shell, examinez l’URL qui s’affiche lorsque vous consultez une page Workfront.

| L’URL Workfront commence par : | URL des appels API : |
|---|---|
| `<yourdomain>.my.workfront.com` | `<yourdomain>.my.workfront.com` |
| `experience.adobe.com` | `<yourdomain>.my.workfront.adobe.com` |

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td><p>Standard</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Vous devez être un administrateur Workfront</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


Pour localiser votre domaine :

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (si disponible), cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis sur **[!UICONTROL Configuration]** ![icône Configuration](/help/_includes/assets/gear-icon-setup.png).
1. Sélectionnez **Système**, puis **Infos client**.

   Votre domaine est répertorié à droite de l’écran.

   ![Domaine](assets/domain.png)

