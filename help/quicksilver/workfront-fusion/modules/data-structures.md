---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Structures de données dans  [!DNL Adobe Workfront Fusion]
description: Une structure de données est un document qui décrit en détail le format des données transférées vers Adobe Workfront Fusion. Sur la base de ce document, l’éditeur de scénario peut déterminer quel module renvoie ou reçoit quel type de données. Les documents de structure de données sont le plus souvent utilisés pour sérialiser/analyser des formats de données tels que JSON, XML, CSV, etc.
author: Becky
feature: Workfront Fusion
exl-id: 35a7e906-7ca2-433d-87a9-bbb01babffb0
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 34%

---

# Structures de données dans [!DNL Adobe Workfront Fusion]

Une structure de données est un document qui décrit en détail le format des données transférées vers [!DNL Adobe Workfront Fusion]. Sur la base de ce document, l’éditeur de scénario peut déterminer quel module renvoie ou reçoit quel type de données. Les documents de structure de données sont le plus souvent utilisés pour sérialiser/analyser des formats de données tels que JSON, XML, CSV, etc.

Vous pouvez créer une structure de données en cliquant sur le bouton [!UICONTROL Créer une structure de données] dans la section [!UICONTROL Présentation de la structure de données] ou dans les paramètres du module qui nécessite la spécification de la structure de données.

Les types de données pris en charge sont décrits dans l’article [[!UICONTROL Types de modules]](../../workfront-fusion/modules/module-types.md) .

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

## Générateur de structure de données

Les structures de données n&#39;ont pas toujours besoin d&#39;être créées. Vous pouvez faciliter la tâche en utilisant un modèle issu de notre générateur intégré. En fournissant un échantillon de données, le générateur crée automatiquement une structure de données basée sur l’échantillon de données que vous avez saisi. La structure de données créée peut alors être modifiée manuellement.

![](assets/data-structure-generator-350x341.jpg)
