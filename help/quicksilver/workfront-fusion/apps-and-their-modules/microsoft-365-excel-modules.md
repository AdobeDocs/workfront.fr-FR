---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: connector
navigation-topic: apps-and-their-modules
title: Modules Excel Microsoft Office 365
description: Dans un [!DNL Adobe Workfront Fusion] vous pouvez automatiser les workflows qui utilisent Microsoft 365 Excel et les connecter à plusieurs applications et services tiers.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 9aa3739d-6800-4eb1-a17f-32fdfd8ed0f2
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '2625'
ht-degree: 0%

---

# [!DNL Microsoft Office 365 Excel] modules

Dans un [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les workflows qui utilisent [!DNL Microsoft 365 Excel], ainsi que de la connecter à plusieurs applications et services tiers.

Si vous avez besoin d’instructions sur la création d’un scénario, reportez-vous à la section [Création d’un scénario dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Pour plus d’informations sur les modules, voir [Modules dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

Pour utiliser [!DNL Microsoft office 365 Excel], vous devez disposer d’un compte Microsoft.

## [!DNL Microsoft Office 365 Excel] modules et leurs champs

Lorsque vous configurez [!DNL Microsoft 365 Excel] modules, [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. En plus de ces [!DNL Microsoft 365 Excel] peut s’afficher, selon des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, voir [Mappage des informations d’un module à un autre dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Classeur](#workbook)
* [Feuille de travail](#worksheet)
* [Tableau](#table)
* [Autre](#other)

### Classeur

* [Classeurs](#watch-workbooks)
* [Classeurs de recherche](#search-workbooks)
* [Téléchargement d’un classeur](#download-a-workbook)

#### [!UICONTROL Classeurs]

Ce module de déclenchement lance un scénario lorsqu’un classeur est créé.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Office 365] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connectez l’application ou le service Web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td> <p>Sélectionnez le dossier que vous souhaitez consulter pour les nouveaux classeurs.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Filter]</p> </td> 
   <td> <p>Vous pouvez définir un filtre afin de ne surveiller que les classeurs qui répondent aux critères sélectionnés.</p> <p>Pour chaque filtre, saisissez le champ que le filtre doit évaluer, l’opérateur et la valeur que le filtre doit autoriser. Vous pouvez utiliser plusieurs filtres en ajoutant des règles ET ou OU.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td> <p>Saisissez ou mappez le nombre maximal de classeurs que le module doit renvoyer au cours de chaque cycle d’exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Classeurs de recherche]

Ce module d’action recherche [!DNL Excel] classeurs .

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Office 365] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connectez l’application ou le service Web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
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
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td> <p>Saisissez ou mappez le nombre maximal de feuilles de calcul que le module doit renvoyer au cours de chaque cycle d’exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Téléchargement d’un classeur]

Ce module d’action télécharge le contenu du classeur Excel spécifié.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Office 365] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connectez l’application ou le service Web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Télécharger un classeur]</td> 
   <td> <p>Sélectionnez le mode d’identification du classeur à télécharger.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL En saisissant un ID manuellement]</strong> </p> <p>Dans le champ [!UICONTROL ID du classeur], saisissez ou mappez l’identifiant du classeur spécifique que vous souhaitez que le module télécharge.</p> </li> 
     <li> <p><strong>[!UICONTROL En effectuant une sélection depuis le chemin d’accès]</strong> </p> <p>Dans le champ [!UICONTROL Classeur] , sélectionnez le classeur à télécharger par le module.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Feuille de travail

* [[!UICONTROL Lignes de feuille de calcul de contrôle]](#watch-worksheet-rows)
* [[!UICONTROL Liste des feuilles de calcul]](#list-worksheets)
* [[!UICONTROL Lignes de feuille de calcul de liste]](#list-worksheet-rows)
* [[!UICONTROL Ajouter une feuille de calcul]](#add-a-worksheet)
* [[!UICONTROL Ajouter une ligne de feuille de calcul]](#add-a-worksheet-row)
* [[!UICONTROL Mettre à jour une ligne de feuille de calcul]](#update-a-worksheet-row)
* [[!UICONTROL Suppression d’une ligne de feuille de calcul]](#delete-a-worksheet-row)

#### [!UICONTROL Lignes de feuille de calcul de contrôle]

Ce module de déclenchement lance un scénario lorsqu’une nouvelle ligne est ajoutée à la feuille.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Office 365] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connectez l’application ou le service Web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Classeur] </td>
   <td> <p>Sélectionnez le classeur qui contient la feuille de calcul à surveiller pour les nouvelles lignes.</p> </td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL Feuille de calcul] </td>
   <td> <p>Sélectionnez la feuille Excel à surveiller pour les nouvelles lignes.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Limite]</td>
   <td> <p>Saisissez ou mappez le nombre maximal de lignes de feuille de calcul que le module doit renvoyer au cours de chaque cycle d’exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Liste des feuilles de calcul]

Ce module d’action récupère une liste de feuilles de calcul dans le classeur spécifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Office 365] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connectez l’application ou le service Web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Classeur] </td>
   <td> <p>Sélectionnez le classeur qui contient les feuilles de calcul que le module doit répertorier.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Limite]</td>
   <td> <p>Saisissez ou mappez le nombre maximal de feuilles de calcul que le module doit renvoyer au cours de chaque cycle d’exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Lignes de feuille de calcul de liste]

Ce module d’action récupère une liste de lignes dans la feuille de calcul spécifiée.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Office 365] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connectez l’application ou le service Web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL Classeur] </td>
   <td> <p>Sélectionnez le classeur qui contient la feuille de calcul contenant les lignes que vous souhaitez répertorier.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Feuille de calcul] </td>
   <td> <p>Sélectionnez la feuille de calcul qui contient les lignes que vous souhaitez répertorier.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Limite]</td>
   <td> <p>Saisissez ou mappez le nombre maximal de lignes de feuille de calcul que le module doit renvoyer au cours de chaque cycle d’exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ajouter une feuille de calcul]

