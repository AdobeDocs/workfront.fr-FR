---
title: Encryptor
description: Les modules Adobe Workfront Fusion Encryptor vous permettent de chiffrer n’importe quelle donnée de texte. Ils prennent actuellement en charge le chiffrement des messages via AES256 et PGP (OpenPGP).
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: 9664c4f1-6467-45c9-8b9e-5a41d0e9ccb9
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 91%

---

# Encryptor

Les modules [!DNL Adobe Workfront Fusion] [!UICONTROL Encryptor] vous permettent de chiffrer n’importe quelle donnée de texte. Ils prennent actuellement en charge le chiffrement des messages via AES256 et PGP ([!UICONTROL OpenPGP]).

## Conditions d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] formule*</td>
  <td> <p>[!UICONTROL Pro] ou version supérieure</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licence**</td> 
   <td>
   <p>Exigences de licence actuelles : aucune exigence de licence [!DNL Workfront Fusion] requise.</p>
   <p>Ou</p>
   <p>Exigences en matière de licences héritées : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration], [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Exigences actuelles du produit : si vous avez le plan [!UICONTROL Select] ou [!UICONTROL Prime] [!DNL Adobe Workfront], votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article. [!DNL Workfront Fusion] est inclus dans la formule [!DNL Workfront] [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Exigences liées aux produits hérités : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi qu’[!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez votre équipe d’administration [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], consultez la section licences [[!DNL Adobe Workfront Fusion] ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Chiffrement et déchiffrement des messages à l’aide de PGP

Lors du chiffrement et du déchiffrement via PGP, il est nécessaire d’utiliser un trousseau et de créer une clé privée ou publique (ou les deux).

Pour plus d’informations sur les clés publiques et privées, voir [Termes de base dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/basic-terms.md). Pour plus d’informations sur les trousseaux, voir [Clés dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/connections/keys.md).

## Modules [!UICONTROL Encryptor] et leurs champs

Lorsque vous configurez les modules [!UICONTROL Encryptor], les champs suivants s’affichent. Un titre en gras dans un module indique un champ obligatoire.

### Chiffrer un message PGP

Ce module permet de chiffrer un message à l’aide de clés publiques et privées.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Private key]</td>
        <td>Saisissez la clé privée de l’expéditeur ou de l’expéditrice. Cela permet d’authentifier l’identité de l’expéditeur ou de l’expéditrice.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Public key]</td>
        <td>Saisissez la clé publique de la personne destinataire.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Message]</td>
        <td>Saisissez le message que vous souhaitez chiffrer.</td>
    </tr>

### Déchiffrer un message PGP

Ce module permet de déchiffrer un message à l’aide de clés publiques et privées.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Private key]</td>
        <td>Saisissez la clé privée de la personne destinataire.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Public key]</td>
        <td>Saisissez la clé publique de la personne destinataire. Cela permet d’authentifier l’identité de l’expéditeur ou de l’expéditrice.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Message]</td>
        <td>Mappez le message que vous souhaitez déchiffrer.</td>
    </tr>
</table>
