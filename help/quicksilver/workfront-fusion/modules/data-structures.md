---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Structures de données dans [!DNL Adobe Workfront Fusion]
description: Une structure de données est un document qui décrit en détail le format des données transférées vers Adobe Workfront Fusion. Sur la base de ce document, l’éditeur de scénario peut déterminer quel module renvoie ou reçoit quel type de données. Les documents de structure de données sont le plus souvent utilisés pour sérialiser/analyser des formats de données tels que JSON, XML, CSV, etc.
author: Becky
feature: Workfront Fusion
exl-id: 35a7e906-7ca2-433d-87a9-bbb01babffb0
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 0%

---

# Structures de données dans [!DNL Adobe Workfront Fusion]

Une structure de données est un document qui décrit en détail le format des données transférées vers [!DNL Adobe Workfront Fusion]. Sur la base de ce document, l’éditeur de scénario peut déterminer quel module renvoie ou reçoit quel type de données. Les documents de structure de données sont le plus souvent utilisés pour sérialiser/analyser des formats de données tels que JSON, XML, CSV, etc.

Vous pouvez créer une structure de données en cliquant sur le [!UICONTROL Création d’une structure de données] dans le [!UICONTROL Présentation de la structure de données] ou dans les paramètres du module qui nécessite la spécification de la structure de données.

Les types de données pris en charge sont décrits dans la section [[!UICONTROL Types de modules]](../../workfront-fusion/modules/module-types.md) article.

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

## Générateur de structure de données

Les structures de données n&#39;ont pas toujours besoin d&#39;être créées. Vous pouvez faciliter la tâche en utilisant un modèle issu de notre générateur intégré. En fournissant un échantillon de données, le générateur crée automatiquement une structure de données basée sur l’échantillon de données que vous avez saisi. La structure de données créée peut alors être modifiée manuellement.

![](assets/data-structure-generator-350x341.jpg)
