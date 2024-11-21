---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: connecteur
navigation-topic: apps-and-their-modules
title: Modules Google Sheets
description: Pour utiliser  [!DNL Google Sheets]  avec l’extension  [!DNL Adobe Workfront Fusion],you need the [!UICONTROL Workfront Fusion Google Sheets]  (facultative, mais requise pour les déclencheurs instantanés).
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 11d62222-df34-472d-93d7-f0d53eb95c9b
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '4023'
ht-degree: 97%

---

# Modules [!DNL Google Sheets]

Dans un scénario [!DNL Adobe Workfront Fusion], vous pouvez automatiser les workflows qui utilisent [!DNL Google Sheets] et le connecter à plusieurs applications et services tiers.

Pour savoir comment connecter votre compte [!DNL Google Sheets] à [!DNL Workfront Fusion], voir la section [Créer une connexion à  [!DNL Adobe Workfront Fusion]  - Instructions de base](../../workfront-fusion/connections/connect-to-fusion-general.md).

## Conditions d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] formule*</td>
  <td> <p>[!UICONTROL Pro] ou version supérieure</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licence**</td> 
   <td>
   <p>Exigences de licence actuelles : aucune exigence de licence [!DNL Workfront Fusion] requise.</p>
   <p>Ou</p>
   <p>Exigences de licence héritées : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Exigences actuelles du produit : si vous avez le plan [!UICONTROL Select] ou [!UICONTROL Prime] [!DNL Adobe Workfront], votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article. [!DNL Workfront Fusion] est inclus dans la formule [!DNL Workfront] [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Exigences liées aux produits hérités : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi qu’[!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez votre équipe d’administration [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], voir Licences [[!DNL Adobe Workfront Fusion] ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Conditions préalables

Pour utiliser les modules [!UICONTROL Google Sheets], vous devez avoir un compte [!UICONTROL Google].

## Informations sur l’API Google Sheets

Le connecteur Google Sheets utilise les éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">URL de base</td> 
   <td> https://sheets.googleapis.com/v4</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Version de l’API</td> 
   <td> v4 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Balise API</td> 
   <td>v2.5.7</td> 
  </tr>
 </tbody> 
 </table>

## Déclencheurs

### [!UICONTROL Surveiller les lignes]

Récupère les valeurs de chaque ligne nouvellement ajoutée dans la feuille de calcul.

Le module récupère uniquement les nouvelles lignes qui n’ont pas été remplies auparavant. Le déclencheur ne traite pas une ligne remplacée.

>[!IMPORTANT]
>
>Si la feuille de calcul contient une ligne vide, aucune ligne après la ligne vide ne sera traitée.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Google Sheets] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connecter l’application ou le service web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Créer un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Spreadsheet] </td> 
   <td> <p>Sélectionnez la feuille de calcul qui contient la feuille à surveiller.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sheet] </td> 
   <td> <p>Sélectionnez la feuille dans laquelle vous souhaitez surveiller l’ajout d’une ligne.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Table contains headers]</td> 
   <td> <p> Indiquez si la feuille de calcul contient la ligne d’en-tête.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Yes]</strong> </p> <p>Le module ne récupère pas la ligne d’en-tête comme données de sortie. </p> <p>Les noms de variables dans la sortie sont appelés par les en-têtes.</p> </li> 
     <li> <p><strong>[!UICONTROL No]</strong> </p> <p>Le module récupère également la première ligne du tableau.</p> <p>Les noms de variables dans la sortie sont appelés A, B, C, D, etc.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Row with headers] </td> 
   <td> <p>Saisissez la plage de la ligne d’en-tête. Par exemple, <code>A1:F1</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL First table row]</td> 
   <td> <p>Saisissez la plage de la première ligne du tableau. Par exemple, <code>A1:F1</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Value render option]</p> </td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Formatted value]</p> <p>Les valeurs seront calculées et mises en forme dans la réponse en fonction de la mise en forme de la cellule. La mise en forme est basée sur les paramètres régionaux de la feuille de calcul et non sur ceux de l’utilisateur ou de l’utilisatrice qui s’en sert. Par exemple, si <code>A1</code> est <code>1.23</code> et que <code>A2</code> est <code>=A1</code> et est mis en forme en tant que devise, <code>A2</code> renvoie <code>"$1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL Unformatted value]</p> <p>Les valeurs seront calculées, mais ne seront pas mises en forme dans la réponse. Par exemple, si <code>A1</code> est <code>1.23</code> et que <code>A2</code> est <code>=A1</code> et est mis en forme en tant que devise, <code>A2</code> renvoie le nombre <code>"1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL Formula]</p> <p>Les valeurs ne seront pas calculées. La réponse comprendra les formules. Par exemple, si <code>A1</code> est <code>1.23</code> et que <code>A2</code> est <code>=A1</code> et est mis en forme en tant que devise, <code>A2</code> renvoie <code>"=A1"</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Date and time render option]</p> </td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Serial number]</p> <p>Indique que les champs date, heure, date/heure et durée doivent être produits en double au format « numéro de série », comme popularisé par Lotus 1-2-3. La partie entière de la valeur (à gauche de la décimale) compte les jours écoulés depuis le 30 décembre 1899. La partie fractionnaire (à droite de la décimale) compte le temps comme une fraction de la journée. Par exemple, le 1er janvier 1900 à midi serait 2,5, 2 pour 2 jours après le 30 décembre 1899, et 0,5 parce que midi est une demi-journée. Le 1er février 1900 à 15 heures serait 33,625. L’année 1900 est traitée comme une année non bissextile, ce qui est correct.</p> <p style="font-weight: bold;">[!UICONTROL Formatted string]</p> <p>Indique que les champs date, heure, date/heure et durée doivent être produits sous forme de chaînes de caractères dans leur format numérique donné (qui dépend du paramètre local de la feuille de calcul).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Définissez le nombre maximal de résultats avec lesquels [!DNL Workfront Fusion] fonctionnera pendant un cycle d’exécution.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Actions

