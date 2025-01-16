---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Modules JSON
description: La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement. Cet article est obsolète, mais contient un lien vers le nouvel article qui couvre cette fonctionnalité.
author: Becky
feature: Workfront Fusion
exl-id: 60540608-9d2e-4e10-9fb2-5388dda64784
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '1256'
ht-degree: 92%

---

# Modules [!UICONTROL JSON]

>[!IMPORTANT]
>
>La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement.
>
>Les informations contenues dans cet article se trouvent désormais dans l’article :
>
>* [Modules JSON](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/tools-and-transformers/json-modules.html)
>
>Mettez à jour les signets.
>
>Cet article n’est plus mis à jour et sera supprimé prochainement.

L’application [!DNL Adobe Workfront Fusion] [!UICONTROL JSON] fournit des modules pour traiter les données au format JSON afin qu’[!DNL Adobe Workfront Fusion] puisse continuer à travailler avec le contenu des données ou créer un nouveau contenu JSON.

## Conditions d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] formule*</td>
  <td> <p>[!UICONTROL Pro] ou version supérieure</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licence**</td> 
   <td>
   <p>Exigences de licence actuelles : aucune exigence de licence [!DNL Workfront Fusion] requise.</p>
   <p>Ou</p>
   <p>Exigences en matière de licences héritées : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration], [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Exigences actuelles du produit : si vous disposez du plan de [!DNL Adobe Workfront] [!UICONTROL Select] ou [!UICONTROL Prime], votre entreprise doit acheter du [!DNL Adobe Workfront Fusion] et [!DNL Adobe Workfront] utiliser les fonctionnalités décrites dans cet article. [!DNL Workfront Fusion] est inclus dans la formule [!DNL Workfront] [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Exigences liées aux produits hérités : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi qu’[!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez votre équipe d’administration [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], voir Licences [[!DNL Adobe Workfront Fusion] ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Analyse JSON

* [Structure des données](#data-structure)
* [Collection ou tableau](#collection-vs-array)

### Structures des données

La structure des données décrit la manière dont les données JSON sont organisées et permet de mapper des éléments JSON individuels avec d’autres modules de votre scénario. Si vous ne fournissez pas la structure des données, vous pouvez exécuter manuellement le module et [!DNL Workfront Fusion] construira la structure à partir du JSON fourni :

1. Ajoutez le module [!UICONTROL Analyse JSON] à un scénario.
1. Dans le champ **[!UICONTROL Chaîne de caractères JSON]**, saisissez le JSON à partir duquel vous souhaitez créer une structure des données.
1. Ne connectez pas encore d’autres modules au module [!UICONTROL Analyse JSON]. Comme [!DNL Workfront Fusion] ne connaît pas encore la structure des données JSON, il n’est pas encore possible de mapper les données du module [!UICONTROL Analyse JSON] à d’autres modules de votre scénario.
1. Exécutez manuellement le scénario. Cela permet au module [!UICONTROL Analyse JSON] d’identifier la structure du JSON à partir du JSON que vous avez fourni.
1. Vous pouvez maintenant connecter les modules suivants. Les éléments du module Analyse JSON sont maintenant disponibles pour le mappage.

Pour plus d’informations, voir [Structures des données dans [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-structures.md).

### Collection ou tableau

Si le champ Chaîne de caractères JSON contient une collection `{ ... }`, la sortie est un paquet unique contenant les éléments de la collection.

>[!INFO]
>
>**Exemple :**
>
>```
>{
>       "name" : "Peter",
>
>    
   "ID" : 1
>}
>```
>
>![](assets/json-collection.png)

Si le champ Chaîne de caractères JSON contient un tableau `[ ... ]`, la sortie est une série de paquets. Chaque paquet contient un élément du tableau.

>[!INFO]
>
>**Exemple :**
>
>```
>[
>   {
>       "name" : "Peter",
>       "ID" : 1
>   },
>
>  
 {
>       "name" : "Mike",
>       "ID" : 2
>   }
>]
>```
>
>![](assets/json-array.png)

## Modules [!UICONTROL JSON] et leurs champs

Lorsque vous configurez les modules [!DNL JSON], [!DNL Workfront Fusion] affiche les champs énumérés ci-dessous. En plus de ces champs, d’autres champs JSON peuvent s’afficher, en fonction de facteurs tels que votre niveau d’accès à l’application ou au service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton « Mapper » apparaît au-dessus d’un champ ou d’une fonction, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, voir [Mapper des informations d’un module à l’autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Convertir JSON en XML](#convert-json-to-xml)
* [Analyser la chaîne JSON](#parse-json)
* [Créer une chaîne JSON](#create-json)
* [Transformer la chaîne JSON](#transform-json)

### Agrégateurs

#### [!UICONTROL Agréger en chaîne JSON]

Ce module agrégateur regroupe les résultats d’un module précédent en chaîne JSON.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source module] </td> 
   <td> <p>Sélectionnez le module qui produit les données que vous souhaitez agréger en chaîne JSON.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data structure]</td> 
   <td> <p>Sélectionnez la structure de données que vous souhaitez utiliser pour créer la chaîne JSON. La structure des données détermine les autres champs disponibles dans ce module. Pour plus d’informations, voir <a href="#data-structure" class="MCXref xref">Structure des données</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Indentation]</td> 
   <td> <p> Indiquez si vous souhaitez indenter la chaîne JSON en utilisant des tabulations, deux espaces ou quatre espaces.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Group by]</td> 
   <td>Définissez une expression selon laquelle vous souhaitez regrouper la sortie agrégée. Cette expression peut contenir un ou plusieurs éléments mappés. Les données agrégées sont ensuite séparées en groupes à l’aide de la valeur de cette expression. Chaque groupe se présente sous la forme d’un lot distinct avec une clé (l’expression évaluée) et une valeur (le texte agrégé). Vous pouvez utiliser la clé comme filtre dans les modules suivants.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Stop processing after an empty aggregation]</td> 
   <td>Activez cette option pour arrêter le scénario lorsqu’il n’y a aucun résultat.</td> 
  </tr> 
 </tbody> 
</table>

### Transformateurs

* [Convertir JSON en XML](#convert-json-to-xml)
* [Créer une chaîne JSON](#create-json)
* [Analyser la chaîne JSON](#parse-json)
* [Transformer la chaîne JSON](#transform-json)

#### [!UICONTROL Convertir la chaîne JSON en XML]

Ce module d’action convertit une chaîne JSON en XML.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL JSON string] </td> 
   <td> <p>Saisissez ou mappez le code JSON que vous souhaitez convertir en XML.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Créer un code JSON]

Ce module d’action crée du code JSON à partir d’une structure de données.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">Structures des données</td> 
   <td> <p>Sélectionnez la structure de données que vous souhaitez utiliser pour créer la chaîne JSON. Pour plus d’informations, voir <a href="#data-structure" class="MCXref xref">Structure des données</a> dans cet article.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Analyser le code JSON]

Ce module d’action analyse une chaîne JSON dans une structure de données, ce qui vous permet d’accéder aux données contenues dans la chaîne JSON.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data structure]</td> 
   <td> <p>Sélectionnez la structure de données que vous souhaitez utiliser pour créer la chaîne JSON. Pour plus d’informations, voir <a href="#data-structure" class="MCXref xref">Structure des données</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL JSON string] </td> 
   <td> <p>Saisissez ou mappez le code JSON que vous souhaitez analyser.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Transformer une chaîne JSON]

Ce module d’action transforme un objet en une chaîne JSON.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Object]</td> 
   <td> <p>Saisissez ou mappez l’objet que vous souhaitez transformer en chaîne JSON.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Transformation des enregistrements de données en chaîne JSON

>[!INFO]
>
>**Exemple :** l’exemple suivant montre comment transformer des enregistrements de données de [!DNL Google Sheets] au format JSON :
>
>1. Placez le module [!DNL Google Sheets] > [!UICONTROL Sélectionner des lignes] dans votre scénario pour récupérer les données. Configurez le module pour récupérer les lignes de votre feuille de calcul [!DNL Google]. Définissez le **[!UICONTROL Nombre maximal de lignes renvoyées]** sur un petit nombre, mais plus grand que 1 à des fins de test (par exemple, trois). Exécutez le module [!DNL Google Sheets] en cliquant dessus avec le bouton droit et en choisissant « **[!UICONTROL Exécuter ce module uniquement]** ». Vérifiez la sortie du module.
>
1. Connectez-vous au module [!UICONTROL Agrégateur de tableau] après le module [!DNL Google Sheets]. Dans la configuration du module, choisissez le module [!DNL Google Sheets] dans le champ **[!UICONTROL Nœud source]**. Laissez les autres champs tels quels pour le moment.
>
1. Connectez [!UICONTROL JSON] > module [!UICONTROL Créer JSON] après le module [!UICONTROL Agrégateur de tableaux]. La configuration du module nécessite une structure de données qui décrit le format JSON. Cliquez sur **[!UICONTROL Ajouter]** pour ouvrir la configuration de la structure de données. La manière la plus simple de créer cette structure de données est de la générer automatiquement à partir d’un exemple JSON. Cliquez sur **[!UICONTROL Générateur]** et collez votre exemple JSON dans le champ **[!UICONTROL Données d’exemple]** :
>
**Exemple :**
>
```
{

"books": [

{

"id": "ID",

"title": "Title",

"author": "Author"

}

]

}
```
>
1. Cliquer sur **[!UICONTROL Enregistrer]**. Le champ [!UICONTROL Spécification] de la structure de données contient maintenant la structure générée.
1. Attribuez à votre structure de données un nom plus spécifique et cliquez sur **[!UICONTROL Enregistrer]**. Un champ correspondant à l’attribut de tableau racine apparaît comme champ mappable dans la configuration du module JSON.
>
1. Cliquez sur le bouton **[!UICONTROL Mapper]** en regard du champ et mappez-y l’élément `Array[]` de la sortie de l’Agrégateur de tableaux.
>
1. Cliquez sur **[!UICONTROL OK]** pour fermer la configuration du module [!UICONTROL JSON].
>
1. Ouvrez la configuration du module [!UICONTROL Agrégateur de tableau]. Modifiez la **[!UICONTROL structure cible]** de [!UICONTROL Personnalisée] en champ du module [!UICONTROL JSON] correspondant à l’attribut tableau racine. Mappez les éléments du module [!DNL Google Sheets] aux champs appropriés.
>
1. Cliquez sur **[!UICONTROL OK]** pour fermer la configuration du module [!UICONTROL Agrégateur de tableau].
>
1. Exécutez le scénario.
>
Le module [!UICONTROL JSON] produit le bon format JSON.
>
1. Ouvrez la configuration du module [!DNL Google Sheets] et augmentez le [!UICONTROL nombre maximal de lignes renvoyées] pour que ce nombre soit supérieur au nombre de lignes de votre feuille de calcul afin de traiter toutes les données.

## Dépannage

### Impossible de mapper les données du module [!UICONTROL Analyser JSON].

Assurez-vous que le contenu JSON est correctement mappé dans le module [!UICONTROL Analyser JSON] et que la structure des données est correctement définie. Pour plus d’informations, voir [Transformer des enregistrements de données en JSON](#transforming-data-records-to-json) dans cet article.

### Le module échoue lors de l’utilisation d’instructions conditionnelles dans JSON.

Lorsque vous utilisez des instructions conditionnelles telles que `if` dans JSON, mettez les guillemets à l’extérieur de l’instruction conditionnelle.

>[!INFO]
>
**Exemple :**
>
![](assets/quotes-in-json-350x120.png)
