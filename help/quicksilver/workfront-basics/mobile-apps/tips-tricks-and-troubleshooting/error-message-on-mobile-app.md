---
content-type: tips-tricks-troubleshooting
product-previous: mobile
navigation-topic: tips-tricks-and-troubleshooting-mobile-apps
title: '"Message d’erreur sur l’application mobile  [!DNL Adobe Workfront]  : "Votre compte n’est pas activé sur l’API.""'
description: '"Message d’erreur sur l’application mobile  [!DNL Adobe Workfront]  : "Votre compte n’est pas activé sur l’API.""'
author: Lisa
feature: Get Started with Workfront
exl-id: 120e56f4-9fd5-4c41-890e-981937714db0
source-git-commit: fdef22d9685d349a6f9492dec98475493ee9c048
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 14%

---

# Message d’erreur sur l’application mobile [!DNL Adobe Workfront] : &quot;[!UICONTROL Votre compte n’est pas activé dans l’API.]&quot;

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan</strong></td> 
   <td> <p> N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe de la licence [!DNL Workfront]</strong></td> 
   <td> <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurations du niveau d’accès</strong></td> 
   <td> <p>[!UICONTROL Administrateur système] </p> </td> 
  </tr> 
 </tbody> 
</table>

## Problème

Lorsque vous essayez de vous connecter à l&#39;application mobile [!DNL Adobe Workfront], vous recevez l&#39;erreur suivante : *[!UICONTROL Votre compte n&#39;est pas activé par l&#39;API. Faites savoir à votre administrateur système et il vous installera. Désolé.]*

## Cause

Votre administrateur [!DNL Workfront] n&#39;a pas activé l&#39;accès à votre environnement [!DNL Workfront] à partir d&#39;un appareil mobile.

## Solution

1. Connectez-vous à l’application web [!DNL Workfront] en tant qu’administrateur [!DNL Workfront].
1. Accédez à la zone **[!UICONTROL Setup]** .
1. Développez le menu **[!UICONTROL Système]**, puis cliquez sur **[!UICONTROL Préférences]**.

1. Dans la section **[!UICONTROL Sécurité]** , sélectionnez l&#39;option **[!UICONTROL Permettre aux utilisateurs d&#39;utiliser les applications mobiles de [!DNL Workfront] et l&#39;option [!DNL Workfront Outlook] Add-in]** pour l&#39;activer.

1. Cliquer sur **[!UICONTROL Enregistrer]**.\
   Tous les utilisateurs du système peuvent désormais accéder à [!DNL Workfront] à partir de leurs applications mobiles et à partir de [!DNL Outlook].
