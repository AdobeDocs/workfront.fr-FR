---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Modules JSON
description: L’application JSON Adobe Workfront Fusion fournit des modules pour traiter les données au format JSON afin qu’Adobe Workfront Fusion puisse continuer à utiliser le contenu des données ou créer du contenu JSON.
author: Becky
feature: Workfront Fusion
exl-id: 60540608-9d2e-4e10-9fb2-5388dda64784
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1157'
ht-degree: 0%

---

# [!UICONTROL JSON] modules

Le [!DNL Adobe Workfront Fusion] [!UICONTROL JSON] L’application fournit des modules pour traiter les données au format JSON de sorte que [!DNL Adobe Workfront Fusion] peut continuer à utiliser le contenu des données ou créer du contenu JSON.

## Exigences d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
  <td> <p>[!UICONTROL Pro] ou version ultérieure</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail] </p> <p>[!UICONTROL [!DNL Workfront Fusion] pour l’automatisation du travail] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>Votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</td> 
  </tr> 
 </tbody> 
</table>

Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

Pour plus d’informations sur [!DNL Adobe Workfront Fusion] licences, voir [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Analyse JSON

* [Structure des données](#data-structure)
* [Collection vs. Array](#collection-vs-array)

### Structure des données

La structure de données décrit l’organisation des données JSON et permet le mappage de différents éléments JSON à d’autres modules dans votre scénario. Si vous ne fournissez pas la structure de données, vous pouvez exécuter manuellement le module et [!DNL Workfront Fusion] crée la structure à partir du fichier JSON fourni :

1. Ajoutez la variable [!UICONTROL Analyse JSON] dans un scénario.
1. Dans le **[!UICONTROL Chaîne JSON]** , saisissez le code JSON à partir duquel vous souhaitez créer une structure de données.
1. Ne connectez pas d’autres modules à la fonction [!UICONTROL Analyse JSON] à l’heure actuelle. Parce que [!DNL Workfront Fusion] ne connaît pas encore la structure des données JSON, il n’est pas encore possible de mapper les données de la variable [!UICONTROL Analyse JSON] vers d’autres modules dans votre scénario.
1. Exécutez manuellement le scénario. Cela permet à la variable [!UICONTROL Analyse JSON] pour identifier la structure JSON du code JSON que vous avez fourni.
1. Vous pouvez maintenant connecter les modules suivants. Les éléments du module JSON d’analyse sont désormais disponibles pour le mappage.

Pour plus d’informations, voir [Structures de données dans [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-structures.md).

### Collection vs. Array

Si le champ de chaîne JSON contient une collection `{ ... }`, la sortie est un lot unique contenant les éléments de la collection.

>[!INFO]
>
>**Exemple:**
>
>
```
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
>**Exemple:**
>
>
```
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

## [!UICONTROL JSON] modules et leurs champs

Lorsque vous configurez [!DNL JSON] modules, [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. En outre, d’autres champs JSON peuvent s’afficher, selon des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, voir [Mappage des informations d’un module à un autre dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Agrégation vers JSON](#aggregate-to-json)
* [Convertir JSON en XML](#convert-json-to-xml)
* [Analyse JSON](#parse-json)
* [Création de JSON](#create-json)
* [Transformer JSON](#transform-json)

### [!UICONTROL Agrégation vers JSON]

Ce module d’agrégation regroupe la sortie d’un module précédent dans JSON.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Module source] </td> 
   <td> <p>Sélectionnez le module qui génère les données que vous souhaitez agréger au format JSON.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Structure de données]</td> 
   <td> <p>Sélectionnez la structure de données à utiliser pour créer JSON. La structure de données détermine les autres champs disponibles dans ce module. Pour plus d’informations, voir <a href="#data-structure" class="MCXref xref">Structure des données</a> dans cet article.</p> </td> 
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

### [!UICONTROL Analyse JSON]

Ce module d’action analyse une chaîne JSON dans une structure de données, ce qui vous permet d’accéder aux données contenues dans la chaîne JSON.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Structure de données]</td> 
   <td> <p>Sélectionnez la structure de données à utiliser pour créer JSON. Pour plus d’informations, voir <a href="#data-structure" class="MCXref xref">Structure des données</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Chaîne JSON] </td> 
   <td> <p>Saisissez ou mappez le fichier JSON que vous souhaitez analyser.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Création de JSON]

Ce module d’action crée le fichier JSON à partir d’une structure de données.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">Structure des données</td> 
   <td> <p>Sélectionnez la structure de données à utiliser pour créer JSON. Pour plus d’informations, voir <a href="#data-structure" class="MCXref xref">Structure des données</a> dans cet article.</p> </td> 
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
>1. Placez le [!DNL Google Sheets] > [!UICONTROL Sélectionner des lignes] dans votre scénario pour récupérer les données. Configurez le module pour récupérer les lignes de votre [!DNL Google] feuille de calcul. Définissez la &#x200B;**[!UICONTROL Nombre maximal de lignes renvoyées]** à un petit nombre, mais plus grand qu’un à des fins de test (par exemple, trois). Exécutez le [!DNL Google Sheets] en cliquant dessus avec le bouton droit et en choisissant &quot;**[!UICONTROL Exécuter ce module uniquement]**.&quot; Vérifiez la sortie du module.
1. Connectez-vous au [!UICONTROL Agrégateur de tableau] après l’événement [!DNL Google Sheets] module . Dans la configuration du module, sélectionnez la variable [!DNL Google Sheets] du module **[!UICONTROL Noeud source]** champ . Laissez les autres champs tels quels pour le moment.
1. Connexion [!UICONTROL JSON] > [!UICONTROL Création de JSON] après l’événement [!UICONTROL Agrégateur de tableau] module . La configuration du module nécessite une structure de données qui décrit le format JSON. Cliquez sur **[!UICONTROL Ajouter]** pour ouvrir la configuration de la structure de données . La méthode la plus simple pour créer cette structure de données consiste à la générer automatiquement à partir d’un exemple JSON. Cliquez sur **[!UICONTROL Générateur]** et collez votre exemple JSON dans le **[!UICONTROL Exemples de données]** field :

   **Exemple:**
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
1. Cliquer sur **[!UICONTROL Enregistrer]**. Le [!UICONTROL Spécification] dans la structure de données contient désormais la structure générée.
1. Remplacez le nom de votre structure de données par un nom plus spécifique, puis cliquez sur **[!UICONTROL Enregistrer]**. Un champ correspondant à l’attribut de tableau racine apparaît comme champ mappable dans la configuration du module JSON.
1. Cliquez sur le bouton **[!UICONTROL Carte]** en regard du champ et mappez le `Array[]` de la sortie de l’agrégateur Array vers celui-ci.
1. Cliquez sur **[!UICONTROL OK]** pour fermer la [!UICONTROL JSON] configuration du module.
1. Ouvrez la configuration du [!UICONTROL Agrégateur de tableau] module . Modifiez la variable **[!UICONTROL Structure cible]** de [!UICONTROL Personnalisé] au [!UICONTROL JSON] champ du module correspondant à l’attribut du tableau racine. Mappage d’éléments à partir de [!DNL Google Sheets] aux champs appropriés.
1. Cliquez sur **[!UICONTROL OK]** pour fermer la [!UICONTROL Agrégateur de tableau] configuration du module.
1. Exécutez le scénario.
   Le [!UICONTROL JSON] génère le format JSON correct.
1. Ouvrez la configuration du [!DNL Google Sheets] et augmentez la variable [!UICONTROL Nombre maximal de lignes renvoyées] pour traiter toutes les données.


## Dépannage

### Impossible de mapper les données de la variable [!UICONTROL Analyse JSON] module

Assurez-vous que le contenu JSON est correctement mappé dans la variable [!UICONTROL Analyse JSON] et que la structure des données est correctement définie. Pour plus d’informations, voir [Transformation des enregistrements de données en JSON](#transforming-data-records-to-json) dans cet article.

### Échec du module lors de l’utilisation d’instructions conditionnelles dans JSON

Lorsque vous utilisez des instructions conditionnelles telles que `if` dans votre fichier JSON, placez les guillemets en dehors de l’instruction conditionnelle.

>[!INFO]
**Exemple:**
![](assets/quotes-in-json-350x120.png)
