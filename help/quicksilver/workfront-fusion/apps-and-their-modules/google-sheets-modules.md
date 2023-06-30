---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: connector
navigation-topic: apps-and-their-modules
title: Modules Google Sheets
description: Pour utiliser [!DNL Google Sheets] avec [!DNL Adobe Workfront Fusion],you need the [!UICONTROL Workfront Fusion Google Sheets] extension (facultative, mais requise pour les déclencheurs instantanés).
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 11d62222-df34-472d-93d7-f0d53eb95c9b
source-git-commit: 6f4e5042054f3936fa0e387bfbebaa1775d16573
workflow-type: tm+mt
source-wordcount: '3941'
ht-degree: 0%

---

# [!DNL Google Sheets] modules

Dans un [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les workflows qui utilisent [!DNL Google Sheets], ainsi que de la connecter à plusieurs applications et services tiers.

Pour obtenir des instructions sur la connexion à [!DNL Google Sheets] compte à [!DNL Workfront Fusion], voir [Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base](../../workfront-fusion/connections/connect-to-fusion-general.md)

## Exigences d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
  <td> <p>[!UICONTROL Pro] ou version ultérieure</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
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

## Conditions préalables

Pour utiliser [!UICONTROL Google Sheets] modules, vous devez disposer d’un [!UICONTROL Google] compte .

## Triggers

### [!UICONTROL Lignes de contrôle]

Récupère les valeurs de chaque ligne nouvellement ajoutée dans la feuille de calcul.

Le module récupère uniquement les nouvelles lignes qui n’ont pas été remplies auparavant. Le déclencheur ne traite pas une ligne remplacée.

>[!IMPORTANT]
>
>Si la feuille de calcul contient une ligne vierge, aucune ligne après la ligne vierge ne sera traitée.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Google Sheets] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connectez l’application ou le service Web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Feuille de calcul] </td> 
   <td> <p>Sélectionnez la feuille de calcul qui contient la feuille à regarder.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Feuille] </td> 
   <td> <p>Sélectionnez la feuille à surveiller pour une nouvelle ligne.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Table contient des en-têtes]</td> 
   <td> <p> Indiquez si la feuille de calcul contient la rangée d’en-tête.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Oui]</strong> </p> <p>Le module ne récupère pas la ligne d’en-tête comme données de sortie. </p> <p>Les noms de variables dans la sortie sont appelés par les en-têtes.</p> </li> 
     <li> <p><strong>[!UICONTROL No]</strong> </p> <p>Le module récupère également la première ligne du tableau.</p> <p>Les noms de variables dans la sortie sont appelés A, B, C, D, etc.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Rangée avec en-têtes] </td> 
   <td> <p>Entrez la plage de la ligne d’en-tête. Par exemple, <code>A1:F1</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Première ligne de tableau]</td> 
   <td> <p>Entrez la plage de la première ligne du tableau. Par exemple, <code>A1:F1</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Option de rendu de valeur]</p> </td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Valeur formatée]</p> <p>Les valeurs seront calculées et formatées dans la réponse selon le formatage de la cellule. Le formatage est basé sur les paramètres régionaux de la feuille de calcul et non sur ceux de l’utilisateur qui la demande. Par exemple, si <code>A1</code> is <code>1.23</code> et <code>A2</code> is <code>=A1</code> et formaté en tant que devise, puis <code>A2</code> serait renvoyé <code>"$1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL Valeur non formatée]</p> <p>Les valeurs seront calculées, mais pas formatées dans la réponse. Par exemple, si <code>A1</code> is <code>1.23</code> et <code>A2</code> is <code>=A1</code> et formaté en tant que devise, puis <code>A2</code> renvoie le nombre. <code>"1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL Formule]</p> <p>Les valeurs ne seront pas calculées. La réponse comportera les formules. Par exemple, si <code>A1</code> is <code>1.23</code> et <code>A2</code> is <code>=A1</code> et formaté en tant que devise, puis <code>A2</code> serait renvoyé <code>"=A1"</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Option de rendu de date et d’heure]</p> </td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Numéro de série]</p> <p>Indique la date, l’heure, la date et l’heure ainsi que les champs de durée à produire en double au format "numéro de série", tel que popularisé par Lotus 1-2-3. La partie numérique de la valeur (à gauche de la décimale) compte les jours depuis le 30 décembre 1899. La partie fractionnaire (à droite de la décimale) comptabilise l’heure comme une fraction du jour. Par exemple, le 1er janvier 1900 à midi serait de 2,5, 2 parce qu'il est 2 jours après le 30 décembre 1899 et 0,5 parce que midi est une demi-journée. Le 1er février 1900 à 15h00 aura 33.625. L'année 1900 n'est donc pas une année bissextile.</p> <p style="font-weight: bold;">[!UICONTROL Chaîne formatée]</p> <p>Indique les champs Date, Heure, Date et Heure et Durée à générer sous la forme de chaînes dans leur format de nombre donné (qui dépend des paramètres régionaux de la feuille de calcul).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite] </td> 
   <td> <p>Définissez le nombre maximal de résultats qui [!DNL Workfront Fusion] fonctionnera pendant un cycle d’exécution.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Actions

