---
content-type: overview
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: Présentation des instructions IF
description: Vous pouvez utiliser des instructions "IF" dans des langages de programmation généraux. Dans Adobe Workfront, les instructions "IF" vous permettent de comparer, formater et associer des champs de données à des fins de création de rapports et de données personnalisées. En outre, la réflexion mathématique sur les instructions "IF" conduit à une meilleure compréhension conceptuelle puisque les variables pour les expressions sont généralement utilisées.
author: Nolan
feature: Reports and Dashboards
exl-id: 090a85fd-fdbe-4507-8bad-ce8c29bf8fc9
source-git-commit: 32966d4732221d73aa3397771e157b630f7d5760
workflow-type: tm+mt
source-wordcount: '925'
ht-degree: 0%

---

# Présentation des instructions &quot;IF&quot;

Vous pouvez utiliser des instructions &quot;IF&quot; dans des langages de programmation généraux. Dans Adobe Workfront, les instructions &quot;IF&quot; vous permettent de comparer, formater et associer des champs de données à des fins de création de rapports et de données personnalisées. En outre, la réflexion mathématique sur les instructions &quot;IF&quot; conduit à une meilleure compréhension conceptuelle puisque les variables pour les expressions sont généralement utilisées.

## Recommendations pour les instructions &quot;IF&quot;

Tenez compte des points suivants avant de créer une instruction &quot;IF&quot; :

