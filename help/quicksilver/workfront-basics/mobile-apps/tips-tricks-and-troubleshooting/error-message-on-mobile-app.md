---
content-type: tips-tricks-troubleshooting
product-previous: mobile
navigation-topic: tips-tricks-and-troubleshooting-mobile-apps
title: '"Message d’erreur sur le [!DNL Adobe Workfront] Application mobile : "Votre compte n’est pas activé sur l’API.""'
description: '"Message d’erreur sur le [!DNL Adobe Workfront] Application mobile : "Votre compte n’est pas activé sur l’API.""'
author: Lisa
feature: Get Started with Workfront
exl-id: 120e56f4-9fd5-4c41-890e-981937714db0
source-git-commit: fdef22d9685d349a6f9492dec98475493ee9c048
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 2%

---

# Message d’erreur sur la variable [!DNL Adobe Workfront] Application mobile : &quot;[!UICONTROL Votre compte n’est pas activé dans l’API.]&quot;

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan</strong></td> 
   <td> <p> Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe [!DNL Workfront] license</strong></td> 
   <td> <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Paramétrages du niveau d'accès</strong></td> 
   <td> <p>[!UICONTROL Administrateur système] </p> </td> 
  </tr> 
 </tbody> 
</table>

## Problème

Lors de la tentative de connexion à la variable [!DNL Adobe Workfront] mobile, vous recevez l’erreur suivante : *[!UICONTROL Votre compte n’est pas activé dans l’API. Faites savoir à votre administrateur système et il vous installera. Désolé pour ça.]*

## Cause

Votre [!DNL Workfront] L’administrateur n’a pas activé votre [!DNL Workfront] à accéder à partir d’un appareil mobile.

## Solution

1. Connectez-vous au [!DNL Workfront] application web en tant que [!DNL Workfront] Administrateur.
1. Accédez au **[!UICONTROL Configuration]** zone.
1. Développez l’objet **[!UICONTROL Système]** , puis cliquez sur **[!UICONTROL Préférences]**.

1. Sous , **[!UICONTROL Sécurité]** , sélectionnez **[!UICONTROL Laisser les utilisateurs utiliser [!DNL Workfront]des applications mobiles et de la variable [!DNL Workfront Outlook] Module complémentaire]** pour l’activer.

1. Cliquer sur **[!UICONTROL Enregistrer]**.\
   Tous les utilisateurs du système peuvent désormais accéder à [!DNL Workfront] à partir de leurs applications mobiles et de [!DNL Outlook].
