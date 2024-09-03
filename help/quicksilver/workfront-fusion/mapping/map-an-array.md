---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Mapper un tableau dans  [!DNL Adobe]  Workfront Fusion
description: Vous pouvez mapper un tableau à un champ de module dans Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 725e0c24-cb4b-46c4-9c00-4f9cc334fbc7
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 100%

---

# Mapper un tableau dans [!DNL Adobe Workfront Fusion]

Un tableau est un type spécial d’élément qui peut contenir les éléments suivants :

* Une ou plusieurs valeurs de texte (tableau simple)
* Une ou plusieurs collections du même type (tableau complexe)

>[!INFO]
>
>**Exemple :** le module [!UICONTROL Contrôle des e-mails] renvoie un tableau de pièces jointes pour chaque e-mail. Chaque pièce jointe représente une collection pouvant contenir un nom, un contenu, une taille, etc.

Pour plus d’informations, consultez [Types de données d’élément dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md).

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

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], voir [[!DNL Adobe Workfront Fusion] Licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Mapper un tableau

1. Cliquez sur le bouton situé dans le champ cible.

   >[!INFO]
   >
   >  **Exemple :** Dans l’exemple ci-dessus, cliquez sur le bouton [!UICONTROL Ajouter une pièce jointe] pour un e-mail.
   >
   >![](assets/add-an-attachment-button-350x152.jpg)

1. Dans la zone qui s’affiche, saisissez l’élément.

   Le panneau vous permet de mapper les champs de la même manière qu’avec tout autre type d’élément. Si vous ne souhaitez pas remplir chaque élément séparément, mais que vous souhaitez mapper un autre tableau dans le champ cible, utilisez le bouton [!UICONTROL Mapper]. Dans ce cas, assurez-vous que les deux tableaux (le tableau source et le tableau cible) ont la même structure.

   Vous pouvez ajouter n’importe quel nombre d’éléments à un tableau.

Vous pouvez diviser un tableau en lots individuels à l’aide d’un itérateur. Pour plus d’informations, consultez Module d’[[!UICONTROL itération] dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md).
