---
product-area: projects
navigation-topic: issue-information
title: Utiliser « opTask » et « issue » pour faire référence à des problèmes
description: Le nom d’un problème apparaît sous la forme opTask dans la base de données Adobe Workfront. Bien que vous ayez parfois besoin d’utiliser le nom du champ de problème pour faire référence aux problèmes, la plupart du temps, vous devez utiliser le nom du champ opTask plutôt que le nom du champ lorsque vous référencez des problèmes.
author: Alina
feature: Work Management
exl-id: 91107c04-616c-49b2-aa78-10e373d11f6b
source-git-commit: 813b97ee0979e29a90293d9ddaba12a33c99f64d
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 6%

---

# Utiliser « opTask » et « issue » pour faire référence à des problèmes

Le nom d’un problème apparaît sous la forme `opTask` dans la base de données Adobe Workfront. Bien que vous ayez parfois besoin d’utiliser le nom du champ `issue` pour faire référence aux problèmes, la plupart du temps, vous devez utiliser le nom du champ `opTask` au lieu de `issue` lorsque vous référencez des problèmes.

Pour plus d’informations sur la façon dont les objets apparaissent dans la base de données Workfront, consultez l’ [Explorateur API](https://developer.adobe.com/workfront/api-explorer/).

## `opTask` filename

Utilisez le nom du champ `opTask` lorsque vous référencez des problèmes dans les contextes suivants :

* Lorsque vous créez un rapport personnalisé en mode texte pour les problèmes et que vous souhaitez référencer des problèmes dans les vues, les filtres, les regroupements ou les invites.

  Pour plus d’informations sur l’utilisation du mode texte dans un rapport, voir [Présentation du mode texte](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

<!--* When you pull information about issues using our API.  
  For more information about the Workfront API, see [Adobe Workfront API](../../../wf-api/workfront-api.md)-->

* Lorsque vous mettez à jour des champs de problème dans une feuille d’importateur de données de démarrage rapide.

  Pour plus d’informations sur l’importation de données dans Workfront à l’aide d’un démarrage rapide, voir [Importation de données dans Adobe Workfront à l’aide d’un modèle de démarrage rapide](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

## `issue` nom du champ

Utilisez le nom du champ `issue` pour référencer des problèmes dans les contextes suivants :

* Lorsque vous référencez des problèmes dans une collection à l’aide du mode texte dans un rapport.
* Lorsque vous référencez une collecte de problèmes à l’aide de l’API Workfront.

Pour plus d’informations sur la création de rapports sur les collections, voir [Référence sur les collections dans un rapport](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md).

<!--
<note type="tip">
For information about how issues appear in a collection, see the
<a href="https://developer.adobe.com/workfront/api-explorer/" target="_blank">API Explorer</a> and select the API Unsupported option from the upper-right corner of the page.
<br>(NOTE: Drafted because this might not be needed.)
</note>
-->