* [[!UICONTROL Ajouter une ligne]](#add-a-row)
* [[!UICONTROL Mettre à jour une ligne]](#update-a-row)
* [[!UICONTROL Effacer une ligne]](#clear-a-row)
* [[!UICONTROL Supprimer une ligne]](#delete-a-row)
* [[!UICONTROL Obtenir une cellule]](#get-a-cell)
* [[!UICONTROL Mettre à jour une cellule]](#update-a-cell)
* [[!UICONTROL Effacer une cellule]](#clear-a-cell)
* [[!UICONTROL Ajouter une feuille]](#add-a-sheet)
* [[!UICONTROL Créer une feuille de calcul]](#create-a-spreadsheet)
* [[!UICONTROL Supprimer une feuille]](#delete-a-sheet)
* [[!UICONTROL Effectuer un appel API]](#make-an-api-call)

### [!UICONTROL Ajouter une ligne]

Ce module ajoute une ligne à une feuille.

Lorsque vous configurez les modules [!DNL Google Sheets], [!DNL Workfront Fusion] affiche les champs énumérés ci-dessous. En plus de ces derniers, des champs [!DNL Google Sheets] supplémentaires peuvent s’afficher, selon des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton « Mapper » apparaît au-dessus d’un champ ou d’une fonction, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, consultez la section [Mapper des informations d’un module à l’autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Google Sheets] à [!DNL Workfront Fusion], voir la section <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connecter l’application ou le service web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Créer un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Mode]</td> 
   <td> <p>Indiquez si vous souhaitez sélectionner la feuille de calcul et la feuille manuellement ou par mappage.</p> <p>Remarque : le mappage manuel est utile, par exemple, lorsqu’une nouvelle feuille de calcul est créée dans un scénario [!DNL Workfront Fusion] et que vous souhaitez ajouter des données dans la feuille de calcul que vous venez de créer directement dans le scénario.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Spreadsheet] </td> 
   <td> <p>Sélectionnez la feuille de calcul [!DNL Google].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sheet] </td> 
   <td> <p>Sélectionnez la feuille à laquelle vous souhaitez ajouter une ligne.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Column Range]</td> 
   <td>Sélectionnez la plage de colonnes à utiliser.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Table contains headers]</td> 
   <td> <p> Indiquez si la feuille de calcul contient la ligne d’en-tête.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Yes]</strong> </p> <p>Le module ne récupère pas la ligne d’en-tête comme données de sortie. </p> <p>Les noms de variables dans la sortie sont appelés par les en-têtes.</p> </li> 
     <li> <p><strong>[!UICONTROL No]</strong> </p> <p>Le module récupère également la première ligne du tableau.</p> <p>Les noms de variables dans la sortie sont appelés A, B, C, D, etc.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Values] </td> 
   <td> <p>Entrez ou mappez les cellules de votre choix dans la ligne à ajouter.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Value input option]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL User entered]</strong></p> <p>Les valeurs sont traitées comme si l’utilisateur ou l’utilisatrice les avait saisies dans l’interface utilisateur. Les nombres restent des nombres, mais les chaînes peuvent être converties en nombres, en dates ou en autres formats en suivant les mêmes règles que celles qui s’appliquent lors d’une saisie de texte dans une cellule dans l’interface utilisateur de [!DNL Google Sheets].</p> </li> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p> Les valeurs saisies par l’utilisateur ou l’utilisatrice ne sont pas traitées et sont stockées en l’état. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Insert data option]</td> 
   <td> <p>Indiquez le mode de modification des données existantes lors de la saisie de nouvelles données. </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Insert rows]</strong></p> <p>Des lignes sont insérées pour les nouvelles données.</p> </li> 
     <li> <p><strong>[!UICONTROL Overwrite]</strong> </p> <p>Les nouvelles données remplacent les données existantes dans les zones où elles sont écrites. L’ajout de données à la fin de la feuille insère de nouvelles lignes ou colonnes afin que les données puissent être écrites.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Mettre à jour une ligne]

