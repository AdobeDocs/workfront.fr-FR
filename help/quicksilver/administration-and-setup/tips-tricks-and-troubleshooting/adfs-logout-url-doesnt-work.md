---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: L'URL de déconnexion ADFS ne fonctionne pas
description: La procédure décrite sur cette page s’applique uniquement aux organisations qui ne sont pas encore intégrées à Adobe Admin Console.
author: Becky, Lisa
feature: System Setup and Administration
role: Admin
exl-id: 4d868625-e976-47b4-9e80-f1eca84a2768
TQID: https://experienceleague.adobe.com/RRaLL70JcSBcvoS6EUFuWj5Ejwljekt4QuQ3kXDx-44
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 250
ht-degree: 80%

---

# L’URL de déconnexion ADFS ne fonctionne pas

<!-- Audited: 1/2024 -->

<!--Remove me October 2026-->

>[!IMPORTANT]
>
>La procédure décrite sur cette page s’applique uniquement aux organisations qui n’ont pas encore intégré .
>
>Comme toutes les organisations ont désormais intégré Adobe Admin Console, cet article sera supprimé dans un proche avenir.
>
>Si votre entreprise est intégrée à [!UICONTROL Adobe Admin Console], consultez l’article [Différences d’administration selon les plateformes ([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

## Problème

Lors de l’utilisation de l’URL de déconnexion ADFS (https://myadfsserver.domain.net/adfs/ls/?wa=wsignout1.0), vous recevez une page de message d’erreur : « Un problème s’est produit lors de l’accès au site. Essayez de revenir sur le site. »

Si le problème persiste, contactez l’administration de ce site et indiquez le numéro de référence suivant pour identifier le problème : **57092dfc-751a-4915-8e6a-b4c5d413f8c6**

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe [!DNL Workfront]</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe [!DNL Workfront]</td> 
   <td>
   <p>Standard</p>
   <p>Plan</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td>[!UICONTROL System Administrator]</td>  
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Solution

1. Dans votre serveur de gestion ADFS, accédez aux propriétés **[!UICONTROL Relations de confiance]** > **[!UICONTROL Partie de confiance]** > `<your party trust>`.

1. Sous l’onglet **[!UICONTROL Points d’entrée]**, cliquez sur **[!UICONTROL Ajouter]**.

1. **[!UICONTROL Type de point d’entrée]** = Déconnexion SAML, liaison = POST, URL = https://myadfsserver.domain.net/adfs/ls/?wa=wsignout1.0

   Vous pouvez définir une URL de réponse si vous souhaitez qu’elle revienne vers une autre page. Nous vous recommandons toutefois le site ADFS, car il vous avertit de votre déconnexion, mais vous devez également fermer votre navigateur.
