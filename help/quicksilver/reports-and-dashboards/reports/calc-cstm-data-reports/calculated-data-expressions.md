---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: Expressions de données calculées
description: Vous pouvez utiliser des expressions de données pour définir des champs de données personnalisés calculés dans Adobe Workfront. Ils connectent des champs Workfront existants dans des instructions qui génèrent un nouveau champ.
author: Nolan
feature: Reports and Dashboards
exl-id: cfb3ace9-76c3-4006-878f-e2ad25ffa03b
source-git-commit: 22438c38727f5cc36b07b3530818f5bda2b0bacf
workflow-type: tm+mt
source-wordcount: '2270'
ht-degree: 7%

---

# Expressions de données calculées

Vous pouvez utiliser des expressions de données pour définir des champs de données personnalisés calculés dans Adobe Workfront. Ils connectent des champs Workfront existants dans des instructions qui génèrent un nouveau champ.

Vous pouvez utiliser des expressions de données calculées dans :

* Un formulaire personnalisé

   Pour plus d’informations sur la création de champs de données personnalisées calculées sur des formulaires personnalisés dans Workfront, voir [Ajout de données calculées à un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

* Une colonne personnalisée calculée dans un rapport ou une liste lorsque vous utilisez le mode texte

   Pour plus d’informations sur l’utilisation du mode texte dans les rapports et les vues, voir [Présentation du mode texte](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Syntaxe des champs personnalisés calculés par rapport aux colonnes personnalisées calculées

Bien que les fonctions que vous utilisez soient les mêmes, la syntaxe de création d’une expression dans un champ personnalisé calculé peut être différente de celle utilisée pour créer une colonne personnalisée calculée.

Par exemple :

* Dans un champ personnalisé, sur un formulaire personnalisé pour les tâches, vous utiliserez les éléments suivants pour générer le nom du projet parent de la tâche à laquelle le formulaire personnalisé est joint :

   ```
   {project}.{name}
   ```

* Dans une colonne personnalisée d’un rapport, vous pouvez utiliser les éléments suivants pour ajouter une colonne personnalisée Nom du projet à un rapport de tâche :

   ```
   valuefield=project:name
   ```

   Ou

   ```
   valueexpression={project}.{name}
   ```

   >[!TIP]
   >
   >La même syntaxe s’applique à tous les éléments de rapport en mode texte dans lesquels des expressions calculées sont utilisées : vues, filtres, regroupements, invites.

Les différences entre les deux syntaxes sont les suivantes :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Champ personnalisé calculé</strong></td> 
   <td><strong>Elément de rapport personnalisé calculé</strong></td> 
  </tr> 
   <td>Placez les noms de champ entre accolades.</td> 
   <td>Ne placez pas les noms de champ entre crochets ou parenthèses lors de leur utilisation dans une <code>valuefield </code>ligne. <p>Placez les noms de champ entre accolades lorsque vous les utilisez dans une balise <code>valueexpression</code> ligne.</p> </td> 
  </tr> 
  <tr> 
   <td>Séparez les champs par des points.</td> 
   <td> <p>Séparez les champs par deux-points lors de leur utilisation dans un <code>valuefield </code>line</p> <p>Séparez les champs par des points lors de leur utilisation dans une <code>valueexpression </code>ligne. </p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur la syntaxe que vous devez utiliser dans une colonne personnalisée calculée, voir [Présentation du mode texte](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Expressions de données que vous pouvez utiliser

Les listes ci-dessous définissent les expressions disponibles que vous pouvez utiliser lorsque vous créez l’un des trois types différents de champs personnalisés calculés dans Workfront :

* [Champs personnalisés calculés par date et heure](#date-time-calculated-custom-fields)
* [Champs personnalisés calculés mathématiques](#mathematical-calculated-custom-fields)
* [Champs personnalisés calculés par le texte](#text-calculated-custom-fields)

### Champs personnalisés calculés par date et heure {#date-time-calculated-custom-fields}

>[!NOTE]
>
>Si vous créez un calcul de date et heure qui n’inclut pas de partie horaire ou qui utilise les caractères génériques $$TODAY ou $$NOW, le système utilise la date selon le fuseau horaire universel coordonné (UTC), et non selon votre fuseau horaire local. Cela peut entraîner un résultat de date inattendu.

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
   <td> <p>Cette expression ajoute le nombre de jours à la date et est formatée comme suit :</p><pre>ADDDAYS(date, number)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>AJOUTERJOURSSEMAINE</strong> </td> 
   <td> <p>Cette expression ajoute à la date le nombre de jours de la semaine et est formatée comme suit :</p><pre>AJOUTERJOURSSEMAINE(date, nombre)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDMONTHS</strong> </td> 
   <td> <p>Cette expression ajoute le nombre de mois à la date et est formatée comme suit :</p><pre>ADDMONTHS(date, number)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDYEARS</strong> </td> 
   <td> <p>Cette expression ajoute le nombre d'années à la date et est formatée comme suit :</p><pre>ADDYEARS(date, number)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>CLEARTIME</strong> </td> 
   <td> <p>Cette expression efface la partie heure d’une date et est formatée comme suit. Dans cet exemple, la date est la date d’entrée d’un objet de travail.</p><pre>CLEARTIME({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DATE</strong> </td> 
   <td> <p>Cette expression convertit une chaîne en date et est formatée comme suit :</p><pre>DATE(string)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DATEDIFF</strong> </td> 
   <td> <p>Cette expression renvoie le nombre de jours entre les deux dates, en prenant en compte les jours de début et de fin de la période sélectionnée ainsi que les horodatages de ces jours. Par exemple, si l’heure de début de la date est 15 heures, le jour de début n’est pas compté comme une journée complète.</p> <p>L’expression est formatée comme suit :</p><pre>DATEDIFF(date1, date2)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYOFMONTH</strong> </td> 
   <td> <p>Cette expression renvoie le jour du mois pour la date sous forme numérique, entre 1 et 31.</p> <p>L’expression est formatée comme suit. Dans cet exemple, la date est la date d’entrée d’un objet de travail.</p><pre>DAYOFMONTH({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYOFWEEK</strong> </td> 
   <td> <p>Cette expression renvoie le jour de la semaine pour la date sous la forme d’un nombre, compris entre 1 (dimanche) et 7 (samedi).</p> <p>L’expression est formatée comme suit. Dans cet exemple, la date est la date d’entrée d’un objet de travail.</p><pre>DAYOFWEEK({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINMONTH</strong> </td> 
   <td> <p>Cette expression renvoie le nombre total de jours dans le mois de la date et est formatée comme suit. Dans cet exemple, la date est la date d’entrée d’un objet de travail.</p><pre>DAYSINMONTH({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINSPLITWEEK</strong> </td> 
   <td> <p>Cette expression renvoie le nombre total de jours de la semaine entre la date et la fin de la semaine, ou la fin du mois, selon la condition qui s’affiche en premier. Dans cet exemple, la date est la date d’entrée d’un objet de travail.</p> <p>L’expression est formatée comme suit :</p><pre>DAYSINSPLITWEEK({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINYEAR</strong> </td> 
   <td> <p>Cette expression renvoie le nombre total de jours dans l’année de la date et est formatée comme suit. Dans cet exemple, la date est la date d’entrée d’un objet de travail.</p><pre>DAYSINYEAR({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DMAX</strong> </td> 
   <td> <p>Cette expression renvoie la dernière date de la liste et est formatée comme suit :</p><pre>DMAX(date1, date2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DMIN</strong> </td> 
   <td> <p>Cette expression renvoie la date la plus ancienne de la liste et est formatée comme suit :</p><pre>DMIN(date1, date2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>HOUR</strong> </td> 
   <td> <p>Cette expression renvoie l’heure de la date sous la forme d’un nombre compris entre 0 et 23.</p> <p>L’expression est formatée comme suit. Dans cet exemple, la date est la date d’entrée d’un objet de travail.</p><pre>HOUR({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>MINUTE</strong> </td> 
   <td> <p>Cette expression renvoie la minute de la date sous la forme d’un nombre compris entre 0 et 60, au format suivant. Dans cet exemple, la date est la date d’entrée d’un objet de travail.</p><pre>MINUTE({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>MOIS</strong> </td> 
   <td> <p>Cette expression renvoie le mois de la date sous la forme d’un nombre compris entre 1 et 12, au format suivant. Dans cet exemple, la date est la date d’entrée d’un objet de travail.</p><pre>MONTH({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SECOND</strong> </td> 
   <td> <p>Cette expression renvoie la seconde de la date sous la forme d’un nombre compris entre 0 et 60, au format suivant. Dans cet exemple, la date est la date d’entrée d’un objet de travail.</p><pre>SECOND({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>WEEKDAYDIFF</strong> </td> 
   <td> <p>Cette expression renvoie le nombre de jours de la semaine entre deux dates, en tenant compte des jours de début et de fin de la période sélectionnée, ainsi que des horodatages de ces jours. Par exemple, si l’heure de début de la date est 15 heures, le jour de début n’est pas compté comme une journée complète.</p> <p>L’expression est formatée comme suit :</p><pre>WEEKDAYDIFF(date2, date1)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>WORKMINUTESDIFF</strong> </td> 
   <td> <p>Cette expression renvoie le nombre de minutes planifiées entre les dates selon le planning par défaut.</p> <p>L’expression est formatée comme suit :</p><pre>WORKMINUTESDIFF(date1, date2)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ANNÉE</strong> </td> 
   <td> <p>Cette expression renvoie l’année de la date sous la forme d’un nombre à 4 chiffres, au format suivant. Dans cet exemple, la date est la date d’entrée d’un objet de travail.</p><pre>YEAR({entryDate})</pre> </td> 
  </tr> 
 </tbody> 
</table>

### Champs personnalisés calculés mathématiques {#mathematical-calculated-custom-fields}

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
   <td>Cette expression renvoie la valeur absolue du nombre et est formatée comme suit. Cet exemple utilise le nombre d’objets situés sous l’objet auquel le formulaire personnalisé est associé.<pre>ABS({numberOfChildren})</pre></td> 
  </tr> 
  <tr> 
   <td><strong>AVERAGE</strong> </td> 
   <td>Cette expression renvoie la moyenne des nombres et est formatée comme suit :<pre>AVERAGE(number1, number2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>CEIL</strong> </td> 
   <td>Cette expression arrondit un nombre à l’entier le plus proche et est formatée comme suit. Cet exemple utilise le nombre d’objets situés sous l’objet auquel le formulaire personnalisé est associé.<pre>CEIL({numberOfChildren})</pre></td> 
  </tr> 
  <tr> 
   <td><strong>DIV</strong> </td> 
   <td>Cette expression divise tous les nombres dans l’ordre indiqué et est formatée comme suit :<pre>DIV(number1, number2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>ARRONDI À L’INFÉRIEUR</strong> </td> 
   <td>Cette expression arrondit un nombre à l’entier le plus proche et est formatée comme suit. Cet exemple utilise le nombre d’objets situés sous l’objet auquel le formulaire personnalisé est associé.<pre>FLOOR({numberOfChildren})</pre></td> 
  </tr> 
  <tr> 
   <td><strong>LN</strong> </td> 
   <td>Cette expression renvoie la valeur de logarithme népérienne du nombre et est formatée comme suit :<pre>LN({numberOfChildren})</pre></td> 
  </tr> 
  <tr> 
   <td><strong>LOG</strong> </td> 
   <td>Cette expression renvoie la valeur logarithmique number2 à la base number1 et est formatée comme suit :<pre>LOG(number1, number2)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>MAX</strong> </td> 
   <td>Cette expression renvoie l’élément le plus grand de la liste et est formatée comme suit :<pre>MAX(item1, item2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>MIN</strong> </td> 
   <td>Cette expression renvoie le plus petit élément de la liste et est formatée comme suit :<pre>MIN(item1, item2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>NUMBER</strong> </td> 
   <td>Cette expression convertit une chaîne en nombre et est formatée comme suit :<pre>NUMBER(string)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>POWER</strong> </td> 
   <td>Cette expression renvoie un nombre élevé à une puissance et est formatée comme suit :<pre>POWER(number, power)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>PROD</strong> </td> 
   <td>Cette expression multiplie tous les nombres et est formatée comme suit :<pre>PROD(number1, number2, ....)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>ARRONDIR</strong> </td> 
   <td>Cette expression arrondit le nombre à des décimales de précision spécifiées et est formatée comme suit :<p>ROUND(nombre, précision)</p></td> 
  </tr> 
  <tr> 
   <td><strong>SORTASCNUM</strong> </td> 
   <td> <p> Cette expression classe les nombres par ordre croissant et se présente comme suit :</p><pre>SORTASCNUM(number1, number2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTDESCNUM</strong> </td> 
   <td>Cette expression classe les nombres dans l'ordre décroissant, au format suivant :<pre>SORTDESCNUM(number1, number2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>SQRT</strong> </td> 
   <td> <p>Cette expression renvoie une racine carrée d’un nombre et est formatée comme suit. Cet exemple utilise le nombre d’objets situés sous l’objet auquel le formulaire personnalisé est associé.</p><pre>SQRT({numberOfChildren})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SUB</strong> </td> 
   <td>Cette expression soustrait tous les nombres dans l’ordre indiqué et est formatée comme suit :<pre>SUB(number1, number2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>SUM</strong> </td> 
   <td>Cette expression ajoute tous les nombres et est formatée comme suit :<pre>SUM(number1, number2, ...)</pre></td> 
  </tr> 
 </tbody> 
</table>

### Champs personnalisés calculés par le texte {#text-calculated-custom-fields}

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
   <td><strong>CASE</strong> </td> 
   <td> <p>Cette expression est utilisée avec d’autres expressions pour choisir une valeur dans une liste, en fonction d’un numéro d’index. Un numéro d’index est un champ ou une fonction qui renvoie une valeur numérique (généralement comprise dans une plage connue).</p> <p>L’expression est formatée comme suit :</p><pre>CASE(indexNumber, value1, value2, etc.)</pre> <p>Par exemple, l’expression suivante renvoie le nom du jour de la semaine, où 1=dimanche, 2=lundi, etc., dans une colonne calculée :</p><pre>CASE(DAYOFWEEK({entryDate}),"Dimanche","Lundi","Mardi","Mercredi","jeudi","Vendredi","samedi")</pre> <p>Cette expression fonctionne mieux avec d’autres expressions qui renvoient un nombre, telles que DAYOFWEEK, DAYOFMONTH et MONTH.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>CONCAT</strong> </td> 
   <td> <p>Cette expression concatène la chaîne et est formatée comme suit :</p><pre>CONCAT(string1,"separator", string2)</pre> <p>Voici des exemples de séparateurs que vous pouvez inclure :</p> 
    <ul> 
     <li>un espace : "</li> 
     <li>un tiret : "-"</li> 
     <li>une barre oblique : "/"</li> 
     <li>une virgule : ","</li> 
     <li>un mot : "or", "and"</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><strong>CONTIENT</strong> </td> 
   <td>Cette expression renvoie true si la chaîne findText se trouve dans la chaîne WithinText et est formatée comme suit :<pre>CONTAINS(findText, withinText)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>ENCODEURL</strong> </td> 
   <td>Cette expression extrait tous les caractères spéciaux de la chaîne afin qu’ils puissent être inclus dans un argument URL.<p>L’expression est formatée comme suit :</p><pre>ENCODEURL(string)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>IF</strong> </td> 
   <td> <p>Cette expression évalue une condition que vous spécifiez et renvoie la valeur de trueExpression si elle est vraie ou la valeur de falseExpression si elle est fausse.</p> <p>L’expression est formatée comme suit :</p><pre>IF(condition, trueExpression, falseExpression)</pre> <p>Par exemple, vous pouvez comparer deux champs de date différents suivis d’un résultat True/False sous la forme d’une chaîne de données :</p><pre>IF({ProjectionCompletionDate}&gt;{scheduledCompletionDate},"Off Track","On Track")</pre> <p>Dans le discours quotidien, cette déclaration signifie : "Si la date de fin prévue de mon objet est "Supérieur à" la date de fin planifiée du même objet, affichez les mots "Désactivé le suivi" dans ce champ. sinon, affichez les mots "Sur suivi".</p> <p>Si vous ne souhaitez pas libeller les expressions true ou false, vous devez insérer un libellé vide dans votre instruction, tel que :</p><pre>IF({ProjectionCompletionDate}&gt;{scheduledCompletionDate},",","On Track")</pre> <p>Ou</p><pre>IF({ProjectionCompletionDate}&gt;{scheduledCompletionDate},"Off Track",")</pre> <p>Pour plus d’informations sur la création d’instructions "IF", voir <a href="../../../reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md" class="MCXref xref">Présentation des instructions "IF"</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>IFIN</strong> </td> 
   <td> <p>Cette expression vous permet de rechercher une valeur spécifique dans une chaîne de valeurs possibles. Si la valeur recherchée est égale à l’une des valeurs fournies, l’expression renvoie la valeur trueExpression ; sinon, elle renvoie la falseExpression.</p> <p>L’expression est formatée comme suit :</p><pre>IFIN(valeur, valeur1, valeur2,..., trueExpression, falseExpression)</pre> <p>Par exemple, vous pouvez trouver un propriétaire de projet spécifique et marquer ces projets avec une balise spécifique dans la vue de projet : <br><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team","Other Teams")</code></p> <p> Dans le discours quotidien, cette déclaration signifie : "Si le propriétaire du projet est Jennifer Campbell ou Rick Kuvec, marquez ce projet avec "Équipe marketing". sinon, marquez-le avec "Autres équipes".</p> <p> Si vous ne souhaitez pas libeller les expressions true ou false, vous devez insérer un libellé vide dans votre instruction, tel que : </p> <p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","","Other Teams")</code></p> <p>Ou </p> <p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team",""</code> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>DANS</strong> </td> 
   <td> <p>Cette expression renvoie true si la valeur est égale à l’une des valeurs fournies ; sinon, l’expression renvoie false.</p> <p>L’expression est formatée comme suit :</p><pre>IN(value, value1[, value2...])</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ISBLANK</strong> </td> 
   <td> <p>Cette expression renvoie true si la valeur est nulle ou vide ; sinon, l’expression renvoie false.</p> <p>L’expression est formatée comme suit :</p><pre>ISBLANK(value)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>GAUCHE</strong> </td> 
   <td> <p>Cette expression renvoie un nombre spécifié de caractères à partir du côté gauche d’une chaîne et est formatée comme suit :</p><pre>LEFT(string, length)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>LEN</strong> </td> 
   <td> <p>Cette expression renvoie la longueur d’une chaîne et est formatée comme suit :</p><pre>LEN(string)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>LOWER</strong> </td> 
   <td>Cette expression renvoie la chaîne en minuscules et est formatée comme suit :<pre>LOWER(string)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>REMPLACER</strong> </td> 
   <td> <p>Cette expression remplace toutes les occurrences de string2 par string3 dans string1.</p> <p>L’expression est formatée comme suit :</p><pre>REPLACE(string1, string2, string3)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DROITE</strong> </td> 
   <td> <p>Cette expression renvoie un nombre spécifié de caractères à partir du côté droit d’une chaîne et est formatée comme suit :</p><pre>RIGHT(string, length)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SEARCH</strong> </td> 
   <td> <p>Cette expression renvoie l’index de la première occurrence de findText dans la chaîne dansText, en commençant à la position de départ donnée, ou -1 si le texte est introuvable.</p> <p>L’expression est formatée comme suit :</p><pre>SEARCH(findText, insideText, start)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>STRING</strong> </td> 
   <td> <p>Cette expression convertit un nombre en chaîne et est formatée comme suit :</p><pre>STRING(number)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTASCSTRING</strong> </td> 
   <td> <p>Cette expression trie une liste de chaînes par ordre croissant et se présente comme suit :</p><pre>SORTASCSTRING(string1, string2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTDESCSTRING</strong> </td> 
   <td> <p> Cette expression trie une liste de chaînes dans l’ordre décroissant et est formatée comme suit :</p><pre>SORTDESCSTRING(string1, string2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SUBSTR</strong> </td> 
   <td> <p>Cette expression renvoie les caractères d’une chaîne en fonction de l’index de début et de fin spécifié et est formaté comme suit :</p><pre>SUBSTR({string}, nombre de position de départ, nombre de position de fin)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>TRIM</strong> </td> 
   <td> <p>Cette expression supprime les espaces du début et de la fin d’une chaîne et est formatée comme suit :</p><pre>TRIM(string)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>UPPER</strong> </td> 
   <td> <p>Cette expression renvoie une chaîne en majuscules, au format suivant :</p><pre>UPPER(string)</pre> </td> 
  </tr> 
 </tbody> 
</table>
