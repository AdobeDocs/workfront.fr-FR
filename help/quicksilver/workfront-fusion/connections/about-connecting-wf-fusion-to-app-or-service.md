---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: A propos de la connexion [!DNL Adobe Workfront Fusion] vers une application ou un service
description: Pour la plupart des applications, il est nécessaire de créer une connexion, par laquelle [!DNL Adobe Workfront Fusion] peut communiquer avec le service tiers donné en fonction des paramètres du scénario spécifique.
author: Becky
feature: Workfront Fusion
exl-id: 2d5cf083-9893-45e8-8f7d-0f8f5a74eef3
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 0%

---

# A propos de la connexion [!DNL Adobe Workfront Fusion] vers une application ou un service

Pour la plupart des applications, il est nécessaire de créer une connexion, par laquelle [!DNL Adobe Workfront Fusion] peut communiquer avec le service tiers donné en fonction des paramètres du scénario spécifique.

Par exemple, si vous souhaitez créer un scénario qui récupère des informations de [!DNL Workfront], vous devez accorder l’autorisation d’accès pour [!DNL Workfront Fusion] pour accéder à [!DNL Workfront] compte .

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

## Droits d’accès

Pour chaque connexion, [!DNL Workfront Fusion] ne nécessite que les droits d’accès nécessaires pour réussir un scénario donné. Par exemple, si vous créez un scénario pour répertorier des documents à partir de [!DNL Google Docs], [!DNL Workfront Fusion] ne demande pas l’autorisation d’obtenir le contenu des documents.

Malheureusement, tous les services ne vous permettent pas de limiter l’accès à des tâches spécifiques. Par conséquent, [!DNL Workfront Fusion] doivent exiger des droits d’accès complets. Pour plus d’informations sur les restrictions [!DNL Workfront Fusion] pour accéder à votre compte enregistré pour ces services, consultez la documentation spécifique à l’application.

## À propos de l’administration des connexions

Vous pouvez administrer toutes les connexions à partir du [!UICONTROL Connexions] zone. Ici, vous pouvez :

* Identifier les autorisations accordées à [!DNL Workfront Fusion] pour chaque connexion
* Renommer les connexions
* Réautoriser les connexions existantes
* Suppression de connexions existantes
* Vérifier que la connexion au service a bien été établie

Pour ouvrir la [!UICONTROL Connexions] zone, cliquez sur <b>[!UICONTROL Connexions]</b> dans le volet de navigation de gauche.

## Renouveler une connexion

[!DNL Workfront Fusion] obtient généralement des droits d’accès à un service donné pendant une période illimitée. Cependant, ce n&#39;est pas toujours le cas. Avec certains services, l’autorisation d’accès doit être renouvelée après un certain temps. Dans ce cas, [!DNL Workfront Fusion] vous avertit par e-mail peu de temps avant l’expiration de ses droits d’accès.

Pour renouveler une connexion :

1. Cliquez sur le bouton **[!UICONTROL Réautoriser]** dans le **[!UICONTROL Connexions]** zone.
