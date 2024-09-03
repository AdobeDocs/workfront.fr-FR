---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
navigation-topic: apps-and-their-modules
title: Analyseur de texte
description: Vous pouvez utiliser l’outil d’analyse de texte pour analyser le texte en vue de l’utiliser dans d’autres modules de scénario  [!DNL Adobe Workfront Fusion] . L’analyseur de texte ne nécessite pas de connexion.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 7d71cf64-4f86-42c5-81e7-8fc15333cbd7
source-git-commit: 8b4182ae2b32488a02cacc16fcb6a246fcb571fd
workflow-type: tm+mt
source-wordcount: '1034'
ht-degree: 100%

---

# [!UICONTROL Analyseur de texte]

Vous pouvez utiliser l’[!UICONTROL outil d’analyse de texte] pour analyser le texte en vue de l’utiliser dans d’autres modules de scénario [!DNL Adobe Workfront Fusion]. L’[!UICONTROL analyseur de texte] ne nécessite pas de connexion.

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
   <p>Conditions requises du produit actuel : si vous disposez de la formule [!DNL Adobe Workfront] [!UICONTROL Select] ou [!UICONTROL Prime], votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article. [!DNL Workfront Fusion] est inclus dans la formule [!DNL Workfront] [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Exigences liées aux produits hérités : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi qu’[!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez votre équipe d’administration [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], voir Licences [[!DNL Adobe Workfront Fusion] ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Modules de l’[!UICONTROL analyseur de texte] et leurs champs

Lorsque vous configurez les modules de l’[!UICONTROL analyseur de texte], [!DNL Adobe Workfront Fusion] affiche les champs répertoriés ci-dessous. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton « Mapper » apparaît au-dessus d’un champ ou d’une fonction, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, voir [Mapper des informations d’un module à un autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Transformateurs

* [[!UICONTROL Obtenir des éléments à partir de HTML]](#get-elements-from-html)
* [[!UICONTROL Obtenir des éléments à partir de texte]](#get-elements-from-text)
* [[!UICONTROL HTML vers texte]](#html-to-text)
* [[!UICONTROL Motif correspondant]](#match-pattern)
* [[!UICONTROL Remplacer]](#replace)

#### [!UICONTROL Obtenir des éléments à partir de HTML]

Récupère les éléments souhaités à partir du code HTML.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Continue the execution of the route even if the module finds no matches]</td> 
   <td> <p>Activez cette option pour vous assurer que le module n’arrête pas le scénario s’il ne renvoie aucun résultat.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Element type]</td> 
   <td> <p> Sélectionnez le type d’élément que vous souhaitez récupérer dans le code HTML. </p> 
    <ul> 
     <li>[!UICONTROL Image]</li> 
     <li>[!UICONTROL Link]</li> 
     <li>[!UICONTROL iFrame element(s)]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL HTML] </td> 
   <td> <p>Saisissez ou mappez le code HTML à partir duquel vous souhaitez récupérer les types d’éléments spécifiés.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtenir des éléments à partir de texte]

Analyse les éléments du texte en fonction du modèle donné.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Input text]</td> 
   <td> <p>Saisissez ou mappez le texte à analyser.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pattern]</td> 
   <td> <p>Sélectionnez le motif qui reflète les éléments que vous souhaitez analyser à partir du texte.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ignore Duplicate Occurrences]</td> 
   <td> <p>Cochez cette case pour ignorer les occurrences en double d’un élément de texte.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL HTML en texte]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL HTML] </td> 
   <td> <p>Saisissez le code HTML à convertir en texte brut.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Line break] </td> 
   <td> <p>Sélectionnez le type de nouvelle ligne (saut de ligne).</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Uppercase headings]</p> </td> 
   <td> <p>Activez cette option pour convertir le texte inclus dans les balises d’en-tête (telles que &lt;h2&gt; &lt;/h2&gt;) en texte en majuscules.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Motif correspondant]

Le module [!UICONTROL Motif correspondant] vous permet de rechercher et d’extraire des éléments de chaîne de caractères correspondant à un motif de recherche d’un texte donné. Ce module utilise des expressions régulières (également appelées regex ou regexp).

