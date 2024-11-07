---
product-area: reporting
navigation-topic: reporting-elements
title: '« Éléments de création de rapports : filtres, vues et regroupements »'
description: Les éléments principaux que chaque liste et rapport doivent avoir dans Workfront sont un filtre, une vue et un regroupement. Chaque élément fournit des informations différentes dans n’importe quel rapport.
author: Nolan
feature: Reports and Dashboards
exl-id: 5697905e-42c0-403b-85d4-798a1a3a2e7f
source-git-commit: 3cee374b68b26f2a423d41101300ec8b6685fadd
workflow-type: tm+mt
source-wordcount: '838'
ht-degree: 100%

---

# Éléments de rapport : filtres, vues et regroupements

<!-- Audited: 11/2024 -->

<!--AL: Add information here about all the different kinds of FVGs: in reports, in lists, beta, etc // OR: this article should be a high-level overview of reporting elements. Then, each type of element should have:</p>
<p>- overview for Filters</p>
<p>- create a filter</p>
<p>- share a filter</p>
<p>ALL in Reporting elements but the Shared ones should be linked to Basics> Sharing; some of the articles in the Basics> Navigation> Use lists might beed to link here as well-->

Plusieurs éléments rendent possible une liste ou un rapport dans Adobe Workfront. Les éléments principaux que chaque liste et rapport doivent comporter sont un filtre, une vue et un regroupement. Chaque élément fournit des informations différentes dans n’importe quel rapport.

## Remarques sur les éléments de création de rapports

Tenez compte des points suivants lorsque vous utilisez des filtres, des vues et des regroupements :

* Les éléments de création de rapports fonctionnent comme les blocs de création de rapports. Ils définissent l’aspect d’un rapport ou d’une liste, ainsi que les informations qu’ils contiennent.
* Les rapports dans Workfront sont spécifiques à un objet. Vous devez définir l’objet principal d’un rapport avant de pouvoir le créer. Par conséquent, tous les éléments de création de rapports sont spécifiques à un objet.
* Votre équipe d’administration Workfront doit vous accorder l’accès aux filtres, vues et regroupements de votre niveau d’accès pour pouvoir les afficher ou les modifier dans les listes et les rapports.

  Pour plus d’informations sur l’octroi de l’accès aux filtres, vues et regroupements, voir [Accorder l’accès aux filtres, vues et regroupements](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).

* Pour pouvoir afficher ou modifier des rapports, votre équipe d’administration Workfront doit vous accorder l’accès aux rapports, tableaux de bord et calendriers de votre niveau d’accès.

  Pour plus d’informations sur l’accès aux rapports, tableaux de bord et calendriers, voir [Accorder l’accès aux rapports, tableaux de bord et calendriers](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

* Si vous sélectionnez un filtre, une vue ou un regroupement sur un rapport ou une liste, Workfront conserve cette sélection pour les listes de cet objet même après une déconnexion ou une fermeture du navigateur. Par exemple, si vous sélectionnez une vue spécifique pour un rapport de tâche, cette sélection s’affiche pour d’autres listes de tâches, telles que celle d’un projet.

## Filtres

Le filtre contrôle les résultats qui apparaissent dans un rapport, en réduisant généralement les résultats généraux au niveau spécifique. Cela fonctionne comme une passoire qui récupère uniquement les informations dont vous avez besoin et les ramène dans votre rapport.

Par exemple, si vous souhaitez uniquement afficher les tâches affectées à la personne connectée, vous pouvez créer un filtre intitulé « Mes tâches », définir les critères qui doivent être remplis pour le filtre et exécuter le rapport pour afficher uniquement les tâches affectées à cet utilisateur ou cette utilisatrice.

Parmi les attributs de filtres, nous retrouvons les suivants :

* Par défaut, Workfront fournit plusieurs filtres pour divers objets.
* Vous pouvez personnaliser les filtres que vous possédez ou gérez.

  Pour plus d’informations sur les filtres, voir l’article [Vue d’ensemble des filtres](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

## Vues

En définissant la vue d’un rapport, vous définissez les informations que vous incluez dans le rapport. Comme tous les éléments de création de rapports, les vues sont basées sur un type d’objet.

Par exemple, une vue pour un rapport de tâche peut afficher les dates d’échéance, inclure des détails financiers importants tels que le coût ou servir à afficher les affectations et les détails de la date de livraison. Les vues peuvent être utilisées pour fournir divers détails sur les données du rapport.

Parmi les attributs de vue, nous retrouvons les suivants :

* Vous pouvez utiliser une vue Workfront par défaut ou créer la vôtre.
* Vous pouvez appliquer des vues supplémentaires à partir du champ déroulant Vue après l’exécution d’un rapport.
* Les vues supplémentaires remplacent temporairement la vue définie lors de la création du rapport. Toutefois, la vue par défaut s’affiche la prochaine fois que vous revenez au rapport.

  Pour plus d’informations sur les vues, voir l’article [Vue d’ensemble des vues dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

## Regroupements

Un regroupement contrôle la manière dont vous organisez les données, ce qui facilite la lecture et la compréhension. Les regroupements créent des barres horizontales tout au long d’un rapport qui affichent les résultats répertoriés ensemble par des attributs communs. Vous définissez les critères permettant de regrouper les résultats de votre rapport lors de la création du regroupement.

Par exemple, le regroupement d’une liste de tâches qui s’étendent sur plusieurs projets par nom de projet classe toutes les tâches respectives qui appartiennent à un seul projet sous ce nom.

Parmi les attributs des regroupements, nous retrouvons les suivants :

* Les regroupements sont un élément de création de rapports obligatoire si vous souhaitez ajouter ultérieurement un graphique à votre rapport.
* Les regroupements affichent une valeur d’agrégat dans les résultats.
* Les groupes déterminent l’axe des graphiques.
* Les groupes déterminent l’identification de l’en-tête dans les rapports de matrice.\
  Pour plus d’informations sur les rapports de matrice, voir l’article [Créer un rapport de matrice](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

* Les regroupements permettent de créer l’onglet « Résumé » d’un rapport en fournissant les valeurs agrégées du rapport.
* Par défaut, Workfront fournit plusieurs regroupements pour différents objets.
* Vous pouvez personnaliser les regroupements que vous possédez ou gérez.

  Pour plus d’informations sur les regroupements, consultez la section [Vue d’ensemble des regroupements dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

## Autres éléments de création de rapports

Outre les filtres, les vues et les regroupements, vous pouvez ajouter les éléments suivants à un rapport :

* **Invite** : un filtre ouvert qui peut être personnalisé et appliqué différemment chaque fois que vous exécutez un rapport.\
  Pour plus d’informations sur les invites, consultez l’article [Ajouter une invite à un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

* **Graphique** : pour améliorer vos rapports, vous pouvez afficher les informations visuellement en ajoutant un graphique.\
  Pour plus d’informations sur les graphiques dans les rapports, consultez l’article [Ajouter un graphique à un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).
