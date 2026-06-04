---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Format de domaine pour les appels API Adobe Workfront
description: Localiser votre domaine à utiliser dans l’API Adobe Workfront
author: Becky
feature: Workfront API
role: Developer
exl-id: 8f5b78c9-b84f-4f56-b7cc-ba686fac2da1
TQID: https://experienceleague.adobe.com/jzwKwes6zxs0KwpjFyP4VL7k2oRVx6KGUP07EQHE-gY
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 165
ht-degree: 84%

---

# Format de domaine pour les appels API Adobe Workfront

Lorsque vous effectuez un appel API vers l’API Workfront, vous utilisez le domaine de votre entreprise dans l’appel.

L’URL que vous créez pour l’appel API dépend de l’URL que vous utilisez pour vous connecter à Workfront.

| L’URL Workfront commence par : | URL des appels API : |
|---|---|
| `experience.adobe.com` | `<yourdomain>.my.workfront.adobe.com` |

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
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

