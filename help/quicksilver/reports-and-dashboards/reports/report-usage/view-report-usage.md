---
product-area: reporting
navigation-topic: report-usage
title: Afficher l’utilisation du rapport
description: Afficher l’utilisation du rapport
author: Nolan
feature: Reports and Dashboards
exl-id: 51d9067c-8c55-433e-b560-7da241ef33ae
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1001'
ht-degree: 11%

---

# Afficher l’utilisation du rapport

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: : *** DO NOT CHANGE, REMOVE, CHANGE LINK, RENAME THIS ARTICLE- IT IS LINKED TO THE PENDO GUIDE FOR THE MAIN REPORTS AREA***)</p>
-->

Pour comprendre l’utilisation intensive des rapports dans votre système, vous pouvez consulter les informations suivantes dans une liste de rapports :

* Les 10 derniers utilisateurs ayant consulté le rapport
* Affichage du nombre au cours d’une période spécifiée

  >[!NOTE]
  >
  >Adobe Workfront compte une vue par utilisateur et par jour. Si vous accédez au même rapport plusieurs fois par jour, Workfront le comptabilise comme une vue pour ce rapport. Si un autre utilisateur accède au même rapport le même jour, Workfront le comptabilise comme une nouvelle vue pour le deuxième utilisateur.

* Dernière date d&#39;affichage
* Dernière consultation par l’utilisateur
* Liste des tableaux de bord qui contiennent le rapport\
  Pour plus d’informations sur l’affichage du nom des tableaux de bord sur lesquels des rapports peuvent être ajoutés dans une liste de rapports, consultez l’article [Comprendre comment organiser des rapports sur un tableau de bord](../../../reports-and-dashboards/reports/report-usage/understand-how-organize-reports-dashboard.md).

