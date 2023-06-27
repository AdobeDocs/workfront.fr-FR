---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Mise en correspondance des éléments à l’aide de fonctions dans [!DNL Adobe Workfront Fusion]
description: Lorsque vous mappez des éléments, vous pouvez utiliser des fonctions pour créer des formules simples ou complexes.
author: Becky
feature: Workfront Fusion
exl-id: e64d9b1e-8576-43db-ac29-0d386a482fbc
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '532'
ht-degree: 0%

---

# Mise en correspondance des éléments à l’aide de fonctions dans [!DNL Adobe Workfront Fusion]

Lorsque vous mappez des éléments, vous pouvez utiliser des fonctions pour créer des formules simples ou complexes.

Les fonctions disponibles dans [!DNL Adobe Workfront Fusion] sont similaires aux fonctions d’Excel et de certains langages de programmation. Ils évaluent la logique générale, les maths, le texte, les dates et les tableaux. Ils vous permettent d’effectuer une logique conditionnelle et des transformations des valeurs d’élément, comme convertir du texte en majuscules, rogner du texte, convertir une date dans un format différent, etc. Pour plus d’informations, voir [Mappage des informations d’un module à un autre dans Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).

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

## Insérer des fonctions dans les champs

Si vous cliquez sur un champ, la variable [!UICONTROL mapping] s’affiche. Le panneau de mappage contient plusieurs onglets :

![](assets/functions-toolbar-350x189.png)

Premier onglet ![](assets/toolbar-icon-functions-you-map-from-other-modules.png) (affiché à l’ouverture du panneau) affiche les éléments que vous pouvez mapper à partir d’autres modules.

Les autres onglets contiennent les types de fonctions suivants :

* **Fonctions générales** ![](assets/toolbar-icon-general-function.png) - Voir [Fonctions générales dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/general-functions.md) pour plus d’informations.

* **Fonctions mathématiques** ![](assets/toolbar-icon-math-functions.png) - Voir [Fonctions mathématiques dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/math-functions.md) pour plus d’informations.

* **Fonctions de texte et binaires** ![](assets/toolbar-icon-text&binary-functions.png) - Voir [Fonctions de chaîne dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/string-functions.md) pour plus d’informations.

* **Date et heure** ![](assets/toolbar-icon-date&time-functions.png) - Voir [Fonctions de date et d’heure dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/date-and-time-functions.md) et les articles ci-dessous pour plus d’informations.

   * [Jetons pour le formatage de la date et de l’heure dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-formatting.md)
   * [Jetons d’analyse de date et d’heure dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-parsing.md)

* **Fonctions relatives à l’utilisation de tableaux** ![](assets/toolbar-icon-functions-for-arrays.png) - Voir [Fonctions de tableau dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/array-functions.md) pour plus d’informations.

Pour insérer une fonction dans un champ :

1. Cliquez sur le nom de la fonction.

   Ou

   Faites glisser la fonction dans le champ.

>[!INFO]
>
>**Exemple :** Certains types de données empêchent les utilisateurs de saisir plus d’un certain nombre de caractères. Vous pouvez utiliser la fonction substring pour limiter une valeur à un certain nombre de caractères.
>
>Dans cet exemple, la fonction substring limite le nom du projet à 50 caractères.
>
>![](assets/example-meet-length-restriction-350x184.png)

## Imbrication de fonctions

Vous pouvez imbriquer des fonctions entre elles.

## Utilisation [!DNL Google Sheets] fonctions

If [!DNL Workfront Fusion] ne présente pas une fonction que vous souhaitez utiliser, mais elle est présentée par [!DNL Google Sheets], vous pouvez l’utiliser en procédant comme suit :

1. Dans [!DNL Google Sheets], créez une feuille de calcul vide.
1. Dans [!DNL Workfront Fusion], ouvrez votre scénario.
1. Ajoutez la variable **[!DNL Google Sheets]** >**[!UICONTROL Mettre à jour une cellule]** du scénario.

   Pour plus d’informations sur l’ajout d’un module, voir [Ajouter un module dans un scénario](../../workfront-fusion/scenarios/create-a-scenario.md#add) dans l’article [Création d’un scénario dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. Configurez le module :

   1. Sélectionnez la feuille de calcul nouvellement créée dans la **[!UICONTROL Feuille de calcul]** champ .
   1. Insérez votre formule contenant le [!DNL Google Sheets] fonction(s) dans la fonction **[!UICONTROL Valeur]** champ .

      Vous pouvez utiliser la sortie des modules précédents comme vous le faites habituellement.

      ![](assets/exploit-google-sheet-functions-350x218.png)

1. Insérez le **[!UICONTROL Google Sheets] >[!UICONTROL Obtention d’une cellule]** pour obtenir le résultat calculé.
1. Configurez le module à l’aide du même identifiant de cellule que celui utilisé à l’étape 4.

   ![](assets/exploit-google-sheet-functions-2-350x187.png)