* [[!UICONTROL Ajouter une ligne]](#add-a-row)
* [[!UICONTROL Mettre à jour une ligne]](#update-a-row)
* [[!UICONTROL Effacement d’une ligne]](#clear-a-row)
* [[!UICONTROL Supprimer une ligne]](#delete-a-row)
* [[!UICONTROL Obtention d’une cellule]](#get-a-cell)
* [[!UICONTROL Mettre à jour une cellule]](#update-a-cell)
* [[!UICONTROL Effacement d’une cellule]](#clear-a-cell)
* [[!UICONTROL Ajouter une feuille]](#add-a-sheet)
* [[!UICONTROL Création d’une feuille de calcul]](#create-a-spreadsheet)
* [[!UICONTROL Suppression d’une feuille]](#delete-a-sheet)
* [[!UICONTROL Lancer un appel API]](#make-an-api-call)

### [!UICONTROL Ajouter une ligne]

Ce module ajoute une ligne à une feuille.

Lorsque vous configurez [!DNL Google Sheets] modules, [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. En plus de ces [!DNL Google Sheets] peut s’afficher, selon des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, voir [Mappage des informations d’un module à un autre dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Google Sheets] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connectez l’application ou le service Web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Mode]</td> 
   <td> <p>Indiquez si vous souhaitez sélectionner manuellement la feuille de calcul et la feuille de calcul ou par mappage.</p> <p>Remarque : La mise en correspondance manuelle s’avère utile, par exemple, lorsqu’une nouvelle feuille de calcul est créée dans une [!DNL Workfront Fusion] et vous souhaitez ajouter des données dans la feuille de calcul nouvellement créée directement dans le scénario.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Feuille de calcul] </td> 
   <td> <p>Sélectionnez la [!DNL Google] feuille de calcul.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Feuille] </td> 
   <td> <p>Sélectionnez la feuille à laquelle vous souhaitez ajouter une rangée.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Plage des colonnes]</td> 
   <td>Sélectionnez la plage de colonnes à utiliser.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Table contient des en-têtes]</td> 
   <td> <p> Indiquez si la feuille de calcul contient la rangée d’en-tête.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Oui]</strong> </p> <p>Le module ne récupère pas la ligne d’en-tête comme données de sortie. </p> <p>Les noms de variables dans la sortie sont appelés par les en-têtes.</p> </li> 
     <li> <p><strong>[!UICONTROL No]</strong> </p> <p>Le module récupère également la première ligne du tableau.</p> <p>Les noms de variables dans la sortie sont appelés A, B, C, D, etc.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Values] </td> 
   <td> <p>Entrez ou mappez les cellules de votre choix dans la ligne à ajouter.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Option de saisie de valeur]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL Utilisateur saisi]</strong></p> <p>Les valeurs sont analysées comme si l’utilisateur les avait saisies dans l’interface utilisateur. Les nombres restent des nombres, mais les chaînes peuvent être converties en nombres, dates ou autres formats suivant les mêmes règles que celles appliquées lors de la saisie de texte dans une cellule via le [!DNL Google Sheets] Interface utilisateur.</p> </li> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p> Les valeurs saisies par l’utilisateur ne sont pas analysées et sont stockées en l’état. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Option d’insertion de données]</td> 
   <td> <p>Indiquez le mode de modification des données existantes lors de la saisie de nouvelles données. </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Insérer des lignes]</strong></p> <p>Des lignes sont insérées pour les nouvelles données.</p> </li> 
     <li> <p><strong>[!UICONTROL Remplacer]</strong> </p> <p>Les nouvelles données remplacent les données existantes dans les zones où elles sont écrites. L’ajout de données à la fin de la feuille insère de nouvelles lignes ou colonnes afin que les données puissent être écrites.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Mettre à jour une ligne]

