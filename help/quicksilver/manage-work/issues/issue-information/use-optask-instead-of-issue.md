---
product-area: projects
navigation-topic: issue-information
title: Utiliser « opTask » et « issue » pour faire référence à des problèmes
description: Le nom d’un problème apparaît comme opTask dans la base de données Adobe Workfront. Bien qu’il soit parfois nécessaire d’utiliser le nom du champ « issue » pour faire référence à des problèmes, la plupart du temps, vous devez utiliser le nom du champ « opTask » au lieu d’« issue » pour faire référence à des problèmes.
author: Alina
feature: Work Management
exl-id: 91107c04-616c-49b2-aa78-10e373d11f6b
source-git-commit: 813b97ee0979e29a90293d9ddaba12a33c99f64d
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 100%

---

# Utiliser « opTask » et « issue » pour faire référence à des problèmes

Le nom d’un problème apparaît comme `opTask` dans la base de données Adobe Workfront. Bien qu’il soit parfois nécessaire d’utiliser le nom de champ `issue` pour faire référence à des problèmes, la plupart du temps, vous devez utiliser le nom de champ `opTask` au lieu d’`issue` pour faire référence à des problèmes.

Pour plus d’informations sur la façon dont les objets apparaissent dans la base de données Workfront, consultez [Explorateur d’API](https://developer.adobe.com/workfront/api-explorer/).

## Nom du fichier `opTask`

Utilisez le nom du champ `opTask` lorsque vous faites référence à des problèmes dans les contextes suivants :

* Lorsque vous créez un rapport personnalisé en mode texte pour les problèmes et que vous souhaitez faire référence aux problèmes dans les vues, les filtres, les regroupements ou les invites.

  Pour plus d’informations sur l’utilisation du mode texte dans un rapport, voir [Vue d’ensemble du mode texte](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

<!--* When you pull information about issues using our API.  
  For more information about the Workfront API, see [Adobe Workfront API](../../../wf-api/workfront-api.md)-->

* Lorsque vous mettez à jour les champs de problème dans une feuille d’import de données Kickstart.

  Pour plus d’informations sur l’import de données dans Workfront à l’aide d’un Kickstart, voir [Importer des données dans Adobe Workfront à l’aide d’un modèle Kickstart](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

## Nom du champ `issue`

Utilisez le nom du champ `issue` pour faire référence à des problèmes dans les contextes suivants :

* Lorsque vous faites référence à des problèmes d’une collection en utilisant le mode texte dans un rapport.
* Lorsque vous faites référence à une collection de problèmes à l’aide de l’API Workfront.

Pour plus d’informations sur la création de rapports sur les collections, voir [Faire référence à des collections dans un rapport](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md).

<!--
<note type="tip">
For information about how issues appear in a collection, see the
<a href="https://developer.adobe.com/workfront/api-explorer/" target="_blank">API Explorer</a> and select the API Unsupported option from the upper-right corner of the page.
<br>(NOTE: Drafted because this might not be needed.)
</note>
-->
