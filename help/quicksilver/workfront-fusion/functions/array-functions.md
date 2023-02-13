---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Fonctions de tableau dans Adobe Workfront Fusion
description: Les fonctions de tableau suivantes sont disponibles dans le panneau Mappage de fusion Adobe Workfront .
author: Becky
feature: Workfront Fusion
exl-id: bf065d00-5d84-47e1-8169-bf9e01e2429d
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '603'
ht-degree: 0%

---

# Fonctions de tableau dans Adobe Workfront Fusion

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

## [!UICONTROL add (tableau); value1; value2; ...)]

Ajoute des valeurs spécifiées dans les paramètres à un tableau et renvoie ce tableau.

## [!UICONTROL contains (tableau) ; value)]

Vérifie si un tableau contient la valeur .

## [!UICONTROL distinct (tableau) ; [key])]

Supprime les doublons dans un tableau. Utilisez le[!UICONTROL key]&quot; pour accéder aux propriétés dans des objets complexes. Pour accéder aux propriétés imbriquées, utilisez la notation par points. Le premier élément d’un tableau est index 1.

>[!INFO]
>
>**Exemple :** `distinct(Contacts[];name)`
>
>Supprime les doublons dans un tableau de contacts en comparant la propriété &quot;name&quot;.

## [!UICONTROL aplatissement (tableau)]

Crée un tableau avec tous les éléments de sous-tableau concaténés, de manière récursive, jusqu’à la profondeur spécifiée.


## [!UICONTROL join (tableau); separator)]

Concatène tous les éléments d’un tableau dans une chaîne, à l’aide du séparateur spécifié entre chaque élément.

## [!UICONTROL keys (objet)]

Renvoie un tableau des propriétés d’un objet ou d’un tableau donné.

## [!UICONTROL length (tableau)]

Renvoie le nombre d’éléments d’un tableau.

## [!UICONTROL map (tableau complexe); key;[clé de filtrage];[valeurs possibles pour le filtrage])]

Renvoie un tableau primitif contenant les valeurs d’un tableau complexe. Cette fonction permet de filtrer les valeurs. Utilisez des noms de variable bruts pour les clés.

>[!INFO]
>
>**Exemples:**
>
>* `map(Emails[];email)`
  >
>  Renvoie un tableau primitif avec des emails
>
>* `map(Emails[];email;label;work;home)`
  >
>  Renvoie un tableau primitif avec des emails dont le libellé est égal au travail ou à la maison

Pour plus d’informations, voir [Mappage des informations d’un module à un autre dans [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)


## [!UICONTROL merge (tableau1); array2; ...)]

Fusionne un ou plusieurs tableaux en un seul tableau.

## [!UICONTROL remove (tableau) ; value1; value2; ...)]

Supprime les valeurs spécifiées dans les paramètres d’un tableau. Cette fonction n’est efficace que sur des tableaux primitifs de texte ou de nombres.

## [!UICONTROL reverse (tableau)]

Le premier élément du tableau devient le dernier élément, le second devient le prochain au dernier, etc.

## [!UICONTROL slice (tableau); start; [end])]

Renvoie un nouveau tableau contenant uniquement les éléments sélectionnés.

## [!UICONTROL sort (tableau); [order]; [key])]

Trie les valeurs d’un tableau. Les valeurs valides de la variable `order` sont les suivants :

* `asc`

   (par défaut) - Ordre croissant : 1, 2, 3, ... pour le type Nombre. A, B, C, a, b, c, etc. pour le type Texte

* `desc`

   ordre décroissant : ..., 3, 2, 1 pour le type Nombre. ..., c, b, a, C, B, A pour le type Texte.

* `asc ci`

   ordre croissant non sensible à la casse : A, a, B, b, C, c, ... pour le type Texte.

* `desc ci`

   ordre décroissant non sensible à la casse : ..., C, c, B, b, A, a pour le type Texte.

Utilisez la variable `key` pour accéder aux propriétés dans des objets complexes.

Utilisez des noms de variable bruts pour les clés.

Pour accéder aux propriétés imbriquées, utilisez la notation par points.

Le premier élément d’un tableau est index 1.

>[!INFO]
>
>**Exemples:**
>
>* `sort(Contacts[];name)`
   >
   >    Trie un tableau de contacts par propriété &quot;name&quot; dans l’ordre croissant par défaut.
>
>* `sort(Contacts[];desc;name)`
   >
   >   Trie un tableau de contacts par propriété &quot;name&quot; dans l’ordre décroissant.
>
>* `sort(Contacts[];asc ci;name)`
   >
   >    Trie un tableau de contacts par propriété &quot;name&quot; dans l’ordre croissant sans distinction de la casse.
>
>* `sort(Emails[];sender.name)`
   >
   >    Trie un tableau d’emails par la propriété &quot;sender.name&quot;


## [!UICONTROL arrayDifference [tableau1, tableau2, mode]]

Renvoie la différence entre deux tableaux.

Saisissez l’une des valeurs suivantes pour la variable `mode` .

* `classic`: Renvoie un nouveau tableau qui contient tous les éléments de `array1` qui n’existent pas dans `array2`.

* `symmetric`: Renvoie un tableau d’éléments qui ne sont pas communs aux deux tableaux.

   En d’autres termes, la fonction renvoie un tableau contenant tous les éléments de la variable `array1` qui n’existent pas dans `array2`et tous les éléments de la variable `array2` qui n’existent pas dans `array1`.

   >[!INFO]
   >
   >**Exemples:**
   >
   >Compte tenu des tableaux suivants :
   >
   >
   ```
   >myArray = [1,2,3,4,5]
   >```
   >
   >
   ```
   >yourArray = [3,4,5,6,7]
   >```
   >
   >* `arrayDifference [myArray, yourArray, classic]`
      >
      >    Renvoie `[1,2]`
   >
   >* `arrayDifference [yourArray, myArray, classic]`
      >
      >    Renvoie `[6,7]`
   >
   >* `arrayDifference [myArray, yourArray, symmetric]`
      >
      >    Renvoie `[1,2,6,7]`

