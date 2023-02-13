---
title: Crypteur
description: Les modules Adobe Workfront Fusion Encryptor permettent de crypter toutes les données texte. Ils prennent actuellement en charge le cryptage des messages via AES256 et PGP (OpenPGP).
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: 9664c4f1-6467-45c9-8b9e-5a41d0e9ccb9
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 0%

---

# Crypteur

[!DNL Adobe Workfront Fusion] [!UICONTROL Crypteur] Les modules permettent de crypter des données texte. Ils prennent actuellement en charge le cryptage des messages via AES256 et PGP ([!UICONTROL OpenPGP]).

## Exigences d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
  <td> <p>[!UICONTROL Pro] ou version ultérieure</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail] </p>   <p>[!UICONTROL [!DNL Workfront Fusion] pour l’automatisation du travail]</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>Votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</td> 
  </tr> 
 </tbody> 
</table>

Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

Pour plus d’informations sur [!DNL Adobe Workfront Fusion] licences, voir [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Cryptage et décryptage des messages à l’aide de PGP

Lors du cryptage et du décryptage via PGP, il est nécessaire d’utiliser un trousseau et de créer une clé privée ou publique (ou les deux).

Pour plus d’informations sur les clés publiques et privées, voir [Termes de base [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/basic-terms.md). Pour plus d’informations sur les chaînes de clés, voir [Raccourcis clavier [!DNL Adobe Workfront Fusion]](../../workfront-fusion/connections/keys.md).

## [!UICONTROL Crypteur] modules et leurs champs

Lors de la configuration [!UICONTROL Crypteur] , les champs suivants s’affichent. Un titre en gras dans un module indique un champ obligatoire.

### Chiffrer un message PGP

Ce module vous permet de chiffrer un message à l’aide de clés publique et privée.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Clé privée]</td>
        <td>Saisissez la clé privée de l’expéditeur. Cela peut authentifier l’identité de l’expéditeur.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Clé publique]</td>
        <td>Saisissez la clé publique du destinataire.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Message]</td>
        <td>Saisissez le message que vous souhaitez chiffrer.</td>
    </tr>

### Décrypter un message PGP

Ce module permet de déchiffrer un message à l’aide de clés publiques et privées.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Clé privée]</td>
        <td>Saisissez la clé privée du destinataire.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Clé publique]</td>
        <td>Saisissez la clé publique du destinataire. Cela peut authentifier l’identité de l’expéditeur.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Message]</td>
        <td>Faites correspondre le message que vous souhaitez décrypter.</td>
    </tr>
</table>
