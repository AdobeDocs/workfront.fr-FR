---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Fonctions générales dans Adobe Workfront Fusion
description: Les fonctions générales suivantes sont disponibles dans le panneau Mappage de fusion Adobe Workfront .
author: Becky
feature: Workfront Fusion
exl-id: 74bfda4e-5690-4b8c-ac58-20cf261f188d
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 2%

---

# Fonctions générales dans [!DNL Adobe Workfront Fusion]

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

## [!UICONTROL get (objet ou tableau) ; path)]

Renvoie le chemin d’accès à la valeur d’un objet ou d’un tableau. Pour accéder aux objets imbriqués, utilisez la notation par points. Le premier élément d’un tableau est index 1.

>[!INFO]
>
>**Exemples:**
>
>* `get( array ; 1 + 1 )`
>* `get( array ; 5.raw_name )`
>* `get( object ; raw_name )`
>* `get( object ; raw_name.sub_raw_name )`


## [!UICONTROL if (expression) value1; value2)]

Renvoie le `value1` si l’expression est évaluée à true ; Sinon, elle renvoie la variable `value2`.

>[!INFO]
>
>**Exemples:**
>
>* `if( 1 = 1 ; A ; B )`
   >
   >    Renvoie A
>
>* `if( = 2 ; A ; B )`
   >
   >   Renvoie B


## [!UICONTROL ifempty (value1; value2)]

Renvoie le `value1` si cette valeur n’est pas vide ; Sinon, elle renvoie la variable `value2`.

>[!INFO]
>
>**Exemples:**
>
>* `ifempty(` `A` `;` `B` )
   >
   >   Renvoie A
>
>* `ifempty(` `unknown` `;` `B` )
   >
   >   Renvoie B
>
>* `ifempty(` `""` `;` `B` )
   >
   >   Renvoie B


## [!UICONTROL switch (expression); value1; result1; [value2; result2; ...]; [else])]

évalue une valeur (appelée expression) par rapport à une liste de valeurs ; renvoie le résultat correspondant à la première valeur correspondante.

>[!INFO]
>
>**Exemples:**
>
>* `switch( B ; A ; 1 ; B ; 2 ; C ; 3 )`
   >
   >   Renvoie 2
>
>* `switch( C ; A ; 1 ; B ; 2 ; C ; 3 )`
   >
   >   Renvoie 3
>
>* `switch( X ; A ; 1 ; B ; 2 ; C ; 3 ; 4 )`
>
>  Renvoie 4

## [!UICONTROL omit(object); key1; [key2; ...])]

Omet les clés données de l’objet et renvoie le reste.

>[!INFO]
>
>**Exemple:**
>
>`omit(` Utilisateur `;` password `)`
>
>Renvoie une collection des informations de l’utilisateur, à l’exclusion du mot de passe.

## [!UICONTROL pick(objet); key1; [key2; ...])]

Sélectionne uniquement les clés données de l’objet.

>[!INFO]
>
>**Exemple:**
>
>`pick(` Utilisateur `;` password `;` email `)`
>
>Renvoie une collection contenant uniquement le mot de passe et l’adresse électronique de l’utilisateur.
