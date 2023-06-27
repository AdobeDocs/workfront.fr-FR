---
product-previous: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: Réception d’un webhook à partir d’un service Web
description: Si un service Web n’est pas actuellement implémenté en tant qu’application dans [!DNL Adobe Workfront Fusion], mais il prend en charge l’envoi de webhooks, vous pouvez ajouter le service à un scénario à l’aide du module webhook personnalisé en tant que déclencheur instantané.
author: Becky
feature: Workfront Fusion
exl-id: f1a67dbf-c245-4936-9dcc-3fdbfc6ee3b1
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 0%

---

# Réception d’un webhook à partir d’un service Web

Si un service Web n’est pas actuellement implémenté en tant qu’application dans [!DNL Adobe Workfront Fusion], mais il prend en charge l’envoi de webhooks, vous pouvez ajouter le service à un scénario à l’aide du module webhook personnalisé en tant que déclencheur instantané.

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

## Réception d’un webhook

1. Ajoutez la variable **[!UICONTROL Webhooks] >[!UICONTROL Webhook personnalisé]** à votre scénario.
1. Cliquez sur **[!UICONTROL Ajouter]**, saisissez une **[!UICONTROL Nom du webhook]** dans la zone qui s’affiche, puis cliquez sur **[!UICONTROL Enregistrer]**.

1. Cliquez sur **[!UICONTROL Copier l’adresse dans le presse-papiers]**, puis cliquez sur **[!UICONTROL OK]**.

1. Connectez-vous au service Web et procédez comme suit :

   1. Dans le [!UICONTROL Paramètres] pour le service web, créez un webhook.
   1. Collez l’adresse que vous avez copiée dans le presse-papiers à l’ étape 3 .
   1. Sélectionnez l’événement qui déclenchera le webhook.

1. Dans le [!DNL Workfront Fusion] , indiquez le ou les événements que vous souhaitez déclencher [!UICONTROL Webhook personnalisé] module .
1. Exécutez le scénario.

   Lorsque l’événement ou les événements se produisent, la variable [!UICONTROL Webhook personnalisé] se déclenchent et le scénario s’exécute.