Ce module permet de modifier le contenu de la cellule dans une ligne sélectionnée.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Google Sheets] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connectez l’application ou le service Web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Mode]</td> 
   <td> <p>Indiquez si vous souhaitez sélectionner manuellement la feuille de calcul et la feuille de calcul ou par mappage.</p> <p>Remarque : Le mappage manuel est utile, par exemple, lorsqu’une nouvelle feuille de calcul est créée dans le scénario [!UICONTROL Workfront Fusion] et que vous souhaitez ajouter des données à la nouvelle feuille de calcul directement dans le scénario.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Feuille de calcul] </td> 
   <td> <p>Sélectionnez la [!DNL Google] feuille de calcul.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Feuille] </td> 
   <td> <p>Sélectionnez la feuille dans laquelle vous souhaitez mettre à jour une ligne.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Numéro de ligne]</td> 
   <td> <p> Saisissez le nombre de lignes à mettre à jour.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Table contient des en-têtes]</td> 
   <td> <p> Indiquez si la feuille de calcul contient la rangée d’en-tête.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Oui]</strong> </p> <p>Le module ne récupère pas la ligne d’en-tête comme données de sortie. </p> <p>Les noms de variables dans la sortie sont appelés par les en-têtes.</p> </li> 
     <li> <p><strong>[!UICONTROL No]</strong> </p> <p>Le module récupère également la première ligne du tableau.</p> <p>Les noms de variables dans la sortie sont appelés A, B, C, D, etc.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Values] </td> 
   <td> <p>Entrez ou mappez les valeurs dans les cellules de votre choix de la ligne à modifier (mise à jour).</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Option de saisie de valeur]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL Utilisateur saisi]</strong></p> <p>Les valeurs sont analysées comme si l’utilisateur les avait saisies dans l’interface utilisateur. Les nombres restent des nombres, mais les chaînes peuvent être converties en nombres, dates ou autres formats suivant les mêmes règles que celles appliquées lors de la saisie de texte dans une cellule via le [!DNL Google Sheets] Interface utilisateur.</p> </li> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p> Les valeurs saisies par l’utilisateur ne sont pas analysées et sont stockées en l’état. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Effacement d’une ligne]

Supprime les valeurs d’une ligne spécifiée.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Google Sheets] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connectez l’application ou le service Web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Feuille de calcul] </td> 
   <td> <p>Sélectionnez la [!DNL Google] feuille de calcul contenant la feuille dont vous souhaitez supprimer une ligne.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Feuille] </td> 
   <td> <p> Sélectionnez la feuille à partir de laquelle vous souhaitez effacer les données.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Numéro de ligne]</td> 
   <td> <p>Saisissez le nombre de lignes à partir desquelles vous souhaitez effacer les données. Par exemple, <code> 23</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Supprimer une ligne]

Supprime une ligne spécifiée.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Google Sheets] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connectez l’application ou le service Web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Feuille de calcul] </td> 
   <td> <p>Sélectionnez la feuille de calcul Google contenant la feuille à partir de laquelle vous souhaitez supprimer une ligne.</p> </td> 
  </tr> 
  <tr> 
   <td>Feuille </td> 
   <td> <p>Sélectionnez la feuille dans laquelle vous souhaitez supprimer une ligne.</p> </td> 
  </tr> 
  <tr> 
   <td>Numéro de ligne</td> 
   <td> <p>Saisissez le nombre de lignes à supprimer. Exemple: <code>23</code></p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Obtention d’une cellule]

