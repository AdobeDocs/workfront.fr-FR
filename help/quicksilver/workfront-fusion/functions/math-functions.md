---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Fonctions mathématiques dans Adobe Workfront Fusion
description: Les fonctions mathématiques suivantes sont disponibles dans le panneau de mappage d’Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 8a3c7a89-62b5-45e9-b857-8beedd0e5af4
source-git-commit: c325e16ba0cde4cd48fc3e40358a9ea9ed310659
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 100%

---

# Fonctions mathématiques dans [!DNL Adobe Workfront Fusion]

<!--Audited: 4/2024-->

## Conditions d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto"> 
 <col>  
 <col>  
 <tbody>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront] plan</td>  
   <td> <p>Tous</p> </td>  
  </tr>  
  <tr data-mc-conditions="">  
   <td role="rowheader">[!DNL Adobe Workfront] licence</td>  
   <td> <p>Nouvelle : [!UICONTROL Standard]</p><p>Ou</p><p>Actuelle : [!UICONTROL Work] ou niveau supérieur</p> </td>  
  </tr>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licence**</td>  
   <td> 
   <p>Actuelle : aucune exigence de licence [!DNL Workfront Fusion] requise.</p> 
   <p>Ou</p> 
   <p>Héritée : n’importe laquelle. </p> 
   </td>  
  </tr>  
  <tr>  
   <td role="rowheader">Produit</td>  
   <td> 
   <p>Nouveau :</p> <ul><li>Forfait [!DNL Workfront] [!UICONTROL Select] ou [!UICONTROL Prime] : votre entreprise doit acheter [!DNL Adobe Workfront Fusion].</li><li>Forfait [!DNL Workfront] [!UICONTROL Ultimate] : [!DNL Workfront Fusion] est inclus.</li></ul> 
   <p>Ou</p> 
   <p>Actuel : votre entreprise doit acheter [!DNL Adobe Workfront Fusion].</p> 
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
>**Exemples :**
>
>* `ceil(` `1.2` `)`
>
>   Renvoie 2
>
>* `ceil(` `4` `)`
>
>   Renvoie 4

## [!UICONTROL floor (nombre)]

Renvoie le plus grand entier inférieur ou égal à un nombre spécifié.

>[!INFO]
>
>**Exemples :**
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

## [!UICONTROL max ([tableau de valeurs]), max(valeur1;valeur2; ...)]

Renvoie le plus grand nombre d’un tableau spécifié ou le plus grand nombre parmi les nombres renseignés individuellement.

## [!UICONTROL min ([tableau de valeurs]), min(valeur1; valeur2; ...)]

Renvoie le plus petit nombre dans un tableau spécifié ou le plus petit nombre parmi les nombres saisis individuellement.

## [!UICONTROL round (nombre)]

Arrondit le nombre au nombre entier immédiatement inférieur.

>[!INFO]
>
>**Exemples :**
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

## [!UICONTROL sum ([tableau de valeurs]), sum(valeur1; valeur2; ...)]

Renvoie la somme des valeurs d’un tableau spécifié ou la somme des nombres saisis individuellement.

## [!UICONTROL parseNumber (nombre ; séparateur décimal)]

Analyse une chaîne avec un nombre et renvoie le nombre. Par exemple, parseNumber(1 756,456;,)

## [!UICONTROL formatNumber (nombre ; decimalPOINTS; [decimalSeparator]; [thousandsSeparator])]

Renvoie un nombre au format demandé. Par défaut, le point décimal est une virgule (,) et le séparateur des milliers est un point (.).

>[!INFO]
>
>**Exemple :**
>
>`formatNumber( 123456789 ; 3 ; , ; . )`
>
>Renvoie 123.456.789,000
