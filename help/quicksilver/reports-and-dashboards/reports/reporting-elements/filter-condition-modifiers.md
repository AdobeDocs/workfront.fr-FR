---
product-area: reporting
navigation-topic: reporting-elements
title: Modificateurs de filtre et de condition
description: Les modificateurs de filtre et de condition vous permettent de créer des filtres et d’établir des conditions pour formater les résultats de votre rapport.
author: Nolan
feature: Reports and Dashboards
exl-id: 13e9d926-8a89-490e-aa7a-e6e8baf2a36b
source-git-commit: 6bd9dc626befc4dfa4054760e7ec7d677f6da6e5
workflow-type: tm+mt
source-wordcount: '1593'
ht-degree: 91%

---

# Modificateurs de filtre et de condition

<!-- Audited: 11/2024 -->

<!--(NOTE: Alina: This is temporary - Lilit is fixing this in a future story: NOTE If the field you are filtering for has multiple options, this filters out the results that contain only the choice you specify. If the field contains additional options including the one specified, those results are not filtered from the report. See this document and search for "not equal" for the link to the req doc: https://docs.google.com/document/d/1WA0zZ_wws-2qb908i53BFQ8zDwL3nPJHyIybtJvvnqU/edit)-->

Les modificateurs de filtre et de condition vous permettent de créer des filtres et d’établir des conditions pour formater les résultats de votre rapport.

Pour plus d’informations sur la création de filtres, voir l’article [Vue d’ensemble des filtres](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

Pour plus d’informations sur l’utilisation de la mise en forme conditionnelle dans les vues, voir l’article [Utiliser une mise en forme conditionnelle dans les vues](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

## Modificateurs de filtre et de condition

Certains modificateurs sont intégrés et vous pouvez les choisir dans un menu déroulant à l’intérieur de votre filtre ou de votre instruction de mise en forme conditionnelle. D’autres modificateurs ne peuvent être utilisés que dans les filtres de mode texte.

Pour plus d’informations sur le mode texte, voir [Vue d’ensemble du mode texte](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

Pour obtenir une liste des modificateurs de période intégrés, reportez-vous à l’article [Filtrage des rapports par période](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/filter-reports-time-frames.md).

Vous pouvez utiliser les modificateurs de condition suivants dans les filtres et les instructions de mise en forme conditionnelle :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Modificateur intégré</strong> </p> </th> 
   <th> <p><strong>Modificateur de mode texte</strong> </p> </th> 
   <th> <p><strong>Description</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr valign="top"> 
   <td> <p><strong>Est vide</strong> </p> </td> 
   <td> <p><strong>blank</strong> </p> </td> 
   <td> <p>Le champ existe pour l’objet, mais il ne contient actuellement aucune valeur.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>N’est pas vide</strong> </p> </td> 
   <td> <p><strong>notblank</strong> </p> </td> 
   <td> <p>Le champ pour lequel vous filtrez existe et a reçu une valeur.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>null</strong> </p> </td> 
   <td> <p>Le champ est vide ou n’existe pas. Par exemple, vous souhaitez rechercher des éléments sans ID de tâche parent. Cela signifie que vous ne souhaitez afficher que les tâches autonomes. Le qualificateur de l’« ID de tâche parent » serait <strong>null</strong>, puisqu’une tâche sans ID (dans ce cas, le parent) n’existe pas. </p> <p>Ce modificateur ne peut être utilisé que dans les filtres du mode texte. Pour plus d’informations sur le mode texte dans les filtres, voir <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Modifier un filtre à l’aide du mode texte</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notnull</strong> </p> </td> 
   <td> <p>Le champ pour lequel vous filtrez les données existe et contient une valeur qui n’est pas nulle.</p> <p>Ce modificateur ne peut être utilisé que dans les filtres du mode texte. Pour plus d’informations sur le mode texte dans les filtres, voir <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Modifier un filtre à l’aide du mode texte</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Contient</strong> </p> </td> 
   <td> <p><strong>cicontains</strong> </p> </td> 
   <td> <p>Il s’agit de la version <i>non sensible à la casse</i> de <strong>contains</strong>. Par exemple : <code>cicontains inf</code> capture toute valeur qui contient <code>Inf</code> ou <code>inf</code>.</p> <p> <p>Note : Adobe Workfront recherche le mot exact ou l’expression exacte que vous spécifiez pour chaque instruction de filtre. Par exemple, si vous recherchez un projet contenant l’expression <code>new project</code> dans le nom, Workfront n’affiche pas les projets dont le nom ne contiennent que <code>new</code> ou <code>project</code>, ou <code>new main project</code>. Le filtre recherche uniquement les projets dont le nom contient l’expression exacte <code>new project</code>.</p> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Ne contient pas</strong> </p> </td> 
   <td> <p><strong>cinotcontains</strong> </p> </td> 
   <td> <p>Il s’agit de la version <i>non sensible à la casse</i> de <strong>notcontains</strong>.</p><p>Ce modificateur filtre les éléments qui ne contiennent pas la valeur spécifiée.</p> <p>Par exemple : <code>does not contain inf</code> capture tout élément dont le nom ne contient pas <code>Inf</code> ni <code>inf</code>.</p> <p>Remarque : lorsqu’il est appliqué à des champs contenant plusieurs valeurs (par exemple, un ensemble de notes dans un projet), le filtre détermine l’exclusion comme suit :
<ul>
    <li>Si tous les éléments d'une collection contiennent le texte spécifié, l'enregistrement entier est exclu des résultats.</li>
    <li>Si au moins un élément de la collection ne contient pas le texte spécifié, l'enregistrement reste dans les résultats.</li>
</ul>
 </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td> <p><strong>contains</strong> </p> </td> 
   <td> <p> Recherche le texte <i>sensible à la casse</i> spécifié dans toute une chaîne de texte.</p> <p>Par exemple, l’utilisation de <code>contains Inf</code> permet de capturer tout ce qui contient <code>Inf</code>, par exemple, le mot <code>Infinity.</code></p> <p>Ce modificateur ne peut être utilisé que dans les filtres du mode texte. Pour plus d’informations sur le mode texte dans les filtres, voir <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Modifier un filtre à l’aide du mode texte</a>.</p> </td> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notcontains</strong> </p> </td> 
   <td> <p>Cela filtre les éléments qui ne disposent pas de la valeur <i>sensible à la casse</i> spécifiée.</p> <p>Par exemple : <code>notcontains inf</code> capture tout élément sans <code>inf</code>, mais affiche les valeurs qui contiennent <code>Inf</code>.</p> <p>Ce modificateur ne peut être utilisé que dans les filtres de mode texte. Pour plus d’informations sur le mode texte dans les filtres, voir <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Modifier un filtre à l’aide du mode texte</a>.</p> </td> 
  </tr> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cieq</strong> </p> </td> 
   <td> <p>Il s’agit de l’option <i>non sensible à la casse</i> de <strong>eq</strong>. Cela ne renvoie qu’une correspondance exacte de la valeur recherchée.</p> <p>Par exemple, lors de la recherche d’une tâche portant un nom spécifique, <code>task name cieq test</code> recherche les tâches dont le nom est <code>Test</code>, <code>TEST</code> ou <code>Test</code>, mais ne trouve pas de tâche nommée <code>test 123.</code></p> <p>Avec la recherche d’un statut, le modificateur <strong>cieq</strong> n’est pas pris en charge. Vous devez utiliser le modificateur qui respecte la casse, <strong>eq</strong>, pour rechercher un statut.</p> <p>Ce modificateur ne peut être utilisé que dans les filtres de mode texte. Pour plus d’informations sur le mode texte dans les filtres, voir <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Modifier un filtre à l’aide du mode texte</a>.</p> </td>
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td><strong>cine</strong> </td> 
   <td> <p>Il s’agit de l’option <i>non sensible à la casse</i> de <strong>ne</strong>, et est l’inverse du modificateur <b>cieq</b>. Elle renvoie uniquement les résultats qui ne correspondent pas exactement à la valeur recherchée, sans tenir compte de la casse de la valeur.</p> <p>Par exemple, <b>cine</b> renvoie les valeurs qui ne sont pas égales à « current » (en cours) ou à « Current » (En cours). </p> <p>Ce modificateur ne peut être utilisé que dans les filtres du mode texte. Pour plus d’informations sur le mode texte dans les filtres, voir <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Modifier un filtre à l’aide du mode texte</a>.</p> </td> 
  </tr>   <tr valign="top"> 
   <td> </td> 
   <td> <p><strong>eq</strong> </p> </td> 
   <td> <p>Ce modificateur ne renvoie qu’une correspondance exacte <i>sensible à la casse</i> de la valeur recherchée.</p> <p>Par exemple, lors de la recherche de projets complets, <code>eq CPL</code> renvoie tous les projets dont le satut est Complete (Terminé). <code>eq CPL, CUR</code> ne renvoie pas de résultat, car un projet ne peut pas être terminé et en cours en même temps.</p> <p>Ce modificateur ne peut être utilisé que dans les filtres du mode texte. Pour plus d’informations sur le mode texte dans les filtres, voir <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Modifier un filtre à l’aide du mode texte</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td><strong>ne</strong> </td> 
   <td> <p>Il s’agit de l’opposé <i>sensible à la casse</i> de <strong>eq</strong>. Cela renvoie uniquement les résultats qui ne correspondent pas exactement à la valeur recherchée et correspondent également à la casse de la valeur.</p> <p>Par exemple : <b>ne</b> renvoie les valeurs qui ne sont pas égales à « Current », mais ne renvoie aucune valeur qui ne correspond pas à « current ». </p> <p>Ce modificateur ne peut être utilisé que dans les filtres du mode texte. Pour plus d’informations sur le mode texte dans les filtres, voir <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Modifier un filtre à l’aide du mode texte</a>.<br></p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>ciin</strong> </p> </td> 
   <td> <p> Il s’agit de la version <i>non sensible à la casse</i> de <strong>in</strong>.</p> <p>Ce modificateur ne peut être utilisé que dans les filtres du mode texte. Pour plus d’informations sur le mode texte dans les filtres, voir <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Modifier un filtre à l’aide du mode texte</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cinotin</strong> </p> </td> 
   <td> <p>Il s’agit de la version <i>non sensible à la casse</i> de <strong>notin</strong>.</p> <p>Ce modificateur ne peut être utilisé que dans les filtres du mode texte. Pour plus d’informations sur le mode texte dans les filtres, voir <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Modifier un filtre à l’aide du mode texte</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> <p> </p> <p> </p> <p><strong>Equal</strong> </p> </td> 
   <td> <p><strong>in</strong> </p> </td> 
   <td> <p>Ce modificateur vous permet de créer une liste séparée par des virgules de variables <i>sensibles à la casse</i> à comparer à un attribut unique évalué dans un filtre. La liste entière est traitée comme une instruction OU et renvoie les résultats qui répondent aux critères d’une ou de plusieurs des variables.</p> <p>Par exemple, lors de la recherche de projets, l’utilisation de <code>in CUR, PLN, CPL</code> renvoie tous les projets qui ont le statut Current (En cours), OU Planning (Planification), OU Complete (Terminé).</p> <p>Le modificateur intégré <strong>Equal</strong> (Égal à) correspond au modificateur de mode texte de <strong>in</strong>. Cela signifie que vous pouvez sélectionner Equal avec plusieurs valeurs pour le champ.</p> <p>Par exemple, vous pouvez choisir « Status equals Current, Planning, Dead » (Statut égal à En cours, Planification, Immobilisé) dans un rapport de projet et vous pouvez afficher les projets dans n’importe lequel de ces statuts.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Not Equal</strong> </p> </td> 
   <td> <p><strong>notin</strong> </p> </td> 
   <td> <p>Il s’agit de l’opposé <i>sensible à la casse</i> de <strong>in</strong>. Elle renvoie uniquement les résultats qui ne figurent pas dans la liste spécifiée.</p> <p>Ce modificateur ne peut être utilisé que dans les filtres du mode texte. Pour plus d’informations sur le mode texte dans les filtres, voir <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Modifier un filtre à l’aide du mode texte</a>.</p> <p>Note : <span>si le champ pour lequel vous filtrez les données comporte plusieurs options, les résultats qui contiennent à la fois le choix que vous spécifiez, ainsi que le choix que vous spécifiez et les autres choix sont filtrés.</span> </p> </td> 
  </tr>
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>like</strong> </p> </td> 
   <td> <p>Ce modificateur recherche des parties d’une chaîne de texte <i>sensible à la casse</i> de la même manière que <strong>contains</strong>. Cependant, <strong>like</strong> permet d’insérer des caractères génériques pour séparer le texte.</p> <p>Par exemple, lors de la recherche de notes, l’utilisation de <code>like %Current% %Dead%</code> renvoie toute note contenant l’expression « Actuel à inactif ». Elle n’inclut aucune note contenant « Inactif à actuel ». Chaque valeur est recherchée dans l’ordre dans lequel elle est répertoriée. Le % représente un caractère joker pour remplacer des caractères ou des segments de texte. Un trait de soulignement peut également être utilisé pour un seul caractère générique, comme dans <code>like Project_</code> qui renvoie à la fois « Projet » et « Projets ». Si vous envisagez d’utiliser un modificateur <strong>like</strong> ou <strong>clike</strong> dans votre filtrage, nous vous recommandons d’éviter les caractères % ou _ dans les noms de champs de données personnalisés, les valeurs d’option de paramètre ou d’autres noms d’objet.</p><p>Ce modificateur ne peut être utilisé que dans les filtres du mode texte. Pour plus d’informations sur le mode texte dans les filtres, voir <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Modifier un filtre à l’aide du mode texte</a>.</p> </td> 
  </tr>  
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cilike</strong> </p> </td> 
   <td> <p>Il s’agit de la version <i>non sensible à la casse</i> de <strong>like</strong>. Par exemple : <code>cilike %Current% %Dead%</code> renvoie les notes qui contiennent <code>Current to Dead</code> ou <code>current to dead</code>.</p> <p>Ce modificateur ne peut être utilisé que dans les filtres du mode texte. Pour plus d’informations sur le mode texte dans les filtres, voir <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Modifier un filtre à l’aide du mode texte</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td><strong>N’existe pas</strong> </td> 
   <td><strong>NOTEXISTES</strong> </td> 
   <td> <p>Ce modificateur est utilisé uniquement avec des filtres complexes dans une instruction EXISTS. Ces filtres ne font référence qu’aux objets suivants : </p> 
    <ul> 
     <li>Objets s’étendant sur plusieurs niveaux dans la hiérarchie des objets </li> 
     <li>Objets manquants </li> 
    </ul> <p>Pour plus d’informations sur la création de filtres complexes à l’aide d’instructions EXISTS, voir l’article <a href="../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md">Créer des filtres de mode texte complexes à l’aide d’instructions EXISTS</a>. Il s’agit du seul modificateur utilisé dans les instructions EXISTS.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Supérieur à</strong> </p> </td> 
   <td> <p><strong>gt</strong> </p> </td> 
   <td> <p>Cela permet de rechercher tous les résultats dont la valeur est supérieure à la valeur saisie, sans compter la valeur saisie.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Inférieur à</strong> </p> </td> 
   <td> <p><strong>lt</strong> </p> </td> 
   <td> <p>Cela permet de rechercher tous les résultats dont la valeur est inférieure à ce qui est entré, sans compter la valeur saisie.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Supérieur ou égal à</strong> </p> </td> 
   <td> <p><strong>gte</strong> </p> </td> 
   <td> <p>Cela permet de rechercher tous les résultats avec des valeurs supérieures ou égales à la valeur saisie.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Inférieur ou égal à</strong> </p> </td> 
   <td> <p><strong>lte</strong> </p> </td> 
   <td> <p>Cela permet de rechercher tous les résultats dont la valeur est inférieure ou égale à la valeur saisie.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Entre</strong> </p> </td> 
   <td> <p><strong>between</strong> </p> </td> 
   <td> <p>Fournit deux valeurs de champ requises et effectue une recherche pour tous les résultats compris dans la plage des deux champs, y compris les valeurs saisies.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notbetween</strong> </p> </td> 
   <td> <p>Il s’agit de l’inverse de <strong>between</strong>. Elle fournit deux champs de valeur requises et recherche tous les résultats en dehors de la plage des deux champs, y compris les valeurs saisies.</p> <p>Ce modificateur ne peut être utilisé que dans les filtres du mode texte. Pour plus d’informations sur le mode texte dans les filtres, voir <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Modifier un filtre à l’aide du mode texte</a>.</p> </td> 
  </tr>

</tbody> 
</table>
