---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Types de données d’élément dans [!DNL Adobe Workfront Fusion]
description: Votre [!DNL Adobe Workfront Fusion] les scénarios peuvent contenir les types d’éléments répertoriés ci-dessous dans un lot.
author: Becky
feature: Workfront Fusion
exl-id: 36c25a86-0d05-4871-a6a6-4fd54cfcc4b1
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '660'
ht-degree: 0%

---

# Types de données d’élément dans [!DNL Adobe Workfront Fusion]

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>Votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</td> 
  </tr> 
 </tbody> 
</table>

Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

Pour plus d’informations sur [!DNL Adobe Workfront Fusion] licences, voir [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Types de données d’élément

Vous pouvez contenir les types d’éléments répertoriés ci-dessous dans un lot.

Pour plus d’informations sur les types d’éléments [!DNL Workfront Fusion] permet de convertir les uns entre les autres, voir [Type de contrainte dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/type-coercion.md).

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Texte</p> </td> 
   <td> <p>Type d’élément le plus courant. Pour certains éléments de texte, [!DNL Adobe Workfront Fusion] vérifie si la longueur maximale ou minimale autorisée est respectée ou si l’élément effectue la validation du format (email, URL ou nom de fichier).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Nombre</p> </td> 
   <td> <p>Pour certains éléments numériques, [!DNL Workfront Fusion] peut valider l’entrée pour une plage spécifiée (valeur minimale ou maximale autorisée).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Booléen (Oui/Non)</p> </td> 
   <td> <p>Ce type est utilisé pour les éléments ne comportant que deux valeurs possibles : true ou false. </p> <p>Lors de la définition de modules, le type booléen peut apparaître sous deux formes différentes :</p> 
    <ul> 
     <li> <p>La case à cocher obligatoire s’affiche si le champ est obligatoire et doit être renseigné.</p> <p> <img src="assets/boolean-checkbox-350x158.jpg" style="width: 350;height: 158;"> </p> </li> 
     <li> <p>Les champs facultatifs qui peuvent ne pas être renseignés s’affichent sous forme de zone de sélection, ce qui permet d’effectuer une sélection parmi trois valeurs : <code>Yes</code>, <code>No</code>, et <code>Not defined</code> (par défaut).</p> <p> <img src="assets/boolean-convert-file-350x129.jpg" style="width: 350;height: 129;"> </p> </li> 
    </ul> <p>Vous pouvez cliquer sur <strong>[!UICONTROL Map]</strong> si vous devez mapper la valeur à un élément à partir d’un autre module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Date</p> </td> 
   <td> <p>Les dates sont renseignées au format de date ISO 8601, par exemple : <code>2015-09-18T11:58Z</code>. Vous pouvez modifier le fuseau horaire dans les paramètres du profil, comme expliqué à la section <a href="../../workfront-fusion/workfront-fusion-basics/change-profile-settings.md" class="MCXref xref">Modification des paramètres de profil dans [!DNL Adobe Workfront Fusion]</a>. </p> <p>Si vous cliquez sur un champ qui nécessite une date, un calendrier contextuel s’affiche dans les paramètres du module. Le temps n’est pas nécessaire pour certains éléments.</p> <p>Les valeurs des éléments de date sont formatées à l’aide du fuseau horaire local et Web sélectionné dans votre profil. Vous pouvez afficher la version ISO 8601 de la valeur d’un élément de date en pointant la souris sur l’élément.</p> <p>Remarque : Si la valeur ISO ne s’affiche pas, l’élément est probablement du texte et non une date.</p> <p>L’heure est saisie dans la variable <code>hours:minutes:seconds</code> format, par exemple :<code>14:03:52</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Mémoire tampon (données binaires)</p> </td> 
   <td> <p>Le contenu du fichier est généralement envoyé sous forme de contenu de type Mémoire tampon (contenu de l’image, fichier vidéo, etc.). Dans certains cas, les données de texte sont incluses dans ce type (par exemple, un fichier texte). [!DNL Workfront Fusion] peut automatiquement convertir des données texte en code binaire en texte et du texte en données texte en code binaire. Pour plus d’informations, voir <a href="../../workfront-fusion/mapping/about-mapping-files.md" class="MCXref xref">À propos du mappage des fichiers dans [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Collection</p> </td> 
   <td> <p>Une collection est un élément composé de plusieurs sous-éléments. L’élément Expéditeur d’un email est un exemple de collection : il contient le nom de l'expéditeur (type texte) et l'adresse email de l'expéditeur (type texte).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Sélectionner (menu)</p> </td> 
   <td> <p>Lorsque vous configurez les paramètres du module, comme décrit dans <a href="../../workfront-fusion/modules/configure-a-modules-settings.md" class="MCXref xref">Configurez les paramètres d’un module dans [!DNL Adobe Workfront Fusion]</a>, vous pouvez effectuer une sélection parmi plusieurs éléments du même type. Par exemple, le menu de sélection de dossier dans les paramètres de la variable [!DNL Dropbox] modules. </p> <p>Lors de la définition des modules, le menu de sélection peut apparaître sous deux formes :</p> <p> <p>Si plusieurs sélections sont possibles, plusieurs éléments avec des cases à cocher s’affichent.</p> <p> <img src="assets/image-kb-type-list-multi-350x232.jpg" style="width: 350;height: 232;"> </p> </p> <p>Si une seule option est possible, un menu déroulant s’affiche.</p> <p> <img src="assets/select-menu-dropdown-350x130.jpg" style="width: 350;height: 130;"> </p> <p>Si vous devez mapper un élément à partir d’un autre module, utilisez la variable <strong>Carte</strong> bouton . Ce bouton ouvre un champ de texte au lieu du menu de sélection. Pour plus d’informations, voir <a href="../../workfront-fusion/mapping/map-information-between-modules.md" class="MCXref xref">Mappage des informations d’un module à un autre dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Tableau</p> </td> 
   <td> <p>Vous pouvez utiliser le type de tableau pour utiliser plusieurs valeurs du même type, y compris des collections. Par exemple, les modules [!UICONTROL Email] : ils renvoient un tableau de pièces jointes et chaque pièce jointe contient le nom, le contenu, la taille, etc. Pour plus d’informations, voir <a href="../../workfront-fusion/mapping/map-an-array.md" class="MCXref xref">Mappage d’un tableau dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Validation</p> </td> 
   <td> <p>[!DNL Workfront Fusion] peut effectuer la validation sur chaque type d’élément. Si un élément ne passe pas la validation, le module arrête le traitement en raison d’une erreur de données. Pour plus d’informations, voir <a href="../../workfront-fusion/errors/error-processing.md" class="MCXref xref">Traitement des erreurs dans [!DNL Adobe Workfront Fusion]</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>