Vous pouvez créer une vue pour une liste de rapports dans laquelle afficher ces informations.\
Vous pouvez filtrer une liste de rapports selon certains de ces champs.\
Pour plus d’informations sur les champs par lesquels vous pouvez filtrer un rapport, consultez l’article [Filtrer une liste de rapports par informations d’utilisation](#filter-a-report-list-by-usage-information).

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Modification de l’accès aux rapports, tableaux de bord et calendriers</p> <p>Modifier l’accès aux filtres, vues et groupes</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Affichage des informations d’utilisation d’un rapport dans l’affichage d’une liste de rapports

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit de Workfront, puis sur **Rapports**.

1. Dans la liste des rapports, cliquez sur le menu déroulant **Afficher** .
1. (Facultatif) Sélectionnez la vue **Report Usage** pour afficher les informations les plus courantes sur l’utilisation des rapports.\
   Ou

1. Cliquez sur **Nouvelle vue** pour créer une vue personnalisée.
1. Cliquez sur **Ajouter une colonne**.
1. Commencez à saisir l’un des champs suivants et sélectionnez-les lorsqu’ils apparaissent dans la liste sous l’objet **Report** pour les ajouter à une nouvelle colonne :

   * **10 derniers utilisateurs** : affiche les noms des 10 derniers utilisateurs qui ont consulté le rapport.
   * **Vues** : affiche le nombre de vues dans l’une des périodes suivantes :

      * **Ce Mois, Trimestre, Année**
      * **Mois dernier, Trimestre, Année**
      * **Toutes les vues** : affiche un nombre global pour toutes les vues du rapport

   * **Dernière consultation par** : affiche des informations sur l’utilisateur qui a consulté le rapport en dernier.
   * **Date de dernière consultation** : affiche la date de la dernière consultation du rapport.

1. Cliquez sur **Enregistrer la vue**.\
   Les informations d&#39;utilisation du rapport s&#39;affichent dans les colonnes que vous avez ajoutées à la vue.\
   Vous pouvez également créer un rapport pour l’objet de rapport et utiliser cette vue dans le rapport.\
   Pour plus d’informations sur la création d’un rapport, consultez l’article [Créer un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).\
   Pour créer un rapport, vous devez disposer de l’accès Modifier aux rapports au niveau d’accès .\
   Pour plus d’informations sur l’accès aux rapports, consultez l’article [Accorder l’accès aux rapports, tableaux de bord et calendriers](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

## Filtrage d’une liste de rapports par informations d’utilisation {#filter-a-report-list-by-usage-information}

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit de Workfront, puis sur **Rapports**.
1. Dans la liste des rapports, cliquez sur le menu déroulant **Filtre** .
1. Cliquez sur **Nouveau filtre**, puis sur **Ajouter une règle de filtre**.
1. Commencez à saisir l’un des champs suivants et sélectionnez-les lorsqu’ils apparaissent dans la liste sous l’objet **Report** pour les ajouter en tant que nouvelle règle de filtre :

   * **Vues** : affiche le nombre de vues dans l’une des périodes suivantes :

      * **Ce Mois, Trimestre, Année**
      * **Mois dernier, Trimestre, Année**
      * **Toutes les vues**

   * **Dernière consultation par** : affiche des informations sur l’utilisateur qui a consulté le rapport en dernier.
   * **Date de dernière consultation** : affiche la date de la dernière consultation du rapport.

1. Sélectionnez un modificateur pour votre champ, puis spécifiez une valeur lorsque vous y êtes invité.\
   ![](assets/qs-report-usage-filter-statistics-350x150.png)

1. Cliquez sur **Enregistrer le filtre**.\
   Cette option affiche la liste des rapports qui contiennent les informations d’utilisation que vous avez définies.\
   Vous pouvez également créer un rapport pour l’objet de rapport et utiliser ce filtre dans le rapport.\
   Pour plus d’informations sur la création d’un rapport, consultez l’article [Créer un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md). Pour créer un rapport, vous devez disposer de l’accès Modifier aux rapports au niveau d’accès .\
   Pour plus d’informations sur l’accès aux rapports, consultez l’article [Accorder l’accès aux rapports, tableaux de bord et calendriers](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

## Exceptions lors de l’affichage des informations sur l’utilisation des rapports

>[!IMPORTANT]
>
>Les informations sur l’utilisation du rapport sont collectées depuis mars 2018. Aucune information n’est disponible avant cette date.

Voici quelques exceptions à connaître lorsque vous utilisez des informations sur l’utilisation des rapports :

* Chaque fois qu’un rapport est affiché sur un tableau de bord ou un onglet personnalisé, il est compté comme une vue. L’utilisateur qui affiche ce rapport dans son tableau de bord est affiché en tant que Dernière vue par : nommez l’utilisateur et la date à laquelle le tableau de bord s’affiche est la date Dernière vue le .
* Workfront ne collecte pas d’informations d’utilisation pour les rapports natifs.\
  Pour plus d’informations sur les rapports natifs Workfront, reportez-vous à l’article [Utilisation des rapports natifs Adobe Workfront](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md).

* Workfront ne collecte pas d’informations d’utilisation sur les rapports distribués. Un rapport livré ne compte pas comme une vue.\
  Pour plus d’informations sur les rapports distribués, consultez l’article [Présentation de la diffusion des rapports](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

* Lorsqu’un administrateur système ou de groupe se connecte en tant qu’autre utilisateur, les vues sont comptabilisées et associées à l’administrateur système ou de groupe.
* Workfront ne collecte pas d’informations d’utilisation pour les rapports par trimestres personnalisés. Seuls les trimestres intégrés standard sont référencés dans les champs d’utilisation du rapport.
* Workfront ne collecte pas d’informations d’utilisation pour les rapports partagés et affichés publiquement. Lorsqu’un rapport public est consulté par une personne qui ne se connecte pas à Workfront, les vues de rapport ne sont pas comptabilisées.\
  Pour plus d’informations sur le partage de rapports, consultez l’article [Partager un rapport dans Adobe Workfront](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).
