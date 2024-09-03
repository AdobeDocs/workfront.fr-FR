---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Fonctions de tableau dans Adobe Workfront Fusion
description: Les fonctions de tableau suivantes sont disponibles dans le panneau de mappage d’Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: bf065d00-5d84-47e1-8169-bf9e01e2429d
source-git-commit: 033a9f4aa1f191e5e3cabd0c0f232128fa6bce5d
workflow-type: tm+mt
source-wordcount: '665'
ht-degree: 100%

---

# Fonctions de tableau dans Adobe Workfront Fusion

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

## Fonctions

* [join](#join-array-separator)
* [length](#length-array)
* [keys](#keys-object)
* [slice](#slice-array-start-end)
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
* [deduplicate]

### [!UICONTROL join (array; separator)]

Concatène tous les éléments d’un tableau en une chaîne, en utilisant le séparateur spécifié entre chaque élément.

### [!UICONTROL length (array)]

Renvoie le nombre d’éléments d’un tableau.

### [!UICONTROL keys (object)]

Renvoie un tableau des propriétés d’un objet ou d’un tableau donné.

### [!UICONTROL slice (array; start; [end])]

Renvoie un nouveau tableau contenant uniquement les éléments sélectionnés.

### [!UICONTROL merge (array1; array2; ...)]

Fusionne un ou plusieurs tableaux en un seul.

### [!UICONTROL contains (array; value)]

Vérifie si un tableau contient la valeur.

### [!UICONTROL remove (array; value1; value2; ...)]

Supprime les valeurs spécifiées dans les paramètres d’un tableau. Cette fonction est efficace uniquement pour les tableaux primitifs de textes ou de nombres.

### [!UICONTROL add (array; value1; value2; ...)]

Ajoute les valeurs spécifiées dans les paramètres à un tableau et renvoie ce tableau.

### [!UICONTROL map (complex array; key;[key for filtering];[valeurs possibles pour le filtrage])]

Renvoie un tableau primitif contenant les valeurs d’un tableau complexe. Cette fonction permet de filtrer les valeurs. Utilisez des noms de variables bruts pour les clés.

>[!INFO]
>
>**Exemples :**
>
>* `map(Emails[];email)`
>
>  Renvoie un tableau primitif contenant les e-mails.
>
>* `map(Emails[];email;label;work;home)`
>
>  Renvoie un tableau primitif contenant les e-mails dont le libellé est « travail » ou « perso ».

Pour plus d’informations, voir [Mapper des informations d’un module à l’autre dans [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)

### shuffle

### [!UICONTROL sort (array; [order]; [key])]

Trie les valeurs d’un tableau. Les valeurs valides du paramètre `order` sont les suivantes :

* `asc`

  (par défaut) - ordre croissant : 1, 2, 3, ... pour le type Nombre. A, B, C, a, b, c, ... pour le type Texte.

* `desc`

  ordre décroissant : ..., 3, 2, 1 pour le type Nombre. ..., c, b, a, C, B, A pour le type Texte.

* `asc ci`

  ordre croissant insensible à la casse : A, a, B, b, C, c, ... pour le type Texte.

* `desc ci`

  ordre décroissant insensible à la casse : ..., C, c, B, b, A, a pour le type Texte.

Utilisez le paramètre `key` pour accéder aux propriétés des objets complexes.

Utilisez des noms de variables bruts pour les clés.

Pour accéder aux propriétés imbriquées, utilisez la notation avec point.

Le premier élément d’un tableau est l’index 1.

>[!INFO]
>
>**Exemples :**
>
>* `sort(Contacts[];name)`
>
>    Trie un tableau de contacts en fonction de la propriété « name » dans l’ordre croissant par défaut.
>
>* `sort(Contacts[];desc;name)`
>
>   Trie un tableau de contacts en fonction de la propriété « name » dans l’ordre décroissant.
>
>* `sort(Contacts[];asc ci;name)`
>
>    Trie un tableau de contacts en fonction de la propriété « name » dans l’ordre croissant insensible à la casse.
>
>* `sort(Emails[];sender.name)`
>
>    Trie un tableau d’e-mails en fonction de la propriété « sender.name ».

### [!UICONTROL reverse (array)]

Le premier élément du tableau devient le dernier élément, le deuxième devient l’avant-dernier, et ainsi de suite.

### [!UICONTROL flatten (array)]

Crée un nouveau tableau dans lequel sont concaténés tous les éléments des sous-tableaux, de manière récursive, jusqu’à la profondeur spécifiée.

### [!UICONTROL distinct (array; [key])]

Supprime les doublons dans un tableau. Utilisez l’argument « [!UICONTROL key] » pour accéder aux propriétés des objets complexes. Pour accéder aux propriétés imbriquées, utilisez la notation avec point. Le premier élément d’un tableau est l’index 1.

>[!INFO]
>
>**Exemple :** `distinct(Contacts[];name)`
>
>Supprime les doublons dans un tableau de contacts en comparant la propriété « nom ».

### toCollection

### toArray

Cette fonction convertit une collection en un tableau de paires clé-valeur.

>[!INFO]
>
>**Exemples :**
>
>Prenons l’exemple de la collection suivante :
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

### [!UICONTROL arrayDifference [array1, array2, mode]]

Renvoie la différence entre deux tableaux.

Saisissez l’une des valeurs suivantes pour le paramètre `mode`.

* `classic` : renvoie un nouveau tableau contenant tous les éléments de `array1` qui n’existent pas dans `array2`.

* `symmetric` : renvoie un tableau d’éléments qui ne sont pas communs aux deux tableaux.

  En d’autres termes, la fonction renvoie un tableau contenant tous les éléments de `array1` qui n’existent pas dans `array2`, et tous les éléments de `array2` qui n’existent pas dans `array1`.

  >[!INFO]
  >
  >**Exemples :**
  >
  >Les tableaux suivants :
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
  >    Retourne `[1,2]`
  >
  >* `arrayDifference [yourArray, myArray, classic]`
  >
  >    Renvoie `[6,7]`
  >
  >* `arrayDifference [myArray, yourArray, symmetric]`
  >
  >    Renvoie `[1,2,6,7]`

### deDuplicate

## Mots-clés

### emptyarray