Ce module permet de modifier le contenu d’une cellule dans une ligne sélectionnée.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Google Sheets] à [!DNL Workfront Fusion], voir la section <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connecter l’application ou le service web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Créer un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Mode]</td> 
   <td> <p>Indiquez si vous souhaitez sélectionner la feuille de calcul et la feuille manuellement ou par mappage.</p> <p>Remarque : le mappage manuel est utile, par exemple, lorsqu’une nouvelle feuille de calcul est créée dans le scénario [!UICONTROL Workfront Fusion] et que vous souhaitez ajouter des données à la nouvelle feuille de calcul directement dans le scénario.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Spreadsheet] </td> 
   <td> <p>Sélectionnez la feuille de calcul [!DNL Google].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sheet] </td> 
   <td> <p>Sélectionnez la feuille dans laquelle vous souhaitez mettre à jour une ligne.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Row number]</td> 
   <td> <p> Saisissez le numéro de la ligne à mettre à jour.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Table contains headers]</td> 
   <td> <p> Indiquez si la feuille de calcul contient la ligne d’en-tête.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Yes]</strong> </p> <p>Le module ne récupère pas la ligne d’en-tête comme données de sortie. </p> <p>Les noms de variables dans la sortie sont appelés par les en-têtes.</p> </li> 
     <li> <p><strong>[!UICONTROL No]</strong> </p> <p>Le module récupère également la première ligne du tableau.</p> <p>Les noms de variables dans la sortie sont appelés A, B, C, D, etc.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Values] </td> 
   <td> <p>Entrez ou mappez les valeurs dans les cellules de votre choix de la ligne à modifier (mettre à jour).</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Value input option]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL User entered]</strong></p> <p>Les valeurs sont traitées comme si l’utilisateur ou l’utilisatrice les avait saisies dans l’interface utilisateur. Les nombres restent des nombres, mais les chaînes peuvent être converties en nombres, en dates ou en autres formats en suivant les mêmes règles que celles qui s’appliquent lors d’une saisie de texte dans une cellule dans l’interface utilisateur de [!DNL Google Sheets].</p> </li> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p> Les valeurs saisies par l’utilisateur ou l’utilisatrice ne sont pas traitées et sont stockées en l’état. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Effacer une ligne]

Supprime les valeurs d’une ligne spécifiée.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Google Sheets] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connecter l’application ou le service web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Créer un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Spreadsheet] </td> 
   <td> <p>Sélectionnez la feuille de calcul [!DNL Google] contenant la feuille dont vous souhaitez supprimer une ligne.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sheet] </td> 
   <td> <p> Sélectionnez la feuille dont vous souhaitez effacer des données.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Row number]</td> 
   <td> <p>Saisissez le numéro de la ligne dont vous souhaitez effacer les données. Par exemple, <code> 23</code>.</p> </td> 
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
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Google Sheets] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connecter l’application ou le service web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Créer un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Spreadsheet] </td> 
   <td> <p>Sélectionnez la feuille de calcul Google contenant la feuille dont vous souhaitez supprimer une ligne.</p> </td> 
  </tr> 
  <tr> 
   <td>Feuille </td> 
   <td> <p>Sélectionnez la feuille dont vous souhaitez supprimer une ligne.</p> </td> 
  </tr> 
  <tr> 
   <td>Numéro de ligne</td> 
   <td> <p>Saisissez le numéro de la ligne à supprimer. Exemple : <code>23</code></p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Obtenir une cellule]

