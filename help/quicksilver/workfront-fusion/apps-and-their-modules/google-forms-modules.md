---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: connector
navigation-topic: apps-and-their-modules
title: Modules Google Forms
description: Le [!DNL Adobe Workfront Fusion Google Forms] Les modules vous permettent de surveiller, sélectionner, ajouter, mettre à jour ou supprimer des réponses sur Google Forms.
author: Becky
feature: Workfront Fusion
exl-id: 45c86879-bc4e-4134-b63c-02410b9de43b
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1382'
ht-degree: 0%

---

# [!DNL Google Forms] modules

Le [!DNL Adobe Workfront Fusion] [!DNL Google Forms] Les modules vous permettent de surveiller, sélectionner, ajouter, mettre à jour ou supprimer des réponses sur vos [!DNL Google Forms].

Pour utiliser [!DNL Google Docs] avec [!DNL Adobe Workfront Fusion], il est nécessaire d’avoir une [!DNL Google] compte . Si vous n’avez pas de [!DNL Google] vous pouvez toutefois en créer un à l’adresse [!DNL Google] Page d’aide du compte.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>Votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</td> 
  </tr> 
 </tbody> 
</table>

Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

Pour plus d’informations sur [!DNL Adobe Workfront Fusion] licences, voir [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Conditions préalables

Pour utiliser [!DNL Google Forms] modules, vous devez disposer d’un [!DNL Google] compte .

## Création d’une feuille de calcul à partir du formulaire

Pour travailler avec vos réponses de formulaire, la feuille de calcul de vos réponses doit être créée.

1. Ouvrez votre formulaire.
1. Accédez au **[!UICONTROL Réponses]** .
1. Cliquez sur le bouton **[!UICONTROL Créer une feuille de calcul]** icon ![](assets/spreadsheet-icon.png).

1. Indiquez si vous souhaitez créer une feuille de calcul ou une feuille de calcul existante.
1. Cliquez sur **[!UICONTROL Créer]**.

## [!DNL Google Forms] modules et leurs champs

Lorsque vous configurez [!DNL Google Forms] modules, [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. En plus de ces [!DNL Google Forms] peut s’afficher, selon des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, voir [Mappage des informations d’un module à un autre dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Actions](#actions)
* [Recherches](#searches)

### Triggers

#### [!UICONTROL Regarder les réponses]

Regarde le formulaire pour trouver de nouvelles réponses.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Google] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connectez l’application ou le service Web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Feuille de calcul]</td> 
   <td> <p>Sélectionnez la feuille de calcul qui contient les réponses du formulaire que vous souhaitez consulter pour les nouvelles réponses.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Feuille]</td> 
   <td> <p> Sélectionnez la feuille contenant les réponses du formulaire.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Rangée avec en-têtes]</td> 
   <td>Spécifiez la rangée d’en-tête du tableau. La ligne par défaut est <code>A1:Z1</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Value Render Option]</td> 
   <td> <p>Indiquez le mode de rendu des valeurs dans la sortie.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Valeur formatée]</strong> </p> <p>Les valeurs sont calculées et formatées dans la réponse selon le formatage de la cellule. Le formatage est basé sur les paramètres régionaux de la feuille de calcul et non sur ceux de l’utilisateur qui la demande. Par exemple, si <code>A1</code> is <code>1. 23</code> et <code>A2 </code>is <code>=A1</code> et formaté en tant que devise, puis <code>A2</code> renvoie <code>$1. 23</code> .</p> </li> 
     <li> <p><strong>[!UICONTROL Valeur non formatée]</strong> </p> <p>Les valeurs sont calculées, mais pas formatées dans la réponse. Par exemple, si <code>A1</code> is <code>1. 23</code> et <code>A2 </code>is <code>=A1</code> et formaté en tant que devise, puis <code>A2</code> renvoie le nombre <code>1. 23</code> .</p> </li> 
     <li> <p><strong>[!UICONTROL Formule]</strong> </p> <p>Les valeurs ne sont pas calculées. La réponse comprend les formules. Par exemple, si <code>A1</code> is <code>1. 23</code> et <code>A2 </code>is <code>=A1</code> et formaté en tant que devise, puis <code>A2</code> renvoie <code>=A1</code>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Option de rendu de date et d’heure]</td> 
   <td>Sélectionnez le mode de représentation des dates, heures et durée dans la sortie. Ce champ est ignoré si [!UICONTROL Value Render Option] est défini sur [!UICONTROL Formatted Value].</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td> <p> Définissez le nombre maximal de réponses qui [!DNL Workfront Fusion] fonctionne avec pendant un cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Actions

