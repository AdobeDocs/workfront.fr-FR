---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Modules d’image
description: Les modules Adobe Workfront Fusion Image vous permettent d’obtenir des informations sur une image spécifique (dimensions, type, etc.), de convertir une image dans un autre format de fichier et de modifier directement la taille de l’image.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 89efa9d5-00c9-4bb5-97b3-2b2f9d73721d
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '912'
ht-degree: 16%

---

# Modules d’image

Les modules [!DNL Adobe Workfront Fusion] [!UICONTROL Image] vous permettent d’obtenir des informations sur une image spécifique (dimensions, type, etc.), de convertir une image dans un autre format de fichier et de modifier directement la taille de l’image.

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

## Modules [!UICONTROL Image] et leurs champs

Lors de la configuration de ce module, les champs suivants s’affichent. Un titre en gras dans un module indique un champ obligatoire.

* [[!UICONTROL Resize]](#resize)
* [[!UICONTROL Convertir un format]](#convert-a-format)
* [[!UICONTROL Extraction de métadonnées]](#extract-metadata)

### [!UICONTROL Resize]

Ce module du transformateur modifie la hauteur et la largeur d’une image en fonction des critères que vous spécifiez.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Sélectionnez la source de l’image que vous souhaitez convertir. Vous pouvez sélectionner la sortie d’un module précédent ou mapper le fichier de données et le nom de fichier. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data]</td> 
   <td>Mappez le fichier que vous souhaitez convertir. Ce champ est disponible si vous avez sélectionné [!UICONTROL Map] dans le champ [!UICONTROL Source file] .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File name]</td> 
   <td>Saisissez le nom du fichier converti. Ce champ est disponible si vous avez sélectionné [!UICONTROL Map] dans le champ [!UICONTROL Source file] .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Je veux]</td> 
   <td>Indiquez si vous souhaitez conserver le rapport hauteur-largeur ou modifier les dimensions en hauteur et largeur spécifiées.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Selon]</td> 
   <td> <p>Sélectionnez la manière dont vous souhaitez que le module détermine la nouvelle taille de l’image. Ce champ s’affiche si vous avez choisi de conserver le rapport hauteur-largeur dans le champ Je veux. D’autres champs s’affichent en fonction de la sélection effectuée dans ce champ.</p> 
    <ul> 
     <li> <p>[!UICONTROL Largeur maximale]</p> <p>Réduit une image à une largeur que vous spécifiez. La hauteur est calculée automatiquement.</p> </li> 
     <li> <p>[!UICONTROL Hauteur maximale]</p> <p>Réduit une image à une hauteur que vous spécifiez. La largeur est calculée automatiquement.</p> </li> 
     <li> <p>[!UICONTROL Hauteur ou largeur maximale]</p> <p>Réduit une image de sorte que sa hauteur et sa largeur ne dépassent pas les valeurs que vous spécifiez. Comme cette option conserve les proportions, l’une des dimensions peut être plus petite que celle spécifiée. Par exemple, si la hauteur et la largeur sont toutes deux définies sur 40, une image de 400x300 sera réduite à 40x30.</p> </li> 
     <li> <p>[!UICONTROL Largeur minimale]</p> <p>agrandit une image à une largeur que vous spécifiez. La hauteur est calculée automatiquement.</p> </li> 
     <li> <p>[!UICONTROL Hauteur minimale]</p> <p>agrandit une image à une hauteur que vous spécifiez. La largeur est calculée automatiquement.</p> </li> 
     <li> <p>[!UICONTROL Hauteur ou largeur minimale]</p> <p>agrandit une image de sorte que sa hauteur et sa largeur ne soient pas inférieures aux valeurs que vous spécifiez. Comme cette option conserve les proportions, l’une des dimensions peut être plus grande que celle spécifiée. Par exemple, si la hauteur et la largeur sont toutes deux définies comme 300, une image de 40x30 sera étendue à 400x300.</p> </li> 
     <li> <p>[!UICONTROL Pourcentage]</p> <p>Modifie la taille de l’image d’un pourcentage en fonction de la valeur que vous spécifiez. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Width]</td> 
   <td>Saisissez ou mappez la largeur souhaitée de l’image redimensionnée en pixels.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Hauteur]</td> 
   <td>Saisissez ou mappez la hauteur souhaitée de l’image redimensionnée en pixels.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Convertir un format]

Ce module du transformateur modifie le format d’un fichier image. Ce module est compatible avec les formats suivants :

* PNG
* JPG
* GIF
* BMP

Le fichier source et la sortie doivent se trouver dans l’un de ces formats. Par exemple, le module [!UICONTROL Image] >[!UICONTROL Convertir un format] peut transformer un fichier PNG en fichier BMP, ou un fichier BMP en JPG.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Sélectionnez la source de l’image que vous souhaitez convertir. Vous pouvez sélectionner la sortie d’un module précédent ou mapper le fichier de données et le nom de fichier. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data]</td> 
   <td>Mappez le fichier que vous souhaitez convertir. Ce champ est disponible si vous avez sélectionné [!UICONTROL Map] dans le champ [!UICONTROL Source file] .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File name]</td> 
   <td>Saisissez le nom du fichier converti. Ce champ est disponible si vous avez sélectionné [!UICONTROL Map] dans le champ [!UICONTROL Source file] .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Format de sortie]</td> 
   <td>Sélectionnez le format dans lequel vous souhaitez que le module convertisse le fichier source. </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Extraction de métadonnées]

Ce module du transformateur renvoie des informations de base sur un module.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Sélectionnez la source de l’image que vous souhaitez convertir. Vous pouvez sélectionner la sortie d’un module précédent ou mapper le fichier de données et le nom de fichier. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data]</td> 
   <td>Mappez le fichier que vous souhaitez convertir. Ce champ est disponible si vous avez sélectionné Mappage dans le champ [!UICONTROL Fichier Source] .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File name]</td> 
   <td>Saisissez le nom du fichier converti. Ce champ est disponible si vous avez sélectionné Mappage dans le champ [!UICONTROL Fichier Source] .</td> 
  </tr> 
 </tbody> 
</table>

## Problèmes possibles

### Action terminée avec une erreur

Il existe trois cas où une action peut se terminer par une erreur :

* Les données reçues n’étaient pas au format JPG/GIF/PNG/BMP.
* La limite de largeur/hauteur maximale a été dépassée lors de la modification des dimensions de l’image. La taille de l’image ne doit pas dépasser 3 840 pixels de largeur et 2 160 pixels de hauteur.
* La taille maximale autorisée d’une image a été dépassée lors de la modification des dimensions ou du format de l’image.