Récupère une valeur d’une cellule sélectionnée.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Google Sheets] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connecter l’application ou le service web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Créer un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Spreadsheet] </td> 
   <td> <p>Sélectionnez la feuille de calcul [!DNL Google].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sheet] </td> 
   <td> <p>Sélectionnez la feuille contenant la cellule à partir de laquelle vous souhaitez récupérer des données.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cell] </td> 
   <td> <p>Saisissez l’ID de la cellule à partir de laquelle vous souhaitez récupérer des données. Exemple : <code>A6</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Value render option]</td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Formatted value]</p> <p>Les valeurs seront calculées et mises en forme dans la réponse en fonction de la mise en forme de la cellule. La mise en forme est basée sur les paramètres régionaux de la feuille de calcul et non sur ceux de l’utilisateur ou de l’utilisatrice qui s’en sert. Par exemple, si <code>A1</code> est <code>1.23</code> et que <code>A2</code> est <code>=A1</code> et est mis en forme en tant que devise, <code>A2</code> renverra <code>"$1.23"</code>.</p> <p style="font-weight: bold;">[!DNL Unformatted value]</p> <p>Les valeurs seront calculées, mais ne seront pas mises en forme dans la réponse. Par exemple, si <code>A1</code> est <code>1.23</code> et que <code>A2</code> est <code>=A1</code> et est mis en forme en tant que devise, <code>A2</code> renverra le nombre <code>"1.23"</code>.</p> <p style="font-weight: bold;">[!DNL Formula]</p> <p>Les valeurs ne seront pas calculées. La réponse comprendra les formules. Par exemple, si <code>A1</code> est <code>1.23</code> et que <code>A2</code> est <code>=A1</code> et est mis en forme en tant que devise, <code>A2</code> renverra <code>"=A1"</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!DNL Date and time render option]</td> 
   <td> <p style="font-weight: bold;">[!DNL Serial number]</p> <p>Indique que les champs date, heure, date/heure et durée doivent être produits en double au format « numéro de série », comme popularisé par Lotus 1-2-3. La partie entière de la valeur (à gauche de la décimale) compte les jours écoulés depuis le 30 décembre 1899. La partie fractionnaire (à droite de la décimale) compte le temps comme une fraction de la journée. Par exemple, le 1er janvier 1900 à midi serait 2,5, 2 pour 2 jours après le 30 décembre 1899, et 0,5 parce que midi est une demi-journée. Le 1er février 1900 à 15 heures serait 33,625. L’année 1900 est traitée comme une année non bissextile, ce qui est correct.</p> <p style="font-weight: bold;">[!DNL Formatted string]</p> <p>Indique que les champs date, heure, date/heure et durée doivent être produits sous forme de chaînes de caractères dans leur format numérique donné (qui dépend du paramètre local de la feuille de calcul).</p> </td> 
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
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Google Sheets] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connecter l’application ou le service web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Créer un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Spreadsheet] </td> 
   <td> <p>Sélectionnez la feuille de calcul [!DNL Google].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cell] </td> 
   <td> <p>Saisissez l’ID de la cellule que vous souhaitez mettre à jour. Exemple : <code>A5</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Value]</td> 
   <td> <p>Saisissez la nouvelle valeur de la cellule.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Value input option]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL User entered]</strong></p> <p>Les valeurs sont traitées comme si l’utilisateur ou l’utilisatrice les avait saisies dans l’interface utilisateur. Les nombres restent des nombres, mais les chaînes peuvent être converties en nombres, en dates ou en autres formats en suivant les mêmes règles que celles qui s’appliquent lors d’une saisie de texte dans une cellule dans l’interface utilisateur de [!DNL Google Sheets].</p> </li> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p> Les valeurs saisies par l’utilisateur ou l’utilisatrice ne sont pas traitées et sont stockées en l’état. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Effacer une cellule]

