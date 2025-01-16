---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Types de données d’élément dans  [!DNL Adobe Workfront Fusion]
description: La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement. Cet article est obsolète, mais contient un lien vers le nouvel article qui couvre cette fonctionnalité.
author: Becky
feature: Workfront Fusion
exl-id: 36c25a86-0d05-4871-a6a6-4fd54cfcc4b1
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '771'
ht-degree: 90%

---

# Types de données d’élément dans [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement.
>
>Les informations contenues dans cet article se trouvent désormais dans l’article :
>
>* [Types de données d’élément](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/mapping-panel/data-types/item-data-types.html)
>
>Mettez à jour les signets.
>
>Cet article n’est plus mis à jour et sera supprimé prochainement.

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
  </tr> 
 </tbody> 
</table>

Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez votre équipe d’administration [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], consultez Licences [[!DNL Adobe Workfront Fusion] ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Types de données d’élément

Vous pouvez contenir les types d’éléments répertoriés ci-dessous dans un lot.

Pour savoir quels types d’éléments [!DNL Workfront Fusion] permettent de les convertir entre eux, voir [Coercition de type dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/type-coercion.md).

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Texte</p> </td> 
   <td> <p>Type d’élément le plus courant. Pour certains éléments de texte, [!DNL Adobe Workfront Fusion] vérifie si la longueur maximale ou minimale autorisée est respectée ou si l’élément effectue la validation du format (e-mail, URL ou nom de fichier).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Nombre</p> </td> 
   <td> <p>Pour certains éléments numériques, [!DNL Workfront Fusion] peut valider l’entrée pour une plage spécifiée (valeur minimale ou maximale autorisée).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Booléen (oui/non)</p> </td> 
   <td> <p>Ce type est utilisé pour les éléments qui n’ont que deux valeurs possibles : true ou false. </p> <p>Lors de la définition de modules, le type booléen peut apparaître sous deux formes différentes :</p> 
    <ul> 
     <li> <p>La case à cocher obligatoirement s’affiche si le champ est obligatoire et doit être renseigné.</p> <p> <img src="assets/boolean-checkbox-350x158.jpg" style="width: 350;height: 158;"> </p> </li> 
     <li> <p>Les champs facultatifs qui peuvent rester vides s’affichent sous forme de zone de sélection, ce qui permet d’effectuer une sélection parmi trois valeurs : <code>Yes</code>, <code>No</code>, et <code>Not defined</code> (par défaut).</p> <p> <img src="assets/boolean-convert-file-350x129.jpg" style="width: 350;height: 129;"> </p> </li> 
    </ul> <p>Cliquez sur <strong>[!UICONTROL Map]</strong> si vous devez mapper la valeur à un élément à partir d’un autre module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Date</p> </td> 
   <td> <p>Les dates sont saisies au format de date ISO 8601, par exemple : <code>2015-09-18T11:58Z</code>. Vous pouvez modifier le fuseau horaire dans les paramètres de votre profil, tel qu’indiqué dans <a href="../../workfront-fusion/workfront-fusion-basics/change-profile-settings.md" class="MCXref xref">Modifier les paramètres de profil dans [!DNL Adobe Workfront Fusion]</a>. </p> <p>Si vous cliquez sur un champ qui nécessite une date, un calendrier contextuel s’affiche dans les paramètres du module. L’heure n’est pas nécessaire pour certains éléments.</p> <p>Les valeurs des éléments de date sont formatées à l’aide du fuseau horaire local et web sélectionné dans votre profil. Vous pouvez afficher la version ISO 8601 de la valeur d’un élément de date en pointant la souris sur l’élément.</p> <p>Note : si la valeur ISO ne s’affiche pas, l’élément est probablement du texte et non pas une date.</p> <p>L’heure est saisie au format <code>hours:minutes:seconds</code>, par exemple : <code>14:03:52</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Buffer (données binaires)</p> </td> 
   <td> <p>Le contenu du fichier est généralement envoyé sous forme de contenu de type buffer (contenu de l’image, fichier vidéo, etc.). Dans certains cas, les données de texte sont incluses dans ce type (par exemple, un fichier texte). [!DNL Workfront Fusion] peut automatiquement convertir des données de texte en code binaire puis en texte et du texte en données de texte puis en code binaire. Pour plus d’informations, voir <a href="../../workfront-fusion/mapping/about-mapping-files.md" class="MCXref xref">À propos du mappage des fichiers dans [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Collection</p> </td> 
   <td> <p>Une collection est un élément composé de plusieurs sous-éléments. L’élément Expéditeur ou expéditrice d’un e-mail est un exemple de collection : il contient le nom de l’expéditeur ou de l’expéditrice (type texte) et son adresse e-mail (type texte).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Sélectionner (menu)</p> </td> 
   <td> <p>Lorsque vous configurez les paramètres du module, comme décrit dans <a href="../../workfront-fusion/modules/configure-a-modules-settings.md" class="MCXref xref">Configurer les paramètres d’un module dans [!DNL Adobe Workfront Fusion]</a>, vous pouvez effectuer une sélection parmi plusieurs éléments du même type. Par exemple, le menu de sélection de dossier dans les paramètres des modules [!DNL Dropbox]. </p> <p>Lors de la définition des modules, le menu de sélection peut apparaître sous deux formes :</p> <p> <p>Si plusieurs sélections sont possibles, plusieurs éléments avec des cases à cocher s’affichent.</p> <p> <img src="assets/image-kb-type-list-multi-350x232.jpg" style="width: 350;height: 232;"> </p> </p> <p>Si une seule option est possible, un menu déroulant s’affiche.</p> <p> <img src="assets/select-menu-dropdown-350x130.jpg" style="width: 350;height: 130;"> </p> <p>Si vous devez mapper un élément à partir d’un autre module, utilisez le bouton <strong>Mapper</strong>. Ce bouton ouvre un champ de texte au lieu du menu de sélection. Pour plus d’informations, consultez <a href="../../workfront-fusion/mapping/map-information-between-modules.md" class="MCXref xref">Mapper des informations d’un module à l’autre dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Tableau</p> </td> 
   <td> <p>Vous pouvez utiliser le type de tableau pour utiliser plusieurs valeurs du même type, y compris des collections. Par exemple, les modules [!UICONTROL Email] renvoient un tableau de pièces jointes et chaque pièce jointe contient le nom, le contenu, la taille, etc. Pour plus d’informations, consultez <a href="../../workfront-fusion/mapping/map-an-array.md" class="MCXref xref">Mapper un tableau dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Validation</p> </td> 
   <td> <p>[!DNL Workfront Fusion] peut effectuer la validation sur chaque type d’élément. Si un élément ne passe pas la validation, le module arrête le traitement en raison d’une erreur de données. Pour plus d’informations, consultez <a href="../../workfront-fusion/errors/error-processing.md" class="MCXref xref">Traitement des erreurs dans [!DNL Adobe Workfront Fusion]</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>
