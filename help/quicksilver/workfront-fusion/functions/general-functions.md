---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Fonctions générales dans Adobe Workfront Fusion
description: La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement. Cet article est obsolète, mais contient un lien vers le nouvel article qui couvre cette fonctionnalité.
author: Becky
feature: Workfront Fusion
exl-id: 74bfda4e-5690-4b8c-ac58-20cf261f188d
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '455'
ht-degree: 59%

---

# Fonctions générales dans [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement.
>
>Les informations contenues dans cet article se trouvent désormais dans l’article :
>
>* [Fonctions générales](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/mapping-panel/functions/general-functions.html)
>
>Mettez à jour les signets.
>
>Cet article n’est plus mis à jour et sera supprimé prochainement.

## Conditions d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] formule*</td> 
   <td> <p>[!DNL Pro] ou une version ultérieure</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence [!UICONTROL Adobe Workfront Fusion]**</td> 
   <td>
   <p>Exigence de licence actuelle : aucune exigence de licence [!DNL Workfront Fusion].</p>
   <p>Ou</p>
   <p>Exigences de licence héritées : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
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

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], consultez [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL get (object or array; path)]

Renvoie le chemin d’accès à la valeur d’un objet ou d’un tableau. Pour accéder aux objets imbriqués, utilisez la notation par points. Le premier élément d’un tableau est l’index 1.

>[!INFO]
>
>**Exemples :**
>
>* `get( array ; 1 + 1 )`
>* `get( array ; 5.raw_name )`
>* `get( object ; raw_name )`
>* `get( object ; raw_name.sub_raw_name )`

## [!UICONTROL if (expression; value1; value2)]

Renvoie la `value1` si l’expression est considérée comme true ; sinon elle renvoie la `value2`.

Pour créer une instruction if qui renvoie une valeur uniquement si plusieurs expressions sont évaluées sur true, utilisez le mot-clé `and`.

Pour combiner des instructions `if`, utilisez les opérateurs `and` et `or` .

![opérateur and](/help/quicksilver/workfront-fusion/functions/assets/and-in-if-statement.png)

>[!INFO]
>
>**Exemples :**
>
>* `if( 1 = 1 ; A ; B )`
>
>    Renvoie A
>
>* `if( 1 = 2 ; A ; B )`
>
>   Renvoie B
>
>* `if( 1 = 2 and 1 = 2 ; A ; B )`
>
>    Renvoie B
>   

## [!UICONTROL ifempty (value1; value2)]

Renvoie la `value1` si cette valeur n’est pas vide ; sinon elle renvoie la `value2`.

>[!INFO]
>
>**Exemples :**
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

## [!UICONTROL switch (expression; value1; result1; [value2; result2; ...]; [else])]

Évalue une valeur (appelée expression) par rapport à une liste de valeurs ; renvoie le résultat correspondant à la première valeur correspondante. Pour inclure une valeur `else`, ajoutez-la après l’expression ou la valeur finale.

>[!INFO]
>
>**Exemples :**
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
>   Renvoie 4
>   
>   Dans cette fonction, 4 est la valeur à renvoyer si aucune expression ne s’applique (la valeur `else`).

## [!UICONTROL omit(object; key1; [key2; ...])]

Omet les clés données de l’objet et renvoie le reste.

>[!INFO]
>
>**Exemple :**
>
>`omit(` User `;` password `)`
>
>Renvoie une collection des informations de l’utilisateur ou de l’utilisatrice, à l’exclusion du mot de passe.

## [!UICONTROL pick(object; key1; [key2; ...])]

Sélectionne uniquement les clés données de l’objet.

>[!INFO]
>
>**Exemple :**
>
>`pick(` User `;` password `;` email `)`
>
>Renvoie une collection contenant uniquement le mot de passe et l’adresse e-mail de l’utilisateur ou de l’utilisatrice.

## mergeCollections(collection1 ; collection2)

Fusionne deux collections en combinant leurs paires clé-valeur. Si les deux collections contiennent la même clé, la valeur de la deuxième collection remplace celle de la première collection.