Supprime une valeur d’une cellule spécifiée.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Google Sheets] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connecter l’application ou le service web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Créer un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Spreadsheet] </td> 
   <td> <p>Sélectionnez la feuille de calcul Google contenant la feuille dont vous souhaitez effacer une cellule.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sheet] </td> 
   <td> <p>Sélectionnez la feuille dont vous souhaitez effacer une cellule.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cell] </td> 
   <td> <p>Saisissez l’ID de la cellule à effacer. Exemple : <code>A5</code>.</p> </td> 
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
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Google Sheets] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connecter l’application ou le service web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Créer un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Spreadsheet] </td> 
   <td> <p>Sélectionnez la feuille de calcul Google dans laquelle vous souhaitez ajouter une feuille.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Properties]</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">[!UICONTROL Title]</p> <p>Saisissez le nom de la nouvelle feuille.</p> </li> 
     <li> <p style="font-weight: bold;">[!UICONTROL Index]</p> <p>Saisissez la position de la feuille. La valeur par défaut est 0 (place la feuille en première position).</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Créer une feuille de calcul]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Google Sheets] à [!DNL Workfront Fusion], consultez la section <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connecter l’application ou le service web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Créer un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Title] </td> 
   <td> <p>Saisissez le nom d’une nouvelle feuille de calcul.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Locale]</td> 
   <td> <p>Saisissez les paramètres régionaux de la feuille de calcul dans l’un des formats suivants :</p> 
    <ul> 
     <li>un code de langue ISO 639-1 tel que <code>en</code></li> 
     <li>un code de langue ISO 639-2 tel que <code>haw</code>, s’il n’existe aucun code 639-1</li> 
     <li>une combinaison du code de langue ISO et du code de pays, telle que <code>en_US</code></li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Recalculation interval]</td> 
   <td> <p>Le temps d’attente avant que les fonctions volatiles ne soient recalculées :</p> <p style="font-weight: bold;">[!UICONTROL On change]</p> <p>Les fonctions volatiles sont mises à jour à chaque modification.</p> <p style="font-weight: bold;">[!UICONTROL On change and every minute]</p> <p>Les fonctions volatiles sont mises à jour à chaque modification et chaque minute.</p> <p style="font-weight: bold;">[!UICONTROL On change and hourly]</p> <p>Les fonctions volatiles sont mises à jour à chaque modification et toutes les heures.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Time zone]</td> 
   <td> <p> Sélectionnez le fuseau horaire de la feuille de calcul.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Number format]</td> 
   <td> <p>Sélectionnez le format par défaut de toutes les cellules de la feuille de calcul.</p> <p><strong>[!UICONTROL Text]</strong> : mise en forme du texte. Exemple : <code>1000. 12</code></p> <p><strong>[!UICONTROL Number]</strong> : mise en forme des nombres. Exemple : <code>1,000.12</code></p> <p><strong>[!UICONTROL Percent]</strong> : mise en forme des pourcentages. Exemple : <code>10. 12%</code></p> <p><strong>[!UICONTROL Currency]</strong> : mise en forme de la devise. Exemple : <code>$1,000.12</code></p> <p><strong>[!UICONTROL Date]</strong> : mise en forme des dates. Exemple : <code>9/26/2008</code></p> <p><strong>[!UICONTROL Time]</strong> : mise en forme de l’heure. Exemple : <code>3:59:00 PM</code></p> <p><strong>[!UICONTROL Date time]</strong> : mise en forme de la date et de l’heure. Exemple : <code>9/26/08 15:59:00</code> </p> <p><strong>[!UICONTROL Scientific]</strong> : mise en forme de l’écriture scientifique. Exemple : <code>1. 01E+03</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sheets] </td> 
   <td> <p>Cliquez sur <strong>[!UICONTROL Add]</strong> pour ajouter une feuille à la feuille de calcul. Pour chaque feuille, saisissez ou mappez un titre pour la feuille et l’index de la feuille. Un index de 0 représente la première feuille.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Supprimer une feuille]

Supprime une feuille spécifique.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Google Sheets] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connecter l’application ou le service web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Créer un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Spreadsheet] </td> 
   <td> <p>Sélectionnez la feuille de calcul [!DNL Google].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sheet] </td> 
   <td> <p>Sélectionnez la feuille à supprimer.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Réaliser un appel API]

Ce module d’action vous permet d’effectuer un appel API personnalisé.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [Fusion App] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td>Saisissez un chemin d’accès relatif à <code>https://sheets.googleapis.com/v4/</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Method]</p> </td> 
   <td> <p>Sélectionnez la méthode de requête HTTP dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Ajoutez les en-têtes de la requête sous la forme d’un objet JSON standard. Par exemple : <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] ajoute les en-têtes d’autorisation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p> Ajoutez la requête pour l’appel API sous la forme d’un objet JSON standard.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard.</p> <p>Note :   <p>Lors de l’utilisation d’instructions conditionnelles telles que <code>if</code> dans votre fichier JSON, placez les guillemets autour de l’instruction conditionnelle.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

## Recherches

