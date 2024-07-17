---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Modules JSON
description: L’application JSON Adobe Workfront Fusion fournit des modules pour traiter les données au format JSON afin qu’Adobe Workfront Fusion puisse continuer à utiliser le contenu des données ou créer du contenu JSON.
author: Becky
feature: Workfront Fusion
exl-id: 60540608-9d2e-4e10-9fb2-5388dda64784
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1205'
ht-degree: 16%

---

# Modules [!UICONTROL JSON]

L’application [!DNL Adobe Workfront Fusion] [!UICONTROL JSON] fournit des modules pour traiter les données au format JSON afin que [!DNL Adobe Workfront Fusion] puisse continuer à travailler avec le contenu des données ou créer du contenu JSON.

## Conditions d’accès

Pour utiliser les fonctionnalités décrites dans cet article, vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] forfait*</td>
  <td> <p>[!UICONTROL Pro] ou un forfait supérieur</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licence**</td> 
   <td>
   <p>Exigences de licence actuelle : aucune exigence de licence [!DNL Workfront Fusion]</p>
   <p>Ou</p>
   <p>Exigences de licence héritée : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration], [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Exigences du produit actuel : si vous disposez du forfait [!DNL Adobe Workfront] [!UICONTROL Select] ou [!UICONTROL Prime], votre entreprise doit acheter [!DNL Adobe Workfront Fusion] et [!DNL Adobe Workfront] pour utiliser les fonctionnalités décrites dans cet article. [!DNL Workfront Fusion] est inclus dans le forfait [!DNL Workfront] [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Exigences du produit hérité : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] et [!DNL Adobe Workfront] pour utiliser les fonctionnalités décrites dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez vote administrateur ou administratrice [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], consultez les [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Parse JSON

* [Structure de données](#data-structure)
* [Collection vs. Array](#collection-vs-array)

### Structure des données

La structure de données décrit l’organisation des données JSON et permet le mappage de différents éléments JSON à d’autres modules dans votre scénario. Si vous ne fournissez pas la structure de données, vous pouvez exécuter manuellement le module et [!DNL Workfront Fusion] construira la structure à partir du JSON fourni :

1. Ajoutez le module [!UICONTROL Parse JSON] à un scénario.
1. Dans le champ **[!UICONTROL JSON String]**, saisissez le JSON à partir duquel vous souhaitez créer une structure de données.
1. Ne connectez pas encore d’autres modules au module [!UICONTROL Parse JSON]. Étant donné que [!DNL Workfront Fusion] ne connaît pas encore la structure des données JSON, il n’est pas encore possible de mapper les données du module [!UICONTROL Parse JSON] à d’autres modules de votre scénario.
1. Exécutez manuellement le scénario. Cela permet au module [!UICONTROL Parse JSON] d’identifier la structure JSON à partir du JSON que vous avez fourni.
1. Vous pouvez maintenant connecter les modules suivants. Les éléments du module JSON d’analyse sont désormais disponibles pour le mappage.

Pour plus d’informations, voir [Structures de données dans [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-structures.md).

### Collection vs. Array

Si le champ de chaîne JSON contient une collection `{ ... }`, la sortie est un seul lot contenant les éléments de la collection.

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

Si le champ de chaîne JSON contient un tableau `[ ... ]`, la sortie est une série de lots. chaque lot contient un élément du tableau .

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

Lorsque vous configurez des modules [!DNL JSON], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. En outre, d’autres champs JSON peuvent s’afficher, en fonction de facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, consultez [Mapper les informations d’un module à un autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Agrégat vers JSON](#aggregate-to-json)
* [Convertir JSON en XML](#convert-json-to-xml)
* [Parse JSON](#parse-json)
* [Créer JSON](#create-json)
* [Transformer JSON](#transform-json)

### [!UICONTROL Agrégat vers JSON]

Ce module d’agrégation regroupe la sortie d’un module précédent dans JSON.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">Module [!UICONTROL Source] </td> 
   <td> <p>Sélectionnez le module qui génère les données que vous souhaitez agréger au format JSON.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Structure de données]</td> 
   <td> <p>Sélectionnez la structure de données à utiliser pour créer JSON. La structure de données détermine les autres champs disponibles dans ce module. Pour plus d’informations, voir <a href="#data-structure" class="MCXref xref">Structure de données</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Indentation]</td> 
   <td> <p> Indiquez si vous souhaitez mettre le fichier JSON en retrait à l’aide d’onglets, de deux espaces ou de quatre espaces.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Groupe [!UICONTROL par]</td> 
   <td>Définissez une expression selon laquelle vous souhaitez regrouper la sortie agrégée. Cette expression peut contenir un ou plusieurs éléments mappés. Les données agrégées sont ensuite séparées en groupes à l’aide de la valeur de cette expression. Chaque groupe génère un lot distinct avec une clé (l’expression évaluée) et une valeur (le texte agrégé). Vous pouvez utiliser la clé comme filtre dans les modules suivants.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Arrêter le traitement après une agrégation vide]</td> 
   <td>Activez cette option pour arrêter le scénario lorsqu’il n’y a aucun résultat.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Convertir JSON en XML]

Ce module d’action convertit une chaîne JSON en XML.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Chaîne JSON] </td> 
   <td> <p>Saisissez ou mappez le fichier JSON que vous souhaitez convertir en XML.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Parse JSON]

Ce module d’action analyse une chaîne JSON dans une structure de données, ce qui vous permet d’accéder aux données contenues dans la chaîne JSON.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Structure de données]</td> 
   <td> <p>Sélectionnez la structure de données à utiliser pour créer JSON. Pour plus d’informations, voir <a href="#data-structure" class="MCXref xref">Structure de données</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Chaîne JSON] </td> 
   <td> <p>Saisissez ou mappez le fichier JSON que vous souhaitez analyser.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Créer JSON]

Ce module d’action crée le fichier JSON à partir d’une structure de données.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">Structure des données</td> 
   <td> <p>Sélectionnez la structure de données à utiliser pour créer JSON. Pour plus d’informations, voir <a href="#data-structure" class="MCXref xref">Structure de données</a> dans cet article.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Transformer JSON]

