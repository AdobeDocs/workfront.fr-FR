---
title: Encryptor
description: Les modules Adobe Workfront Fusion Encryptor permettent de crypter toutes les données texte. Ils prennent actuellement en charge le cryptage des messages via AES256 et PGP (OpenPGP).
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: 9664c4f1-6467-45c9-8b9e-5a41d0e9ccb9
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 39%

---

# Encryptor

Les modules [!DNL Adobe Workfront Fusion] [!UICONTROL Encryptor] vous permettent de chiffrer des données texte. Ils prennent actuellement en charge le cryptage des messages via AES256 et PGP ([!UICONTROL OpenPGP]).

## Conditions d’accès

Pour utiliser les fonctionnalités décrites dans cet article, vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] forfait*</td>
  <td> <p>[!UICONTROL Pro] ou un forfait supérieur</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licence**</td> 
   <td>
   <p>Exigences de licence actuelle : aucune exigence de licence [!DNL Workfront Fusion]</p>
   <p>Ou</p>
   <p>Exigences de licence héritée : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration], [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Exigences du produit actuel : si vous disposez du forfait [!DNL Adobe Workfront] [!UICONTROL Select] ou [!UICONTROL Prime], votre entreprise doit acheter [!DNL Adobe Workfront Fusion] et [!DNL Adobe Workfront] pour utiliser les fonctionnalités décrites dans cet article. [!DNL Workfront Fusion] est inclus dans le forfait [!DNL Workfront] [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Exigences du produit hérité : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] et [!DNL Adobe Workfront] pour utiliser les fonctionnalités décrites dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez vote administrateur ou administratrice [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], consultez les [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Cryptage et décryptage des messages à l’aide de PGP

Lors du cryptage et du décryptage via PGP, il est nécessaire d’utiliser un trousseau et de créer une clé privée ou publique (ou les deux).

Pour plus d’informations sur les clés publiques et privées, voir [Termes de base dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/basic-terms.md). Pour plus d&#39;informations sur les chaînes de clés, voir [Clés dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/connections/keys.md).

## Modules [!UICONTROL Encryptor] et leurs champs

Lorsque vous configurez les modules [!UICONTROL Encryptor], les champs suivants s’affichent. Un titre en gras dans un module indique un champ obligatoire.

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
