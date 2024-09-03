---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: connecteur
navigation-topic: apps-and-their-modules
title: Modules Microsoft Office 365 Excel
description: Dans un scénario  [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les workflows qui utilisent Microsoft 365 Excel et les connecter à plusieurs applications et services tiers.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 9aa3739d-6800-4eb1-a17f-32fdfd8ed0f2
source-git-commit: 7d5f7c21fe38d43fb5601c81b8a31cc80587848f
workflow-type: tm+mt
source-wordcount: '2744'
ht-degree: 100%

---

# Modules [!DNL Microsoft Office 365 Excel]

Dans un scénario [!DNL Adobe Workfront Fusion], vous pouvez automatiser les workflows qui utilisent [!DNL Microsoft 365 Excel] et le connecter à plusieurs applications et services tiers.

Si vous avez besoin d’instructions sur la création d’un scénario, consultez [Créer un scénario dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Pour plus d’informations sur les modules, voir [Modules dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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
   <p>Conditions requises du produit actuel : si vous disposez de la formule [!DNL Adobe Workfront] [!UICONTROL Select] ou [!UICONTROL Prime], votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article. [!DNL Workfront Fusion] est inclus dans la formule [!DNL Workfront] [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Exigences liées aux produits hérités : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi qu’[!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez votre équipe d’administration [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], voir Licences [[!DNL Adobe Workfront Fusion] ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Conditions préalables

Pour utiliser [!DNL Microsoft office 365 Excel], vous devez disposer d’un compte Microsoft.



## Connecter le service [!DNL Office 365 Excel] à [!DNL Workfront Fusion]

Pour obtenir des instructions sur la connexion de votre compte [!DNL Office 365 Excel] à [!UICONTROL Workfront Fusion], voir [Créer une connexion à [!UICONTROL Adobe Workfront Fusion] : instructions de base](../../workfront-fusion/connections/connect-to-fusion-general.md)

>[!NOTE]
>
>Certaines applications Microsoft utilisent la même connexion, qui est liée à des autorisations d’utilisateur ou d’utilisatrice. Ainsi, lors de la création d’une connexion, l’écran de consentement aux autorisations affiche les autorisations précédemment accordées à la connexion de cet utilisateur ou de cette utilisatrice, en plus des nouvelles autorisations nécessaires à l’application actuelle.
>
>Par exemple, si un utilisateur ou une utilisatrice dispose d’autorisations « Lire le tableau » accordées via le connecteur Excel, puis crée une connexion dans le connecteur Outlook pour lire les e-mails, l’écran de consentement aux autorisations affiche à la fois l’autorisation « Lire le tableau » déjà accordée et l’autorisation « Écrire des e-mails » nouvellement requise.

## Modules [!DNL Microsoft Office 365 Excel] et leurs champs

Lorsque vous configurez les modules [!DNL Microsoft 365 Excel], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. En plus de ces derniers, des champs [!DNL Microsoft 365 Excel] supplémentaires peuvent s’afficher, selon des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton « Mapper » apparaît au-dessus d’un champ ou d’une fonction, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, consultez [Mapper des informations d’un module à un autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Classeur](#workbook)
* [Feuille de travail](#worksheet)
* [Tableau](#table)
* [Autre](#other)

### Classeur

* [Surveiller des classeurs](#watch-workbooks)
* [Rechercher des classeurs](#search-workbooks)
* [Télécharger un classeur](#download-a-workbook)

#### [!UICONTROL Surveiller des classeurs]

Ce module de déclenchement démarre un scénario lorsqu’un classeur est créé.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la procédure de connexion de votre compte [!DNL Office 365] à [!DNL Workfront Fusion], consultez <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connecter l’application ou le service web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Créer un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td> <p>Sélectionnez le dossier que vous souhaitez utiliser pour surveiller les nouveaux classeurs.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Filter]</p> </td> 
   <td> <p>Vous pouvez définir un filtre afin de ne surveiller que les classeurs qui répondent aux critères que vous sélectionnez.</p> <p>Pour chaque filtre, saisissez le champ que le filtre doit évaluer, l’opérateur et la valeur que le filtre doit autoriser. Vous pouvez utiliser plusieurs filtres en ajoutant des règles ET ou OU.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Saisissez ou mappez le nombre maximal de classeurs que le module doit renvoyer au cours de chaque cycle d’exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Rechercher des classeurs]

Ce module d’action recherche des classeurs [!DNL Excel].

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la procédure de connexion de votre compte [!DNL Office 365] à [!DNL Workfront Fusion], consultez <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connecter l’application ou le service web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Créer un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td> <p>Sélectionnez le dossier dans lequel vous souhaitez rechercher des classeurs.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Filter]</p> </td> 
   <td> <p>Vous pouvez définir un filtre afin de rechercher uniquement les classeurs qui répondent aux critères sélectionnés.</p> <p>Pour chaque filtre, saisissez le champ que le filtre doit évaluer, l’opérateur et la valeur que le filtre doit autoriser. Vous pouvez utiliser plusieurs filtres en ajoutant des règles ET ou OU.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Saisissez ou mappez le nombre maximal de feuilles de calcul que le module doit renvoyer au cours de chaque cycle d’exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Télécharger un classeur]

Ce module d’action télécharge le contenu du classeur Excel spécifié.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions afin de connecter votre compte [!DNL Office 365] à [!DNL Workfront Fusion], consultez <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connecter l’application ou le service web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Créer un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Download a workbook]</td> 
   <td> <p>Sélectionnez le mode d’identification du classeur à télécharger.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL By entering an ID manually]</strong> </p> <p>Dans le champ [!UICONTROL Workbook ID], saisissez ou mappez l’identifiant du classeur spécifique que le module doit télécharger.</p> </li> 
     <li> <p><strong>[!UICONTROL By selecting from the path]</strong> </p> <p>Dans le champ [!UICONTROL Workbook], sélectionnez le classeur que le module doit télécharger.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Feuille de travail

* [[!UICONTROL Surveiller des lignes de feuille de travail]](#watch-worksheet-rows)
* [[!UICONTROL Répertorier des feuilles de calcul]](#list-worksheets)
* [[!UICONTROL Répertorier des lignes de feuille de travail]](#list-worksheet-rows)
* [[!UICONTROL Ajouter une feuille de travail]](#add-a-worksheet)
* [[!UICONTROL Ajouter une ligne de feuille de travail]](#add-a-worksheet-row)
* [[!UICONTROL Mettre à jour une ligne de feuille de travail]](#update-a-worksheet-row)
* [[!UICONTROL Supprimer une ligne de feuille de travail]](#delete-a-worksheet-row)

#### [!UICONTROL Surveiller des lignes de feuille de travail]

Ce module déclencheur lance un scénario lorsqu’une nouvelle ligne est ajoutée à la feuille.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions afin de connecter votre compte [!DNL Office 365] à [!DNL Workfront Fusion], consultez <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connecter l’application ou le service web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Créer un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Workbook] </td>
   <td> <p>Sélectionnez le classeur qui contient la feuille de travail dans laquelle vous souhaitez surveiller les nouvelles lignes.</p> </td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL Worksheet] </td>
   <td> <p>Sélectionnez la feuille Excel dans laquelle vous souhaitez surveiller les nouvelles lignes.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Limit]</td>
   <td> <p>Saisissez ou mappez le nombre maximal de lignes de feuille de travail que le module doit renvoyer au cours de chaque cycle d’exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Répertorier des feuilles de calcul]

Ce module d’action récupère une liste de feuilles de calcul dans le classeur spécifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions afin de connecter votre compte [!DNL Office 365] à [!DNL Workfront Fusion], consultez <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connecter l’application ou le service web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Créer un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Workbook] </td>
   <td> <p>Sélectionnez le classeur qui contient les feuilles de calcul que le module doit répertorier.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Limit]</td>
   <td> <p>Saisissez ou mappez le nombre maximal de feuilles de calcul que le module doit renvoyer au cours de chaque cycle d’exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Lister les lignes de feuille de travail]

Ce module d’action récupère une liste de lignes d’une feuille de travail spécifiée.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions afin de connecter votre compte [!DNL Office 365] à [!DNL Workfront Fusion], consultez <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connecter l’application ou le service web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Créer un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL Workbook] </td>
   <td> <p>Sélectionnez le classeur qui contient la feuille de travail et les lignes que vous souhaitez répertorier.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Worksheet] </td>
   <td> <p>Sélectionnez la feuille de travail qui contient les lignes que vous souhaitez répertorier.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Limit]</td>
   <td> <p>Saisissez ou mappez le nombre maximal de lignes de feuille de travail que le module doit renvoyer au cours de chaque cycle d’exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ajouter une feuille de travail]

Ce module d’action crée une feuille de travail dans le classeur sélectionné.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions afin de connecter votre compte [!DNL Office 365] à [!DNL Workfront Fusion], consultez <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connecter l’application ou le service web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Créer un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL Workbook] </td>
   <td> <p>Sélectionnez le classeur dans lequel vous souhaitez ajouter une feuille de travail.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Name] </td>
   <td> <p>Saisissez ou mappez un nom pour la nouvelle feuille de travail.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ajouter une ligne de feuille de travail]

