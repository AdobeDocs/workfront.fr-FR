---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
navigation-topic: apps-and-their-modules
title: Analyseur de texte
description: Vous pouvez utiliser l’outil d’analyse de texte pour analyser le texte en vue de l’utiliser dans d’autres [!DNL Adobe Workfront Fusion] modules de scénario. L’analyseur de texte ne nécessite pas de connexion.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 7d71cf64-4f86-42c5-81e7-8fc15333cbd7
source-git-commit: 8b4182ae2b32488a02cacc16fcb6a246fcb571fd
workflow-type: tm+mt
source-wordcount: '1044'
ht-degree: 0%

---

# [!UICONTROL Analyseur de texte]

Vous pouvez utiliser la variable [!UICONTROL Outil d’analyse de texte] pour analyser le texte en vue de l’utiliser dans d’autres [!DNL Adobe Workfront Fusion] modules de scénario. Le [!UICONTROL Analyseur de texte] ne nécessite pas de connexion.

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
   <p>Exigences de licence héritées : [!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail, [!UICONTROL [!DNL Workfront Fusion] pour l’automatisation du travail]</p>
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

## [!UICONTROL Analyseur de texte] modules et leurs champs

Lorsque vous configurez [!UICONTROL Analyseur de texte] modules, [!DNL Adobe Workfront Fusion] affiche les champs répertoriés ci-dessous. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, voir [Mappage des informations d’un module à un autre dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Transformers

* [[!UICONTROL Obtention d’éléments à partir d’un HTML]](#get-elements-from-html)
* [[!UICONTROL Obtenir des éléments à partir de texte]](#get-elements-from-text)
* [[!UICONTROL HTML au texte]](#html-to-text)
* [[!UICONTROL Modèle de correspondance]](#match-pattern)
* [[!UICONTROL Remplacer]](#replace)

#### [!UICONTROL Obtention d’éléments à partir d’un HTML]

Récupère les éléments souhaités à partir du code de HTML.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Poursuivre l’exécution de l’itinéraire même si le module ne trouve aucune correspondance]</td> 
   <td> <p>Activez cette option pour vous assurer que le module n’arrête pas le scénario s’il ne renvoie aucun résultat.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Type d’élément]</td> 
   <td> <p> Sélectionnez le type d’élément que vous souhaitez récupérer dans le code du HTML. </p> 
    <ul> 
     <li>[!UICONTROL Image]</li> 
     <li>[!UICONTROL Link]</li> 
     <li>[!UICONTROL Eléments d’iFrame]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL HTML] </td> 
   <td> <p>Saisissez ou mappez le code de HTML à partir duquel vous souhaitez récupérer les types d’éléments spécifiés.</p> </td> 
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
   <td>[!UICONTROL Texte d’entrée]</td> 
   <td> <p>Saisissez ou mappez le texte à analyser.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pattern]</td> 
   <td> <p>Sélectionnez le modèle qui reflète les éléments que vous souhaitez analyser à partir du texte.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ignorer les occurrences en double]</td> 
   <td> <p>Cochez cette case pour ignorer les occurrences en double d’un élément de texte.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL HTML au texte]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL HTML] </td> 
   <td> <p>Saisissez le code de HTML à convertir en texte brut.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Saut de ligne] </td> 
   <td> <p>Sélectionnez le type de saut de ligne (saut de ligne).</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL En-têtes majuscules]</p> </td> 
   <td> <p>Activez cette option pour convertir le texte inclus dans les balises d’en-tête (telles que &lt;h2&gt; &lt;/h2&gt;) en majuscules.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Modèle de correspondance]

Le [!UICONTROL Modèle de correspondance] vous permet de rechercher et d’extraire des éléments de chaîne correspondant à un modèle de recherche à partir d’un texte donné. Ce module utilise des expressions régulières (également appelées regex ou regexp).

Une expression régulière est une séquence de caractères dans laquelle chaque caractère est soit un métacaractère, ayant une signification spéciale, soit un caractère normal ayant une signification littérale. Ces caractères et métacaractères identifient un modèle qui peut être utilisé pour rechercher du texte. Par exemple, si vous souhaitez rechercher des noms, vous pouvez configurer une expression régulière pour rechercher un modèle constitué de deux mots consécutifs commençant par des majuscules. Les expressions régulières sont un puissant outil de recherche et de manipulation de texte.

