---
product-area: reporting
navigation-topic: reporting-elements
title: "Éléments de reporting : filtres, vues et regroupements"
description: Les éléments principaux que chaque liste et rapport doit avoir dans Workfront sont un filtre, une vue et un groupement. Chaque élément fournit des informations différentes dans n’importe quel rapport.
author: Nolan
feature: Reports and Dashboards
exl-id: 5697905e-42c0-403b-85d4-798a1a3a2e7f
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '840'
ht-degree: 0%

---

# Éléments de reporting : filtres, vues et regroupements

<!--
<div style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>AL: Add information here about all the different kinds of FVGs: in reports, in lists, beta, etc // OR: this article should be a high-level overview of reporting elements. Then, each type of element should have:</p>
<p>- overview for Filters</p>
<p>- create a filter</p>
<p>- share a filter</p>
<p>ALL in Reporting elements but the Shared ones should be linked to Basics> Sharing; some of the articles in the Basics> Navigation> Use lists might beed to link here as well</p>
</div>
-->

Plusieurs éléments rendent possible une liste ou un rapport dans Adobe Workfront. Les éléments principaux que chaque liste et rapport doit comporter sont un filtre, une vue et un groupement. Chaque élément fournit des informations différentes dans n’importe quel rapport.

## Considérations sur les éléments de création de rapports

Tenez compte des points suivants lorsque vous utilisez des filtres, des vues et des regroupements :

* Les éléments de création de rapports fonctionnent comme les blocs de création de rapports. Elles définissent l’aspect d’un rapport ou d’une liste, ainsi que les informations contenues dans le rapport ou la liste.
* Les rapports dans Workfront sont spécifiques à un objet. Vous devez définir l’objet principal d’un rapport avant de pouvoir le créer. Par conséquent, tous les éléments de rapport sont spécifiques à un objet.
* Votre administrateur Workfront doit vous accorder l’accès aux filtres, vues et regroupements de votre niveau d’accès pour pouvoir les afficher ou les modifier dans les listes et les rapports.

  Pour plus d’informations sur l’octroi de l’accès aux filtres, aux vues et aux regroupements, voir [Accorder l’accès aux filtres, vues et regroupements](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).

* Pour pouvoir afficher ou modifier des rapports, votre administrateur Workfront doit vous accorder l’accès aux rapports, tableaux de bord et calendriers de votre niveau d’accès.

  Pour plus d’informations sur l’accès aux rapports, aux tableaux de bord et aux calendriers, voir [Accorder l’accès aux rapports, aux tableaux de bord et aux calendriers](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

* Si vous sélectionnez un filtre, une vue ou un regroupement sur un rapport ou une liste, Workfront conserve cette sélection pour les listes de cet objet même après vous être déconnecté ou avoir fermé votre navigateur. Par exemple, si vous sélectionnez une vue spécifique pour un rapport de tâche, cette sélection s’affiche pour d’autres listes de tâches, telles que la liste des tâches d’un projet.

## Filtres

Le filtre contrôle les résultats qui apparaissent dans un rapport, en réduisant généralement les résultats généraux à spécifiques. Cela fonctionne comme un passoire qui récupère uniquement les informations dont vous avez besoin et les ramène à votre rapport.

Par exemple, si vous souhaitez uniquement afficher les tâches affectées à l’utilisateur connecté, vous pouvez créer un filtre intitulé &quot;Mes tâches&quot;, définir les critères qui doivent être satisfaits pour le filtre et exécuter le rapport pour afficher uniquement les tâches affectées à l’utilisateur connecté.

Certains attributs de filtres sont les suivants :

* Par défaut, Workfront fournit plusieurs filtres pour divers objets.
* Vous pouvez personnaliser les filtres que vous possédez ou gérez.

  Pour plus d’informations sur les filtres, voir l’article [Présentation des filtres](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

![Icône Filtrer](assets/projects-list-with-filter-drop-down-highlighted-nwe.png)

## Vues

En définissant la vue d&#39;un rapport, vous définissez les informations que vous incluez dans le rapport. Comme tous les éléments de création de rapports, les vues sont basées sur un type d’objet.\
Par exemple, une vue pour un rapport de tâche peut afficher les dates d’échéance, inclure des détails financiers clés tels que le coût ou être utilisée pour afficher les affectations et les détails de la date de remise. Les vues peuvent être utilisées pour fournir divers détails sur les données du rapport.

Voici quelques attributs de vue :

* Vous pouvez utiliser une vue Workfront par défaut ou créer la vôtre.
* Vous pouvez appliquer des vues supplémentaires à partir du champ déroulant Affichage après l’exécution d’un rapport.
* Les vues supplémentaires remplacent temporairement la vue définie lors de la création du rapport. Toutefois, la vue par défaut s’affiche la prochaine fois que vous revenez au rapport.

  Pour plus d’informations sur les vues, voir l’article [Présentation des vues dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

## Regroupements

Un groupement contrôle la manière dont vous organisez les données, ce qui facilite la lecture et la compréhension. Les groupes créent des barres horizontales tout au long d’un rapport qui affichent les résultats répertoriés ensemble par des attributs communs. Vous définissez les critères permettant de regrouper les résultats de votre rapport lors de la création du groupement.

Par exemple, le regroupement d’une liste de tâches qui s’étendent sur plusieurs projets par nom de projet classe toutes les tâches respectives qui appartiennent à un seul projet sous ce nom.

Voici quelques attributs de regroupements :

* Les regroupements sont un élément de reporting obligatoire si vous souhaitez ajouter ultérieurement un graphique à votre rapport.
* Les groupements affichent une valeur d&#39;agrégat dans les résultats. &#x200B;
* Les groupes déterminent l’axe des graphiques.
* Les groupes déterminent l’identification de l’en-tête dans les rapports de matrice.\
  Pour plus d’informations sur les rapports de matrice, voir l’article [Créer un rapport de matrice](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

* Les regroupements permettent de créer l’onglet Résumé d’un rapport, fournissant les valeurs agrégées du rapport.
* Par défaut, Workfront fournit plusieurs regroupements pour différents objets.
* Vous pouvez personnaliser les regroupements que vous possédez ou gérez.

  Pour plus d’informations sur les regroupements, voir [Présentation des regroupements dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

## Autres éléments de reporting

Outre les filtres, les vues et les regroupements, vous pouvez ajouter les éléments suivants à un rapport :

* **Invite**: filtre ouvert qui peut être personnalisé et appliqué différemment chaque fois que vous exécutez un rapport.\
  Pour plus d’informations sur les invites, voir l’article [Ajouter une invite à un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

* **Graphique**: vous pouvez améliorer vos rapports en y ajoutant un graphique et en affichant les informations visuellement.\
  Pour plus d’informations sur les graphiques dans les rapports, voir l’article [Ajouter un graphique à un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).
