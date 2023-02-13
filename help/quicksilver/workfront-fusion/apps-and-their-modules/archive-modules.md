---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Archiver les modules
description: Dans un [!DNL Adobe Workfront Fusion] vous pouvez connecter une archive (un fichier compressé, par exemple) à plusieurs applications et services tiers. Vous pouvez, par exemple, configurer un scénario qui
author: Becky
feature: Workfront Fusion
exl-id: e29b6d39-3666-4d6d-a178-1983ae9f3aa9
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 0%

---

# [!UICONTROL Archiver] modules

Dans un [!DNL Adobe Workfront Fusion] , vous pouvez utiliser une archive (un fichier compressé, par exemple) dans votre scénario, ce qui vous permet de l’utiliser dans vos automatisations ou intégrations.

Si vous avez besoin d’instructions sur la création d’un scénario, reportez-vous à la section [Création d’un scénario dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md). Pour plus d’informations sur les modules, voir [Modules dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## [!UICONTROL Archiver] modules et leurs champs

Lorsque vous configurez [!UICONTROL Archiver] modules, [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. En plus de ces [!UICONTROL Archiver] peut s’afficher, selon des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, voir [Mappage des informations d’un module à un autre dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [[!UICONTROL Extraction d’une archive]](#extract-an-archive)
* [[!UICONTROL Création d’une archive]](#create-an-archive)
* [[!UICONTROL Inflation]](#inflate)
* [[!UICONTROL Deflate]](#deflate)

## [!UICONTROL Extraction d’une archive]

Ce module d’action extrait un fichier que vous identifiez à partir d’une archive.

Le module renvoie l’identifiant du fichier et des champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Fichier source]</td> 
   <td> <p> Sélectionnez le fichier à extraire. Ce fichier peut être mappé à partir d’un module précédent (tel que le [!DNL Workfront] &gt;[!UICONTROL Télécharger un module de document]).</p>  </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Exemple :** Obtention du fichier ZIP à partir du défini [!DNL Dropbox] dossier (Archives, par exemple), extrayez-le à l’aide de l’option [!UICONTROL Archiver] et envoyer les fichiers extraits à l’adresse électronique souhaitée sous la forme de pièces jointes avec le [!UICONTROL Email] ou [!DNL Gmail] module .
>
>![](assets/example-dropbox-350x134.png)

## [!UICONTROL Création d’une archive]

Ce module d’agrégation ajoute les fichiers souhaités à un [!UICONTROL ZIP] ou [!UICONTROL TAR] archive.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Module source]</td> 
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
   <td>[!UICONTROL Fichier source]</td> 
   <td> <p>Sélectionnez un fichier source à partir d’un module précédent ou mappez le nom et les données du fichier source.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Exemple :** Regarder les emails entrants à l’aide de la fonction [!DNL Gmail] >[!UICONTROL Regarder les emails] module . Si un courrier électronique est reçu, ses pièces jointes sont itérées dans des lots individuels, puis archivées dans la variable [!DNL ZIP] et enregistré dans le dossier de Dropbox défini.
>
>![](assets/example-gmail-350x102.png)

## [!UICONTROL Inflation]

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
