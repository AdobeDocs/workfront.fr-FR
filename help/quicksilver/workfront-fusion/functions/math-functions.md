---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Fonctions mathématiques dans Adobe Workfront Fusion
description: Les fonctions mathématiques suivantes sont disponibles dans le panneau Mappage de fusion Adobe Workfront .
author: Becky
feature: Workfront Fusion
exl-id: 8a3c7a89-62b5-45e9-b857-8beedd0e5af4
source-git-commit: c325e16ba0cde4cd48fc3e40358a9ea9ed310659
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 16%

---

# Fonctions mathématiques dans [!DNL Adobe Workfront Fusion]

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
   <td role="rowheader">[!DNL Adobe Workfront] license</td>  
   <td> <p>Nouveau : [!UICONTROL Standard]</p><p>Ou</p><p>Actuel : [!UICONTROL Travail] ou version ultérieure</p> </td>  
  </tr>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licence**</td>  
   <td> 
   <p>Actuel : Non [!DNL Workfront Fusion] conditions requises pour obtenir une licence.</p> 
   <p>Ou</p> 
   <p>Hérité : Tout </p> 
   </td>  
  </tr>  
  <tr>  
   <td role="rowheader">Produit</td>  
   <td> 
   <p>Nouveau :</p> <ul><li>[!UICONTROL Select] ou [!UICONTROL Prime] [!DNL Workfront] Plan : votre entreprise doit acheter [!DNL Adobe Workfront Fusion].</li><li>[!UICONTROL Ultimate] [!DNL Workfront] Plan : [!DNL Workfront Fusion] est inclus.</li></ul> 
   <p>Ou</p> 
   <p>Actuel : votre entreprise doit acheter [!DNL Adobe Workfront Fusion].</p> 
   </td>  
  </tr> 
 </tbody>  
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], consultez les [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL average ([tableau de valeurs]) average(value1; [value2], ...)]

Renvoie la valeur moyenne des valeurs numériques d’un tableau spécifique ou la valeur moyenne des valeurs numériques saisies unitairement.

## [!UICONTROL ceil (nombre)]

Renvoie le plus petit entier supérieur ou égal à un nombre spécifié.

>[!INFO]
>
>**Exemples :**
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
>**Exemples :**
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

## [!UICONTROL max ([tableau de valeurs]), max(value1;value2; ...)]

Renvoie le plus grand nombre d’un tableau spécifié ou le plus grand nombre parmi les nombres renseignés individuellement.

## [!UICONTROL min ([tableau de valeurs]), min(value1; value2; ...)]

Renvoie le plus petit nombre d’un tableau spécifié ou le plus petit nombre parmi les nombres saisis individuellement.

## [!UICONTROL round (nombre)]

Arrondit une valeur numérique à l’entier le plus proche.

>[!INFO]
>
>**Exemples :**
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

## [!UICONTROL sum ([tableau de valeurs]), sum(value1; value2;..)]

Renvoie la somme des valeurs d’un tableau spécifié ou la somme des nombres renseignés individuellement.

## [!UICONTROL parseNumber (nombre ; séparateur décimal)]

Analyse une chaîne avec un nombre et renvoie le nombre. Par exemple, parseNumber(1 756,456;,)

## [!UICONTROL formatNumber (number; decimalPOINTS; [decimalSeparator]; [millierSeparator])]

Renvoie un nombre au format demandé. Par défaut, la virgule est une virgule (,) et le séparateur des milliers est un point (.).

>[!INFO]
>
>**Exemple :**
>
>`formatNumber( 123456789 ; 3 ; , ; . )`
>
>Renvoie 123,456,789 000