Ce module d’action transforme un objet en chaîne json.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Object]</td> 
   <td> <p>Saisissez ou mappez l’objet que vous souhaitez transformer en JSON.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Transformation des enregistrements de données en JSON

>[!INFO]
>
>**Exemple :** L’exemple suivant montre comment transformer des enregistrements de données de [!DNL Google Sheets] au format JSON :
>
>1. Placez le module [!DNL Google Sheets] > [!UICONTROL Sélectionner les lignes] dans votre scénario pour récupérer les données. Configurez le module pour récupérer les lignes de votre feuille de calcul [!DNL Google]. Définissez la &#x200B;**[!UICONTROL Nombre maximal de lignes renvoyées]** sur un petit nombre, mais plus grand qu’un à des fins de test (par exemple, trois). Exécutez le module [!DNL Google Sheets] en cliquant dessus avec le bouton droit de la souris et en choisissant &quot;**[!UICONTROL Exécuter ce module uniquement]**&quot;. Vérifiez la sortie du module.
>
1. Connectez le module [!UICONTROL Agrégateur de tableau] après le module [!DNL Google Sheets]. Dans la configuration du module, choisissez le module [!DNL Google Sheets] dans le champ **[!UICONTROL Noeud Source]** . Laissez les autres champs tels quels pour le moment.
>
1. Connectez-vous au module [!UICONTROL JSON] > [!UICONTROL Créer JSON] après le module [!UICONTROL Agrégateur de tableau]. La configuration du module nécessite une structure de données qui décrit le format JSON. Cliquez sur **[!UICONTROL Ajouter]** pour ouvrir la configuration de la structure de données. La méthode la plus simple pour créer cette structure de données consiste à la générer automatiquement à partir d’un exemple JSON. Cliquez sur **[!UICONTROL Generator]** et collez votre exemple JSON dans le champ **[!UICONTROL Sample data]** :
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
1. Cliquer sur **[!UICONTROL Enregistrer]**. Le champ [!UICONTROL Spécification] de la structure de données contient désormais la structure générée.
1. Remplacez le nom de votre structure de données par quelque chose de plus spécifique et cliquez sur **[!UICONTROL Enregistrer]**. Un champ correspondant à l’attribut de tableau racine apparaît comme champ mappable dans la configuration du module JSON.
>
1. Cliquez sur le bouton **[!UICONTROL Map]** en regard du champ et mappez l’élément `Array[]` de la sortie de l’agrégateur de tableau à celui-ci.
>
1. Cliquez sur **[!UICONTROL OK]** pour fermer la configuration du module [!UICONTROL JSON].
>
1. Ouvrez la configuration du module [!UICONTROL Agrégateur de tableau] . Remplacez la **[!UICONTROL structure cible]** de [!UICONTROL Custom] par le champ du module [!UICONTROL JSON] correspondant à l’attribut du tableau racine. Faites correspondre les éléments du module [!DNL Google Sheets] aux champs appropriés.
>
1. Cliquez sur **[!UICONTROL OK]** pour fermer la configuration du module [!UICONTROL Agrégateur de tableau].
>
1. Exécutez le scénario.
>
Le module [!UICONTROL JSON] génère le format JSON correct.
>
1. Ouvrez la configuration du module [!DNL Google Sheets] et augmentez le nombre [!UICONTROL maximal de lignes renvoyées] à un nombre supérieur au nombre de lignes dans votre feuille de calcul pour traiter toutes les données.

## Dépannage

### Impossible de mapper les données du module [!UICONTROL Parse JSON]

Assurez-vous que le contenu JSON est correctement mappé dans le module [!UICONTROL Parse JSON] et que la structure de données est correctement définie. Pour plus d’informations, reportez-vous à la section [Transformation des enregistrements de données en JSON](#transforming-data-records-to-json) de cet article.

### Échec du module lors de l’utilisation d’instructions conditionnelles dans JSON

lors de l’utilisation d’instructions conditionnelles telles que `if` dans votre JSON, placez les guillemets en dehors de l’instruction conditionnelle.

>[!INFO]
>
**Exemple :**
>
![](assets/quotes-in-json-350x120.png)
