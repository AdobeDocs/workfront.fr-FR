---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Modules MIME
description: Vous pouvez utiliser les types MIME dans Adobe Workfront Fusion. Les types MIME (Multipurpose Internet Mail Extension) sont des étiquettes qui permettent aux logiciels d’identifier différents types de données partagées sur Internet. Les serveurs Web et les navigateurs utilisent le type MIME pour déterminer ce qui doit être fait avec un fichier. Par exemple, un fichier de type MIME text/html sera traité dans un navigateur différemment d’un fichier de type MIME image/jpeg. Les types MIME fonctionnent indépendamment du système d’exploitation et du matériel.
author: Becky
feature: Workfront Fusion
exl-id: ebbf6ad0-a1d0-47f8-849f-7bba1e0763d3
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 0%

---

# [!UICONTROL MIME] modules

Vous pouvez utiliser les types MIME dans Adobe Workfront Fusion. Les types MIME (Multipurpose Internet Mail Extension) sont des étiquettes qui permettent aux logiciels d’identifier différents types de données partagées sur Internet. Les serveurs Web et les navigateurs utilisent le type MIME pour déterminer ce qui doit être fait avec un fichier. Par exemple, un fichier de type MIME `text/html` sera traité dans un navigateur différemment d’un fichier de type MIME. `image/jpeg`. Les types MIME fonctionnent indépendamment du système d’exploitation et du matériel.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail] </p> <p>[!UICONTROL [!DNL Workfront Fusion] pour l’automatisation du travail]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>Votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</td> 
  </tr> 
 </tbody> 
</table>

Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

Pour plus d’informations sur [!DNL Adobe Workfront Fusion] licences, voir [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL MIME] modules et leurs champs

### [!UICONTROL Obtention d’un type MIME]

Ce module du transformateur renvoie le type MIME associé à un nom, un chemin ou une extension donnés.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL File]</td> 
   <td> <p>Saisissez ou mappez le fichier pour lequel vous souhaitez déterminer le type MIME. </p> <p>Vous pouvez saisir le fichier à l’aide de :</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Chemin du fichier]</strong> </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemple : </b></span></span>/file/image.jpeg</p> </li> 
     <li><strong>[!UICONTROL Nom du fichier]</strong>  <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemple : </b></span></span>image.jpeg</p> </li> 
     <li><strong>[!UICONTROL Extension de fichier]</strong>  <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemple : </b></span></span>jpeg</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Obtention d’une extension de fichier]

Ce module du transformateur renvoie l’extension de fichier d’origine pour un type MIME donné.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL MIME type]</td> 
   <td> <p>Saisissez ou mappez le type MIME pour lequel vous souhaitez déterminer l’extension de fichier. </p> </td> 
  </tr> 
 </tbody> 
</table>
