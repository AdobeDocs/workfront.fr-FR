---
product-area: reporting
navigation-topic: reporting-elements
title: Utiliser des caractères génériques basés sur l’utilisateur ou l’utilisatrice pour généraliser les rapports
description: Vous pouvez généraliser un rapport en utilisant des caractères génériques au lieu d’informations spécifiques lors de la création de certains éléments de rapport.
author: Nolan
feature: Reports and Dashboards
exl-id: 216e2869-b4f8-4cc7-9497-a12ebe00fe49
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '499'
ht-degree: 23%

---

# Utiliser des caractères génériques basés sur l’utilisateur ou l’utilisatrice pour généraliser les rapports

Vous pouvez généraliser un rapport en utilisant des caractères génériques au lieu d’informations spécifiques lors de la création de certains éléments de rapport. Par exemple, si vous souhaitez créer un rapport qui affiche les tâches affectées à un utilisateur spécifique, vous pouvez utiliser son nom dans le champ Affecté à du filtre. Cependant, si vous souhaitez créer un rapport qui affiche les tâches assignées à l’utilisateur connecté, quel que soit l’utilisateur, vous pouvez utiliser un caractère générique qui indique que lorsqu’un utilisateur consulte le rapport, il affiche uniquement les informations le concernant. Ainsi, vous générez le rapport une seule fois, mais comme vous utilisez un caractère générique dans le filtre, il produit des résultats différents chaque fois qu’une autre personne le lit.

Vous pouvez utiliser des caractères génériques basés sur l’utilisateur lors de la création des éléments de création de rapports suivants :

* Filtres
* Etapes personnalisées
* Affichages lors de l’ajout de règles pour les colonnes

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Forfait Adobe Workfront*</strong></td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licence Adobe Workfront*</strong></td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurations des niveau d’accès*</strong></td> 
   <td> <p>Modifier l’accès aux filtres, vues et groupes</p> <p>Modification de l’accès aux rapports, tableaux de bord et calendriers pour la modification des éléments de rapport dans un rapport</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet</strong></td> 
   <td> <p>Gérer les autorisations d’un rapport pour modifier les éléments de rapport dans un rapport</p> <p>Gérer les autorisations d’un affichage ou d’un filtre pour les modifier</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Conditions préalables

Vous devez créer un rapport avant d’y ajouter une variable de caractère générique.

Pour plus d&#39;informations sur la création de rapports, voir [Création d&#39;un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Étapes pratiques

Pour insérer un caractère générique (générique) basé sur l’utilisateur dans un rapport :

1. Accédez à un rapport pour lequel vous souhaitez insérer un caractère générique (générique) basé sur l’utilisateur.
1. Cliquez sur **Actions de rapport**, puis sur **Modifier**.

1. Cliquez sur l’onglet **Filtres** .
1. Cliquez sur **Ajouter une règle de filtre**.
1. Commencez à saisir le nom du champ en fonction duquel vous souhaitez filtrer les données.\
   Vous devez saisir des champs qui font référence à l’objet utilisateur ou des informations sur les utilisateurs.
1. Sélectionnez **Equal** dans le menu déroulant pour la variable de filtre.

   >[!TIP]
   >
   >Vous devez toujours sélectionner la variable de filtre **Equal** lorsque vous utilisez des caractères génériques dans Adobe Workfront.

1. Dans la zone **Commencer à saisir le nom...**, saisissez : `$$USER.ID` ou `$$USER.name` si vous souhaitez que le rapport affiche des informations sur l’utilisateur qui se connecte, en fonction de son nom. Vous pouvez insérer d’autres caractères génériques qui font référence au groupe, à l’équipe, à la société ou à d’autres informations de l’utilisateur connecté.

   Pour obtenir la liste complète des caractères génériques basés sur l’utilisateur, reportez-vous à la section [Présentation des variables de filtre générique](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

   ![](assets/user-based-wildcard-in-project-filter-350x74.png)

1. Cliquez sur **Enregistrer + Fermer**.

## Informations supplémentaires

Voir aussi :

<!--outdated: * [Basic Report Creation Program](https://one.workfront.com/s/basic-report-creation-program) -->
* [Présentation des variables de filtre générique](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)
* [Création ou modification de filtres dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
* [Présentation des filtres](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [Ajouter une invite à un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)
* [Utiliser la mise en forme conditionnelle dans les vues](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)