* [[!UICONTROL Ajout d’une réponse]](#add-a-response)
* [[!UICONTROL Mise à jour d’une réponse]](#update-a-response)
* [[!UICONTROL Suppression d’une réponse]](#delete-a-response)

#### [!UICONTROL Ajout d’une réponse]

Ce module ajoute une nouvelle réponse au bas de la feuille de calcul du formulaire.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Google] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connectez l’application ou le service Web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Feuille de calcul]</td> 
   <td> <p>Sélectionnez la feuille de calcul contenant la feuille dans laquelle vous souhaitez ajouter une réponse.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Feuille]</td> 
   <td> <p> Sélectionnez la feuille contenant les réponses du formulaire.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Values]</p> </td> 
   <td> <p>Saisissez les valeurs souhaitées dans les colonnes de la feuille.</p> <p>Pour la colonne [!UICONTROL Horodatage] au format correct, utilisez la valeur suivante :</p><pre>formatDate(maintenant;JJ/MM/AAAA HH:mm;UTC)</pre> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Option de saisie de valeur]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p> Les valeurs saisies par l’utilisateur ne sont pas analysées et sont stockées en l’état. </p> </li> 
     <li> <p><strong>[!UICONTROL Utilisateur saisi]</strong></p> <p>Les valeurs sont analysées comme si l’utilisateur les avait saisies dans l’interface utilisateur. Les nombres restent des nombres, mais les chaînes peuvent être converties en nombres, dates ou autres formats suivant les mêmes règles que celles appliquées lors de la saisie de texte dans une cellule via le [!DNL Google Sheets] Interface utilisateur.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Option d’insertion de données]</td> 
   <td> <p>Indiquez le mode de modification des données existantes lors de la saisie de nouvelles données. </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Remplacer]</strong> </p> <p>Les nouvelles données remplacent les données existantes dans les zones où elles sont écrites. L’ajout de données à la fin de la feuille insère de nouvelles lignes ou colonnes afin que les données puissent être écrites.</p> </li> 
     <li> <p><strong>[!UICONTROL Insérer des lignes]</strong></p> <p>Des lignes sont insérées pour les nouvelles données.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mise à jour d’une réponse]

Ce module met à jour la réponse sélectionnée.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Google] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connectez l’application ou le service Web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Feuille de calcul]</td> 
   <td> <p>Sélectionnez la feuille de calcul contenant la feuille dans laquelle vous souhaitez mettre à jour une réponse.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Feuille]</td> 
   <td> <p> Sélectionnez la feuille contenant les réponses du formulaire.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Numéro de ligne]</p> </td> 
   <td> <p>Saisissez ou mappez le nombre de lignes à mettre à jour.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Values]</p> </td> 
   <td> <p>Saisissez les nouvelles valeurs dans les colonnes de votre choix.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Option de saisie de valeur]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p> Les valeurs saisies par l’utilisateur ne sont pas analysées et sont stockées en l’état. </p> </li> 
     <li> <p><strong>[!UICONTROL Utilisateur saisi]</strong></p> <p>Les valeurs sont analysées comme si l’utilisateur les avait saisies dans l’interface utilisateur. Les nombres restent des nombres, mais les chaînes peuvent être converties en nombres, dates ou autres formats suivant les mêmes règles que celles appliquées lors de la saisie de texte dans une cellule via le [!DNL Google Sheets] Interface utilisateur.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Suppression d’une réponse]

Ce module supprime une réponse sélectionnée.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Google] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connectez l’application ou le service Web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Feuille de calcul]</td> 
   <td> <p>Sélectionnez la feuille de calcul contenant la feuille dans laquelle vous souhaitez supprimer une réponse.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Feuille]</td> 
   <td> <p> Sélectionnez la feuille contenant les réponses du formulaire.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Numéro de ligne]</p> </td> 
   <td> <p>Saisissez ou mappez le nombre de lignes à supprimer.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Recherches

