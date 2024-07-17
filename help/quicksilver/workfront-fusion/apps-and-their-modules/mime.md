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
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '378'
ht-degree: 32%

---

# Modules [!UICONTROL MIME]

Vous pouvez utiliser les types MIME dans Adobe Workfront Fusion. Les types MIME (Multipurpose Internet Mail Extension) sont des étiquettes qui permettent aux logiciels d’identifier différents types de données partagées sur Internet. Les serveurs Web et les navigateurs utilisent le type MIME pour déterminer ce qui doit être fait avec un fichier. Par exemple, un fichier avec le type MIME `text/html` sera traité dans un navigateur différemment d’un fichier avec le type MIME `image/jpeg`. Les types MIME fonctionnent indépendamment du système d’exploitation et du matériel.

## Conditions d’accès

Pour utiliser les fonctionnalités décrites dans cet article, vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] forfait*</td>
  <td> <p>[!UICONTROL Pro] ou un forfait supérieur</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licence**</td> 
   <td>
   <p>Exigences de licence actuelle : aucune exigence de licence [!DNL Workfront Fusion]</p>
   <p>Ou</p>
   <p>Exigences de licence héritée : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration], [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
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

## Modules [!UICONTROL MIME] et leurs champs

### [!UICONTROL Obtenir un type MIME]

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
     <li><strong>[!UICONTROL Nom de fichier]</strong>  <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemple : </b></span></span>image.jpeg</p> </li> 
     <li><strong>[!UICONTROL Extension de fichier]</strong>  <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemple : </b></span></span>jpeg</p> </li> 
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
   <td role="rowheader">[!UICONTROL MIME type]</td> 
   <td> <p>Saisissez ou mappez le type MIME pour lequel vous souhaitez déterminer l’extension de fichier. </p> </td> 
  </tr> 
 </tbody> 
</table>
