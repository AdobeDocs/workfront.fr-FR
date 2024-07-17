---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: Connecteur
navigation-topic: apps-and-their-modules
title: Modules Google Forms
description: Les modules  [!DNL Adobe Workfront Fusion Google Forms]  vous permettent de surveiller, sélectionner, ajouter, mettre à jour ou supprimer des réponses sur votre Forms Google.
author: Becky
feature: Workfront Fusion
exl-id: 45c86879-bc4e-4134-b63c-02410b9de43b
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1420'
ht-degree: 19%

---

# Modules [!DNL Google Forms]

Les modules [!DNL Adobe Workfront Fusion] [!DNL Google Forms] vous permettent de surveiller, sélectionner, ajouter, mettre à jour ou supprimer des réponses sur votre [!DNL Google Forms].

Pour utiliser [!DNL Google Docs] avec [!DNL Adobe Workfront Fusion], il est nécessaire d&#39;avoir un compte [!DNL Google]. Si vous n&#39;avez pas encore de compte [!DNL Google], vous pouvez en créer un sur la page d&#39;aide du compte [!DNL Google].

Si vous avez besoin d’instructions sur la création d’un scénario, voir [Créer un scénario dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Pour plus d’informations sur les modules, consultez [Modules dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Conditions d’accès

Pour utiliser les fonctionnalités décrites dans cet article, vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] forfait*</td>
  <td> <p>[!UICONTROL Pro] ou un forfait supérieur</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licence**</td> 
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

## Conditions préalables

Pour utiliser des modules [!DNL Google Forms], vous devez disposer d’un compte [!DNL Google].

## Création d’une feuille de calcul à partir du formulaire

Pour travailler avec vos réponses de formulaire, la feuille de calcul de vos réponses doit être créée.

1. Ouvrez votre formulaire.
1. Accédez à l’onglet **[!UICONTROL Réponses]** .
1. Cliquez sur l’icône **[!UICONTROL Créer une feuille de calcul]** ![](assets/spreadsheet-icon.png) .

1. Indiquez si vous souhaitez créer une feuille de calcul ou une feuille de calcul existante.
1. Cliquez sur **[!UICONTROL Créer]**.

## Modules [!DNL Google Forms] et leurs champs

Lorsque vous configurez des modules [!DNL Google Forms], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. Des champs [!DNL Google Forms] supplémentaires peuvent également s’afficher, en fonction des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, consultez [Mapper les informations d’un module à un autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Déclencheurs](#triggers)
* [Actions](#actions)
* [Recherches](#searches)

### Déclencheurs

#### [!UICONTROL Watch Responses]

Regarde le formulaire pour trouver de nouvelles réponses.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Google] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connexion de l'application du module ou du service Web à [!DNL Workfront Fusion]</a> dans l'article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Créer un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
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
     <li> <p><strong>[!UICONTROL Valeur formatée]</strong> </p> <p>Les valeurs sont calculées et formatées dans la réponse selon le formatage de la cellule. Le formatage est basé sur les paramètres régionaux de la feuille de calcul et non sur ceux de l’utilisateur qui la demande. Par exemple, si <code>A1</code> est <code>1. 23</code> et <code>A2 </code> est <code>=A1</code> et formaté en tant que devise, alors <code>A2</code> renvoie <code>$1. 23</code> .</p> </li> 
     <li> <p><strong>[!UICONTROL Valeur non formatée]</strong> </p> <p>Les valeurs sont calculées, mais pas formatées dans la réponse. Par exemple, si <code>A1</code> est <code>1. 23</code> et <code>A2 </code> est <code>=A1</code> et formaté en tant que devise, alors <code>A2</code> renvoie le nombre <code>1. 23</code> .</p> </li> 
     <li> <p><strong>[!UICONTROL Formule]</strong> </p> <p>Les valeurs ne sont pas calculées. La réponse comprend les formules. Par exemple, si <code>A1</code> est <code>1. 23</code> et <code>A2 </code> est <code>=A1</code> et formaté en tant que devise, alors <code>A2</code> renvoie <code>=A1</code>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Option de rendu de date et d’heure]</td> 
   <td>Sélectionnez le mode de représentation des dates, heures et durée dans la sortie. Ce champ est ignoré si [!UICONTROL Value Render Option] est défini sur [!UICONTROL Formatted Value].</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p> Définissez le nombre maximal de réponses avec lesquelles [!DNL Workfront Fusion] fonctionne au cours d’un cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Actions

* [[!UICONTROL Ajouter une réponse]](#add-a-response)
* [[!UICONTROL Mettre à jour une réponse]](#update-a-response)
* [[!UICONTROL Supprimer une réponse]](#delete-a-response)

#### [!UICONTROL Ajouter une réponse]

Ce module ajoute une nouvelle réponse au bas de la feuille de calcul du formulaire.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Google] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connexion de l'application du module ou du service Web à [!DNL Workfront Fusion]</a> dans l'article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Créer un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
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
     <li> <p><strong>[!UICONTROL Utilisateur saisi]</strong></p> <p>Les valeurs sont analysées comme si l’utilisateur les avait saisies dans l’interface utilisateur. Les nombres restent des nombres, mais les chaînes peuvent être converties en nombres, dates ou autres formats suivant les mêmes règles que celles appliquées lors de la saisie de texte dans une cellule via l’interface utilisateur de [!DNL Google Sheets].</p> </li> 
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

#### [!UICONTROL Mettre à jour une réponse]

Ce module met à jour la réponse sélectionnée.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Google] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connexion de l'application du module ou du service Web à [!DNL Workfront Fusion]</a> dans l'article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Créer un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
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
     <li> <p><strong>[!UICONTROL Utilisateur saisi]</strong></p> <p>Les valeurs sont analysées comme si l’utilisateur les avait saisies dans l’interface utilisateur. Les nombres restent des nombres, mais les chaînes peuvent être converties en nombres, dates ou autres formats suivant les mêmes règles que celles appliquées lors de la saisie de texte dans une cellule via l’interface utilisateur de [!DNL Google Sheets].</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Supprimer une réponse]

Ce module supprime une réponse sélectionnée.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Google] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connexion de l'application du module ou du service Web à [!DNL Workfront Fusion]</a> dans l'article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Créer un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
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
* [[!UICONTROL Réponses de recherche (avancées])](#search-responses-advanced)

#### [!UICONTROL Réponses de recherche]

Ce module renvoie des réponses correspondant aux critères donnés.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
    <td>Connexion</td>
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Google] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connexion de l'application du module ou du service Web à [!DNL Workfront Fusion]</a> dans l'article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Créer un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
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
     <li> <p><strong>[!UICONTROL Valeur formatée]</strong></p> <p>Les valeurs sont calculées et formatées dans la réponse selon le formatage de la cellule. Le formatage est basé sur les paramètres régionaux de la feuille de calcul et non sur ceux de l’utilisateur qui la demande. Par exemple, si <code>A1</code> est <code>1. 23</code> et <code>A2 </code> est <code>=A1</code> et formaté en tant que devise, alors <code>A2</code> renvoie <code>$1. 23</code> .</p> </li> 
     <li> <p><strong>[!UICONTROL Valeur non formatée]</strong> </p> <p>Les valeurs sont calculées, mais pas formatées dans la réponse. Par exemple, si <code>A1</code> est <code>1. 23</code> et <code>A2 </code> est <code>=A1</code> et formaté en tant que devise, alors <code>A2</code> renvoie le nombre <code>1. 23</code> .</p> </li> 
     <li> <p><strong>[!UICONTROL Formule]</strong> </p> <p>Les valeurs ne sont pas calculées. La réponse comprend les formules. Par exemple, si <code>A1</code> est <code>1. 23</code> et <code>A2 </code> est <code>=A1</code> et formaté en tant que devise, alors <code>A2</code> renvoie <code>=A1</code>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions="">
    <td>[!UICONTROL Option de rendu de date et d’heure]</td>
    <td>Sélectionnez le mode de représentation des dates, heures et durée dans la sortie. Ce champ est ignoré si l’option [!UICONTROL Value Render] est définie sur Valeur formatée. </td>
  </tr> 
  <tr>
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">[!UICONTROL Nombre maximal de réponses renvoyées]</td>
   <td> <p> Définissez le nombre maximal de réponses que [!DNL Workfront Fusion] renvoie au cours d’un cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Réponses de recherche (avancées)]

Ce module effectue une recherche à l’aide de [[!DNL Google Charts Query Language]](https://developers.google.com/chart/interactive/docs/querylanguage). Ce module ne renvoie pas de numéro de ligne.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL Connection]</td>
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Google] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connexion de l'application du module ou du service Web à [!DNL Workfront Fusion]</a> dans l'article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Créer un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
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
   <td> <p>Définissez la requête de recherche à l’aide de <a href="https://developers.google.com/chart/interactive/docs/querylanguage">[!DNL Google Charts Query Language]</a>.</p> <p>Exemple : <code>select * where C = "John"</code> récupère toutes les valeurs de la ligne où la colonne C est "John".</p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Nombre maximal de lignes renvoyées]</td>
   <td> <p> Définissez le nombre maximal de réponses que [!DNL Workfront Fusion] renvoie au cours d’un cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>