* [[!UICONTROL Effectuer une recherche dans les lignes]](#search-rows)
* [[!UICONTROL Effectuer une recherche dans les lignes (avancé)]](#search-rows-advanced)
* [[!UICONTROL Obtenir les valeurs de plage]](#get-range-values)
* [[!UICONTROL Répertorier les feuilles]](#list-sheets)

### [!UICONTROL Effectuer une recherche dans les lignes]

Effectue une recherche dans les lignes à l’aide des options de filtre.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [Fusion App] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Spreadsheet] </td> 
   <td> <p>Sélectionnez la feuille de calcul [!DNL Google].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sheet] </td> 
   <td> <p>Sélectionnez la feuille dans laquelle vous souhaitez effectuer une recherche sur les lignes.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Table contains headers]</td> 
   <td> <p> Indiquez si la feuille de calcul contient la ligne d’en-tête. Si l’option [!UICONTROL Yes] est sélectionnée, le module ne récupère pas la ligne d’en-tête, car les données de sortie et les noms de variable dans la sortie sont alors appelés par les en-têtes. Si l’option [!UICONTROL No] est sélectionnée, le module récupère également la première ligne de tableau et les noms de variable dans la sortie sont alors appelés uniquement A, B, C, D, etc.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Column range]</td> 
   <td>Sélectionnez la plage de colonnes à utiliser. Exemple : <code>A-F</code></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Filter]</td> 
   <td> <p>Définissez le filtre correspondant à la ligne devant faire l’objet de la recherche.</p> <p>Pour plus d’informations sur les filtres, voir la section <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">Ajouter un filtre à un scénario dans [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sort order]</td> 
   <td>Indiquez si vous souhaitez trier par ordre croissant ou décroissant.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Order by]</td> 
   <td>Sélectionnez la colonne sur laquelle effectuer le tri.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Value render option]</td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Formatted value]</p> <p>Les valeurs seront calculées et mises en forme dans la réponse en fonction de la mise en forme de la cellule. La mise en forme est basée sur les paramètres régionaux de la feuille de calcul et non sur ceux de l’utilisateur ou de l’utilisatrice qui s’en sert. Par exemple, si <code>A1</code> est <code>1.23</code> et que <code>A2</code> est <code>=A1</code> et est mis en forme en tant que devise, <code>A2</code> renvoie <code>"$1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL Unformatted value]</p> <p>Les valeurs seront calculées, mais ne seront pas mises en forme dans la réponse. Par exemple, si <code>A1</code> est <code>1.23</code> et que <code>A2</code> est <code>=A1</code> et est mis en forme en tant que devise, <code>A2</code> renvoie le nombre <code>"1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL Formula]</p> <p>Les valeurs ne seront pas calculées. La réponse comprendra les formules. Par exemple, si <code>A1</code> est <code>1.23</code> et que <code>A2</code> est <code>=A1</code> et est mis en forme en tant que devise, <code>A2</code> renvoie <code>"=A1"</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Date and time render option]</td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Serial number]</p> <p>Indique que les champs date, heure, date/heure et durée doivent être produits en double au format « numéro de série », comme popularisé par Lotus 1-2-3. La partie entière de la valeur (à gauche de la décimale) compte les jours écoulés depuis le 30 décembre 1899. La partie fractionnaire (à droite de la décimale) compte le temps comme une fraction de la journée. Par exemple, le 1er janvier 1900 à midi serait 2,5, 2 pour 2 jours après le 30 décembre 1899, et 0,5 parce que midi est une demi-journée. Le 1er février 1900 à 15 heures serait 33,625. L’année 1900 est traitée comme une année non bissextile, ce qui est correct.</p> <p style="font-weight: bold;">[!UICONTROL Formatted string]</p> <p>Indique que les champs date, heure, date/heure et durée doivent être produits sous forme de chaînes de caractères dans leur format numérique donné (qui dépend du paramètre local de la feuille de calcul).</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximum number of returned rows]</td> 
   <td>Définissez le nombre maximum de lignes que [!DNL Workfront Fusion] renverra pendant un cycle d’exécution.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Effectuer une recherche sur les lignes (avancé)]

