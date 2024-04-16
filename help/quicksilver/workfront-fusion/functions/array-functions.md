---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Fonctions de tableau dans Adobe Workfront Fusion
description: Les fonctions de tableau suivantes sont disponibles dans le panneau Mappage de fusion Adobe Workfront .
author: Becky
feature: Workfront Fusion
exl-id: bf065d00-5d84-47e1-8169-bf9e01e2429d
source-git-commit: 033a9f4aa1f191e5e3cabd0c0f232128fa6bce5d
workflow-type: tm+mt
source-wordcount: '665'
ht-degree: 8%

---

# Fonctions de tableau dans Adobe Workfront Fusion

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

## Fonctions

* [join](#join-array-separator)
* [length](#length-array)
* [keys](#keys-object)
* [tranche](#slice-array-start-end)
* [merge](#merge-array1-array2)
* [contient](#contains-array-value)
* [remove](#remove-array-value1-value2)
* [add](#add-array-value1-value2)
* [map](#map-complex-array-keykey-for-filteringpossible-values-for-filtering)
* [shuffle]
* [sort](#sort-array-order-key)
* [reverse](#reverse-array)
* [flatten](#flatten-array)
* [distinct](#distinct-array-key)
* [toCollection]
* [toArray](#toarray)
* [arrayDifference](#arraydifference-array1-array2-mode)
* [dédupliquer]

### [!UICONTROL join (tableau ; séparateur)]

Concatène tous les éléments d’un tableau dans une chaîne, à l’aide du séparateur spécifié entre chaque élément.

### [!UICONTROL length (tableau)]

Renvoie le nombre d’éléments d’un tableau.

### [!UICONTROL keys (objet)]

Renvoie un tableau des propriétés d’un objet ou d’un tableau donné.

### [!UICONTROL slice (tableau ; démarrage) ; [end])]

Renvoie un nouveau tableau contenant uniquement les éléments sélectionnés.

### [!UICONTROL merge (tableau1 ; tableau2 ; ...)]

Fusionne un ou plusieurs tableaux en un seul tableau.

### [!UICONTROL contains (tableau ; valeur)]

Vérifie si un tableau contient la valeur .

### [!UICONTROL remove (tableau ; valeur1 ; valeur2 ; ...)]

Supprime les valeurs spécifiées dans les paramètres d’un tableau. Cette fonction n’est efficace que sur des tableaux primitifs de texte ou de nombres.

### [!UICONTROL add (tableau ; valeur1 ; valeur2 ; ...)]

Ajoute des valeurs spécifiées dans les paramètres à un tableau et renvoie ce tableau.

### [!UICONTROL map (tableau complexe; clé;[clé de filtrage];[valeurs possibles pour le filtrage])]

Renvoie un tableau primitif contenant les valeurs d’un tableau complexe. Cette fonction permet de filtrer les valeurs. Utilisez des noms de variable bruts pour les clés.

>[!INFO]
>
>**Exemples :**
>
>* `map(Emails[];email)`
>
>  Renvoie un tableau primitif avec des emails
>
>* `map(Emails[];email;label;work;home)`
>
>  Renvoie un tableau primitif avec des emails dont le libellé est égal au travail ou à la maison

Pour plus d’informations, voir [Mappage des informations d’un module à un autre dans [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)

### shuffle

### [!UICONTROL sort (tableau); [order]; [key])]

Trie les valeurs d’un tableau. Les valeurs valides de la variable `order` sont les suivants :

* `asc`

  (par défaut) - ordre croissant : 1, 2, 3, ... pour le type Nombre. A, B, C, a, b, c, etc. pour le type Texte

* `desc`

  ordre décroissant : ..., 3, 2, 1 pour le type Nombre. ..., c, b, a, C, B, A pour le type Texte.

* `asc ci`

  ordre croissant insensible à la casse : A, a, B, b, C, c, ... pour le type Texte.

* `desc ci`

  ordre décroissant non sensible à la casse : ..., C, c, B, b, A, a pour le type Texte.

Utilisez la variable `key` pour accéder aux propriétés dans des objets complexes.

Utilisez des noms de variable bruts pour les clés.

Pour accéder aux propriétés imbriquées, utilisez la notation par points.

Le premier élément d’un tableau est index 1.

>[!INFO]
>
>**Exemples :**
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

### [!UICONTROL reverse (tableau)]

Le premier élément du tableau devient le dernier élément, le second devient le prochain au dernier, etc.

### [!UICONTROL aplatissement (tableau)]

Crée un tableau avec tous les éléments de sous-tableau concaténés, de manière récursive, jusqu’à la profondeur spécifiée.

### [!UICONTROL distinct (tableau) ; [key])]

Supprime les doublons dans un tableau. Utilisez le[!UICONTROL key]&quot; pour accéder aux propriétés dans des objets complexes. Pour accéder aux propriétés imbriquées, utilisez la notation par points. Le premier élément d’un tableau est index 1.

>[!INFO]
>
>**Exemple :** `distinct(Contacts[];name)`
>
>Supprime les doublons dans un tableau de contacts en comparant la propriété &quot;name&quot;

### toCollection

### toArray

Cette fonction convertit une collection en un tableau de paires clé-valeur.

>[!INFO]
>
>**Exemples :**
>
>Compte tenu de la collection
>
>`{ key1: "value1", key2: "value2:}`
>
>La fonction
>
>`toArray({ key1: "value1", key2: "value2:})`
>
>Renvoie le tableau de paires clé-valeur
>
>`[{ key1: "value1"}, { key2: "value2"}]`

### [!UICONTROL arrayDifference [tableau1, tableau2, mode]]

Renvoie la différence entre deux tableaux.

Saisissez l’une des valeurs suivantes pour la variable `mode` .

* `classic`: renvoie un nouveau tableau contenant tous les éléments de `array1` qui n’existent pas dans `array2`.

* `symmetric`: renvoie un tableau d’éléments qui ne sont pas communs aux deux tableaux.

  En d’autres termes, la fonction renvoie un tableau contenant tous les éléments de la variable `array1` qui n’existent pas dans `array2`et tous les éléments de la variable `array2` qui n’existent pas dans `array1`.

  >[!INFO]
  >
  >**Exemples :**
  >
  >Compte tenu des tableaux suivants :
  >
  >```
  >myArray = [1,2,3,4,5]
  >```
  >
  >```
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

### dédupliquer

## Mots-clés

### emptyarray
