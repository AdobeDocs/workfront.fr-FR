---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Modules Archive
description: Dans un scénario  [!DNL Adobe Workfront Fusion] , vous pouvez connecter une archive, telle qu’un fichier compressé, à plusieurs applications et services tiers. Vous pouvez, par exemple, configurer un scénario qui
author: Becky
feature: Workfront Fusion
exl-id: e29b6d39-3666-4d6d-a178-1983ae9f3aa9
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 24%

---

# [!UICONTROL Archiver] modules

Dans un scénario [!DNL Adobe Workfront Fusion], vous pouvez utiliser une archive, telle qu’un fichier compressé, dans votre scénario, ce qui vous permet de l’utiliser dans vos automatisations ou intégrations.

Si vous avez besoin d’instructions sur la création d’un scénario, consultez la section [Créer un scénario dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md). Pour plus d’informations sur les modules, consultez [Modules dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Modules [!UICONTROL Archive] et leurs champs

Lorsque vous configurez les modules [!UICONTROL Archive], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. En plus de cela, d’autres champs [!UICONTROL Archive] peuvent s’afficher, selon des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, consultez [Mapper les informations d’un module à un autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [[!UICONTROL Extraire une archive]](#extract-an-archive)
* [[!UICONTROL Créer une archive]](#create-an-archive)
* [[!UICONTROL Inflate]](#inflate)
* [[!UICONTROL Deflate]](#deflate)

## [!UICONTROL Extraire une archive]

Ce module d’action extrait un fichier que vous identifiez à partir d’une archive.

Le module renvoie l’ID du fichier et tous les champs associés, ainsi que les valeurs et les champs personnalisés auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Source file]</td> 
   <td> <p> Sélectionnez le fichier à extraire. Ce fichier peut être mappé à partir d’un module précédent (tel que le module [!DNL Workfront] &gt;[!UICONTROL Télécharger un document] ).</p>  </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Exemple :** Obtenez le fichier ZIP du dossier [!DNL Dropbox] défini (par exemple, Archives), extrayez-le à l’aide du module [!UICONTROL Archive] et envoyez les fichiers extraits à l’adresse électronique souhaitée en tant que pièces jointes au module [!UICONTROL Email] ou [!DNL Gmail].
>
>![](assets/example-dropbox-350x134.png)

## [!UICONTROL Créer une archive]

Ce module d&#39;agrégation ajoute les fichiers souhaités à une archive [!UICONTROL ZIP] ou [!UICONTROL TAR].

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Module [!UICONTROL Source]</td> 
   <td> <p> Sélectionnez le module à partir duquel vous souhaitez récupérer les fichiers.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Type] </td> 
   <td> <p>Indiquez si vous souhaitez ajouter des fichiers à une archive [!UICONTROL ZIP] ou à une archive [!UICONTROL TAR].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Comment]</td> 
   <td>Saisissez un commentaire à ajouter à l’archive.</td> 
  </tr> 
  <tr> 
   <td>Groupe [!UICONTROL par]</td> 
   <td> <p>Définissez une expression selon laquelle vous souhaitez regrouper la sortie agrégée. Cette expression peut contenir un ou plusieurs éléments mappés. Les données agrégées seront ensuite séparées en groupes à l’aide de la valeur de cette expression. Chaque groupe génère un lot distinct avec une clé (l’expression évaluée) et une valeur (le texte agrégé). Vous pouvez utiliser la clé comme filtre dans les modules suivants.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Arrêter le traitement après une agrégation vide]</td> 
   <td>Sélectionnez cette option pour arrêter le scénario lorsqu’il n’y a aucun résultat.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nom de l’archive]</td> 
   <td> <p> Saisissez le nom de l’archive créée. N’ajoutez pas d’extension.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source file]</td> 
   <td> <p>Sélectionnez un fichier source à partir d’un module précédent ou mappez le nom et les données du fichier source.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Exemple :** Regardez les emails entrants à l’aide du module [!DNL Gmail] >[!UICONTROL Regarder les emails] . Si un email est reçu, ses pièces jointes sont itérées dans des lots individuels, puis archivées dans le fichier [!DNL ZIP] et enregistrées dans le dossier de Dropbox défini.
>
>![](assets/example-gmail-350x102.png)

## [!UICONTROL Inflate]

Ce module du transformateur décompresse les données binaires à l’aide d’un algorithme d’inflation.

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

## [!UICONTROL Deflate]

Ce module du transformateur compresse les données binaires à l’aide d’un algorithme de déflation.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data] </td> 
   <td> <p>Saisissez ou mappez les données que vous souhaitez compresser à l’aide de la fonction dégonfler .</p> </td> 
  </tr> 
 </tbody> 
</table>
