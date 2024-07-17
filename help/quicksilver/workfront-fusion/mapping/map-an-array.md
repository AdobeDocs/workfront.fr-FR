---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Mappage d’un tableau dans  [!DNL Adobe] Workfront Fusion
description: Vous pouvez mapper un tableau à un champ de module dans Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 725e0c24-cb4b-46c4-9c00-4f9cc334fbc7
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 35%

---

# Mapper un tableau dans [!DNL Adobe Workfront Fusion]

Un tableau est un type spécial d’élément qui peut contenir les éléments suivants :

* Une ou plusieurs valeurs de texte (tableau simple)
* Une ou plusieurs collections du même type (tableau complexe)

>[!INFO]
>
>**Exemple :** Le module [!UICONTROL Watch emails] renvoie un tableau de pièces jointes pour chaque courrier électronique. Chaque pièce jointe représente une collection pouvant contenir un nom, un contenu, une taille, etc.

Pour plus d’informations, voir [Types de données d’élément dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md).

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

## Mappage d’un tableau

1. Cliquez sur le bouton situé dans le champ cible.

   >[!INFO]
   >
   >  **Exemple :** Dans l&#39;exemple ci-dessus, vous allez cliquer sur le bouton [!UICONTROL Ajouter une pièce jointe] pour un email.
   >
   >![](assets/add-an-attachment-button-350x152.jpg)

1. Dans la zone qui s’affiche, saisissez l’élément .

   Le panneau vous permet de mapper les champs de la même manière qu’avec tout autre type d’élément. Si vous ne souhaitez pas remplir séparément chaque élément, mais que vous souhaitez mapper un autre tableau dans le champ cible, utilisez le bouton [!UICONTROL Map] . Dans ce cas, assurez-vous que les deux tableaux (le tableau source et le tableau cible) ont la même structure.

   Vous pouvez ajouter n’importe quel nombre d’éléments à un tableau.

Vous pouvez diviser un tableau en lots individuels à l’aide d’un itérateur. Pour plus d’informations, voir le module [[!UICONTROL Itérateur] dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md).
