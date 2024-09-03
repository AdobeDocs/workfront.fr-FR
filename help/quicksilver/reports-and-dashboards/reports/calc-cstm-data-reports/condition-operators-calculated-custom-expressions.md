---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: Opérateurs de condition dans les expressions personnalisées calculées
description: Vous pouvez utiliser des opérateurs ou des modificateurs de condition lors de la création de données calculées personnalisées dans Adobe Workfront lors de l’utilisation du mode texte.
author: Nolan
feature: Reports and Dashboards
exl-id: ce98ca39-cb86-4ef7-b75c-29ceb916e885
source-git-commit: 639a696c19d79cf2415a45ccb9849ec183fb0bb8
workflow-type: tm+mt
source-wordcount: '718'
ht-degree: 100%

---

# Opérateurs de condition dans les champs personnalisés calculés

<!-- Audited: 2/2024 -->

Vous pouvez utiliser des opérateurs ou des modificateurs de condition lors de la création de données calculées personnalisées dans Adobe Workfront lors de l’utilisation du mode texte. Pour plus d’informations sur l’utilisation du mode texte dans Workfront, voir [Vue d’ensemble du mode texte](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

Les opérateurs ou modificateurs de condition permettent de créer une instruction de condition en connectant des champs Workfront existants dans des instructions et en générant un nouveau champ. L’utilisation la plus courante des opérateurs de condition consiste à créer la condition d’une instruction « IF ».

Vous pouvez utiliser des instructions « IF » dans Workfront pour comparer, formater et associer des champs de données à des fins de création de rapports et de données personnalisées.

Vous pouvez créer des instructions « IF » pour les éléments Workfront suivants :

* Vues
* Regroupements
* Champs personnalisés calculés

Pour plus d’informations sur la création d’instructions « IF », voir [Vue d’ensemble des instructions « IF »](../../../reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md).

Les exemples de ce guide illustrent l’utilisation des opérateurs de condition dans les champs personnalisés calculés. Vous pouvez également les utiliser dans des colonnes ou des regroupements personnalisés calculés en respectant la syntaxe correcte des champs personnalisés calculés dans les rapports.

Pour plus d’informations sur la différence de syntaxe entre les champs personnalisés calculés et les données personnalisées calculées dans les rapports, voir [Champs personnalisés calculés par rapport aux colonnes calculées](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md).

Reportez-vous à l’explorateur d’API pour trouver les champs que vous souhaitez référencer dans vos expressions personnalisées calculées. Pour plus d’informations sur l’explorateur d’API, voir [Explorateur d’API](../../../wf-api/general/api-explorer.md).

Vous pouvez utiliser les modificateurs de condition suivants dans Workfront :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Opérateur de condition</th> 
   <th>Syntaxe de l’opérateur de condition</th> 
   <th>Définition de l’opérateur de condition</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Égal à (non sensible à la casse)</td> 
   <td>= </td> 
   <td> <p>Utilisez cet opérateur pour indiquer que la condition est remplie lorsque le premier champ de votre instruction est égal au second champ.</p> <p>Par exemple, utilisez l’instruction suivante dans un champ personnalisé calculé pour créer une instruction « IF » qui compare la date d’achèvement prévue à la date d’achèvement prévisionnelle d’une tâche : </p><p><code>IF({projectedCompletionDate}={plannedCompletionDate},"On Track","Off Track")</code></p> </td> 
  </tr> 
  <tr> 
   <td>Supérieur à </td> 
   <td>&gt; </td> 
   <td>Utilisez cet opérateur pour indiquer que la condition est remplie lorsque le premier champ de votre instruction est supérieur au second champ. <p>Par exemple, utilisez l’instruction suivante dans un champ personnalisé calculé pour créer une instruction « IF » qui compare la date d’achèvement prévue à la date d’achèvement prévisionnelle d’une tâche : </p><p><code>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"Late","")</code></p></td> 
  </tr> 
  <tr> 
   <td>Est supérieur ou égal à </td> 
   <td>&gt;= </td> 
   <td>Utilisez cet opérateur pour indiquer que la condition est remplie lorsque le premier champ de votre instruction est supérieur ou égal au second champ. <p>Par exemple, utilisez l’instruction suivante dans un champ personnalisé calculé pour créer une instruction « IF » qui compare la date d’achèvement prévue à la date d’achèvement prévisionnelle d’une tâche : </p><p><code>IF({projectedCompletionDate}&gt;={plannedCompletionDate},"Late","Early")</code></p></td> 
  </tr> 
  <tr> 
   <td>Inférieur à </td> 
   <td>&lt; </td> 
   <td>Utilisez cet opérateur pour indiquer que la condition est remplie lorsque le premier champ de votre instruction est inférieur au second champ. <p>Par exemple, utilisez l’instruction suivante dans un champ personnalisé calculé pour créer une instruction « IF » qui compare la date d’achèvement prévue à la date d’achèvement prévisionnelle d’une tâche : </p><p><code>IF({projectedCompletionDate}&lt;{plannedCompletionDate},"Early","")</code></p></td> 
  </tr> 
  <tr> 
   <td>Inférieur ou égal à </td> 
   <td>&lt;= </td> 
   <td>Utilisez cet opérateur pour indiquer que la condition est remplie lorsque le premier champ de votre instruction est inférieur ou égal au second champ. <p>Par exemple, utilisez l’instruction suivante dans un champ personnalisé calculé pour créer une instruction « IF » qui compare la date d’achèvement prévue à la date d’achèvement prévisionnelle d’une tâche : </p><p><code>IF({projectedCompletionDate}&lt;={plannedCompletionDate},"Early","Late")</code></p></td> 
  </tr> 
  <tr> 
   <td>Est différent de </td> 
   <td>! </td> 
   <td> <p>Ajoutez cet opérateur devant l’un des opérateurs ci-dessus pour annuler l’opérateur. </p> <p>Par exemple : </p> 
    <ul> 
     <li>Est égal à : = </li> 
     <li>Est différent de : != </li> 
    </ul> <p>L’ajout de cet opérateur devant les expressions de données suivantes ajoute une instruction négative aux expressions : </p> 
    <ul> 
     <li>CONTIENT </li> 
     <li>DANS </li> 
     <li>IFIN </li> 
     <li>ISBLANK </li> 
    </ul> <p>Pour plus d’informations sur ces expressions de données et pour obtenir une liste complète, voir <a href="../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md" class="MCXref xref">Vue d’ensemble des expressions de données calculées</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>Ou </td> 
   <td>|| </td> 
   <td> <p>Utilisez cet opérateur pour indiquer que la condition est remplie lorsque l’expression trouve la première ou la seconde valeur de votre instruction. </p> <p>Par exemple, utilisez l’instruction suivante dans un champ personnalisé calculé pour créer une instruction « IF » qui marque les projets dont les statuts Actuel ou Planification sont « Actif » : </p><p><code>IF({status}="PLN"||{status}="CUR","Active","Not Active")</code></p> </td> 
  </tr> 
  <tr> 
   <td>Et </td> 
   <td>&amp;&amp; </td> 
   <td> <p>Utilisez cet opérateur pour indiquer que la condition est remplie lorsque l’expression trouve un élément qui répond simultanément à deux conditions. </p> <p>Par exemple, utilisez l’instruction suivante dans un champ personnalisé calculé pour créer une instruction « IF » qui recherche les projets qui sont au statut Actuel et qui ont un statut En danger et les marque comme « médiation nécessaire ». </p><p><code>IF({status}="CUR"&&{condition}="AR","Mediation Needed","")</code></p> </td> 
  </tr> 
 </tbody> 
</table>