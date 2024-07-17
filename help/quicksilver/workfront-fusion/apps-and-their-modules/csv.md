---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
navigation-topic: apps-and-their-modules
title: CSV
description: Les modules CSV Adobe Workfront Fusion vous permettent de créer des fichiers CSV et d’analyser le texte CSV à partir d’une valeur de texte reçue ou d’un fichier.
author: Becky
feature: Workfront Fusion
exl-id: 4e37482a-e84e-4ab2-a48f-7e7bfbecee56
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '995'
ht-degree: 13%

---

# CSV

Les modules [!DNL Adobe Workfront Fusion] [!UICONTROL CSV] vous permettent de créer des fichiers CSV et d’analyser le texte CSV à partir d’une valeur de texte reçue ou d’un fichier.

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
   <p>Exigences de licence héritée : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration], [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
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

## [!UICONTROL Créer un fichier CSV]

L’agrégateur [!UICONTROL Créer un CSV] permet de créer un texte CSV à partir des valeurs de texte reçues.

Pour plus d&#39;informations sur les agrégateurs, voir [Module d&#39;agrégation dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Source Module]</td>
        <td>Sélectionnez le module que vous utilisez pour agréger les champs dont vous avez besoin.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Champs agrégés]</td>
        <td>Sélectionnez les champs que vous souhaitez agréger dans la liste des champs disponibles.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Inclure les en-têtes à la première ligne]</td>
        <td>Sélectionnez cette option pour inclure les en-têtes dans le résultat.</td>
    </tr>
    <tr>
        <td>Groupe [!UICONTROL par]</td>
        <td>Saisissez le filtre pour regrouper les résultats. Par exemple, saisissez une date.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Arrêter le traitement après une agrégation vide]</td>
        <td>Sélectionnez cette option pour arrêter le scénario lorsqu’il n’y a aucun résultat.</td>
    </tr>
</table>

## [!UICONTROL Créer un fichier CSV (avancé)]

L’agrégateur [!UICONTROL Créer un fichier CSV (avancé)] permet de créer un texte CSV à partir des valeurs de texte reçues. Il utilise une structure de données qui définit les colonnes CSV dans le fichier CSV obtenu. Une fois définies, les colonnes apparaissent sous la forme de champs dans la configuration du module CSV et peuvent être mappées à un module ultérieur dans le scénario.

Pour plus d&#39;informations sur les agrégateurs, voir [Module d&#39;agrégation dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source Module]</td> 
   <td>Sélectionnez le module d’application que vous utilisez pour agréger les champs dont vous avez besoin.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data Structure]</td> 
   <td> <p>Sélectionnez la structure de données pour agréger les champs comme vous le souhaitez. Après avoir défini la structure des données, vous pouvez mapper les éléments aux champs correspondants.</p> <p>Pour plus d’informations, voir <a href="../../workfront-fusion/modules/data-structures.md" class="MCXref xref">Structures de données dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inclure les en-têtes à la première ligne] </td> 
   <td>Sélectionnez cette option pour inclure les en-têtes dans le résultat. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Groupe [!UICONTROL par] </td> 
   <td>Saisissez le filtre pour regrouper les résultats. Par exemple, saisissez une date. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Arrêter le traitement après une agrégation vide] </td> 
   <td>Sélectionnez cette option pour arrêter le scénario lorsqu’il n’y a aucun résultat. </td> 
  </tr> 
 </tbody> 
</table>


