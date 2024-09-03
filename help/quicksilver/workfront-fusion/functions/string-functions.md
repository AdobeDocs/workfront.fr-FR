---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Fonctions de chaîne dans Adobe Workfront Fusion
description: Les fonctions de chaîne suivantes sont disponibles dans le panneau Mappage d’Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: c6676a87-2498-4de8-b877-7edc30aeabae
source-git-commit: 0b286e43ed77669329fbee25618394ee5641e428
workflow-type: tm+mt
source-wordcount: '696'
ht-degree: 100%

---

# Fonctions de chaîne dans [!DNL Adobe Workfront Fusion]

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

## [!UICONTROL length (text or buffer)]

Renvoie la longueur de la chaîne de texte (nombre de caractères) ou du buffer binaire (taille du buffer en octets).

>[!INFO]
>
>**Exemple :**
>
>`length( hello )`
>
>Renvoie : 5

## [!UICONTROL lower (text)]

Convertit en minuscules tous les caractères alphabétiques d’une chaîne de texte.

>[!INFO]
>
>**Exemple :**
>
>`lower( Hello )`
>
>Renvoie : hello.

## [!UICONTROL capitalize (text)]

Convertit le premier caractère d’une chaîne de texte en majuscules.

>[!INFO]
>
>**Exemple :**
>
>`capitalize( workfront )`
>
>Renvoie : [!DNL Workfront]

## [!UICONTROL startcase (text)]

Met en majuscule la première lettre de chaque mot et toutes les autres lettres en minuscules.

>[!INFO]
>
>**Exemple :**
>`startcase( hello WORLD )`
>
>Renvoie : [!UICONTROL Hello World].

## [!UICONTROL ascii (text; [remove diacritics])]

Supprime tous les caractères non ascii d’une chaîne de texte.

>[!INFO]
>
>**Exemples :**
>
>* `ascii(` `Wěošrčkřfžrýoáníté` `)`
>
>   Renvoie : [!DNL Workfront]
>
>* `ascii(` `ěščřž` `;` `true` `)`
>
>   Renvoie : [!UICONTROL escrz].



## [!UICONTROL replace (text;search string; replacement string)]

Remplace la chaîne de recherche par la nouvelle chaîne.

>[!INFO]
>
>**Exemple :**
>
>`replace( Hello World ; Hello ; Hi )`
>
>Renvoie : [!UICONTROL Hi World]

Des expressions régulières (incluses dans `/.../`) peuvent être utilisées comme chaîne de recherche avec une combinaison d’indicateurs ajoutés (comme `g`, `i`, `m`) :

>[!INFO]
>
>**Exemple :**
>
>![](assets/replace---1-350x31.png)
>
>Tous ces nombres X X X X sont remplacés par X

La chaîne de remplacement peut inclure les modèles de remplacement spéciaux suivants :

* `$&` insère la sous-chaîne correspondante.
* `$n` insère la nième chaîne de sous-matchs entre parenthèses lorsque n est un entier positif inférieur à 100. Il s’agit d’une indexation à partir de 1.

>[!INFO]
>
>**Exemples :**
>
>![](assets/variable-value-350x63.png)
>
>Renvoie : numéro de téléphone : `+420777111222`
>>
>![](assets/variable-value---2-350x55.png)
>
>Renvoie : numéro de téléphone : `+420777111222`

>[!CAUTION]
>
>N’utilisez pas de groupes de capture nommés tels que `/ is (?<number>\d+)/` dans l’argument de chaîne de remplacement. Cela entraîne une erreur.

Pour plus d’informations sur les expressions régulières, consultez la section [Analyseur de texte](../../workfront-fusion/apps-and-their-modules/text-parser.md).

## [!UICONTROL trim (texte)]

Supprime les espaces au début ou à la fin du texte.

## [!UICONTROL upper (texte)]

Convertit en majuscules tous les caractères alphabétiques d’une chaîne de texte.

>[!INFO]
>
>**Exemple :**
>
>`upper( Hello )`
>
>Renvoie : [!UICONTROL HELLO]

## [!UICONTROL substring (text; start;end)]

Renvoie une partie d’une chaîne de texte entre la position « début » et la position « fin ».

>[!INFO]
>
>**Exemples :**
>
>* `substring( Hello ; 0 ; 3)`
>
>   Renvoie : Hel
>
>* `substring( Hello ; 1 ; 3 )`
>
>   Renvoie : el

## [!DNL indexOf (string; value; [start])]

Renvoie la position de la première occurrence d’une valeur spécifiée dans une chaîne. Cette méthode renvoie « -1 » si la valeur recherchée n’est pas présente. La valeur de début indique où la recherche doit commencer dans la chaîne.

>[!INFO]
>
>**Exemples :**
>
>* `indexOf( Workfront ; o )`
>
>   Renvoie : 1
>
>* `indexOf( Workfront ; x )`
>
>   Renvoie : -1
>
>* `indexOf( Workfront ; o ; 3 )`
>
>   Renvoie : 6

