---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
navigation-topic: apps-and-their-modules
title: CSV
description: La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement. Cet article est obsolète, mais contient un lien vers le nouvel article qui couvre cette fonctionnalité.
author: Becky
feature: Workfront Fusion
exl-id: 4e37482a-e84e-4ab2-a48f-7e7bfbecee56
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '1044'
ht-degree: 90%

---

# CSV

>[!IMPORTANT]
>
>La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement.
>
>Les informations contenues dans cet article se trouvent désormais dans l’article :
>
>* [CSV](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/tools-and-transformers/csv.html)
>
>Mettez à jour les signets.
>
>Cet article n’est plus mis à jour et sera supprimé prochainement.

Les modules [!UICONTROL CSV] d’[!DNL Adobe Workfront Fusion] vous permettent de créer des fichiers CSV et d’analyser du texte CSV à partir d’une valeur textuelle reçue ou d’un fichier.

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
   <p>Exigences en matière de licences héritées : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration], [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Exigences actuelles du produit : si vous disposez du plan de [!DNL Adobe Workfront] [!UICONTROL Select] ou [!UICONTROL Prime], votre entreprise doit acheter du [!DNL Adobe Workfront Fusion] et [!DNL Adobe Workfront] utiliser les fonctionnalités décrites dans cet article. [!DNL Workfront Fusion] est inclus dans la formule [!DNL Workfront] [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Exigences liées aux produits hérités : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi qu’[!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez votre équipe d’administration [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], consultez la section Licences [[!DNL Adobe Workfront Fusion] ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL Créer un CSV]

L’agrégateur [!UICONTROL Créer CSV] vous permet de créer un texte CSV à partir de valeurs de texte reçues.

Pour plus d’informations sur les agrégateurs, consultez [Module d’agrégateur dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Source Module]</td>
        <td>Sélectionnez le module que vous utilisez pour agréger les champs dont vous avez besoin.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Aggregated Fields]</td>
        <td>Sélectionnez les champs que vous souhaitez agréger dans la liste des champs disponibles.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Include headers in the first row]</td>
        <td>Sélectionnez cette option pour inclure les en-têtes dans le résultat.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Group by]</td>
        <td>Saisissez le filtre pour grouper les résultats. Par exemple, saisissez une date.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Stop processing after an empty aggregation]</td>
        <td>Sélectionnez cette option pour arrêter le scénario lorsqu’il n’y a aucun résultat.</td>
    </tr>
</table>

## [!UICONTROL Créer un CSV (avancé)]

L’agrégateur [!UICONTROL Créer un CSV (avancé)] vous permet de créer un texte CSV à partir de valeurs de texte reçues. Il utilise une structure de données qui définit les colonnes CSV dans le fichier CSV résultant. Une fois définies, les colonnes apparaissent comme des champs dans la configuration du module CSV et peuvent être mappées à d’autres modules du scénario.

Pour plus d’informations sur les agrégateurs, consultez [Module d’agrégateur dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source Module]</td> 
   <td>Sélectionnez le module de l’application que vous utilisez pour agréger les champs dont vous avez besoin.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data Structure]</td> 
   <td> <p>Sélectionnez la structure de données pour agréger les champs comme vous le souhaitez. Après avoir défini la structure des données, vous pouvez mapper les éléments aux champs correspondants.</p> <p>Pour plus d’informations, consultez <a href="../../workfront-fusion/modules/data-structures.md" class="MCXref xref">Structures de données dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Include headers in the first row] </td> 
   <td>Sélectionnez cette option pour inclure les en-têtes dans le résultat. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Group by] </td> 
   <td>Saisissez le filtre pour grouper les résultats. Par exemple, saisissez une date. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Stop processing after an empty aggregation] </td> 
   <td>Sélectionnez cette option pour arrêter le scénario lorsqu’il n’y a aucun résultat. </td> 
  </tr> 
 </tbody> 
</table>


