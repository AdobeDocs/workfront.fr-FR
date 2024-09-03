---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Modules Archive
description: Dans un scénario  [!DNL Adobe Workfront Fusion] , vous pouvez connecter une archive, comme un fichier compressé, à plusieurs applications et services tiers. Par exemple, vous pouvez configurer un scénario qui fait ce qui suit.
author: Becky
feature: Workfront Fusion
exl-id: e29b6d39-3666-4d6d-a178-1983ae9f3aa9
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 100%

---

# Modules d’[!UICONTROL archive]

Dans un scénario [!DNL Adobe Workfront Fusion], vous pouvez utiliser une archive, comme un fichier compressé, dans votre scénario, ce qui vous permet de l’utiliser dans vos automatismes ou vos intégrations.

Si vous avez besoin d’instructions sur la création d’un scénario, voir [Créer un scénario dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md). Pour plus d’informations sur les modules, voir [Modules dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Modules d’[!UICONTROL archive] et leurs champs

Lorsque vous configurez des modules d’[!UICONTROL archive], [!DNL Workfront Fusion] affiche les champs énumérés ci-dessous. En plus de ces champs, d’autres champs d’[!UICONTROL archive] peuvent s’afficher, en fonction de facteurs tels que votre niveau d’accès à l’application ou au service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton « Mapper » apparaît au-dessus d’un champ ou d’une fonction, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, voir [Mapper des informations d’un module à l’autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [[!UICONTROL Extraire une archive]](#extract-an-archive)
* [[!UICONTROL Créer une archive]](#create-an-archive)
* [[!UICONTROL Gonfler]](#inflate)
* [[!UICONTROL Dégonfler]](#deflate)

## [!UICONTROL Extraire une archive]

Ce module d’action extrait d’une archive un fichier que vous avez identifié.

Le module renvoie l’ID du fichier et tous les champs associés, ainsi que les valeurs et les champs personnalisés auxquels la connexion a accès. Vous pouvez mettre en correspondance ces informations dans les modules suivants du scénario.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Source file]</td> 
   <td> <p> Sélectionnez le fichier à extraire. Ce fichier peut être mappé à partir d’un module précédent (tel que le module [!DNL Workfront] &gt; [!UICONTROL Download a document]).</p>  </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Exemple :** récupérez le fichier ZIP dans le dossier [!DNL Dropbox] défini (par exemple, Archives), extrayez-le à l’aide du module [!UICONTROL Archive] et envoyez les fichiers extraits à l’adresse e-mail souhaitée sous forme de pièces jointes à l’aide du module [!UICONTROL E-mail] ou [!DNL Gmail].
>
>![](assets/example-dropbox-350x134.png)

## [!UICONTROL Créer une archive]

Ce module agrégateur ajoute les fichiers souhaités à une archive [!UICONTROL ZIP] ou [!UICONTROL TAR].

Lorsque vous configurez ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Source module]</td> 
   <td> <p> Sélectionnez le module à partir duquel vous souhaitez récupérer les fichiers.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Type] </td> 
   <td> <p>Sélectionnez si vous souhaitez ajouter des fichiers à une archive [!UICONTROL ZIP] ou à une archive [!UICONTROL TAR].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Comment]</td> 
   <td>Saisissez un commentaire que vous souhaitez ajouter à l’archive.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Group by]</td> 
   <td> <p>Définissez une expression selon laquelle vous souhaitez regrouper la sortie agrégée. Cette expression peut contenir un ou plusieurs éléments mappés. Les données agrégées seront ensuite séparées en groupes à l’aide de la valeur de cette expression. Chaque groupe se présente sous la forme d’un lot distinct avec une clé (l’expression évaluée) et une valeur (le texte agrégé). Vous pouvez utiliser la clé comme filtre dans les modules suivants.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Stop processing after an empty aggregation]</td> 
   <td>Sélectionnez cette option pour arrêter le scénario lorsqu’il n’y a aucun résultat.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Archive name]</td> 
   <td> <p> Saisissez un nom pour l’archive créée. N’ajoutez pas d’extension.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source file]</td> 
   <td> <p>Sélectionnez un fichier source à partir d’un module précédent ou mappez le nom et les données du fichier source.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Exemple :** surveillez les e-mails entrants à l’aide du module [!DNL Gmail] > [!UICONTROL Surveiller les e-mails]. Si un e-mail est reçu, ses pièces jointes sont itérées en lots individuels, puis archivées dans le fichier [!DNL ZIP] et enregistrées dans le dossier Dropbox défini.
>
>![](assets/example-gmail-350x102.png)

## [!UICONTROL Gonfler]

Ce module transformateur décompresse les données binaires à l’aide d’un algorithme d’inflation.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data] </td> 
   <td> <p>Saisissez ou mappez les données que vous souhaitez décompresser à l’aide de la fonction de gonflage.</p> </td> 
  </tr> 
 </tbody> 
</table>

## [!UICONTROL Dégonfler]

Ce module de transformation compresse les données binaires à l’aide d’un algorithme de déflation.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data] </td> 
   <td> <p>Saisissez ou mappez les données que vous souhaitez compresser à l’aide de la fonction dégonfler.</p> </td> 
  </tr> 
 </tbody> 
</table>
