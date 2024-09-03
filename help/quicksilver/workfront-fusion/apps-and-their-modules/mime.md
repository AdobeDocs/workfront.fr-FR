---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Modules MIME
description: Vous pouvez utiliser les types MIME dans Adobe Workfront Fusion. Les types MIME (Multipurpose Internet Mail Extension) sont des libellés qui permettent aux logiciels d’identifier les différents types des données partagées sur Internet. Les serveurs web et les navigateurs utilisent le type MIME pour déterminer ce qu’il convient de faire avec un fichier. Par exemple, un fichier de type MIME texte/HTML sera traité dans un navigateur différemment d’un fichier de type MIME image/JPEG. Les types MIME fonctionnent indépendamment du système d’exploitation et du matériel.
author: Becky
feature: Workfront Fusion
exl-id: ebbf6ad0-a1d0-47f8-849f-7bba1e0763d3
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '378'
ht-degree: 100%

---

# Modules [!UICONTROL MIME]

Vous pouvez utiliser les types MIME dans Adobe Workfront Fusion. Les types MIME (Multipurpose Internet Mail Extension) sont des libellés qui permettent aux logiciels d’identifier les différents types des données partagées sur Internet. Les serveurs web et les navigateurs utilisent le type MIME pour déterminer ce qu’il convient de faire avec un fichier. Par exemple, un fichier de type MIME `text/html` sera traité dans un navigateur différemment d’un fichier de type MIME `image/jpeg`. Les types MIME fonctionnent indépendamment du système d’exploitation et du matériel.

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
   <p>Exigences en matière de licences héritées : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration], [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
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

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], voir Licences [[!DNL Adobe Workfront Fusion] ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Modules [!UICONTROL MIME] et leurs champs

### [!UICONTROL Obtenir un type MIME]

Ce module du transformateur renvoie le type MIME associé à un nom, un chemin ou une extension donnés.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL File]</td> 
   <td> <p>Saisissez ou mappez le fichier pour lequel vous souhaitez déterminer le type MIME. </p> <p>Vous pouvez saisir le fichier à l’aide des éléments suivants :</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL File path]</strong> </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemple : </b></span></span>/file/image.jpeg</p> </li> 
     <li><strong>[!UICONTROL File name]</strong>  <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemple : </b></span></span>image.jpeg</p> </li> 
     <li><strong>[!UICONTROL File extension]</strong>  <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemple : </b></span></span>jpeg</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Obtenir une extension de fichier]

Ce module du transformateur renvoie l’extension de fichier d’origine pour un type MIME donné.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL MIME type]</td> 
   <td> <p>Saisissez ou mappez le type MIME pour lequel vous souhaitez déterminer l’extension de fichier. </p> </td> 
  </tr> 
 </tbody> 
</table>