Récupère une valeur d’une cellule sélectionnée.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Google Sheets] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connectez l’application ou le service Web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Feuille de calcul] </td> 
   <td> <p>Sélectionnez la [!DNL Google] feuille de calcul.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Feuille] </td> 
   <td> <p>Sélectionnez la feuille contenant la cellule à partir de laquelle vous souhaitez récupérer les données.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cell] </td> 
   <td> <p>Saisissez l’identifiant de la cellule à partir de laquelle vous souhaitez récupérer les données. Exemple: <code>A6</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Option de rendu de valeur]</td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Valeur formatée]</p> <p>Les valeurs seront calculées et formatées dans la réponse selon le formatage de la cellule. Le formatage est basé sur les paramètres régionaux de la feuille de calcul et non sur ceux de l’utilisateur qui la demande. Par exemple, si <code>A1</code> is <code>1.23</code> et <code>A2</code> is <code>=A1</code> et formaté en tant que devise, puis <code>A2</code> serait renvoyé <code>"$1.23"</code>.</p> <p style="font-weight: bold;">[!DNL Unformatted value]</p> <p>Les valeurs seront calculées, mais pas formatées dans la réponse. Par exemple, si <code>A1</code> is <code>1.23</code> et <code>A2</code> is <code>=A1</code> et formaté en tant que devise, puis <code>A2</code> renvoie le nombre. <code>"1.23"</code>.</p> <p style="font-weight: bold;">[!DNL Formula]</p> <p>Les valeurs ne seront pas calculées. La réponse comportera les formules. Par exemple, si <code>A1</code> is <code>1.23</code> et <code>A2</code> is <code>=A1</code> et formaté en tant que devise, puis <code>A2</code> serait renvoyé <code>"=A1"</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!DNL Date and time render option]</td> 
   <td> <p style="font-weight: bold;">[!DNL Serial number]</p> <p>Indique la date, l’heure, la date et l’heure ainsi que les champs de durée à produire en double au format "numéro de série", tel que popularisé par Lotus 1-2-3. La partie numérique de la valeur (à gauche de la décimale) compte les jours depuis le 30 décembre 1899. La partie fractionnaire (à droite de la décimale) comptabilise l’heure comme une fraction du jour. Par exemple, le 1er janvier 1900 à midi serait de 2,5, 2 parce qu'il est 2 jours après le 30 décembre 1899 et 0,5 parce que midi est une demi-journée. Le 1er février 1900 à 15h00 aura 33.625. L'année 1900 n'est donc pas une année bissextile.</p> <p style="font-weight: bold;">[!DNL Formatted string]</p> <p>Indique les champs Date, Heure, Date et Heure et Durée à générer sous la forme de chaînes dans leur format de nombre donné (qui dépend des paramètres régionaux de la feuille de calcul).</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Mettre à jour une cellule]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Google Sheets] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connectez l’application ou le service Web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Feuille de calcul] </td> 
   <td> <p>Sélectionnez la [!DNL Google] feuille de calcul.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cell] </td> 
   <td> <p>Saisissez l’identifiant de la cellule que vous souhaitez mettre à jour. Exemple: <code>A5</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Value]</td> 
   <td> <p>Entrez la nouvelle valeur de la cellule.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Option de saisie de valeur]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL Utilisateur saisi]</strong></p> <p>Les valeurs sont analysées comme si l’utilisateur les avait saisies dans l’interface utilisateur. Les nombres restent des nombres, mais les chaînes peuvent être converties en nombres, dates ou autres formats suivant les mêmes règles que celles appliquées lors de la saisie de texte dans une cellule via le [!DNL Google Sheets] Interface utilisateur.</p> </li> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p> Les valeurs saisies par l’utilisateur ne sont pas analysées et sont stockées en l’état. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Effacement d’une cellule]

Supprime une valeur d’une cellule spécifiée.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Google Sheets] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connectez l’application ou le service Web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Feuille de calcul] </td> 
   <td> <p>Sélectionnez la feuille de calcul Google contenant la feuille à partir de laquelle vous souhaitez effacer une cellule.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Feuille] </td> 
   <td> <p>Sélectionnez la feuille à partir de laquelle vous souhaitez effacer une cellule.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cell] </td> 
   <td> <p>Saisissez l’identifiant de la cellule à effacer. Exemple: <code>A5</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Ajouter une feuille]