Ce module d’action crée une nouvelle feuille de calcul dans le classeur sélectionné.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Office 365] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connectez l’application ou le service Web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL Classeur] </td>
   <td> <p>Sélectionnez le classeur dans lequel vous souhaitez ajouter une feuille de calcul.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Name] </td>
   <td> <p>Saisissez ou mappez un nom pour la nouvelle feuille de calcul.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ajouter une ligne de feuille de calcul]

Ce module d’action ajoute une nouvelle ligne à la feuille de calcul sélectionnée.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Office 365] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connectez l’application ou le service Web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Classeur] </td>
   <td> <p>Sélectionnez le classeur qui contient la feuille de calcul dans laquelle vous souhaitez ajouter une ligne.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Feuille de calcul] </td>
   <td> <p>Sélectionnez la feuille de calcul dans laquelle vous souhaitez ajouter une ligne.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Type de valeurs en cours de saisie]</p> </td> 
   <td> <p>Sélectionnez le type de valeur à renseigner dans la feuille de calcul. </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Formules]</strong> </p> <p> Excel tente d’évaluer l’expression spécifiée. Les noms des fonctions d’une formule sont en anglais. Exemple: <code>[!DNL =SUM(A1:A10)]</code></p> </li> 
     <li> <p><strong>[!UICONTROL Formules locales]</strong> </p> <p>Excel tente d’évaluer l’expression spécifiée. Les noms des fonctions sont dans la langue de votre application Excel. Exemple : <code>=SUM(A1, 1.5)</code> vs <code>=SUMME(A1; 1,5)</code></p> </li> 
     <li> <p><strong>[!UICONTROL Value]</strong> </p> <p>Excel n’évalue pas la valeur. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Row]</td>
    <td>Pour chaque colonne, saisissez la valeur que la colonne doit avoir dans la nouvelle ligne.</td>
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mettre à jour une ligne de feuille de calcul]

