---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Variables mathématiques dans [!DNL Adobe Workfront Fusion]
description: Les variables mathématiques suivantes sont disponibles dans la variable [!DNL Adobe Workfront Fusion mapping] du panneau.
author: Becky
feature: Workfront Fusion
exl-id: 2fb561d2-0780-4fd6-87b3-5360a02df177
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '118'
ht-degree: 0%

---

# Variables mathématiques dans [!DNL Adobe Workfront Fusion]

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail] </p><p>[!UICONTROL [!DNL Workfront Fusion] pour l’automatisation du travail]</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>Votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</td> 
  </tr> 
 </tbody> 
</table>

Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

Pour plus d’informations sur [!DNL Adobe Workfront Fusion] licences, voir [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL random]

Renvoie un nombre pseudo-aléatoire à virgule flottante dans la plage [`0`,`1`] (inclus `0`, mais pas `1`).

Utilisez la formule suivante pour générer un nombre pseudo-aléatoire entier dans la plage [`min`,`max`] (y compris les deux `min` et `max`) :

![](assets/math-variable-random-350x61.png)

```
{{floor(random * (1.max - 1.min + 1)) + 1.min}}
```
