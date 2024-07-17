---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Variables mathématiques dans [!DNL Adobe Workfront Fusion]
description: Les variables mathématiques suivantes sont disponibles dans le panneau  [!DNL Adobe Workfront Fusion mapping] .
author: Becky
feature: Workfront Fusion
exl-id: 2fb561d2-0780-4fd6-87b3-5360a02df177
source-git-commit: c325e16ba0cde4cd48fc3e40358a9ea9ed310659
workflow-type: tm+mt
source-wordcount: '131'
ht-degree: 40%

---

# Variables mathématiques dans [!DNL Adobe Workfront Fusion]

<!--Audited: 4/2024-->

## Conditions d’accès

Pour utiliser les fonctionnalités décrites dans cet article, vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col>  
 <col>  
 <tbody>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront] plan</td>  
   <td> <p>N’importe quelle</p> </td>  
  </tr>  
  <tr data-mc-conditions="">  
   <td role="rowheader">[!DNL Adobe Workfront] licence</td>  
   <td> <p>Nouvelle : [!UICONTROL Standard]</p><p>Ou</p><p>Actuelle : [!UICONTROL Work] ou licence supérieure</p> </td>  
  </tr>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licence**</td>  
   <td> 
   <p>Actuel : aucune exigence de licence [!DNL Workfront Fusion].</p> 
   <p>Ou</p> 
   <p>Hérité : Tout </p> 
   </td>  
  </tr>  
  <tr>  
   <td role="rowheader">Produit</td>  
   <td> 
   <p>Nouveau :</p> <ul><li>Formule [!UICONTROL Select] ou [!UICONTROL Prime] [!DNL Workfront] : votre entreprise doit acheter [!DNL Adobe Workfront Fusion].</li><li>Plan [!UICONTROL Ultimate] [!DNL Workfront] : [!DNL Workfront Fusion] est inclus.</li></ul> 
   <p>Ou</p> 
   <p>Actuel : votre organisation doit acheter [!DNL Adobe Workfront Fusion].</p> 
   </td>  
  </tr> 
 </tbody>  
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], consultez les [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## pi

Représente le symbole mathématique $\pi$.

## [!UICONTROL random]

Renvoie un nombre pseudo-aléatoire à virgule flottante dans la plage [`0`,`1`] (y compris `0`, mais pas `1`).

Utilisez la formule suivante pour générer un nombre pseudo-aléatoire entier dans la plage [`min`,`max`] (y compris `min` et `max`) :

![](assets/math-variable-random-350x61.png)

```
floor(random * (1.max - 1.min + 1)) + 1.min
```
