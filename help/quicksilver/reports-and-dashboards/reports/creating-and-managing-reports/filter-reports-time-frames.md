---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Filtrer des rapports par périodes
description: Vous pouvez filtrer un rapport selon la période d’une date existant sur un objet. Vous pouvez, par exemple, filtrer un rapport d’heure pour une période donnée de la saisie des heures.
author: Nolan
feature: Reports and Dashboards
exl-id: 7dea484c-d38e-4786-85d0-f4c106cfa46f
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1059'
ht-degree: 14%

---

# Filtrer des rapports par périodes

Vous pouvez filtrer un rapport selon la période d’une date existant sur un objet. Vous pouvez, par exemple, filtrer un rapport d’heure pour une période donnée de la saisie des heures.

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

## Conditions préalables

Le rapport doit être créé avant de filtrer ses résultats.

Pour plus d&#39;informations sur la création de rapports, voir [Création d&#39;un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Filtrage d’un rapport selon la période d’une date {#filter-a-report-by-the-time-frame-of-a-date}

1. Cliquez sur l&#39;icône **Menu principal** ![](assets/main-menu-icon.png), puis sur **Reporting**.

1. Cliquez sur **Nouveau rapport**, puis sélectionnez le type de rapport de votre choix.\
   Par exemple, sélectionnez **Rapport horaire**.

1. Sélectionnez l’onglet **Filtres** .
1. Cliquez sur **Ajouter une règle de filtre**, puis sélectionnez **Date d’entrée de l’heure**.\
   ![](assets/qs-filtering-hour-report-by-timeframe-350x357.png)

1. Dans le menu déroulant suivant, sélectionnez l’une des options suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Égal à</td> 
      <td>Après avoir sélectionné ce modificateur, spécifiez la date à laquelle les heures ont été saisies.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Non égal à</td> 
      <td>Après avoir sélectionné ce modificateur, spécifiez la date à laquelle les heures ont été saisies pour exclure cette date de votre rapport. Le rapport affiche les heures enregistrées dans toutes les dates, attendues à la date que vous avez spécifiée.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Null</td> 
      <td>Sélectionnez ce modificateur pour afficher uniquement les heures où la date d’entrée est manquante.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Non null</td> 
      <td>Sélectionnez ce modificateur pour afficher uniquement les heures pour lesquelles la date d’entrée a une valeur.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Entre</td> 
      <td>Après avoir sélectionné ce modificateur, spécifiez une période au moment de la saisie des heures. Le rapport affiche les heures saisies entre les dates spécifiées.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Inférieur à</td> 
      <td>Après avoir sélectionné ce modificateur, spécifiez une date avant laquelle les heures ont été saisies. Le rapport affiche les heures saisies avant la date spécifiée, et non la date spécifiée.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Inférieur ou égal à</td> 
      <td>Après avoir sélectionné ce modificateur, spécifiez une date avant laquelle les heures ont été saisies. Le rapport affiche les heures saisies avant la date spécifiée, y compris la date spécifiée.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Supérieur à</td> 
      <td>Après avoir sélectionné ce modificateur, spécifiez une date à partir de laquelle les heures ont été saisies. Le rapport affiche les heures saisies après la date spécifiée, et non la date spécifiée.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Supérieur ou égal à</td> 
      <td> <p>Après avoir sélectionné ce modificateur, spécifiez une date à partir de laquelle les heures ont été saisies. Le rapport affiche les heures entrées après la date spécifiée, y compris la date spécifiée.</p> <p>Sélectionnez l’un des modificateurs de période intégrés, comme décrit dans la section <a href="#built-in-time-frame-modifiers" class="MCXref xref">Modificateurs de période intégrés</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Ces modificateurs sont disponibles pour n’importe quel champ de date d’un filtre ou d’une invite dans n’importe quel rapport.
1. Cliquez sur **Enregistrer + Fermer**.