Une expression régulière est une séquence de caractères dans laquelle chaque caractère est soit un métacaractère, ayant une signification spéciale, soit un caractère régulier ayant une signification littérale. Ces caractères et métacaractères identifient un motif qui peut être utilisé pour rechercher du texte. Par exemple, si vous souhaitez rechercher des noms, vous pouvez configurer une expression régulière pour rechercher un motif constitué de deux mots consécutifs commençant par des majuscules. Les expressions régulières sont un puissant outil de recherche et de manipulation de texte.

Le présent article ne vise pas à aborder la question des expressions régulières. Nous vous recommandons les ressources suivantes :

* Pour obtenir la liste complète des métacaractères, voir [Expressions régulières](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions) dans la documentation web MDN.
* Pour un tutoriel sur la création d’expressions régulières, nous vous recommandons [RegexOne](https://regexone.com/).
* Pour expérimenter des expressions régulières, nous vous recommandons le site web [Regular Expressions 101](https://regex101.com/). Sélectionnez le ECMAScript (JavaScript) FLAVOR dans le panneau de gauche.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Pattern] </td> 
   <td> <p>Saisissez le motif d’expression régulière. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemple : </b></span></span> <code>[+-]?(\d+(\.\d+)?|\.\d+)([eE][+-]?\d+)?</code> extrait tous les chiffres du texte fourni.</p> <p>Note :  <p>Le motif doit contenir au moins un groupe de capture entre parenthèses <code>()</code>. Si le motif ne contient aucun groupe de capture, le lot de sortie est vide.</p> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Global match]</td> 
   <td> <p>Activez cette option pour récupérer toutes les correspondances dans le texte. Chaque correspondance est générée dans un lot distinct. Si cette option est désactivée, le module récupère uniquement la première entrée.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Case sensitive]</td> 
   <td> <p> Activez cette option pour que ce module traite le texte comme étant sensible à la casse.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Multiline] </td> 
   <td> <p>Activez cette option pour vous assurer que les métacaractères de début et de fin (<code>^</code> et <code>$</code>) correspondent au début ou à la fin de chaque ligne, et pas seulement au début ou à la fin de l’ensemble de la chaîne de caractères d’entrée.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Singleline]</td> 
   <td>Activez cette option pour vous assurer que le point (.) correspond aux caractères de saut de ligne (<code>\n</code>).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Continue the execution of the route even if the module returns no results]</td> 
   <td> <p>Activez cette option pour vous assurer que le module n’arrête pas le scénario s’il ne renvoie aucun résultat.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Text] </td> 
   <td> <p>Saisissez ou mappez le texte que vous souhaitez faire correspondre au motif.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Remplacer]

Recherche une valeur ou une expression régulière dans le texte saisi et remplace le résultat par la nouvelle valeur.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Pattern] </td> 
   <td> <p>Saisissez le terme de recherche. Vous pouvez également utiliser une expression régulière. Pour plus d’informations sur l’expression régulière, voir le module <a href="#match-pattern" class="MCXref xref">[!UICONTROL Match Pattern]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL New value]</td> 
   <td> <p> Saisissez une valeur qui remplace le terme recherché.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Global match]</td> 
   <td> <p>Activez cette option pour récupérer toutes les correspondances dans le texte. Chaque correspondance est générée dans un lot distinct. Si cette option est désactivée, le module récupère uniquement la première entrée.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Case sensitive]</td> 
   <td> <p> Activez cette option pour que ce module traite le texte comme étant sensible à la casse.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Multiline] </td> 
   <td> <p>Activez cette option pour vous assurer que les métacaractères de début et de fin (<code>^</code> et <code>$</code>) correspondent au début ou à la fin de chaque ligne, et pas seulement au début ou à la fin de l’ensemble de la chaîne de caractères d’entrée.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Singleline]</td> 
   <td>Activez cette option pour vous assurer que le point (.) correspond aux caractères de saut de ligne (<code>\n</code>).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Text] </td> 
   <td> <p>Saisissez le texte à rechercher.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Récupération de données

La récupération de données, parfois appelée web scraping, extraction des données ou web harvesting, est le processus de collecte de données à partir de sites web et de stockage de ces données dans votre base de données ou feuille de calcul locale. Si vous souhaitez récupérer les données d’un site web et que vous ne connaissez pas les expressions régulières, vous pouvez utiliser un outil de récupération de données.

Si l’outil de récupération de données fournit une API REST, vous pouvez vous y connecter via nos [[!UICONTROL modules HTTP]](../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md) et [Webhooks](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md) universels.