* [[!UICONTROL Réponses de recherche]](#search-responses)
* [[!UICONTROL Réponses de recherche (avancées)])](#search-responses-advanced)

#### [!UICONTROL Réponses de recherche]

Ce module renvoie des réponses correspondant aux critères donnés.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
    <td>Connexion</td>
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Google] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connectez l’application ou le service Web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
    <td>[!UICONTROL Feuille de calcul]</td>
   <td> <p>Sélectionnez le formulaire dans lequel vous souhaitez effectuer des recherches.</p> </td> 
  </tr> 
  <tr data-mc-conditions="">
    <td>[!UICONTROL Feuille] </td>
   <td> <p>Sélectionnez la feuille contenant les réponses du formulaire.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
    <td>[!UICONTROL Plage des colonnes]</td>
   <td> <p> Sélectionnez la plage de colonnes à rechercher.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td> <p>Définissez le filtre de recherche des réponses en fonction de .</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
    <td>[!UICONTROL Ordre de tri] </td>
   <td> <p>Choisissez si vous souhaitez trier les réponses renvoyées par ordre croissant ou décroissant.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
    <td>[!UICONTROL Ordre Par]</td>
   <td> <p> Sélectionnez la colonne dans laquelle vous souhaitez classer les réponses renvoyées.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Value Render Option]</td> 
   <td> <p>Indiquez le mode de rendu des valeurs dans la sortie.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Valeur formatée]</strong></p> <p>Les valeurs sont calculées et formatées dans la réponse selon le formatage de la cellule. Le formatage est basé sur les paramètres régionaux de la feuille de calcul et non sur ceux de l’utilisateur qui la demande. Par exemple, si <code>A1</code> is <code>1. 23</code> et <code>A2 </code>is <code>=A1</code> et formaté en tant que devise, puis <code>A2</code> renvoie <code>$1. 23</code> .</p> </li> 
     <li> <p><strong>[!UICONTROL Valeur non formatée]</strong> </p> <p>Les valeurs sont calculées, mais pas formatées dans la réponse. Par exemple, si <code>A1</code> is <code>1. 23</code> et <code>A2 </code>is <code>=A1</code> et formaté en tant que devise, puis <code>A2</code> renvoie le nombre <code>1. 23</code> .</p> </li> 
     <li> <p><strong>[!UICONTROL Formule]</strong> </p> <p>Les valeurs ne sont pas calculées. La réponse comprend les formules. Par exemple, si <code>A1</code> is <code>1. 23</code> et <code>A2 </code>is <code>=A1</code> et formaté en tant que devise, puis <code>A2</code> renvoie <code>=A1</code>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions="">
    <td>[!UICONTROL Option de rendu de date et d’heure]</td>
    <td>Sélectionnez le mode de représentation des dates, heures et durée dans la sortie. Ce champ est ignoré si l’option [!UICONTROL Value Render] est définie sur Valeur formatée. </td>
  </tr> 
  <tr>
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">[!UICONTROL Nombre maximal de réponses renvoyées]</td>
   <td> <p> Définissez le nombre maximal de réponses qui [!DNL Workfront Fusion] renvoie pendant un cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Réponses de recherche (avancées)]

Ce module effectue une recherche à l’aide de la fonction [[!DNL Google Charts Query Language]](https://developers.google.com/chart/interactive/docs/querylanguage). Ce module ne renvoie pas de numéro de ligne.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL Connection]</td>
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Google] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connectez l’application ou le service Web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Feuille de calcul]</td>
   <td> <p>Sélectionnez la feuille de calcul qui contient la feuille à rechercher.</p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Feuille]</td>
   <td> <p> Sélectionnez la feuille contenant les réponses du formulaire.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td> <p>Définissez la requête à l’aide du <a href="https://developers.google.com/chart/interactive/docs/querylanguage">[!DNL Google Charts Query Language]</a>.</p> <p>Exemple : <code>select * where C = "John"</code> récupère toutes les valeurs de la ligne où la colonne C est "John".</p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Nombre maximal de lignes renvoyées]</td>
   <td> <p> Définissez le nombre maximal de réponses qui [!DNL Workfront Fusion] renvoie pendant un cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>
