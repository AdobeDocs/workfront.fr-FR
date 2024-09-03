---
product-area: reporting
navigation-topic: report-usage
title: Afficher le rapport d’utilisation
description: Afficher le rapport d’utilisation
author: Nolan
feature: Reports and Dashboards
exl-id: 51d9067c-8c55-433e-b560-7da241ef33ae
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1001'
ht-degree: 100%

---

# Afficher le rapport d’utilisation

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: : *** DO NOT CHANGE, REMOVE, CHANGE LINK, RENAME THIS ARTICLE- IT IS LINKED TO THE PENDO GUIDE FOR THE MAIN REPORTS AREA***)</p>
-->

Afin de comprendre comment les rapports sont utilisés dans votre système, vous pouvez consulter les informations suivantes dans une liste de rapports :

* Les 10 dernières personnes ayant consulté le rapport
* Nombre de vues dans un laps de temps donné

  >[!NOTE]
  >
  >Adobe Workfront compte une seule vue par personne et par jour. Si vous accédez au même rapport plusieurs fois par jour, Workfront considère qu’il ne s’agit que d’une seule vue. Si le même rapport est consulté par une autre personne au cours de la même journée, Workfront considère qu’il s’agit d’une nouvelle vue (affichée par la deuxième personne).

* Dernière date d&#39;affichage
* Dernière consultation par la personne
* Liste des tableaux de bord contenant le rapport\
  Pour plus d’informations sur l’affichage du nom des tableaux de bord sur lesquels les rapports peuvent être ajoutés dans une liste de rapports, voir l’article [Comprendre l’organisation des rapports sur un tableau de bord](../../../reports-and-dashboards/reports/report-usage/understand-how-organize-reports-dashboard.md).