Crée une feuille dans une feuille de calcul sélectionnée.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Google Sheets] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connectez l’application ou le service Web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Feuille de calcul] </td> 
   <td> <p>Sélectionnez la feuille de calcul Google dans laquelle vous souhaitez ajouter une feuille.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Propriétés]</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">[!UICONTROL Title]</p> <p>Saisissez le nom de la nouvelle feuille.</p> </li> 
     <li> <p style="font-weight: bold;">[!UICONTROL Index]</p> <p>Saisissez la position de la feuille. La valeur par défaut est 0 (place la feuille en premier lieu).</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Création d’une feuille de calcul]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Google Sheets] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connectez l’application ou le service Web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Title] </td> 
   <td> <p>Saisissez le nom d’une nouvelle feuille de calcul.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Locale]</td> 
   <td> <p>Saisissez les paramètres régionaux de la feuille de calcul dans l’un des formats suivants :</p> 
    <ul> 
     <li>un code de langue ISO 639-1 tel que <code>en</code></li> 
     <li>un code de langue ISO 639-2 tel que <code>haw</code>, si aucun code 639-1 n’existe</li> 
     <li>une combinaison du code de langue ISO et du code de pays, telle que <code>en_US</code></li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Intervalle de recalcul]</td> 
   <td> <p>Le temps d’attente avant que les fonctions volatiles ne soient recalculées :</p> <p style="font-weight: bold;">[!UICONTROL En cas de modification]</p> <p>Les fonctions variables sont mises à jour à chaque modification.</p> <p style="font-weight: bold;">[!UICONTROL À la modification et toutes les minutes]</p> <p>Les fonctions variables sont mises à jour à chaque modification et chaque minute.</p> <p style="font-weight: bold;">[!UICONTROL Au changement et toutes les heures]</p> <p>Les fonctions variables sont mises à jour à chaque modification et toutes les heures.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fuseau horaire]</td> 
   <td> <p> Sélectionnez le fuseau horaire de la feuille de calcul.</p> </td> 
  </tr> 
  <tr> 
   <td>Format [!UICONTROL Number]</td> 
   <td> <p>Sélectionnez le format par défaut de toutes les cellules de la feuille de calcul.</p> <p><strong>[!UICONTROL Texte]</strong>: Formatage du texte. Exemple: <code>1000. 12</code></p> <p><strong>[!UICONTROL Number]</strong>: Formatage des nombres. Exemple: <code>1,000.12</code></p> <p><strong>[!UICONTROL Pourcentage]</strong>: Pourcentage de mise en forme. Exemple: <code>10. 12%</code></p> <p><strong>[!UICONTROL Currency]</strong>: Mise en forme des devises. Exemple: <code>$1,000.12</code></p> <p><strong>[!UICONTROL Date]</strong>: Formatage des dates. Exemple: <code>9/26/2008</code></p> <p><strong>[!UICONTROL Time]</strong>: Formatage de l’heure. Exemple: <code>3:59:00 PM</code></p> <p><strong>[!UICONTROL Date et heure]</strong>: Formatage des dates et heures. Exemple: <code>9/26/08 15:59:00</code> </p> <p><strong>[!UICONTROL Scientific]</strong>Formatage scientifique des nombres. Exemple: <code>1. 01E+03</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sheets] </td> 
   <td> <p>Cliquez sur <strong>[!UICONTROL Ajouter]</strong> pour ajouter une feuille à la feuille de calcul. Pour chaque feuille, saisissez ou mappez un titre pour la feuille et l’index de la feuille. Un index de 0 représente la première feuille.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Suppression d’une feuille]

Supprime une feuille spécifique.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Google Sheets] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connectez l’application ou le service Web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Feuille de calcul] </td> 
   <td> <p>Sélectionnez la [!DNL Google] feuille de calcul.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Feuille] </td> 
   <td> <p>Sélectionnez la feuille à supprimer.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Lancer un appel API]

Ce module d’action vous permet d’effectuer un appel API personnalisé.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [Fusion App] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td>Saisissez un chemin relatif à <code>https://sheets.googleapis.com/v4/</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Méthode [!UICONTROL]</p> </td> 
   <td> <p>Sélectionnez la méthode de requête HTTP dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Ajoutez les en-têtes de la requête sous la forme d’un objet JSON standard. Par exemple : <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] ajoute les en-têtes d’autorisation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p> Ajoutez la requête pour l’appel API sous la forme d’un objet JSON standard.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard.</p> <p>Note:   <p>Lorsque vous utilisez des instructions conditionnelles telles que <code>if</code> dans votre fichier JSON, placez les guillemets en dehors de l’instruction conditionnelle.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

## Recherches