* Nous recommandons une compréhension de base de tout langage de programmation général, mais nous n’en avons pas besoin pour ce guide.
* Nous avons besoin d’une compréhension avancée de la syntaxe du mode texte de Workfront. Cela permet de comprendre la terminologie de l’API Workfront et la syntaxe des données personnalisées dans ces formats spécifiques.

  Pour plus d’informations sur l’API Workfront, voir [Principes de base des API](../../../wf-api/general/api-basics.md).

  Pour plus d’informations sur l’utilisation du mode texte, voir [Présentation du mode texte](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

* Vous pouvez créer des instructions &quot;IF&quot; pour les éléments Workfront suivants :

   * Vues
   * Regroupements
   * Champs personnalisés calculés

* Vous ne pouvez pas créer d’instructions &quot;IF&quot; pour les filtres. Cela entraîne une erreur &quot;Oups&quot; dans Workfront.
* L’équipe d’assistance n’aide pas à créer des données personnalisées. Vous pouvez contacter l’équipe d’assistance après avoir créé les champs ou colonnes personnalisés et ne pas voir les résultats souhaités. Pour obtenir de l’aide sur la création d’une expression, contactez votre gestionnaire de compte pour obtenir des renseignements au sujet de nos options de conseil.
* Nous vous recommandons d’écrire ces expressions dans un éditeur de texte, tel que Sublime ou Visual Studio Code, car cela vous permet d’afficher les données plus clairement que dans Workfront.

## Composants d’une instruction &quot;IF&quot;

Vous pouvez créer des instructions &quot;IF&quot; dans Workfront au format suivant :
<pre>IF(Condition,True Expression,False Expression)</pre>Les composants d’une instruction "IF" sont les suivants :

* **IF**= Il s’agit de l’expression de données calculées Workfront pour la &quot;fonction&quot;. Tout comme les expressions SUM et PROD, cela indique tout d’abord au système de comprendre la fonction en tant qu’instruction &quot;IF&quot;. Utilisez toujours des majuscules pour &quot;IF&quot; dans cette instruction.\
  Pour obtenir la liste de toutes les expressions de données calculées, voir [Présentation des expressions de données calculées](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

* **Condition**= Il s’agit de la condition que la variable Workfront doit remplir et qui est la base de cette équation. Tout ce qui peut être spécifié ultérieurement dans l’équation dépend de la condition. Vous pouvez utiliser un certain nombre de références, comparaisons ou expressions mathématiques pour commencer une équation. Voici quelques exemples de conditions :

   * Une date est supérieure à une autre date sur un objet spécifié.
   * Un état est égal à l’un des états disponibles sur un objet spécifié.
   * Le pourcentage d’achèvement d’une tâche est inférieur ou supérieur à un certain pourcentage.

* **Opérateur de condition** = il s’agit de l’opérateur qui vous aide à créer la condition de votre instruction &quot;IF&quot;. Par exemple, &quot;est égal à&quot; ou &quot;est supérieur à&quot; sont des opérateurs de condition. Pour obtenir la liste des opérateurs de condition que vous pouvez utiliser dans les instructions, voir [Opérateurs de condition dans les expressions personnalisées calculées](../../../reports-and-dashboards/reports/calc-cstm-data-reports/condition-operators-calculated-custom-expressions.md).

* **True****Expression**= Il s’agit de la variable &quot;True&quot;, qui indique à l’équation quel indicateur afficher une fois que les critères de la condition sont satisfaits (indicateurs true).

* **False Expression**= Il s’agit de la variable &quot;False&quot;, qui indique à l’équation quel indicateur afficher lorsque les critères de la condition ne sont pas satisfaits (faux indicateurs).

Dans l’exemple suivant, le format d’instruction d’origine est utilisé pour écrire une expression de données simple pour une instruction &quot;IF&quot;. L’expression compare deux champs de date différents dans Workfront, suivis d’un résultat True/False sous la forme d’une chaîne de données :

```
IF({projectedCompletionDate}>{plannedCompletionDate},"Off Track","On Track")
```

Dans les discours de tous les jours, cette instruction signifie : si la date d’achèvement prévue de mon objet est &quot;Supérieur à&quot; la date d’achèvement planifiée du même objet, affichez les mots &quot;Suivi désactivé&quot; dans ce champ. Dans le cas contraire, affichez les mots &quot;Sur la piste&quot;.

## Créer des champs calculés dans des formulaires personnalisés ou des colonnes personnalisées à l’aide d’instructions &quot;IF&quot;

Vous pouvez créer des instructions &quot;IF&quot; dans un champ calculé dans un formulaire personnalisé ou dans une colonne personnalisée.

Il existe une différence entre la syntaxe que vous utilisez dans un formulaire personnalisé calculé et celle d’une colonne personnalisée calculée. Reportez-vous aux exemples suivants :

* [Instructions &quot;IF&quot; uniques](#single-if-statements)
* [Plusieurs instructions &quot;IF&quot;](#multiple-if-statements)

### Instructions &quot;IF&quot; uniques {#single-if-statements}

Voici des exemples d’un champ personnalisé calculé et de sa colonne correspondante à l’aide d’une instruction &quot;IF&quot; :

* Champ personnalisé calculé :

Lors de la création d’un champ personnalisé, utilisez la syntaxe suivante pour une instruction &quot;IF&quot; :

```
IF({Projected Completion Date}>{Planned Completion Date},"Off Track","On Track")
```

* Colonne personnalisée calculée :

Lors de la création d’une colonne personnalisée, vous devez utiliser la syntaxe suivante pour l’instruction &quot;IF&quot; dans la ligne d’expression de valeur :

```
valueexpression=IF({projectedCompletionDate}>{plannedCompletionDate},"Off Track","On Track")
```

### Plusieurs instructions &quot;IF&quot; {#multiple-if-statements}

Vous pouvez assembler plusieurs instructions &quot;IF&quot; avec l’instruction suivante pour créer une expression plus complexe et dynamique :

<pre>IF(Condition1,True Expression,IF(Condition2,True Expression,False Expression))</pre>Notez qu’il n’existe désormais aucune fausse instruction pour le premier "IF". Au lieu de cela, nous l'avons remplacée par le début d'un second "IF".

Vous trouverez ci-dessous des exemples d’un champ personnalisé calculé et de sa colonne personnalisée correspondante à l’aide de plusieurs instructions &quot;IF&quot; :

* Champ personnalisé calculé :

  ```
  IF({projectedCompletionDate}>{plannedCompletionDate},"Off Track",IF({plannedCompletionDate}>{projectedCompletionDate},"Off Track","On Track"))
  ```

* Colonne personnalisée calculée :

```
valueexpression=IF({"projectedCompletionDate"}>{"plannedCompletionDate"},"Off Track",IF({plannedCompletionDate}>{projectedCompletionDate},"Off Track","On Track"))
```

Dans cet exemple, la même chose a été accomplie en assemblant deux variables de critères différentes.\
Vous pouvez explorer ces options plus en détail en recréant ces exemples dans votre propre environnement.

La meilleure façon d&#39;apprendre cela est d&#39;expérimenter différents domaines et scénarios. Familiarisez-vous également avec l’explorateur d’API, qui révèle les noms des champs qui peuvent être utilisés. Pour plus d’informations sur l’explorateur d’API, voir [Explorateur d’API](../../../wf-api/general/api-explorer.md).

Pour plus d’informations sur la syntaxe Workfront des expressions de données calculées, voir [Présentation des expressions de données calculées](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).