Ce module d’action ajoute une nouvelle ligne à la feuille de travail sélectionnée.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions afin de connecter votre compte [!DNL Office 365] à [!DNL Workfront Fusion], consultez <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connecter l’application ou le service web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Créer un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Workbook] </td>
   <td> <p>Sélectionnez le classeur qui contient la feuille de travail dans laquelle vous souhaitez ajouter une ligne.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Worksheet] </td>
   <td> <p>Sélectionnez la feuille de travail dans laquelle vous souhaitez ajouter une ligne.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Type of values being entered]</p> </td> 
   <td> <p>Sélectionnez le type de valeur à renseigner dans la feuille de travail. </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Formulas]</strong> </p> <p> Excel tente d’évaluer l’expression spécifiée. Les noms des fonctions d’une formule sont en anglais. Exemple : <code>[!DNL =SUM(A1:A10)]</code></p> </li> 
     <li> <p><strong>[!UICONTROL Formulas local]</strong> </p> <p>Excel tente d’évaluer l’expression spécifiée. Les noms des fonctions sont dans la langue de l’application Excel. Exemple : <code>=SUM(A1, 1.5)</code> vs <code>=SUMME(A1; 1,5)</code></p> </li> 
     <li> <p><strong>[!UICONTROL Value]</strong> </p> <p>Excel n’évalue pas la valeur. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Row]</td>
    <td>Pour chaque colonne, saisissez la valeur à lui donner dans la nouvelle ligne.</td>
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mettre à jour une ligne de feuille de travail]

