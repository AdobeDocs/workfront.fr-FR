---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Fonctions mathématiques dans Adobe Workfront Fusion
description: Les fonctions mathématiques suivantes sont disponibles dans le panneau Mappage de fusion Adobe Workfront .
author: Becky
feature: Workfront Fusion
exl-id: 8a3c7a89-62b5-45e9-b857-8beedd0e5af4
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 1%

---

# Fonctions mathématiques dans [!DNL Adobe Workfront Fusion]

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

## [!UICONTROL average ([tableau de valeurs]) average(value1; [value2], ...)]

Renvoie la valeur moyenne des valeurs numériques d’un tableau spécifique ou la valeur moyenne des valeurs numériques saisies unitairement.

## [!UICONTROL ceil (nombre)]

Renvoie le plus petit entier supérieur ou égal à un nombre spécifié.

>[!INFO]
>
>**Exemples:**
>
>* `ceil(` `1.2` `)`
   >
   >   Renvoie 2
>
>* `ceil(` `4` `)`
   >
   >   Renvoie 4


## [!UICONTROL floor (number)]

Renvoie le plus grand entier inférieur ou égal à un nombre spécifié.

>[!INFO]
>
>**Exemples:**
>
>* `floor(` `1.2` `)`
   >
   >   Renvoie 1
>
>* `floor(` `1.9` `)`
   >
   >   Renvoie 1
>
>* `floor(` `4` `)`
   >
   >   Renvoie 4


## [!UICONTROL formatNumber (number); decimalPOINTS; [decimalSeparator]; [millierSeparator])]

Renvoie un nombre au format demandé. Par défaut, la virgule est une virgule (,) et le séparateur des milliers est un point (.).

>[!INFO]
>
>**Exemple:**
>
>`formatNumber( 123456789 ; 3 ; , ; . )`
>
>Renvoie 123,456,789 000

## [!UICONTROL max ([tableau de valeurs]), max(value1;value2; ...)]

Renvoie le plus grand nombre d’un tableau spécifié ou le plus grand nombre parmi les nombres renseignés individuellement.

## [!UICONTROL min ([tableau de valeurs]), min(value1; value2; ...)]

Renvoie le plus petit nombre d’un tableau spécifié ou le plus petit nombre parmi les nombres saisis individuellement.

## [!UICONTROL parseNumber (number); séparateur décimal)]

Analyse une chaîne avec un nombre et renvoie le nombre. Par exemple, parseNumber(1 756,456;,)

## [!UICONTROL round (nombre)]

Arrondit une valeur numérique à l’entier le plus proche.

>[!INFO]
>
>**Exemples:**
>
>* `round(` `1.2` `)`
   >
   >   Renvoie 1
>
>* `round(` `1.5` `)`
   >
   >   Renvoie 2
>
>* `round(` `1.7` `)`
   >
   >   Renvoie 2
> 
>* `round(` `2` `)`
   >
   >   Renvoie 2


## [!UICONTROL sum ([tableau de valeurs]), sum(value1; value2; ...)]

Renvoie la somme des valeurs d’un tableau spécifié ou la somme des nombres renseignés individuellement.