* [[!UICONTROL Lignes de recherche]](#search-rows)
* [[!UICONTROL Lignes de recherche (avancées)]](#search-rows-advanced)
* [[!UICONTROL Obtenir les valeurs de plage]](#get-range-values)
* [[!UICONTROL Feuilles de liste]](#list-sheets)

### [!UICONTROL Lignes de recherche]

Recherche les lignes à l’aide des options de filtre.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [Fusion App] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Feuille de calcul] </td> 
   <td> <p>Sélectionnez la [!DNL Google] feuille de calcul.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Feuille] </td> 
   <td> <p>Sélectionnez la feuille dans laquelle vous souhaitez rechercher les lignes.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Table contient des en-têtes]</td> 
   <td> <p> Indiquez si la feuille de calcul contient la rangée d’en-tête. Si l’option [!UICONTROL Oui] est sélectionnée, le module ne récupère pas la ligne d’en-tête, car les données de sortie et les noms de variable dans la sortie sont alors appelés par les en-têtes. Si l’option [!UICONTROL Non] est sélectionnée, le module récupère également la première ligne de tableau et les noms de variable dans la sortie sont alors appelés uniquement A, B, C, D, etc.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Plage des colonnes]</td> 
   <td>Sélectionnez la plage de colonnes à utiliser. Exemple: <code>A-F</code></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Filter]</td> 
   <td> <p>Définissez le filtre correspondant à la ligne à rechercher.</p> <p>Pour plus d’informations sur les filtres, voir <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">Ajouter un filtre à un scénario dans [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordre de tri]</td> 
   <td>Indiquez si vous souhaitez trier par ordre croissant ou décroissant.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordre par]</td> 
   <td>Sélectionnez la colonne à trier.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Option de rendu de valeur]</td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Valeur formatée]</p> <p>Les valeurs seront calculées et formatées dans la réponse selon le formatage de la cellule. Le formatage est basé sur les paramètres régionaux de la feuille de calcul et non sur ceux de l’utilisateur qui la demande. Par exemple, si <code>A1</code> is <code>1.23</code> et <code>A2</code> is <code>=A1</code> et formaté en tant que devise, puis <code>A2</code> serait renvoyé <code>"$1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL Valeur non formatée]</p> <p>Les valeurs seront calculées, mais pas formatées dans la réponse. Par exemple, si <code>A1</code> is <code>1.23</code> et <code>A2</code> is <code>=A1</code> et formaté en tant que devise, puis <code>A2</code> renvoie le nombre. <code>"1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL Formule]</p> <p>Les valeurs ne seront pas calculées. La réponse comportera les formules. Par exemple, si <code>A1</code> is <code>1.23</code> et <code>A2</code> is <code>=A1</code> et formaté en tant que devise, puis <code>A2</code> serait renvoyé <code>"=A1"</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Option de rendu de date et d’heure]</td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Numéro de série]</p> <p>Indique la date, l’heure, la date et l’heure ainsi que les champs de durée à générer en double au format "numéro de série", tel que popularisé par Lotus 1-2-3. La partie numérique de la valeur (à gauche de la décimale) compte les jours depuis le 30 décembre 1899. La partie fractionnaire (à droite de la décimale) comptabilise l’heure comme une fraction du jour. Par exemple, le 1er janvier 1900 à midi serait de 2,5, 2 parce qu'il est 2 jours après le 30 décembre 1899 et 0,5 parce que midi est une demi-journée. Le 1er février 1900 à 15h00 aura 33.625. L'année 1900 n'est donc pas une année bissextile.</p> <p style="font-weight: bold;">[!UICONTROL Chaîne formatée]</p> <p>Indique les champs Date, Heure, Date et Heure et Durée à générer sous la forme de chaînes dans leur format de nombre donné (qui dépend des paramètres régionaux de la feuille de calcul).</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nombre maximal de lignes renvoyées]</td> 
   <td>Définissez le nombre maximal de lignes qui [!DNL Workfront Fusion] renverra pendant un cycle d'exécution.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Lignes de recherche (avancées)]