Le présent article ne vise pas à aborder la question des expressions régulières. Nous vous recommandons les ressources suivantes :

* Pour obtenir la liste complète des métacaractères, voir [Expressions régulières](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions) dans la documentation web MDN.
* Pour un tutoriel sur la création d’expressions régulières, nous vous recommandons de [RegexOne](https://regexone.com/).
* Pour expérimenter des expressions régulières, nous vous recommandons le [Expressions régulières 101](https://regex101.com/) site web. Sélectionnez l’INDICATEUR ECMAScript (JavaScript) dans le panneau de gauche.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Pattern] </td> 
   <td> <p>Saisissez le modèle d’expression régulière. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemple : </b></span></span> <code>[+-]?(\d+(\.\d+)?|\.\d+)([eE][+-]?\d+)?</code> extrait tous les chiffres du texte fourni.</p> <p>Note:  <p>Le modèle doit contenir au moins un groupe de capture entre parenthèses. <code>()</code>. Si le modèle ne contient aucun groupe de capture, le lot de sortie est vide.</p> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Correspondance globale]</td> 
   <td> <p>Activez cette option pour récupérer toutes les correspondances dans le texte. Chaque correspondance est générée dans un lot distinct. Si cette option est désactivée, le module récupère uniquement la première entrée.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Respect de la casse]</td> 
   <td> <p> Activez cette option pour que ce module traite le texte comme sensible à la casse.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Multiligne] </td> 
   <td> <p>Activez cette option pour vous assurer que les métacaractères de début et de fin (<code>^</code> et <code>$</code>) correspond au début ou à la fin de chaque ligne, et pas seulement au début ou à la fin de l’ensemble de la chaîne d’entrée.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL mono-ligne]</td> 
   <td>Activez cette option pour vous assurer que le point (.) correspond aux caractères de saut de ligne (<code>\n</code>).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Poursuivre l’exécution de l’itinéraire même si le module ne renvoie aucun résultat]</td> 
   <td> <p>Activez cette option pour vous assurer que le module n’arrête pas le scénario s’il ne renvoie aucun résultat.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Texte] </td> 
   <td> <p>Saisissez ou mappez le texte que vous souhaitez faire correspondre au modèle.</p> </td> 
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
   <td> <p>Saisissez le terme à rechercher. Vous pouvez également utiliser une expression régulière. Pour plus d’informations sur l’expression régulière, reportez-vous à la section <a href="#match-pattern" class="MCXref xref">[!UICONTROL Modèle de correspondance]</a> module .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nouvelle valeur]</td> 
   <td> <p> Saisissez une valeur qui remplace le terme recherché.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Correspondance globale]</td> 
   <td> <p>Activez cette option pour récupérer toutes les correspondances dans le texte. Chaque correspondance est générée dans un lot distinct. Si cette option est désactivée, le module récupère uniquement la première entrée.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Respect de la casse]</td> 
   <td> <p> Activez cette option pour que ce module traite le texte comme sensible à la casse.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Multiligne] </td> 
   <td> <p>Activez cette option pour vous assurer que les métacaractères de début et de fin (<code>^</code> et <code>$</code>) correspond au début ou à la fin de chaque ligne, et pas seulement au début ou à la fin de l’ensemble de la chaîne d’entrée.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL mono-ligne]</td> 
   <td>Activez cette option pour vous assurer que le point (.) correspond aux caractères de saut de ligne (<code>\n</code>).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Texte] </td> 
   <td> <p>Saisissez le texte à rechercher.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Nettoyage des données

La récupération de données, parfois appelée raclage Web, extraction de données ou récupération Web, est le processus de collecte de données à partir de sites Web et de stockage de données dans votre base de données ou feuille de calcul locale. Si vous souhaitez récupérer des données d’un site web et que vous ne connaissez pas les expressions régulières, vous pouvez utiliser un outil de récupération de données.

Si l’outil de récupération des données fournit une API REST, vous pouvez vous y connecter via notre [[!UICONTROL HTTP] modules](../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md) et [Webhooks](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md) modules.
