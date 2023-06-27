---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Configurez les paramètres d’un module dans [!DNL Adobe Workfront Fusion]
description: Vous devez configurer les paramètres de chaque module que vous créez.
author: Becky
feature: Workfront Fusion
exl-id: 7e66728d-8c6f-4597-98c4-bc6d36f96911
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 1%

---

# Configurez les paramètres d’un module dans [!DNL Adobe Workfront Fusion]

Vous devez configurer les paramètres de chaque module que vous créez.

Par exemple, la variable [[!DNL Dropbox] modules](../../workfront-fusion/apps-and-their-modules/dropbox-modules.md) Les modules nécessitent de spécifier le dossier cible dans lequel vous souhaitez charger les fichiers. Pour le [[!UICONTROL Email] modules](../../workfront-fusion/apps-and-their-modules/email-modules.md) , vous devez saisir l’adresse email à laquelle les emails doivent être envoyés.

>[!NOTE]
>
>Outre les paramètres du module, vous pouvez également ajuster les paramètres d’un scénario. Vous pouvez renommer votre scénario, modifier sa planification et spécifier des paramètres supplémentaires, entre autres actions.

## Exigences d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] ou supérieur</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence [!UICONTROL Adobe Workfront Fusion]**</td> 
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

## Configuration des paramètres d’un module

1. Ajoutez un nouveau module à un scénario.

   Ou

   Cliquez sur l’icône du module dans l’éditeur de scénarios, comme décrit dans la section [Création d’un scénario dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. Si nécessaire pour le module, créez une **[!UICONTROL Connexion]** à votre compte utilisateur enregistré pour ce service donné, comme décrit dans la section [A propos de la connexion [!DNL Adobe Workfront Fusion] vers une application ou un service](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).
1. Dans chaque champ, saisissez le texte approprié.

   Ou

   Cliquez sur **[!UICONTROL Carte]** s’il apparaît à droite du champ, mappez un élément à partir d’un autre module dans votre scénario.

   Des paramètres bodés sont requis.

   Pour plus d’informations sur les différents types de données d’élément [!DNL Workfront Fusion] peut reconnaître (date, nombre et texte, par exemple), voir [Types de données d’élément dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md).

1. (Conditionnel) Si le module contient des options avancées que vous souhaitez afficher et utiliser, sélectionnez **[!UICONTROL Afficher les paramètres avancés]**.