Renvoie des résultats correspondant aux critères donnés.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Google Sheets] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connectez l’application ou le service Web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Feuille de calcul] </td> 
   <td> <p>Sélectionnez la feuille de calcul Google contenant la feuille à rechercher.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Feuille] </td> 
   <td> <p>Sélectionnez la feuille contenant les lignes à rechercher.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Query]</td> 
   <td> <p>Utilisez la variable [!DNL Google Charts Query Language]. Exemple: <code>select * where B = "John"</code></p> <p>Pour plus d’informations sur [!DNL Google Charts Query Language], voir <a href="https://developers.google.com/chart/interactive/docs/querylanguage">Référence du langage de requête</a> dans le [!DNL Google] documentation.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Obtenir les valeurs de plage]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Google Sheets] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connectez l’application ou le service Web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Feuille de calcul] </td> 
   <td> <p>Sélectionnez la [!DNL Google] feuille de calcul.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Feuille] </td> 
   <td> <p>Sélectionnez la feuille à partir de laquelle vous souhaitez obtenir le contenu de la plage.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Range] </td> 
   <td> <p>Entrez la plage que vous souhaitez obtenir. Exemple: <code>A1:D25</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Table contient des en-têtes]</td> 
   <td> <p>Cochez cette case si la feuille comporte une rangée d’en-tête.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Rangée avec en-têtes]</td> 
   <td>Saisissez la plage des en-têtes du tableau. Exemple <code>A1:F1</code>. Si vous laissez le champ vide, [!DNL Workfront Fusion] supposons que l’en-tête se trouve dans la première ligne de la plage spécifiée.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Option de rendu de valeur]</td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Valeur formatée]</p> <p>Les valeurs seront calculées et formatées dans la réponse selon le formatage de la cellule. Le formatage est basé sur les paramètres régionaux de la feuille de calcul et non sur ceux de l’utilisateur qui la demande. Par exemple, si <code>A1</code> is <code>1.23</code> et <code>A2</code> is <code>=A1</code> et formaté en tant que devise, puis <code>A2</code> serait renvoyé <code>"$1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL Valeur non formatée]</p> <p>Les valeurs seront calculées, mais pas formatées dans la réponse. Par exemple, si <code>A1</code> is <code>1.23</code> et <code>A2</code> is <code>=A1</code> et formaté en tant que devise, puis <code>A2</code> renvoie le nombre. <code>"1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL Formule]</p> <p>Les valeurs ne seront pas calculées. La réponse comportera les formules. Par exemple, si <code>A1</code> is <code>1.23</code> et <code>A2</code> is <code>=A1</code> et formaté en tant que devise, puis <code>A2</code> serait renvoyé <code>"=A1"</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Option de rendu de date et d’heure]</td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Numéro de série]</p> <p>Indique la date, l’heure, la date et l’heure ainsi que les champs de durée à générer en double au format "numéro de série", tel que popularisé par Lotus 1-2-3. La partie numérique de la valeur (à gauche de la décimale) compte les jours depuis le 30 décembre 1899. La partie fractionnaire (à droite de la décimale) comptabilise l’heure comme une fraction du jour. Par exemple, le 1er janvier 1900 à midi serait de 2,5, 2 parce qu'il est 2 jours après le 30 décembre 1899 et 0,5 parce que midi est une demi-journée. Le 1er février 1900 à 15h00 aura 33.625. L'année 1900 n'est donc pas une année bissextile.</p> <p style="font-weight: bold;">[!UICONTROL Chaîne formatée]</p> <p>Indique les champs Date, Heure, Date et Heure et Durée à générer sous la forme de chaînes dans leur format de nombre donné (qui dépend des paramètres régionaux de la feuille de calcul).</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Feuilles de liste]

Ce module renvoie une liste de toutes les feuilles d’une feuille de calcul.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Google Sheets] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connectez l’application ou le service Web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Feuille de calcul] </td> 
   <td> <p>Sélectionnez la [!DNL Google] feuille de calcul contenant les feuilles que vous souhaitez répertorier.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Limites d’utilisation

Si l’erreur `429: RESOURCE_EXHAUSTED` , vous avez dépassé la limite de débit de l’API.

Le [!DNL Google Sheets] L’API est limitée à 500 demandes par 100 secondes par projet et à 100 demandes par 100 secondes par utilisateur. Les limites des lectures et écritures sont suivies séparément. Il n’y a pas de limite d’utilisation quotidienne.

