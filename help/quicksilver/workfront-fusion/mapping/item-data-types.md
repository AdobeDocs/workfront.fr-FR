---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Types de données d’élément dans  [!DNL Adobe Workfront Fusion]
description: Vos  [!DNL Adobe Workfront Fusion]  scénarios peuvent contenir les types d’éléments répertoriés ci-dessous dans un lot.
author: Becky
feature: Workfront Fusion
exl-id: 36c25a86-0d05-4871-a6a6-4fd54cfcc4b1
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '710'
ht-degree: 17%

---

# Types de données d’élément dans [!DNL Adobe Workfront Fusion]

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
  </tr> 
 </tbody> 
</table>

Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez vote administrateur ou administratrice [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], consultez les [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Types de données d’élément

Vous pouvez contenir les types d’éléments répertoriés ci-dessous dans un lot.

Pour plus d&#39;informations sur les types d&#39;éléments [!DNL Workfront Fusion] qui permettent une conversion entre eux, voir [Contrainte de type dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/type-coercion.md).

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
   <td> <p>Pour certains éléments numériques, [!DNL Workfront Fusion] peut valider l’entrée pour une plage spécifiée (la valeur minimale ou maximale autorisée).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Booléen (Oui/Non)</p> </td> 
   <td> <p>Ce type est utilisé pour les éléments qui n’ont que deux valeurs possibles : true ou false. </p> <p>Lors de la définition de modules, le type booléen peut apparaître sous deux formes différentes :</p> 
    <ul> 
     <li> <p>La case à cocher obligatoire s’affiche si le champ est obligatoire et doit être renseigné.</p> <p> <img src="assets/boolean-checkbox-350x158.jpg" style="width: 350;height: 158;"> </p> </li> 
     <li> <p>Les champs facultatifs qui peuvent être laissés vides s’affichent sous forme de zone de sélection, ce qui permet la sélection parmi trois valeurs : <code>Yes</code>, <code>No</code> et <code>Not defined</code> (par défaut).</p> <p> <img src="assets/boolean-convert-file-350x129.jpg" style="width: 350;height: 129;"> </p> </li> 
    </ul> <p>Vous pouvez cliquer sur <strong>[!UICONTROL Map]</strong> si vous devez mapper la valeur à un élément à partir d’un autre module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Date</p> </td> 
   <td> <p>Les dates sont entrées dans le format de date ISO 8601, par exemple, <code>2015-09-18T11:58Z</code>. Vous pouvez modifier le fuseau horaire dans les paramètres de votre profil, comme expliqué dans la section <a href="../../workfront-fusion/workfront-fusion-basics/change-profile-settings.md" class="MCXref xref">Modification des paramètres de profil dans [!DNL Adobe Workfront Fusion]</a>. </p> <p>Si vous cliquez sur un champ qui nécessite une date, un calendrier contextuel s’affiche dans les paramètres du module. Le temps n’est pas nécessaire pour certains éléments.</p> <p>Les valeurs des éléments de date sont formatées à l’aide du fuseau horaire local et Web sélectionné dans votre profil. Vous pouvez afficher la version ISO 8601 de la valeur d’un élément de date en pointant la souris sur l’élément.</p> <p>Remarque : Si la valeur ISO ne s’affiche pas, l’élément est probablement du texte, pas une date.</p> <p>L’heure est saisie au format <code>hours:minutes:seconds</code>, par exemple,<code>14:03:52</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Mémoire tampon (données binaires)</p> </td> 
   <td> <p>Le contenu du fichier est généralement envoyé sous forme de contenu de type Mémoire tampon (contenu de l’image, fichier vidéo, etc.). Dans certains cas, les données de texte sont incluses dans ce type (par exemple, un fichier texte). [!DNL Workfront Fusion] peut automatiquement convertir des données texte en code binaire en texte et du texte en données texte en code binaire. Pour plus d’informations, voir <a href="../../workfront-fusion/mapping/about-mapping-files.md" class="MCXref xref">À propos des fichiers de mappage dans [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Collection</p> </td> 
   <td> <p>Une collection est un élément composé de plusieurs sous-éléments. L'élément Expéditeur d'un email est un exemple de collection : il contient le nom de l'expéditeur (type texte) et l'adresse email de l'expéditeur (type texte).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Sélectionner (menu)</p> </td> 
   <td> <p>Lorsque vous configurez les paramètres du module comme décrit dans <a href="../../workfront-fusion/modules/configure-a-modules-settings.md" class="MCXref xref">Configurer les paramètres d'un module dans [!DNL Adobe Workfront Fusion]</a>, vous pouvez sélectionner plusieurs éléments du même type. Par exemple, le menu de sélection de dossier dans les paramètres des modules [!DNL Dropbox]. </p> <p>Lors de la définition des modules, le menu de sélection peut apparaître sous deux formes :</p> <p> <p>Si plusieurs sélections sont possibles, plusieurs éléments avec des cases à cocher s’affichent.</p> <p> <img src="assets/image-kb-type-list-multi-350x232.jpg" style="width: 350;height: 232;"> </p> </p> <p>Si une seule option est possible, un menu déroulant s’affiche.</p> <p> <img src="assets/select-menu-dropdown-350x130.jpg" style="width: 350;height: 130;"> </p> <p>Si vous devez mapper un élément à partir d’un autre module, utilisez le bouton <strong>Map</strong> . Ce bouton ouvre un champ de texte au lieu du menu de sélection. Pour plus d'informations, voir <a href="../../workfront-fusion/mapping/map-information-between-modules.md" class="MCXref xref">Mappage des informations d'un module à un autre dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Tableau</p> </td> 
   <td> <p>Vous pouvez utiliser le type de tableau pour utiliser plusieurs valeurs du même type, y compris des collections. Par exemple, les modules [!UICONTROL Email] : ils renvoient un tableau de pièces jointes et chaque pièce jointe contient le nom, le contenu, la taille, etc. Pour plus d’informations, voir <a href="../../workfront-fusion/mapping/map-an-array.md" class="MCXref xref">Mappage d’un tableau dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Validation</p> </td> 
   <td> <p>[!DNL Workfront Fusion] peut effectuer la validation sur chaque type d’élément. Si un élément ne passe pas la validation, le module arrête le traitement en raison d’une erreur de données. Pour plus d’informations, voir <a href="../../workfront-fusion/errors/error-processing.md" class="MCXref xref">Traitement des erreurs dans [!DNL Adobe Workfront Fusion]</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>