## [!UICONTROL toBinary (valeur)]

Convertit n’importe quelle valeur en données binaires.

Vous pouvez également indiquer le codage comme second argument pour appliquer des conversions binaires de hex ou base64 aux données binaires.

>[!INFO]
>
>**Exemples :**
>
>* `toBinary( Workfront )`
>
>   Renvoie : 57 6f 72 6b 66 72 6f 6e 74
>
>* `toBinary( V29ya2Zyb250 ; base64 )`
>
>   Renvoie : 57 6f 72 6b 66 72 6f 6e 74

## [!UICONTROL toString (valeur)]

Convertit n’importe quelle valeur en chaîne.

## [!UICONTROL encodeURL (texte)]

Code les caractères spéciaux en texte à une adresse URL valide.

## [!UICONTROL decodeURL (texte)]

Décode les caractères spéciaux d’une URL en texte.

>[!INFO]
>
>**Exemple :**
>`decodeURL( Automate%20your%20workflow )`
>
>Renvoie : [!UICONTROL Automate your workflow] (automatiser votre workflow).

## [!UICONTROL escapeHTML (texte)]

Échappe toutes les balises de HTML dans le texte.

>[!INFO]
>
>**Exemple :**
>
>`escapeHTML( <b>Hello</b> )`
>
> Renvoie : `&lt;b&gt;Hello&lt;/b&gt;`

## [!UICONTROL escapeMarkdown(texte)]

Permet d’ignorer toutes les balises Markdown dans le texte.

>[!INFO]
>
>**Exemple :**
>
>`escapeMarkdown( # Header )`
>
>Renvoie : `&#35; Header`

## [!UICONTROL stripHTML (texte)]

Supprime toutes les balises de HTML du texte.

>[!INFO]
>
>**Exemple :**
>
>`stripHTML( <b>Hello</b> )`
>
>Renvoie : Hello

## contains (texte; chaîne de recherche)

Vérifie si le texte contient la chaîne de recherche.

>[!INFO]
>
>**Exemples :**
>
>* `contains( Hello World ; Hello )`
>
>   Renvoie : [!UICONTROL true]
>
>* `contains( Hello World ; Bye )`
>
>   Renvoie : [!UICONTROL false]

## [!UICONTROL split (texte; séparateur)]

Divise une chaîne en une séquence de chaînes de caractères en la séparant en sous-chaînes.

>[!INFO]
>
>**Exemple :**
>
>`split( John, George, Paul ; , )`

## [!UICONTROL md5 (text)]

Calcule le hachage md5 d’une chaîne.

>[!INFO]
>
>**Exemple :**
>
>`md5( Workfront )`
>
>Renvoie : `1448bbbeaa7a9b8091d426999f1f666b`

## [!UICONTROL sha1 (text; [encoding]; [key])]

Calcule le hachage sha1 d’une chaîne. Si l’argument key est spécifié, le hachage HMAC sha1 est renvoyé à la place. Codages pris en charge : « hex » (par défaut), « base64 » ou « latin1 ».

>[!INFO]
>
>**Exemple :**
>
>`sha1( workfront )`
>
>Renvoie : b2b30b8ae1f9e5b40fbb0696eaabdbfd8d0c087f

## [!UICONTROL sha256 (text; [encoding]; [key])]

Calcule le hachage sha256 d’une chaîne. Si l’argument key est spécifié, le hachage HMAC sha256 est renvoyé à la place. Codages pris en charge : « hex » (par défaut), « base64 » ou « latin1 ».>

>[!INFO]
>
>**Exemple :**
>
>`sha256( workfront )`
>
>Renvoie : ed3d7397eec7b94453035b67ba4468c83ee3bedeb57137f7371f2e0cf5e2bbc

## [!UICONTROL sha512 (texte; [codage de sortie]; [clé]; [codage de la clé])]

Calcule le hachage sha512 d’une chaîne. Si l’argument clé est spécifié, le hachage sha512 HMAC est renvoyé à la place.

Codages pris en charge :

* « [!UICONTROL hex] » (par défaut)
* « [!UICONTROL base64] »
* « [!UICONTROL latin1] »

Codages de clé pris en charge :

* « [!UICONTROL text] » (par défaut)
* « [!UICONTROL hex] »
* « [!UICONTROL base64] » ou « [!UICONTROL binary] »

Lors de l’utilisation du codage de clé [!UICONTROL binary], une clé doit être un buffer, pas une chaîne.

>[!INFO]
>
>**Exemple :**
>
>`sha512(workfront)`
>
>Renvoie : 789ae41b9456357e4f27c6a09956a767abbb8d80b206003ffdd1e94dbc687cd119b85e1e19db58bb44b234493af35fd431639c0345aadf2cf7ec26e9f4a7fb19

## [!UICONTROL base64 (texte)]

Transforme le texte en base64.

>[!INFO]
>
>**Exemple :**
>
>`base64( workfront )`
>
>Renvoie : d29ya2Zyb250==
