---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Modules Qualtrics
description: Dans un [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les workflows qui utilisent Qualtrics et les connecter à plusieurs applications et services tiers.
author: Becky
feature: Workfront Fusion
exl-id: 146802cd-b863-4c93-b767-50e05892c4de
source-git-commit: 8b4182ae2b32488a02cacc16fcb6a246fcb571fd
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 0%

---

# Modules Qualtrics

Dans un [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les workflows qui utilisent [!DNL Qualtrics], ainsi que de la connecter à plusieurs applications et services tiers.

Si vous avez besoin d’instructions sur la création d’un scénario, reportez-vous à la section [Création d’un scénario dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Pour plus d’informations sur les modules, voir [Modules dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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
   <td>
   <p>Exigences de licence actuelles : Non [!DNL Workfront Fusion] conditions requises pour obtenir une licence.</p>
   <p>Ou</p>
   <p>Exigences de licence héritées : [!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Exigences actuelles du produit : Si vous disposez de [!UICONTROL Select] ou [!UICONTROL Prime] [!DNL Adobe Workfront] Planifiez, votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article. [!DNL Workfront Fusion] est inclus dans l’[!UICONTROL Ultimate] [!DNL Workfront] planifiez.</p>
   <p>Ou</p>
   <p>Exigences de produit héritées : Votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

Pour plus d’informations sur [!DNL Adobe Workfront Fusion] licences, voir [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Conditions préalables

Pour utiliser [!DNL Qualtrics] modules, vous devez disposer d’un [!UICONTROL Qualtrics] compte .

## Connexion [!DNL Qualtrics] to [!DNL Workfront Fusion]

Vous pouvez créer une connexion à votre [!DNL Qualtrics] compte directement depuis l’intérieur d’un [!UICONTROL Qualtrics] module .

1. Dans n’importe quel [!UICONTROL Qualtrics] module, cliquez sur **[!UICONTROL Ajouter]** en regard de [!UICONTROL Connexion] champ .
1. Renseignez les informations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Nom de la connexion]</p> </td> 
      <td> <p>Saisissez le nom de la nouvelle connexion.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL ID du centre de données] </td> 
      <td>Utiliser le format <code>&lt;Data Center ID>.qualtrics.com</code>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Clé API]</td> 
      <td>Pour localiser votre clé d’API, reportez-vous à la section [!DNL Qualtrics] documentation.</td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **[!UICONTROL Continuer]** pour créer la connexion et revenir au module .

## [!DNL Qualtrics] modules et leurs champs

Les modules suivants sont disponibles pour la [!DNL Qualtrics] connecteur :

* [!UICONTROL Afficher la nouvelle réponse à une enquête]
* [!UICONTROL Création d’un contact de répertoire]
* [!UICONTROL Suppression d’un contact d’annuaire]
* [!UICONTROL Obtention d’un contact de répertoire]
* [!UICONTROL Mettre à jour un contact de répertoire]
* [!UICONTROL Créer une nouvelle distribution d&#39;enquête par SMS]
* [!UICONTROL Diffuser un questionnaire par email]
* [!UICONTROL Effectuer un appel API]
* [!UICONTROL Répertorier les contacts du répertoire]
