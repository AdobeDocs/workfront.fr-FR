---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Mappage d’un tableau dans [!DNL Adobe] Workfront Fusion
description: Vous pouvez mapper un tableau à un champ de module dans Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 725e0c24-cb4b-46c4-9c00-4f9cc334fbc7
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 0%

---

# Mappage d’un tableau dans [!DNL Adobe Workfront Fusion]

Un tableau est un type spécial d’élément qui peut contenir les éléments suivants :

* Une ou plusieurs valeurs de texte (tableau simple)
* Une ou plusieurs collections du même type (tableau complexe)

>[!INFO]
>
>**Exemple :** Le [!UICONTROL Regarder les emails] renvoie un tableau de pièces jointes pour chaque email. Chaque pièce jointe représente une collection pouvant contenir un nom, un contenu, une taille, etc.

Pour plus d’informations, voir [Types de données d’élément dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md).

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
  </tr> 
 </tbody> 
</table>

Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

Pour plus d’informations sur [!DNL Adobe Workfront Fusion] licences, voir [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Mappage d’un tableau

1. Cliquez sur le bouton situé dans le champ cible.

   >[!INFO]
   >
   >  **Exemple :** Dans l’exemple ci-dessus, cliquez sur le bouton [!UICONTROL Ajout d’une pièce jointe] pour un email.
   >
   >![](assets/add-an-attachment-button-350x152.jpg)

1. Dans la zone qui s’affiche, saisissez l’élément .

   Le panneau vous permet de mapper les champs de la même manière qu’avec tout autre type d’élément. Si vous ne souhaitez pas remplir chaque élément séparément, mais que vous souhaitez mapper un autre tableau dans le champ cible, utilisez la variable [!UICONTROL Carte] bouton . Dans ce cas, assurez-vous que les deux tableaux (le tableau source et le tableau cible) ont la même structure.

   Vous pouvez ajouter n’importe quel nombre d’éléments à un tableau.

Vous pouvez diviser un tableau en lots individuels à l’aide d’un itérateur. Pour plus d’informations, voir [[!UICONTROL Itérateur] module dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md).