Vous pouvez créer une vue pour une liste de rapports permettant d’afficher ces informations.\
Vous pouvez filtrer une liste de rapports en fonction de certains de ces champs.\
Pour plus d’informations sur les champs par lesquels vous pouvez filtrer un rapport, voir l’article [Filtrer une liste de rapports en fonction des informations d’utilisation](#filter-a-report-list-by-usage-information).

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux rapports, tableaux de bord et calendriers</p> <p>Modifier l’accès aux filtres, vues et groupes</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre équipe d’administration Workfront.

## Afficher les informations sur l’utilisation des rapports dans la vue d’une liste de rapports

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit de Workfront, puis cliquez sur **Rapports**.

1. Dans la liste des rapports, cliquez sur le menu déroulant **Affichage**.
1. (Facultatif) Sélectionnez la vue **Utilisation des rapports** pour afficher les informations les plus courantes sur l’utilisation des rapports.\
   Ou

1. Cliquez sur **Nouvel affichage** pour créer une vue personnalisée.
1. Cliquez sur **Ajouter une colonne**.
1. Commencez à saisir l’un des champs suivants et sélectionnez-le lorsqu’il apparaît dans la liste sous l’objet **Rapport** pour l’ajouter à une nouvelle colonne :

   * **10 dernières personnes** : affiche les noms des 10 dernières personnes qui ont consulté le rapport.
   * **Vues** : affiche le nombre de vues dans l’une des périodes suivantes :

      * **Mois en cours, trimestre en cours, année en cours**
      * **Mois dernier, trimestre dernier, année dernière**
      * **Toutes les vues** : affiche un décompte global de toutes les vues du rapport.

   * **Dernière consultation par** : affiche des informations sur la personne qui a consulté le rapport en dernier.
   * **Date de dernière consultation** : affiche la date à laquelle le rapport a été consulté pour la dernière fois.

1. Cliquez sur **Enregistrer la vue**.\
   Les informations relatives à l’utilisation du rapport sont affichées dans les colonnes que vous avez ajoutées à la vue.\
   Vous pouvez également créer un rapport pour l’objet du rapport et utiliser cette vue dans le rapport.\
   Pour plus d’informations sur la création d’un rapport, voir l’article [Créer un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).\
   Pour créer un rapport, vous devez avoir l’autorisation de « Modifier l’accès aux rapport » dans votre niveau d’accès.\
   Pour plus d’informations sur l’accès aux rapports, consultez l’article [Accorder l’accès aux rapports, tableaux de bord et calendriers](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

## Filtrer une liste de rapports en fonction des informations d’utilisation {#filter-a-report-list-by-usage-information}

1. Cliquez sur l’icône de **Menu principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit de Workfront, puis cliquez sur **Rapports**.
1. Dans la liste des rapports, cliquez sur le menu déroulant **Filtrer**.
1. Cliquez sur **Nouveau filtre**, puis sur **Ajouter une règle de filtre**.
1. Commencez à saisir l’un des champs suivants et sélectionnez-le lorsqu’il apparaît dans la liste sous l’objet **Rapport** pour l’ajouter en tant que nouvelle règle de filtrage :

   * **Vues** : affiche le nombre de vues au cours de l’une des périodes suivantes :

      * **Mois en cours, trimestre en cours, année en cours**
      * **Mois dernier, trimestre dernier, année dernière**
      * **Toutes les vues**

   * **Dernière consultation par** : affiche des informations sur la personne qui a consulté le rapport en dernier.
   * **Date de dernière consultation** : affiche la date à laquelle le rapport a été consulté pour la dernière fois.

1. Sélectionnez un modificateur pour votre champ, puis indiquez une valeur lorsque l’application vous y invite.\
   ![](assets/qs-report-usage-filter-statistics-350x150.png)

1. Cliquez sur **Enregistrer le filtre**.\
   Cette option permet d’afficher une liste de rapports correspondant aux informations d’utilisation que vous avez définies.\
   Vous pouvez également créer un rapport pour l’objet du rapport et utiliser ce filtre dans le rapport.\
   Pour plus d’informations sur la création d’un rapport, consultez l’article [Créer un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md). Pour créer un rapport, vous devez avoir l’autorisation de « Modifier l’accès aux rapport » dans votre niveau d’accès.\
   Pour plus d’informations sur l’accès aux rapports, consultez l’article [Accorder l’accès aux rapports, tableaux de bord et calendriers](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

## Exceptions lors de l’affichage des informations sur l’utilisation des rapports

>[!IMPORTANT]
>
>Les informations sur l’utilisation du rapport ont été collectées depuis mars 2018. Toute information antérieure à cette date n’est pas disponible.

Les exceptions suivantes sont à prendre en compte lors de l’utilisation des informations relatives à l’utilisation des rapports :

* Chaque fois qu’un rapport est affiché sur un tableau de bord ou un onglet personnalisé, il est comptabilisé comme une vue. Le nom de l’utilisateur ou de l’utilisatrice qui affiche ce rapport sur son tableau de bord est indiqué sous « Dernière consultation par » et la date à laquelle le tableau de bord a été affiché est indiquée sous « Date de dernière consulation ».
* Workfront ne collecte pas d’informations sur l’utilisation pour les rapports intégrés.\
  Pour plus d’informations sur les rapports intégrés de Workfront, consultez l’article [Utiliser les rapports intégrés d’Adobe Workfront](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md).

* Workfront ne collecte pas d’informations sur l’utilisation des rapports remis. Un rapport remis ne compte pas comme une vue.\
  Pour plus d’informations sur les rapports remis, consultez l’article [Vue d’ensemble de la remise de rapports](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

* Lorsqu’un administrateur ou une administratrice de groupes ou de systèmes se connecte en tant qu’utilisateur ou utilisatrice, les vues sont comptabilisées et associées à l’administrateur ou l’administratrice de groupes ou de système.
* Workfront ne collecte pas d’informations sur l’utilisation des rapports par trimestres personnalisés. Seuls les trimestres intégrés standard sont référencés dans les champs d’utilisation du rapport.
* Workfront ne recueille pas d’informations sur l’utilisation des rapports qui sont partagés et consultés publiquement. Lorsqu’un rapport public est consulté par une personne qui ne s’est pas connectée à Workfront, les consultations du rapport ne sont pas comptabilisées.\
  Pour plus d’informations sur le partage de rapports, consultez l’article [Partager un rapport dans Adobe Workfront](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).
