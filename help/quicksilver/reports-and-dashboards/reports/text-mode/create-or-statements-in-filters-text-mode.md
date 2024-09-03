---
product-area: reporting
navigation-topic: text-mode-reporting
title: Créer des instructions « OR » dans les filtres en mode texte
description: Vous pouvez inclure plusieurs instructions lorsque vous créez un filtre dans des listes et des rapports.
author: Nolan
feature: Reports and Dashboards
exl-id: be145e22-d66c-4a74-af0e-8bb0598b4d67
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '561'
ht-degree: 100%

---

# Créer des instructions « OR » dans les filtres en mode texte

Vous pouvez inclure plusieurs instructions lorsque vous créez un filtre dans des listes et des rapports.

Pour plus d’informations sur la création de filtres, reportez-vous aux articles suivants :

* [Vue d’ensemble des filtres](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [Modifier un filtre en mode texte](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)

## Opérateurs de filtre en mode texte

Pour plus d’informations sur les opérateurs de filtre Adobe Workfront dans l’interface des filtres standard, consultez [Vue d’ensemble des filtres](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

Workfront comporte deux opérateurs de filtre qui connectent chaque instruction de filtre :

* **AND** : lorsque vous joignez deux instructions de filtre par l’opérateur AND, vous indiquez que vous souhaitez que les deux instructions de filtre soient satisfaites en même temps.

  Par défaut, les instructions d’un filtre sont jointes par l’opérateur AND.

  Lors de la création d’un filtre AND dans l’interface du mode texte, vous n’avez pas besoin d’utiliser l’opérateur AND. C’est implicite.

  **Exemple :** pour filtrer les tâches dont la date d’achèvement prévue est aujourd’hui et le pourcentage terminé est inférieur à 100 %, utilisez le code suivant en mode texte :

  <pre>plannedCompletionDate=$$TODAY</pre><pre>plannedCompletionDate_Mod=eq</pre><pre>percentComplete=100</pre><pre>percentComplete_Mod=lt</pre>

* **OR** : lorsque vous joignez deux instructions de filtre par l’opérateur OR, vous indiquez que vous souhaitez que l’une ou l’autre instruction soit remplie.

  >[!TIP]
  >
  >Lorsque vous modifiez vos instructions AND en instructions OR, le nombre d’éléments de votre rapport doit augmenter.

  Lors de la création d’un filtre OR à l’aide de l’interface du mode texte, vous devez utiliser l’opérateur OR.

  **Exemple :** pour filtrer les tâches dont la date d’achèvement prévue est aujourd’hui ou dont la valeur Pourcentage terminé est inférieure à 100 %, utilisez le code suivant en mode texte :

  <pre>plannedCompletionDate=$$TODAY</pre><pre>plannedCompletionDate_Mod=eq</pre><pre>OR:1:percentComplete=100</pre><pre>OR:1:percentComplete_Mod=lt</pre>

## Syntaxe du mode texte pour les filtres OR

La syntaxe du mode texte d’un filtre OR doit contenir les éléments suivants :

* L’opérateur OR est suivi de deux-points, d’un nombre et à nouveau de deux-points au début de chaque ligne de filtre qui fait référence à l’objet dans l’instruction OR.Cela inclut la ligne qui fait référence au champ ou à l’attribut de filtre et la ligne qui fait référence au modificateur de filtre.

  Suivez ce modèle lors de la création d’un filtre OR :

  <pre><field name in camel case>=<value></pre><pre><field name in camel case>_Mod=<modifier value></pre><pre>OU:1:<field name in camel case>=<value></pre><pre>OU:1:<field name in camel case>_Mod=<modifier value></pre>

  >[!TIP]
  >
  >L’opérateur OR est sensible à la casse et il est toujours en majuscules.

  Un filtre peut contenir plusieurs instructions OR. Dans ce cas, chaque instruction OR reçoit un nombre, dans l’ordre où vous souhaitez que les instructions soient appliquées.

  **Exemple :** pour filtrer les tâches dont la date d’achèvement prévue est inférieure à 100 % OU dont la valeur Pourcentage terminé est inférieure à 100 % OU dont le statut est Nouvelle, utilisez le code suivant en mode texte :

  <pre>plannedCompletionDate=$$TODAY</pre><pre>plannedCompletionDate_Mod=eq</pre><pre>OR:1:status=NEW</pre><pre>OR:1:status_Mod=in</pre><pre>OR:2:percentComplete=100</pre><pre>OR:2:percentComplete_Mod=lt</pre>

* Le nom des champs ou des attributs que vous référencez dans un filtre doit être écrit en camel case. Pour plus d’informations sur le camel case, consultez [Vue d’ensemble de la syntaxe du mode texte](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md).
* Lorsque vous faites référence à des champs personnalisés dans un filtre OR, vous devez insérer DE: entre la syntaxe du modificateur OR et le nom du champ personnalisé. Vous devez épeler le nom du champ personnalisé tel qu’il apparaît dans l’interface de Workfront.

  **Exemple :** pour filtrer les tâches dont le statut est Nouvelle OU Pourcentage terminé inférieur à 100 % OU un champ personnalisé appelé « Type de compte » avec la valeur « Égal », utilisez le code en mode texte suivant :

  <pre>status=NEW</pre><pre>status_Mod=in</pre><pre>OR:1:percentComplete=100</pre><pre>OR:1:percentComplete_Mod=lt</pre><pre>OR:2:DE:Account Type=Capital</pre><pre>OR:2:DE:Account Type_Mod=in</pre>