Ce module d’action met à jour une ligne de feuille de calcul existante.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Office 365] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connectez l’application ou le service Web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Classeur] </td>
   <td> <p>Sélectionnez le classeur qui contient la feuille de calcul contenant la ligne à mettre à jour.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Feuille de calcul] </td>
   <td> <p>Sélectionnez la feuille de calcul contenant la ligne à mettre à jour.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Type de valeurs en cours de saisie]</p> </td> 
   <td> <p>Sélectionnez le type de valeur à renseigner dans la feuille de calcul. </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Formules]</strong> </p> <p> Excel tente d’évaluer l’expression spécifiée. Les noms des fonctions d’une formule sont en anglais. Exemple: <code>[!DNL =SUM(A1:A10)]</code></p> </li> 
     <li> <p><strong>[!UICONTROL Formules locales]</strong> </p> <p>Excel tente d’évaluer l’expression spécifiée. Les noms des fonctions sont dans la langue de votre application Excel. Exemple : <code>=SUM(A1, 1.5)</code> vs <code>=SUMME(A1; 1,5)</code></p> </li> 
     <li> <p><strong>[!UICONTROL Value]</strong> </p> <p>Excel n’évalue pas la valeur. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Identifiant de ligne]</td> 
   <td>Sélectionnez le numéro de la ligne à mettre à jour.</td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Row]</td>
    <td>Pour chaque colonne, saisissez la valeur que la colonne doit avoir dans la nouvelle ligne.</td>
   —&gt; 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Suppression d’une ligne de feuille de calcul]

Ce module d’action supprime une ligne d’une feuille de calcul.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Office 365] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connectez l’application ou le service Web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Classeur] </td>
   <td> <p>Sélectionnez le classeur qui contient la feuille de calcul contenant la ligne à supprimer.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Feuille de calcul]</td>
   <td> <p> Sélectionnez la feuille de calcul contenant la ligne à supprimer.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Identifiant de ligne]</td>
   <td>Saisissez ou mappez l’identifiant de la ligne à supprimer.</td> 
  </tr> 
 </tbody> 
</table>

### Tableau

* [[!UICONTROL Regarder les lignes du tableau]](#watch-table-rows)
* [[!UICONTROL Tableaux de liste]](#list-tables)
* [[!UICONTROL Lignes du tableau de liste]](#list-table-rows)
* [[!UICONTROL Obtention d’un tableau]](#get-a-table)
* [[!UICONTROL Ajouter un tableau]](#add-a-table)
* [[!UICONTROL Ajout d’une ligne de tableau]](#add-a-table-row)
* [[!UICONTROL Mettre à jour une table]](#update-a-table)
* [[!UICONTROL Suppression d’un tableau]](#delete-a-table)

#### [!UICONTROL Regarder les lignes du tableau]

Ce déclencheur lance un scénario lorsqu’une nouvelle ligne est ajoutée à un tableau.

>[!NOTE]
>
>Le tableau ici fait référence à l’élément de tableau incorporé dans le classeur. Pas le tableau entier (classeur/feuille).

![](assets/embedded-table-350x420.png)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Office 365] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connectez l’application ou le service Web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Classeur]</p> </td> 
   <td> <p>Sélectionnez le classeur qui contient le tableau à regarder.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Feuille de calcul] </td>
   <td> <p> Sélectionnez la feuille de calcul contenant le tableau à regarder.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Table]</p> </td> 
   <td> <p>Sélectionnez le tableau à regarder.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Limite]</td>
   <td> <p>Saisissez ou mappez le nombre maximal de lignes que le module doit renvoyer pour chaque cycle d’exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Tableaux de liste]

Ce module de recherche récupère une liste de tous les objets de tableau.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Office 365] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connectez l’application ou le service Web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL Classeur] </td>
   <td> <p>Sélectionnez le classeur qui contient les tableaux que vous souhaitez répertorier.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Feuille de calcul] </td>
   <td> <p>Sélectionnez la feuille de calcul contenant les tables que vous souhaitez répertorier.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Limite]</td>
   <td> <p>Saisissez ou mappez le nombre maximum de tables que le module doit renvoyer pour chaque cycle d'exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Lignes du tableau de liste]

