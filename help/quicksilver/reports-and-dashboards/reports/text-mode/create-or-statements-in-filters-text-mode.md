---
product-area: reporting
navigation-topic: text-mode-reporting
title: Créer des instructions "OR" dans les filtres de mode texte
description: Vous pouvez inclure plusieurs instructions lorsque vous créez un filtre dans des listes et des rapports.
author: Nolan
feature: Reports and Dashboards
exl-id: be145e22-d66c-4a74-af0e-8bb0598b4d67
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 0%

---

# Créer des instructions &quot;OR&quot; dans les filtres de mode texte

Vous pouvez inclure plusieurs instructions lorsque vous créez un filtre dans des listes et des rapports.

Pour plus d’informations sur la création de filtres, reportez-vous aux articles suivants :

* [Présentation des filtres dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [Modification d’un filtre à l’aide du mode texte](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)

## Opérateurs de filtre de mode texte

Pour plus d’informations sur les opérateurs de filtrage Adobe Workfront dans l’interface de filtrage standard, voir [Présentation des filtres dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

Workfront comporte 2 opérateurs de filtrage qui connectent chaque instruction de filtre :

* **ET**: Lorsque vous joignez une instruction de filtre 2 par l’opérateur AND, vous indiquez que vous souhaitez que les deux instructions de filtre soient satisfaites en même temps.

   Par défaut, les instructions d’un filtre sont jointes par l’opérateur AND.

   Lors de la création d’un filtre ET dans l’interface du mode texte, vous n’avez pas besoin d’utiliser l’opérateur AND. C’est supposé.

   **Exemple :** Pour filtrer les tâches dont la date d’achèvement prévue est aujourd’hui et le pourcentage d’achèvement est inférieur à 100 %, utilisez le code de mode de texte suivant :

   <pre>scheduledCompletionDate=$$TODAY</pre><pre>scheduleCompletionDate_Mod=eq</pre><pre>percentComplete=100</pre><pre>percentComplete_Mod=lt</pre>

* **OU**: Lorsque vous joignez 2 instructions de filtre par l’opérateur OU, vous indiquez que vous souhaitez que l’une ou l’autre instruction soit remplie.

   >[!TIP]
   >
   >Lorsque vous modifiez vos instructions AND en instructions OR, le nombre d’éléments de votre rapport doit augmenter.

   Lors de la création d’un filtre OU à l’aide de l’interface du mode texte, vous devez utiliser l’opérateur OU.

   **Exemple :** Pour filtrer les tâches dont la date d’achèvement prévue est aujourd’hui ou dont la valeur Pourcentage d’achèvement est inférieure à 100 %, utilisez le code de mode de texte suivant :

   <pre>scheduledCompletionDate=$$TODAY</pre><pre>scheduleCompletionDate_Mod=eq</pre><pre>OU:1:percentComplete=100</pre><pre>OU:1:percentComplete_Mod=lt</pre>

## Syntaxe du mode texte pour les filtres OU

La syntaxe du mode texte d’un filtre OU doit contenir les éléments suivants :

* L’opérateur OU est suivi d’un deux-points, d’un nombre et d’un autre deux-points au début de chaque ligne de filtre qui fait référence à l’objet dans l’instruction OU. Cela inclut la ligne qui fait référence au champ ou à l’attribut de filtre et la ligne qui fait référence au modificateur de filtre.

   Suivez ce modèle lors de la création d’un filtre OU :

   <pre><field name in camel case>=<value></pre><pre><field name in camel case>_Mod=<modifier value></pre><pre>OU:1:<field name in camel case>=<value></pre><pre>OU:1:<field name in camel case>_Mod=<modifier value></pre>

   >[!TIP]
   >
   >L’opérateur OU est sensible à la casse et il est toujours en majuscules.

   Un filtre peut contenir plusieurs instructions OR. Dans ce cas, chaque instruction OU reçoit un nombre, dans l’ordre où vous souhaitez que les instructions soient appliquées.

   **Exemple :**  Pour filtrer les tâches dont la date d’achèvement planifiée est inférieure à 100 % OU dont la valeur est inférieure à 100 % OU dont l’état est nouveau, utilisez le code de mode de texte suivant :

   <pre>scheduledCompletionDate=$$TODAY</pre><pre>scheduleCompletionDate_Mod=eq</pre><pre>OU:1:status=NEW</pre><pre>OU:1:status_Mod=in</pre><pre>OU:2:percentComplete=100</pre><pre>OU:2:percentComplete_Mod=lt</pre>

* Le nom des champs ou des attributs que vous référencez dans un filtre doit être écrit en majuscules. Pour plus d’informations sur la casse des chameaux, voir [Présentation de la syntaxe du mode texte](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md).
* Lorsque vous faites référence à des champs personnalisés dans un filtre OU, vous devez insérer DE : entre la syntaxe du modificateur OU et le nom du champ personnalisé. Vous devez épeler le nom du champ personnalisé tel qu’il apparaît dans l’interface de Workfront.

   **Exemple :** Pour filtrer les tâches dont le statut est Nouveau OU Pourcentage Terminé inférieur à 100 % OU un champ personnalisé appelé &quot;Type de compte&quot; avec la valeur &quot;Égal à&quot;, utilisez le code de mode de texte suivant :

   <pre>status=NEW</pre><pre>status_Mod=in</pre><pre>OU:1:percentComplete=100</pre><pre>OU:1:percentComplete_Mod=lt</pre><pre>OU:2:DE:Type de compte=Capital</pre><pre>OU:2:DE:Account Type_Mod=in</pre>