Ce module d’action met à jour une ligne de feuille de travail existante.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions afin de connecter votre compte [!DNL Office 365] à [!DNL Workfront Fusion], consultez <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connecter l’application ou le service web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Créer un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Workbook] </td>
   <td> <p>Sélectionnez le classeur qui contient la feuille de travail et la ligne à mettre à jour.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Worksheet] </td>
   <td> <p>Sélectionnez la feuille de travail contenant la ligne à mettre à jour.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Type of values being entered]</p> </td> 
   <td> <p>Sélectionnez le type de valeur à renseigner dans la feuille de travail. </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Formulas]</strong> </p> <p> Excel tente d’évaluer l’expression spécifiée. Les noms des fonctions d’une formule sont en anglais. Exemple : <code>[!DNL =SUM(A1:A10)]</code></p> </li> 
     <li> <p><strong>[!UICONTROL Formulas local]</strong> </p> <p>Excel tente d’évaluer l’expression spécifiée. Les noms des fonctions sont dans la langue de l’application Excel. Exemple : <code>=SUM(A1, 1.5)</code> vs <code>=SUMME(A1; 1,5)</code></p> </li> 
     <li> <p><strong>[!UICONTROL Value]</strong> </p> <p>Excel n’évalue pas la valeur. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Row ID]</td> 
   <td>Sélectionnez le numéro de la ligne à mettre à jour.</td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Row]</td>
    <td>Pour chaque colonne, saisissez la valeur à lui donner dans la nouvelle ligne.</td>
   --&gt; 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Supprimer une ligne de feuille de travail]

Ce module d’action supprime une ligne d’une feuille de travail.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions afin de connecter votre compte [!DNL Office 365] à [!DNL Workfront Fusion], consultez <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connecter l’application ou le service web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Créer un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Workbook] </td>
   <td> <p>Sélectionnez le classeur qui contient la feuille de travail et la ligne à supprimer.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Worksheet]</td>
   <td> <p> Sélectionnez la feuille de travail contenant la ligne à supprimer.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Row ID]</td>
   <td>Saisissez ou mappez l’identifiant de la ligne à supprimer.</td> 
  </tr> 
 </tbody> 
</table>

### Tableau