Renvoie des résultats correspondant aux critères donnés.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Google Sheets] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connecter l’application ou le service web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Créer un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Spreadsheet] </td> 
   <td> <p>Sélectionnez la feuille de calcul Google contenant la feuille devant faire l’objet de la recherche.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sheet] </td> 
   <td> <p>Sélectionnez la feuille contenant les lignes devant faire l’objet de la recherche.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Query]</td> 
   <td> <p>Utilisez le [!DNL Google Charts Query Language]. Exemple : <code>select * where B = "John"</code></p> <p>Pour plus d’informations sur [!DNL Google Charts Query Language], voir la section <a href="https://developers.google.com/chart/interactive/docs/querylanguage?hl=fr">Référence du langage de requête</a> dans la documentation [!DNL Google].</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Obtenir des valeurs de plage]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Google Sheets] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connecter l’application ou le service web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Créer un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Spreadsheet] </td> 
   <td> <p>Sélectionnez la feuille de calcul [!DNL Google].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sheet] </td> 
   <td> <p>Sélectionnez la feuille à partir de laquelle vous souhaitez obtenir le contenu de la plage.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Range] </td> 
   <td> <p>Saisissez la plage que vous souhaitez obtenir. Exemple : <code>A1:D25</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Table contains headers]</td> 
   <td> <p>Cochez cette case si la feuille comporte une ligne d’en-tête.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Row with headers]</td> 
   <td>Saisissez la plage des en-têtes de tableau. Exemple : <code>A1:F1</code>. Si vous laissez le champ vide, [!DNL Workfront Fusion] supposera que l’en-tête se trouve dans la première ligne de la plage spécifiée.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Value render option]</td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Formatted value]</p> <p>Les valeurs seront calculées et mises en forme dans la réponse en fonction de la mise en forme de la cellule. La mise en forme est basée sur les paramètres régionaux de la feuille de calcul et non sur ceux de l’utilisateur ou de l’utilisatrice qui s’en sert. Par exemple, si <code>A1</code> est <code>1.23</code> et que <code>A2</code> est <code>=A1</code> et est mis en forme en tant que devise, <code>A2</code> renvoie <code>"$1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL Unformatted value]</p> <p>Les valeurs seront calculées, mais ne seront pas mises en forme dans la réponse. Par exemple, si <code>A1</code> est <code>1.23</code> et que <code>A2</code> est <code>=A1</code> et est mis en forme en tant que devise, <code>A2</code> renvoie le nombre <code>"1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL Formula]</p> <p>Les valeurs ne seront pas calculées. La réponse comprendra les formules. Par exemple, si <code>A1</code> est <code>1.23</code> et que <code>A2</code> est <code>=A1</code> et est mis en forme en tant que devise, <code>A2</code> renvoie <code>"=A1"</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Date and time render option]</td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Serial number]</p> <p>Indique que les champs date, heure, date/heure et durée doivent être produits en double au format « numéro de série », comme popularisé par Lotus 1-2-3. La partie entière de la valeur (à gauche de la décimale) compte les jours écoulés depuis le 30 décembre 1899. La partie fractionnaire (à droite de la décimale) compte le temps comme une fraction de la journée. Par exemple, le 1er janvier 1900 à midi serait 2,5, 2 pour 2 jours après le 30 décembre 1899, et 0,5 parce que midi est une demi-journée. Le 1er février 1900 à 15 heures serait 33,625. L’année 1900 est traitée comme une année non bissextile, ce qui est correct.</p> <p style="font-weight: bold;">[!UICONTROL Formatted string]</p> <p>Indique que les champs date, heure, date/heure et durée doivent être produits sous forme de chaînes de caractères dans leur format numérique donné (qui dépend du paramètre local de la feuille de calcul).</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Répertorier les feuilles]

Ce module renvoie une liste de toutes les feuilles d’une feuille de calcul.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Google Sheets] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connecter l’application ou le service web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Créer un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Spreadsheet] </td> 
   <td> <p>Sélectionnez la feuille de calcul [!DNL Google] qui contient les feuilles que vous souhaitez répertorier.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Limites d’utilisation

Si l’erreur `429: RESOURCE_EXHAUSTED` se produit, vous avez dépassé la limite de l’API.

L’API [!DNL Google Sheets] est limitée à 500 requêtes par 100 secondes par projet et à 100 requêtes par 100 secondes par personne. Les limites de lecture et d’écriture sont suivies séparément. Il n’y a pas de limite d’utilisation quotidienne.