<p>Supposons que vous souhaitiez exporter vos contacts Google vers un fichier CSV comportant deux colonnes « Nom complet » et « E-mail ». Le lot de sortie du module [!UICONTROL Google Contacts] &gt; [!UICONTROL Get contacts from a group] a la structure suivante. Les adresses e-mail sont stockées dans l’élément <code>[!UICONTROL Emails[]]</code>, qui est un tableau de collections, chaque collection contenant deux éléments : <code>Label</code> et <code>Email</code>.</p>
<p> <img src="assets/transforming-350x546.png" style="width: 350;height: 546;"> </p>
<p>Si vous utilisez le module simple [!DNL Create CSV], vous obtenez une liste de cases à cocher correspondant aux éléments de premier niveau d’un lot. Si vous essayez de cocher les éléments <code>Full name</code> et <code>Emails</code>, le module [!UICONTROL Create CSV] produit la sortie suivante, qui n’est probablement pas ce que vous souhaitez :</p>
<p>"emails","fullName"</p>
<p>"[object Object]","Shon Winer"</p>
<p>"[object Object]","Lizeth Fulmore"</p>
<p>"[object Object]","Hilario Gullatt"</p>
<p>"[object Object]","Abby Eisenbarth"</p>
<p>L’élément <code>Full Name</code> étant de type simple Texte, il est exporté sans problème. Mais l’élément <code>Emails</code>, qui est d’un type complexe Tableau de collections, est exporté sous la forme [object Object], ce qui correspond à la façon dont les Collections et les Tableaux sont transformés en texte par défaut. Pour plus d’informations, voir <a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref">Types de données d’éléments dans Adobe Workfront Fusion</a>.</p>
<p>Pour exporter le contenu de l’élément <code>Email </code>de la première collection du tableau <code>Emails[]</code>, il est nécessaire d’utiliser le module [!UICONTROL Create CSV (advanced)]. Le module vous permet de définir des colonnes individuelles de votre fichier CSV et d’y affecter des éléments, y compris les colonnes imbriquées.</p>
<ol>
<li value="1">Insérez le module [!UICONTROL Create CSV (advanced)] dans un scénario et ouvrez sa configuration.</li>
<li value="2">Cliquez sur le bouton <strong>[!UICONTROL Add]</strong> à côté du champ [!UICONTROL Data structure] pour créer une nouvelle structure de données.</li>
<li value="3"> <p>Donnez un nom à la structure de données et cliquez sur le bouton <strong>[!UICONTROL Add item]</strong> pour ajouter les différentes colonnes. Si vous souhaitez exporter deux colonnes : « Nom complet » et « E-mail », la structure de données résultante ressemblerait à ceci :</p> <p> <img src="assets/google-contacts-350x524.png" style="width: 350;height: 524;"> </p> </li>
<li value="4"> <p>Une fois que vous avez défini avec succès la structure des données, les champs correspondant à chaque colonne devraient apparaître dans la configuration du module [!UICONTROL Create CSV (advanced)] afin que vous puissiez mapper les éléments. Prenez le premier élément du tableau <code>[!UICONTROL Emails[]]</code> et associez son élément <code>Email </code> au champ/colonne E-mail :</p> <p> <img src="assets/create-csv-advanced-350x308.png" style="width: 350;height: 308;"> </p> </li>
<li value="5"> <p>Exécutez le scénario. Comme l’élément <code>Emails[1]: Email</code> mappé à la colonne « E-mail » est de type simple Texte, il est maintenant exporté correctement :</p> <p>« Nom complet », « E-mail »</p> <p>"Shon Winer","Shon@Winer.com"</p> <p>"Lizeth Fulmore","Lizeth@Fulmore.com"</p> <p>"Hilario Gullatt","Hilario@Gullatt.com"</p> <p>"Abby Eisenbarth","Abby@Eisenbarth.com"</p> </li>
</ol>
</div>

## [!UICONTROL Analyse CSV]

Le transformateur [!UICONTROL Analyse CSV] vous permet d’analyser un texte CSV à partir d’une valeur textuelle reçue ou d’un fichier.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number of columns]</td> 
   <td>Indiquez le nombre de colonnes dans le fichier CSV.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL CSV contains headers]</td> 
   <td> <p>Sélectionnez cette option si la première ligne du texte CSV contient des en-têtes.</p> <p>Note : le module n’utilise pas ces en-têtes pour étiqueter les colonnes dans le résultat. En revanche, ce champ garantit que les en-têtes ne sont pas inclus dans les données de sortie.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL delimiterType]</td> 
   <td> <p>Sélectionnez le délimiteur pour le fichier CSV. Le délimiteur est le caractère de texte qui indique la limite entre des valeurs ou des champs distincts.</p> 
    <ul> 
     <li>[!UICONTROL Comma]</li> 
     <li>[!UICONTROL Tab]</li> 
     <li> <p>[!UICONTROL Other]</p> <p>Si vous sélectionnez [!UICONTROL Other], saisissez le caractère de délimitation que le fichier CSV utilise pour séparer les valeurs. Vous devez saisir exactement un caractère.<br></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Preserve quotes inside unquoted field]</td> 
   <td>Activez cette option pour conserver les quillemets.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL CSV]</td> 
   <td>Saisissez ou mappez le fichier CSV que vous souhaitez analyser.<p>Note : <p>Si vos données sont sous forme binaire (typiquement à partir d’un fichier), vous devez utiliser la fonction toString() pour convertir les données binaires en [!UICONTROL String] :</p><p><img src="assets/parse-csv-350x123.png" style="width: 350;height: 123;"></p></p></td> 
  </tr> 
 </tbody> 
</table>
