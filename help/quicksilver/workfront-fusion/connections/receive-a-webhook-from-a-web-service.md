---
product-previous: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: Recevoir un webhook à partir d’un service web
description: Si un service web n’est pas actuellement implémenté en tant qu’application dans  [!DNL Adobe Workfront Fusion], mais qu’il prend en charge l’envoi de webhooks, vous pouvez ajouter le service à un scénario à l’aide du module webhook personnalisé en tant que déclencheur instantané.
author: Becky
feature: Workfront Fusion
exl-id: f1a67dbf-c245-4936-9dcc-3fdbfc6ee3b1
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 100%

---

# Recevoir un webhook à partir d’un service web

Si un service web n’est pas actuellement implémenté en tant qu’application dans [!DNL Adobe Workfront Fusion], mais qu’il prend en charge l’envoi de webhooks, vous pouvez ajouter le service à un scénario à l’aide du module webhook personnalisé en tant que déclencheur instantané.

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
   <p>Exigences de licence héritées : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Conditions requises du produit actuel : si vous disposez de la formule [!DNL Adobe Workfront] [!UICONTROL Select] ou [!UICONTROL Prime], votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article. [!DNL Workfront Fusion] est inclus dans la formule [!DNL Workfront] [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Exigences liées aux produits hérités : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi qu’[!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez votre équipe d’administration [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], consultez Licences [[!DNL Adobe Workfront Fusion] ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Recevoir un webhook

1. Ajoutez le module **[!UICONTROL Webhooks] > [!UICONTROL Webhook personnalisé]** à votre scénario.
1. Cliquez sur **[!UICONTROL Ajouter]**, saisissez un **[!UICONTROL Nom de webhook]** dans la zone qui s’affiche, puis cliquez sur **[!UICONTROL Enregistrer]**.

1. Cliquez sur **[!UICONTROL Copier l’adresse dans le presse-papiers]**, puis cliquez sur **[!UICONTROL OK]**.

1. Connectez-vous au service web et procédez comme suit :

   1. Dans la zone des [!UICONTROL Paramètres] pour le service web, créez un webhook.
   1. Collez l’adresse que vous avez copiée dans le presse-papiers à l’étape 3.
   1. Sélectionnez l’événement qui déclenchera le webhook.

1. Dans le scénario [!DNL Workfront Fusion], indiquez le ou les événements pour lesquels vous souhaitez déclencher le module [!UICONTROL Webhook personnalisé].
1. Exécutez le scénario.

   Lorsque l’événement ou les événements se produisent, le module [!UICONTROL Webhook personnalisé] se déclenche et le scénario s’exécute.