Pour plus d’informations, voir [developers.google.com/sheets/api/limits](https://developers.google.com/sheets/api/limits).

## Conseils et astuces

* [Comment obtenir des cellules vides à partir d’un [!DNL Google] Feuille](#how-to-get-empty-cells-from-a-google-sheet)
* [Ajouter un bouton dans une feuille pour exécuter un scénario](#add-a-button-in-a-sheet-to-run-a-scenario)

### Comment obtenir des cellules vides à partir d’un [!DNL Google Sheet]

Utilisez la variable [!UICONTROL Lignes de recherche (avancées)] et utiliser cette formule pour obtenir les colonnes vides.
<pre>select * where E is null</pre>Ici "E" est la colonne et "is null" est la condition. Vous pouvez créer une requête plus avancée à l’aide de [Google Query Lang](https://developers.google.com/chart/interactive/docs/querylanguage).

### Ajouter un bouton dans une feuille pour exécuter un scénario

1. Dans [!DNL Workfront Fusion], insérez la variable **[!UICONTROL Webhook]** > **[!UICONTROL Webhooks personnalisés]** module/déclencheur dans le scénario et configurez-le (voir [Webhooks](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md)).

1. Copiez l’URL du webhook.
1. Exécutez le scénario.
1. Dans les feuilles de calcul Google Sheets, choisissez **[!UICONTROL Insérer]** > **[!UICONTROL Dessin]**... dans la barre de menus principale.

1. Dans le [!UICONTROL Dessin] , cliquez sur le bouton **[!UICONTROL Zone de texte]** icon ![](assets/text-box.png) près du haut de la fenêtre.
1. Concevez un bouton et cliquez sur le bouton **[!UICONTROL Enregistrer et fermer]** dans le coin supérieur droit :
1. Le bouton sera placé dans votre feuille de calcul. Cliquez sur les trois points verticaux dans le coin supérieur droit du bouton :
1. Choisir **[!UICONTROL Attribuer un script..].** dans le menu.
1. Saisissez le nom de votre script (fonction), par exemple : `runScenario` et cliquez sur **[!UICONTROL OK]**:
1. Choisir **[!UICONTROL Outils]** > **[!UICONTROL Editeur de script]** dans la barre de menus principale.

1. Insérez le code suivant :

   * Le nom de la fonction doit correspondre au nom que vous avez spécifié à l’étape 9.
   * Remplacez l’URL par l’URL du webhook que vous avez copiée à l’étape 2.

     <pre>function runScenario() {</pre><pre>UrlFetchApp.fetch("<webhook you copied>");</pre><pre>}</pre>

1. Press **[!UICONTROL Ctrl+S]** pour enregistrer le fichier de script, saisissez un nom de projet, puis cliquez sur **[!UICONTROL OK]**.

1. Revenir à [!DNL Google Sheets] et cliquez sur le nouveau bouton.
1. Octroyez l’autorisation requise au script :
1. Dans [!DNL Workfront Fusion], vérifiez que le scénario a bien été exécuté.

## Stockage des dates dans une feuille de calcul

Si vous stockez une valeur Date dans une feuille de calcul sans mise en forme, elle apparaît dans la feuille de calcul au format texte au format ISO 8601. Cependant, [!DNL Google Sheets] formules ou fonctions qui fonctionnent avec des dates qui ne comprennent pas ce texte (exemple : formule `=A1+10`) affiche l’erreur suivante :

![](assets/mceclip6-350x87.png)

Pour autoriser [!DNL Google Sheets] pour comprendre la date, formatez-la avec la fonction [[!UICONTROL formatDate] (date; format ; [fuseau horaire])](../../workfront-fusion/functions/date-and-time-functions.md#formatda) fonction . Le format correct transmis à la fonction comme second argument dépend des paramètres régionaux de la feuille de calcul.

Pour déterminer le format correct :

1. Choisir **[!UICONTROL Fichier]** > **[!UICONTROL Feuille de calcul]** dans le menu principal pour vérifier/définir les paramètres régionaux.

1. Une fois que vous avez vérifié/défini les paramètres régionaux appropriés, déterminez le format de date et d’heure correspondant en choisissant **[!UICONTROL Format]** > **[!UICONTROL Nombre]** dans le menu principal. Le format s’affiche en regard de l’option de menu Date et heure :

1. Pour composer le format correct qui doit être transmis au [!UICONTROL formatDate()] fonction, voir la liste des [Jetons pour le formatage de la date et de l’heure dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-formatting.md).

**Exemple :** L’utilisation de `MM/DD/YYYY HH:mm:ss` format des paramètres régionaux des États-Unis :

![](assets/locale-time-350x83.png)

## Exploiter [!DNL Google Sheets] fonctions

Si une fonction intégrée vous manque, mais qu’elle est présentée par [!DNL Google Sheets], vous pouvez l’exploiter. Pour plus d’informations, voir [Utilisation [!DNL Google Sheets] fonctions](../../workfront-fusion/functions/map-using-functions.md#exploiti) in [Mise en correspondance des éléments à l’aide de fonctions dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/map-using-functions.md) .

## Conserver [!DNL Google Sheets] de la modification des nombres en dates

Il se peut qu’une chaîne de nombres que vous utilisez comme texte soit interprétée comme une date dans une variable [!DNL Google] de la feuille de calcul. Par exemple, saisissez 1-2019, dans l’intention de le définir comme texte, mais Google l’interprète comme une date. Pour éviter cela, vous pouvez pré-formater le nombre en texte brut.

1. Dans [!DNL Google Sheets], mettez en surbrillance la colonne ou la cellule contenant le nombre ou les nombres.
1. Cliquez sur **[!UICONTROL Format]** > **[!UICONTROL Nombre]** > **[!UICONTROL Texte brut]**.

Autre solution de contournement dans [!DNL Workfront Fusion] est de saisir une apostrophe (’) avant un nombre, par exemple &quot;1-2019&quot; ou &quot;1/47&quot;. L’apostrophe ne s’affiche pas dans la cellule une fois les données envoyées à partir de [!DNL Workfront Fusion].