<p>Supposons que vous souhaitiez exporter vos contacts Google vers un fichier CSV comportant deux colonnes "Nom complet" et "Email". Le lot de sortie du module [!UICONTROL Contacts Google] &gt;[!UICONTROL Obtenir des contacts d’un groupe] possède la structure suivante. Les adresses électroniques sont stockées dans l’élément <code>[!UICONTROL Emails[]]</code>, qui est un tableau de collections, chaque collection contenant deux éléments : <code>Label</code> et <code>Email</code>.</p>
<p> <img src="assets/transforming-350x546.png" style="width: 350;height: 546;"> </p>
<p>Si vous utilisez le module [!DNL Create CSV] simple, une liste de cases à cocher correspondant aux éléments de niveau supérieur d’un lot vous est proposée. Si vous essayez de cocher des éléments <code>Full name</code> et <code>Emails</code>, le module [!UICONTROL Créer CSV] produit la sortie suivante, ce qui n’est probablement pas ce que vous souhaitez :</p>
<p>"emails","fullName"</p>
<p>"[objet]","Shon Winer"</p>
<p>"[objet]", "Lizeth Fulmore"</p>
<p>"[objet]","Hilario Gullatt"</p>
<p>"[objet]","Abby Eisenbarth"</p>
<p>Comme l'élément <code>Full Name</code> est de type Texte simple, il est exporté très bien. Mais l’élément <code>Emails</code>, de type complexe Tableau de collections, est exporté sous la forme [objet Objet], c’est-à-dire que les collections et les tableaux sont transformés en texte par défaut. Pour plus d’informations, voir <a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref">Types de données d’élément dans Adobe Workfront Fusion</a>.</p>
<p>Pour exporter le contenu de l’élément <code>Email </code> de la première collection du tableau <code>Emails[]</code> à la place, il est nécessaire d’utiliser le module [!UICONTROL Créer CSV (avancé)]. Le module vous permet de définir des colonnes individuelles de votre fichier CSV et de leur mapper des éléments, y compris les éléments imbriqués.</p>
<ol>
<li value="1">Insérez le module [!UICONTROL Créer CSV (avancé)] dans un scénario et ouvrez sa configuration.</li>
<li value="2">Cliquez sur le bouton <strong>[!UICONTROL Ajouter]</strong> en regard du champ [!UICONTROL Structure de données] pour créer une nouvelle structure de données.</li>
<li value="3"> <p>Saisissez un nom pour la structure de données et cliquez sur le bouton <strong>[!UICONTROL Ajouter un élément]</strong> pour ajouter les colonnes individuelles. Si vous souhaitez exporter deux colonnes : "Nom complet" et "Email", la structure de données résultante se présenterait comme suit :</p> <p> <img src="assets/google-contacts-350x524.png" style="width: 350;height: 524;"> </p> </li>
<li value="4"> <p>Une fois que vous avez défini la structure de données, les champs correspondant à chaque colonne individuelle doivent apparaître dans la configuration du module [!UICONTROL Créer CSV (avancé)] afin que vous puissiez mapper les éléments. Prenez le premier élément du tableau <code>[!UICONTROL Emails[]]</code> et mappez son élément <code>Email </code> avec le champ/la colonne Email :</p> <p> <img src="assets/create-csv-advanced-350x308.png" style="width: 350;height: 308;"> </p> </li>
<li value="5"> <p>Exécutez le scénario. Puisque l’élément <code>Emails[1]: Email</code> mappé à la colonne "Email" est de type Texte simple, il s’exporte correctement maintenant :</p> <p>"Nom complet", "Email"</p> <p>"Shon Winer","Shon@Winer.com"</p> <p>"Lizeth Fulmore","Lizeth@Fulmore.com"</p> <p>"Hilario Gullatt","Hilario@Gullatt.com"</p> <p>"Abby Eisenbarth","Abby@Eisenbarth.com"</p> </li>
</ol>
</div>

## [!UICONTROL Parse CSV]

Le transformateur [!UICONTROL Parse CSV] permet d’analyser le texte CSV d’une valeur de texte reçue ou d’un fichier.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre de colonnes]</td> 
   <td>Spécifiez le nombre de colonnes dans le fichier CSV.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL CSV contient des en-têtes]</td> 
   <td> <p>Sélectionnez cette option si la première ligne du texte CSV contient des en-têtes.</p> <p>Remarque : Le module n’utilise pas ces en-têtes pour libeller les colonnes de la sortie. Ce champ permet de s’assurer que les en-têtes ne sont pas inclus dans les données de sortie.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL separiterType]</td> 
   <td> <p>Sélectionnez le délimiteur du fichier CSV. Le délimiteur est le caractère de texte qui indique la limite entre des valeurs ou des champs distincts.</p> 
    <ul> 
     <li>[!UICONTROL Virgule]</li> 
     <li>Onglet [!UICONTROL]</li> 
     <li> <p>[!UICONTROL Autre]</p> <p>Si vous sélectionnez [!UICONTROL Autre], saisissez le caractère de délimiteur utilisé par le fichier CSV pour séparer les valeurs. Vous devez saisir exactement un caractère.<br></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conserver les guillemets dans un champ non entre guillemets]</td> 
   <td>Activez cette option pour conserver les guillemets.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL CSV]</td> 
   <td>Saisissez ou mappez le fichier CSV à analyser.<p>Remarque : <p>Si vos données proviennent d’un fichier binaire (généralement d’un fichier), vous devez utiliser la fonction `toString()` pour convertir les données binaires en [!UICONTROL String] :</p><p><img src="assets/parse-csv-350x123.png" style="width: 350;height: 123;"></p></p></td> 
  </tr> 
 </tbody> 
</table>
