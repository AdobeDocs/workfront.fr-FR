---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Mise en correspondance des éléments à l’aide de fonctions dans [!DNL Adobe Workfront Fusion]
description: Lorsque vous mappez des éléments, vous pouvez utiliser des fonctions pour créer des formules simples ou complexes.
author: Becky
feature: Workfront Fusion
exl-id: e64d9b1e-8576-43db-ac29-0d386a482fbc
source-git-commit: d175a3d43f13338661d8b7e1cb79038a36522ff9
workflow-type: tm+mt
source-wordcount: '504'
ht-degree: 10%

---

# Mise en correspondance des éléments à l’aide de fonctions dans [!DNL Adobe Workfront Fusion]

Lorsque vous mappez des éléments, vous pouvez utiliser des fonctions pour créer des formules simples ou complexes. Les fonctions disponibles dans [!DNL Adobe Workfront Fusion] sont similaires aux fonctions d’Excel et de certains langages de programmation :

* Ils évaluent la logique générale, les maths, le texte, les dates et les tableaux.
* Ils vous permettent d’effectuer une logique conditionnelle et des transformations des valeurs d’élément, comme convertir du texte en majuscules, rogner du texte, convertir une date dans un format différent, etc.

Pour plus d’informations, voir [Mappage des informations d’un module à un autre dans Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).


## Conditions d’accès

Pour utiliser les fonctionnalités décrites dans cet article, vous devez disposer des éléments suivants :

<table style="table-layout:auto">

<col>  
 <col>  
 <tbody>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront] plan</td>  
   <td> <p>N’importe quelle</p> </td>  
  </tr>  
  <tr data-mc-conditions="">  
   <td role="rowheader">[!DNL Adobe Workfront] licence</td>  
   <td> <p>Nouvelle : [!UICONTROL Standard]</p><p>Ou</p><p>Actuelle : [!UICONTROL Work] ou licence supérieure</p> </td>  
  </tr>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licence**</td>  
   <td> 
   <p>Actuel : aucune exigence de licence [!DNL Workfront Fusion].</p> 
   <p>Ou</p> 
   <p>Hérité : Tout </p> 
   </td>  
  </tr>  
  <tr>  
   <td role="rowheader">Produit</td>  
   <td> 
   <p>Nouveau :</p> <ul><li>Formule [!UICONTROL Select] ou [!UICONTROL Prime] [!DNL Workfront] : votre entreprise doit acheter [!DNL Adobe Workfront Fusion].</li><li>Plan [!UICONTROL Ultimate] [!DNL Workfront] : [!DNL Workfront Fusion] est inclus.</li></ul> 
   <p>Ou</p> 
   <p>Actuel : votre organisation doit acheter [!DNL Adobe Workfront Fusion].</p> 
   </td>  
  </tr> 
 </tbody>  
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], consultez les [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).


## Onglet Mappage - Aperçu

Pour ouvrir le panneau [!UICONTROL mapping] pour un champ :

1. Cliquez sur **Scénarios** dans le panneau de gauche.
1. Choisissez un scénario.

![](assets/open-functions-bar.png)


### Onglets du panneau de mappage

Vous trouverez ci-dessous des onglets dans le panneau de mappage :

* **Fonctions générales** ![](assets/toolbar-icon-general-function.png) - Voir [Fonctions générales dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/general-functions.md) pour plus d’informations.

* **Fonctions mathématiques** ![](assets/toolbar-icon-math-functions.png) - Voir [Fonctions mathématiques dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/math-functions.md) pour plus d’informations.

* **Fonctions de texte et binaires** ![](assets/toolbar-icon-text&binary-functions.png) - Voir [Fonctions de chaîne dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/string-functions.md) pour plus d’informations.

* **Date et heure** ![](assets/toolbar-icon-date&time-functions.png) - Voir [Fonctions de date et d’heure dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/date-and-time-functions.md) et les articles ci-dessous pour plus d’informations :

   * [Jetons pour le formatage de la date et de l’heure dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-formatting.md)
   * [Jetons pour l’analyse de date et d’heure dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-parsing.md)

* **Fonctions pour l’utilisation de tableaux** ![](assets/toolbar-icon-functions-for-arrays.png) - Voir [Fonctions de tableau dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/array-functions.md) pour plus d’informations.

* **Mapper d’autres fonctions** ![](assets/toolbar-icon-functions-you-map-from-other-modules.png) affiche les éléments que vous pouvez mapper à partir d’autres modules. Cet onglet n’est pas toujours disponible.

![](assets/functions-toolbar-350x189.png)

## Insérer des fonctions dans les champs

Pour insérer une fonction dans un champ :

1. Cliquez sur le nom de la fonction.

   Ou

   Faites glisser la fonction dans le champ.


>[!BEGINSHADEBOX]

**Exemple :** Certains types de données empêchent les utilisateurs de saisir plus d’un certain nombre de caractères. Vous pouvez utiliser la fonction substring pour limiter une valeur à un certain nombre de caractères.

Dans cet exemple, la fonction substring limite le nom du projet à 50 caractères.

![](assets/example-meet-length-restriction-350x184.png)

>[!ENDSHADEBOX]

## Imbrication de fonctions

Vous pouvez imbriquer des fonctions entre elles.

## Utilisation des fonctions [!DNL Google Sheets]

Si [!DNL Workfront Fusion] ne comporte pas de fonction que vous souhaitez utiliser, mais qu&#39;elle est présentée par [!DNL Google Sheets], vous pouvez l&#39;utiliser en procédant comme suit :

1. Dans [!DNL Google Sheets], créez une feuille de calcul vide.
1. Dans [!DNL Workfront Fusion], ouvrez votre scénario.
1. Ajoutez le module **[!DNL Google Sheets]** >**[!UICONTROL Mettre à jour une cellule]** au scénario.

   Pour plus d’informations sur l’ajout d’un module, voir [Ajout d’un module dans un scénario](../../workfront-fusion/scenarios/create-a-scenario.md#add) dans l’article [Création d’un scénario dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. Configurez le module :

   1. Sélectionnez la feuille de calcul nouvellement créée dans le champ **[!UICONTROL Feuille de calcul]** .
   1. Insérez votre formule contenant la ou les fonctions [!DNL Google Sheets] dans le champ **[!UICONTROL Valeur]**.

      Vous pouvez utiliser la sortie des modules précédents comme vous le faites habituellement.

      ![](assets/exploit-google-sheet-functions-350x218.png)

1. Insérez le module **[!UICONTROL Google Sheets] >[!UICONTROL Get a cell]** pour obtenir le résultat calculé.
1. Configurez le module à l’aide du même identifiant de cellule que celui utilisé à l’étape 4.

   ![](assets/exploit-google-sheet-functions-2-350x187.png)
