---
product-previous: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: Recevoir un webhook d’un service web
description: Si un service web n’est actuellement pas implémenté en tant qu’application dans  [!DNL Adobe Workfront Fusion], mais qu’il prend en charge l’envoi de webhooks, vous pouvez ajouter le service à un scénario à l’aide du module webhook personnalisé en tant que déclencheur instantané.
author: Becky
feature: Workfront Fusion
exl-id: f1a67dbf-c245-4936-9dcc-3fdbfc6ee3b1
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 42%

---

# Recevoir un webhook d’un service web

Si un service Web n’est actuellement pas implémenté en tant qu’application dans [!DNL Adobe Workfront Fusion], mais qu’il prend en charge l’envoi de webhooks, vous pouvez ajouter le service à un scénario à l’aide du module webhook personnalisé en tant que déclencheur instantané.

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

## Réception d’un webhook

1. Ajoutez le module **[!UICONTROL Webhooks] >[!UICONTROL Webhook personnalisé]** à votre scénario.
1. Cliquez sur **[!UICONTROL Ajouter]**, saisissez un **[!UICONTROL nom de webhook]** dans la zone qui s’affiche, puis cliquez sur **[!UICONTROL Enregistrer]**.

1. Cliquez sur **[!UICONTROL Copier l’adresse dans le Presse-papiers]**, puis sur **[!UICONTROL OK]**.

1. Connectez-vous au service Web et procédez comme suit :

   1. Dans la zone [!UICONTROL Settings] du service Web, créez un webhook.
   1. Collez l’adresse que vous avez copiée dans le presse-papiers à l’ étape 3 .
   1. Sélectionnez l’événement qui déclenchera le webhook.

1. Dans le scénario [!DNL Workfront Fusion], spécifiez l’événement ou les événements qui doivent déclencher le module [!UICONTROL webhook personnalisé].
1. Exécutez le scénario.

   Lorsque l’événement ou les événements se produisent, le module [!UICONTROL webhook personnalisé] se déclenche et le scénario s’exécute.
