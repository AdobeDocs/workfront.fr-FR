---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: À propos des fichiers de mappage dans [!DNL Adobe Workfront Fusion]
description: Certains modules peuvent traiter des fichiers. Ces modules peuvent renvoyer un fichier de sortie à envoyer pour un traitement ultérieur ou exiger qu’un fichier leur soit transmis pour traitement. Avant que ces modules puissent travailler ensemble pour traiter les fichiers, ils doivent être mappés les uns aux autres.
author: Becky
feature: Workfront Fusion
exl-id: 9ed5f176-86d8-4139-b582-c2f58aaed8d4
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '468'
ht-degree: 25%

---

# À propos des fichiers de mappage dans [!DNL Adobe Workfront Fusion]

Certains modules peuvent traiter des fichiers. Ces modules peuvent renvoyer un fichier de sortie à envoyer pour un traitement ultérieur ou exiger qu’un fichier leur soit transmis pour traitement. Avant que ces modules puissent travailler ensemble pour traiter les fichiers, ils doivent être mappés les uns aux autres.

## Conditions d’accès

Pour utiliser les fonctionnalités décrites dans cet article, vous devez disposer des éléments suivants :

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] forfait*</td> 
   <td> <p>[!DNL Pro] ou supérieur</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence [!UICONTROL Adobe Workfront Fusion]**</td> 
   <td>
   <p>Exigences de licence actuelle : aucune exigence de licence [!DNL Workfront Fusion]</p>
   <p>Ou</p>
   <p>Exigence de licence héritée : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Exigences du produit actuel : si vous disposez du forfait [!DNL Adobe Workfront] [!UICONTROL Select] ou [!UICONTROL Prime], votre entreprise doit acheter [!DNL Adobe Workfront Fusion] et [!DNL Adobe Workfront] pour utiliser les fonctionnalités décrites dans cet article. [!DNL Workfront Fusion] est inclus dans le forfait [!DNL Workfront] [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Exigences du produit hérité : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] et [!DNL Adobe Workfront] pour utiliser les fonctionnalités décrites dans cet article.</p>
   </td> 
  </tr>  </tbody> 
</table>

Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez vote administrateur ou administratrice [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], consultez les [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Mappage de fichiers

Les modules pouvant utiliser des fichiers requièrent deux éléments d’informations :

* Nom du fichier
* Contenu du fichier (données)

Lorsque vous mappez un fichier, vous choisissez dans votre scénario les modules à partir desquels vous souhaitez obtenir les données. Le nom de fichier et le contenu du fichier sont alors automatiquement mappés tels quels.

>[!NOTE]
>
>Si vous devez traiter un fichier à partir d’une URL, nous vous recommandons d’utiliser le module `HTTP > Get a File` pour télécharger le fichier à partir de l’URL, puis de mapper le fichier du module `HTTP > Get a File` au champ du module souhaité dans votre scénario.

>[!INFO]
>
>**Exemple :** Cet exemple montre comment télécharger des documents de [!DNL Adobe Workfront] vers [!DNL Google Drive]. Le déclencheur [!DNL Workfront] [!UICONTROL Watch Record] renvoie des informations détaillées sur chaque document, y compris son nom et son identifiant.
>
>Le module suivant, [!UICONTROL Télécharger le document], télécharge les données réelles afin qu’elles puissent être chargées sur Google Drive.
>
>Pour mapper ces informations à [!DNL Google Drive] afin qu&#39;elles puissent être chargées, vous devez spécifier le fichier source à partir duquel les informations seront mappées. Si vous sélectionnez l’option [!DNL Workfront] > [!UICONTROL Télécharger le document] sous le fichier source, [!DNL Workfront Fusion] mappe le nom de fichier et le contenu du fichier afin que le document de [!DNL Workfront] soit téléchargé dans le dossier Google spécifié.
>
>![](assets/wf-download-document-350x605.png)
>
>Cependant, si vous souhaitez renommer le fichier, tout en conservant les données telles quelles, vous pouvez utiliser l’option [!UICONTROL Map] pour mapper séparément le nom du fichier et le contenu du fichier. Vous devez saisir le nom de fichier complet, y compris l’extension . Les formats de texte et de binaire, tels que les photos, les vidéos et les PDF, sont pris en charge.
>
>![](assets/use-the-map-option-350x358.png)