Ce module de recherche récupère une liste de toutes les lignes d’un tableau dans un classeur.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Office 365] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connectez l’application ou le service Web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Classeur] </td>
   <td> <p>Sélectionnez le classeur qui contient le tableau contenant les lignes à répertorier.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Feuille de calcul] </td>
   <td> <p>Sélectionnez la feuille de calcul qui contient le tableau contenant les lignes à répertorier.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Table] </td>
   <td> <p>Sélectionnez le tableau contenant les lignes à répertorier.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Limite]</td>
   <td> <p>Saisissez ou mappez le nombre maximal de lignes de tableau que le module doit renvoyer pour chaque cycle d’exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtention d’un tableau]

Ce module d’action récupère les métadonnées de la table spécifiée.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> 
     <p >[!UICONTROL Connection]</p>
   </td> 
   <td> 
     <p>Pour obtenir des instructions sur la connexion de votre compte Office 365 à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connectez l’application ou le service Web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p>
    --&gt; </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Obtenir une table]</td> 
   <td> <p>Sélectionnez le mode d'identification de la table que vous souhaitez récupérer.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrée manuelle]</strong> </p> <p>Dans le champ [!UICONTROL ID du classeur], saisissez ou mappez l’identifiant du classeur qui contient le tableau que vous souhaitez récupérer.</p> <p>Dans le champ [!UICONTROL Nom de la table], saisissez ou mappez le nom de la table à récupérer.</p> </li> 
     <li> <p><strong>[!UICONTROL Effectuer une sélection dans la liste]</strong> </p> <p>Sélectionnez le classeur et la feuille de calcul qui contiennent le tableau à récupérer, puis sélectionnez le tableau.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ajouter un tableau]

Ce module d’action crée un élément de tableau dans la feuille de calcul Excel.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Office 365] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connectez l’application ou le service Web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Classeur] </td> 
   <td> <p>Sélectionnez le classeur qui contient la feuille de calcul dans laquelle vous souhaitez ajouter un tableau.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Feuille de calcul] </td> 
   <td> <p>Sélectionnez la feuille de calcul dans laquelle vous souhaitez ajouter un tableau.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL En-têtes]</td> 
   <td> <p>Activez cette option pour définir la première ligne comme en-têtes de tableau.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Address]</p> </td> 
   <td> <p>Définissez la taille du tableau en indiquant les cellules supérieure gauche et inférieure droite. Exemple : <code>A1:C10</code> crée un tableau de 3 colonnes et 10 lignes.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ajout d’une ligne de tableau]

Ce module d&#39;action modifie une table existante.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Office 365] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connectez l’application ou le service Web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Classeur] </td>
   <td> <p>Sélectionnez le classeur qui contient le tableau dans lequel vous souhaitez ajouter une ligne.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Feuille de calcul] </td>
   <td> <p>Sélectionnez la feuille de calcul contenant le tableau dans lequel vous souhaitez ajouter une ligne.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Table]</td>
   <td>Sélectionnez le tableau dans lequel vous souhaitez ajouter une rangée.</td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL Row]</td>
    <td>Pour chaque colonne, saisissez la valeur que la colonne doit avoir dans la nouvelle ligne.</td>
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Identifiant de ligne]</p> </td> 
   <td> <p>Pour ajouter une ligne à un emplacement spécifique du tableau, saisissez ou mappez un numéro de ligne. Le module insère la nouvelle ligne après cette ligne.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mettre à jour une table]