## Modificateurs de période intégrés {#built-in-time-frame-modifiers}

Adobe Workfront comporte des modificateurs de période intégrés que vous pouvez utiliser sans définir de date spécifique. 

Ces modificateurs sont disponibles pour n’importe quel champ de date d’un filtre ou d’une invite dans n’importe quel rapport. 

Pour plus d’informations sur le filtrage d’un rapport selon une période associée à une date, voir  [Filtrez un rapport selon la période d&#39;une date](#filter-a-report-by-the-time-frame-of-a-date).

Par exemple, si vous créez un rapport d’heure et souhaitez afficher les heures entrées dans une période spécifique, vous pouvez choisir parmi les options de filtre de période intégrée suivantes :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Aujourd’hui</td> 
   <td>Affiche les heures où se trouve la date d’entrée aujourd’hui.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Cette semaine</td> 
   <td>Affiche les heures où la date d’entrée est une date de la semaine en cours, où la semaine commence un dimanche et se termine un samedi.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Semaine prochaine</td> 
   <td>Affiche les heures où la date d’entrée est une date de la semaine qui suit la semaine en cours, où la semaine commence un dimanche et se termine un samedi. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Semaine dernière</td> 
   <td>Affiche les heures où la date d’entrée est une date de la semaine précédant la semaine en cours, où la semaine commence un dimanche et se termine un samedi. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ce mois</td> 
   <td>Affiche les heures où la date d’entrée est une date du mois en cours.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Mois prochain</td> 
   <td>Affiche les heures où la date d’entrée est une date du mois suivant le mois en cours.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Mois dernier</td> 
   <td>Affiche les heures où la date d’entrée est une date du mois précédant le mois en cours.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ce trimestre</td> 
   <td> <p>Affiche les heures pour lesquelles la Date d’entrée est une date du trimestre en cours, où les trimestres sont définis comme suit :</p> 
    <ul> 
     <li>Premier trimestre : 1er janvier - 30 mars</li> 
     <li>Second trimestre : 1er avril - 30 juin</li> 
     <li>Troisième trimestre : 1er juillet - 30 septembre</li> 
     <li>Quatrième trimestre : 1er octobre au 31 décembre</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Trimestre prochain</td> 
   <td>Affiche les heures pour lesquelles la Date d’entrée est une date du trimestre suivant le trimestre en cours, où les trimestres sont définis ci-dessus.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Trimestre dernier</td> 
   <td> <p>Affiche les heures pour lesquelles la Date d’entrée est une date du trimestre précédent le trimestre en cours, où les trimestres sont définis ci-dessus.</p> <p>Remarque : Si votre administrateur Workfront a activé et défini des trimestres personnalisés pour votre système, les filtres intégrés pour les trimestres sont remplacés par vos informations de trimestre personnalisées. Pour plus d’informations sur l’activation des trimestres personnalisés, voir <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref">Activation des trimestres personnalisés pour les projets</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Cette année</td> 
   <td>Affiche les heures où la date d’entrée est une date de l’année en cours, où l’année en cours commence le 1er janvier et se termine le 31 décembre.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Année passée</td> 
   <td>Affiche les heures pour lesquelles la date d’entrée est une date de l’année passée, où l’année passée commence 12 mois avant la date actuelle.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Année dernière</td> 
   <td> <p>Affiche les heures pour lesquelles la date d’entrée est une date de la dernière année, où la dernière année commence le 1er janvier et se termine le 31 décembre de l’année précédant l’année en cours.</p> <p>Remarque : Il n’existe pas de période intégrée pour l’exercice. Vous pouvez créer un rapport et filtrer les informations par date à l’aide d’un modificateur personnalisé pour la période de l’année fiscale, tel qu’il est défini dans votre organisation. Si vous souhaitez choisir une période pour un exercice fiscal sur place, vous devez utiliser une invite au lieu d’un filtre. </p> </td> 
  </tr> 
 </tbody> 
</table>