* [[!UICONTROL Surveiller les lignes de tableau]](#watch-table-rows)
* [[!UICONTROL Lister les tableaux]](#list-tables)
* [[!UICONTROL Lister les lignes de tableau]](#list-table-rows)
* [[!UICONTROL Obtenir un tableau]](#get-a-table)
* [[!UICONTROL Ajouter un tableau]](#add-a-table)
* [[!UICONTROL Ajouter une ligne de tableau]](#add-a-table-row)
* [[!UICONTROL Mettre à jour un tableau]](#update-a-table)
* [[!UICONTROL Supprimer un tableau]](#delete-a-table)

#### [!UICONTROL Surveiller les lignes de tableau]

Ce déclencheur lance un scénario lorsqu’une nouvelle ligne est ajoutée à un tableau.

>[!NOTE]
>
>Le tableau désigne ici l’élément de tableau incorporé dans le classeur. Il ne s’agit pas du tableau complet (classeur/feuille).

![](assets/embedded-table-350x420.png)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions afin de connecter votre compte [!DNL Office 365] à [!DNL Workfront Fusion], consultez <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connecter l’application ou le service web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Créer un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Workbook]</p> </td> 
   <td> <p>Sélectionnez le classeur qui contient le tableau à surveiller.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Worksheet] </td>
   <td> <p> Sélectionnez la feuille de travail contenant le tableau à surveiller.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Table]</p> </td> 
   <td> <p>Sélectionnez le tableau à surveiller.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Limit]</td>
   <td> <p>Saisissez ou mappez le nombre maximal de lignes que le module doit renvoyer pour chaque cycle d’exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Lister des tableaux]

Ce module de recherche récupère une liste de tous les objets de tableau.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions afin de connecter votre compte [!DNL Office 365] à [!DNL Workfront Fusion], consultez <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connecter l’application ou le service web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Créer un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL Workbook] </td>
   <td> <p>Sélectionnez le classeur qui contient les tableaux que vous souhaitez répertorier.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Worksheet] </td>
   <td> <p>Sélectionnez la feuille de travail qui contient les tableaux que vous souhaitez répertorier.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Limit]</td>
   <td> <p>Saisissez ou mappez le nombre maximum de tableaux que le module doit renvoyer pour chaque cycle d’exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Répertorier des lignes de tableau]

Ce module de recherche récupère une liste de toutes les lignes d’un tableau dans un classeur.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions afin de connecter votre compte [!DNL Office 365] à [!DNL Workfront Fusion], consultez <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connecter l’application ou le service web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Créer un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Workbook] </td>
   <td> <p>Sélectionnez le classeur qui contient le tableau comprenant les lignes à répertorier.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Worksheet] </td>
   <td> <p>Sélectionnez la feuille de travail qui contient le tableau comprenant les lignes à répertorier.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Table] </td>
   <td> <p>Sélectionnez le tableau contenant les lignes à répertorier.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Limit]</td>
   <td> <p>Saisissez ou mappez le nombre maximal de lignes de tableau que le module doit renvoyer pour chaque cycle d’exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtenir un tableau]

Ce module d’action récupère les métadonnées du tableau spécifié.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> 
     <p >[!UICONTROL Connection]</p>
   </td> 
   <td> 
     <p>Pour obtenir des instructions afin de connecter votre compte Office 365 à [!DNL Workfront Fusion], consultez <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connecter l’application ou le service web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Créer un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p>
    --&gt; </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Get a table]</td> 
   <td> <p>Sélectionnez le mode d’identification du tableau que vous souhaitez récupérer.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>Dans le champ [!UICONTROL Workbook ID], saisissez ou mappez l’identifiant du classeur qui contient le tableau que vous souhaitez récupérer.</p> <p>Dans le champ [!UICONTROL Table Name], saisissez ou mappez le nom du tableau à récupérer.</p> </li> 
     <li> <p><strong>[!UICONTROL Select from the list]</strong> </p> <p>Sélectionnez le classeur et la feuille de travail qui contiennent le tableau à récupérer, puis sélectionnez le tableau.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ajouter un tableau]

Ce module d’action crée un élément de tableau dans la feuille de travail Excel.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions afin de connecter votre compte [!DNL Office 365] à [!DNL Workfront Fusion], consultez <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connecter l’application ou le service web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Créer un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workbook] </td> 
   <td> <p>Sélectionnez le classeur qui contient la feuille de travail dans laquelle vous souhaitez ajouter un tableau.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Worksheet] </td> 
   <td> <p>Sélectionnez la feuille de travail dans laquelle vous souhaitez ajouter un tableau.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Has headers]</td> 
   <td> <p>Activez cette option pour définir la première ligne comme en-têtes de tableau.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Address]</p> </td> 
   <td> <p>Définissez la taille du tableau en indiquant les cellules supérieure gauche et inférieure droite. Exemple : <code>A1:C10</code> crée un tableau de 3 colonnes et 10 lignes.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ajouter une ligne de tableau]

