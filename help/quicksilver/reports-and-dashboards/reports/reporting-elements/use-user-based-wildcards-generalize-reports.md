---
product-area: reporting
navigation-topic: reporting-elements
title: Utiliser des caractères génériques basés sur l’utilisateur ou l’utilisatrice pour généraliser les rapports
description: Vous pouvez généraliser un rapport en utilisant des caractères génériques au lieu d’informations spécifiques lors de la création de certains éléments de rapport.
author: Courtney
feature: Reports and Dashboards
exl-id: 216e2869-b4f8-4cc7-9497-a12ebe00fe49
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/S5vsXfapgDf4fjhAPV6iet9kobyEUCM14QMF-ZvvaDc
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 457
ht-degree: 100%

---

# Utiliser des caractères génériques basés sur l’utilisateur ou l’utilisatrice pour généraliser les rapports

<!-- Audited: 11/2024 -->

Vous pouvez généraliser un rapport en utilisant des caractères génériques au lieu d’informations spécifiques lors de la création de certains éléments de rapport. Par exemple, si vous voulez créer un rapport qui montre les tâches assignées à une personne spécifique, vous pouvez utiliser le nom de la personne dans le champ Affecté à du filtre. Cependant, si vous voulez créer un rapport qui montre les tâches affectées à la personne connectée, indépendamment de l’identité de cette personne, vous pouvez utiliser un caractère générique qui indique que lorsqu’une personne consulte le rapport, ce dernier affiche uniquement les informations qui concernent cette personne. De cette façon, vous créez le rapport une fois, mais comme vous utilisez un caractère générique dans le filtre, il produit des résultats différents chaque fois qu’une autre personne le lit.

Vous pouvez utiliser des caractères génériques basés sur la personne lors de la création des éléments de rapport suivants :

* Filtres
* Invites personnalisées
* Vues lors de l’ajout de règles pour les colonnes

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</strong></td> 
   <td> 
    <p>Standard</p>
    <p>Plan</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès aux filtres, vues et groupes</p> <p>Modifier l’accès aux rapports, aux tableaux de bord et aux calendriers pour la modification des éléments de rapport dans un rapport</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
    <td> <p>Gérer les autorisations d’un rapport pour modifier les éléments de rapport dans un rapport</p> <p>Gérer les autorisations d’une vue ou d’un filtre pour les modifier</p></td> 
   </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur le contenu de ce tableau, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

Vous devez créer un rapport avant de pouvoir y ajouter une variable de caractère générique.

Pour obtenir des instructions sur la création de rapports, voir [Créer un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Étapes pratiques

Pour insérer un caractère générique basé sur la personne dans un rapport, procédez comme suit :

1. Accédez à un rapport pour lequel vous souhaitez insérer un caractère générique basé sur la personne.
1. Cliquez sur **Actions de rapport**, puis sur **Modifier**.

1. Cliquez sur l’onglet **Filtres**.
1. Cliquez sur **Ajouter une règle de filtre**.
1. Saisissez le nom du champ dont vous souhaitez filtrer les données.\
   Vous devez saisir les champs qui font référence à l’objet utilisateur ou utilisatrice, ou à des informations sur les personnes.
1. Sélectionnez **Égal** dans le menu déroulant de la variable de filtre.

   >[!TIP]
   >
   >Vous devez toujours sélectionner la variable de filtre **Égal** lors de l’utilisation de caractères génériques dans Adobe Workfront.

1. Dans la zone **Commencez à saisir le nom...**, saisissez : `$$USER.ID` ou `$$USER.name` si vous voulez que le rapport affiche des informations sur la personne qui se connecte, sur la base de son nom. Vous pouvez insérer d’autres caractères génériques faisant référence au groupe, à l’équipe, à l’entreprise ou à d’autres informations relatives à la personne connectée.

   Pour une liste complète des caractères génériques basés sur la personne, voir [Vue d’ensemble des variables de filtrage des caractères génériques](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

1. Cliquez sur **Enregistrer + Fermer**.

## Informations supplémentaires

Voir aussi :

<!--outdated: * [Basic Report Creation Program](https://one.workfront.com/s/basic-report-creation-program) -->
* [Vue d’ensemble des variables de filtre de caractères génériques](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)
* [Créer ou modifier des filtres dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
* [Vue d’ensemble des filtres](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [Ajouter une invite à un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)
* [Utiliser une mise en forme conditionnelle dans les vues](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)
