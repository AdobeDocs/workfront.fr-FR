---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: À propos du mappage des fichiers dans [!DNL Adobe Workfront Fusion]
description: Certains modules peuvent traiter des fichiers. Ces modules peuvent renvoyer un fichier de sortie à envoyer pour un traitement ultérieur ou exiger qu’un fichier leur soit transmis pour traitement. Avant que ces modules puissent travailler ensemble pour traiter les fichiers, ils doivent être mappés les uns aux autres.
author: Becky
feature: Workfront Fusion
exl-id: 9ed5f176-86d8-4139-b582-c2f58aaed8d4
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '468'
ht-degree: 0%

---

# À propos du mappage des fichiers dans [!DNL Adobe Workfront Fusion]

Certains modules peuvent traiter des fichiers. Ces modules peuvent renvoyer un fichier de sortie à envoyer pour un traitement ultérieur ou exiger qu’un fichier leur soit transmis pour traitement. Avant que ces modules puissent travailler ensemble pour traiter les fichiers, ils doivent être mappés les uns aux autres.

## Exigences d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] ou supérieur</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence [!UICONTROL Adobe Workfront Fusion]**</td> 
   <td>
   <p>Exigences de licence actuelles : Non [!DNL Workfront Fusion] conditions requises pour obtenir une licence.</p>
   <p>Ou</p>
   <p>Exigences de licence héritées : [!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Exigences actuelles du produit : Si vous disposez de [!UICONTROL Select] ou [!UICONTROL Prime] [!DNL Adobe Workfront] Planifiez, votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article. [!DNL Workfront Fusion] est inclus dans l’[!UICONTROL Ultimate] [!DNL Workfront] planifiez.</p>
   <p>Ou</p>
   <p>Exigences de produit héritées : Votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
   </td> 
  </tr>  </tbody> 
</table>

Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

Pour plus d’informations sur [!DNL Adobe Workfront Fusion] licences, voir [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Mappage de fichiers

Les modules pouvant utiliser des fichiers requièrent deux éléments d’informations :

* Nom du fichier
* Contenu du fichier (données)

Lorsque vous mappez un fichier, vous choisissez dans votre scénario les modules à partir desquels vous souhaitez obtenir les données. Le nom de fichier et le contenu du fichier sont alors automatiquement mappés tels quels.

>[!NOTE]
>
>Si vous devez traiter un fichier à partir d’une URL, il est recommandé d’utiliser la variable `HTTP > Get a File` pour télécharger le fichier à partir de l’URL, puis mapper le fichier à partir de la fonction `HTTP > Get a File` au champ du module souhaité dans votre scénario.

>[!INFO]
>
>**Exemple :** Cet exemple montre comment télécharger des documents à partir de [!DNL Adobe Workfront] to [!DNL Google Drive]. Le [!DNL Workfront] trigger [!UICONTROL Surveiller les enregistrements] renvoie des informations détaillées sur chaque document, y compris son nom et son identifiant.
>
>le module suivant, [!UICONTROL Télécharger le document], télécharge les données réelles afin qu’elles puissent être chargées sur Google Drive.
>
>Pour mapper ces informations à [!DNL Google Drive] pour qu’il puisse être téléchargé, vous devez spécifier le fichier source à partir duquel les informations seront mappées. Si vous sélectionnez la variable [!DNL Workfront] > [!UICONTROL Télécharger le document] sous le fichier source, [!DNL Workfront Fusion] mappe le nom de fichier et le contenu du fichier de sorte que le document de [!DNL Workfront] est chargé dans le dossier Google spécifié.
>
>![](assets/wf-download-document-350x605.png)
>
>Cependant, si vous souhaitez renommer le fichier, tout en conservant les données telles quelles, vous pouvez utiliser la variable [!UICONTROL Carte] pour mapper séparément le nom du fichier et le contenu du fichier. Vous devez saisir le nom de fichier complet, y compris l’extension . Les formats de texte et de binaire, tels que les photos, les vidéos et les PDF, sont pris en charge.
>
>![](assets/use-the-map-option-350x358.png)
