---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: Vue d’ensemble des expressions de données calculées
description: Vous pouvez utiliser des expressions de données pour définir des champs de données personnalisées calculés dans Adobe Workfront. Les expressions calculées connectent des champs Workfront existants dans des instructions qui génèrent un nouveau champ.
author: Nolan
feature: Reports and Dashboards
exl-id: cfb3ace9-76c3-4006-878f-e2ad25ffa03b
source-git-commit: e66d4223b13bcd4813156f147769e7ee99c3f8ef
workflow-type: tm+mt
source-wordcount: '2425'
ht-degree: 90%

---

# Vue d’ensemble des expressions de données calculées

<!--Audited: 12/2023-->

Vous pouvez utiliser des expressions de données pour définir des champs personnalisées calculés dans Adobe Workfront. Les expressions calculées connectent des champs Workfront existants dans des instructions qui génèrent un nouveau champ.

Vous pouvez utiliser des expressions de données calculés dans :

* Un champ personnalisé calculé sur un formulaire personnalisé

  Pour plus d’informations sur la création de champs calculés personnalisés sur des formulaires personnalisés dans Workfront, voir [Ajouter des champs calculés à un formulaire](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

* Une colonne personnalisée calculée dans un rapport ou une liste lorsque vous utilisez le mode texte

  Pour plus d’informations sur l’utilisation du mode texte dans les rapports et les vues, voir [Vue d’ensemble du mode texte](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Syntaxe des champs personnalisés calculés par rapport aux colonnes personnalisées calculées

Bien que les fonctions que vous utilisez soient les mêmes, la syntaxe de création d’une expression dans un champ personnalisé calculé peut être différente de celle utilisée pour créer une colonne personnalisée calculée.

Les différences entre les deux syntaxes sont les suivantes :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Champ personnalisé calculé</strong></td> 
   <td><strong>Élément de rapport personnalisé calculé</strong></td> 
  </tr> 
   <td>Placez les noms de champ entre accolades.</td> 
   <td>Ne placez pas les noms de champ entre crochets ou parenthèses lors de leur utilisation dans une <p><code>valuefield </code></p>ligne. <p>Placez les noms de champ entre accolades lorsque vous les utilisez dans une <p><code>valueexpression</code></p> ligne.</p> </td> 
  </tr> 
  <tr> 
   <td>Séparer les champs par des points</td> 
   <td> <p>Séparez les champs par deux-points lors de leur utilisation dans une <p><code>valuefield </code></p>ligne.</p> <p>Séparez les champs par des points lors de leur utilisation dans une <p><code>valueexpression </code></p>ligne. </p> </td> 
  </tr> 
 </tbody> 
</table>

Par exemple :

* Dans un champ personnalisé, sur un formulaire personnalisé pour les tâches, vous utiliserez les éléments suivants pour générer le nom du projet parent de la tâche à laquelle le formulaire personnalisé est joint :


  ` {project}.{name}`


* Dans une colonne personnalisée d’un rapport, vous pouvez utiliser les éléments suivants pour ajouter une colonne personnalisée Nom du projet à un rapport de tâche :


  `valuefield=project:name`


  Ou

  `valueexpression={project}.{name}`


  >[!TIP]
  >
  >La même syntaxe s’applique à tous les éléments de rapport en mode texte dans lesquels des expressions calculées sont utilisées : vues, filtres, regroupements et invites.

Pour plus d’informations sur la syntaxe que vous devez utiliser dans une colonne personnalisée calculée, voir [Vue d’ensemble du mode texte](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Expressions de données utilisables

Les listes ci-dessous définissent les expressions disponibles que vous pouvez utiliser lorsque vous créez l’un des trois types différents de champs personnalisés calculés dans Workfront :

* [Champs personnalisés calculés par date et heure](#date-time-calculated-custom-fields)
* [Champs personnalisés calculés mathématiquement](#mathematical-calculated-custom-fields)
* [Champs personnalisés calculés avec du texte](#text-calculated-custom-fields)

Vous pouvez utiliser les expressions répertoriées ci-dessous pour créer des colonnes calculées personnalisées. Cependant, vous devez utiliser la syntaxe correcte pour une colonne personnalisée calculée, comme décrit dans la section [Syntaxe des champs personnalisés calculés par rapport aux colonnes personnalisées calculées](#syntax-of-calculated-custom-fields-vs-calculated-custom-columns) dans cet article.

### Champs personnalisés calculés par date et heure {#date-time-calculated-custom-fields}

>[!NOTE]
>
>Si vous créez un calcul de date et heure qui n’inclut pas de partie horaire ou qui utilise les caractères génériques $$TODAY ou $$NOW, le système utilise la date selon le fuseau horaire universel coordonné (UTC), et non selon votre fuseau horaire local. Cela peut entraîner un résultat de date inattendu.

Vous pouvez créer un champ personnalisé calculé par date ou heure à l’aide des expressions suivantes :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Expression...</th> 
   <th>Explication et exemple</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>ADDDAYS</strong> </td> 
   <td> <p>Ajoute le nombre de jours à la date. La valeur du nombre peut inclure des jours partiels. Par exemple, 1.5 ajoute un jour et demi à la date.</p> <p>L’expression est formatée comme suit :</p>

<p><code>ADDDAYS(date, number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDWEEKDAYS</strong> </td> 
   <td> <p>Ajoute le nombre de jours de la semaine à la date. Cette expression ajoute uniquement des valeurs entières à la date, en arrondissant à l’unité inférieure. </p> <p>L’expression est formatée comme suit :</p>

<p><code>ADDWEEKDAYS(date, number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDMONTHS</strong> </td> 
   <td> <p>Ajoute le nombre de mois à la date et est formaté comme suit :

</p><p><code>ADDMONTHS(date, number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDYEARS</strong> </td> 
   <td> <p>Ajoute le nombre d’années à la date et est formaté comme suit :</p>

<p><code>ADDYEARS(date, number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDHOURS</strong> </td> 
   <td> <p>Ajoute le nombre d'heures à la date et est formaté comme suit :</p>

<p><code>ADDHOUR(date, number)</code></p>
   <p>Remarque : cette expression n'est pas prise en charge dans Workfront Planning.</p></td> 
  </tr>
  <tr> 
   <td><strong>CLEARTIME</strong> </td> 
   <td> <p>Efface la partie heure d’une date, au format suivant. Dans cet exemple, la date est la date d’entrée d’un objet de travail.</p>

<p><code>CLEARTIME({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DATE</strong> </td> 
   <td> <p>Convertit une chaîne en dat, au format suivant :</p>

<p><code>DATE(string)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DATEDIFF</strong> </td> 
   <td> <p>Renvoie le nombre de jours entre deux dates, en tenant compte des jours de début et de fin de la période sélectionnée ainsi que des horodatages de ces jours. Par exemple, si l’heure de la date de début est 15 h, le jour de début n’est pas compté comme une journée complète.</p> <p>L’expression est formatée comme suit :</p>

<p><code>DATEDIFF(date1, date2)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYOFMONTH</strong> </td> 
   <td> <p>Retourne le jour du mois pour la date sous la forme d’un nombre entre 1 et 31.</p> <p>L’expression est formatée comme suit. Dans cet exemple, la date est la date d’entrée d’un objet de travail.</p>

<p><code>DAYOFMONTH({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYOFWEEK</strong> </td> 
   <td> <p>Retourne le jour de la semaine pour la date sous la forme d’un nombre entre 1 (dimanche) et 7 (samedi).</p> <p>L’expression est formatée comme suit. Dans cet exemple, la date est la date d’entrée d’un objet de travail.</p>

<p><code>DAYOFWEEK({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINMONTH</strong> </td> 
   <td> <p>Renvoie le nombre total de jours dans le mois de la date sous la forme d’un nombre, au format suivant. Dans cet exemple, la date est la date d’entrée d’un objet de travail.</p>

<p><code>DAYSINMONTH({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINSPLITWEEK</strong> </td> 
   <td> <p>Retourne le nombre de jours total de la semaine entre la date et la fin de la semaine ou la fin du mois, à la première échéance. Dans cet exemple, la date est la date d’entrée d’un objet de travail.</p> <p>L’expression est formatée comme suit :</p>

<p><code>DAYSINSPLITWEEK({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINYEAR</strong> </td> 
   <td> <p>Renvoie le nombre total de jours dans l’année de la date sous la forme d’un nombre avec le formant suivant. Dans cet exemple, la date est la date d’entrée d’un objet de travail.</p>

<p><code>DAYSINYEAR({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DMAX</strong> </td> 
   <td> <p>Renvoie la date la plus récente de la liste, au format suivant :</p>

<p><code>DMAX(date1, date2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DMIN</strong> </td> 
   <td> <p>Renvoie la date la plus ancienne de la liste, au format suivant :</p>

<p><code>DMIN(date1, date2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>HOUR</strong> </td> 
   <td> <p>Retourne l’heure de la date sous la forme d’un nombre entre 0 et 23.</p> <p>L’expression est formatée comme suit. Dans cet exemple, la date est la date d’entrée d’un objet de travail.</p>

<p><code>HOUR({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>MINUTE</strong> </td> 
   <td> <p>Renvoie la minute de la date sous la forme d’un nombre entre 0 et 60, au format suivant. Dans cet exemple, la date est la date d’entrée d’un objet de travail.</p>

<p><code>MINUTE({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>MONTH</strong> </td> 
   <td> <p>Renvoie le mois de la date sous la forme d’un nombre entre 1 et 12, au format suivant. Dans cet exemple, la date est la date d’entrée d’un objet de travail.</p>

<p><code>MONTH({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SECOND</strong> </td> 
   <td> <p>Renvoie la seconde de la date sous la forme d’un nombre compris entre 0 et 60, au format suivant. Dans cet exemple, la date est la date d’entrée d’un objet de travail.</p>

<p><code>SECOND({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>WEEKDAYDIFF</strong> </td> 
   <td> <p>Renvoie le nombre de jours de la semaine entre deux dates, en tenant compte des jours de début et de fin de la période sélectionnée, ainsi que des horodatages de ces jours. Par exemple, si l’heure de début de la date de début est 15 h, le jour de début n’est pas compté comme une journée complète.</p> <p>L’expression est formatée comme suit :</p>

<p><code>WEEKDAYDIFF(date2, date1)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>WORKMINUTESDIFF</strong> </td> 
   <td> <p>Renvoie le nombre de minutes planifiées entre les deux dates selon le planning par défaut.</p> <p>L’expression est formatée comme suit :</p>

<p><code>WORKMINUTESDIFF(date1, date2)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>YEAR</strong> </td> 
   <td> <p>Renvoie l’année de la date sous la forme d’un nombre à 4 chiffres, au format suivant. Dans cet exemple, la date est la date d’entrée d’un objet de travail.</p>

<p><code>YEAR({entryDate})</code></p> </td> 
  </tr> 
 </tbody> 
</table>

### Champs personnalisés calculés mathématiques {#mathematical-calculated-custom-fields}

Vous pouvez créer un champ personnalisé calculé qui utilise certaines des expressions mathématiques suivantes :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Expression...</th> 
   <th>Explication</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>ABS</strong> </td> 
   <td>Renvoie la valeur absolue du nombre au format suivant. Cet exemple utilise le nombre d’objets situés sous l’objet auquel le formulaire personnalisé est associé.

<p><code>ABS({numberOfChildren})</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>AVERAGE</strong> </td> 
   <td>Renvoie la moyenne des nombres au format suivant :

<p><code>AVERAGE(number1, number2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>CEIL</strong> </td> 
   <td>Arrondit un nombre à l’entier supérieur le plus proche au format suivant. Cet exemple utilise le nombre d’objets situés sous l’objet auquel le formulaire personnalisé est associé.

<p><code>CEIL({numberOfChildren})</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>DIV</strong> </td> 
   <td>Répartit tous les nombres dans l’ordre indiqué au format suivant :

<p><code>DIV(number1, number2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>FLOOR</strong> </td> 
   <td>Arrondit un nombre à l’entier inférieur le plus proche au format suivant. Cet exemple utilise le nombre d’objets situés sous l’objet auquel le formulaire personnalisé est associé.

<p><code>FLOOR({numberOfChildren})</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>LN</strong> </td> 
   <td>Renvoie la valeur du logarithme naturel du nombre au format suivant :

<p><code>LN({numberOfChildren})</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>LOG</strong> </td> 
   <td>Renvoie la valeur du logarithme de number2 au number1 de base au format suivant :

<p><code>LOG(number1, number2)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>MAX</strong> </td> 
   <td>Renvoie l’élément le plus grand de la liste au format suivant :

<p><code>MAX(item1, item2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>MIN</strong> </td> 
   <td>Renvoie l’élément le plus petit de la liste au format suivant :

<p><code>MIN(item1, item2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>NUMBER</strong> </td> 
   <td>Convertit une chaîne en nombre au format suivant :<p><code>NUMBER(string)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>POWER</strong> </td> 
   <td>Renvoie un nombre élevé à une puissance au format suivant :

<p><code>POWER(number, power)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>PROD</strong> </td> 
   <td>Multiplie tous les nombres au format suivant :

<p><code>PROD(number1, number2, ....)</code></p>
   <p><b>NOTE</b></p>

<p>Lorsque vous multipliez des champs qui contiennent des heures, veillez à comprendre si la base de données enregistre les heures dans les champs sélectionnés en minutes, heures ou secondes. Si les heures sont enregistrées en minutes ou en secondes mais s’affichent en heures dans l’interface de Workfront, vous devrez peut-être tenir compte de la conversion de minutes ou de secondes en heures lors de l’écriture d’une expression à l’aide de ce calcul. </p>
   </td> 
  </tr> 
  <tr> 
   <td><strong>ROUND</strong> </td> 
   <td>Arrondit le nombre à la hausse à des décimales de précision spécifiées au format suivant :

<p><code>ROUND(number, precision)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>SORTASCNUM</strong> </td> 
   <td> <p> Trie les nombres par ordre croissant au format suivant :</p>

<p><code>SORTASCNUM(number1,number2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTDESCNUM</strong> </td> 
   <td>Trie les nombres dans l’ordre décroissant au format suivant :

<p><code>SORTDESCNUM(number1, number2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>SQRT</strong> </td> 
   <td> <p>Renvoie la racine carrée d’un nombre au format suivant. Cet exemple utilise le nombre d’objets situés sous l’objet auquel le formulaire personnalisé est associé.</p>

<p><code>SQRT({numberOfChildren})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SUB</strong> </td> 
   <td>Soustrait tous les nombres dans l’ordre indiqué au format suivant :

<p><code>SUB(number1, number2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>SUM</strong> </td> 
   <td>Additionne tous les nombres au format suivant :

<p><code>SUM(number1, number2, ...)</code></p></td> 
  </tr> 
 </tbody> 
</table>

### Champs personnalisés calculés avec du texte {#text-calculated-custom-fields}

Vous pouvez créer un champ personnalisé calculé qui affiche une valeur au format texte à l’aide des expressions suivantes :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Expression...</th> 
   <th>Explication</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>TABLEAU</strong> </td> 
   <td> <p>Convertit une chaîne en tableau. Le délimiteur peut être n’importe quelle chaîne.</p> 
   <p>L’expression est formatée comme suit :</p>
   <p><code>ARRAY(string1, "delimiter")</code></p> 
   </td> 
  </tr>
  <tr> 
   <td><strong>ARRAYLENGTH</strong> </td> 
   <td> <p>Renvoie le nombre d’éléments dans le tableau et est formaté comme suit :</p>
   <p><code>ARRAYLENGTH(array)</code></p> 
   </td> 
  </tr>
  <tr> 
   <td><strong>ARRAYELEMENT</strong> </td> 
   <td> <p>Renvoie l’élément au nombre spécifié dans le tableau . Si l’index est hors limites, il renvoie vide.</p> 
   <p>L’expression est formatée comme suit :</p>
   <p><code>ARRAYELEMENT(array, number)</code></p> 
   </td> 
  </tr>
  <tr> 
   <td><strong> SORTASCARRAY </strong> </td> 
   <td> <p>Classe les éléments du tableau dans l’ordre croissant et les convertit en type du premier élément.</p>
   <p>L’expression est formatée comme suit :</p>
   <p><code>SORTASCARRAY(array)</code></p>
   <p>Par exemple, [« -12.6 », -13.0] devient [« -12.6 », « -13 »].</p>
   <p>Remarque : cette expression n'est pas prise en charge dans Workfront Planning.</p></td> 
  </tr>
  <tr> 
   <td><strong>SORTDESCARRAY </strong> </td> 
   <td> <p>Classe les éléments du tableau dans l’ordre décroissant et les convertit en type du premier élément.</p>
   <p>L’expression est formatée comme suit :</p>
   <p><code>SORTDESCARRAY(array)</code></p>
   <p>Par exemple, [« -12.6 », -13.0] devient [« -13 », « -12.6 »].</p>
   <p>Remarque : cette expression n'est pas prise en charge dans Workfront Planning.</p></td> 
  </tr>
  <tr>   
   <td><strong>CASE</strong> </td> 
   <td> <p>Utilisé avec d’autres expressions pour choisir une valeur dans une liste, en fonction d’un numéro d’index. </p>
   <p>Un numéro d’index est un champ ou une fonction qui renvoie une valeur numérique (généralement comprise dans une plage connue).</p> 
   <p>L’expression est formatée comme suit :</p>
   <p><code>CASE(indexNumber, value1, value2, ...)</code></p>

<p>Par exemple, l’expression suivante renvoie le nom du jour de la semaine, où 1=dimanche, 2=lundi, etc., dans une colonne calculée :</p>

<p><code>CASE(DAYOFWEEK({entryDate}),"Sunday","Monday","Tuesday","Wednesday","Thursday","Friday","Saturday")</code></p>

<p>Fonctionne mieux avec d’autres expressions qui renvoient un nombre, telles que DAYOFWEEK, DAYOFMONTH et MONTH.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>CONCAT</strong> </td> 
   <td> <p>Concatène la chaîne de caractères au format suivant :</p><p><code>CONCAT(string1,"separator", string2)</code></p> <p>Vous trouverez ci-dessous des exemples de séparateurs que vous pouvez inclure :</p> 
    <ul> 
     <li>Espace : « »</li> 
     <li>Tiret : « - »</li> 
     <li>Barre oblique : « / »</li> 
     <li>Virgule : « , »</li> 
     <li>Mot : « ou », « et »</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><strong>CONTAINS</strong> </td> 
   <td>Renvoie la valeur « true » si la chaîne findText est trouvée dans la chaîne withinText au format suivant :

<p><code>CONTAINS(findText, withinText)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>ENCODEURL</strong> </td> 
   <td>Ignore tous les caractères spéciaux dans la chaîne afin qu’ils puissent être inclus dans un argument URL.<p>L’expression est formatée comme suit :</p>

<p><code>ENCODEURL(string)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>FORMAT </strong> </td> 
   <td><p>Renvoie le texte formaté. Les options de couleur sont $$POSITIVE, $$INFORMATIVE, $$NEGATIVE, $$NOTICE, et les autres options de mise en forme sont $$BOLD, $$ITALIC, $$UNDERLINE. Une seule option de couleur peut être utilisée par fonction, ainsi que jusqu’à trois autres options de mise en forme. Si aucune option de couleur n’est spécifiée, la couleur par défaut du système est appliquée.</p>
   <p>L’expression est formatée comme suit :</p>
   <p><code>FORMAT($$POSITIVE, $$BOLD, $$ITALIC)</code></p>
   <p>Remarque : cette expression n'est pas prise en charge dans Workfront Planning.</p></td> 
  </tr>   
  <tr> 
   <td><strong>IF</strong> </td> 
   <td> <p>Évalue une condition que vous spécifiez et renvoie la valeur de trueExpression si elle est vraie, ou la valeur de falseExpression si elle est fausse.</p>

<p>L’expression est formatée comme suit :</p>

<p><code>IF(condition, trueExpression, falseExpression)</code></p>

<p>Par exemple, vous pouvez comparer deux champs de date différents suivis d’un résultat True/False sous la forme d’une chaîne de données :</p>

<p><code>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"Off Track","On Track")</code></p>

<p>En langage courant, cette instruction signifie : « Si (IF) la date d’achèvement projetée de mon objet est « Greater Than » (supérieure à) la date d’achèvement prévue du même objet, affichez les mots « En retard » dans ce champ ; dans le cas contraire, affichez les mots « Dans les temps ».</p>

<p>Si vous ne souhaitez pas libeller les expressions true ou false, vous devez insérer un libellé vide dans votre instruction, tel que :</p>

<p><code>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"","On Track")</code></p> 
   <p>Ou</p>

<p><code>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"Off Track","")</code></p>

<p>Pour plus d’informations sur la création d’instructions « IF », voir <a href="../../../reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md" class="MCXref xref">Vue d’ensemble des instructions « IF »</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>IFIN</strong> </td> 
   <td> <p>Permet de rechercher une valeur spécifique dans une chaîne de valeurs possibles. Si la valeur que vous recherchez est égale à l’une des valeurs fournies, l’expression renvoie trueExpression ; dans le cas contraire, elle renvoie falseExpression.</p> 
   <p>L’expression est formatée comme suit :</p>

<p><code>IFIN(value, value1, value2,..., trueExpression, falseExpression)</code></p>

<p>Par exemple, vous pouvez trouver une personne propriétaire de projet spécifique et marquer ces projets avec une balise spécifique dans la vue de projet : <br><p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team","Other Teams")
   </code></p>
    <p> En langage courant, cette instruction signifie : « Si la personne propriétaire du projet est Jennifer Campbell ou Rick Kuvec, marquez ce projet comme "Équipe marketing" ; sinon, marquez-le comme "Autres équipes" ».</p> 
    <p> Si vous ne souhaitez pas libeller les expressions true ou false, vous devez insérer un libellé vide dans votre instruction, tel que : </p> 
    <p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","","Other Teams")</code></p> 
    <p>Ou </p> 
    <p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team","")</code></p> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>IN</strong> </td> 
   <td> <p>Renvoie true si la valeur est égale à l’une des valeurs fournies ; dans le cas contraire, l’expression renvoie false.</p> <p>L’expression est formatée comme suit :

</p><p><code>IN(value, value1[, value2...])</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ISBLANK</strong> </td> 
   <td> <p>Renvoie la valeur true si la valeur est null ou vide ; dans le cas contraire, l’expression renvoie la valeur false.</p> <p>L’expression est formatée comme suit :

</p><p><code>ISBLANK(value)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>LEFT</strong> </td> 
   <td> <p>Renvoie un nombre spécifié de caractères à partir de la gauche d’une chaîne et présente le format suivant :</p>

<p><code>LEFT(string, length)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>LEN</strong> </td> 
   <td> <p>Renvoie la longueur d’une chaîne et présente le format suivant :</p>

<p><code>LEN(string)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>LOWER</strong> </td> 
   <td>Renvoie la chaîne en minuscules au format suivant :

<p><code>LOWER(string)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>REPLACE</strong> </td> 
   <td> <p>Remplace toutes les occurrences de string2 par string3 dans string1.</p> <p>L’expression est formatée comme suit :</p>

<p><code>REPLACE(string1, string2, string3)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>RIGHT</strong> </td> 
   <td> <p>Renvoie un nombre spécifié de caractères à partir de la droite d’une chaîne au format suivant :</p>

<p><code>RIGHT(string, length)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SEARCH</strong> </td> 
   <td> <p>Renvoie l’index de la première occurrence de findText dans la chaîne withinText, en commençant à la position de début donnée, ou -1 si le texte n’est pas trouvé.</p> <p>L’expression est formatée comme suit :</p>

<p><code>SEARCH(findText, withinText, start)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>STRING</strong> </td> 
   <td> <p>Convertit un nombre en chaîne au format suivant :</p>

<p><code>STRING(number)</code></p> </td> 
  </tr>
  <tr> 
   <td><strong>SORTASCSTRING</strong> </td> 
   <td> <p>Trie une liste de chaînes par ordre croissant au format suivant :</p>
   <p><code>SORTASCSTRING(string1, string2, ...)</code></p> </td> 
  </tr>
  <tr> 
   <td><strong>SORTDESCSTRING</strong> </td> 
   <td> <p> Trie une liste de chaînes par ordre décroissant et présente le format suivant :</p>
   <p><code>SORTDESCSTRING(string1, string2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SUBSTR</strong> </td> 
   <td> <p>Renvoie les caractères d’une chaîne selon l’index de début et de fin spécifié et présente le format suivant :</p>

<p><code>SUBSTR({string}, number of start position, number of end position)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SWITCH</strong> </td> 
   <td> <p>Evalue l'expression par rapport à une liste de valeurs, et retourne le résultat correspondant à la première valeur correspondante.</p>
   <p>L’expression est formatée comme suit :</p>
   <p><code>SWITCH(expression, value1, result1, [value2, result2], ...)</code></p>
   <p>Cette expression n'est pas prise en charge dans Workfront Planning.</p></td> 
  </tr>   
  <tr> 
   <td><strong>TRIM</strong> </td> 
   <td> <p>Supprime les espaces au début et à la fin d’une chaîne et présente le format suivant :</p>

<p><code>TRIM(string)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>UPPER</strong> </td> 
   <td> <p>Renvoie une chaîne en majuscules et présente le format suivant :</p>

<p><code>UPPER(string)</code></p> </td> 
  </tr> 
 </tbody> 
</table>
