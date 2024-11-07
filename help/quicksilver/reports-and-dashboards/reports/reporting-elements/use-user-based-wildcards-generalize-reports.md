---
product-area: reporting
navigation-topic: reporting-elements
title: Utiliser des caractères génériques basés sur l’utilisateur ou l’utilisatrice pour généraliser les rapports
description: Vous pouvez généraliser un rapport en utilisant des caractères génériques au lieu d’informations spécifiques lors de la création de certains éléments de rapport.
author: Nolan
feature: Reports and Dashboards
exl-id: 216e2869-b4f8-4cc7-9497-a12ebe00fe49
source-git-commit: 3cee374b68b26f2a423d41101300ec8b6685fadd
workflow-type: tm+mt
source-wordcount: '456'
ht-degree: 95%

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
   <td> 
      <p>Nouveau :</p>
         <ul>
         <li><p>Standard</p></li>
         </ul>
      <p>Actuel :</p>
         <ul>
         <li><p>Plan</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurations du niveau d’accès*</strong></td> 
   <td> <p>Modifier l’accès aux filtres, vues et groupes</p> <p>Modification de l’accès aux rapports, tableaux de bord et calendriers pour la modification des éléments de rapport dans un rapport</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet</strong></td> 
   <td> <p>Gérer les autorisations d’un rapport pour modifier les éléments de rapport dans un rapport</p> <p>Gérer les autorisations d’une vue ou d’un filtre pour les modifier</p></td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations, voir [Exigences d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