Ce module d’action modifie un tableau existant.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions afin de connecter votre compte [!DNL Office 365] à [!DNL Workfront Fusion], consultez <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connecter l’application ou le service web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Créer un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Workbook] </td>
   <td> <p>Sélectionnez le classeur qui contient le tableau dans lequel vous souhaitez ajouter une ligne.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Worksheet] </td>
   <td> <p>Sélectionnez la feuille de travail contenant le tableau dans lequel vous souhaitez ajouter une ligne.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Table]</td>
   <td>Sélectionnez le tableau dans lequel vous souhaitez ajouter une ligne.</td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL Row]</td>
    <td>Pour chaque colonne, saisissez la valeur à lui donner dans la nouvelle ligne.</td>
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Row ID]</p> </td> 
   <td> <p>Pour ajouter une ligne à un emplacement spécifique du tableau, saisissez ou mappez un numéro de ligne. Le module insère la nouvelle ligne après cette ligne.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mettre à jour un tableau]

Ce module d’action met à jour un tableau existant.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Office 365] à [!DNL Workfront Fusion], consultez la section <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connecter l’application ou le service web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Créer un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Update a table]</td> 
   <td> <p>Sélectionnez le mode d’identification du tableau à mettre à jour.</p> 
    <ul> 
     <li> <p><strong>Saisie manuelle</strong> </p> <p>Dans le champ [!UICONTROL Workbook ID], saisissez ou mappez l’identifiant du classeur qui contient le tableau à mettre à jour.</p> <p>Dans le champ [!UICONTROL Table Name], saisissez ou mappez le nom du tableau à mettre à jour.</p> </li> 
     <li> <p><strong>[!UICONTROL Select from the list]</strong> </p> <p>Sélectionnez le classeur et la feuille de travail qui contiennent le tableau à mettre à jour, puis sélectionnez le tableau.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Table] </td> 
   <td> <p>Sélectionnez le tableau à mettre à jour.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name]</td> 
   <td> <p>Si vous souhaitez renommer le tableau, saisissez ou mappez un nouveau nom pour le tableau.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Show Headers]</td> 
   <td> <p>Activez cette option pour afficher les en-têtes du tableau mis à jour.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Show totals]</td> 
   <td>Activez cette option pour afficher les valeurs totales du tableau.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Style]</td> 
   <td>Appliquez un style pour le nouveau tableau.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Supprimer un tableau]

Ce module d’action supprime le tableau spécifié d’une feuille de travail [!DNL Excel].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Office 365] à [!DNL Workfront Fusion], consultez la section <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connecter l’application ou le service web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Créer un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Get a table]</td> 
   <td> <p>Sélectionnez le mode d’identification du tableau à supprimer.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>Dans le champ [!UICONTROL Workbook ID], saisissez ou mappez l’identifiant du classeur qui contient le tableau à supprimer.</p> <p>Dans le champ [!UICONTROL Table Name], saisissez ou mappez le nom du tableau à supprimer.</p> </li> 
     <li> <p><strong>[!UICONTROL Select from the list]</strong> </p> <p>Sélectionnez le classeur et la feuille de travail qui contiennent le tableau à supprimer, puis sélectionnez-le.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Autre

* [[!UICONTROL Récupérer les données]](#retrieve-data)
* [[!UICONTROL Effectuer un appel API]](#make-an-api-call)

#### [!UICONTROL Récupérer les données]

Cette action récupère les données de la plage de feuilles de travail définie et renvoie un lot pour chaque ligne.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions afin de connecter votre compte [!DNL Office 365] à [!DNL Workfront Fusion], consultez <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connecter l’application ou le service web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Créer un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workbook] </td> 
   <td> <p>Sélectionnez le classeur qui contient les données à récupérer.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Worksheet] </td> 
   <td> <p>Sélectionnez la feuille de travail contenant les données à récupérer.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Range] </td> 
   <td> <p>Indiquez la zone de la feuille à partir de laquelle vous souhaitez récupérer les données en indiquant les cellules supérieure gauche et inférieure droite. Exemple : <code>A1:D10</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Effectuer un appel API]

Ce module d’action vous permet d’effectuer un appel API personnalisé.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Office 365] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connecter l’application ou le service web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Créer un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Saisissez un chemin relatif à <code>https://graph.microsoft.com</code>. Exemple :<code> /v1.0/me/drive/root/children</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   td&gt; <p>Sélectionnez la méthode de requête HTTP dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Ajoutez les en-têtes de la requête sous la forme d’un objet JSON standard.</p> <p>Par exemple, <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion ajoute les en-têtes d’autorisation pour vous.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>Ajoutez la requête pour l’appel API sous la forme d’un objet JSON standard.</p> <p>Par exemple : <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard.</p> <p>Note :   <p>Lors de l’utilisation d’instructions conditionnelles telles que <code>if</code> dans votre fichier JSON, placez les guillemets en dehors de l’instruction conditionnelle.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>
