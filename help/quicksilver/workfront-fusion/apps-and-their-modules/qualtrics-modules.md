---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connecteur
navigation-topic: apps-and-their-modules
title: Modules Qualtrics
description: Dans un scénario  [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les processus qui utilisent Qualtrics et les connecter à plusieurs applications et services tiers.
author: Becky
feature: Workfront Fusion
exl-id: 146802cd-b863-4c93-b767-50e05892c4de
source-git-commit: 8b4182ae2b32488a02cacc16fcb6a246fcb571fd
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 53%

---

# Modules Qualtrics

Dans un scénario [!DNL Adobe Workfront Fusion], vous pouvez automatiser les workflows qui utilisent [!DNL Qualtrics] et les connecter à plusieurs applications et services tiers.

Si vous avez besoin d’instructions sur la création d’un scénario, voir [Créer un scénario dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Pour plus d’informations sur les modules, consultez [Modules dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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
   <p>Exigence de licence héritée : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
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

## Conditions préalables

Pour utiliser les modules [!DNL Qualtrics], vous devez disposer d’un compte [!UICONTROL Qualtrics].

## Connexion de [!DNL Qualtrics] à [!DNL Workfront Fusion]

Vous pouvez créer une connexion à votre compte [!DNL Qualtrics] directement depuis un module [!UICONTROL Qualtrics].

1. Dans un module [!UICONTROL  Qualtrics], cliquez sur **[!UICONTROL Ajouter]** en regard du champ [!UICONTROL Connexion].
1. Renseignez les informations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Connection name]</p> </td> 
      <td> <p>Saisissez un nom pour la nouvelle connexion.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL ID du centre de données] </td> 
      <td>Utilisez le format <code>&lt;Data Center ID>.qualtrics.com</code>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Clé API]</td> 
      <td>Pour localiser votre clé d’API, consultez la documentation [!DNL Qualtrics].</td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **[!UICONTROL Continuer]** pour créer la connexion et retourner au module.

## Modules [!DNL Qualtrics] et leurs champs

Les modules suivants sont disponibles pour le connecteur [!DNL Qualtrics] :

* [!UICONTROL Regarder la nouvelle réponse à une enquête]
* [!UICONTROL Créer un contact de répertoire]
* [!UICONTROL Supprimer un contact de répertoire]
* [!UICONTROL Obtenir un contact de répertoire]
* [!UICONTROL Mettre à jour un contact de répertoire]
* [!UICONTROL Créer une distribution d&#39;enquête par SMS]
* [!UICONTROL Diffuser une enquête par courrier électronique]
* [!UICONTROL Effectuer un appel API]
* [!UICONTROL Contacts de répertoire de liste]
