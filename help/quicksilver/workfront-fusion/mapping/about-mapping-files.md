---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: À propos du mappage de fichiers dans  [!DNL Adobe Workfront Fusion]
description: La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement. Cet article est obsolète, mais contient un lien vers le nouvel article qui couvre cette fonctionnalité.
author: Becky
feature: Workfront Fusion
exl-id: 9ed5f176-86d8-4139-b582-c2f58aaed8d4
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 84%

---

# À propos du mappage de fichiers dans [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement.
>
>Les informations contenues dans cet article se trouvent désormais dans l’article :
>
>* [Mapper un fichier entre modules](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/map-data/map-files.html)
>
>Mettez à jour les signets.
>
>Cet article n’est plus mis à jour et sera supprimé prochainement.

Certains modules ont la capacité de traiter des fichiers. Ces modules peuvent soit renvoyer un fichier de sortie à envoyer pour traitement ultérieur, soit exiger qu’un fichier leur soit transmis pour traitement. Avant que ces modules puissent travailler ensemble pour traiter les fichiers, ils doivent être mis en correspondance les uns avec les autres.

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
  </tr>  </tbody> 
</table>

Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez votre équipe d’administration [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], consultez Licences [[!DNL Adobe Workfront Fusion] ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Mapper des fichiers

Les modules qui ont la capacité de travailler avec des fichiers ont besoin de deux informations :

* Nom du fichier
* Contenu du fichier (données)

Lorsque vous mappez un fichier, vous choisissez les modules de votre scénario à partir desquels vous souhaitez obtenir les données. Le nom et le contenu du fichier sont alors automatiquement mappés tels quels.

>[!NOTE]
>
>Si vous devez traiter un fichier à partir d’une URL, nous vous recommandons d’utiliser le module `HTTP > Get a File` pour télécharger le fichier à partir de l’URL, puis de mapper le fichier du module `HTTP > Get a File` au champ du module souhaité dans votre scénario.

>[!INFO]
>
>**Exemple :** cet exemple montre comment télécharger des documents d’[!DNL Adobe Workfront] vers [!DNL Google Drive]. Le déclencheur [!DNL Workfront] [!UICONTROL Surveiller l’enregistrement] renvoie des informations détaillées sur chaque document, y compris son nom et son ID.
>
>Le module suivant, [!UICONTROL Télécharger le document], télécharge les données réelles afin qu’elles puissent être chargées sur Google Drive.
>
>Pour mapper ces informations sur [!DNL Google Drive] afin qu’elles puissent être chargées, vous devez spécifier le fichier source à partir duquel les informations seront mappées. Si vous sélectionnez l’option [!DNL Workfront] > [!UICONTROL Télécharger le document] sous le fichier source, [!DNL Workfront Fusion] associe le nom et le contenu du fichier de manière à ce que le document provenant de [!DNL Workfront] soit chargé dans le dossier Google spécifié.
>
>![](assets/wf-download-document-350x605.png)
>
>Toutefois, si vous souhaitez renommer le fichier tout en conservant les données telles quelles, vous pouvez utiliser l’option [!UICONTROL Mapper] pour mapper séparément le nom et le contenu du fichier. Vous devez saisir le nom complet du fichier, y compris l’extension. Les formats texte et les formats binaires, tels que les photos, les vidéos et les PDF, sont pris en charge.
>
>![](assets/use-the-map-option-350x358.png)
