---
content-type: tips-tricks-troubleshooting
product-previous: mobile
navigation-topic: tips-tricks-and-troubleshooting-mobile-apps
title: 'Message d’erreur sur l’application mobile  [!DNL Adobe Workfront]  : « Votre compte n’est pas activé pour l’API ».'
description: 'Message d’erreur sur l’application mobile  [!DNL Adobe Workfront]  : « Votre compte n’est pas activé pour l’API ».'
author: Lisa
feature: Get Started with Workfront
exl-id: 120e56f4-9fd5-4c41-890e-981937714db0
TQID: https://experienceleague.adobe.com/t-ANxgXpzPBSM8cGUipyAIczqSEUJGXTthbaVP5dh2E
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: d095671a-1355-40aa-8b5f-06c33c68080b
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 161
ht-degree: 68%

---

# Message d’erreur sur l’application mobile [!DNL Adobe Workfront] : « [!UICONTROL Votre compte n’est pas activé dans l’API.] »

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan</strong></td> 
   <td> <p> Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licence Adobe [!DNL Workfront]</strong></td> 
   <td> <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurations des niveaux d’accès</strong></td> 
   <td> <p>[!UICONTROL System administrator] </p> </td> 
  </tr> 
 </tbody> 
</table>

## Problème

Lors de la tentative de connexion à l’application mobile [!DNL Adobe Workfront], vous recevez le message d’erreur suivant : *[!UICONTROL Votre compte n’est pas activé dans l’API. Faites le savoir à votre administrateur ou administratrice système pour que votre compte soit activé. Toutes nos excuses.]*

## Cause

Votre administrateur ou administratrice [!DNL Workfront] n’a pas activé votre environnement [!DNL Workfront] pour que vous puissiez y accéder à partir d’un appareil mobile.

## Solution

1. Connectez-vous à l’application web [!DNL Workfront] en tant qu’administrateur ou administratrice [!DNL Workfront].
1. Accédez à la zone **[!UICONTROL Configuration]**.
1. Développez le menu **[!UICONTROL Système]**, puis cliquez sur **[!UICONTROL Préférences]**.

1. Dans la section **[!UICONTROL Sécurité]**, sélectionnez l’option **[!UICONTROL Autoriser les personnes à utiliser les applications mobiles de [!DNL Workfront]]** pour l’activer.

1. Cliquer sur **[!UICONTROL Enregistrer]**.\
   Tous les utilisateurs du système peuvent désormais accéder à [!DNL Workfront] à partir de leurs applications mobiles.
