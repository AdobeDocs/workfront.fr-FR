---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Configurez les paramètres d’un module dans [!DNL Adobe Workfront Fusion]
description: Vous devez configurer les paramètres de chaque module que vous créez.
author: Becky
feature: Workfront Fusion
exl-id: 7e66728d-8c6f-4597-98c4-bc6d36f96911
source-git-commit: f11af8d9d1e5fa65c2efb4d882d25f9e13784611
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 31%

---

# Configurez les paramètres d’un module dans [!DNL Adobe Workfront Fusion]

Vous devez configurer les paramètres de chaque module que vous créez.

Par exemple, la variable [[!DNL Dropbox] modules](../../workfront-fusion/apps-and-their-modules/dropbox-modules.md) Les modules nécessitent de spécifier le dossier cible dans lequel vous souhaitez charger les fichiers. Pour le [[!UICONTROL Email] modules](../../workfront-fusion/apps-and-their-modules/email-modules.md) , vous devez saisir l’adresse email à laquelle les emails doivent être envoyés.

>[!NOTE]
>
>Outre les paramètres du module, vous pouvez également ajuster les paramètres d’un scénario. Vous pouvez renommer votre scénario, modifier sa planification et spécifier des paramètres supplémentaires, entre autres actions.

## Conditions d’accès

Pour utiliser les fonctionnalités décrites dans cet article, vous devez disposer des éléments suivants :

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] forfait*</td> 
   <td> <p>[!DNL Pro] ou supérieur</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence [!UICONTROL Adobe Workfront Fusion]**</td> 
   <td>
   <p>Exigences de licence actuelle : aucune exigence de licence [!DNL Workfront Fusion]</p>
   <p>Ou</p>
   <p>Exigences de licence héritées : [!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail] </p>
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

## Configuration des paramètres d’un module

1. Ajoutez un nouveau module à un scénario.

   Ou

   Cliquez sur l’icône du module dans l’éditeur de scénarios, comme décrit dans la section [Créez un scénario dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. Si nécessaire pour le module, créez une **[!UICONTROL Connexion]** à votre compte utilisateur enregistré pour ce service donné, comme décrit dans la section [Présentation des connexions](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).
1. Dans chaque champ, saisissez le texte approprié.

   Ou

   Cliquez sur **[!UICONTROL Carte]** s’il apparaît à droite du champ, mappez un élément à partir d’un autre module dans votre scénario.

   Des paramètres bodés sont requis.

   Pour plus d’informations sur les différents types de données d’élément [!DNL Workfront Fusion] peut reconnaître (date, nombre et texte, par exemple), voir [Types de données d’élément dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md).

1. (Conditionnel) Si le module contient des options avancées que vous souhaitez afficher et utiliser, sélectionnez **[!UICONTROL Afficher les paramètres avancés]**.
