---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Type de licence utilisateur externe manquant dans les niveaux d'accès
description: Je ne peux plus voir le type de licence utilisateur externe sous Niveaux d’accès dans Configuration.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: fcc876d9-0512-424a-a731-6bbacd55af3f
TQID: https://experienceleague.adobe.com/g65Yq7r0Hvr6ZyC2niVw4Dnbil37epPeoyfQVOWOiy8
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: d095671a-1355-40aa-8b5f-06c33c68080bid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 119
ht-degree: 92%

---

# Le type de licence Utilisateur externe ne figure pas dans les niveaux d’accès

## Problème

Je ne peux plus voir le type de licence utilisateur externe sous Niveaux d’accès dans Configuration.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] paquet</td> 
   <td><p>Tous</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licence</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Solution

1. Accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Système]** > **[!UICONTROL Préférences]**.

1. Dans la section **[!UICONTROL Sécurité]**, assurez-vous que l’option **[!UICONTROL Collaborer avec des personnes sans les comptes Workfront en utilisant leur adresse e-mail]** est activée.

   Si cette option n’est pas activée, l’utilisateur ou l’utilisatrice externe n’apparaît pas dans la configuration du niveau d’accès.
