---
product-area: reporting
navigation-topic: reporting-elements
title: Utiliser des caractères génériques basés sur des dates pour la généralisation des rapports
description: Vous pouvez généraliser un rapport en utilisant des caractères génériques au lieu d’informations spécifiques lors de la création de certains éléments de rapport.
author: Nolan
feature: Reports and Dashboards
exl-id: 759b0bea-729e-4206-808c-0a7216ded4ff
source-git-commit: 28dd016d5edf51807c35cb392706107a08fb95f2
workflow-type: tm+mt
source-wordcount: '687'
ht-degree: 95%

---

# Utiliser des caractères génériques basés sur des dates pour la généralisation des rapports

Vous pouvez généraliser un rapport en utilisant des caractères génériques au lieu d’informations spécifiques lors de la création de certains éléments de rapport.

Par exemple, si vous souhaitez créer un rapport qui affiche les tâches disposant d’une date de début prévue spécifique, vous pouvez utiliser le calendrier de sélection de date dans un filtre pour sélectionner une date spécifique. Cependant, si vous souhaitez créer un rapport qui affiche les tâches dont la date de début prévue est située dans une certaine période à compter de la date d’accès au rapport, vous pouvez utiliser un caractère générique indiquant que lorsqu’une personne consulte le rapport, celui-ci affiche des informations sur une période dépendant du moment de la consultation du rapport.

Par exemple, la semaine dernière, l’année passée, les deux prochaines semaines, etc. Ainsi, vous créez le rapport une seule fois, mais comme vous utilisez un caractère générique dans le filtre, il produit des résultats différents chaque fois qu’une personne le consulte, car il s’adapte en fonction du jour où celle-ci exécute le rapport.

Vous pouvez utiliser des caractères génériques basés sur des dates lors de la création des éléments de rapport suivants :

* Filtres
* Invites personnalisées
* Vues lors de l’ajout de règles pour les colonnes

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Formule Adobe Workfront*</strong></td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licence Adobe Workfront*</strong></td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurations du niveau d’accès*</strong></td> 
   <td> <p>Modifier l’accès aux filtres, vues et groupes</p> <p>Modifier l’accès aux rapports, aux tableaux de bord et aux calendriers pour la modification des éléments de rapport dans un rapport</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet</strong></td> 
   <td> <p>Gérer les autorisations d’un rapport pour modifier les éléments de rapport dans un rapport</p> <p>Gérer les autorisations d’une vue ou d’un filtre pour les modifier</p> <p>Pour plus d’informations sur les demandes d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès à des objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Conditions préalables

Vous devez créer un rapport avant de pouvoir y ajouter des variables de caractères génériques.

Pour plus d’informations sur la création d’un rapport, consultez [Créer un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Étapes pratiques

Pour insérer un caractère générique basé sur des dates dans un rapport :

1. Accédez à un rapport dans lequel vous souhaitez insérer un caractère générique basé sur des dates.
1. Cliquez sur **Actions de rapport**, puis sur **Modifier**.
1. Cliquez sur l’onglet **Filtres**.
1. Cliquez sur **Ajouter une règle de filtre**.
1. Saisissez le nom du champ dont vous souhaitez filtrer les données.\
   Vous devez saisir des champs qui référencent une date.
1. Sélectionnez **Égal** dans le menu déroulant de la variable de filtre.

   >[!TIP]
   >
   >Vous devez toujours sélectionner la variable de filtre **Égal** lors de l’utilisation de caractères génériques dans Adobe Workfront.

1. Cliquez sur le bouton bascule **Définir la date relative** , puis, dans la zone de texte qui s&#39;affiche comme type : `$$TODAY` si vous souhaitez afficher des informations sur un événement qui se produit le jour même de l&#39;exécution du rapport.

   Ou

   Saisissez `$$NOW` si vous souhaitez afficher des informations sur un événement qui se produit à la même date et à la même heure que l’exécution du rapport.

   Cette date est toujours différente, car elle change en fonction de la date à laquelle le rapport est effectivement consulté par un utilisateur ou une utilisatrice. Les informations contenues dans le rapport sont donc différentes d’un jour à l’autre.

1. (Facultatif) Si vous souhaitez afficher des informations sur une période ultérieure à la date d’exécution du rapport, saisissez `$$TODAY+1w` pour afficher les informations de la semaine prochaine, ou `$$TODAY+2m` pour afficher les informations des deux prochains mois. Vous pouvez également indiquer les trimestres, heures, jours ou années.
1. (Facultatif) Si vous souhaitez afficher des informations sur un événement survenu au cours d’une période antérieure à la date d’exécution du rapport, saisissez `$$TODAY-1w` pour afficher les informations de la semaine précédente, ou `$$TODAY-2m` pour afficher les informations des deux mois précédents. Vous pouvez également indiquer les trimestres, heures, jours ou années.

   Pour obtenir la liste complète des attributs, qualificateurs et opérateurs que vous pouvez utiliser dans les caractères génériques basés sur la date, consultez l’article [Vue d’ensemble des variables de filtre de caractères génériques](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

1. Cliquez sur **Enregistrer + Fermer**.

## Informations supplémentaires

Voir aussi :

<!--outdated: * [Basic Report Creation Program](https://one.workfront.com/s/basic-report-creation-program) -->
* [Vue d’ensemble des variables de filtre de caractères génériques](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)
* [Créer ou modifier des filtres dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
* [Ajouter une invite à un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)
* [Utiliser une mise en forme conditionnelle dans les vues](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)