Ce module d&#39;action met à jour une table existante.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Office 365] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connectez l’application ou le service Web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mettre à jour une table]</td> 
   <td> <p>Sélectionnez le mode d'identification du tableau à mettre à jour.</p> 
    <ul> 
     <li> <p><strong>Saisir manuellement</strong> </p> <p>Dans le champ [!UICONTROL ID du classeur], saisissez ou mappez l’identifiant du classeur qui contient le tableau à mettre à jour.</p> <p>Dans le champ [!UICONTROL Nom de la table], saisissez ou mappez le nom de la table que vous souhaitez mettre à jour.</p> </li> 
     <li> <p><strong>[!UICONTROL Effectuer une sélection dans la liste]</strong> </p> <p>Sélectionnez le classeur et la feuille de calcul qui contiennent le tableau à mettre à jour, puis sélectionnez le tableau.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Table] </td> 
   <td> <p>Sélectionnez le tableau à mettre à jour.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name]</td> 
   <td> <p>Si vous souhaitez renommer la table, saisissez ou mappez un nouveau nom pour la table.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Afficher les en-têtes]</td> 
   <td> <p>Activez cette option pour afficher les en-têtes du tableau mis à jour.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Afficher les totaux]</td> 
   <td>Activez cette option pour afficher les valeurs totales du tableau.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Style]</td> 
   <td>Choisissez un style pour la nouvelle table.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Suppression d’un tableau]

Ce module d’action supprime la table spécifiée d’une [!DNL Excel] de la feuille de calcul.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Office 365] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connectez l’application ou le service Web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Obtenir une table]</td> 
   <td> <p>Sélectionnez le mode d’identification du tableau à supprimer.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrée manuelle]</strong> </p> <p>Dans le champ [!UICONTROL ID du classeur], saisissez ou mappez l’identifiant du classeur qui contient le tableau à supprimer.</p> <p>Dans le champ [!UICONTROL Nom de la table], saisissez ou mappez le nom de la table à supprimer.</p> </li> 
     <li> <p><strong>[!UICONTROL Effectuer une sélection dans la liste]</strong> </p> <p>Sélectionnez le classeur et la feuille de calcul qui contiennent le tableau à supprimer, puis sélectionnez-le.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Autre

* [[!UICONTROL Récupération des données]](#retrieve-data)
* [[!UICONTROL Lancer un appel API]](#make-an-api-call)

#### [!UICONTROL Récupération des données]

Cette action récupère les données de la plage de feuilles de calcul définie et renvoie un lot pour chaque ligne.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Office 365] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connectez l’application ou le service Web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Classeur] </td> 
   <td> <p>Sélectionnez le classeur qui contient les données à récupérer.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Feuille de calcul] </td> 
   <td> <p>Sélectionnez la feuille de calcul contenant les données que vous souhaitez récupérer.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Range] </td> 
   <td> <p>Spécifiez la zone de la feuille à partir de laquelle vous souhaitez récupérer les données en indiquant les cellules supérieure gauche et inférieure droite. Exemple: <code>A1:D10</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Lancer un appel API]

Ce module d’action vous permet d’effectuer un appel API personnalisé.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Office 365] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connectez l’application ou le service Web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Saisissez un chemin relatif à <code>https://graph.microsoft.com</code>. Exemple:<code> /v1.0/me/drive/root/children</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Méthode [!UICONTROL]</td> 
   td&gt; <p>Sélectionnez la méthode de requête HTTP dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Ajoutez les en-têtes de la requête sous la forme d’un objet JSON standard.</p> <p>Par exemple, <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion ajoute les en-têtes d’autorisation à votre place.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>Ajoutez la requête pour l’appel API sous la forme d’un objet JSON standard.</p> <p>Par exemple : <code>{"name":"something-urgent"}</code></p> </td> 
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