Pour plus de détails, voir [developers.google.com/sheets/api/limits](https://developers.google.com/sheets/api/limits).

## Conseils et astuces

* [Comment obtenir les cellules vides d’une feuille  [!DNL Google] ](#how-to-get-empty-cells-from-a-google-sheet)
* [Ajouter un bouton dans une feuille pour exécuter un scénario](#add-a-button-in-a-sheet-to-run-a-scenario)

### Comment obtenir les cellules vides d’une [!DNL Google Sheet]

Utilisez le module [!UICONTROL Effectuer une recherche dans les lignes (avancé)] et utilisez cette formule pour obtenir les colonnes qui sont vides.
<pre>select * where E is null</pre>Ici, « E » est la colonne et « is null » est la condition. Vous pouvez créer une requête plus avancée en utilisant [Google Query Lang] (https://developers.google.com/chart/interactive/docs/querylanguage?hl=fr).

### Ajouter un bouton dans une feuille pour exécuter un scénario

1. Dans [!DNL Workfront Fusion], insérez le module/déclencheur **[!UICONTROL Webhook]** > **[!UICONTROL Webhooks personnalisés]** dans le scénario et configurez-le (voir [Webhooks](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md)).

1. Copiez l’URL du webhook.
1. Exécutez le scénario.
1. Dans Google Sheets, choisissez **[!UICONTROL Insérer]** > **[!UICONTROL Dessin]**... dans la barre de menu principale.

1. Dans la fenêtre [!UICONTROL Dessin], cliquez sur l’icône **[!UICONTROL Zone de texte]** ![](assets/text-box.png) en haut de la fenêtre.
1. Créez un bouton et cliquez sur le bouton **[!UICONTROL Enregistrer et fermer]** dans le coin supérieur droit :
1. Le bouton sera placé dans votre feuille de calcul. Cliquez sur les trois points verticaux dans le coin supérieur droit du bouton :
1. Choisissez **[!UICONTROL Attribuer un script...]** dans le menu.
1. Saisissez le nom de votre script (fonction), par exemple `runScenario`, et cliquez sur **[!UICONTROL OK]** :
1. Choisissez **[!UICONTROL Outils]** > **[!UICONTROL Éditeur de script]** dans la barre de menu principale.

1. Insérez le code suivant :

   * Le nom de la fonction doit correspondre au nom que vous avez spécifié à l’étape 9.
   * Remplacez l’URL par l’URL du webhook que vous avez copié à l’étape 2.

     <pre>function runScenario() {</pre><pre>UrlFetchApp.fetch("&lt;webhook que vous avez copié&gt;");</pre><pre>}</pre>

1. Appuyez sur **[!UICONTROL Ctrl + S]** pour enregistrer le fichier script, saisissez un nom de projet et cliquez sur **[!UICONTROL OK]**.

1. Revenez à [!DNL Google Sheets] et cliquez sur votre nouveau bouton.
1. Accorder l’autorisation obligatoire au script :
1. Dans [!DNL Workfront Fusion], vérifiez que le scénario s’est bien exécuté.

## Stocker des dates dans une feuille de calcul

Si vous stockez une valeur de date dans une feuille de calcul sans aucun formatage, elle apparaîtra dans la feuille de calcul sous forme de texte au format ISO 8601. Cependant, les formules ou fonctions de [!DNL Google Sheets] qui travaillent avec des dates et qui ne comprennent pas ce texte (exemple : formule `=A1+10`) afficheront l’erreur suivante :

![](assets/mceclip6-350x87.png)

Pour permettre à [!DNL Google Sheets] de comprendre la date, formatez-la avec la fonction [[!UICONTROL formatDate] (date; format; [timezone])](../../workfront-fusion/functions/date-and-time-functions.md#formatda). Le format correct transmis à la fonction en tant que deuxième argument dépend des paramètres locaux de la feuille de calcul.

Pour déterminer le format correct :

1. Choisissez les paramètres **[!UICONTROL Fichier]** > **[!UICONTROL Feuille de calcul]** dans le menu principal pour vérifier/régler les paramètres locaux.

1. Une fois que vous avez vérifié/réglé les paramètres locaux, déterminez le format de date et d’heure correspondant en choisissant **[!UICONTROL Format]** > **[!UICONTROL Nombre]** dans le menu principal. Le format est affiché à côté de l’élément de menu Date et heure :

1. Pour composer le format correct à transmettre à la fonction [!UICONTROL formatDate()], consultez la liste des [Jetons pour le formatage de la date et de l’heure dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-formatting.md).

**Exemple :** l&#39;utilisation du format `MM/DD/YYYY HH:mm:ss` pour les États-Unis :

![](assets/locale-time-350x83.png)

## Exploiter les fonctions de [!DNL Google Sheets]

Si une fonction intégrée vous manque, mais qu’elle est disponible sur [!DNL Google Sheets], vous pouvez l’exploiter. Pour plus d’informations, voir [Utiliser les fonctions de  [!DNL Google Sheets] ](../../workfront-fusion/functions/map-using-functions.md#exploiti) dans [Mapper des éléments à l’aide des fonctions de  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/map-using-functions.md).

## Empêcher [!DNL Google Sheets] de transformer des nombres en dates

Vous pouvez constater qu’une chaîne de chiffres que vous utilisez comme texte est interprétée comme une date dans une feuille de calcul [!DNL Google]. Par exemple, vous tapez 1-2019, en pensant que c’est du texte, mais Google l’interprète comme une date. Pour éviter cela, vous pouvez préformater le numéro en texte brut.

1. Dans [!DNL Google Sheets], mettez en évidence la colonne ou la cellule contenant le ou les nombres.
1. Cliquez sur **[!UICONTROL Format]** > **[!UICONTROL Nombre]** > **[!UICONTROL Texte brut]**.

Une autre solution dans [!DNL Workfront Fusion] consiste à saisir une apostrophe (&#39;) avant un nombre, par exemple &#39;1-2019&#39; ou &#39;1/47&#39;. L’apostrophe ne s’affiche pas dans la cellule après l’envoi des données depuis [!DNL Workfront Fusion].
